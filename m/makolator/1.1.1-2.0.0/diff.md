# Comparing `tmp/makolator-1.1.1.tar.gz` & `tmp/makolator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-1.1.1.tar", max compression
+gzip compressed data, was "makolator-2.0.0.tar", max compression
```

## Comparing `makolator-1.1.1.tar` & `makolator-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-1.1.1/LICENSE
--rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-1.1.1/README.md
--rw-r--r--   0        0        0     5034 2023-06-22 23:04:42.104996 makolator-1.1.1/makolator/__init__.py
--rw-r--r--   0        0        0     8158 2023-06-23 07:21:22.575192 makolator-1.1.1/makolator/_inplace.py
--rw-r--r--   0        0        0     2066 2023-06-21 13:54:07.929256 makolator-1.1.1/makolator/config.py
--rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-1.1.1/makolator/datamodel.py
--rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-1.1.1/makolator/escape.py
--rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-1.1.1/makolator/exceptions.py
--rw-r--r--   0        0        0     7571 2023-06-22 22:49:56.884585 makolator-1.1.1/makolator/makolator.py
--rw-r--r--   0        0        0     2186 2023-06-23 07:23:04.852972 makolator-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-2.0.0/README.md
+-rw-r--r--   0        0        0     5006 2023-06-23 15:54:24.125144 makolator-2.0.0/makolator/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-23 20:30:05.045375 makolator-2.0.0/makolator/__main__.py
+-rw-r--r--   0        0        0     8305 2023-06-23 20:51:04.188011 makolator-2.0.0/makolator/_inplace.py
+-rw-r--r--   0        0        0     4189 2023-06-23 20:33:51.637383 makolator-2.0.0/makolator/cli.py
+-rw-r--r--   0        0        0     2209 2023-06-23 19:03:41.601501 makolator-2.0.0/makolator/config.py
+-rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-2.0.0/makolator/datamodel.py
+-rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-2.0.0/makolator/escape.py
+-rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-2.0.0/makolator/exceptions.py
+-rw-r--r--   0        0        0     7662 2023-06-23 20:50:50.723768 makolator-2.0.0/makolator/makolator.py
+-rw-r--r--   0        0        0     2290 2023-06-23 20:54:37.851855 makolator-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-2.0.0/PKG-INFO
```

### Comparing `makolator-1.1.1/LICENSE` & `makolator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-1.1.1/README.md` & `makolator-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `makolator-1.1.1/makolator/__init__.py` & `makolator-2.0.0/makolator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,58 +80,58 @@
 ... generated-bot: ${name} ${kwargs}
 ... </%def>\\
 ... ${datamodel}
 ... ${top('foo')}\\
 ... ${bot('foo', b=4)}\\
 ... ''') and None
 
-:any:`render` use ``sys.stdout`` by default ...
+:any:`gen` use ``sys.stdout`` by default ...
 
->>> mklt.render([Path('file.txt.mako')])
+>>> mklt.gen([Path('file.txt.mako')])
 Datamodel()
 generated-top: foo
 generated-bot: foo {'b': 4}
 
 ... or use ``dest`` for file creation - the verbose mode shares some nice information:
 
->>> mklt.render([Path('file.txt.mako')], dest=Path("file.txt"))
+>>> mklt.gen([Path('file.txt.mako')], dest=Path("file.txt"))
 'file.txt'... CREATED.
->>> mklt.render([Path('file.txt.mako')], dest=Path("file.txt"))
+>>> mklt.gen([Path('file.txt.mako')], dest=Path("file.txt"))
 'file.txt'... identical. untouched.
 
 Datamodel
 ~~~~~~~~~
 
 The :any:`Datamodel` is your container to forward data to the template.
 
 >>> mklt.datamodel.mydata = {'a': 0, 'b': 1}
 
 The output looks like that:
 
->>> mklt.render([Path('file.txt.mako')])
+>>> mklt.gen([Path('file.txt.mako')])
 Datamodel(mydata={'a': 0, 'b': 1})
 generated-top: foo
 generated-bot: foo {'b': 4}
 
 and you get notified about the changed content:
 
->>> mklt.render([Path('file.txt.mako')], dest=Path("file.txt"))
+>>> mklt.gen([Path('file.txt.mako')], dest=Path("file.txt"))
 'file.txt'... UPDATED.
 
 Differential output
 ~~~~~~~~~~~~~~~~~~~
 
 If you like it even more verbose - try:
 
 >>> mklt.config.diffout = print
 
 This will send any diff of the updated files to stdout.
 
 >>> mklt.datamodel.mydata['b'] = 2
->>> mklt.render([Path('file.txt.mako')], dest=Path("file.txt")) # doctest: +SKIP
+>>> mklt.gen([Path('file.txt.mako')], dest=Path("file.txt")) # doctest: +SKIP
 ---
 +++
 @@ -1,3 +1,3 @@
 -Datamodel(mydata={'a': 0, 'b': 1})
 +Datamodel(mydata={'a': 0, 'b': 2})
  generated-top: foo
  generated-bot: foo {'b': 4}
@@ -155,15 +155,15 @@
 ... This is handwritten text.
 ... GENERATE INPLACE BEGIN top('bar')
 ...   this line will be replaced
 ... GENERATE INPLACE END top
 ... This is handwritten text too.
 ... ''') and None
 
->>> mklt.render_inplace([Path('file.txt.mako')], Path("inplace.txt"))
+>>> mklt.inplace([Path('file.txt.mako')], Path("inplace.txt"))
 'inplace.txt'... UPDATED.
 
 >>> print(Path('inplace.txt').read_text())
 I am a regular text file.
 This is handwritten text.
 GENERATE INPLACE BEGIN top('bar')
 generated-top: bar
```

### Comparing `makolator-1.1.1/makolator/_inplace.py` & `makolator-2.0.0/makolator/_inplace.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,29 +19,31 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Inplace Generation."""
 import io
+import logging
 import re
-from logging import Logger
 from pathlib import Path
 from typing import Any, List, Optional, Tuple
 
 from attrs import define, field
 from mako.exceptions import text_error_template
 from mako.lookup import TemplateLookup
 from mako.runtime import Context
 from mako.template import Template
 
 from .exceptions import MakolatorError
 
 # pylint: disable=too-many-arguments,too-few-public-methods
 
+LOGGER = logging.getLogger("makolator")
+
 
 @define
 class InplaceInfo:
 
     """Inplace Rendering Context Information."""
 
     lineno: int
@@ -63,15 +65,14 @@
 
 
 @define
 class InplaceRenderer:
 
     """Inplace Renderer."""
 
-    logger: Logger
     template_marker: str
     inplace_marker: str
     templates: Tuple[Template, ...]
     ignore_unknown: bool
     context: dict
 
     def render(self, lookup: TemplateLookup, filepath: Path, outputfile, context: dict):
@@ -127,14 +128,15 @@
         if tplinfo:
             raise MakolatorError(f"{filepath!s}:{tplinfo.lineno} BEGIN without END.")
 
     def _process_inplace(self, filepath: Path, outputfile, context: dict, inputiter, iinfo):
         while True:
             # search for "INPLACE END <funcname>"
             lineno, line = next(inputiter)
+
             endmatch = iinfo.end.match(line)
             if endmatch:
                 # fill
                 self._fill_inplace(filepath, outputfile, iinfo, context)
                 # propagate INPLACE END tag
                 outputfile.write(line)
                 self._check_indent(filepath, lineno, iinfo, endmatch.group("indent"))
@@ -149,14 +151,15 @@
         while True:
             _, line = next(inputiter)
             # propagate
             outputfile.write(line)
             # search for "INPLACE END"
             endmatch = tend.match(line)
             if endmatch:
+                LOGGER.info("Template '%s:%d'", outputfile, tplinfo.lineno)
                 templates.append(Template("".join(tplinfo.lines), lookup=lookup))
                 break
             if line.startswith(pre):
                 line = line[prelen:]
             tplinfo.lines.append(line)
 
     def _start_inplace(
@@ -171,23 +174,24 @@
             return InplaceInfo(lineno, indent, funcname, args, func, end)
         if not self.ignore_unknown:
             raise MakolatorError(f"{filepath!s}:{lineno} Function '{funcname}' is not found in templates.")
         return None
 
     def _check_indent(self, filepath: Path, lineno: int, inplace: InplaceInfo, endindent):
         if endindent != inplace.indent:
-            self.logger.warning(
+            LOGGER.warning(
                 "%s:%d Indent of END tag %r does not match indent of BEGIN tag %r.",
                 filepath,
                 lineno,
                 endindent,
                 inplace.indent,
             )
 
     def _fill_inplace(self, filepath: Path, outputfile, inplace: InplaceInfo, context: dict):
+        LOGGER.info("Inplace '%s:%d'", filepath, inplace.lineno)
         # determine args, kwargs
         try:
             # pylint: disable=eval-used
             args, kwargs = eval(f"_extract({inplace.args})", {"_extract": _extract})
         except Exception as exc:
             raise MakolatorError(
                 f"{filepath!s}:{inplace.lineno} Function invocation failed. "
```

### Comparing `makolator-1.1.1/makolator/config.py` & `makolator-2.0.0/makolator/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,8 +55,13 @@
     template_marker: str = "MAKO TEMPLATE"
     """Search marker for template code within output file."""
 
     inplace_marker: str = "GENERATE INPLACE"
     """Search marker for output code within output file."""
 
     cache_path: Optional[Path] = None
-    """Cache Directory."""
+    """
+    Cache Directory.
+
+    Used to store converted templates. Use if you have many and/or large templates.
+    Speeds up rendering. Share it between runs.
+    """
```

### Comparing `makolator-1.1.1/makolator/datamodel.py` & `makolator-2.0.0/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-1.1.1/makolator/escape.py` & `makolator-2.0.0/makolator/escape.py`

 * *Files identical despite different names*

### Comparing `makolator-1.1.1/makolator/makolator.py` & `makolator-2.0.0/makolator/makolator.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from uniquer import uniquelist
 
 from ._inplace import InplaceRenderer
 from .config import Config
 from .datamodel import Datamodel
 from .exceptions import MakolatorError
 
-LOGGER = logging.getLogger(__name__)
+LOGGER = logging.getLogger("makolator")
 
 
 @define
 class Makolator:
     """
     The Makolator.
 
@@ -84,44 +84,46 @@
             try:
                 yield file
             finally:
                 file.close()
                 if self.config.verbose:
                     print(f"'{filepath!s}'... {file.state.value}")
 
-    def render(self, template_filepaths: List[Path], dest: Optional[Path] = None, context: Optional[dict] = None):
+    def gen(self, template_filepaths: List[Path], dest: Optional[Path] = None, context: Optional[dict] = None):
         """
         Render template file.
 
         Args:
             template_filepaths: Templates.
 
         Keyword Args:
             dest: Output File.
             context: Key-Value Pairs pairs forwarded to the template.
         """
-        LOGGER.debug("render(%r, %r)", [str(filepath) for filepath in template_filepaths], dest)
+        LOGGER.debug("gen(%r, %r)", [str(filepath) for filepath in template_filepaths], dest)
         tplfilepaths, lookup = self._create_template_lookup(
             template_filepaths, self.config.template_paths, required=True
         )
         templates = self._create_templates(tplfilepaths, lookup)
         context = context or {}
         if dest is None:
             self._render(next(templates), sys.stdout, None, context)
         else:
             # Mako takes care about proper newline handling. Therefore we deactivate
             # the universal newline mode, by setting newline="".
             with self.open_outputfile(dest, newline="") as output:
-                self._render(next(templates), output, dest, context)
+                template = next(templates)  # Load template
+                LOGGER.info("Generate '%s'", dest)
+                self._render(template, output, dest, context)
 
     def _render(self, template: Template, output, dest: Optional[Path], context: dict):
         context = Context(output, **self._get_render_context(dest, context))
         template.render_context(context)
 
-    def render_inplace(
+    def inplace(
         self,
         template_filepaths: List[Path],
         filepath: Path,
         context: Optional[dict] = None,
         ignore_unknown: bool = False,
     ):
         """
@@ -131,28 +133,27 @@
             template_filepaths: Templates.
             dest: File to update.
 
         Keyword Args:
             context: Key-Value Pairs pairs forwarded to the template.
             ignore_unknown: Ignore unknown inplace markers, instead of raising an error.
         """
-        LOGGER.debug("render_inplace(%r, %r)", [str(filepath) for filepath in template_filepaths], filepath)
+        LOGGER.debug("inplace(%r, %r)", [str(filepath) for filepath in template_filepaths], filepath)
         tplfilepaths, lookup = self._create_template_lookup(template_filepaths, self.config.template_paths)
         templates = tuple(self._create_templates(tplfilepaths, lookup))
         config = self.config
         context = context or {}
-        inplace = InplaceRenderer(
-            LOGGER, config.template_marker, config.inplace_marker, templates, ignore_unknown, context
-        )
+        inplace = InplaceRenderer(config.template_marker, config.inplace_marker, templates, ignore_unknown, context)
         with self.open_outputfile(filepath, existing=Existing.KEEP_TIMESTAMP, newline="") as outputfile:
             context = self._get_render_context(filepath, context or {})
             inplace.render(lookup, filepath, outputfile, context)
 
     def _create_templates(self, tplfilepaths: List[Path], lookup: TemplateLookup) -> Generator[Template, None, None]:
         for tplfilepath in tplfilepaths:
+            LOGGER.info("Template '%s'", tplfilepath)
             yield lookup.get_template(tplfilepath.name)
 
     def _create_template_lookup(
         self, template_filepaths: List[Path], searchpaths: List[Path], required: bool = False
     ) -> Tuple[List[Path], TemplateLookup]:
         cache_path = self.cache_path
         tplfilepaths = list(self._find_files(template_filepaths, searchpaths, required=required))
@@ -196,16 +197,16 @@
         if not found and required:
             raise MakolatorError(f"None of the templates {_humanify(filepaths)} found at {_humanify(searchpaths)}.")
 
     def _get_render_context(self, output_filepath: Optional[Path], context: dict) -> dict:
         result = {
             "datamodel": self.datamodel,
             "output_filepath": output_filepath,
-            "render": self.render,
-            "render_inplace": self.render_inplace,
+            "gen": self.gen,
+            "inplace": self.inplace,
         }
         result.update(context)
         return result
 
 
 def _humanify(iterable):
     if iterable:
```

### Comparing `makolator-1.1.1/pyproject.toml` & `makolator-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "1.1.1"
+version = "2.0.0"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -16,15 +16,16 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/nbiotcloud/makolator"
 "Documentation" = "https://makolator.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/nbiotcloud/makolator/issues"
 
-#[tool.poetry.scripts]
+[tool.poetry.scripts]
+makolator = "makolator.cli:main"
 
 
 [tool.poetry.dependencies]
 python = '^3.7.2'
 attrs = "^23.1.0"
 outputfile = "^0.2.0"
 mako = "^1.2.4"
@@ -100,14 +101,15 @@
     LANGUAGE=en_US
 
 commands =
     poetry install --with=test --with=doc
     poetry run black .
     poetry run isort .
     poetry run coverage run --source=makolator --branch -m pytest --doctest-glob=docs/*.rst --doctest-modules --ignore-glob=tests/testdata* --ignore=docs/conf.py --log-level=DEBUG -vv --junitxml=report.xml
+    poetry run coverage run -a --source=makolator --branch -m makolator
     poetry run coverage report
     poetry run coverage html
     poetry run coverage xml
     poetry run pylint makolator tests
     poetry run mypy makolator
     poetry run make html -C docs
 """
```

### Comparing `makolator-1.1.1/PKG-INFO` & `makolator-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 1.1.1
+Version: 2.0.0
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

