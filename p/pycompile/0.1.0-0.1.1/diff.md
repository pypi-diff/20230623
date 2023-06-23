# Comparing `tmp/pycompile-0.1.0.tar.gz` & `tmp/pycompile-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompile-0.1.0.tar", max compression
+gzip compressed data, was "pycompile-0.1.1.tar", max compression
```

## Comparing `pycompile-0.1.0.tar` & `pycompile-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1074 2023-02-26 11:54:32.633817 pycompile-0.1.0/LICENSE
--rw-r--r--   0        0        0     1984 2023-06-22 15:08:59.709454 pycompile-0.1.0/README.md
--rw-r--r--   0        0        0     1233 2023-06-23 16:44:31.817845 pycompile-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      303 2023-06-22 19:01:47.157750 pycompile-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     3711 2023-06-23 14:45:40.936099 pycompile-0.1.0/src/benchmark.py
--rw-r--r--   0        0        0     3532 2023-06-23 14:49:05.974794 pycompile-0.1.0/src/cli.py
--rw-r--r--   0        0        0     2638 2023-06-23 14:37:06.677278 pycompile-0.1.0/src/compiler_handler.py
--rw-r--r--   0        0        0     3368 2023-06-22 20:23:59.862617 pycompile-0.1.0/src/compilers.py
--rw-r--r--   0        0        0        0 2023-06-23 15:28:11.478073 pycompile-0.1.0/src/examples/__init__.py
--rw-r--r--   0        0        0      192 2023-06-23 15:28:11.477359 pycompile-0.1.0/src/examples/fib.py
--rw-r--r--   0        0        0      254 2023-06-23 15:28:11.475241 pycompile-0.1.0/src/examples/harmonic.py
--rw-r--r--   0        0        0      176 2023-06-23 15:28:11.474441 pycompile-0.1.0/src/examples/sum.py
--rw-r--r--   0        0        0      144 2023-06-23 16:52:49.172923 pycompile-0.1.0/src/examples/sum_of_sqaures.py
--rw-r--r--   0        0        0       99 2023-06-23 15:28:11.478864 pycompile-0.1.0/src/examples/test_fib.py
--rw-r--r--   0        0        0      131 2023-06-23 15:28:11.476651 pycompile-0.1.0/src/examples/test_harmonic_mean.py
--rw-r--r--   0        0        0       95 2023-06-23 15:28:11.475960 pycompile-0.1.0/src/examples/test_sum.py
--rw-r--r--   0        0        0      131 2023-06-23 15:28:11.480540 pycompile-0.1.0/src/examples/test_sum_of_sqaures.py
--rw-r--r--   0        0        0     4074 2023-03-05 18:06:23.411177 pycompile-0.1.0/src/file_handler.py
--rw-r--r--   0        0        0     1194 2023-06-22 17:17:53.521707 pycompile-0.1.0/src/helpers.py
--rw-r--r--   0        0        0     1341 2023-06-22 19:01:46.446391 pycompile-0.1.0/src/logging_setup.py
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 pycompile-0.1.0/setup.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 pycompile-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-23 17:09:20.432946 pycompile-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1984 2023-06-23 17:09:20.432946 pycompile-0.1.1/README.md
+-rw-r--r--   0        0        0     1233 2023-06-23 17:09:20.432946 pycompile-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      303 2023-06-23 17:09:20.432946 pycompile-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     3711 2023-06-23 17:09:20.432946 pycompile-0.1.1/src/benchmark.py
+-rw-r--r--   0        0        0     3532 2023-06-23 17:09:20.432946 pycompile-0.1.1/src/cli.py
+-rw-r--r--   0        0        0     2638 2023-06-23 17:09:20.432946 pycompile-0.1.1/src/compiler_handler.py
+-rw-r--r--   0        0        0     3368 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/compilers.py
+-rw-r--r--   0        0        0        0 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/fib.py
+-rw-r--r--   0        0        0      254 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/harmonic.py
+-rw-r--r--   0        0        0      176 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/sum.py
+-rw-r--r--   0        0        0      144 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/sum_of_sqaures.py
+-rw-r--r--   0        0        0       99 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/test_fib.py
+-rw-r--r--   0        0        0      131 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/test_harmonic_mean.py
+-rw-r--r--   0        0        0       95 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/test_sum.py
+-rw-r--r--   0        0        0      131 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/examples/test_sum_of_sqaures.py
+-rw-r--r--   0        0        0     4074 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/file_handler.py
+-rw-r--r--   0        0        0     1194 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/helpers.py
+-rw-r--r--   0        0        0     1341 2023-06-23 17:09:20.436946 pycompile-0.1.1/src/logging_setup.py
+-rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 pycompile-0.1.1/PKG-INFO
```

### Comparing `pycompile-0.1.0/LICENSE` & `pycompile-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/README.md` & `pycompile-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/pyproject.toml` & `pycompile-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycompile"
-version = "0.1.0"
+version = "0.1.1"
 description = "A CLI tool for compiling python"
 authors = ["iplitharas <johnplitharas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src" }
 ]
```

### Comparing `pycompile-0.1.0/src/benchmark.py` & `pycompile-0.1.1/src/benchmark.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/src/cli.py` & `pycompile-0.1.1/src/cli.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/src/compiler_handler.py` & `pycompile-0.1.1/src/compiler_handler.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/src/compilers.py` & `pycompile-0.1.1/src/compilers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/src/file_handler.py` & `pycompile-0.1.1/src/file_handler.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/src/helpers.py` & `pycompile-0.1.1/src/helpers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/src/logging_setup.py` & `pycompile-0.1.1/src/logging_setup.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.0/setup.py` & `pycompile-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,79 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pycompile
+Version: 0.1.1
+Summary: A CLI tool for compiling python
+License: MIT
+Author: iplitharas
+Author-email: johnplitharas@gmail.com
+Requires-Python: >3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: cython (>=0.29.33,<0.30.0)
+Requires-Dist: nuitka (>=1.4.8,<2.0.0)
+Requires-Dist: pytest-benchmark (>=4.0.0,<5.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Description-Content-Type: text/markdown
+
+# pycompile
+
+```python
+"""                                        _ _
+    _ __  _   _  ___ ___  _ __ ___  _ __ (_) | ___
+   | '_ \| | | |/ __/ _ \| '_ ` _ \| '_ \| | |/ _ \
+   | |_) | |_| | (_| (_) | | | | | | |_) | | |  __/
+   | .__/ \__, |\___\___/|_| |_| |_| .__/|_|_|\___|
+   |_|    |___/                    |_|
+   
+"""
+```
+A CLI tool for compiling python source code using [Cython](https://cython.org/)  or
+[Nuitka](https://nuitka.net/).
+
+## Table of contents
+1. [Local-development](#local-development)
+2. [Usage](#usage)
+
+### Local-development
+For local development run the following command
+```bash
+make setup-local-dev
+```
+All available `make` commands
+```bash
+make help
+```
+
+## Usage
+
+```bash
+pycompile -i your_python_files --clean-source --engine nuitka 
+```
+
+By default, the [Cython](https://cython.org/) is being used as the default
+compiler. 
+
+
+| Syntax                | Description                                                   |
+|-----------------------|---------------------------------------------------------------|
+| `--input-path PATH`   | by default it will exclude any `test` and `__init__.py` files |
+| `--clean-source`      | Deletes the sources files.                                    |
+| `--keep-builds`       | Keeps the temp build files.                                   |
+| `--clean-executables` | Deletes the shared objects (`.so`) files.                     |
+| `--engine`            | Can be `cython` or `nuitka`.                                  |
+| `-exclude-glob-paths` | Glob file patterns for excluding specific files.              |
+| `--verbose`           | Increase log messages.                                        |
+
+### Compiling the examples
+For compiling the `examples` use the following command:
+```bash
+pycompile -i examples
+```
+which by default, deletes any temp build files and keeps the source files.
 
-packages = \
-['src', 'src.examples']
+[![asciicast](https://asciinema.org/a/QK5h8zR0oW2CGvfJtrmWZ3es0.svg)](https://asciinema.org/a/QK5h8zR0oW2CGvfJtrmWZ3es0)
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'cython>=0.29.33,<0.30.0',
- 'nuitka>=1.4.8,<2.0.0',
- 'pytest-benchmark>=4.0.0,<5.0.0',
- 'tqdm>=4.64.1,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['pycompile = src.cli:main']}
-
-setup_kwargs = {
-    'name': 'pycompile',
-    'version': '0.1.0',
-    'description': 'A CLI tool for compiling python',
-    'long_description': '# pycompile\n\n```python\n"""                                        _ _\n    _ __  _   _  ___ ___  _ __ ___  _ __ (_) | ___\n   | \'_ \\| | | |/ __/ _ \\| \'_ ` _ \\| \'_ \\| | |/ _ \\\n   | |_) | |_| | (_| (_) | | | | | | |_) | | |  __/\n   | .__/ \\__, |\\___\\___/|_| |_| |_| .__/|_|_|\\___|\n   |_|    |___/                    |_|\n   \n"""\n```\nA CLI tool for compiling python source code using [Cython](https://cython.org/)  or\n[Nuitka](https://nuitka.net/).\n\n## Table of contents\n1. [Local-development](#local-development)\n2. [Usage](#usage)\n\n### Local-development\nFor local development run the following command\n```bash\nmake setup-local-dev\n```\nAll available `make` commands\n```bash\nmake help\n```\n\n## Usage\n\n```bash\npycompile -i your_python_files --clean-source --engine nuitka \n```\n\nBy default, the [Cython](https://cython.org/) is being used as the default\ncompiler. \n\n\n| Syntax                | Description                                                   |\n|-----------------------|---------------------------------------------------------------|\n| `--input-path PATH`   | by default it will exclude any `test` and `__init__.py` files |\n| `--clean-source`      | Deletes the sources files.                                    |\n| `--keep-builds`       | Keeps the temp build files.                                   |\n| `--clean-executables` | Deletes the shared objects (`.so`) files.                     |\n| `--engine`            | Can be `cython` or `nuitka`.                                  |\n| `-exclude-glob-paths` | Glob file patterns for excluding specific files.              |\n| `--verbose`           | Increase log messages.                                        |\n\n### Compiling the examples\nFor compiling the `examples` use the following command:\n```bash\npycompile -i examples\n```\nwhich by default, deletes any temp build files and keeps the source files.\n\n[![asciicast](https://asciinema.org/a/QK5h8zR0oW2CGvfJtrmWZ3es0.svg)](https://asciinema.org/a/QK5h8zR0oW2CGvfJtrmWZ3es0)\n\n',
-    'author': 'iplitharas',
-    'author_email': 'johnplitharas@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>3.8',
-}
-
-
-setup(**setup_kwargs)
```

