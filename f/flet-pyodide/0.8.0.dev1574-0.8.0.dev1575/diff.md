# Comparing `tmp/flet_pyodide-0.8.0.dev1574.tar.gz` & `tmp/flet_pyodide-0.8.0.dev1575.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.8.0.dev1574.tar", max compression
+gzip compressed data, was "flet_pyodide-0.8.0.dev1575.tar", max compression
```

## Comparing `flet_pyodide-0.8.0.dev1574.tar` & `flet_pyodide-0.8.0.dev1575.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/README.md
--rw-r--r--   0        0        0      644 2023-06-23 19:01:19.867190 flet_pyodide-0.8.0.dev1574/pyproject.toml
--rw-r--r--   0        0        0       61 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2285 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3851 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-06-23 19:00:43.701522 flet_pyodide-0.8.0.dev1574/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.8.0.dev1574/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/README.md
+-rw-r--r--   0        0        0      644 2023-06-23 19:34:56.706583 flet_pyodide-0.8.0.dev1575/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2285 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-06-23 19:34:22.187322 flet_pyodide-0.8.0.dev1575/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.8.0.dev1575/PKG-INFO
```

### Comparing `flet_pyodide-0.8.0.dev1574/README.md` & `flet_pyodide-0.8.0.dev1575/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.8.0.dev1574/pyproject.toml` & `flet_pyodide-0.8.0.dev1575/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.8.0.dev1574"
+version = "0.8.0.dev1575"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.8.0.dev1574"
+flet-core = "0.8.0.dev1575"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.8.0.dev1574/src/flet/flet.py` & `flet_pyodide-0.8.0.dev1575/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.8.0.dev1574/src/flet/pyodide_connection.py` & `flet_pyodide-0.8.0.dev1575/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.8.0.dev1574/PKG-INFO` & `flet_pyodide-0.8.0.dev1575/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.8.0.dev1574
+Version: 0.8.0.dev1575
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.8.0.dev1574)
+Requires-Dist: flet-core (==0.8.0.dev1575)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

