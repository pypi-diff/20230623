# Comparing `tmp/kevbits-0.8.0.tar.gz` & `tmp/kevbits-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kevbits-0.8.0.tar", max compression
+gzip compressed data, was "kevbits-0.9.0.tar", max compression
```

## Comparing `kevbits-0.8.0.tar` & `kevbits-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.8.0/kevbits/__init__.py
--rw-r--r--   0        0        0     2559 2023-06-21 09:53:25.100230 kevbits-0.8.0/kevbits/logconfig.py
--rw-r--r--   0        0        0      631 2023-03-12 08:27:49.627869 kevbits-0.8.0/kevbits/math.py
--rw-r--r--   0        0        0     2738 2023-06-21 09:54:02.808201 kevbits-0.8.0/kevbits/misc.py
--rw-r--r--   0        0        0     5900 2023-06-21 09:55:00.215123 kevbits-0.8.0/kevbits/sgconv.py
--rw-r--r--   0        0        0      916 2023-06-21 09:56:20.851629 kevbits-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      219 2023-03-12 07:21:14.714981 kevbits-0.8.0/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 kevbits-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.9.0/kevbits/__init__.py
+-rw-r--r--   0        0        0      618 2023-06-23 09:41:42.361146 kevbits-0.9.0/kevbits/capture_stdout.py
+-rw-r--r--   0        0        0     2559 2023-06-21 09:53:25.100230 kevbits-0.9.0/kevbits/logconfig.py
+-rw-r--r--   0        0        0      631 2023-03-12 08:27:49.627869 kevbits-0.9.0/kevbits/math.py
+-rw-r--r--   0        0        0     2738 2023-06-21 09:54:02.808201 kevbits-0.9.0/kevbits/misc.py
+-rw-r--r--   0        0        0     5900 2023-06-21 09:55:00.215123 kevbits-0.9.0/kevbits/sgconv.py
+-rw-r--r--   0        0        0      916 2023-06-23 09:43:31.968263 kevbits-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-03-12 07:21:14.714981 kevbits-0.9.0/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 kevbits-0.9.0/PKG-INFO
```

### Comparing `kevbits-0.8.0/kevbits/logconfig.py` & `kevbits-0.9.0/kevbits/logconfig.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.8.0/kevbits/math.py` & `kevbits-0.9.0/kevbits/math.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.8.0/kevbits/misc.py` & `kevbits-0.9.0/kevbits/misc.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.8.0/kevbits/sgconv.py` & `kevbits-0.9.0/kevbits/sgconv.py`

 * *Files identical despite different names*

### Comparing `kevbits-0.8.0/pyproject.toml` & `kevbits-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kevbits"
-version = "0.8.0"
+version = "0.9.0"
 description = "Small helper functions and objects"
 authors = ["Evgeny Klunko <eklunko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kevbits-0.8.0/PKG-INFO` & `kevbits-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevbits
-Version: 0.8.0
+Version: 0.9.0
 Summary: Small helper functions and objects
 Author: Evgeny Klunko
 Author-email: eklunko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

