# Comparing `tmp/glean-cli-0.5.6.tar.gz` & `tmp/glean-cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.5.6.tar", last modified: Mon Apr 17 15:30:26 2023, max compression
+gzip compressed data, was "glean-cli-0.6.0.tar", last modified: Fri Jun 23 20:04:33 2023, max compression
```

## Comparing `glean-cli-0.5.6.tar` & `glean-cli-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.938509 glean-cli-0.5.6/
--rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 glean-cli-0.5.6/LICENSE
--rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-04-17 15:30:26.938568 glean-cli-0.5.6/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      832 2023-01-19 16:41:15.000000 glean-cli-0.5.6/README.md
--rw-r--r--   0 anixon     (501) staff       (20)      103 2022-12-17 00:47:55.000000 glean-cli-0.5.6/pyproject.toml
--rw-r--r--   0 anixon     (501) staff       (20)      793 2023-04-17 15:30:26.938846 glean-cli-0.5.6/setup.cfg
--rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 glean-cli-0.5.6/setup.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.934561 glean-cli-0.5.6/src/
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.936367 glean-cli-0.5.6/src/glean/
--rw-r--r--   0 anixon     (501) staff       (20)       18 2023-04-17 15:29:18.000000 glean-cli-0.5.6/src/glean/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)    19217 2023-04-11 21:15:13.000000 glean-cli-0.5.6/src/glean/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1598 2022-12-17 00:47:55.000000 glean-cli-0.5.6/src/glean/credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     2048 2022-12-17 00:47:55.000000 glean-cli-0.5.6/src/glean/filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)    12288 2023-04-17 15:29:18.000000 glean-cli-0.5.6/src/glean/glean_api.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.937120 glean-cli-0.5.6/src/glean/utils/
--rw-r--r--   0 anixon     (501) staff       (20)        0 2022-12-17 00:47:55.000000 glean-cli-0.5.6/src/glean/utils/__init__.py
--rw-r--r--   0 anixon     (501) staff       (20)      509 2023-01-03 16:54:54.000000 glean-cli-0.5.6/src/glean/utils/cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1583 2023-01-19 16:41:15.000000 glean-cli-0.5.6/src/glean/utils/grn.py
--rw-r--r--   0 anixon     (501) staff       (20)     1035 2023-01-19 16:41:15.000000 glean-cli-0.5.6/src/glean/utils/validate_config.py
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.937904 glean-cli-0.5.6/src/glean_cli.egg-info/
--rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 anixon     (501) staff       (20)      588 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anixon     (501) staff       (20)        1 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anixon     (501) staff       (20)       41 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 anixon     (501) staff       (20)       84 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 anixon     (501) staff       (20)        6 2023-04-17 15:30:26.000000 glean-cli-0.5.6/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-04-17 15:30:26.938408 glean-cli-0.5.6/tests/
--rw-r--r--   0 anixon     (501) staff       (20)      309 2022-12-17 00:47:55.000000 glean-cli-0.5.6/tests/test_cli.py
--rw-r--r--   0 anixon     (501) staff       (20)     1652 2022-12-17 00:47:55.000000 glean-cli-0.5.6/tests/test_credentials.py
--rw-r--r--   0 anixon     (501) staff       (20)     1715 2023-01-19 16:41:15.000000 glean-cli-0.5.6/tests/test_filesystem.py
--rw-r--r--   0 anixon     (501) staff       (20)      666 2022-12-17 00:47:55.000000 glean-cli-0.5.6/tests/test_glean_api.py
+drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.280097 glean-cli-0.6.0/
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)    11357 2023-01-11 18:02:06.000000 glean-cli-0.6.0/LICENSE
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1283 2023-06-23 20:04:33.280162 glean-cli-0.6.0/PKG-INFO
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      832 2023-06-23 20:03:49.000000 glean-cli-0.6.0/README.md
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      103 2023-01-11 18:02:06.000000 glean-cli-0.6.0/pyproject.toml
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      814 2023-06-23 20:04:33.280447 glean-cli-0.6.0/setup.cfg
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)       38 2023-01-11 18:02:06.000000 glean-cli-0.6.0/setup.py
+drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.275496 glean-cli-0.6.0/src/
+drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.277548 glean-cli-0.6.0/src/glean/
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)       18 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/__init__.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)    28983 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/cli.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1598 2023-01-11 18:02:06.000000 glean-cli-0.6.0/src/glean/credentials.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     3904 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/filesystem.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)    13622 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/glean_api.py
+drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.278446 glean-cli-0.6.0/src/glean/utils/
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)        0 2023-01-11 18:02:06.000000 glean-cli-0.6.0/src/glean/utils/__init__.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      509 2023-01-11 18:02:06.000000 glean-cli-0.6.0/src/glean/utils/cli.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     2622 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/utils/grn.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1356 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/utils/resource.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1089 2023-06-23 20:04:07.000000 glean-cli-0.6.0/src/glean/utils/validate_config.py
+drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.279199 glean-cli-0.6.0/src/glean_cli.egg-info/
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1283 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      616 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)        1 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)       41 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      102 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)        6 2023-06-23 20:04:33.000000 glean-cli-0.6.0/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 nathanielstokoe   (501) staff       (20)        0 2023-06-23 20:04:33.279964 glean-cli-0.6.0/tests/
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      309 2023-01-11 18:02:06.000000 glean-cli-0.6.0/tests/test_cli.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     1652 2023-01-11 18:02:06.000000 glean-cli-0.6.0/tests/test_credentials.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)     4632 2023-06-23 20:04:07.000000 glean-cli-0.6.0/tests/test_filesystem.py
+-rw-r--r--   0 nathanielstokoe   (501) staff       (20)      666 2023-01-11 18:02:06.000000 glean-cli-0.6.0/tests/test_glean_api.py
```

### Comparing `glean-cli-0.5.6/LICENSE` & `glean-cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.6/PKG-INFO` & `glean-cli-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.5.6
+Version: 0.6.0
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.5.6/README.md` & `glean-cli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.6/setup.cfg` & `glean-cli-0.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 python_requires = >=3.7
 install_requires = 
 	Click >= 8.0
 	pyyaml >= 6.0
 	requests >= 2.0
 	ruamel.yaml >= 0.17
 	yaspin >= 2.1.0
+	GitPython >= 3.1.30
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	glean = glean.cli:main
```

### Comparing `glean-cli-0.5.6/src/glean/cli.py` & `glean-cli-0.6.0/src/glean/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,62 @@
+from contextlib import suppress
+from itertools import count
 import logging
 import os
+import string
 from typing import Optional, List
+from uuid import UUID, uuid3
 import webbrowser
+from pathlib import Path, PurePath, PurePosixPath
 
 import click
+import git
 from requests import Session
-import ruamel.yaml
+import ruamel.yaml as yaml
 from yaspin import yaspin
 
 from glean import VERSION
 
+from glean.filesystem import local_resources
 from glean.credentials import get_credentials
 from glean.glean_api import (
     build_details_uri,
     clear_model_cache,
     create_build_from_git_revision,
     create_build_from_local_files,
     login,
     preview_model_uri,
     get_datasources,
     get_tables,
     get_model_and_build_summary,
     export_query,
+    pull_resource,
 )
 from glean.utils.cli import cli_error_boundary, getenv_bool
-from glean.utils.grn import GRN_TYPE_KEY_MODEL, parse_grn
+from glean.utils.grn import GRN_TYPE_KEY_MODEL, GRNComponents, parse_grn
+from glean.utils.resource import Resource
 
 
 GLEAN_DEBUG = getenv_bool("GLEAN_DEBUG")
 
 # Turning this on will result in secrets getting logged to stdout.
 GLEAN_VERBOSE_DEBUG_UNSAFE = getenv_bool("GLEAN_VERBOSE_DEBUG_UNSAFE")
 
 
 MAX_COLUMN_REGEX_LENGTH = 30
 MAX_COLUMN_FILTER_CHARS = 1000
 
 
 def main():
     with cli_error_boundary(debug=GLEAN_DEBUG):
+        if not _check_version():
+            logging.warn(
+                "There is a newer version of the Glean CLI available on PyPI. Upgrade your glean-cli package for the latest features.\n"
+            )
+
         cli()
 
 
 git_revision_option = click.option(
     "--git-revision",
     type=str,
     required=False,
@@ -56,14 +70,23 @@
     type=str,
     required=False,
     help="""
     A path within your git repo that will be used as the top-level directory for the Build.
     Only applicable when also using the `--git-revision` flag.
     """,
 )
+dbt_manifest_option = click.option(
+    "--dbt-manifest",
+    "dbt_manifest_path",
+    required=False,
+    # TODO(meyer): unhide when feature is stable
+    hidden=True,
+    help="Path to dbt manifest JSON file (if using Glean dbt integration).",
+    type=click.Path(exists=True, readable=True, file_okay=True, dir_okay=False),
+)
 local_path_argument = click.argument(
     "filepath", type=click.Path(exists=True), default="."
 )
 
 
 @click.group(context_settings=dict(max_content_width=130))
 @click.version_option(version=VERSION, prog_name="Glean")
@@ -92,68 +115,75 @@
     ctx.obj["allow_dangerous_empty_build"] = allow_dangerous_empty_build
     ctx.obj["credentials"] = get_credentials(os.path.expanduser(credentials_filepath))
 
 
 @cli.command()
 @git_revision_option
 @git_path_option
+@dbt_manifest_option
 @local_path_argument
 @click.pass_context
-def preview(ctx, git_revision, git_path, filepath):
+def preview(ctx, git_revision, git_path, dbt_manifest_path, filepath):
     """Validates resource configurations and generates a preview link."""
     click.echo("🏗️  Creating preview build...")
     build_results = _create_build_using_options(
         ctx,
         filepath,
         git_revision=git_revision,
         git_path=git_path,
         deploy=False,
+        dbt_manifest_path=dbt_manifest_path,
     )
     _echo_build_results(build_results, False)
 
 
 @cli.command()
 @git_revision_option
 @git_path_option
+@dbt_manifest_option
 @local_path_argument
 @click.option(
     "--preview / --no-preview",
     default=True,
     help="Whether to generate a Preview Build before deploying.",
 )
 @click.pass_context
 def deploy(
     ctx: click.Context,
     git_revision: Optional[str],
     git_path: Optional[str],
+    dbt_manifest_path: Optional[PurePath],
     filepath: str,
     preview: bool,
 ):
     """Validates and deploys resource configurations to your project."""
+
     if preview:
         click.echo("🏗️  Creating preview build...")
         build_results = _create_build_using_options(
             ctx,
             filepath,
             git_revision=git_revision,
             git_path=git_path,
             deploy=False,
+            dbt_manifest_path=dbt_manifest_path,
         )
         _echo_build_results(build_results, False)
         click.echo("")
         if not click.confirm("Continue with deploy?"):
             exit(1)
 
     click.echo("🚀 Creating deploy build...")
     build_results = _create_build_using_options(
         ctx,
         filepath,
         git_revision=git_revision,
         git_path=git_path,
         deploy=True,
+        dbt_manifest_path=dbt_manifest_path,
     )
     _echo_build_results(build_results, True)
     click.echo("")
     click.echo(click.style("✅ Deploy complete.", fg="bright_green"))
 
 
 @cli.command()
@@ -214,14 +244,192 @@
         exit(1)
 
     clear_model_cache(s, grn.gluid)
     click.echo(f"Successfully cleared cache for {resource_grn}.")
 
 
 @cli.command()
+@click.argument("grn", required=False, type=str)
+@click.option(
+    "--allow-dirty",
+    is_flag=True,
+    default=False,
+    help="Overwrite resources even if the working directory has changes",
+)
+@click.pass_context
+def pull(
+    ctx: click.Context,
+    grn: str,
+    allow_dirty: bool = False,
+):
+    """Pull the latest DataOps resource configuration from Glean into the working directory.
+
+    GRN is the Glean resource name of the target resource. If the resource has DataOps dependencies, they will also be
+    retrieved. If no GRN is specified, all resources for the project are pulled.
+    """
+
+    try:
+        repo = git.Repo(Path("."), search_parent_directories=True)
+        if repo.is_dirty() and not allow_dirty:
+            raise click.ClickException(
+                "️🚩 The working directory has uncommitted changes that might be overwritten. (Skip this check with --allow-dirty.)"
+            )
+    except git.InvalidGitRepositoryError:
+        click.confirm(
+            "The working directory is not a Git repository; this operation may irreversibly change files. Proceed?",
+            default=False,
+            abort=True,
+            show_default=True,
+        )
+
+    s = Session()
+    project_id = login(s, ctx.obj["credentials"])
+
+    resource_type = None
+    resource_id = None
+
+    # map the GRN resource type abbreviation to the full name
+    RESOURCE_TYPE_FROM_ABBREV = {
+        "dsb": "dashboard",
+        "sv": "savedView",
+        "m": "model",
+        "palette": "colorPalette"
+        # todo: support for launch config, collections...
+    }
+    if grn:
+        grn_components = parse_grn(grn)
+
+        # TODO(meyer): add support for aliases
+        try:
+            resource_type = RESOURCE_TYPE_FROM_ABBREV[grn_components.resource_type]
+        except:
+            raise click.ClickException(
+                "Glean pull currently only supports models, saved views, dashboards, and color palettes"
+            )
+        resource_id = grn_components.gluid
+
+    SUPPORTED_TYPES = ["dashboard", "saved_view", "model", "color_palette"]
+    local_by_path = {
+        k: v for k, v in local_resources(Path(".")).items() if v.type in SUPPORTED_TYPES
+    }
+
+    def get_grn(path: PurePosixPath, resource: Resource) -> GRNComponents:
+        RESOURCE_TYPE_TO_ABBREV = {
+            "model": "m",
+            "saved_view": "sv",
+            "dashboard": "dsb",
+            "color_palette": "palette",
+            # TODO(meyer): support for the other resources
+        }
+        if resource.grn is not None:
+            return resource.grn
+
+        elif resource.type == "saved_view":
+            # terrible special case logic for saved views to maintain backwards compatibility,
+            # since saved view IDs include a hash of the model ID
+
+            model_ref: str = resource.raw["model"]
+            model_grn = None
+            try:
+                # resolve model references by file paths to their project-local path
+                model_path = (
+                    Path(path.parent / model_ref).resolve().relative_to(Path.cwd())
+                )
+                if model_path.exists():
+                    model = local_by_path[PurePosixPath(model_path)]
+                    assert model is not None
+                    model_grn = get_grn(PurePosixPath(model_path), model)
+            except OSError:  # python 3.7, Path.exists can throw if the path is invalid
+                pass
+            except ValueError:
+                pass
+
+            # if model is not a local path, it must be a GRN
+            if not model_grn:
+                model_grn = parse_grn(model_ref)
+
+            model_id = model_grn.gluid
+            assert model_id is not None
+
+            default_namespace = UUID("{00000000-0000-0000-0000-000000000000}")
+            initial_id = GRNComponents.generate("sv", project_id, path).gluid
+            assert initial_id is not None
+            sv_id = str(uuid3(default_namespace, model_id + initial_id))
+
+            return GRNComponents("sv", sv_id)
+
+        else:
+            return GRNComponents.generate(
+                RESOURCE_TYPE_TO_ABBREV[resource.type], project_id, path
+            )
+
+    # Can't use a map here because we actually _do_ want to compare GRNs that hash to different values!
+    # In particular, if they have the same type/alias but different guid (because local hasn't received a guid),
+    # they should be considered equal.
+    local_by_grn = list(
+        (get_grn(path, resource), path, resource)
+        for (path, resource) in local_by_path.items()
+    )
+    local_grns = list(local_grn for (local_grn, _, _) in local_by_grn)
+
+    result = pull_resource(s, project_id, resource_type, resource_id)
+    if result.get("errors"):
+        _echo_pull_errors_and_exit(result["errors"])
+        return
+
+    remote: list[Resource] = result["configs"]
+
+    updated_files = []
+    for resource in remote:
+        assert resource.grn is not None
+        with suppress(ValueError):
+            index = local_grns.index(resource.grn)
+            # we've matched the resource to a local file
+            (_, path, local_resource) = local_by_grn[index]
+            if local_resource.raw == resource.raw:
+                continue
+
+            updated_files.append(Path(path))
+            # the resource has changed!
+            with open(Path(path), "w") as f:
+                yaml.dump(resource.raw, f, Dumper=yaml.RoundTripDumper)
+
+            continue
+
+        # not present locally, so we need to make a new file
+        name = "".join(
+            filter(
+                lambda x: x in string.ascii_letters or x in string.digits,
+                resource.raw.get("name", "untitled").lower().replace(" ", "_"),
+            )
+        )
+        name = resource.grn.resource_type + "_" + name
+        for i in count(0):
+            if i > 0:
+                path = Path(f"{name}_{i}.yml")
+            else:
+                path = Path(f"{name}.yml")
+            if path.exists():
+                continue
+
+            updated_files.append(path)
+            with open(path, "w") as f:
+                yaml.dump(resource.raw, f, Dumper=yaml.RoundTripDumper)
+
+            break
+
+    click.echo()
+    if updated_files:
+        click.echo("✅ Done. Files created or modified:")
+        _echo_list([str(p) for p in updated_files])
+    else:
+        click.echo("✅ Done. No files were updated.")
+
+
+@cli.command()
 @click.argument("database")
 @click.argument("table")
 @click.option(
     "--exclude",
     "-e",
     help="A comma-separated list of columns to exclude from the preview.",
 )
@@ -299,18 +507,18 @@
             model, build_summary = get_model_and_build_summary(
                 s, datasource_id, project_id, **model_spec
             )
 
     config = export_query(
         s, "model", model, additional_headers={"Content-Type": "yaml"}
     )
-    model_yaml = ruamel.yaml.load(config, Loader=ruamel.yaml.RoundTripLoader)
+    model_yaml = yaml.load(config, Loader=yaml.RoundTripLoader)
     if "grn" in model_yaml:
         del model_yaml["grn"]
-    config = ruamel.yaml.dump(model_yaml, Dumper=ruamel.yaml.RoundTripDumper)
+    config = yaml.dump(model_yaml, Dumper=yaml.RoundTripDumper)
 
     filename = model["name"]
     _save_config(config, filename, skip_confirmation=skip_confirmation)
 
     _echo_build_results(build_summary, False, query_name="modelPreviewBuildFromGleanDb")
     webbrowser.open(preview_model_uri(model["id"], build_summary))
 
@@ -387,14 +595,15 @@
 
     click.echo("")
 
 
 def _create_build_using_options(
     ctx: click.Context,
     filepath: str,
+    dbt_manifest_path: Optional[PurePath] = None,
     git_revision: Optional[str] = None,
     git_path: Optional[str] = None,
     deploy: bool = False,
     targets: Optional[set] = None,
 ):
     s = Session()
     project_id = login(s, ctx.obj["credentials"])
@@ -403,23 +612,25 @@
         return create_build_from_git_revision(
             s,
             project_id,
             git_revision,
             git_path,
             deploy,
             allow_dangerous_empty_build=allow_dangerous_empty_build,
+            dbt_manifest_path=dbt_manifest_path,
         )
     else:
         return create_build_from_local_files(
             s,
             project_id,
             filepath,
             deploy,
             targets,
             allow_dangerous_empty_build=allow_dangerous_empty_build,
+            dbt_manifest_path=dbt_manifest_path,
         )
 
 
 def _echo_tables(table_names: list, datasource: str) -> None:
     click.secho(f"📂 Available Tables From {datasource}", fg="bright_green")
     _echo_list(table_names)
 
@@ -477,14 +688,27 @@
         _echo_build_warnings(created_build_results["warnings"])
 
     _echo_build_resources(created_build_results["resources"], deploy)
     click.echo("")
     click.echo(f"Details: {build_details_uri(build_results, query_name=query_name)}")
 
 
+def _echo_pull_errors_and_exit(errors: List[str]):
+    click.echo("")
+    click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="red")
+    click.echo("❗ Errors encountered when pulling resources")
+    click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="red")
+    if not errors:
+        errors = ["Something went wrong, please contact Glean for support."]
+    _echo_list(errors, color="red")
+    click.echo("")
+    click.secho("Pull failed. No files were changed.", fg="red")
+    exit(1)
+
+
 def _echo_build_errors_and_exit(errors: List[str]):
     click.echo("")
     click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="red")
     click.echo("❗ Errors encountered when creating your build")
     click.secho("―――――――――――――――――――――――――――――――――――――――――――――――――", fg="red")
     if not errors:
         errors = ["Something went wrong, please contact Glean for support."]
@@ -560,15 +784,14 @@
                 for _ in homepage_launchpads
             ]
         )
         click.echo()
 
 
 def _echo_build_resources(resources: dict, deploy: bool):
-
     added = click.style("Added:" if deploy else "Will add:", bold=True, fg="green")
     _echo_resources_with_status(resources, "added", added)
 
     updated = click.style(
         "Updated:" if deploy else "Will update:", bold=True, fg="cyan"
     )
     _echo_resources_with_status(resources, "changed", updated)
@@ -587,7 +810,56 @@
     logging.basicConfig()
     logging.getLogger().setLevel(logging.DEBUG)
     requests_log = logging.getLogger("urllib3")
     requests_log.setLevel(logging.DEBUG)
     requests_log.propagate = True
     if GLEAN_VERBOSE_DEBUG_UNSAFE:
         HTTPConnection.debuglevel = 1
+
+
+def _check_version():
+    from pathlib import Path
+    import time, requests
+
+    ttl = 24 * 60 * 60
+    path = Path.home() / ".glean" / ".cache" / "version"
+
+    try:
+        os.makedirs(path.parent, exist_ok=True)
+    except:
+        # Could be a permissions issue, or hard drive full, or weird cosmic bit flip...
+        # Just assume we're up-to-date.
+        return True
+
+    try:
+        prev_mtime = os.path.getmtime(path)
+    except Exception:
+        prev_mtime = None
+
+    if prev_mtime is None or time.time() - prev_mtime > ttl:
+        # delete stale cache
+        try:
+            path.unlink()  # missing_ok not available in Python 3.7
+        except:
+            pass
+
+    try:
+        with open(path, "r") as f:
+            return VERSION == f.readline().strip()
+    except:
+        pass
+
+    # cache was stale or did not exist; fetch from pypi
+    try:
+        with open(path, "w+") as f:
+            PACKAGE_JSON_URL = "https://pypi.org/pypi/glean-cli/json"
+            resp = requests.get(PACKAGE_JSON_URL, timeout=1)
+            data = resp.json()
+            LATEST_VERSION: str = list(data["releases"].keys())[-1]
+            f.write(LATEST_VERSION)
+            return VERSION == LATEST_VERSION
+    except Exception as e:
+        logging.warn(
+            f"Unable to check whether this is the latest version of the CLI: {e}."
+        )
+        # Unable to pull version information currently, just return true
+        return True
```

### Comparing `glean-cli-0.5.6/src/glean/credentials.py` & `glean-cli-0.6.0/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.6/src/glean/glean_api.py` & `glean-cli-0.6.0/src/glean/glean_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import json
 import os
-from typing import Optional, Tuple, Dict
+from pathlib import PurePath
+from typing import List, Optional, Tuple, Dict
+from collections import OrderedDict
 
 import click
 from click import ClickException
 from requests import Session
 
 from glean.credentials import CliCredentials
 from glean.filesystem import build_spec_from_local
 from glean import VERSION
+from glean.utils.resource import Resource
 
 GLEAN_BASE_URI = os.environ.get("GLEAN_CLI_BASE_URI", default="https://glean.io")
 
 
 def login(session: Session, credentials: CliCredentials):
     """Authenticates the session with the provided credentials.
 
@@ -46,32 +49,40 @@
 def create_build_from_git_revision(
     session: Session,
     project_id: str,
     git_revision: Optional[str],
     git_path: Optional[str],
     deploy: bool,
     allow_dangerous_empty_build: bool = False,
+    dbt_manifest_path: Optional[PurePath] = None,
 ):
     """Creates a build based on a git revision and returns the result."""
-    build_spec = {"configFilesFromGit": {"revision": git_revision, "path": git_path}}
+    build_spec = {
+        "configFilesFromGit": {
+            "revision": git_revision,
+            "path": git_path,
+            "dbtManifestPath": dbt_manifest_path,
+        }
+    }
     return _create_build(
         session, project_id, build_spec, deploy, allow_dangerous_empty_build
     )
 
 
 def create_build_from_local_files(
     session: Session,
     project_id: str,
     path: str,
     deploy: bool,
     targets: Optional[set],
     allow_dangerous_empty_build: bool = False,
+    dbt_manifest_path: Optional[PurePath] = None,
 ):
     """Creates a build using local files and returns the result."""
-    build_spec = build_spec_from_local(path, project_id, targets)
+    build_spec = build_spec_from_local(path, project_id, targets, dbt_manifest_path)
     return _create_build(
         session, project_id, build_spec, deploy, allow_dangerous_empty_build
     )
 
 
 def get_model_and_build_summary(
     session: Session,
@@ -117,14 +128,50 @@
             updateModelFreshnessKey(id: $id)
         }
         """,
         {"id": model_id},
     )
 
 
+class PullResourceResponse(dict):
+    configs: List[Resource]
+    errors: List[str]
+
+
+def pull_resource(
+    s: Session,
+    project_id: str,
+    resource_type: Optional[str],
+    resource_id: Optional[str],
+) -> PullResourceResponse:
+    """Pulls the DataOps config for the given resource, or all resources in the project if none is specified."""
+    res = _graphql_query(
+        s,
+        """
+        query PullResource($projectId: String!, $resourceType: String, $resourceId: String) {
+            pullResource(
+                projectId: $projectId,
+                resourceType: $resourceType,
+                resourceId: $resourceId
+            ) { configs, errors }
+        }
+        """,
+        {
+            "projectId": project_id,
+            "resourceType": resource_type,
+            "resourceId": resource_id,
+        },
+    )["data"]["pullResource"]
+    res["configs"] =  [
+        Resource.from_dict(json.loads(string))
+        for string in res["configs"]
+    ]
+    return res
+
+
 def _parse_table_data(table_data: dict) -> Dict[str, Dict[str, str]]:
     """Formats table names for output, and returns tables names and schemas"""
     tables = table_data["data"]["getAvailableGleanDbTables"]
     tables_by_name = {}
     for table in tables:
         name = (
             table["schema"] + "." + table["name"] if table["schema"] else table["name"]
@@ -324,15 +371,15 @@
     elif r.status_code != 200:
         raise ClickException("Unexpected error received from the Glean server.")
 
     results = r.json()
     graphql_exceptions = results.get("errors")
     if (
         graphql_exceptions
-        and type(graphql_exceptions[0]) is dict
+        and isinstance(graphql_exceptions[0], dict)
         and graphql_exceptions[0].get("message")
     ):
         error = graphql_exceptions[0]["message"]
         raise ClickException(
             f"Unexpected error received from the Glean server:\n  {error}"
         )
```

### Comparing `glean-cli-0.5.6/src/glean/utils/grn.py` & `glean-cli-0.6.0/src/glean/utils/grn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from pathlib import PurePath, PurePosixPath
 from typing import Optional
 from dataclasses import dataclass
+from uuid import UUID, uuid3
 
 from click import ClickException
 
 
 GRN_TYPE_KEY_MODEL = "m"
 GRN_TYPE_KEY_SAVED_VIEW = "sv"
 GRN_TYPE_KEY_DASHBOARD = "dsb"
@@ -12,14 +14,41 @@
 
 @dataclass
 class GRNComponents:
     resource_type: str
     gluid: Optional[str] = None
     alias: Optional[str] = None
 
+    @staticmethod
+    def generate(resource_type: str, project_id: str, local_path: PurePath):
+        # mirrors server logic
+        default_namespace = UUID("{00000000-0000-0000-0000-000000000000}")
+        path: PurePosixPath = (
+            PurePosixPath("/tmp/repos") / project_id / PurePosixPath(local_path)
+        )
+        return GRNComponents(resource_type, str(uuid3(default_namespace, f"{project_id}|{str(path)}")))
+    
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, GRNComponents):
+            return False
+        if self.resource_type != other.resource_type:
+            return False
+
+        if self.alias and other.alias:
+            return self.alias == other.alias 
+
+        return self.gluid == other.gluid
+
+    def __str__(self) -> str:
+        if self.alias is not None:
+            return f"{self.resource_type}:{self.gluid}:{self.alias}"
+        else:
+            return f"{self.resource_type}:{self.gluid}"
+
 
 def parse_grn(grn: str) -> GRNComponents:
     components = grn.split(":")
 
     resource_type = components[0]
     if resource_type not in [
         GRN_TYPE_KEY_MODEL,
```

### Comparing `glean-cli-0.5.6/src/glean/utils/validate_config.py` & `glean-cli-0.6.0/src/glean/utils/validate_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import yaml
 
 parse_failure_message = lambda filename, e: f"\n Could not parse file {filename}. \n Errors found in this file: \n ---- \n {e}"
 
 def _is_valid_yaml_config_file(contents: str, filename: str) -> bool:
     try:
         data = yaml.safe_load(contents)
-        return data.get("glean") is not None
+        return isinstance(data, dict) and data.get("glean") is not None
     except yaml.YAMLError as e:
         raise ClickException(parse_failure_message(filename, e))
 
 
 def _is_valid_json_config_file(contents: str, filename: str) -> bool:
     try:
         data = json.loads(contents)
-        return data.get("glean") is not None
+        return isinstance(data, dict) and data.get("glean") is not None
     except json.decoder.JSONDecodeError as e:
         raise ClickException(parse_failure_message(filename, e))
 
 
 def is_valid_glean_config_file(filename: str, contents: str) -> bool:
     if filename.endswith(".yml") or filename.endswith(".yaml"):
         return _is_valid_yaml_config_file(contents, filename)
```

### Comparing `glean-cli-0.5.6/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.6.0/src/glean_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.5.6
+Version: 0.6.0
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.5.6/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.6.0/src/glean_cli.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/glean/cli.py
 src/glean/credentials.py
 src/glean/filesystem.py
 src/glean/glean_api.py
 src/glean/utils/__init__.py
 src/glean/utils/cli.py
 src/glean/utils/grn.py
+src/glean/utils/resource.py
 src/glean/utils/validate_config.py
 src/glean_cli.egg-info/PKG-INFO
 src/glean_cli.egg-info/SOURCES.txt
 src/glean_cli.egg-info/dependency_links.txt
 src/glean_cli.egg-info/entry_points.txt
 src/glean_cli.egg-info/requires.txt
 src/glean_cli.egg-info/top_level.txt
```

### Comparing `glean-cli-0.5.6/tests/test_credentials.py` & `glean-cli-0.6.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.5.6/tests/test_glean_api.py` & `glean-cli-0.6.0/tests/test_glean_api.py`

 * *Files identical despite different names*

