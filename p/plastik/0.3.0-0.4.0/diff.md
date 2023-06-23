# Comparing `tmp/plastik-0.3.0.tar.gz` & `tmp/plastik-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plastik-0.3.0.tar", max compression
+gzip compressed data, was "plastik-0.4.0.tar", max compression
```

## Comparing `plastik-0.3.0.tar` & `plastik-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-03-24 12:47:53.081095 plastik-0.3.0/LICENSE
--rw-r--r--   0        0        0      818 2023-03-24 12:47:53.081095 plastik-0.3.0/README.md
--rw-r--r--   0        0        0     1011 2023-03-24 12:48:05.245988 plastik-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      215 2023-03-24 12:48:05.245988 plastik-0.3.0/src/plastik/__init__.py
--rw-r--r--   0        0        0     2852 2023-03-24 12:47:53.093095 plastik-0.3.0/src/plastik/axes.py
--rw-r--r--   0        0        0     5514 2023-03-24 12:47:53.093095 plastik-0.3.0/src/plastik/legends.py
--rw-r--r--   0        0        0    12220 2023-03-24 12:47:53.093095 plastik-0.3.0/src/plastik/ridge.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 plastik-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 10:15:55.485187 plastik-0.4.0/LICENSE
+-rw-r--r--   0        0        0      818 2023-06-23 10:15:55.485187 plastik-0.4.0/README.md
+-rw-r--r--   0        0        0     1031 2023-06-23 10:16:11.965225 plastik-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/__init__.py
+-rw-r--r--   0        0        0     2852 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/axes.py
+-rw-r--r--   0        0        0     8874 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/colors.py
+-rw-r--r--   0        0        0      942 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/default.mplstyle
+-rw-r--r--   0        0        0     5514 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/legends.py
+-rw-r--r--   0        0        0    12220 2023-06-23 10:15:55.501187 plastik-0.4.0/src/plastik/ridge.py
+-rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 plastik-0.4.0/PKG-INFO
```

### Comparing `plastik-0.3.0/LICENSE` & `plastik-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plastik-0.3.0/README.md` & `plastik-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `plastik-0.3.0/pyproject.toml` & `plastik-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plastik"
-version = "0.3.0"
+version = "0.4.0"
 description = "plastic surgery for plt"
 authors = ["Eirik Rolland Enger <eirroleng@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/engeir/plastik"
 repository = "https://github.com/engeir/plastik"
 documentation = "https://plastik.readthedocs.io/en/latest/"
@@ -17,14 +17,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.21.4"
 matplotlib = "^3.5.0"
 attrs = "^21.4.0"
 importlib-metadata = "^6.1.0"
+pywaffle = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.10.1"
 pre-commit = "^2.15.0"
 pre-commit-hooks = "^4.0.1"
 pyupgrade = "^2.29.1"
```

### Comparing `plastik-0.3.0/src/plastik/axes.py` & `plastik-0.4.0/src/plastik/axes.py`

 * *Files identical despite different names*

### Comparing `plastik-0.3.0/src/plastik/legends.py` & `plastik-0.4.0/src/plastik/legends.py`

 * *Files identical despite different names*

### Comparing `plastik-0.3.0/src/plastik/ridge.py` & `plastik-0.4.0/src/plastik/ridge.py`

 * *Files identical despite different names*

### Comparing `plastik-0.3.0/PKG-INFO` & `plastik-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: plastik
-Version: 0.3.0
+Version: 0.4.0
 Summary: plastic surgery for plt
 Home-page: https://github.com/engeir/plastik
 License: GPLv3
 Author: Eirik Rolland Enger
 Author-email: eirroleng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
 Requires-Dist: importlib-metadata (>=6.1.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
 Requires-Dist: numpy (>=1.21.4,<2.0.0)
+Requires-Dist: pywaffle (>=1.1.0,<2.0.0)
 Project-URL: Documentation, https://plastik.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/engeir/plastik
 Description-Content-Type: text/markdown
 
 # plastik
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
```

