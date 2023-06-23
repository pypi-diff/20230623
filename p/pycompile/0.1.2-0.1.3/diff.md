# Comparing `tmp/pycompile-0.1.2.tar.gz` & `tmp/pycompile-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompile-0.1.2.tar", max compression
+gzip compressed data, was "pycompile-0.1.3.tar", max compression
```

## Comparing `pycompile-0.1.2.tar` & `pycompile-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1074 2023-06-23 18:36:49.071728 pycompile-0.1.2/LICENSE
--rw-r--r--   0        0        0     1984 2023-06-23 18:36:49.071728 pycompile-0.1.2/README.md
--rw-r--r--   0        0        0     1233 2023-06-23 18:36:49.071728 pycompile-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      307 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/__init__.py
--rw-r--r--   0        0        0     3696 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/benchmark.py
--rw-r--r--   0        0        0     3525 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/cli.py
--rw-r--r--   0        0        0     2641 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/compiler_handler.py
--rw-r--r--   0        0        0        0 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/__init__.py
--rw-r--r--   0        0        0      192 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/fib.py
--rw-r--r--   0        0        0      254 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/harmonic.py
--rw-r--r--   0        0        0      176 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/sum.py
--rw-r--r--   0        0        0      144 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/sum_of_sqaures.py
--rw-r--r--   0        0        0       99 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/test_fib.py
--rw-r--r--   0        0        0      131 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/test_harmonic_mean.py
--rw-r--r--   0        0        0       95 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/test_sum.py
--rw-r--r--   0        0        0      131 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/examples/test_sum_of_sqaures.py
--rw-r--r--   0        0        0     4074 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/file_handler.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/helpers.py
--rw-r--r--   0        0        0     1341 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/logging_setup.py
--rw-r--r--   0        0        0     3209 2023-06-23 18:36:49.071728 pycompile-0.1.2/src/wrappers.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 pycompile-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-23 19:00:09.392543 pycompile-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2195 2023-06-23 19:00:09.392543 pycompile-0.1.3/README.md
+-rw-r--r--   0        0        0     1233 2023-06-23 19:00:09.392543 pycompile-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0     3696 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/benchmark.py
+-rw-r--r--   0        0        0     3525 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/cli.py
+-rw-r--r--   0        0        0     2641 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/compiler_handler.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/fib.py
+-rw-r--r--   0        0        0      254 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/harmonic.py
+-rw-r--r--   0        0        0      176 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/sum.py
+-rw-r--r--   0        0        0      144 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/sum_of_sqaures.py
+-rw-r--r--   0        0        0       99 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_fib.py
+-rw-r--r--   0        0        0      131 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_harmonic_mean.py
+-rw-r--r--   0        0        0       95 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_sum.py
+-rw-r--r--   0        0        0      131 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/examples/test_sum_of_sqaures.py
+-rw-r--r--   0        0        0     4074 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/file_handler.py
+-rw-r--r--   0        0        0     1194 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/helpers.py
+-rw-r--r--   0        0        0     1341 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/logging_setup.py
+-rw-r--r--   0        0        0     3209 2023-06-23 19:00:09.392543 pycompile-0.1.3/src/wrappers.py
+-rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 pycompile-0.1.3/PKG-INFO
```

### Comparing `pycompile-0.1.2/LICENSE` & `pycompile-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/pyproject.toml` & `pycompile-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycompile"
-version = "0.1.2"
+version = "0.1.3"
 description = "A CLI tool for compiling python"
 authors = ["iplitharas <johnplitharas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src" }
 ]
```

### Comparing `pycompile-0.1.2/src/benchmark.py` & `pycompile-0.1.3/src/benchmark.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/src/cli.py` & `pycompile-0.1.3/src/cli.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/src/compiler_handler.py` & `pycompile-0.1.3/src/compiler_handler.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/src/file_handler.py` & `pycompile-0.1.3/src/file_handler.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/src/helpers.py` & `pycompile-0.1.3/src/helpers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/src/logging_setup.py` & `pycompile-0.1.3/src/logging_setup.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/src/wrappers.py` & `pycompile-0.1.3/src/wrappers.py`

 * *Files identical despite different names*

### Comparing `pycompile-0.1.2/PKG-INFO` & `pycompile-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompile
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI tool for compiling python
 License: MIT
 Author: iplitharas
 Author-email: johnplitharas@gmail.com
 Requires-Python: >3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -73,7 +73,15 @@
 pycompile -i examples
 ```
 which by default, deletes any temp build files and keeps the source files.
 
 [![asciicast](https://asciinema.org/a/QK5h8zR0oW2CGvfJtrmWZ3es0.svg)](https://asciinema.org/a/QK5h8zR0oW2CGvfJtrmWZ3es0)
 
 
+### Benchmark sample examples
+For running a benchmark on  the `examples` use the following command:
+```bash
+pycompile -b 
+```
+[![asciicast](https://asciinema.org/a/592966.svg)](https://asciinema.org/a/592966)
+
+
```

