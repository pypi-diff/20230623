# Comparing `tmp/pluthon-0.3.8.tar.gz` & `tmp/pluthon-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluthon-0.3.8.tar", last modified: Fri Jun 23 06:01:25 2023, max compression
+gzip compressed data, was "pluthon-0.3.9.tar", last modified: Fri Jun 23 06:11:29 2023, max compression
```

## Comparing `pluthon-0.3.8.tar` & `pluthon-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-06-23 06:01:25.919825 pluthon-0.3.8/
--rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-06-23 06:01:25.919825 pluthon-0.3.8/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1001 2023-06-23 06:00:13.000000 pluthon-0.3.8/README.md
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-06-23 06:01:25.919825 pluthon-0.3.8/pluthon/
--rw-r--r--   0 travis    (1000) travis    (1000)      594 2023-06-23 06:00:13.000000 pluthon-0.3.8/pluthon/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4914 2023-06-23 06:00:13.000000 pluthon-0.3.8/pluthon/pluthon_ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2582 2023-06-23 06:00:13.000000 pluthon-0.3.8/pluthon/pluthon_functional_data.py
--rw-r--r--   0 travis    (1000) travis    (1000)    18285 2023-06-23 06:00:13.000000 pluthon-0.3.8/pluthon/pluthon_sugar.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-06-23 06:01:25.919825 pluthon-0.3.8/pluthon.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-06-23 06:01:25.000000 pluthon-0.3.8/pluthon.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      275 2023-06-23 06:01:25.000000 pluthon-0.3.8/pluthon.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-06-23 06:01:25.000000 pluthon-0.3.8/pluthon.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       23 2023-06-23 06:01:25.000000 pluthon-0.3.8/pluthon.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       13 2023-06-23 06:01:25.000000 pluthon-0.3.8/pluthon.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-06-23 06:01:25.919825 pluthon-0.3.8/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1696 2023-06-23 06:00:13.000000 pluthon-0.3.8/setup.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-06-23 06:11:29.967944 pluthon-0.3.9/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-06-23 06:11:29.967944 pluthon-0.3.9/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1001 2023-06-23 06:10:16.000000 pluthon-0.3.9/README.md
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-06-23 06:11:29.963944 pluthon-0.3.9/pluthon/
+-rw-r--r--   0 travis    (1000) travis    (1000)      594 2023-06-23 06:10:16.000000 pluthon-0.3.9/pluthon/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4914 2023-06-23 06:10:16.000000 pluthon-0.3.9/pluthon/pluthon_ast.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2582 2023-06-23 06:10:16.000000 pluthon-0.3.9/pluthon/pluthon_functional_data.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    18295 2023-06-23 06:10:16.000000 pluthon-0.3.9/pluthon/pluthon_sugar.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-06-23 06:11:29.967944 pluthon-0.3.9/pluthon.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1776 2023-06-23 06:11:29.000000 pluthon-0.3.9/pluthon.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      275 2023-06-23 06:11:29.000000 pluthon-0.3.9/pluthon.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-06-23 06:11:29.000000 pluthon-0.3.9/pluthon.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       23 2023-06-23 06:11:29.000000 pluthon-0.3.9/pluthon.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       13 2023-06-23 06:11:29.000000 pluthon-0.3.9/pluthon.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-06-23 06:11:29.967944 pluthon-0.3.9/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1696 2023-06-23 06:10:16.000000 pluthon-0.3.9/setup.py
```

### Comparing `pluthon-0.3.8/PKG-INFO` & `pluthon-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/imperatorlang/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.3.8/README.md` & `pluthon-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.8/pluthon/__init__.py` & `pluthon-0.3.9/pluthon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from .pluthon_functional_data import *
 except ImportError as e:
     logging.error(
         "Error, trying to import dependencies. Should only occur upon package installation",
         exc_info=e,
     )
 
-VERSION = (0, 3, 8)
+VERSION = (0, 3, 9)
 
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "nielstron"
 __author_email__ = "n.muendler@web.de"
 __copyright__ = "Copyright (C) 2023 nielstron"
 __license__ = "MIT"
 __url__ = "https://github.com/imperatorlang/pluthon"
```

### Comparing `pluthon-0.3.8/pluthon/pluthon_ast.py` & `pluthon-0.3.9/pluthon/pluthon_ast.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.8/pluthon/pluthon_functional_data.py` & `pluthon-0.3.9/pluthon/pluthon_functional_data.py`

 * *Files identical despite different names*

### Comparing `pluthon-0.3.8/pluthon/pluthon_sugar.py` & `pluthon-0.3.9/pluthon/pluthon_sugar.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,15 @@
 
 
 def _concat(append, empty):
     def f(*ss: typing.List[AST]):
         if not ss:
             return empty
         c = ss[-1]
-        for s in ss[:-1]:
+        for s in reversed(ss[:-1]):
             c = append(s, c)
         return c
 
     return f
 
 
 ConcatString = _concat(AppendString, Text(""))
```

### Comparing `pluthon-0.3.8/pluthon.egg-info/PKG-INFO` & `pluthon-0.3.9/pluthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluthon
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pluto-like programming language for Cardano Smart Contracts in Python
 Home-page: https://github.com/imperatorlang/pluthon
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pluthon-0.3.8/setup.py` & `pluthon-0.3.9/setup.py`

 * *Files identical despite different names*

