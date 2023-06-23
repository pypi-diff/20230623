# Comparing `tmp/plone.memoize-3.0.1.tar.gz` & `tmp/plone.memoize-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.memoize-3.0.1.tar", last modified: Thu Apr 13 23:12:29 2023, max compression
+gzip compressed data, was "plone.memoize-3.0.2.tar", last modified: Fri Jun 23 17:03:58 2023, max compression
```

## Comparing `plone.memoize-3.0.1.tar` & `plone.memoize-3.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.518461 plone.memoize-3.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     8332 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    14143 2023-04-13 23:12:29.518716 plone.memoize-3.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      595 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.510250 plone.memoize-3.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1519 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/docs/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      366 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/docs/index.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.510527 plone.memoize-3.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.518235 plone.memoize-3.0.1/plone/memoize/
--rw-r--r--   0 maurits    (501) staff       (20)     4137 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      271 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/compress.py
--rw-r--r--   0 maurits    (501) staff       (20)     1354 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/compress.rst
--rw-r--r--   0 maurits    (501) staff       (20)      320 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      541 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/forever.py
--rw-r--r--   0 maurits    (501) staff       (20)     1216 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/forever.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1745 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/instance.py
--rw-r--r--   0 maurits    (501) staff       (20)     4531 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/instance.rst
--rw-r--r--   0 maurits    (501) staff       (20)      680 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2540 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/ram.py
--rw-r--r--   0 maurits    (501) staff       (20)     2645 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/ram.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/request.py
--rw-r--r--   0 maurits    (501) staff       (20)     3509 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/request.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2189 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     2614 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/view.py
--rw-r--r--   0 maurits    (501) staff       (20)     7485 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/view.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2118 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/volatile.py
--rw-r--r--   0 maurits    (501) staff       (20)     7168 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/plone/memoize/volatile.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:12:29.512593 plone.memoize-3.0.1/plone.memoize.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    14143 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      881 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:12:29.000000 plone.memoize-3.0.1/plone.memoize.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1678 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:12:29.519238 plone.memoize-3.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1990 2023-04-13 23:12:28.000000 plone.memoize-3.0.1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-06-23 17:03:58.468073 plone.memoize-3.0.2/
+-rw-r--r--   0 gil       (1000) gil       (1000)     8441 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      149 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    14159 2023-06-23 17:03:58.467072 plone.memoize-3.0.2/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      465 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-06-23 17:03:58.464072 plone.memoize-3.0.2/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1519 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/docs/LICENSE.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      366 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/docs/index.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-06-23 17:03:58.464072 plone.memoize-3.0.2/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-06-23 17:03:58.467072 plone.memoize-3.0.2/plone/memoize/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4137 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/README.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      271 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/compress.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1354 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/compress.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      320 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      541 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/forever.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1216 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/forever.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1745 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/instance.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4531 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/instance.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      680 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2540 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/ram.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2645 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/ram.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     2534 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/request.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3509 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/request.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     2189 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/tests.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2614 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/view.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7485 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/view.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     2118 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/volatile.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7168 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/plone/memoize/volatile.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-06-23 17:03:58.465072 plone.memoize-3.0.2/plone.memoize.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    14159 2023-06-23 17:03:58.000000 plone.memoize-3.0.2/plone.memoize.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      871 2023-06-23 17:03:58.000000 plone.memoize-3.0.2/plone.memoize.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-06-23 17:03:58.000000 plone.memoize-3.0.2/plone.memoize.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-06-23 17:03:58.000000 plone.memoize-3.0.2/plone.memoize.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-06-23 17:03:58.000000 plone.memoize-3.0.2/plone.memoize.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      145 2023-06-23 17:03:58.000000 plone.memoize-3.0.2/plone.memoize.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-06-23 17:03:58.000000 plone.memoize-3.0.2/plone.memoize.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     3838 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)       38 2023-06-23 17:03:58.468073 plone.memoize-3.0.2/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     2040 2023-06-23 17:03:57.000000 plone.memoize-3.0.2/setup.py
```

### Comparing `plone.memoize-3.0.1/CHANGES.rst` & `plone.memoize-3.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-06-23)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (237ff4c8)
+
+
 3.0.1 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.memoize-3.0.1/PKG-INFO` & `plone.memoize-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.memoize
-Version: 3.0.1
+Version: 3.0.2
 Summary: Decorators for caching the values of functions and methods
 Home-page: https://pypi.org/project/plone.memoize
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: plone memoize decorator cache
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,22 +19,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 plone.memoize
 =============
 
-.. image:: https://travis-ci.org/plone/plone.memoize.svg?branch=master
-       :target: https://travis-ci.org/plone/plone.memoize
-
 plone.memoize provides Python function decorators for caching the
 values of functions and methods.
 
 The type of cache storage is freely configurable by the user, as is
 the cache key, which is what the function's value depends on.
 
 plone.memoize has support for memcached and is easily extended to use
@@ -152,14 +150,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-06-23)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (237ff4c8)
+
+
 3.0.1 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.memoize-3.0.1/docs/LICENSE.rst` & `plone.memoize-3.0.2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/README.rst` & `plone.memoize-3.0.2/plone/memoize/README.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/compress.rst` & `plone.memoize-3.0.2/plone/memoize/compress.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/forever.py` & `plone.memoize-3.0.2/plone/memoize/forever.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/forever.rst` & `plone.memoize-3.0.2/plone/memoize/forever.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/instance.py` & `plone.memoize-3.0.2/plone/memoize/instance.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/instance.rst` & `plone.memoize-3.0.2/plone/memoize/instance.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/interfaces.py` & `plone.memoize-3.0.2/plone/memoize/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/ram.py` & `plone.memoize-3.0.2/plone/memoize/ram.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/ram.rst` & `plone.memoize-3.0.2/plone/memoize/ram.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/request.py` & `plone.memoize-3.0.2/plone/memoize/request.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/request.rst` & `plone.memoize-3.0.2/plone/memoize/request.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/tests.py` & `plone.memoize-3.0.2/plone/memoize/tests.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/view.py` & `plone.memoize-3.0.2/plone/memoize/view.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/view.rst` & `plone.memoize-3.0.2/plone/memoize/view.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/volatile.py` & `plone.memoize-3.0.2/plone/memoize/volatile.py`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone/memoize/volatile.rst` & `plone.memoize-3.0.2/plone/memoize/volatile.rst`

 * *Files identical despite different names*

### Comparing `plone.memoize-3.0.1/plone.memoize.egg-info/PKG-INFO` & `plone.memoize-3.0.2/plone.memoize.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.memoize
-Version: 3.0.1
+Version: 3.0.2
 Summary: Decorators for caching the values of functions and methods
 Home-page: https://pypi.org/project/plone.memoize
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: plone memoize decorator cache
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,22 +19,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 plone.memoize
 =============
 
-.. image:: https://travis-ci.org/plone/plone.memoize.svg?branch=master
-       :target: https://travis-ci.org/plone/plone.memoize
-
 plone.memoize provides Python function decorators for caching the
 values of functions and methods.
 
 The type of cache storage is freely configurable by the user, as is
 the cache key, which is what the function's value depends on.
 
 plone.memoize has support for memcached and is easily extended to use
@@ -152,14 +150,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-06-23)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (237ff4c8)
+
+
 3.0.1 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.memoize-3.0.1/plone.memoize.egg-info/SOURCES.txt` & `plone.memoize-3.0.2/plone.memoize.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/LICENSE.rst
 docs/index.rst
 plone/__init__.py
 plone.memoize.egg-info/PKG-INFO
 plone.memoize.egg-info/SOURCES.txt
 plone.memoize.egg-info/dependency_links.txt
```

### Comparing `plone.memoize-3.0.1/setup.py` & `plone.memoize-3.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,28 @@
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
-import os
 
+version = "3.0.2"
 
-def read(*rnames):
-    return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
-
-
-version = "3.0.1"
-
-long_description = "\n".join(
-    [
-        read("README.rst"),
-        read("plone", "memoize", "README.rst"),
-        read("CHANGES.rst"),
-    ]
+long_description = (
+    f"{Path('README.rst').read_text()}\n"
+    f"{(Path('plone') / 'memoize' / 'README.rst').read_text()}\n"
+    f"{Path('CHANGES.rst').read_text()}"
 )
 
-
 setup(
     name="plone.memoize",
     version=version,
     description="Decorators for caching the values of functions and methods",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
+    # Get more strings from
+    # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope :: 5",
@@ -51,20 +46,20 @@
     include_package_data=True,
     zip_safe=False,
     test_suite="plone.memoize.tests.test_suite",
     python_requires=">=3.8",
     extras_require=dict(
         test=[
             "zope.configuration",
-            "zope.globalrequest",
             "zope.publisher",
             "zope.testing",
         ],
     ),
     install_requires=[
         "setuptools",
         "zope.annotation",
         "zope.component",
+        "zope.globalrequest",
         "zope.interface",
         "zope.ramcache",
     ],
 )
```

