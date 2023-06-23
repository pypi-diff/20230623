# Comparing `tmp/godoo_cli-0.5.1.tar.gz` & `tmp/godoo_cli-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godoo_cli-0.5.1.tar", max compression
+gzip compressed data, was "godoo_cli-0.5.2.tar", max compression
```

## Comparing `godoo_cli-0.5.1.tar` & `godoo_cli-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     7633 2023-06-20 17:50:48.696537 godoo_cli-0.5.1/LICENSE
--rw-r--r--   0        0        0     7304 2023-06-20 17:50:48.696537 godoo_cli-0.5.1/README.md
--rw-r--r--   0        0        0     5004 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       61 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/__init__.py
--rw-r--r--   0        0        0       88 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/__main__.py
--rw-r--r--   0        0        0     1963 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/cli.py
--rw-r--r--   0        0        0     5596 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/cli_common.py
--rw-r--r--   0        0        0      293 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/__init__.py
--rw-r--r--   0        0        0     5929 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/bootstrap.py
--rw-r--r--   0        0        0     1173 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/config.py
--rw-r--r--   0        0        0       28 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/__init__.py
--rw-r--r--   0        0        0      311 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/cli.py
--rw-r--r--   0        0        0     1801 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/connection.py
--rw-r--r--   0        0        0     1325 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/passwords.py
--rw-r--r--   0        0        0    10763 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/launch.py
--rw-r--r--   0        0        0      177 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/__init__.py
--rw-r--r--   0        0        0      897 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/cli.py
--rw-r--r--   0        0        0     1484 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/config_parameters.py
--rw-r--r--   0        0        0     2278 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/importer.py
--rw-r--r--   0        0        0     4828 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/modules.py
--rw-r--r--   0        0        0     4000 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/translations.py
--rw-r--r--   0        0        0     1619 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/shell.py
--rw-r--r--   0        0        0     8544 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/source_get.py
--rw-r--r--   0        0        0     4562 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/test.py
--rw-r--r--   0        0        0      161 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_odoo.py
--rw-r--r--   0        0        0     3296 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_odoo_addons.py
--rw-r--r--   0        0        0     6460 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_repo.py
--rw-r--r--   0        0        0     4585 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_url.py
--rw-r--r--   0        0        0     1575 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/zip_download.py
--rw-r--r--   0        0        0       49 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     2225 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/bootstrap.py
--rw-r--r--   0        0        0      386 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/cli.py
--rw-r--r--   0        0        0     8895 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_files.py
--rw-r--r--   0        0        0     3277 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_manifest.py
--rw-r--r--   0        0        0     2766 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/system.py
--rw-r--r--   0        0        0       22 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/version.py
--rw-r--r--   0        0        0     9324 1970-01-01 00:00:00.000000 godoo_cli-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/LICENSE
+-rw-r--r--   0        0        0     7297 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/README.md
+-rw-r--r--   0        0        0     5004 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/__main__.py
+-rw-r--r--   0        0        0     1963 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/cli.py
+-rw-r--r--   0        0        0     5397 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/cli_common.py
+-rw-r--r--   0        0        0      293 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/__init__.py
+-rw-r--r--   0        0        0     5811 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/bootstrap.py
+-rw-r--r--   0        0        0     1173 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/config.py
+-rw-r--r--   0        0        0       28 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/cli.py
+-rw-r--r--   0        0        0     1801 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/connection.py
+-rw-r--r--   0        0        0     1325 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/db/passwords.py
+-rw-r--r--   0        0        0    10339 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/launch.py
+-rw-r--r--   0        0        0      177 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/cli.py
+-rw-r--r--   0        0        0     1484 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/config_parameters.py
+-rw-r--r--   0        0        0     2278 2023-06-23 20:09:58.643758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/importer.py
+-rw-r--r--   0        0        0     4828 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/modules.py
+-rw-r--r--   0        0        0     4000 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/rpc/translations.py
+-rw-r--r--   0        0        0     1619 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/shell.py
+-rw-r--r--   0        0        0     8544 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/source_get.py
+-rw-r--r--   0        0        0     4437 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/commands/test.py
+-rw-r--r--   0        0        0      161 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_odoo.py
+-rw-r--r--   0        0        0     3296 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_odoo_addons.py
+-rw-r--r--   0        0        0     6460 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_repo.py
+-rw-r--r--   0        0        0     4585 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/git_url.py
+-rw-r--r--   0        0        0     1575 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/git/zip_download.py
+-rw-r--r--   0        0        0       49 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     2225 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/bootstrap.py
+-rw-r--r--   0        0        0      386 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/cli.py
+-rw-r--r--   0        0        0     8895 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_files.py
+-rw-r--r--   0        0        0     3277 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_manifest.py
+-rw-r--r--   0        0        0     2766 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/helpers/system.py
+-rw-r--r--   0        0        0       22 2023-06-23 20:09:58.647758 godoo_cli-0.5.2/src/godoo_cli/version.py
+-rw-r--r--   0        0        0     9317 1970-01-01 00:00:00.000000 godoo_cli-0.5.2/PKG-INFO
```

### Comparing `godoo_cli-0.5.1/LICENSE` & `godoo_cli-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/README.md` & `godoo_cli-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 There are 3 Options to reset the Dev Env.
 
 1. From **Outside** the Container run `make reset` in the project root to delete docker volumes and restart the
    container. (Vscode will prompt to reconnect if still open)
 2. From **Outside** the Container run `make reset-hard` in the project root to force rebuild the main Odoo container and
    then do the same as `make reset`
-3. From **Inside** the Container run `make reset` to drop the DB and delete varlib and the bootstrap flag, which is way
+3. From **Inside** the Container run `make reset` to drop the DB and delete varlib and config file, which is way
    quicker than the other options.
 
 ### Manual Reset
 
 1. Close vscode
 2. Remove `app` and `db` container from docker.
 3. Remove volumes: `db, odoo_thirdparty, odoo_web, vscode_extensions`
```

### Comparing `godoo_cli-0.5.1/pyproject.toml` & `godoo_cli-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gOdoo-cli"
-version = "0.5.1"
+version = "0.5.2"
 description = "Wrapper around Odoo-Bin with some convinience RPC functions."
 authors = ["Joshua Kreuder <Joshua_Kreuder@outlook.com>"]
 license = "LGPL-3"
 readme = "README.md"
 packages = [{include = "godoo_cli",  from = "src"}]
 repository = "https://github.com/OpenJKSoftware/gOdoo"
 keywords = ["odoo", "godoo","devcontainer"]
```

### Comparing `godoo_cli-0.5.1/src/godoo_cli/cli.py` & `godoo_cli-0.5.2/src/godoo_cli/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/cli_common.py` & `godoo_cli-0.5.2/src/godoo_cli/cli_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,21 +69,14 @@
     thirdparty_addon_path: Path = Option(
         ...,
         envvar="ODOO_THIRDPARTY_LOCATION",
         help="folder that contains thirdparty repos like OCA",
         rich_help_panel="Path Options",
     )
 
-    bootstrap_flag_location: Path = Option(
-        ...,
-        envvar="ODOO_BOOTSTRAP_FLAG",
-        help="Location of the Bootstrap indicator file",
-        rich_help_panel="Path Options",
-    )
-
 
 @dataclass
 class RpcCLIArgs:
     rpc_host: str = Option(
         ...,
         envvar="ODOO_RPC_HOST",
         help="Odoo RPC Host",
```

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/bootstrap.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 @CLI.unpacker
 @CLI.arg_annotator
 def bootstrap_odoo(
     odoo_main_path=CLI.odoo_paths.bin_path,
     workspace_addon_path=CLI.odoo_paths.workspace_addon_path,
     thirdparty_addon_path=CLI.odoo_paths.thirdparty_addon_path,
     odoo_conf_path=CLI.odoo_paths.conf_path,
-    bootstrap_flag_location=CLI.odoo_paths.bootstrap_flag_location,
     db_filter=CLI.database.db_filter,
     db_host=CLI.database.db_host,
     db_port=CLI.database.db_port,
     db_name=CLI.database.db_name,
     db_user=CLI.database.db_user,
     db_password=CLI.database.db_password,
     extra_cmd_args=CLI.odoo_launch.extra_cmd_args,
@@ -179,12 +178,10 @@
     )
 
     # Always update Pip reqs regardless of --no-update-source
     _install_py_reqs_by_odoo_cmd(addon_paths=addon_paths, odoo_bin_cmd=cmd_string)
 
     LOGGER.info("Launching Bootstrap Commandline")
     ret = run_cmd(cmd_string).returncode
-    if ret == 0:
-        bootstrap_flag_location.touch()
-    else:
+    if ret != 0:
         LOGGER.error("Odoo-Bin Returned %d", ret)
     return CLI.returner(ret)
```

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/config.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/db/connection.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/db/connection.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/db/passwords.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/db/passwords.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/launch.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/launch.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     odoo_cmd = list(filter(None, odoo_cmd))
     return " ".join(odoo_cmd)
 
 
 def pre_launch(
     odoo_main_path: Path,
     workspace_addon_path: Path,
-    bootstrap_flag_location: Path,
     thirdparty_addon_path: Path,
     odoo_conf_path: Path,
     db_filter: str,
     db_host: str,
     db_port: int,
     db_name: str,
     db_user: str,
@@ -71,24 +70,22 @@
     extra_launch_args: List[str] = None,
     extra_bootstrap_args: List[str] = None,
     log_file_path: Path = None,
     install_workspace_addons: bool = True,
     install_base: bool = True,
     launch_or_bootstrap: bool = False,
 ):
-    """Start Bootstrap if no bootstrap flag is found. And return Launch CMD.
+    """Start Bootstrap if no config file is found. And return Launch CMD.
 
     Parameters
     ----------
     odoo_main_path : Path
         Path to Odoo-bin folder
     workspace_addon_path : Path
         Path to workspace addons
-    bootstrap_flag_location : Path
-        path to bootstrap flag
     thirdparty_addon_path : Path
         path to thirdparty addons folder
     odoo_conf_path : Path
         path to odoo conf
     db_filter : str
         odoo.conf db_filter
     db_host : str
@@ -128,15 +125,15 @@
     LOGGER.info("Starting godoo Init Script")
 
     extra_odoo_args = []
     if log_file_path is not None:
         log_file_path.unlink(missing_ok=True)
         extra_odoo_args.append("--logfile " + str(log_file_path.absolute()))
 
-    bootstraped = bootstrap_flag_location.exists()
+    bootstraped = odoo_conf_path.exists()
     LOGGER.info("Bootstrap Flag Status: %s", bootstraped)
     ret = ""
     if not bootstraped:
         _extra_bootstrap_args = extra_odoo_args.copy()
         if ea := extra_bootstrap_args:
             _extra_bootstrap_args += ea
         if not odoo_demo:
@@ -146,15 +143,14 @@
         ret = bootstrap_odoo(
             db_name=db_name,
             db_filter=db_filter,
             db_user=db_user,
             db_password=db_password,
             db_host=db_host,
             db_port=db_port,
-            bootstrap_flag_location=bootstrap_flag_location,
             thirdparty_addon_path=thirdparty_addon_path,
             odoo_main_path=odoo_main_path,
             odoo_conf_path=odoo_conf_path,
             extra_cmd_args=_extra_bootstrap_args,
             no_install_base=not install_base,
             no_install_workspace_modules=not install_workspace_addons,
             multithread_worker_count=multithread_worker_count,
@@ -189,15 +185,14 @@
 
 
 @CLI.unpacker
 @CLI.arg_annotator
 def launch_odoo(
     odoo_main_path=CLI.odoo_paths.bin_path,
     workspace_addon_path=CLI.odoo_paths.workspace_addon_path,
-    bootstrap_flag_location=CLI.odoo_paths.bootstrap_flag_location,
     thirdparty_addon_path=CLI.odoo_paths.thirdparty_addon_path,
     odoo_conf_path=CLI.odoo_paths.conf_path,
     db_filter=CLI.database.db_filter,
     db_host=CLI.database.db_host,
     db_port=CLI.database.db_port,
     db_name=CLI.database.db_name,
     db_user=CLI.database.db_user,
@@ -214,15 +209,14 @@
     """
     Launch Odoo, Bootstrap if bootstrapflag is not present.
     """
 
     launch_cmd = pre_launch(
         odoo_main_path=odoo_main_path,
         workspace_addon_path=workspace_addon_path,
-        bootstrap_flag_location=bootstrap_flag_location,
         thirdparty_addon_path=thirdparty_addon_path,
         odoo_conf_path=odoo_conf_path,
         db_filter=db_filter,
         db_host=db_host,
         db_port=db_port,
         db_name=db_name,
         db_user=db_user,
@@ -249,15 +243,14 @@
 def launch_import(
     load_data_path: List[Path] = typer.Argument(
         ...,
         help="Starts Async Importer Job with provided path(s).",
     ),
     odoo_main_path=CLI.odoo_paths.bin_path,
     workspace_addon_path=CLI.odoo_paths.workspace_addon_path,
-    bootstrap_flag_location=CLI.odoo_paths.bootstrap_flag_location,
     thirdparty_addon_path=CLI.odoo_paths.thirdparty_addon_path,
     odoo_conf_path=CLI.odoo_paths.conf_path,
     db_filter=CLI.database.db_filter,
     db_host=CLI.database.db_host,
     db_port=CLI.database.db_port,
     db_name=CLI.database.db_name,
     db_user=CLI.database.db_user,
@@ -275,15 +268,14 @@
     multithread_worker_count=CLI.odoo_launch.multithread_worker_count,
 ):
     """Bootstrap and Start odoo. Launches RPC import in second thread."""
 
     launch_cmd = pre_launch(
         odoo_main_path=odoo_main_path,
         workspace_addon_path=workspace_addon_path,
-        bootstrap_flag_location=bootstrap_flag_location,
         thirdparty_addon_path=thirdparty_addon_path,
         odoo_conf_path=odoo_conf_path,
         db_filter=db_filter,
         db_host=db_host,
         db_port=db_port,
         db_name=db_name,
         db_user=db_user,
```

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/cli.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/config_parameters.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/config_parameters.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/importer.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/importer.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/modules.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/translations.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/rpc/translations.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/shell.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/source_get.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/source_get.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/commands/test.py` & `godoo_cli-0.5.2/src/godoo_cli/commands/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 def odoo_test(
     test_modules: List[str] = typer.Argument(
         ...,
         help="Modules to install and test (Use 'all' for all Workspace modules), ('changes:<branch> to compare git changes)",
     ),
     odoo_main_path=CLI.odoo_paths.bin_path,
     workspace_addon_path=CLI.odoo_paths.workspace_addon_path,
-    bootstrap_flag_location=CLI.odoo_paths.bootstrap_flag_location,
     thirdparty_addon_path=CLI.odoo_paths.thirdparty_addon_path,
     odoo_conf_path=CLI.odoo_paths.conf_path,
     db_filter=CLI.database.db_filter,
     db_host=CLI.database.db_host,
     db_port=CLI.database.db_port,
     db_name=CLI.database.db_name,
     db_user=CLI.database.db_user,
@@ -97,15 +96,14 @@
     ]
 
     launch_cmd = pre_launch(
         odoo_main_path=odoo_main_path,
         workspace_addon_path=workspace_addon_path,
         thirdparty_addon_path=thirdparty_addon_path,
         odoo_conf_path=odoo_conf_path,
-        bootstrap_flag_location=bootstrap_flag_location,
         db_filter=db_filter,
         db_host=db_host,
         db_port=db_port,
         db_name=db_name,
         db_user=db_user,
         db_password=db_password,
         dev_mode=False,
```

### Comparing `godoo_cli-0.5.1/src/godoo_cli/git/git_odoo.py` & `godoo_cli-0.5.2/src/godoo_cli/git/git_odoo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/git/git_odoo_addons.py` & `godoo_cli-0.5.2/src/godoo_cli/git/git_odoo_addons.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/git/git_repo.py` & `godoo_cli-0.5.2/src/godoo_cli/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/git/git_url.py` & `godoo_cli-0.5.2/src/godoo_cli/git/git_url.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/git/zip_download.py` & `godoo_cli-0.5.2/src/godoo_cli/git/zip_download.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/helpers/bootstrap.py` & `godoo_cli-0.5.2/src/godoo_cli/helpers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_files.py` & `godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_files.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_manifest.py` & `godoo_cli-0.5.2/src/godoo_cli/helpers/odoo_manifest.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/src/godoo_cli/helpers/system.py` & `godoo_cli-0.5.2/src/godoo_cli/helpers/system.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.1/PKG-INFO` & `godoo_cli-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godoo-cli
-Version: 0.5.1
+Version: 0.5.2
 Summary: Wrapper around Odoo-Bin with some convinience RPC functions.
 Home-page: https://github.com/OpenJKSoftware/gOdoo
 License: LGPL-3
 Keywords: odoo,godoo,devcontainer
 Author: Joshua Kreuder
 Author-email: Joshua_Kreuder@outlook.com
 Requires-Python: >=3.8.1,<3.12
@@ -157,15 +157,15 @@
 
 There are 3 Options to reset the Dev Env.
 
 1. From **Outside** the Container run `make reset` in the project root to delete docker volumes and restart the
    container. (Vscode will prompt to reconnect if still open)
 2. From **Outside** the Container run `make reset-hard` in the project root to force rebuild the main Odoo container and
    then do the same as `make reset`
-3. From **Inside** the Container run `make reset` to drop the DB and delete varlib and the bootstrap flag, which is way
+3. From **Inside** the Container run `make reset` to drop the DB and delete varlib and config file, which is way
    quicker than the other options.
 
 ### Manual Reset
 
 1. Close vscode
 2. Remove `app` and `db` container from docker.
 3. Remove volumes: `db, odoo_thirdparty, odoo_web, vscode_extensions`
```

