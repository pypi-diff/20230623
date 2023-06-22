# Comparing `tmp/poetry_plugin_package_info-0.1.0.tar.gz` & `tmp/poetry_plugin_package_info-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_package_info-0.1.0.tar", max compression
+gzip compressed data, was "tmp.tar", last modified: Thu Jun 22 23:29:41 2023, max compression
```

## Comparing `poetry_plugin_package_info-0.1.0.tar` & `poetry_plugin_package_info-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-06-09 04:29:15.053582 poetry_plugin_package_info-0.1.0/LICENSE
--rw-r--r--   0        0        0     5857 2023-06-09 04:29:15.053582 poetry_plugin_package_info-0.1.0/README.md
--rw-r--r--   0        0        0     1131 2023-06-09 04:29:15.053582 poetry_plugin_package_info-0.1.0/poetry_plugin_package_info/__init__.py
--rw-r--r--   0        0        0    25742 2023-06-09 04:29:15.053582 poetry_plugin_package_info-0.1.0/poetry_plugin_package_info/plugin.py
--rw-r--r--   0        0        0     3616 2023-06-09 04:29:15.053582 poetry_plugin_package_info-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7508 1970-01-01 00:00:00.000000 poetry_plugin_package_info-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8017 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/README.md
+-rw-r--r--   0        0        0     1131 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/__init__.py
+-rw-r--r--   0        0        0     1170 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/formatters/__init__.py
+-rw-r--r--   0        0        0      899 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/formatters/black.py
+-rw-r--r--   0        0        0     1172 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/generators/__init__.py
+-rw-r--r--   0        0        0     8019 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/generators/git.py
+-rw-r--r--   0        0        0     3149 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/generators/project.py
+-rw-r--r--   0        0        0    31723 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/plugin.py
+-rw-r--r--   0        0        0     3786 2023-06-22 23:29:14.821989 poetry_plugin_package_info-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9706 1970-01-01 00:00:00.000000 poetry_plugin_package_info-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 poetry_plugin_package_info/package_info.py
```

### Comparing `poetry_plugin_package_info-0.1.0/LICENSE` & `poetry_plugin_package_info-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_package_info-0.1.0/poetry_plugin_package_info/__init__.py` & `poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_package_info-0.1.0/poetry_plugin_package_info/plugin.py` & `poetry_plugin_package_info-0.2.0/poetry_plugin_package_info/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,38 +20,148 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 """
+import importlib.metadata
+import io
+import tarfile
+import tempfile
 import typing
-from collections.abc import Callable
-from datetime import datetime, timezone
+import zipfile
+from abc import ABC, abstractmethod
+from datetime import datetime
 from pathlib import Path
+from types import NoneType, UnionType
 from typing import Any
 
 from cleo.commands.command import Command
-from cleo.events.console_command_event import (
-    ConsoleCommandEvent,
-)
-from cleo.events.console_events import COMMAND
+from cleo.events.console_events import TERMINATE
+from cleo.events.console_terminate_event import ConsoleTerminateEvent
 from cleo.events.event import Event
 from cleo.events.event_dispatcher import EventDispatcher
 from cleo.io.io import IO
-from git import InvalidGitRepositoryError
-from git import Repo as GitRepo  # type: ignore[attr-defined]
+from colorama import Fore
+from jinja2 import Environment, Template
 from poetry.console.application import Application
 from poetry.console.commands.build import BuildCommand
-from poetry.core.pyproject.toml import PyProjectTOML
+from poetry.core.masonry.builder import Builder
+from poetry.core.masonry.builders.sdist import SdistBuilder
+from poetry.core.masonry.builders.wheel import WheelBuilder
+from poetry.core.masonry.utils.helpers import distribution_name
 from poetry.plugins.application_plugin import ApplicationPlugin
 from tomlkit.container import Container, OutOfOrderTableProxy
 from tomlkit.items import AbstractTable, Array, InlineTable
 
 
+def type_as_python(value: type) -> str:
+    """Returns the python code for the type.
+
+    Returns the python code to represent the given type in the generated
+    .py file.
+    """
+    if issubclass(value, NoneType):
+        return "None"
+
+    builtins = (str, int, float, bool)
+    if issubclass(value, builtins):
+        return value.__name__
+
+    if len(typing.get_args(value)) > 0:
+        args = (
+            "["
+            + ", ".join([as_python(arg) for arg in typing.get_args(value)])
+            + "]"
+        )
+        return value.__name__ + args
+
+    # workaround for freezegun
+    if issubclass(value, datetime):
+        return "datetime.datetime"
+
+    return value.__name__.__module__ + "." + value.__name__
+
+
+def as_python(value: Any) -> str:
+    """Generate Python code to represent the given value."""
+    if value is None:
+        return "None"
+
+    if isinstance(value, UnionType):
+        return " | ".join([as_python(arg) for arg in typing.get_args(value)])
+
+    if isinstance(value, type):
+        return type_as_python(value)
+
+    if isinstance(value, str):
+        return f'"{value}"'
+
+    if isinstance(value, datetime):
+        return f'datetime.datetime.fromisoformat("{value.isoformat()}")'
+
+    return str(value)
+
+
+class PropertyConfig(typing.NamedTuple):
+    """Configuration for properties to be included."""
+
+    property_generator: "PropertyGenerator"
+    property_name: str
+    variable_name: str
+    metadata: dict[str, Any]
+
+
+class Property(typing.NamedTuple):
+    """A generated property."""
+
+    property_config: PropertyConfig
+    property_value: Any
+    property_type: type
+    metadata: dict[str, Any]
+
+
+class PropertyGenerator(ABC):
+    """Abstract generator of properties."""
+
+    @abstractmethod
+    def short_name(self: "PropertyGenerator") -> str:
+        """Shortname/Prefix for properties belonging to this generator."""
+
+    @abstractmethod
+    def init(
+        self: "PropertyGenerator",
+        plugin: "PackageInfoApplicationPlugin",
+    ) -> None:
+        """Initialise the PropertyGenerator for the provided plugin."""
+
+    @abstractmethod
+    def generate_property(
+        self: "PropertyGenerator",
+        property_config: PropertyConfig,
+    ) -> Property:
+        """Generate the property for the given include configuration."""
+
+
+class ContentFormatter(ABC):
+    """Abstract formatter of python file content."""
+
+    @abstractmethod
+    def init(
+        self: "ContentFormatter",
+        plugin: "PackageInfoApplicationPlugin",
+    ) -> None:
+        """Initialise the ContentFormatter for the provided plugin."""
+
+    @abstractmethod
+    def format_content(self: "ContentFormatter", content: str) -> str:
+        """Format the given python file content."""
+
+
 class MissingPropertyFromIncludeConfigItemError(Exception):
     """
     MissingPropertyFromIncludeConfigItemError.
 
     Missing required 'property' value from include item in TOML configuration.
     """
 
@@ -89,48 +199,63 @@
 
         :param include_value: The value that was specified that is unsupported
                               by the plugin.
         """
         super().__init__(f"Unsupported value in includes '{include_value}'")
 
 
-class GeneratePackageInfoCommand(Command):
+class GenerateFilePackageInfoCommand(Command):  # type: ignore[misc]
     """
-    'generate-package-info' poetry command.
+    'package-info generate-file' poetry command.
 
-    'generate-package-info' command to manually trigger the generation of the
-    package_info.py file.
+    'package-info generate-file' command to manually trigger the generation of
+     the package_info.py file.
     """
 
-    name = "generate-package-info"
+    name = "package-info generate-file"
+    description = """\
+Generates a package_info.py file that contains pyproject.toml and git \
+information.\
+"""
 
-    _plugin: "GeneratePackageInfoApplicationPlugin"
+    _plugin: "PackageInfoApplicationPlugin"
 
     def __init__(
-        self: "GeneratePackageInfoCommand",
-        plugin: "GeneratePackageInfoApplicationPlugin",
+        self: "GenerateFilePackageInfoCommand",
+        plugin: "PackageInfoApplicationPlugin",
     ) -> None:
         """
         Construct a new GeneratePackageInfoCommand.
 
         :param plugin: The plugin that registered this command.
         """
         self._plugin = plugin
         super().__init__()
 
-    def handle(self: "GeneratePackageInfoCommand") -> int:
+    def handle(self: "GenerateFilePackageInfoCommand") -> int:
         """
         Execute the command.
 
-        Called by poetry when `poetry generate-package-info` is run from the
-        command line.
+        Called by poetry when `poetry package-info generate-file` is run from
+        the command line.
 
         :return: A status code indicating success (0) or failure (not 0).
         """
-        return self._plugin.generate_package_info(self.io)
+        try:
+            return self._plugin.generate_package_info(self.io)
+        except Exception as e:
+            self.io.write_error_line(
+                f"""\
+[{Fore.BLUE}poetry-plugin-package-info{Fore.RESET}]: \
+{Fore.RED}Error encountered while generating package_info file\
+ - {e} \
+{Fore.RESET}\
+""",
+            )
+            raise
 
 
 class ContainerWrapper:
     """
     A wrapper for TOML Container.
 
     A wrapper for TOML Container that decorates it with additional helper
@@ -144,15 +269,15 @@
         """
         Construct a new instance of ContainerWrapper.
 
         :param container: The container to be wrapped.
         """
         self._container = container
 
-    def get(self: "ContainerWrapper", param: str) -> Any:  # noqa: ANN401
+    def get(self: "ContainerWrapper", param: str) -> Any:
         """
         Get the TOML section/property (if present) otherwise None.
 
         :param param: The name of the TOML section/property
         :return: None if missing, otherwise str, int or wrapped
                  OutOfOrderTableProxy or Container
         """
@@ -166,16 +291,16 @@
             return ContainerWrapper(value)
 
         return value
 
     def get_or_default(
         self: "ContainerWrapper",
         param: str,
-        default: Any,  # noqa: ANN401
-    ) -> Any:  # noqa: ANN401
+        default: Any,
+    ) -> Any:
         """
         Get the TOML section/property (if present) otherwise a default.
 
         :param param: The name of the TOML section/property
         :param default: The default value to use if section or property is
                         missing.
         :return: str, int or wrapped OutOfOrderTableProxy or Container
@@ -193,15 +318,15 @@
             return ContainerWrapper(value)
 
         return value
 
     def get_or_error(
         self: "ContainerWrapper",
         param: str,
-    ) -> Any:  # noqa: ANN401
+    ) -> Any:
         """
         Get the TOML section/property, else raise NoSuchTomlPropertyError.
 
         Get the TOML section/property (if present) otherwise raise
         NoSuchTomlPropertyError.
 
         :param param: The name of the TOML section/property
@@ -221,15 +346,15 @@
             return ContainerWrapper(value)
 
         return value
 
     def get_or_empty(
         self: "ContainerWrapper",
         param: str,
-    ) -> Any:  # noqa: ANN401
+    ) -> Any:
         """
         Get the TOML section/property, otherwise return an 'empty' value.
 
         Get the TOML section/property (if present) otherwise return an empty
         ContainerWrapper.
 
         :param param: The name of the TOML section/property
@@ -246,477 +371,582 @@
             Container | AbstractTable | OutOfOrderTableProxy,
         ):
             return ContainerWrapper(value)
 
         return value
 
 
-class GeneratePackageInfoApplicationPlugin(ApplicationPlugin):
+def get_variable_type(value: Any) -> str:
+    """Determine the type of the variable for the given value."""
+    if isinstance(value, datetime):
+        return "str"
+
+    if isinstance(value, Array):
+        return "list[str]"
+
+    if isinstance(value, bool):
+        return "bool"
+
+    return "str"
+
+
+def types_in(cls: type) -> list[type]:
+    """Recursively returns the type and any type arguments into a list."""
+    result = [cls]
+    for arg in typing.get_args(cls):
+        result += types_in(arg)
+
+    return result
+
+
+def get_imports_from_properties(properties: list[Property]) -> set[str]:
+    """Gets a list of modules that will need importing into the python file."""
+    imports = set()
+    for property_item in properties:
+        types = types_in(property_item.property_type)
+        for cls in types:
+            # Workaround for freezegun
+            if isinstance(cls, type) and issubclass(cls, datetime):
+                imports.add("datetime")
+            elif cls.__module__ != "builtins" and not isinstance(
+                cls,
+                UnionType,
+            ):
+                imports.add(cls.__module__)
+
+    return imports
+
+
+class PackageInfoApplicationPlugin(
+    ApplicationPlugin,  # type: ignore[misc]
+):
     """
     Poetry Plugin to add package_info.py file generation.
 
     Poetry Plugin to add package_info.py file generation to build command and
-    adds a generate-package-info command to poetry CLI.
+    adds a package-info generate-file command to poetry CLI.
     """
 
+    initialized: bool = False
+    application: Application
     default_src_directory: Path
-    run_before_build: bool
-    line_length: int
-    pyproject: PyProjectTOML
+    patch_build_formats: list[str]
     pyproject_file_dir: Path
+    formatter: ContentFormatter
+    template: Template
     line_separator: str
-    include: dict[str, object]
-    footer: str
-    header: str
-    package_info_file_path: Path
-    git_search_parent_directories: bool
-    git_is_bare: bool = False
-    git_repo: GitRepo | None
+    property_configs: list[PropertyConfig]
+    package_info_relative_file_path: Path
+    package_info_absolute_file_path: Path
+    plugin_config: ContainerWrapper
 
-    def __init__(self: "GeneratePackageInfoApplicationPlugin") -> None:
+    def __init__(self: "PackageInfoApplicationPlugin") -> None:
         """Creates a new instance of GeneratePackageInfoApplicationPlugin."""
         super().__init__()
 
+    def new_instance(
+        self: "PackageInfoApplicationPlugin",
+        entry_point: str,
+    ) -> Any:
+        """Create and initialise a new instance of the given entry_point."""
+        module = importlib.import_module(entry_point.split(":", 1)[0])
+        cls = getattr(module, entry_point.split(":", 1)[1])
+        instance = cls()
+        instance.init(self)
+        return instance
+
+    def write_package_info_py(
+        self: "PackageInfoApplicationPlugin",
+        package_info_file_stream: typing.TextIO,
+    ) -> None:
+        """
+        Write the contents of the package_info.py file to the given stream.
+
+        :param package_info_file_stream: The stream to write the
+                                         package_info.py file content to.
+        """
+        properties: list[Property] = []
+        for include in self.property_configs:
+            properties.append(
+                include.property_generator.generate_property(include),
+            )
+
+        imports = get_imports_from_properties(properties)
+
+        package_info_file_stream.write(
+            self.formatter.format_content(
+                self.template.render(properties=properties, imports=imports),
+            ),
+        )
+
     def generate_package_info(
-        self: "GeneratePackageInfoApplicationPlugin",
-        _: IO,
+        self: "PackageInfoApplicationPlugin",
+        out: IO,
     ) -> int:
         """
-        Generate an package_info.py file.
+        Generate a package_info.py file.
 
-        Generate an package_info.py file based on the configuration provided.
+        Generate a package_info.py file based on the configuration provided.
         :param _: The IO channel to log console messages to.
         :return: A status code indicating success(0) or failure (non-zero)
         """
-        with Path(self.package_info_file_path).open(
+        self.initialise()
+        with Path(self.package_info_absolute_file_path).open(
             "w",
         ) as package_info_file_stream:
-            if self.header:
-                self.write_header(package_info_file_stream)
+            self.write_package_info_py(package_info_file_stream)
 
-            added_no_repo_comment = False
-            added_is_bare_comment = False
-
-            for item in self.include:
-                match (
-                    item
-                    if isinstance(item, str)
-                    else item["property"]  # type: ignore[index]
-                ).split("-", maxsplit=1):
-                    case ["project", pyproject_property_name]:
-                        self.write_project_property(
-                            package_info_file_stream,
-                            pyproject_property_name,
-                            item,
-                        )
-                    case ["git", git_property_name]:
-                        if self.git_repo is None:
-                            if not added_no_repo_comment:
-                                added_no_repo_comment = True
-                                package_info_file_stream.write(
-                                    "# No git repository found, skipped git"
-                                    "properties.",
-                                )
-                                package_info_file_stream.write(
-                                    self.line_separator,
-                                )
-                            continue
-                        if self.git_is_bare and not added_is_bare_comment:
-                            added_is_bare_comment = True
-                            package_info_file_stream.write(
-                                "# Git repository is bare, skipped "
-                                "git properties relating to commits.",
-                            )
-                            package_info_file_stream.write(self.line_separator)
-                        self.handle_git_properties(
-                            package_info_file_stream,
-                            git_property_name,
-                            item,
-                        )
-                    case _:
-                        raise UnsupportedIncludeItemError(item)
-
-            if self.footer:
-                package_info_file_stream.write(self.footer)
-                package_info_file_stream.write(self.line_separator)
+        out.write_line(
+            f"""\
+[{Fore.BLUE}poetry-plugin-package-info{Fore.RESET}]: \
+Generated file {Fore.GREEN}{
+        Path(self.package_info_absolute_file_path).relative_to(self.pyproject_file_dir)
+        }{Fore.RESET}\
+""",
+        )
 
         return 0
 
-    def activate(
-        self: "GeneratePackageInfoApplicationPlugin",
-        application: Application,
-    ) -> None:
-        """
-        Activate the plugin, load configuration and register commands.
+    def parse_include_property_configs(
+        self: "PackageInfoApplicationPlugin",
+        property_configs: list[Any],
+    ) -> list[PropertyConfig]:
+        """Parse the property configurations."""
+        includes = []
+        for item in property_configs:
+            if isinstance(item, str):
+                property_generator = self.generators.get(
+                    item.split("-", maxsplit=1)[0],
+                    None,
+                )
+                property_name = item.split("-", maxsplit=1)[1]
+                if property_generator is None:
+                    # TODO: More descriptive error
+                    raise ValueError
+                variable_name = (
+                    property_generator.short_name()
+                    + "_"
+                    + property_name.replace("-", "_")
+                )
+                metadata: dict[str, Any] = {}
+                includes.append(
+                    PropertyConfig(
+                        property_generator,
+                        property_name,
+                        variable_name,
+                        metadata,
+                    ),
+                )
+            elif isinstance(item, InlineTable):
+                property_generator = self.generators.get(
+                    item["property-generator"]
+                    if "property-generator" in item
+                    else None,
+                    None,
+                )
+                property_name = (
+                    item["property-name"] if "property-name" in item else None
+                )
+                if property_name is None or property_generator is None:
+                    # Ignore invalid includes?
+                    continue
+                variable_name = (
+                    item["variable-name"]
+                    if "variable-name" in item
+                    else property_generator.short_name()
+                    + "_"
+                    + property_name.replace("-", "_")
+                )
+                metadata = item["metadata"] if "metadata" in item else {}
+                includes.append(
+                    PropertyConfig(
+                        property_generator,
+                        property_name,
+                        variable_name,
+                        metadata,
+                    ),
+                )
+            else:
+                # Ignore invalid includes?
+                pass
+        return includes
+
+    def load_generators(
+        self: "PackageInfoApplicationPlugin",
+        generators: dict[str, str],
+    ) -> dict[str, PropertyGenerator]:
+        """Load the given list of generators."""
+        return {
+            k: typing.cast(PropertyGenerator, self.new_instance(v))
+            for k, v in generators.items()
+        }
+
+    def load_formatter(
+        self: "PackageInfoApplicationPlugin",
+        formatter: str,
+    ) -> ContentFormatter:
+        """Load the formatter."""
+        return typing.cast(ContentFormatter, self.new_instance(formatter))
+
+    def initialise(self: "PackageInfoApplicationPlugin") -> None:
+        """Initialises the plugin based on pyproject.toml configuration."""
+        if self.initialized:
+            return
+
+        self.pyproject_file_dir = (
+            self.application.poetry.pyproject.file.path.parent
+        )
 
-        :param application: The poetry application.
-        :return: None
-        """
-        self.pyproject = application.poetry.pyproject
-        self.pyproject_file_dir = application.poetry.pyproject.file.path.parent
         self.default_src_directory = Path(
-            application.poetry.package.name.replace("-", "_"),
+            self.application.poetry.package.name.replace("-", "_"),
         )
-        plugin_config: ContainerWrapper = ContainerWrapper(
-            self.pyproject.data.get("tool"),
+
+        self.plugin_config: ContainerWrapper = ContainerWrapper(
+            self.application.poetry.pyproject.data.get("tool"),
         ).get_or_empty("poetry-plugin-package-info")
-        self.run_before_build = plugin_config.get_or_default(
-            "run-before-build",
-            default=False,
-        )
-        self.package_info_file_path = (
-            self.pyproject_file_dir
-            / plugin_config.get_or_default(
+
+        self.patch_build_formats = self.plugin_config.get_or_default(
+            "patch-build-formats",
+            default=[],
+        )
+        if isinstance(self.patch_build_formats, str):
+            if not self.patch_build_formats:
+                self.patch_build_formats = []
+            else:
+                self.patch_build_formats = [self.patch_build_formats]
+
+        self.package_info_relative_file_path = (
+            self.plugin_config.get_or_default(
                 "package-info-file-path",
                 f"{self.default_src_directory}/package_info.py",
             )
         )
+
+        self.package_info_absolute_file_path = (
+            self.pyproject_file_dir / self.package_info_relative_file_path
+        )
+
         # PEP-8 specifies 79 as recommended.
-        self.line_length = plugin_config.get_or_default("line-length", 79)
-        self.line_separator = plugin_config.get_or_default(
+        self.formatter = self.load_formatter(
+            self.plugin_config.get_or_default(
+                "formatter",
+                "poetry_plugin_package_info.formatters.black:BlackContentFormatter",
+            ),
+        )
+
+        env = Environment()
+        self.template = env.from_string(
+            self.plugin_config.get_or_default(
+                "template",
+                """\
+\"\"\"Auto-generated by poetry-plugin-package-info at {{\
+ now().replace(microsecond=0).isoformat() \
+ }}.\"\"\"\
+{% for import in imports %}
+import {{import}}
+{% endfor %}
+class PackageInfo:
+{% for property in properties %}\
+{{ "    " }}{{property.property_config.variable_name}}: \
+{{as_python(property.property_type)}} = \
+{{as_python(property.property_value)}}
+{% endfor %}
+""",
+            ),
+            globals={"now": datetime.now, "as_python": as_python},
+        )
+        self.line_separator = self.plugin_config.get_or_default(
             "line-separator",
             "\n",
         )
-        self.header = plugin_config.get_or_default(
-            "header",
-            '"""Auto-generated by poetry-plugin-package-info at '
-            '{file-write-time}."""',
-        )
-        self.footer = plugin_config.get_or_default("footer", "")
-        self.include = plugin_config.get_or_default(
-            "include",
-            [
-                "project-name",
-                "project-description",
-                "project-version",
-                "project-homepage",
-                "project-repository",
-                "project-documentation",
-                "project-classifiers",
-                "project-authors",
-                "project-license",
-                "git-commit-id",
-                "git-commit-author-name",
-                "git-commit-author-email",
-                "git-commit-timestamp",
-                "git-branch-name",
-                "git-branch-path",
-                "git-is-dirty",
-                "git-is-dirty-excluding-untracked",
-                "git-has-staged-changes",
-                "git-has-unstaged-changes",
-                "git-has-untracked-changes",
-            ],
-        )
-        self.git_search_parent_directories = plugin_config.get_or_default(
-            "git-search-parent-directories",
-            default=False,
+        self.generators = self.load_generators(
+            self.plugin_config.get_or_default(
+                "generators",
+                {
+                    "git": (
+                        "poetry_plugin_package_info"
+                        ".generators.git:"
+                        "GitPropertyGenerator"
+                    ),
+                    "project": (
+                        "poetry_plugin_package_info"
+                        ".generators.project:"
+                        "ProjectPropertyGenerator"
+                    ),
+                },
+            ),
         )
-        try:
-            self.git_repo = GitRepo(
-                self.pyproject_file_dir,
-                search_parent_directories=self.git_search_parent_directories,
-            )
+        self.property_configs = self.parse_include_property_configs(
+            self.plugin_config.get_or_default(
+                "properties",
+                [
+                    "project-name",
+                    "project-description",
+                    "project-version",
+                    "project-authors",
+                    "project-license",
+                    "project-classifiers",
+                    "project-documentation",
+                    "project-repository",
+                    "project-homepage",
+                    "project-maintainers",
+                    "project-keywords",
+                    "git-commit-id",
+                    "git-commit-author-name",
+                    "git-commit-author-email",
+                    "git-commit-timestamp",
+                    "git-branch-name",
+                    "git-branch-path",
+                    "git-tags",
+                    "git-is-dirty",
+                    "git-is-dirty-excluding-untracked",
+                    "git-has-staged-changes",
+                    "git-has-unstaged-changes",
+                    "git-has-untracked-changes",
+                ],
+            ),
+        )
+
+        self.initialized = True
 
-            # Check there is at least one commit in the repo.
-            try:
-                self.git_repo.head.commit  # noqa: B018
-            except ValueError as e:
-                if len(e.args) > 0 and e.args[0].startswith("Reference at"):
-                    self.git_is_bare = True
-        except InvalidGitRepositoryError:
-            self.git_repo = None
+    def activate(
+        self: "PackageInfoApplicationPlugin",
+        application: Application,
+    ) -> None:
+        """
+        Activate the plugin, load configuration and register commands.
 
+        :param application: The poetry application.
+        :return: None
+        """
+        self.application = application
         typing.cast(
             EventDispatcher,
             application.event_dispatcher,
         ).add_listener(
-            COMMAND,
-            self.on_command,
+            TERMINATE,
+            self.try_on_terminate,
         )
         application.command_loader.register_factory(
-            "generate-package-info",
-            lambda: GeneratePackageInfoCommand(self),
+            "package-info generate-file",
+            lambda: GenerateFilePackageInfoCommand(self),
         )
 
-    def on_command(
-        self: "GeneratePackageInfoApplicationPlugin",
-        event: Event,
-        event_name: str,  # noqa: ARG002
-        dispatcher: EventDispatcher,  # noqa: ARG002
+    def get_builder_types(
+        self: "PackageInfoApplicationPlugin",
+        command: BuildCommand,
+    ) -> list[type[Builder]]:
+        """Get the list of build_types set to run as part of BuildCommand."""
+        fmt = command.option("format") or "all"
+        builder = Builder(command.poetry)
+        if fmt in builder._formats:  # noqa: SLF001
+            return [builder._formats[fmt]]  # noqa: SLF001
+        if fmt == "all":
+            return list(builder._formats.values())  # noqa: SLF001
+
+        raise ValueError(f"Unsupported format: {fmt}")  # noqa: TRY003
+
+    def handle_builder_type(
+        self: "PackageInfoApplicationPlugin",
+        builder_type: type[Builder],
+        out: IO,
+    ) -> None:
+        """Handle and processing for the given builder type."""
+        format_all = "all" in self.patch_build_formats
+        if issubclass(builder_type, WheelBuilder) and (
+            builder_type.format in self.patch_build_formats or format_all
+        ):
+            builder_instance = builder_type(self.application.poetry)
+            self.update_wheel(
+                Path(builder_instance.default_target_dir)
+                / builder_instance.wheel_filename,
+                out,
+            )
+        elif issubclass(builder_type, SdistBuilder) and (
+            builder_type.format in self.patch_build_formats or format_all
+        ):
+            builder_instance = builder_type(self.application.poetry)
+            dist_name = distribution_name(
+                self.application.poetry.package.name,
+            )
+            version = builder_instance._meta.version  # noqa: SLF001
+            tar_file_name = f"{dist_name!s}-{version}.tar.gz"
+            self.update_sdist(
+                builder_instance.default_target_dir / tar_file_name,
+                out,
+            )
+        elif format_all:
+            out.write_line(
+                f"""\
+[{Fore.BLUE}poetry-plugin-package-info{Fore.RESET}]: \
+{Fore.YELLOW}Skipped unsupported distribution format \
+{builder_type.format}{Fore.RESET}\
+""",
+            )
+
+    def on_terminate(
+        self: "PackageInfoApplicationPlugin",
+        command: BuildCommand,
+        out: IO,
     ) -> None:
         """
         Event handler for when an event is triggered.
 
         Event handler for when an event is triggered on the poetry (cleo) event
         dispatcher.
         :param event: The event that was triggered.
         :param event_name: The name of the vent that was triggered.
         :param dispatcher: The dispatcher that dispatched the event.
         :return: None
         """
-        if not isinstance(event, ConsoleCommandEvent):
-            return
-        command = event.command
-        if not isinstance(command, BuildCommand):
-            return
+        self.initialise()
 
-        io = event.io
+        if len(self.patch_build_formats) == 0:
+            return
 
-        if self.run_before_build:
-            self.generate_package_info(io)
+        for builder_type in self.get_builder_types(command):
+            self.handle_builder_type(builder_type, out)
 
-    def write_git_property(
-        self: "GeneratePackageInfoApplicationPlugin",
-        package_info_file_stream: typing.TextIO,
-        item: Any,  # noqa: ignore[ANN401]
-        repo_handler: Callable[[GitRepo], Any],
+    def try_on_terminate(
+        self: "PackageInfoApplicationPlugin",
+        event: Event,
+        event_name: str,  # noqa: ARG002
+        dispatcher: EventDispatcher,  # noqa: ARG002
     ) -> None:
         """
-        Write a git property to the stream.
+        Event handler for when an event is triggered.
 
-        :param package_info_file_stream: The stream to write to.
-        :param repo_handler: Function to extract the value from a git Repo.
-        :param item: The property configuration.
+        Event handler for when an event is triggered on the poetry (cleo) event
+        dispatcher.
+        :param event: The event that was triggered.
+        :param event_name: The name of the vent that was triggered.
+        :param dispatcher: The dispatcher that dispatched the event.
         :return: None
         """
-        value = repo_handler(
-            GitRepo(self.pyproject_file_dir, search_parent_directories=True),
-        )
-        self.write_property_object(package_info_file_stream, item, value)
+        out = event.io
+        try:
+            if not isinstance(event, ConsoleTerminateEvent):
+                return
+            command = event.command
+            if not isinstance(command, BuildCommand):
+                return
+
+            self.on_terminate(command, out)
+        except Exception as e:
+            out.write_error_line(
+                f"""\
+[{Fore.BLUE}poetry-plugin-package-info{Fore.RESET}]: \
+{Fore.RED}Error encountered while patching distribution files\
+ - {e} \
+{Fore.RESET}\
+""",
+            )
+            raise
 
-    def write_project_property(
-        self: "GeneratePackageInfoApplicationPlugin",
-        package_info_file_stream: typing.TextIO,
-        param: str,
-        item: InlineTable | str,
+    def update_wheel(
+        self: "PackageInfoApplicationPlugin",
+        wheel_file: Path,
+        out: IO,
     ) -> None:
-        """
-        Write a project property to the stream.
-
-        :param package_info_file_stream: The stream to write to.
-        :param param: The name of the git property.
-        :param variable_name: The name to give the variable in the stream.
-        :return: None
-        """
-        tool_poetry_section: ContainerWrapper = ContainerWrapper(
-            self.pyproject.data.get("tool"),
-        ).get_or_error("poetry")
-        value = tool_poetry_section.get_or_default(param, None)
-        self.write_property_object(package_info_file_stream, item, value)
-
-    def write_property_object(
-        self: "GeneratePackageInfoApplicationPlugin",
-        package_info_file_stream: typing.TextIO,
-        item: str | InlineTable,
-        value: Any,  # noqa: ANN401
+        """Update the wheel distribution with the package_info.py file."""
+        with io.StringIO() as package_info_py_stream:
+            self.write_package_info_py(package_info_py_stream)
+            data = package_info_py_stream.getvalue()
+
+        out.write_line(
+            f"""\
+[{Fore.BLUE}poetry-plugin-package-info{Fore.RESET}]: Patching {Fore.GREEN}\
+{wheel_file.relative_to(self.pyproject_file_dir)!s}{Fore.RESET} with \
+{Fore.GREEN}{self.package_info_relative_file_path}{Fore.RESET}\
+""",
+        )
+        with zipfile.ZipFile(
+            str(wheel_file),
+            mode="a",
+            compression=zipfile.ZIP_DEFLATED,
+        ) as zip_file:
+            zip_file.writestr(str(self.package_info_relative_file_path), data)
+
+    def update_sdist(
+        self: "PackageInfoApplicationPlugin",
+        tar_gz_file: Path,
+        out: IO,
     ) -> None:
-        """
-        Write a property to the stream.
-
-        :param package_info_file_stream: The stream to write to.
-        :param item: The configuration item for the property.
-        :param value: The value to assign to the variable.
-        :return: None
-        """
-        variable_name: str
-        if isinstance(item, InlineTable) and "variable_name" in item:
-            variable_name = str(item["variable_name"])
-        elif isinstance(item, InlineTable) and "property" in item:
-            variable_name = str(item["property"]).replace("-", "_")
-        elif isinstance(item, InlineTable) and "property" not in item:
-            raise MissingPropertyFromIncludeConfigItemError
-        else:
-            variable_name = str(item).replace("-", "_")
-
-        if value is not None:
-            indent = 4
-            value = self.to_python(indent, value)
-            value = self.adjust_to_fit(indent, value)
-            package_info_file_stream.write(f"{variable_name} = {value}")
-            package_info_file_stream.write(self.line_separator)
-
-    def adjust_to_fit(
-        self: "GeneratePackageInfoApplicationPlugin",
-        indent: int,
-        value: Any,  # noqa: ANN401
-    ) -> Any:  # noqa: ANN401
-        """
-        Adjust any strings that would excess the line-length.
-
-        :param indent: The number of characters to indent strings.
-        :param value: The value to adjust.
-        :return: Either original value, or, a multiline string that fits
-                 within the line-length.
-        """
-        if (
-            not isinstance(value, str)
-            or not value.startswith('"')
-            or len(value) <= self.line_length - indent - 2
-        ):
-            return value
-
-        new_value = "("
-        new_value += self.line_separator
-        while len(value) > self.line_length - indent - 2:
-            if new_value:
-                new_value += " " * indent
-
-            new_value += value[: self.line_length - indent - 2]
-            new_value += '"'
-            new_value += self.line_separator
-            value = '"' + value[self.line_length - indent - 2 :]
-
-        new_value += " " * indent
-        new_value += value
-        new_value += self.line_separator
-        new_value += ")"
-        return new_value
-
-    def to_python(
-        self: "GeneratePackageInfoApplicationPlugin",
-        indent: int,
-        value: Any,  # noqa: ANN401
-    ) -> Any:  # noqa: ANN401
-        """
-        Try to turn the object into a valid python code value.
-
-        :param indent: The number of spaces to indent the value.
-        :param value: The value to convert to python code.
-        :return: A python code string, or, the original value.
-        """
-        if isinstance(value, datetime):
-            return '"' + value.isoformat() + '"'
-
-        if isinstance(value, Array):
-            new_value = "["
-            new_value += self.line_separator
-
-            for i in value:
-                new_value += " " * indent
-                new_value += self.to_python(indent, i)
-                new_value += ","
-                new_value += self.line_separator
-
-            new_value += "]"
-            return new_value
-
-        if isinstance(value, str) and not value.startswith('"'):
-            new_value = '"'
-            new_value += value
-            new_value += '"'
-            return self.adjust_to_fit(
-                indent,
-                new_value,
+        """Update the wheel distribution with the package_info.py file."""
+        with io.StringIO() as package_info_py_stream:
+            self.write_package_info_py(package_info_py_stream)
+            data = package_info_py_stream.getvalue()
+
+        out.write_line(
+            f"""\
+[{Fore.BLUE}poetry-plugin-package-info{Fore.RESET}]: Patching \
+{Fore.GREEN}{tar_gz_file.relative_to(self.pyproject_file_dir)!s}\
+{Fore.RESET} with {Fore.GREEN}{self.package_info_relative_file_path}\
+{Fore.RESET}\
+        """,
+        )
+
+        append_tar_file(
+            data.encode("utf-8"),
+            str(self.package_info_relative_file_path),
+            tar_gz_file,
+        )
+
+
+def append_tar_file(
+    data_bytes: bytes,
+    file_name: str,
+    tar_file_path: Path,
+    *,
+    replace: bool = True,
+) -> None:
+    """Append data to an tar file if not already there, or if replace=True."""
+    if not Path(tar_file_path).is_file():
+        return
+
+    compression = get_compression(tar_file_path)
+
+    with tempfile.TemporaryDirectory() as _tempdir:
+        tempdir = Path(_tempdir)
+        tmp_path = tempdir / ("tmp.tar." + compression)
+
+        with tarfile.open(tar_file_path, "r:" + compression) as tar:
+            if not replace and file_name in (member.name for member in tar):
+                return
+
+            fileobj = io.BytesIO(data_bytes)
+            tarinfo = tarfile.TarInfo(file_name)
+            tarinfo.size = len(fileobj.getvalue())
+
+            with tarfile.open(tmp_path, "w:" + compression) as tmp:
+                for member in tar:
+                    if member.name != file_name:
+                        tmp.addfile(member, tar.extractfile(member.name))
+                tmp.addfile(tarinfo, fileobj)
+
+        tmp_path.rename(tar_file_path)
+
+
+def get_compression(filename: Path) -> str:
+    """Determine the compression type of a tar file."""
+    suffixes = filename.suffixes
+    tar, compression = (s.lstrip(".") for s in suffixes[-2:])
+
+    if tar == "tgz":
+        if compression:
+            raise RuntimeError(
+                "Too much suffixes, cannot infer compression scheme from \
+                {}".format(
+                    "".join(suffixes),
+                ),
             )
+        return "gz"
 
-        return value
-
-    def write_header(
-        self: "GeneratePackageInfoApplicationPlugin",
-        package_info_file_stream: typing.TextIO,
-    ) -> None:
-        """
-        Write the header to the file.
-
-        :param package_info_file_stream: stream to write to
-        :return: None
-        """
-        package_info_file_stream.write(
-            self.header.replace(
-                "{file-write-time}",
-                datetime.now(tz=timezone.utc)
-                .replace(microsecond=0)
-                .isoformat()
-                .replace("+00:00", "Z"),
-            ),
+    if tar != "tar":
+        raise RuntimeError(  # noqa: TRY003
+            "Unable to determine tar compression",
         )
-        if not self.header.endswith(self.line_separator):
-            package_info_file_stream.write(self.line_separator)
-
-    def handle_git_properties(
-        self: "GeneratePackageInfoApplicationPlugin",
-        package_info_file_stream: typing.TextIO,
-        git_property_name: str,
-        item: Any,  # noqa: ignore[ANN401]
-    ) -> None:
-        """Handles processing of any properties related to git."""
-        git_lookup_method: Callable[[GitRepo], Any]
-        match git_property_name:
-            case "commit-id":
-                git_lookup_method = (
-                    (lambda repo: repo.head.commit.hexsha)
-                    if not self.git_is_bare
-                    else lambda _: None  # type: ignore[return-value]
-                )
-            case "commit-author-name":
-                git_lookup_method = (
-                    (lambda repo: repo.head.commit.author.name)
-                    if not self.git_is_bare
-                    else lambda _: None
-                )
-            case "commit-author-email":
-                git_lookup_method = (
-                    (lambda repo: repo.head.commit.author.email)
-                    if not self.git_is_bare
-                    else lambda _: None
-                )
-            case "commit-timestamp":
-                git_lookup_method = (
-                    (lambda repo: repo.head.commit.committed_datetime)
-                    if not self.git_is_bare
-                    else lambda _: None  # type: ignore[return-value]
-                )
-            case "is-dirty":
-
-                def git_lookup_method(repo: GitRepo) -> bool:
-                    return repo.is_dirty(untracked_files=True)
-
-            case "is-dirty-excluding-untracked":
 
-                def git_lookup_method(repo: GitRepo) -> bool:
-                    return repo.is_dirty(untracked_files=False)
-
-            case "has-staged-changes":
-                git_lookup_method = (
-                    (
-                        lambda repo: len(
-                            repo.index.diff("HEAD"),
-                        )
-                        > 0
-                    )
-                    if not self.git_is_bare
-                    else lambda _: False
-                )
-            case "has-unstaged-changes":
-
-                def git_lookup_method(repo: GitRepo) -> bool:
-                    return len(repo.index.diff(None)) > 0
-
-            case "has-untracked-changes":
-
-                def git_lookup_method(repo: GitRepo) -> bool:
-                    return len(repo.untracked_files) > 0
-
-            case "branch-name":
+    if not compression:
+        return ""
 
-                def git_lookup_method(
-                    repo: GitRepo,
-                ) -> Any:  # noqa: ANN401
-                    return repo.active_branch.name
-
-            case "branch-path":
-
-                def git_lookup_method(
-                    repo: GitRepo,
-                ) -> Any:  # noqa: ANN401
-                    return repo.active_branch.path
-
-            case _:
-                raise UnsupportedIncludeItemError(
-                    f"git-{git_property_name}",
-                )
-        self.write_git_property(
-            package_info_file_stream,
-            item,
-            git_lookup_method,
-        )
+    return compression
```

### Comparing `poetry_plugin_package_info-0.1.0/pyproject.toml` & `poetry_plugin_package_info-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-package-info"
-version = "0.1.0"
+version = "0.2.0"
 description = "Plugin for poetry that creates/updates an package_info.py file with various details about the project/package."
 authors = ["Ben Ellis <ben.ellis@softweyr.co.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "poetry_plugin_package_info"}]
 homepage = "https://github.com/bellis/poetry-plugin-package-info"
 documentation = "https://github.com/bellis/poetry-plugin-package-info"
@@ -34,29 +34,31 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 poetry = "^1.2"
 gitpython = "^3.1.31"
 mypy = "^1.3.0"
 black = "^23.3.0"
+jinja2 = "^3.1.2"
+colorama = "^0.4.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 coverage = "^7.2.7"
 ruff = "^0.0.271"
 codespell = "^2.2.4"
 freezegun = "^1.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."poetry.application.plugin"]
-generate-package-info-command = "poetry_plugin_package_info.plugin:GeneratePackageInfoApplicationPlugin"
+package-info = "poetry_plugin_package_info.plugin:PackageInfoApplicationPlugin"
 
 [tool.black]
 line-length = 79
 target-version = ['py310']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
@@ -75,32 +77,39 @@
 module = "poetry"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "git"
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+module = "freezegun"
+ignore_missing_imports = true
+
 [tool.coverage.run]
 relative_files = true
 source = ["."]
 omit = ["tests/*", "**/package_info.py"]
 
 [tool.coverage.report]
 omit = ["tests/*"]
 include_namespace_packages = "true"
 exclude_lines = [ 'pragma: no cover', 'raise NotImplementedError', 'if TYPE_CHECKING:', 'if typing.TYPE_CHECKING:', '@overload', '@typing.overload' ]
 
 [tool.ruff]
 line-length = 79
 extend-select = ['W', 'D', 'Q', 'A', 'S', 'B', 'ANN', 'RUF', 'C90', 'UP', 'I', 'N', 'SLF', 'RSE', 'RET', 'T20', 'ARG', 'C4', 'COM', 'DTZ', 'ISC', 'BLE', 'FBT', 'ICN', 'G', 'INP', 'PIE', 'PYI', 'PT', 'SIM', 'TID', 'TCH', 'INT', 'PTH', 'ERA', 'PD', 'PGH', 'PLC', 'PLE', 'PLR', 'PLW', 'TRY', 'NPY']
 pydocstyle.convention = "google"
-ignore = ['PYI014', 'PYI015', 'Q000', 'Q001', 'Q002', 'D211', 'D212']
+ignore = ['PYI014', 'PYI015', 'Q000', 'Q001', 'Q002', 'D211', 'D212', 'ANN401', 'S701']
 flake8-quotes = {inline-quotes = 'single', multiline-quotes = 'double'}
 mccabe = { max-complexity = 10 }
 isort = { known-first-party = ['poetry_plugin_package_info', 'tests'] }
 target-version = "py310"
 
 [tool.ruff.per-file-ignores]
 'tests/**/*.py' = ['S101', 'INP001', 'SLF001', 'D', 'PLR0913']
 
 [tool.codespell]
 skip = '.git,.coverage,.mypy_cache,dist,poetry.lock'
+
+[tool.poetry-plugin-package-info]
+patch-build-formats = "all"
```

### Comparing `poetry_plugin_package_info-0.1.0/PKG-INFO` & `poetry_plugin_package_info-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,190 +1,193 @@
-Metadata-Version: 2.1
-Name: poetry-plugin-package-info
-Version: 0.1.0
-Summary: Plugin for poetry that creates/updates an package_info.py file with various details about the project/package.
-Home-page: https://github.com/bellis/poetry-plugin-package-info
-License: MIT
-Author: Ben Ellis
-Author-email: ben.ellis@softweyr.co.uk
-Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Topic :: System :: Archiving :: Packaging
-Classifier: Topic :: System :: Installation/Setup
-Classifier: Topic :: System :: Software Distribution
-Requires-Dist: black (>=23.3.0,<24.0.0)
-Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: mypy (>=1.3.0,<2.0.0)
-Requires-Dist: poetry (>=1.2,<2.0)
-Project-URL: Documentation, https://github.com/bellis/poetry-plugin-package-info
-Description-Content-Type: text/markdown
-
-# Poetry Plugin: Package Info
-
-[![PyPi](https://img.shields.io/pypi/v/poetry-plugin-package-info.svg)](https://pypi.org/project/poetry-plugin-package-info/)
-[![Stable Version](https://img.shields.io/pypi/v/poetry-plugin-package-info?label=stable)](https://pypi.org/project/poetry-plugin-package-info/)
-[![Pre-release Version](https://img.shields.io/github/v/release/bellis/poetry-plugin-package-info?label=pre-release&include_prereleases&sort=semver)](https://pypi.org/project/poetry-plugin-package-info)
-[![Python Versions](https://img.shields.io/pypi/pyversions/poetry-plugin-package-info)](https://pypi.org/project/poetry-plugin-package-info)
-[![Code coverage Status](https://codecov.io/gh/bellis/poetry-plugin-package-info/branch/main/graph/badge.svg)](https://codecov.io/gh/bellis/poetry-plugin-package-info)
-[![PyTest](https://github.com/bellis/poetry-plugin-package-info/workflows/test/badge.svg)](https://github.com/bellis/poetry-plugin-package-info/actions?query=workflow%3Atest)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/BEllis/poetry-plugin-package-info/main.svg)](https://results.pre-commit.ci/latest/github/BEllis/poetry-plugin-package-info/main)
-[![Download Stats](https://img.shields.io/pypi/dm/poetry-plugin-package-info)](https://pypistats.org/packages/poetry-plugin-package-info)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-This package is a plugin that generates an `package_info.py` file with variables containing values from pyproject.toml and git.
-
-## Installation
-
-The easiest way to install the `package-info` plugin is via the `self add` command of Poetry.
-
-```bash
-poetry self add poetry-plugin-package-info
-```
-
-If you used `pipx` to install Poetry you can add the plugin via the `pipx inject` command.
-
-```bash
-pipx inject poetry poetry-plugin-package-info
-```
-
-Otherwise, if you used `pip` to install Poetry you can add the plugin packages via the `pip install` command.
-
-```bash
-pip install poetry-plugin-plugin-package-info
-```
-
-## Usage
-
-By default, the `package-info.py` file is generated only when using the `generage-package-info` command in poetry,
-
-```
-poetry generate-package-info
-```
-
-The plugin can be enabled to run before `poetry build` command by adding the `run-before-build` to the project pyproject.toml file.
-
-```toml
-[tool.poetry-plugin-package-info]
-run-before-build = true
-```
-
-The plugin can be re-configured in the pyproject.toml file, below are the options and their defaults.
-
-```toml
-[tool.poetry-plugin-package-info]
-
-# Run before poetry build command
-run-before-build = false
-
-# The path relative to the pyproject.toml file
-package-info-file-path = "package_name_in_snake_case/package_info.py"
-
-# The line length to fit python code into.
-line-length = 79
-
-# The line separate to use.
-line-separator = "\n"
-
-# Any header code to put at the top of the file.
-header = "# Auto-generated by poetry-plugin-package-info at {file-write-time}"
-
-# Any foot code to put at the bottom of the file.
-footer = ""
-
-# Search parent directories (relative to pyproject.toml) for .git
-git-search-parent-directories = false
-
-# ordered list of variables to include in the file.
-include = [
-    "project-name",
-    "project-description",
-    "project-version",
-    "project-homepage",
-    "project-repository",
-    "project-documentation",
-    "project-classifiers",
-    "project-authors",
-    "project-license",
-    "git-commit-id",
-    "git-commit-author-name",
-    "git-commit-author-email",
-    "git-commit-timestamp",
-    "git-branch-name",
-    "git-branch-path",
-    "git-has-staged-changes",
-    "git-has-unstaged-changes",
-    "git-has-changes"
-]
-```
-
-Give the defaults, below is an example `package_info.py` file.
-
-```python
-# File was auto-generated by poetry-plugin-package-info at 2023-06-05T00:35:43Z
-__project_name__ = "my-project"
-__project_description__ = "Some description."
-__project_version__ = "1.2.3"
-__project_homepage__ = "https://python-poetry.org"
-__project_repository__ = "https://github.com/python-poetry/poetry"
-__project_documentation__ = "https://python-poetry.org/docs"
-__project_classifiers__ = [
-                              "Topic :: Software Development :: Build Tools",
-                              "Topic :: Software Development :: Libraries :: Python Mo"
-                              "dules",
-                          ]
-__project_authors__ = [
-                          "Ben Ellis <ben.ellis@softweyr.co.uk>",
-                      ]
-__project_license__ = "MIT"
-__git_commit_id__ = "c4192bc5524b6905de5bcbdc0840e932c48d90ff"
-__git_commit_author_name__ = "Ben Ellis"
-__git_commit_author_email__ = "ben.ellis@softweyr.co.uk"
-__git_commit_timestamp__ = "2023-06-05T01:27:30+01:00"
-__git_branch_name__ = "main"
-__git_branch_path__ = "refs/heads/main"
-__git_has_staged_changes__ = False
-__git_has_unstaged_changes__ = False
-__git_has_changes__ = False
-```
-
-## How-to
-
-### Change variable names
-
-```toml
-[tool.poetry-plugin-package-info]
-
-includes = [
-    "project-name",
-    "project-description",
-    "git-commit-id",
-    { "property" = "git-is-dirty", "variable_name" = "clean_me" }
-]
-
-```
-
-## Related Projects
-
-* [website](https://github.com/python-poetry/website): The official Poetry website and blog
-* [poetry-plugin-export](https://github.com/python-poetry/poetry-plugin-export): Export Poetry projects/lock files to
-foreign formats like requirements.txt (Used some test code from this project)
-
+# Poetry Plugin: Package Info
+
+[![PyPi](https://img.shields.io/pypi/v/poetry-plugin-package-info.svg)](https://pypi.org/project/poetry-plugin-package-info/)
+[![Stable Version](https://img.shields.io/pypi/v/poetry-plugin-package-info?label=stable)](https://pypi.org/project/poetry-plugin-package-info/)
+[![Pre-release Version](https://img.shields.io/github/v/release/bellis/poetry-plugin-package-info?label=pre-release&include_prereleases&sort=semver)](https://pypi.org/project/poetry-plugin-package-info)
+[![Python Versions](https://img.shields.io/pypi/pyversions/poetry-plugin-package-info)](https://pypi.org/project/poetry-plugin-package-info)
+[![Code coverage Status](https://codecov.io/gh/bellis/poetry-plugin-package-info/branch/main/graph/badge.svg)](https://codecov.io/gh/bellis/poetry-plugin-package-info)
+[![PyTest](https://github.com/bellis/poetry-plugin-package-info/workflows/test/badge.svg)](https://github.com/bellis/poetry-plugin-package-info/actions?query=workflow%3Atest)
+[![Download Stats](https://img.shields.io/pypi/dm/poetry-plugin-package-info)](https://pypistats.org/packages/poetry-plugin-package-info)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+This package is a plugin that generates an `package_info.py` file with variables containing values from pyproject.toml and git.
+
+## Installation
+
+The easiest way to install the `package-info` plugin is via the `self add` command of Poetry.
+
+```bash
+poetry self add poetry-plugin-package-info
+```
+
+If you used `pipx` to install Poetry you can add the plugin via the `pipx inject` command.
+
+```bash
+pipx inject poetry poetry-plugin-package-info
+```
+
+Otherwise, if you used `pip` to install Poetry you can add the plugin packages via the `pip install` command.
+
+```bash
+pip install poetry-plugin-plugin-package-info
+```
+
+## Usage
+
+By default, the `package-info.py` file is generated only when using the `package-info generate-file` command in poetry,
+
+```
+poetry package-info generate-file
+```
+
+The plugin can be enabled to automatically patch wheel files after `poetry build` is run by adding the `patch-wheels` to the project pyproject.toml file.
+
+```toml
+[tool.poetry-plugin-package-info]
+patch-build-formats = ['wheel', 'sdist']  # or can just do ['all']
+```
+
+The plugin can be re-configured in the pyproject.toml file, below are the options and their defaults.
+
+```toml
+[tool.poetry-plugin-package-info]
+
+# Patch any .whl files produced by `poetry build`
+patch-build-formats = []
+
+# The path relative to the pyproject.toml file
+package-info-file-path = "package_name_in_snake_case/package_info.py"
+
+# Search parent directories (relative to pyproject.toml) for .git
+git-search-parent-directories = false
+
+# The formatter to format the generated package_info.py file.
+formatter = "poetry-plugin-package-info.formatters.black:BlackContentFormatter"
+
+# The generators to use to extract property values.
+generators = {
+    project = "poetry-plugin-package-info.generators.project:ProjectContentFormatter",
+    git = "poetry-plugin-package-info.generators.git:GitContentFormatter",
+}
+
+template = """\
+\"\"\"Auto-generated by poetry-plugin-package-info at {{ now().replace(microsecond=0).isoformat()  }}.\"\"\"\
+{% for import in imports %}
+import {{import}}
+{% endfor %}
+class PackageInfo:
+{% for property in properties %}\
+{{ "    " }}{{property.property_config.variable_name}}: {{as_python(property.property_type)}} = {{as_python(property.property_value)}}
+{% endfor %}
+"""
+
+# ordered list of variables to include in the file.
+properties = [
+    "project-name",
+    "project-description",
+    "project-version",
+    "project-authors",
+    "project-license",
+    "project-classifiers",
+    "project-documentation",
+    "project-repository",
+    "project-homepage",
+    "project-maintainers",
+    "project-keywords",
+    "git-commit-id",
+    "git-commit-author-name",
+    "git-commit-author-email",
+    "git-commit-timestamp",
+    "git-branch-name",
+    "git-branch-path",
+    "git-has-staged-changes",
+    "git-has-unstaged-changes",
+    "git-has-changes"
+]
+```
+
+Give the defaults, below is an example `package_info.py` file.
+
+```python
+"""Auto-generated by poetry-plugin-package-info at 2023-06-11T00:38:17."""
+import datetime
+
+
+class PackageInfo:
+    project_name: str | None = "poetry-plugin-package-info"
+    project_description: str | None = "Plugin for poetry that creates/updates an package_info.py file with various details about the project/package."
+    project_version: str | None = "0.2.0"
+    project_authors: list[str] | None = ["Ben Ellis <ben.ellis@softweyr.co.uk>"]
+    project_license: str | None = "MIT"
+    project_classifiers: list[str] | None = [
+        "Intended Audience :: Developers",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: System Administrators",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Version Control :: Git",
+        "Topic :: Software Development",
+        "Topic :: System :: Archiving :: Packaging",
+        "Topic :: System :: Installation/Setup",
+        "Topic :: System :: Software Distribution",
+        "Development Status :: 3 - Alpha",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: MIT License",
+    ]
+    project_documentation: str | None = (
+        "https://github.com/bellis/poetry-plugin-package-info"
+    )
+    project_repository: str | None = None
+    project_homepage: str | None = (
+        "https://github.com/bellis/poetry-plugin-package-info"
+    )
+    project_maintainers: list[str] | None = None
+    project_keywords: list[str] | None = None
+    git_commit_id: str | None = "b69755ca54300baaabe5f92bc99b7e101712739b"
+    git_commit_author_name: str | None = "Ben Ellis"
+    git_commit_author_email: str | None = "ben.ellis@softweyr.co.uk"
+    git_commit_timestamp: datetime.datetime | None = datetime.datetime.fromisoformat(
+        "2023-06-11T00:31:29+01:00"
+    )
+    git_branch_name: str | None = "main"
+    git_branch_path: str | None = "refs/heads/main"
+    git_is_dirty: bool | None = True
+    git_is_dirty_excluding_untracked: bool | None = True
+    git_has_staged_changes: bool | None = False
+    git_has_unstaged_changes: bool | None = True
+    git_has_untracked_changes: bool | None = False
+```
+
+## How-to
+
+### Change variable names
+
+It is possible to override the name of the generated variable by expanding the properties section to
+
+```toml
+[tool.poetry-plugin-package-info]
+
+properties = [
+    "project-name",
+    "project-description",
+    "git-commit-id",
+    { "property-generator" = "git", "property-name" = "is-dirty", "variable_name" = "clean_me" },
+    { "property-name" = "git-is-dirty", "variable_name" = "clean_me_too" }
+]
+
+```
+
+## Related Projects
+
+* [website](https://github.com/python-poetry/website): The official Poetry website and blog
+* [poetry-plugin-export](https://github.com/python-poetry/poetry-plugin-export): Export Poetry projects/lock files to
+foreign formats like requirements.txt (Used some test code from this project)
```

