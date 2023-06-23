# Comparing `tmp/alt_pytest_asyncio-0.7.0.tar.gz` & `tmp/alt_pytest_asyncio-0.7.1.tar.gz`

## Comparing `alt_pytest_asyncio-0.7.0.tar` & `alt_pytest_asyncio-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/__init__.py
--rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/async_converters.py
--rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/plugin.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/version.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/LICENSE
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/README.rst
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/alt_pytest_asyncio/__init__.py
+-rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/alt_pytest_asyncio/async_converters.py
+-rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/alt_pytest_asyncio/plugin.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/alt_pytest_asyncio/version.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/README.rst
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.1/PKG-INFO
```

### Comparing `alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/__init__.py` & `alt_pytest_asyncio-0.7.1/alt_pytest_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/async_converters.py` & `alt_pytest_asyncio-0.7.1/alt_pytest_asyncio/async_converters.py`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.7.0/alt_pytest_asyncio/plugin.py` & `alt_pytest_asyncio-0.7.1/alt_pytest_asyncio/plugin.py`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.7.0/LICENSE` & `alt_pytest_asyncio-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.7.0/README.rst` & `alt_pytest_asyncio-0.7.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.7.1 - 23 June 2023
+    * No functional changes, only fixing how hatchling understands the
+      license field in the pyproject.toml with thanks to @piotrm-nvidia
+
 0.7.0 - 12 April 2023
     * Changed the pytest dependency to be greater than pytest version 7
     * Using isort now
     * Went from setuptools to hatch
     * CI now runs against python 3.11
 
 0.6.0 - 23 October 2021
```

### Comparing `alt_pytest_asyncio-0.7.0/pyproject.toml` & `alt_pytest_asyncio-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "alt-pytest-asyncio"
 dynamic = ["version"]
 description = "Alternative pytest plugin to pytest-asyncio"
 readme = "README.rst"
-license = "MIT"
+license = { text = "MIT" }
 requires-python = ">= 3.7"
 authors = [
     { name = "Stephen Moore", email = "delfick755@gmail.com" },
 ]
 classifiers = [
     "Framework :: Pytest",
     "Topic :: Software Development :: Testing",
```

### Comparing `alt_pytest_asyncio-0.7.0/PKG-INFO` & `alt_pytest_asyncio-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alt-pytest-asyncio
-Version: 0.7.0
+Version: 0.7.1
 Summary: Alternative pytest plugin to pytest-asyncio
 Project-URL: Homepage, https://github.com/delfick/alt-pytest-asyncio
 Author-email: Stephen Moore <delfick755@gmail.com>
-License-Expression: MIT
+License: MIT
 License-File: LICENSE
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Requires-Dist: pytest>=7.0.0
 Provides-Extra: tests
 Requires-Dist: nest-asyncio==1.0.0; extra == 'tests'
@@ -35,14 +35,18 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.7.1 - 23 June 2023
+    * No functional changes, only fixing how hatchling understands the
+      license field in the pyproject.toml with thanks to @piotrm-nvidia
+
 0.7.0 - 12 April 2023
     * Changed the pytest dependency to be greater than pytest version 7
     * Using isort now
     * Went from setuptools to hatch
     * CI now runs against python 3.11
 
 0.6.0 - 23 October 2021
```

