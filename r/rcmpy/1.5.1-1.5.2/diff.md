# Comparing `tmp/rcmpy-1.5.1.tar.gz` & `tmp/rcmpy-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.5.1.tar", last modified: Wed May 24 19:53:23 2023, max compression
+gzip compressed data, was "rcmpy-1.5.2.tar", last modified: Fri Jun 23 07:27:19 2023, max compression
```

## Comparing `rcmpy-1.5.1.tar` & `rcmpy-1.5.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 19:51:59.000000 rcmpy-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-24 19:53:23.830553 rcmpy-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-24 19:51:59.000000 rcmpy-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 19:51:59.000000 rcmpy-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.826553 rcmpy-1.5.1/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.826553 rcmpy-1.5.1/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/watch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/watch/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-24 19:51:59.000000 rcmpy-1.5.1/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.826553 rcmpy-1.5.1/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 19:53:23.000000 rcmpy-1.5.1/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 19:53:23.830553 rcmpy-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-24 19:51:59.000000 rcmpy-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:53:23.830553 rcmpy-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 19:51:59.000000 rcmpy-1.5.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 19:51:59.000000 rcmpy-1.5.1/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-24 19:51:59.000000 rcmpy-1.5.1/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 07:26:11.000000 rcmpy-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-06-23 07:27:19.369839 rcmpy-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-23 07:26:11.000000 rcmpy-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-23 07:26:11.000000 rcmpy-1.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.361839 rcmpy-1.5.2/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/watch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/watch/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:27:19.369839 rcmpy-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-23 07:26:11.000000 rcmpy-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-23 07:26:11.000000 rcmpy-1.5.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 07:26:11.000000 rcmpy-1.5.2/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 07:26:11.000000 rcmpy-1.5.2/tests/test_xdg.py
```

### Comparing `rcmpy-1.5.1/LICENSE` & `rcmpy-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/PKG-INFO` & `rcmpy-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.1
+Version: 1.5.2
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=744ace272d6f05ecee63ea172bf1a6bd
+    hash=3c7a54d3f5dd7f524b8ad29c1dee448d
     =====================================
 -->
 
-# rcmpy ([1.5.1](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.2](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.5.1/README.md` & `rcmpy-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=744ace272d6f05ecee63ea172bf1a6bd
+    hash=3c7a54d3f5dd7f524b8ad29c1dee448d
     =====================================
 -->
 
-# rcmpy ([1.5.1](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.2](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.5.1/pyproject.toml` & `rcmpy-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.5.1"
+version = "1.5.2"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.5.1/rcmpy/app.py` & `rcmpy-1.5.2/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/commands/all.py` & `rcmpy-1.5.2/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/commands/apply.py` & `rcmpy-1.5.2/rcmpy/commands/apply.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/commands/common.py` & `rcmpy-1.5.2/rcmpy/commands/common.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/commands/dump.py` & `rcmpy-1.5.2/rcmpy/commands/dump.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/commands/use.py` & `rcmpy-1.5.2/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/commands/variant.py` & `rcmpy-1.5.2/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/commands/watch.py` & `rcmpy-1.5.2/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/config/__init__.py` & `rcmpy-1.5.2/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/config/file.py` & `rcmpy-1.5.2/rcmpy/config/file.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.5.2/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/entry.py` & `rcmpy-1.5.2/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/environment/__init__.py` & `rcmpy-1.5.2/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/environment/base.py` & `rcmpy-1.5.2/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/environment/data.py` & `rcmpy-1.5.2/rcmpy/environment/data.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/environment/template.py` & `rcmpy-1.5.2/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/paths/__init__.py` & `rcmpy-1.5.2/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/schemas.py` & `rcmpy-1.5.2/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/state/__init__.py` & `rcmpy-1.5.2/rcmpy/state/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/watch/__init__.py` & `rcmpy-1.5.2/rcmpy/watch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 
 async def command(*args: str, shell: bool = False) -> int:
     """Run a subprocess and return the return code."""
 
     runner = run_shell if shell else run_command
     proc = await runner(LOG, *args)
-    assert proc.returncode is not None
-    return proc.returncode
+    assert proc.proc.returncode is not None
+    return proc.proc.returncode
 
 
 async def entry(stop_sig: Event, params: WatchParams) -> int:
     """The async entry-point for the watch command."""
 
     cache_file = watch_cache()
```

### Comparing `rcmpy-1.5.1/rcmpy/watch/params.py` & `rcmpy-1.5.2/rcmpy/watch/params.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy/xdg/__init__.py` & `rcmpy-1.5.2/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.5.2/rcmpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.1
+Version: 1.5.2
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=744ace272d6f05ecee63ea172bf1a6bd
+    hash=3c7a54d3f5dd7f524b8ad29c1dee448d
     =====================================
 -->
 
-# rcmpy ([1.5.1](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.2](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
```

### Comparing `rcmpy-1.5.1/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.5.2/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/setup.py` & `rcmpy-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.1/tests/test_entry.py` & `rcmpy-1.5.2/tests/test_entry.py`

 * *Files identical despite different names*

