# Comparing `tmp/clidir-0.1.1.tar.gz` & `tmp/clidir-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidir-0.1.1.tar", last modified: Tue Jun 20 14:25:36 2023, max compression
+gzip compressed data, was "clidir-0.1.2.tar", last modified: Fri Jun 23 21:36:22 2023, max compression
```

## Comparing `clidir-0.1.1.tar` & `clidir-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:25:36.538418 clidir-0.1.1/
--rw-r--r--   0 isaacb     (502) staff       (20)     1079 2023-06-20 13:58:56.000000 clidir-0.1.1/LICENSE
--rw-r--r--   0 isaacb     (502) staff       (20)     2464 2023-06-20 14:25:36.538287 clidir-0.1.1/PKG-INFO
--rw-r--r--   0 isaacb     (502) staff       (20)     2019 2023-06-20 14:19:57.000000 clidir-0.1.1/README.md
--rw-r--r--   0 isaacb     (502) staff       (20)      523 2023-06-20 14:24:36.000000 clidir-0.1.1/pyproject.toml
--rw-r--r--   0 isaacb     (502) staff       (20)       38 2023-06-20 14:25:36.538463 clidir-0.1.1/setup.cfg
-drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:25:36.537458 clidir-0.1.1/src/
--rw-r--r--   0 isaacb     (502) staff       (20)        0 2023-06-20 13:58:56.000000 clidir-0.1.1/src/__init__.py
--rw-r--r--   0 isaacb     (502) staff       (20)      603 2023-06-20 13:58:56.000000 clidir-0.1.1/src/arg_parser.py
-drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:25:36.538071 clidir-0.1.1/src/clidir.egg-info/
--rw-r--r--   0 isaacb     (502) staff       (20)     2464 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/PKG-INFO
--rw-r--r--   0 isaacb     (502) staff       (20)      250 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/SOURCES.txt
--rw-r--r--   0 isaacb     (502) staff       (20)        1 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/dependency_links.txt
--rw-r--r--   0 isaacb     (502) staff       (20)       47 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/top_level.txt
--rw-r--r--   0 isaacb     (502) staff       (20)      830 2023-06-20 13:58:56.000000 clidir-0.1.1/src/clidir.py
--rw-r--r--   0 isaacb     (502) staff       (20)      511 2023-06-20 13:58:56.000000 clidir-0.1.1/src/command_loader.py
--rw-r--r--   0 isaacb     (502) staff       (20)     1024 2023-06-20 13:58:56.000000 clidir-0.1.1/src/help.py
+drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-23 21:36:22.542893 clidir-0.1.2/
+-rw-r--r--   0 isaacb     (502) staff       (20)     1079 2023-06-20 13:58:56.000000 clidir-0.1.2/LICENSE
+-rw-r--r--   0 isaacb     (502) staff       (20)     3058 2023-06-23 21:36:22.542782 clidir-0.1.2/PKG-INFO
+-rw-r--r--   0 isaacb     (502) staff       (20)     2592 2023-06-23 21:35:51.000000 clidir-0.1.2/README.md
+-rw-r--r--   0 isaacb     (502) staff       (20)      672 2023-06-23 21:35:51.000000 clidir-0.1.2/pyproject.toml
+-rw-r--r--   0 isaacb     (502) staff       (20)       38 2023-06-23 21:36:22.542991 clidir-0.1.2/setup.cfg
+drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-23 21:36:22.541529 clidir-0.1.2/src/
+-rw-r--r--   0 isaacb     (502) staff       (20)        0 2023-06-20 13:58:56.000000 clidir-0.1.2/src/__init__.py
+-rw-r--r--   0 isaacb     (502) staff       (20)      684 2023-06-23 19:35:40.000000 clidir-0.1.2/src/arg_parser.py
+drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-23 21:36:22.542338 clidir-0.1.2/src/clidir.egg-info/
+-rw-r--r--   0 isaacb     (502) staff       (20)     3058 2023-06-23 21:36:22.000000 clidir-0.1.2/src/clidir.egg-info/PKG-INFO
+-rw-r--r--   0 isaacb     (502) staff       (20)      304 2023-06-23 21:36:22.000000 clidir-0.1.2/src/clidir.egg-info/SOURCES.txt
+-rw-r--r--   0 isaacb     (502) staff       (20)        1 2023-06-23 21:36:22.000000 clidir-0.1.2/src/clidir.egg-info/dependency_links.txt
+-rw-r--r--   0 isaacb     (502) staff       (20)       15 2023-06-23 21:36:22.000000 clidir-0.1.2/src/clidir.egg-info/requires.txt
+-rw-r--r--   0 isaacb     (502) staff       (20)       47 2023-06-23 21:36:22.000000 clidir-0.1.2/src/clidir.egg-info/top_level.txt
+-rw-r--r--   0 isaacb     (502) staff       (20)      867 2023-06-23 19:35:40.000000 clidir-0.1.2/src/clidir.py
+-rw-r--r--   0 isaacb     (502) staff       (20)      532 2023-06-23 19:35:40.000000 clidir-0.1.2/src/command_loader.py
+-rw-r--r--   0 isaacb     (502) staff       (20)     1058 2023-06-23 19:35:40.000000 clidir-0.1.2/src/help.py
+drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-23 21:36:22.542479 clidir-0.1.2/tests/
+-rw-r--r--   0 isaacb     (502) staff       (20)     1518 2023-06-22 17:32:48.000000 clidir-0.1.2/tests/test_clidir.py
```

### Comparing `clidir-0.1.1/LICENSE` & `clidir-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clidir-0.1.1/PKG-INFO` & `clidir-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: clidir
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tiny Python library to easily create CLI applications with sub commands
 Author: Isaac Benitez
 Project-URL: Homepage, https://github.com/isacben/clidir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # clidir
 
+[![PyPI](https://img.shields.io/pypi/v/clidir.svg)](https://pypi.org/project/clidir/)
+[![Changelog](https://img.shields.io/github/v/release/isacben/clidir?include_prereleases&label=changelog)](https://github.com/isacben/clidir/releases)
+[![Tests](https://github.com/isacben/clidir/workflows/Test/badge.svg)](https://github.com/isacben/clidir/actions?query=workflow%3ATest)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/isacben/clidir/blob/master/LICENSE)
+
 Create CLI applications with sub commands easily.
 
 ## Description
 
 Even simple CLI applications usually require sub commands. For example, `git` has `git remote add`, where *remote* and *add* are sub commands. Doing this with `argparse` or even with more developer friendly libraries can be challenging.
 
 Keeping the commands source code organized in the project can also be complicated.
@@ -49,24 +55,28 @@
 
 Install this tool using `pip`:
 
 ```
 pip install clidir
 ```
 
+## Examples
+
+* [Hello World](https://github.com/isacben/clidir-hello-world)
+
 ## Usage
 
 1. Create a `main.py` file with the following code:
 
 ```python
 import sys
 import clidir
 
 def main() -> int:
-    args = sys.argv[1:]
+    args = sys.argv
     clidir.run(args)
     
     return 0
 
 if __name__ == "__main__":
     exit(main())
 ```
```

### Comparing `clidir-0.1.1/pyproject.toml` & `clidir-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clidir"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Isaac Benitez"},
 ]
 description = "A tiny Python library to easily create CLI applications with sub commands"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[project.optional-dependencies]
+test = [
+    "pytest",
+]
+
 [project.urls]
-"Homepage" = "https://github.com/isacben/clidir"
+"Homepage" = "https://github.com/isacben/clidir"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra"
+testpaths = [
+    "tests",
+]
```

### Comparing `clidir-0.1.1/src/arg_parser.py` & `clidir-0.1.2/src/arg_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-def parse(args: list[str], command_files: list[str]) -> list[str]:
+import os
+
+from typing import List
+
+def parse(args: List[str], command_files: List[str]) -> List[str]:
     
     command_path_arg = ""
     args_start = 0
 
     for arg_position in range(len(args)):
 
         path = "./commands/" + '/'.join(args[:arg_position + 1])
 
         if path + ".py" in command_files:
             command_path_arg = path + '.py'
             args_start = arg_position + 1
             break
 
         elif any(path in substring for substring in command_files):
-            command_path_arg = path
-            args_start = arg_position + 1
+            if os.path.exists(path):
+                command_path_arg = path
+                args_start = arg_position + 1
 
         else:
             break
 
     return [command_path_arg] + args[args_start:]
```

### Comparing `clidir-0.1.1/src/clidir.egg-info/PKG-INFO` & `clidir-0.1.2/src/clidir.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: clidir
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tiny Python library to easily create CLI applications with sub commands
 Author: Isaac Benitez
 Project-URL: Homepage, https://github.com/isacben/clidir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # clidir
 
+[![PyPI](https://img.shields.io/pypi/v/clidir.svg)](https://pypi.org/project/clidir/)
+[![Changelog](https://img.shields.io/github/v/release/isacben/clidir?include_prereleases&label=changelog)](https://github.com/isacben/clidir/releases)
+[![Tests](https://github.com/isacben/clidir/workflows/Test/badge.svg)](https://github.com/isacben/clidir/actions?query=workflow%3ATest)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/isacben/clidir/blob/master/LICENSE)
+
 Create CLI applications with sub commands easily.
 
 ## Description
 
 Even simple CLI applications usually require sub commands. For example, `git` has `git remote add`, where *remote* and *add* are sub commands. Doing this with `argparse` or even with more developer friendly libraries can be challenging.
 
 Keeping the commands source code organized in the project can also be complicated.
@@ -49,24 +55,28 @@
 
 Install this tool using `pip`:
 
 ```
 pip install clidir
 ```
 
+## Examples
+
+* [Hello World](https://github.com/isacben/clidir-hello-world)
+
 ## Usage
 
 1. Create a `main.py` file with the following code:
 
 ```python
 import sys
 import clidir
 
 def main() -> int:
-    args = sys.argv[1:]
+    args = sys.argv
     clidir.run(args)
     
     return 0
 
 if __name__ == "__main__":
     exit(main())
 ```
```

### Comparing `clidir-0.1.1/src/clidir.py` & `clidir-0.1.2/src/clidir.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import arg_parser
 import command_loader
 import help
 
 import importlib
 from types import ModuleType
+from typing import List
 
-def run(args: list[str]) -> None:
+def run(args: List[str]) -> None:
 
     command_paths: list = command_loader.commands_lookup()
-    parsed_args: list = arg_parser.parse(args, command_paths)
-    modules: list[ModuleType] = []
+    parsed_args: list = arg_parser.parse(args[1:], command_paths)
+    modules: List[ModuleType] = []
 
     # load all available command modules
     for path in command_paths:
         module_string = path.split('./')[1].replace('/', '.').replace('.py', '')
         modules.append(importlib.import_module(module_string))
 
     if 'py' in parsed_args[0]:
         # convert directory string into the module name
         cmd = parsed_args[0].split('./')[1].replace('/', '.').split('.py')[0]
         for m in modules:
             if m.__name__ == cmd:
                 m.run(parsed_args[1:])
 
     else:
-        help.commands(modules, parsed_args[0])
+        help.commands(args[0], modules, parsed_args[0])
```

### Comparing `clidir-0.1.1/src/help.py` & `clidir-0.1.2/src/help.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from types import ModuleType
+from typing import List
 
-def commands(modules: list[ModuleType], path: str) -> None:
+def commands(app: str, modules: List[ModuleType], path: str) -> None:
     # when no topic is found
     if path == '':
         topic = 'commands'
-        print(f'usage: rapyd [-h] command',end="\n\n")
+        print(f'usage: {app} [-h] command',end="\n\n")
     else:
         # produce format for 'topic': topic1.topic2.topic3
         topic = path.split('./commands/')[1].replace('/', '.')
-        print(f'usage: rapyd {topic.replace(".", " ")} [-h] command',end="\n\n")
+        print(f'usage: {app} {topic.replace(".", " ")} [-h] command',end="\n\n")
     
     print("commands:")
 
     cmd_pointer = "" # this helps print the help for the first command in a sub topic
     for m in modules:
         if topic in m.__name__:
             module_elements = m.__name__.split('.')
```

