# Comparing `tmp/symbex-0.6.tar.gz` & `tmp/symbex-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.6.tar", last modified: Tue Jun 20 22:40:25 2023, max compression
+gzip compressed data, was "symbex-0.7.tar", last modified: Fri Jun 23 03:28:43 2023, max compression
```

## Comparing `symbex-0.6.tar` & `symbex-0.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.602926 symbex-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 22:40:05.000000 symbex-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-20 22:40:25.602926 symbex-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-06-20 22:40:05.000000 symbex-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 22:40:25.602926 symbex-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-20 22:40:05.000000 symbex-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.598926 symbex-0.6/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:05.000000 symbex-0.6/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 22:40:05.000000 symbex-0.6/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-20 22:40:05.000000 symbex-0.6/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-06-20 22:40:05.000000 symbex-0.6/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.602926 symbex-0.6/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 22:40:25.000000 symbex-0.6/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:40:25.602926 symbex-0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-20 22:40:05.000000 symbex-0.6/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-20 22:40:05.000000 symbex-0.6/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-20 22:40:05.000000 symbex-0.6/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 03:28:26.000000 symbex-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-23 03:28:43.516857 symbex-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-06-23 03:28:26.000000 symbex-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 03:28:43.516857 symbex-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-23 03:28:26.000000 symbex-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:26.000000 symbex-0.7/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 03:28:26.000000 symbex-0.7/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-23 03:28:26.000000 symbex-0.7/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-23 03:28:26.000000 symbex-0.7/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_symbols.py
```

### Comparing `symbex-0.6/LICENSE` & `symbex-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.6/PKG-INFO` & `symbex-0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.6
+Version: 0.7
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -26,14 +26,18 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install symbex
 ```
+Or using Homebrew:
+```bash
+brew install simonw/llm/symbex
+```
 ## Usage
 
 `symbex` can search for names of functions and classes that occur at the top level of a Python file.
 
 To search every `.py` file in your current directory and all subdirectories, run like this:
 
 ```bash
@@ -62,18 +66,39 @@
 symbex '*.*'
 ```
 To search within a specific file, pass that file using the `-f` option. You can pass this more than once to search multiple files.
 
 ```bash
 symbex MyClass -f my_file.py
 ```
-To search within a specific directory and all of its subdirectories, use the `-d` option:
+To search within a specific directory and all of its subdirectories, use the `-d/--directory` option:
 ```bash
 symbex Database -d ~/projects/datasette
 ```
+If you know that you want to inspect one or more modules that can be imported by Python, you can use the `-m/--module name` option. This example shows the signatures for every symbol available in the `asyncio` package:
+```bash
+symbex -m asyncio -s --imports
+```
+You can search the directory containing the Python standard library using `--stdlib`. This can be useful for quickly looking up the source code for specific Python library functions:
+```bash
+symbex --stdlib -in to_thread
+```
+`-in` is explained below. If you provide `--stdlib` without any `-d` or `-f` options then `--silent` will be turned on automatically, since the standard library otherwise produces a number of different warnings.
+
+The output starts like this:
+```python
+# from asyncio.threads import to_thread
+async def to_thread(func, /, *args, **kwargs):
+    """Asynchronously run function *func* in a separate thread.
+    # ...
+```
+You can exclude files in specified directories using the `-x/--exclude` option:
+```bash
+symbex Database -d ~/projects/datasette -x ~/projects/datasette/tests
+```
 If `symbex` encounters any Python code that it cannot parse, it will print a warning message and continue searching:
 ```
 # Syntax error in path/badcode.py: expected ':' (<unknown>, line 1)
 ```
 Pass `--silent` to suppress these warnings:
 ```bash
 symbex MyClass --silent
@@ -89,27 +114,28 @@
 - `--async` - only `async def` functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
+- `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
 
 ```bash
 symbex -s --async --untyped
 ```
 
 For class methods instead of functions, you can combine filters with a symbol search argument of `*.*`.
 
-This example shows the full source code of every class method in your project with type annotations on all of the arguments and the return value:
+This example shows the full source code of every class method in the Python standard library that has type annotations for all of the arguments and the return value:
 
 ```bash
-symbex --fully-typed '*.*'
+symbex --fully-typed --no-init '*.*' --stdlib
 ```
 
 ### Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
@@ -137,97 +163,128 @@
             )
         )
 ```
 ### Just the signatures
 
 The `-s/--signatures` option will list just the signatures of the functions and classes, for example:
 ```bash
-symbex -s -d symbex
+symbex -s -f symbex/lib.py
 ```
 <!-- [[[cog
 import cog
 from click.testing import CliRunner
 import pathlib
 from symbex.cli import cli
 
+def sorted_chunks(text):
+    chunks = text.strip().split("\n\n")
+    chunks.sort()
+    return "\n\n".join(chunks)
+
 path = pathlib.Path("symbex").resolve()
 runner = CliRunner()
-result = runner.invoke(cli, ["-s", "-d", str(path)])
-# Need a consistent sort order
-chunks = result.stdout.strip().split("\n\n")
-chunks.sort()
+result = runner.invoke(cli, ["-s", "-f", str(path / "lib.py")])
 cog.out(
-    "```python\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format(sorted_chunks(result.output))
 )
 ]]] -->
 ```python
-# File: symbex/cli.py Line: 95
-def cli(symbols, files, directories, signatures, docstrings, count, silent, async_, function, class_, documented, undocumented, typed, untyped, partially_typed, fully_typed)
-
-# File: symbex/lib.py Line: 105
+# File: symbex/lib.py Line: 106
 def function_definition(function_node: AST)
 
-# File: symbex/lib.py Line: 12
+# File: symbex/lib.py Line: 13
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 173
+# File: symbex/lib.py Line: 174
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 207
+# File: symbex/lib.py Line: 208
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 225
+# File: symbex/lib.py Line: 226
 def read_file(path)
 
-# File: symbex/lib.py Line: 251
+# File: symbex/lib.py Line: 252
 class TypeSummary
 
-# File: symbex/lib.py Line: 256
+# File: symbex/lib.py Line: 257
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 302
+# File: symbex/lib.py Line: 303
 def quoted_string(s)
 
-# File: symbex/lib.py Line: 36
+# File: symbex/lib.py Line: 314
+def import_line_for_function(function_name: str, filepath: str, possible_root_dirs: List[str]) -> str
+
+# File: symbex/lib.py Line: 37
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 70
+# File: symbex/lib.py Line: 71
 def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
 
-# File: symbex/lib.py Line: 80
+# File: symbex/lib.py Line: 81
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
-To include docstrings in those signatures, use `--docstrings`:
+To include estimated import paths, such as `# from symbex.lib import match`, use `--imports`. These will be calculated relative to the directory you specified, or you can pass one or more `--sys-path` options to request that imports are calculated relative to those directories as if they were on `sys.path`:
+
 ```bash
-symbex --docstrings --documented -f symbex/lib.py
+~/dev/symbex/symbex match --imports -s --sys-path ~/dev/symbex
 ```
-
+Example output:
 <!-- [[[cog
-runner = CliRunner()
-result = runner.invoke(cli, ["--docstrings", "--documented", "-f", str(path / "lib.py")])
-# Need a consistent sort order
-chunks = result.stdout.strip().split("\n\n")
-chunks.sort()
+result = runner.invoke(cli, [
+    "--imports", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
+])
 cog.out(
-    "```python\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 12
-def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
-    "Returns ast Nodes matching symbols"
+# File: symbex/lib.py Line: 81
+# from symbex.lib import match
+def match(name: str, symbols: Iterable[str]) -> bool
+```
+<!-- [[[end]]] -->
+To suppress the `# File: ...` comments, use `--no-file` or `-n`.
 
-# File: symbex/lib.py Line: 36
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
-    "Returns the code for a given node"
+So to both show import paths and suppress File comments, use `-in` as a shortcut:
+```bash
+symbex -in match
+```
+Output:
+<!-- [[[cog
+result = runner.invoke(cli, [
+    "-in", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
+])
+cog.out(
+    "```python\n{}\n```\n".format(result.stdout.strip())
+)
+]]] -->
+```python
+# from symbex.lib import match
+def match(name: str, symbols: Iterable[str]) -> bool
+```
+<!-- [[[end]]] -->
 
-# File: symbex/lib.py Line: 80
+To include docstrings in those signatures, use `--docstrings`:
+```bash
+symbex match --docstrings -f symbex/lib.py
+```
+Example output:
+<!-- [[[cog
+result = runner.invoke(cli, ["match", "--docstrings", "-f", str(path / "lib.py")])
+cog.out(
+    "```python\n{}\n```\n".format(result.stdout.strip())
+)
+]]] -->
+```python
+# File: symbex/lib.py Line: 81
 def match(name: str, symbols: Iterable[str]) -> bool
     "Returns True if name matches any of the symbols, resolving wildcards"
 ```
 <!-- [[[end]]] -->
 
 ## Counting symbols
 
@@ -260,15 +317,14 @@
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
 
 <!-- [[[cog
-import cog
 result2 = runner.invoke(cli, ["--help"])
 help = result2.output.replace("Usage: cli", "Usage: symbex")
 cog.out(
     "```\n{}\n```".format(help)
 )
 ]]] -->
 ```
@@ -308,27 +364,34 @@
       # Count the number of --async functions in the project
       symbex --async --count
 
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
+  --stdlib                   Search the Python standard library
+  -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
-  --docstrings               Show function and class signatures plus docstrings
+  -n, --no-file              Don't include the # File: comments in the output
+  -i, --imports              Show 'from x import y' lines for imported symbols
+  -m, --module TEXT          Modules to search within
+  --sys-path TEXT            Calculate imports relative to these on sys.path
+  --docs, --docstrings       Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
   --async                    Filter async functions
   --function                 Filter functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
+  --no-init                  Filter to exclude any __init__ methods
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-0.6/README.md` & `symbex-0.7/symbex.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: symbex
+Version: 0.7
+Summary: Find the Python code for specified symbols
+Home-page: https://github.com/simonw/symbex
+Author: Simon Willison
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/simonw/symbex/issues
+Project-URL: CI, https://github.com/simonw/symbex/actions
+Project-URL: Changelog, https://github.com/simonw/symbex/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # symbex
 
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
@@ -11,14 +26,18 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install symbex
 ```
+Or using Homebrew:
+```bash
+brew install simonw/llm/symbex
+```
 ## Usage
 
 `symbex` can search for names of functions and classes that occur at the top level of a Python file.
 
 To search every `.py` file in your current directory and all subdirectories, run like this:
 
 ```bash
@@ -47,18 +66,39 @@
 symbex '*.*'
 ```
 To search within a specific file, pass that file using the `-f` option. You can pass this more than once to search multiple files.
 
 ```bash
 symbex MyClass -f my_file.py
 ```
-To search within a specific directory and all of its subdirectories, use the `-d` option:
+To search within a specific directory and all of its subdirectories, use the `-d/--directory` option:
 ```bash
 symbex Database -d ~/projects/datasette
 ```
+If you know that you want to inspect one or more modules that can be imported by Python, you can use the `-m/--module name` option. This example shows the signatures for every symbol available in the `asyncio` package:
+```bash
+symbex -m asyncio -s --imports
+```
+You can search the directory containing the Python standard library using `--stdlib`. This can be useful for quickly looking up the source code for specific Python library functions:
+```bash
+symbex --stdlib -in to_thread
+```
+`-in` is explained below. If you provide `--stdlib` without any `-d` or `-f` options then `--silent` will be turned on automatically, since the standard library otherwise produces a number of different warnings.
+
+The output starts like this:
+```python
+# from asyncio.threads import to_thread
+async def to_thread(func, /, *args, **kwargs):
+    """Asynchronously run function *func* in a separate thread.
+    # ...
+```
+You can exclude files in specified directories using the `-x/--exclude` option:
+```bash
+symbex Database -d ~/projects/datasette -x ~/projects/datasette/tests
+```
 If `symbex` encounters any Python code that it cannot parse, it will print a warning message and continue searching:
 ```
 # Syntax error in path/badcode.py: expected ':' (<unknown>, line 1)
 ```
 Pass `--silent` to suppress these warnings:
 ```bash
 symbex MyClass --silent
@@ -74,27 +114,28 @@
 - `--async` - only `async def` functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
+- `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
 
 ```bash
 symbex -s --async --untyped
 ```
 
 For class methods instead of functions, you can combine filters with a symbol search argument of `*.*`.
 
-This example shows the full source code of every class method in your project with type annotations on all of the arguments and the return value:
+This example shows the full source code of every class method in the Python standard library that has type annotations for all of the arguments and the return value:
 
 ```bash
-symbex --fully-typed '*.*'
+symbex --fully-typed --no-init '*.*' --stdlib
 ```
 
 ### Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
@@ -122,97 +163,128 @@
             )
         )
 ```
 ### Just the signatures
 
 The `-s/--signatures` option will list just the signatures of the functions and classes, for example:
 ```bash
-symbex -s -d symbex
+symbex -s -f symbex/lib.py
 ```
 <!-- [[[cog
 import cog
 from click.testing import CliRunner
 import pathlib
 from symbex.cli import cli
 
+def sorted_chunks(text):
+    chunks = text.strip().split("\n\n")
+    chunks.sort()
+    return "\n\n".join(chunks)
+
 path = pathlib.Path("symbex").resolve()
 runner = CliRunner()
-result = runner.invoke(cli, ["-s", "-d", str(path)])
-# Need a consistent sort order
-chunks = result.stdout.strip().split("\n\n")
-chunks.sort()
+result = runner.invoke(cli, ["-s", "-f", str(path / "lib.py")])
 cog.out(
-    "```python\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format(sorted_chunks(result.output))
 )
 ]]] -->
 ```python
-# File: symbex/cli.py Line: 95
-def cli(symbols, files, directories, signatures, docstrings, count, silent, async_, function, class_, documented, undocumented, typed, untyped, partially_typed, fully_typed)
-
-# File: symbex/lib.py Line: 105
+# File: symbex/lib.py Line: 106
 def function_definition(function_node: AST)
 
-# File: symbex/lib.py Line: 12
+# File: symbex/lib.py Line: 13
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 173
+# File: symbex/lib.py Line: 174
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 207
+# File: symbex/lib.py Line: 208
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 225
+# File: symbex/lib.py Line: 226
 def read_file(path)
 
-# File: symbex/lib.py Line: 251
+# File: symbex/lib.py Line: 252
 class TypeSummary
 
-# File: symbex/lib.py Line: 256
+# File: symbex/lib.py Line: 257
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 302
+# File: symbex/lib.py Line: 303
 def quoted_string(s)
 
-# File: symbex/lib.py Line: 36
+# File: symbex/lib.py Line: 314
+def import_line_for_function(function_name: str, filepath: str, possible_root_dirs: List[str]) -> str
+
+# File: symbex/lib.py Line: 37
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 70
+# File: symbex/lib.py Line: 71
 def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
 
-# File: symbex/lib.py Line: 80
+# File: symbex/lib.py Line: 81
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
-To include docstrings in those signatures, use `--docstrings`:
+To include estimated import paths, such as `# from symbex.lib import match`, use `--imports`. These will be calculated relative to the directory you specified, or you can pass one or more `--sys-path` options to request that imports are calculated relative to those directories as if they were on `sys.path`:
+
 ```bash
-symbex --docstrings --documented -f symbex/lib.py
+~/dev/symbex/symbex match --imports -s --sys-path ~/dev/symbex
 ```
-
+Example output:
 <!-- [[[cog
-runner = CliRunner()
-result = runner.invoke(cli, ["--docstrings", "--documented", "-f", str(path / "lib.py")])
-# Need a consistent sort order
-chunks = result.stdout.strip().split("\n\n")
-chunks.sort()
+result = runner.invoke(cli, [
+    "--imports", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
+])
 cog.out(
-    "```python\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 12
-def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
-    "Returns ast Nodes matching symbols"
+# File: symbex/lib.py Line: 81
+# from symbex.lib import match
+def match(name: str, symbols: Iterable[str]) -> bool
+```
+<!-- [[[end]]] -->
+To suppress the `# File: ...` comments, use `--no-file` or `-n`.
 
-# File: symbex/lib.py Line: 36
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
-    "Returns the code for a given node"
+So to both show import paths and suppress File comments, use `-in` as a shortcut:
+```bash
+symbex -in match
+```
+Output:
+<!-- [[[cog
+result = runner.invoke(cli, [
+    "-in", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
+])
+cog.out(
+    "```python\n{}\n```\n".format(result.stdout.strip())
+)
+]]] -->
+```python
+# from symbex.lib import match
+def match(name: str, symbols: Iterable[str]) -> bool
+```
+<!-- [[[end]]] -->
 
-# File: symbex/lib.py Line: 80
+To include docstrings in those signatures, use `--docstrings`:
+```bash
+symbex match --docstrings -f symbex/lib.py
+```
+Example output:
+<!-- [[[cog
+result = runner.invoke(cli, ["match", "--docstrings", "-f", str(path / "lib.py")])
+cog.out(
+    "```python\n{}\n```\n".format(result.stdout.strip())
+)
+]]] -->
+```python
+# File: symbex/lib.py Line: 81
 def match(name: str, symbols: Iterable[str]) -> bool
     "Returns True if name matches any of the symbols, resolving wildcards"
 ```
 <!-- [[[end]]] -->
 
 ## Counting symbols
 
@@ -245,15 +317,14 @@
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
 
 <!-- [[[cog
-import cog
 result2 = runner.invoke(cli, ["--help"])
 help = result2.output.replace("Usage: cli", "Usage: symbex")
 cog.out(
     "```\n{}\n```".format(help)
 )
 ]]] -->
 ```
@@ -293,27 +364,34 @@
       # Count the number of --async functions in the project
       symbex --async --count
 
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
+  --stdlib                   Search the Python standard library
+  -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
-  --docstrings               Show function and class signatures plus docstrings
+  -n, --no-file              Don't include the # File: comments in the output
+  -i, --imports              Show 'from x import y' lines for imported symbols
+  -m, --module TEXT          Modules to search within
+  --sys-path TEXT            Calculate imports relative to these on sys.path
+  --docs, --docstrings       Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
   --async                    Filter async functions
   --function                 Filter functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
+  --no-init                  Filter to exclude any __init__ methods
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-0.6/setup.py` & `symbex-0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.6"
+VERSION = "0.7"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-0.6/symbex/lib.py` & `symbex-0.7/symbex/lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import fnmatch
 import ast
 from ast import literal_eval, parse, AST, AsyncFunctionDef, FunctionDef, ClassDef
 import codecs
 from dataclasses import dataclass
 from itertools import zip_longest
+from pathlib import Path
 import re
 import textwrap
 from typing import Iterable, List, Optional, Tuple
 
 
 def find_symbol_nodes(
     code: str, filename: str, symbols: Iterable[str]
@@ -304,7 +305,36 @@
         # Escape triple double quotes
         s = s.replace('"""', '\\"\\"\\"')
         return f'"""{s}"""'
     else:
         # Escape double quotes
         s = s.replace('"', '\\"')
         return f'"{s}"'
+
+
+def import_line_for_function(
+    function_name: str, filepath: str, possible_root_dirs: List[str]
+) -> str:
+    """
+    Returns eg 'from foo.bar import baz' if filepath is /Users/dev/foo/bar.py
+    and function_name is baz and possible_root_dirs is a list that contains
+    /Users/dev
+    """
+    filepath = Path(filepath).resolve()
+    filename_without_extension = filepath.stem
+
+    # Check for matches in possible_root_dirs
+    for root_dir in possible_root_dirs:
+        root_dir = Path(root_dir).resolve()
+        try:
+            relative_path = filepath.relative_to(root_dir)
+            # Convert path separators to dots and assemble import line
+            import_path = ".".join(
+                relative_path.parts[:-1] + (filename_without_extension,)
+            )
+            return f"from {import_path} import {function_name}"
+        except ValueError:
+            # If ValueError is raised, the filepath is not under the root_dir
+            continue
+
+    # If none of the root_dirs matched return a relative import
+    return f"from .{filename_without_extension} import {function_name}"
```

### Comparing `symbex-0.6/symbex.egg-info/PKG-INFO` & `symbex-0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: symbex
-Version: 0.6
-Summary: Find the Python code for specified symbols
-Home-page: https://github.com/simonw/symbex
-Author: Simon Willison
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/simonw/symbex/issues
-Project-URL: CI, https://github.com/simonw/symbex/actions
-Project-URL: Changelog, https://github.com/simonw/symbex/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # symbex
 
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
@@ -26,14 +11,18 @@
 
 ## Installation
 
 Install this tool using `pip`:
 ```bash
 pip install symbex
 ```
+Or using Homebrew:
+```bash
+brew install simonw/llm/symbex
+```
 ## Usage
 
 `symbex` can search for names of functions and classes that occur at the top level of a Python file.
 
 To search every `.py` file in your current directory and all subdirectories, run like this:
 
 ```bash
@@ -62,18 +51,39 @@
 symbex '*.*'
 ```
 To search within a specific file, pass that file using the `-f` option. You can pass this more than once to search multiple files.
 
 ```bash
 symbex MyClass -f my_file.py
 ```
-To search within a specific directory and all of its subdirectories, use the `-d` option:
+To search within a specific directory and all of its subdirectories, use the `-d/--directory` option:
 ```bash
 symbex Database -d ~/projects/datasette
 ```
+If you know that you want to inspect one or more modules that can be imported by Python, you can use the `-m/--module name` option. This example shows the signatures for every symbol available in the `asyncio` package:
+```bash
+symbex -m asyncio -s --imports
+```
+You can search the directory containing the Python standard library using `--stdlib`. This can be useful for quickly looking up the source code for specific Python library functions:
+```bash
+symbex --stdlib -in to_thread
+```
+`-in` is explained below. If you provide `--stdlib` without any `-d` or `-f` options then `--silent` will be turned on automatically, since the standard library otherwise produces a number of different warnings.
+
+The output starts like this:
+```python
+# from asyncio.threads import to_thread
+async def to_thread(func, /, *args, **kwargs):
+    """Asynchronously run function *func* in a separate thread.
+    # ...
+```
+You can exclude files in specified directories using the `-x/--exclude` option:
+```bash
+symbex Database -d ~/projects/datasette -x ~/projects/datasette/tests
+```
 If `symbex` encounters any Python code that it cannot parse, it will print a warning message and continue searching:
 ```
 # Syntax error in path/badcode.py: expected ':' (<unknown>, line 1)
 ```
 Pass `--silent` to suppress these warnings:
 ```bash
 symbex MyClass --silent
@@ -89,27 +99,28 @@
 - `--async` - only `async def` functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
+- `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
 
 ```bash
 symbex -s --async --untyped
 ```
 
 For class methods instead of functions, you can combine filters with a symbol search argument of `*.*`.
 
-This example shows the full source code of every class method in your project with type annotations on all of the arguments and the return value:
+This example shows the full source code of every class method in the Python standard library that has type annotations for all of the arguments and the return value:
 
 ```bash
-symbex --fully-typed '*.*'
+symbex --fully-typed --no-init '*.*' --stdlib
 ```
 
 ### Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
@@ -137,97 +148,128 @@
             )
         )
 ```
 ### Just the signatures
 
 The `-s/--signatures` option will list just the signatures of the functions and classes, for example:
 ```bash
-symbex -s -d symbex
+symbex -s -f symbex/lib.py
 ```
 <!-- [[[cog
 import cog
 from click.testing import CliRunner
 import pathlib
 from symbex.cli import cli
 
+def sorted_chunks(text):
+    chunks = text.strip().split("\n\n")
+    chunks.sort()
+    return "\n\n".join(chunks)
+
 path = pathlib.Path("symbex").resolve()
 runner = CliRunner()
-result = runner.invoke(cli, ["-s", "-d", str(path)])
-# Need a consistent sort order
-chunks = result.stdout.strip().split("\n\n")
-chunks.sort()
+result = runner.invoke(cli, ["-s", "-f", str(path / "lib.py")])
 cog.out(
-    "```python\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format(sorted_chunks(result.output))
 )
 ]]] -->
 ```python
-# File: symbex/cli.py Line: 95
-def cli(symbols, files, directories, signatures, docstrings, count, silent, async_, function, class_, documented, undocumented, typed, untyped, partially_typed, fully_typed)
-
-# File: symbex/lib.py Line: 105
+# File: symbex/lib.py Line: 106
 def function_definition(function_node: AST)
 
-# File: symbex/lib.py Line: 12
+# File: symbex/lib.py Line: 13
 def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
 
-# File: symbex/lib.py Line: 173
+# File: symbex/lib.py Line: 174
 def class_definition(class_def)
 
-# File: symbex/lib.py Line: 207
+# File: symbex/lib.py Line: 208
 def annotation_definition(annotation: AST) -> str
 
-# File: symbex/lib.py Line: 225
+# File: symbex/lib.py Line: 226
 def read_file(path)
 
-# File: symbex/lib.py Line: 251
+# File: symbex/lib.py Line: 252
 class TypeSummary
 
-# File: symbex/lib.py Line: 256
+# File: symbex/lib.py Line: 257
 def type_summary(node: AST) -> Optional[TypeSummary]
 
-# File: symbex/lib.py Line: 302
+# File: symbex/lib.py Line: 303
 def quoted_string(s)
 
-# File: symbex/lib.py Line: 36
+# File: symbex/lib.py Line: 314
+def import_line_for_function(function_name: str, filepath: str, possible_root_dirs: List[str]) -> str
+
+# File: symbex/lib.py Line: 37
 def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
 
-# File: symbex/lib.py Line: 70
+# File: symbex/lib.py Line: 71
 def add_docstring(definition: str, node: AST, docstrings: bool, is_method: bool) -> str
 
-# File: symbex/lib.py Line: 80
+# File: symbex/lib.py Line: 81
 def match(name: str, symbols: Iterable[str]) -> bool
 ```
 <!-- [[[end]]] -->
 This can be combined with other options, or you can run `symbex -s` to see every symbol in the current directory and its subdirectories.
 
-To include docstrings in those signatures, use `--docstrings`:
+To include estimated import paths, such as `# from symbex.lib import match`, use `--imports`. These will be calculated relative to the directory you specified, or you can pass one or more `--sys-path` options to request that imports are calculated relative to those directories as if they were on `sys.path`:
+
 ```bash
-symbex --docstrings --documented -f symbex/lib.py
+~/dev/symbex/symbex match --imports -s --sys-path ~/dev/symbex
 ```
-
+Example output:
 <!-- [[[cog
-runner = CliRunner()
-result = runner.invoke(cli, ["--docstrings", "--documented", "-f", str(path / "lib.py")])
-# Need a consistent sort order
-chunks = result.stdout.strip().split("\n\n")
-chunks.sort()
+result = runner.invoke(cli, [
+    "--imports", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
+])
 cog.out(
-    "```python\n{}\n```\n".format("\n\n".join(chunks))
+    "```python\n{}\n```\n".format(result.stdout.strip())
 )
 ]]] -->
 ```python
-# File: symbex/lib.py Line: 12
-def find_symbol_nodes(code: str, filename: str, symbols: Iterable[str]) -> List[Tuple[(AST, Optional[str])]]
-    "Returns ast Nodes matching symbols"
+# File: symbex/lib.py Line: 81
+# from symbex.lib import match
+def match(name: str, symbols: Iterable[str]) -> bool
+```
+<!-- [[[end]]] -->
+To suppress the `# File: ...` comments, use `--no-file` or `-n`.
 
-# File: symbex/lib.py Line: 36
-def code_for_node(code: str, node: AST, class_name: str, signatures: bool, docstrings: bool) -> Tuple[(str, int)]
-    "Returns the code for a given node"
+So to both show import paths and suppress File comments, use `-in` as a shortcut:
+```bash
+symbex -in match
+```
+Output:
+<!-- [[[cog
+result = runner.invoke(cli, [
+    "-in", "-d", str(path), "match", "-s", "--sys-path", str(path.parent)
+])
+cog.out(
+    "```python\n{}\n```\n".format(result.stdout.strip())
+)
+]]] -->
+```python
+# from symbex.lib import match
+def match(name: str, symbols: Iterable[str]) -> bool
+```
+<!-- [[[end]]] -->
 
-# File: symbex/lib.py Line: 80
+To include docstrings in those signatures, use `--docstrings`:
+```bash
+symbex match --docstrings -f symbex/lib.py
+```
+Example output:
+<!-- [[[cog
+result = runner.invoke(cli, ["match", "--docstrings", "-f", str(path / "lib.py")])
+cog.out(
+    "```python\n{}\n```\n".format(result.stdout.strip())
+)
+]]] -->
+```python
+# File: symbex/lib.py Line: 81
 def match(name: str, symbols: Iterable[str]) -> bool
     "Returns True if name matches any of the symbols, resolving wildcards"
 ```
 <!-- [[[end]]] -->
 
 ## Counting symbols
 
@@ -260,15 +302,14 @@
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
 
 <!-- [[[cog
-import cog
 result2 = runner.invoke(cli, ["--help"])
 help = result2.output.replace("Usage: cli", "Usage: symbex")
 cog.out(
     "```\n{}\n```".format(help)
 )
 ]]] -->
 ```
@@ -308,27 +349,34 @@
       # Count the number of --async functions in the project
       symbex --async --count
 
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
+  --stdlib                   Search the Python standard library
+  -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
-  --docstrings               Show function and class signatures plus docstrings
+  -n, --no-file              Don't include the # File: comments in the output
+  -i, --imports              Show 'from x import y' lines for imported symbols
+  -m, --module TEXT          Modules to search within
+  --sys-path TEXT            Calculate imports relative to these on sys.path
+  --docs, --docstrings       Show function and class signatures plus docstrings
   --count                    Show count of matching symbols
   --silent                   Silently ignore Python files with parse errors
   --async                    Filter async functions
   --function                 Filter functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
+  --no-init                  Filter to exclude any __init__ methods
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-0.6/tests/test_filters.py` & `symbex-0.7/tests/test_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,14 +130,21 @@
             ],
         ),
         (
             ["--fully-typed", "*.*"],
             ["def method_types", "def __init__", "def method_fully_typed"],
         ),
         (
+            ["--fully-typed", "--no-init", "*.*"],
+            [
+                "def method_types",
+                "def method_fully_typed",
+            ],
+        ),
+        (
             ["--partially-typed", "*.*"],
             ["def method_partially_typed"],
         ),
         # Documented and undocumented
         (
             ["--documented"],
             [
```

### Comparing `symbex-0.6/tests/test_symbex.py` & `symbex-0.7/tests/test_symbex.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 @pytest.fixture
 def directory_full_of_code(tmpdir):
     for path, content in (
         ("foo.py", "def foo1():\n    pass\n\n@decorated\ndef foo2():\n    pass\n\n"),
         ("bar.py", "class BarClass:\n    pass\n\n"),
-        ("nested.py/baz.py", 'def baz(delimiter=", ", type=str):\n    pass\n\n'),
+        ("nested.py/x/baz.py", 'def baz(delimiter=", ", type=str):\n    pass\n\n'),
         ("nested.py/error.py", "def baz_error()" + "bug:\n    pass\n\n"),
         (
             "methods.py",
             textwrap.dedent(
                 """
         class MyClass:
             def __init__(self, a):
@@ -64,29 +64,34 @@
         ),
         (
             ["BarClass", "--silent"],
             "# File: bar.py Line: 1\nclass BarClass:\n    pass\n\n",
         ),
         (
             ["baz", "--silent"],
-            '# File: nested.py/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
+            '# File: nested.py/x/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         (
             ["async_func", "--silent"],
             "# File: async.py Line: 1\nasync def async_func(a, b, c):\n    pass\n\n",
         ),
         # The -f option
         (
-            ["baz", "-f", "nested.py/baz.py", "--silent"],
-            '# File: nested.py/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
+            ["baz", "-f", "nested.py/x/baz.py", "--silent"],
+            '# File: nested.py/x/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
         ),
         # The -d option
         (
             ["baz", "-d", "nested.py", "--silent"],
-            '# File: nested.py/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
+            '# File: nested.py/x/baz.py Line: 1\ndef baz(delimiter=", ", type=str):\n    pass\n\n',
+        ),
+        # The -d option with -x to exclude
+        (
+            ["baz", "-d", "nested.py", "-x", "nested.py/x/", "--silent"],
+            "",
         ),
         # Classes
         (
             ["MyClass", "--silent"],
             "# File: methods.py Line: 2\n"
             "class MyClass:\n"
             "    def __init__(self, a):\n"
@@ -150,15 +155,23 @@
             "\n"
             "# File: foo.py Line: 5\n"
             "def foo2()",
         ),
         (["BarClass", "--silent"], "# File: bar.py Line: 1\n" "class BarClass"),
         (
             ["baz", "--silent"],
-            ("# File: nested.py/baz.py Line: 1\n" 'def baz(delimiter=", ", type=str)'),
+            (
+                "# File: nested.py/x/baz.py Line: 1\n"
+                'def baz(delimiter=", ", type=str)'
+            ),
+        ),
+        # Test for the --module option
+        (
+            ["-m", "pathlib", "Path", "--silent", "-in"],
+            ("# from pathlib import Path\nclass Path(PurePath)"),
         ),
     ),
 )
 def test_symbex_symbols(directory_full_of_code, monkeypatch, args, expected):
     runner = CliRunner()
     monkeypatch.chdir(directory_full_of_code)
     result = runner.invoke(cli, args + ["-s"], catch_exceptions=False)
@@ -170,15 +183,15 @@
 def test_errors(directory_full_of_code, monkeypatch):
     # Test without --silent to see errors
     runner = CliRunner(mix_stderr=False)
     monkeypatch.chdir(directory_full_of_code)
     result = runner.invoke(cli, ["baz"], catch_exceptions=False)
     assert result.exit_code == 0
     expected = (
-        "# File: nested.py/baz.py Line: 1\n"
+        "# File: nested.py/x/baz.py Line: 1\n"
         'def baz(delimiter=", ", type=str):\n'
         "    pass\n\n"
     )
     assert result.stdout == expected
     # This differs between different Python versions
     assert result.stderr.startswith("# Syntax error in nested.py/error.py:")
```

### Comparing `symbex-0.6/tests/test_symbols.py` & `symbex-0.7/tests/test_symbols.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,7 +105,39 @@
         \"\"\"Multiple
         lines\"\"\"
     """.strip()
     actual = result.stdout.strip()
     # Replace 'Line \d' with 'Line X' before comparison using re
     actual = re.sub(r"Line: \d+", "Line: X", actual)
     assert actual == expected
+
+
+@pytest.mark.parametrize("no_file", (False, True))
+def test_imports(no_file):
+    runner = CliRunner()
+    args = [
+        "func_arbitrary*",
+        "--imports",
+        "-s",
+        "-d",
+        str(pathlib.Path(__file__).parent),
+    ] + (["--no-file"] if no_file else [])
+    result = runner.invoke(cli, args, catch_exceptions=False)
+    assert result.exit_code == 0
+    expected = """
+# File: tests/example_symbols.py Line: 28
+# from example_symbols import func_arbitrary_positional_args
+def func_arbitrary_positional_args(*args)
+
+# File: tests/example_symbols.py Line: 33
+# from example_symbols import func_arbitrary_keyword_args
+def func_arbitrary_keyword_args(**kwargs)
+
+# File: tests/example_symbols.py Line: 38
+# from example_symbols import func_arbitrary_args
+def func_arbitrary_args(*args, **kwargs)
+    """.strip()
+    if no_file:
+        lines = expected.split("\n")
+        lines = [line for line in lines if not line.startswith("# File: ")]
+        expected = "\n".join(lines)
+    assert result.output.strip() == expected
```

