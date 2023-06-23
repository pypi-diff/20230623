# Comparing `tmp/arguably-1.2.3.tar.gz` & `tmp/arguably-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguably-1.2.3.tar", max compression
+gzip compressed data, was "arguably-1.2.4.tar", max compression
```

## Comparing `arguably-1.2.3.tar` & `arguably-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1538 2023-06-20 11:10:02.947449 arguably-1.2.3/LICENSE.txt
--rw-r--r--   0        0        0     2445 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/__init__.py
--rw-r--r--   0        0        0     2291 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/__main__.py
--rw-r--r--   0        0        0    14402 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/_argparse_extensions.py
--rw-r--r--   0        0        0    16658 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/_commands.py
--rw-r--r--   0        0        0    40489 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/_context.py
--rw-r--r--   0        0        0     5815 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/_modifiers.py
--rw-r--r--   0        0        0    17310 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/_util.py
--rw-r--r--   0        0        0     6836 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/arg.py
--rw-r--r--   0        0        0        0 2023-06-20 11:10:02.947449 arguably-1.2.3/arguably/py.typed
--rw-r--r--   0        0        0     6832 2023-06-20 11:10:02.947449 arguably-1.2.3/etc/pypi/PYPI_README.md
--rw-r--r--   0        0        0     1129 2023-06-20 11:10:02.951449 arguably-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     7589 1970-01-01 00:00:00.000000 arguably-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-06-23 09:24:29.956304 arguably-1.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     2445 2023-06-23 09:24:29.956304 arguably-1.2.4/arguably/__init__.py
+-rw-r--r--   0        0        0     2291 2023-06-23 09:24:29.956304 arguably-1.2.4/arguably/__main__.py
+-rw-r--r--   0        0        0    14402 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_argparse_extensions.py
+-rw-r--r--   0        0        0    16936 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_commands.py
+-rw-r--r--   0        0        0    40492 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_context.py
+-rw-r--r--   0        0        0     5815 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_modifiers.py
+-rw-r--r--   0        0        0    17310 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/_util.py
+-rw-r--r--   0        0        0     6839 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/arg.py
+-rw-r--r--   0        0        0        0 2023-06-23 09:24:29.960305 arguably-1.2.4/arguably/py.typed
+-rw-r--r--   0        0        0     7143 2023-06-23 09:24:29.960305 arguably-1.2.4/etc/pypi/PYPI_README.md
+-rw-r--r--   0        0        0     1129 2023-06-23 09:24:29.960305 arguably-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7900 1970-01-01 00:00:00.000000 arguably-1.2.4/PKG-INFO
```

### Comparing `arguably-1.2.3/LICENSE.txt` & `arguably-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arguably-1.2.3/arguably/__init__.py` & `arguably-1.2.4/arguably/__init__.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.3/arguably/__main__.py` & `arguably-1.2.4/arguably/__main__.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.3/arguably/_argparse_extensions.py` & `arguably-1.2.4/arguably/_argparse_extensions.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.3/arguably/_commands.py` & `arguably-1.2.4/arguably/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,16 +378,20 @@
             elif arg.input_method.is_positional and arg.is_variadic:
                 args.extend(filtered_args[arg.cli_arg_name])
             else:
                 kwargs[arg.func_arg_name] = filtered_args[arg.cli_arg_name]
 
         # Call the function
         if util.is_async_callable(self.function):
+            util.log_args(
+                util.logger.debug, f"Calling {self.name} function async: ", self.function.__name__, *args, **kwargs
+            )
             return asyncio.get_event_loop().run_until_complete(self.function(*args, **kwargs))
         else:
+            util.log_args(util.logger.debug, f"Calling {self.name} function: ", self.function.__name__, *args, **kwargs)
             return self.function(*args, **kwargs)
 
     def get_subcommand_metavar(self, command_metavar: str) -> str:
         """If this command has a subparser (for subcommands of its own), this can be called to generate a unique name
         for the subparser's command metavar"""
         if self.name == "__root__":
             return command_metavar
```

### Comparing `arguably-1.2.3/arguably/_context.py` & `arguably-1.2.4/arguably/_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,15 +506,15 @@
 
         Returns:
             The return value from the called function.
 
         Examples:
             ```python
             #!/usr/bin/env python3
-            \"\"\"description for this script'''
+            \"\"\"description for this script\"\"\"
             from io import StringIO
 
             import arguably
 
             __version__ = "1.2.3"
 
             @arguably.command
```

### Comparing `arguably-1.2.3/arguably/_modifiers.py` & `arguably-1.2.4/arguably/_modifiers.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.3/arguably/_util.py` & `arguably-1.2.4/arguably/_util.py`

 * *Files identical despite different names*

### Comparing `arguably-1.2.3/arguably/arg.py` & `arguably-1.2.4/arguably/arg.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         import arguably
         from typing import Annotated
 
         @arguably.command
         def move(
             direction: Annotated[str, arguably.arg.choices("left", "right", "up", "down")]
         ):
-            \"\"\"An enum is usually recommended for cases like this'''
+            \"\"\"An enum is usually recommended for cases like this\"\"\"
             print(f"{direction=}")
 
         if __name__ == "__main__":
             arguably.run()
         ```
 
         ```console
```

### Comparing `arguably-1.2.3/etc/pypi/PYPI_README.md` & `arguably-1.2.4/etc/pypi/PYPI_README.md`

 * *Files 6% similar despite different names*

```diff
@@ -99,36 +99,40 @@
 Don't want to write any code? Simply pass any Python script to `arguably` to give it a command line interface.
 
 <div align="right"><sub>
     <a href="https://github.com/treykeown/arguably/blob/main/etc/scripts/party-trick.py">[source]</a>
 </sub></div>
 
 ```console
-user@machine:~$ python3 -m arguably party-trick.py
-usage: party-trick [-h] command ...
+user@machine:~$ python3 -m arguably party-trick.py -h
+usage: party-trick [-h] [--version] command ...
+
+this is the docstring for the whole script
 
 positional arguments:
   command
-    hello                this is the docstring for a function in the script
-    goodbye              any function from a script can be called
-    a-class              so can any __init__ for objects defined in the script
-    a-class.func-static  a @staticmethod on a class can be called
-    a-class.func-cls     so can a @classmethod
+    hello                   this is hello's docstring
+    goodbye                 any function from a script can be called
+    some-class              so can any __init__ for objects defined in the script
+    some-class.func-static  a @staticmethod on a class can be called
+    some-class.func-cls     so can a @classmethod
 
 options:
-  -h, --help             show this help message and exit
+  -h, --help                show this help message and exit
+  --version                 show program's version number and exit
 ```
 
 ## Installation
 
 Install using `pip install arguably`. If you want to install using `conda`, please comment on
 [this issue](https://github.com/treykeown/arguably/issues/12).
 
 ## Documentation
 
+* Why arguably?: [https://treykeown.github.io/arguably/why/](https://treykeown.github.io/arguably/why/)
 * Examples: [https://treykeown.github.io/arguably/examples/](https://treykeown.github.io/arguably/examples/)
 * Tutorial: [https://treykeown.github.io/arguably/tutorial/intro/](https://treykeown.github.io/arguably/tutorial/intro/)
 * API Reference: [https://treykeown.github.io/arguably/api-reference/](https://treykeown.github.io/arguably/api-reference/)
 
 ## Dependencies
 
 All of `arguably` is built on top of `argparse`. It has two dependencies:
@@ -146,8 +150,9 @@
 ## Future roadmap
 
 If you have any interest in these (either as a user or implementer), please leave a comment!
 
 * [#8 - Display all enum options in a command group](https://github.com/treykeown/arguably/issues/8)
 * [#9 - Both positive and negative boolean flags](https://github.com/treykeown/arguably/issues/9)
 * [#10 - Take inputs from environment variables](https://github.com/treykeown/arguably/issues/10)
-* [#13 - Load configuration for a script via a `.yml`](https://github.com/treykeown/arguably/issues/13)
+* [#13 - Implement config interface](https://github.com/treykeown/arguably/issues/13)
+* [#16 - Integration with rich for formatted CLI output](https://github.com/treykeown/arguably/issues/16)
```

### Comparing `arguably-1.2.3/pyproject.toml` & `arguably-1.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arguably"
-version = "1.2.3"
+version = "1.2.4"
 description = "The best Python CLI library, arguably."
 authors = ["treykeown <2755914+treykeown@users.noreply.github.com>"]
 readme = "etc/pypi/PYPI_README.md"
 homepage = "https://treykeown.github.io/arguably/"
 repository = "https://github.com/treykeown/arguably"
 
 [tool.poetry.dependencies]
```

### Comparing `arguably-1.2.3/PKG-INFO` & `arguably-1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arguably
-Version: 1.2.3
+Version: 1.2.4
 Summary: The best Python CLI library, arguably.
 Home-page: https://treykeown.github.io/arguably/
 Author: treykeown
 Author-email: 2755914+treykeown@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -117,36 +117,40 @@
 Don't want to write any code? Simply pass any Python script to `arguably` to give it a command line interface.
 
 <div align="right"><sub>
     <a href="https://github.com/treykeown/arguably/blob/main/etc/scripts/party-trick.py">[source]</a>
 </sub></div>
 
 ```console
-user@machine:~$ python3 -m arguably party-trick.py
-usage: party-trick [-h] command ...
+user@machine:~$ python3 -m arguably party-trick.py -h
+usage: party-trick [-h] [--version] command ...
+
+this is the docstring for the whole script
 
 positional arguments:
   command
-    hello                this is the docstring for a function in the script
-    goodbye              any function from a script can be called
-    a-class              so can any __init__ for objects defined in the script
-    a-class.func-static  a @staticmethod on a class can be called
-    a-class.func-cls     so can a @classmethod
+    hello                   this is hello's docstring
+    goodbye                 any function from a script can be called
+    some-class              so can any __init__ for objects defined in the script
+    some-class.func-static  a @staticmethod on a class can be called
+    some-class.func-cls     so can a @classmethod
 
 options:
-  -h, --help             show this help message and exit
+  -h, --help                show this help message and exit
+  --version                 show program's version number and exit
 ```
 
 ## Installation
 
 Install using `pip install arguably`. If you want to install using `conda`, please comment on
 [this issue](https://github.com/treykeown/arguably/issues/12).
 
 ## Documentation
 
+* Why arguably?: [https://treykeown.github.io/arguably/why/](https://treykeown.github.io/arguably/why/)
 * Examples: [https://treykeown.github.io/arguably/examples/](https://treykeown.github.io/arguably/examples/)
 * Tutorial: [https://treykeown.github.io/arguably/tutorial/intro/](https://treykeown.github.io/arguably/tutorial/intro/)
 * API Reference: [https://treykeown.github.io/arguably/api-reference/](https://treykeown.github.io/arguably/api-reference/)
 
 ## Dependencies
 
 All of `arguably` is built on top of `argparse`. It has two dependencies:
@@ -164,9 +168,10 @@
 ## Future roadmap
 
 If you have any interest in these (either as a user or implementer), please leave a comment!
 
 * [#8 - Display all enum options in a command group](https://github.com/treykeown/arguably/issues/8)
 * [#9 - Both positive and negative boolean flags](https://github.com/treykeown/arguably/issues/9)
 * [#10 - Take inputs from environment variables](https://github.com/treykeown/arguably/issues/10)
-* [#13 - Load configuration for a script via a `.yml`](https://github.com/treykeown/arguably/issues/13)
+* [#13 - Implement config interface](https://github.com/treykeown/arguably/issues/13)
+* [#16 - Integration with rich for formatted CLI output](https://github.com/treykeown/arguably/issues/16)
```

