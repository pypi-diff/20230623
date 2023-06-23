# Comparing `tmp/multitool-0.3.2.tar.gz` & `tmp/multitool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multitool-0.3.2.tar", last modified: Fri Jul  8 17:42:28 2022, max compression
+gzip compressed data, was "multitool-0.4.0.tar", last modified: Fri Jun 23 10:45:00 2023, max compression
```

## Comparing `multitool-0.3.2.tar` & `multitool-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 17:42:28.458669 multitool-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-07-08 17:42:18.000000 multitool-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5540 2022-07-08 17:42:28.458669 multitool-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4951 2022-07-08 17:42:18.000000 multitool-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 17:42:28.454669 multitool-0.3.2/multitool/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/cls.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/console.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 17:42:28.458669 multitool-0.3.2/multitool/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6726 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/plugins/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/silent.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-07-08 17:42:18.000000 multitool-0.3.2/multitool/verbose.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 17:42:28.458669 multitool-0.3.2/multitool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5540 2022-07-08 17:42:28.000000 multitool-0.3.2/multitool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-07-08 17:42:28.000000 multitool-0.3.2/multitool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 17:42:28.000000 multitool-0.3.2/multitool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-08 17:42:28.000000 multitool-0.3.2/multitool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-07-08 17:42:28.000000 multitool-0.3.2/multitool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-08 17:42:28.000000 multitool-0.3.2/multitool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-08 17:42:28.458669 multitool-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-07-08 17:42:18.000000 multitool-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 17:42:28.458669 multitool-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-08 17:42:18.000000 multitool-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-07-08 17:42:18.000000 multitool-0.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:45:00.958942 multitool-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 10:44:50.000000 multitool-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-23 10:45:00.954942 multitool-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-23 10:44:50.000000 multitool-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:45:00.954942 multitool-0.4.0/multitool/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:45:00.954942 multitool-0.4.0/multitool/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/plugins/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/silent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-23 10:44:50.000000 multitool-0.4.0/multitool/verbose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:45:00.954942 multitool-0.4.0/multitool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-23 10:45:00.000000 multitool-0.4.0/multitool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 10:45:00.000000 multitool-0.4.0/multitool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:45:00.000000 multitool-0.4.0/multitool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 10:45:00.000000 multitool-0.4.0/multitool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 10:45:00.000000 multitool-0.4.0/multitool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 10:45:00.000000 multitool-0.4.0/multitool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:45:00.958942 multitool-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-23 10:44:50.000000 multitool-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:45:00.954942 multitool-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:44:50.000000 multitool-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 10:44:50.000000 multitool-0.4.0/tests/test_utils.py
```

### Comparing `multitool-0.3.2/LICENSE` & `multitool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multitool-0.3.2/PKG-INFO` & `multitool-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: multitool
-Version: 0.3.2
+Version: 0.4.0
 Summary: General-purpose command-line interface with plugins support
 Home-page: https://github.com/mdelotavo/multitool
 Author: Matthew Delotavo
 Author-email: matthew.t.delotavo@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 multitool
 =========
 
 Multitool is a general-purpose command-line interface with plugins support.
 
@@ -167,9 +166,7 @@
 
         deactivate
 
 .. _`click`: https://click.palletsprojects.com/
 .. _`apigeecli`: https://pypi.org/project/apigeecli/
 .. _`multitool-plugins`: https://github.com/mdelotavo/multitool-plugins
 .. _`public plugins repository`: https://github.com/mdelotavo/multitool-plugins
-
-
```

### Comparing `multitool-0.3.2/README.rst` & `multitool-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `multitool-0.3.2/multitool/__init__.py` & `multitool-0.4.0/multitool/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 APP = 'multitool'
-__version__ = '0.3.2'
+__version__ = '0.4.0'
 description = 'General-purpose command-line interface with plugins support'
 # long_description = 'General-purpose command-line interface with plugins support'
 
 import builtins
 from pathlib import Path
 
-from multitool.utils import gen_path_str
+from multitool.utils import join_path_components
 
 MULTITOOL_TOGGLE_SILENT = False
 MULTITOOL_TOGGLE_VERBOSE = 0
 
-MULTITOOL_DIRECTORY = gen_path_str(Path.home(), '.multitool')
+MULTITOOL_DIRECTORY = join_path_components(Path.home(), '.multitool')
 
-MULTITOOL_LOG_FILE = gen_path_str(MULTITOOL_DIRECTORY, f'{APP}.log')
+MULTITOOL_LOG_FILE = join_path_components(MULTITOOL_DIRECTORY, f'{APP}.log')
 
-MULTITOOL_PLUGINS_DIRECTORY = gen_path_str(MULTITOOL_DIRECTORY, 'plugins')
-MULTITOOL_PLUGINS_CONFIG_FILE = gen_path_str(MULTITOOL_PLUGINS_DIRECTORY, 'config')
-MULTITOOL_PLUGINS_PATH = gen_path_str(MULTITOOL_PLUGINS_DIRECTORY, '__init__.py')
+MULTITOOL_PLUGINS_DIRECTORY = join_path_components(MULTITOOL_DIRECTORY, 'plugins')
+MULTITOOL_PLUGINS_CONFIG_FILE = join_path_components(MULTITOOL_PLUGINS_DIRECTORY, 'config')
+MULTITOOL_PLUGINS_PATH = join_path_components(MULTITOOL_PLUGINS_DIRECTORY, '__init__.py')
 
 builtins.MULTITOOL_TOGGLE_SILENT = MULTITOOL_TOGGLE_SILENT
 builtins.MULTITOOL_TOGGLE_VERBOSE = MULTITOOL_TOGGLE_VERBOSE
```

### Comparing `multitool-0.3.2/multitool/__main__.py` & `multitool-0.4.0/multitool/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 #!/usr/bin/env python
 # __main__.py
 
-import codecs
-import configparser
-import importlib
-import os
-import re
-import sys
-import time
-from functools import update_wrapper
-
 import click
-import requests
 
-from multitool import (APP, MULTITOOL_LOG_FILE, MULTITOOL_PLUGINS_DIRECTORY,
-                       MULTITOOL_PLUGINS_PATH)
+from multitool import APP, MULTITOOL_LOG_FILE, MULTITOOL_PLUGINS_DIRECTORY
 from multitool import __version__ as version
 from multitool.cls import AliasedGroup
-from multitool.exceptions import exception_handler
+from multitool.exceptions import wrap_with_exception_handling
 from multitool.plugins.commands import plugins
-from multitool.utils import (import_all_modules_in_directory,
-                             run_func_on_dir_files, setup_global_logger,
-                             show_message)
+from multitool.utils import (import_plugins_from_directory,
+                             execute_function_on_directory_files, configure_global_logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.group(
     context_settings=CONTEXT_SETTINGS, cls=AliasedGroup, invoke_without_command=False, chain=False
 )
@@ -41,23 +29,23 @@
     \f
 
     :param click.core.Context ctx: Click context.
     """
     ctx.ensure_object(dict)
 
 
-@exception_handler
+@wrap_with_exception_handling
 def main():
-    setup_global_logger(MULTITOOL_LOG_FILE)
+    configure_global_logger(MULTITOOL_LOG_FILE)
 
     cli_commands = {plugins}
 
-    run_func_on_dir_files(
+    execute_function_on_directory_files(
         MULTITOOL_PLUGINS_DIRECTORY,
-        import_all_modules_in_directory,
+        import_plugins_from_directory,
         args=(cli_commands,),
         glob='[!.][!__]*/__init__.py',
     )
 
     for command in cli_commands:
         cli.add_command(command)
```

### Comparing `multitool-0.3.2/multitool/exceptions.py` & `multitool-0.4.0/multitool/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import functools
 import inspect
-import json
 import logging
 import sys
 
 from multitool import console
 
 
-def exception_handler(func):
+def wrap_with_exception_handling(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         try:
             result = func(*args, **kwargs)
             return result
         except Exception as e:
             logging.error('Exception occurred', exc_info=True)
```

### Comparing `multitool-0.3.2/multitool/plugins/commands.py` & `multitool-0.4.0/multitool/plugins/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,231 +1,229 @@
 import configparser
-import json
 import os
 import shutil
 import stat
 import sys
 from os import path
 from pathlib import Path
 
 import click
 from click_option_group import MutuallyExclusiveOptionGroup, optgroup
 
 from multitool import (MULTITOOL_PLUGINS_CONFIG_FILE,
                        MULTITOOL_PLUGINS_DIRECTORY, MULTITOOL_PLUGINS_PATH,
                        console)
 from multitool.silent import common_silent_options
-from multitool.utils import (is_dir, is_file, make_dirs, read_file,
-                             run_func_on_dir_files, touch)
+from multitool.utils import (is_directory, is_regular_file, create_directory, read_file_content,
+                             execute_function_on_directory_files, create_empty_file)
 from multitool.verbose import common_verbose_options
 
 is_git_installed = False
 plugins_command_help = 'Simple plugins manager for distributing commands.'
 
 try:
-    import git
-    from git import Git, Repo
+    from git import Repo
 
     is_git_installed = True
 except ImportError:
     plugins_command_help = '[Git not found! Please install Git first.] Simple plugins manager for distributing commands. This command requires Git to be installed.'
 
 
-def exit_if_git_not_installed():
+def chmod_directory(directory, mode):
+    """
+    Recursively changes the permissions of a directory and its contents.
+
+    Reference: https://stackoverflow.com/a/58878271
+    
+    Args:
+        directory (str): Path to the directory.
+        mode (int): Permissions to be set (e.g., 0o0700).
+
+    """
+    for root, dirs, files in os.walk(directory):
+        for dir in dirs:
+            os.chmod(path.join(root, dir), mode)
+        for file in files:
+            os.chmod(path.join(root, file), mode)
+
+
+def clone_plugin_repositories(section="sources"):
+    initialize_MULTITOOL_plugins()
+    config = load_plugin_config()
+    if not config._sections:
+        return
+    sources = dict(config._sections[section])
+    for name, uri in sources.items():
+        dest = Path(MULTITOOL_PLUGINS_DIRECTORY) / name
+        if is_directory(dest):
+            continue
+        try:
+            console.echo(f"Installing {name}... ", line_ending="", should_flush=True)
+            Repo.clone_from(uri, dest)
+            console.echo("Done")
+        except Exception as e:
+            console.echo(e)
+
+
+def exit_quietly_if_git_not_installed():
     if not is_git_installed:
         sys.exit(0)
 
 
-@click.group(help=plugins_command_help)
-def plugins():
-    pass
+def initialize_and_save_plugin_config():
+    initialize_MULTITOOL_plugins()
+    config = load_plugin_config()
+    if not config._sections:
+        return
 
 
-def init():
-    make_dirs(MULTITOOL_PLUGINS_DIRECTORY)
-    touch(MULTITOOL_PLUGINS_PATH)
-    touch(MULTITOOL_PLUGINS_CONFIG_FILE)
+def initialize_MULTITOOL_plugins():
+    create_directory(MULTITOOL_PLUGINS_DIRECTORY)
+    create_empty_file(MULTITOOL_PLUGINS_PATH)
+    create_empty_file(MULTITOOL_PLUGINS_CONFIG_FILE)
 
 
-def load_config(config_file=MULTITOOL_PLUGINS_CONFIG_FILE):
+def load_plugin_config(config_file=MULTITOOL_PLUGINS_CONFIG_FILE):
     config = configparser.ConfigParser(allow_no_value=True)
     config.read(config_file)
     return config
 
 
-def save_config(plugins_file, config_file, section='sources'):
-    init()
-    config = load_config()
-    if not config._sections:
-        return
-
-
-def clone_all(section='sources'):
-    init()
-    config = load_config()
+def prune_unused_plugin_directories(section="sources"):
+    initialize_MULTITOOL_plugins()
+    config = load_plugin_config()
     if not config._sections:
         return
     sources = dict(config._sections[section])
-    for name, uri in sources.items():
-        dest = Path(MULTITOOL_PLUGINS_DIRECTORY) / name
-        if is_dir(dest):
-            continue
+
+    def _func(path):
+        if not is_directory(path):
+            return
+        name = Path(path).stem
+        if name in sources:
+            return
+        console.echo(f"Removing {name}... ", line_ending="", should_flush=True)
+        plugin_directory = Path(MULTITOOL_PLUGINS_DIRECTORY) / name
         try:
-            console.echo(f'Installing {name}... ', end='', flush=True)
-            Repo.clone_from(uri, dest)
-            console.echo('Done')
+            chmod_directory(str(Path(plugin_directory) / ".git"), stat.S_IRWXU)
+            shutil.rmtree(plugin_directory)
+            console.echo("Done")
         except Exception as e:
             console.echo(e)
 
+    return execute_function_on_directory_files(MULTITOOL_PLUGINS_DIRECTORY, _func, glob="[!.][!__]*")
+
 
-def pull_all():
+def update_plugin_repositories():
     def _func(path):
-        if not is_dir(path):
+        if not is_directory(path):
             return
-        console.echo(f'Updating {Path(path).stem}... ', end='', flush=True)
+        console.echo(f"Updating {Path(path).stem}... ", line_ending="", should_flush=True)
         repo = Repo(path)
         if repo.bare:
             return
         try:
-            repo.remotes['origin'].pull()
-            console.echo('Done')
+            repo.remotes["origin"].pull()
+            console.echo("Done")
         except Exception as e:
             console.echo(e)
 
-    return run_func_on_dir_files(MULTITOOL_PLUGINS_DIRECTORY, _func, glob='[!.][!__]*')
+    return execute_function_on_directory_files(MULTITOOL_PLUGINS_DIRECTORY, _func, glob="[!.][!__]*")
 
 
-@plugins.command(help='Edit config file manually.')
+@click.group(help=plugins_command_help)
+def plugins():
+    pass
+
+
+@plugins.command(help="Edit config file manually.")
 @common_silent_options
 @common_verbose_options
 @click.option(
-    '-a/-A',
-    '--apply-changes/--no-apply-changes',
+    "-a/-A",
+    "--apply-changes/--no-apply-changes",
     default=False,
-    help='Install plugins from new sources after exiting the editor.',
+    help="Install plugins from new sources after exiting the editor.",
     show_default=True,
 )
 def configure(silent, verbose, apply_changes):
-    exit_if_git_not_installed()
-    init()
+    exit_quietly_if_git_not_installed()
+    initialize_MULTITOOL_plugins()
     click.edit(filename=MULTITOOL_PLUGINS_CONFIG_FILE)
     if apply_changes:
-        clone_all()
-        prune_all()
+        clone_plugin_repositories()
+        prune_unused_plugin_directories()
     else:
-        console.echo('\n  Run `multitool plugins update` to apply any changes,')
-        console.echo('    or rerun `multitool plugins configure` with `-a`')
-        console.echo('    to apply changes automatically.\n')
+        console.echo("\n  Run `apigee plugins update` to apply any changes,")
+        console.echo("    or rerun `apigee plugins configure` with `-a`")
+        console.echo("    to apply changes automatically.\n")
 
 
-def install():
-    pass
-
-
-@plugins.command(help='Update or install plugins.')
+@plugins.command(help="Update or install plugins.")
 @common_silent_options
 @common_verbose_options
-def update(silent, verbose, section='sources'):
-    exit_if_git_not_installed()
-    clone_all()
-    pull_all()
+def update(silent, verbose, section="sources"):
+    exit_quietly_if_git_not_installed()
+    clone_plugin_repositories()
+    update_plugin_repositories()
 
 
-@plugins.command(help='Show plugins information.')
+@plugins.command(help="Show plugins information.")
 @common_silent_options
 @common_verbose_options
-@click.option('-n', '--name', help='name of the plugins package')
-@optgroup.group('Filter options', cls=MutuallyExclusiveOptionGroup, help='The filter options')
+@click.option("-n", "--name", help="name of the plugins package")
+@optgroup.group(
+    "Filter options", cls=MutuallyExclusiveOptionGroup, help="The filter options"
+)
 @optgroup.option(
-    '--show-commit-only/--no-show-commit-only',
+    "--show-commit-only/--no-show-commit-only",
     default=False,
-    help='only print latest Git commit log',
+    help="only print latest Git commit log",
 )
 @optgroup.option(
-    '--show-dependencies-only/--no-show-dependencies-only',
+    "--show-dependencies-only/--no-show-dependencies-only",
     default=False,
-    help='only print list of required packages',
+    help="only print list of required packages",
 )
 def show(
-    silent, verbose, name, section='sources', show_commit_only=False, show_dependencies_only=False
+    silent,
+    verbose,
+    name,
+    section="sources",
+    show_commit_only=False,
+    show_dependencies_only=False,
 ):
     if not name:
-        config = load_config()
+        config = load_plugin_config()
         if not config._sections:
             return
         sources = dict(config._sections[section])
         for name, uri in sources.items():
-            console.echo(f'{name}: {uri}')
+            console.echo(f"{name}: {uri}")
         return
-    plugins_info_file = Path(MULTITOOL_PLUGINS_DIRECTORY) / name / 'multitool-info.json'
-    if not is_file(plugins_info_file):
+    plugins_info_file = Path(MULTITOOL_PLUGINS_DIRECTORY) / name / "apigee-cli.info"
+    if not is_regular_file(plugins_info_file):
         return
-    plugins_info = read_file(plugins_info_file, type='json')
+    plugins_info = read_file_content(plugins_info_file, type="json")
     if show_commit_only:
-        exit_if_git_not_installed()
+        exit_quietly_if_git_not_installed()
         console.echo(
             Repo(Path(MULTITOOL_PLUGINS_DIRECTORY) / name).git.log(
-                '--pretty=format:%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset',
-                '-1',
+                "--pretty=format:%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset",
+                "-1",
             )
         )
         return
     if show_dependencies_only:
-        if plugins_info.get('Requires'):
-            console.echo(plugins_info.get('Requires'))
+        if plugins_info.get("Requires"):
+            console.echo(plugins_info.get("Requires"))
         return
     for k, v in plugins_info.items():
-        console.echo(f'{k}: {v}')
-
-
-def info():
-    pass
-
-
-def chmod_directory(directory, mode):
-    """https://stackoverflow.com/a/58878271"""
-    for root, dirs, files in os.walk(directory):
-        for dir in dirs:
-            os.chmod(path.join(root, dir), mode)
-        for file in files:
-            os.chmod(path.join(root, file), mode)
-
+        console.echo(f"{k}: {v}")
 
-def prune_all(section='sources'):
-    init()
-    config = load_config()
-    if not config._sections:
-        return
-    sources = dict(config._sections[section])
 
-    def _func(path):
-        if not is_dir(path):
-            return
-        name = Path(path).stem
-        if name in sources.keys():
-            return
-        console.echo(f'Removing {name}... ', end='', flush=True)
-        plugin_directory = Path(MULTITOOL_PLUGINS_DIRECTORY) / name
-        try:
-            chmod_directory(str(Path(plugin_directory) / '.git'), stat.S_IRWXU)
-            shutil.rmtree(plugin_directory)
-            console.echo('Done')
-        except Exception as e:
-            console.echo(e)
-
-    return run_func_on_dir_files(MULTITOOL_PLUGINS_DIRECTORY, _func, glob='[!.][!__]*')
-
-
-@plugins.command(help='Prune plugins with removed sources.')
+@plugins.command(help="Prune plugins with removed sources.")
 @common_silent_options
 @common_verbose_options
-def prune(silent, verbose, section='sources'):
-    exit_if_git_not_installed()
-    prune_all()
-
-
-def uninstall():
-    pass
-
-
-def clean():
-    pass
+def prune(silent, verbose, section="sources"):
+    exit_quietly_if_git_not_installed()
+    prune_unused_plugin_directories()
```

### Comparing `multitool-0.3.2/multitool/utils.py` & `multitool-0.4.0/multitool/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,120 +6,124 @@
 import re
 import sys
 from pathlib import Path
 
 import click
 
 
-def gen_path_str(*args):
-    if not args:
-        return
-    path = None
-    for arg in args:
-        if not path:
-            path = Path(arg)
-        else:
-            path /= arg
-    return str(path)
+def apply_function_on_iterable(iterable, func, state_op="append", args=(), kwargs=None):
+    if kwargs is None:
+        kwargs = {}
+    state = []
+    for item in iterable:
+        _tuple = (item,)
+        result = func(*(_tuple + args), **kwargs)
+        if result:
+            getattr(state, state_op)(result)
+    return state
 
 
-def is_dir(d):
-    return os.path.isdir(d)
+def configure_global_logger(log_file):
+    create_empty_file(log_file)
+    remove_file_if_above_size(log_file, size_kb=1000)
+    logging.basicConfig(
+        filename=log_file,
+        level=logging.WARNING,
+        format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+    )
 
 
-def is_envvar_true(value):
-    return value in (True, 'True', 'true', '1')
+def create_empty_file(path):
+    try:
+        create_directory(os.path.split(path)[0])
+        if not os.path.exists(path):
+            with open(path, "x"):
+                os.utime(path, None)
+    except FileExistsError:
+        logging.warning(f"{inspect.stack()[0][3]}; will ignore FileExistsError")
 
 
-def is_file(f):
-    return os.path.isfile(f)
+def create_directory(path):
+    if not path:
+        return
+    if not os.path.exists(path):
+        try:
+            os.makedirs(path)
+        except FileExistsError:
+            logging.warning(f"{inspect.stack()[0][3]}; will ignore FileExistsError")
+
 
+def execute_function_on_directory_files(dir, func, glob="**/*", args=(), kwargs=None):
+    if kwargs is None:
+        kwargs = {}
+    state = []
+    for file_path in Path(get_resolved_directory_path(dir)).resolve().glob(glob):
+        _tuple = (str(file_path),)
+        result = func(*(_tuple + args), **kwargs)
+        if result:
+            state.append(result)
+    return state
 
-def import_all_modules_in_directory(plugins_init_file, existing_commands):
+
+def get_resolved_directory_path(target_directory=None):
+    if target_directory:
+        if not os.path.exists(target_directory):
+            os.makedirs(target_directory)
+        return str(Path(target_directory).resolve())
+    return os.getcwd()
+
+
+def import_plugins_from_directory(plugins_init_file, existing_commands):
     try:
         spec = importlib.util.spec_from_file_location('plugins_modules', plugins_init_file)
         module = importlib.util.module_from_spec(spec)
         sys.modules[spec.name] = module
         spec.loader.exec_module(module)
-        import plugins_modules
-        from plugins_modules import __all__ as all_plugins_modules
+        import plugins_modules # type: ignore
+        from plugins_modules import __all__ as all_plugins_modules # type: ignore
 
         for module in all_plugins_modules:
             _module = getattr(plugins_modules, module)
             if isinstance(_module, (click.core.Command, click.core.Group)):
                 existing_commands.add(_module)
     except ImportError:
         logging.warning(
             f'{inspect.stack()[0][3]}; will skip loading plugin: {module}', exc_info=True
         )
 
 
-def make_dirs(path):
-    if not os.path.exists(path):
-        try:
-            os.makedirs(path)
-        except FileExistsError:
-            logging.warning(f'{inspect.stack()[0][3]}; will ignore FileExistsError')
+def is_directory(d):
+    return os.path.isdir(d)
 
 
-def read_file(file, type='text'):
-    with open(file, 'r') as f:
-        if type == 'json':
-            return json.loads(f.read())
-        return f.read()
+def is_regular_file(f):
+    return os.path.isfile(f)
 
 
-def remove_file_above_size(file, size_kb=100):
-    if os.path.getsize(file) > size_kb * 1024:
-        os.remove(file)
+def is_truthy_envvar(value):
+    return value in (True, "True", "true", "1")
 
 
-def resolve_target_directory(target_directory=None):
-    if target_directory:
-        if not os.path.exists(target_directory):
-            os.makedirs(target_directory)
-        return str(Path(target_directory).resolve())
-    return os.getcwd()
-
-
-def run_func_on_dir_files(dir, func, glob='**/*', args=(), kwargs={}):
-    state = []
-    for file_path in Path(resolve_target_directory(dir)).resolve().glob(glob):
-        _tuple = (str(file_path),)
-        result = func(*(_tuple + args), **kwargs)
-        if result:
-            state.append(result)
-    return state
+def join_path_components(*components):
+    if not components:
+        return
+    path = None
+    for component in components:
+        if not path:
+            path = Path(component)
+        else:
+            path /= component
+    return str(path)
 
 
-def run_func_on_iterable(iterable, func, state_op='append', args=(), kwargs={}):
-    state = []
-    for item in iterable:
-        _tuple = (item,)
-        result = func(*(_tuple + args), **kwargs)
-        if result:
-            getattr(state, state_op)(result)
-    return state
+def read_file_content(file, type="text"):
+    with open(file, "r") as f:
+        return json.loads(f.read()) if type == "json" else f.read()
 
 
-def setup_global_logger(log_file):
-    touch(log_file)
-    logging.basicConfig(
-        filename=log_file,
-        level=logging.DEBUG,
-        format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
-    )
-    remove_file_above_size(log_file, size_kb=1000)
+def remove_file_if_above_size(file, size_kb=100):
+    if os.path.getsize(file) > size_kb * 1024:
+        os.remove(file)
 
 
 def show_message(msg):
     print(msg)
-
-
-def touch(path):
-    try:
-        make_dirs(os.path.split(path)[0])
-        if not os.path.exists(path):
-            with open(path, 'x'):
-                os.utime(path, None)
-    except FileExistsError:
-        logging.warning(f'{inspect.stack()[0][3]}; will ignore FileExistsError')
```

### Comparing `multitool-0.3.2/multitool/verbose.py` & `multitool-0.4.0/multitool/verbose.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import builtins
 import http.client as http_client
 import logging
 
 import click
-import requests
 
 
 def verbose_callback(ctx, param, value):
     builtins.MULTITOOL_TOGGLE_VERBOSE = value
     http_client.HTTPConnection.debuglevel = value
     logging.basicConfig()
     logging.getLogger().setLevel(logging.DEBUG)
```

### Comparing `multitool-0.3.2/multitool.egg-info/PKG-INFO` & `multitool-0.4.0/multitool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: multitool
-Version: 0.3.2
+Version: 0.4.0
 Summary: General-purpose command-line interface with plugins support
 Home-page: https://github.com/mdelotavo/multitool
 Author: Matthew Delotavo
 Author-email: matthew.t.delotavo@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 multitool
 =========
 
 Multitool is a general-purpose command-line interface with plugins support.
 
@@ -167,9 +166,7 @@
 
         deactivate
 
 .. _`click`: https://click.palletsprojects.com/
 .. _`apigeecli`: https://pypi.org/project/apigeecli/
 .. _`multitool-plugins`: https://github.com/mdelotavo/multitool-plugins
 .. _`public plugins repository`: https://github.com/mdelotavo/multitool-plugins
-
-
```

### Comparing `multitool-0.3.2/setup.py` & `multitool-0.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, sys, re
+import os
 
 from multitool import APP
 from multitool import __version__ as version
 from multitool import description
 
 readme = os.path.join(os.path.dirname(__file__), 'README.rst')
 long_description = open(readme).read()
@@ -21,35 +21,33 @@
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.7',
     ],
-    # py_modules = ['multitool',],
-    # entry_points='''
-    #     [console_scripts]
-    #     multitool=multitool.__main__:cli
-    # ''',
-    entry_points={'console_scripts': ['multitool=multitool.__main__:main']},
+    entry_points = {
+        'console_scripts': [
+            'multitool=multitool.__main__:main'
+        ]
+    },
     install_requires = [
-        'requests>=2.22',
-        'click',
-        'click-aliases',
-        'click-option-group',
-        'colorama',
-        'pyotp',
-        'requests',
-        'tqdm',
-        'tabulate',
-        'pyjwt',
-        'python-gnupg>=0.3.5',
-        'gitpython'
+        'requests>=2.28.1',
+        'click>=8.1.3',
+        'click-aliases>=1.0.1',
+        'click-option-group>=0.5.5',
+        'colorama>=0.4.6',
+        'pyotp>=2.8.0',
+        'tqdm>=4.64.1',
+        'tabulate>=0.9.0',
+        'pyjwt>=2.6.0',
+        'python-gnupg>=0.4.9',
+        'gitpython>=3.1.30'
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
 
 if __name__ == '__main__':
     from setuptools import setup, find_packages
 
     SETUP_ARGS['packages'] = find_packages()
     setup(**SETUP_ARGS)
```

