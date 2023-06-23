# Comparing `tmp/starlark_pyo3-2022.1.tar.gz` & `tmp/starlark_pyo3-2022.1.1.tar.gz`

## Comparing `starlark_pyo3-2022.1.tar` & `starlark_pyo3-2022.1.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 starlark_pyo3-2022.1/Cargo.toml
--rw-r--r--   0     1000     1000     4817 2022-10-22 05:15:00.000000 starlark_pyo3-2022.1/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000       55 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/.gitignore
--rw-r--r--   0     1000     1000    11384 2022-09-22 01:51:41.000000 starlark_pyo3-2022.1/LICENSE
--rw-r--r--   0     1000     1000      662 2022-10-22 05:16:59.000000 starlark_pyo3-2022.1/README.md
--rw-r--r--   0     1000     1000      634 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/doc/Makefile
--rw-r--r--   0     1000     1000      499 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/doc/conf.py
--rw-r--r--   0     1000     1000      560 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/doc/index.rst
--rw-r--r--   0     1000     1000      800 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/doc/make.bat
--rw-r--r--   0     1000     1000      496 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/doc/misc.rst
--rw-r--r--   0     1000     1000      848 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/doc/reference.rst
--rw-r--r--   0     1000     1000      771 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/examples/demo.py
--rw-r--r--   0     1000     1000      587 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/examples/dos.py
--rw-r--r--   0     1000     1000      569 2022-09-25 19:05:49.000000 starlark_pyo3-2022.1/pyproject.toml
--rw-r--r--   0     1000     1000       46 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/requirements-dev.txt
--rw-r--r--   0     1000     1000      118 2022-10-21 22:06:55.000000 starlark_pyo3-2022.1/setup.cfg
--rw-r--r--   0     1000     1000    16125 2022-10-22 00:04:24.000000 starlark_pyo3-2022.1/src/lib.rs
--rw-r--r--   0     1000     1000     1554 2022-10-21 22:06:55.000000 starlark_pyo3-2022.1/test/test_starlark.py
--rw-r--r--   0     1000     1000    39298 2022-09-22 02:11:05.000000 starlark_pyo3-2022.1/Cargo.lock
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 starlark_pyo3-2022.1/PKG-INFO
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 starlark_pyo3-2022.1.1/Cargo.toml
+-rw-r--r--   0     1001      121    11384 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/LICENSE
+-rw-r--r--   0     1001      121      662 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/README.md
+-rw-r--r--   0     1001      121      634 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/doc/Makefile
+-rw-r--r--   0     1001      121      499 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/doc/conf.py
+-rw-r--r--   0     1001      121      560 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/doc/index.rst
+-rw-r--r--   0     1001      121      800 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/doc/make.bat
+-rw-r--r--   0     1001      121      496 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/doc/misc.rst
+-rw-r--r--   0     1001      121      848 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/doc/reference.rst
+-rw-r--r--   0     1001      121      771 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/examples/demo.py
+-rw-r--r--   0     1001      121      587 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/examples/dos.py
+-rw-r--r--   0     1001      121      571 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/pyproject.toml
+-rw-r--r--   0     1001      121       46 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/requirements-dev.txt
+-rwxr-xr-x   0     1001      121      769 2022-10-22 05:40:10.000000 starlark_pyo3-2022.1.1/run-maturin-action.sh
+-rw-r--r--   0     1001      121      118 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/setup.cfg
+-rw-r--r--   0     1001      121    16125 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/src/lib.rs
+-rw-r--r--   0     1001      121     1554 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/test/test_starlark.py
+-rw-r--r--   0     1001      121    39298 2022-10-22 05:39:41.000000 starlark_pyo3-2022.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 starlark_pyo3-2022.1.1/PKG-INFO
```

### Comparing `starlark_pyo3-2022.1/Cargo.toml` & `starlark_pyo3-2022.1.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/LICENSE` & `starlark_pyo3-2022.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/README.md` & `starlark_pyo3-2022.1.1/README.md`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/doc/Makefile` & `starlark_pyo3-2022.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/doc/index.rst` & `starlark_pyo3-2022.1.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/doc/make.bat` & `starlark_pyo3-2022.1.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/doc/reference.rst` & `starlark_pyo3-2022.1.1/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/examples/demo.py` & `starlark_pyo3-2022.1.1/examples/demo.py`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/examples/dos.py` & `starlark_pyo3-2022.1.1/examples/dos.py`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/pyproject.toml` & `starlark_pyo3-2022.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.13,<0.14"]
 build-backend = "maturin"
 
 [project]
 name = "starlark-pyo3"
-version = "2022.1"
+version = "2022.1.1"
 description = "Wraps starlark-rust into Python"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     { name = "Andreas Kloeckner", email = "inform@tiker.net" }
     ]
 classifiers = [
```

### Comparing `starlark_pyo3-2022.1/src/lib.rs` & `starlark_pyo3-2022.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/test/test_starlark.py` & `starlark_pyo3-2022.1.1/test/test_starlark.py`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/Cargo.lock` & `starlark_pyo3-2022.1.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `starlark_pyo3-2022.1/PKG-INFO` & `starlark_pyo3-2022.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: starlark-pyo3
-Version: 2022.1
+Version: 2022.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
-License-File: LICENSE~
 Summary: Wraps starlark-rust into Python
 Home-Page: https://github.com/inducer/starlark-pyo3
 Author: Andreas Kloeckner <inform@tiker.net>
 Author-email: Andreas Kloeckner <inform@tiker.net>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

