# Comparing `tmp/maltsev_repeater-1.0.0.tar.gz` & `tmp/maltsev_repeater-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maltsev_repeater-1.0.0.tar", max compression
+gzip compressed data, was "maltsev_repeater-1.0.1.tar", max compression
```

## Comparing `maltsev_repeater-1.0.0.tar` & `maltsev_repeater-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-04-29 08:37:20.253115 maltsev_repeater-1.0.0/LICENSE
--rw-r--r--   0        0        0     2292 2023-06-23 03:19:32.819853 maltsev_repeater-1.0.0/README.md
--rw-r--r--   0        0        0      231 2023-06-23 03:14:02.797907 maltsev_repeater-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-20 17:58:42.732219 maltsev_repeater-1.0.0/src/maltsev_repeater/__init__.py
--rw-r--r--   0        0        0     2059 2023-06-23 03:14:26.866053 maltsev_repeater-1.0.0/src/maltsev_repeater/repeater.py
--rw-r--r--   0        0        0     1466 2023-04-30 12:17:28.689757 maltsev_repeater-1.0.0/src/maltsev_repeater/repeater_result.py
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 maltsev_repeater-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-29 08:37:20.253115 maltsev_repeater-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2292 2023-06-23 03:45:44.325294 maltsev_repeater-1.0.1/README.md
+-rw-r--r--   0        0        0      231 2023-06-23 03:47:28.397021 maltsev_repeater-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 03:45:44.325294 maltsev_repeater-1.0.1/src/maltsev_repeater/__init__.py
+-rw-r--r--   0        0        0     2039 2023-06-23 03:45:52.740916 maltsev_repeater-1.0.1/src/maltsev_repeater/repeater.py
+-rw-r--r--   0        0        0     1466 2023-06-23 03:45:44.325294 maltsev_repeater-1.0.1/src/maltsev_repeater/repeater_result.py
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 maltsev_repeater-1.0.1/PKG-INFO
```

### Comparing `maltsev_repeater-1.0.0/LICENSE` & `maltsev_repeater-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maltsev_repeater-1.0.0/README.md` & `maltsev_repeater-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `maltsev_repeater-1.0.0/src/maltsev_repeater/repeater.py` & `maltsev_repeater-1.0.1/src/maltsev_repeater/repeater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from time import sleep
 from typing import Any
 
-from src.maltsev_repeater.repeater_result import RepeaterResult
+from .repeater_result import RepeaterResult
 
 
 class Repeater:
     __action: Any = None
     __attempts: int = None
     __delay: float = None
```

### Comparing `maltsev_repeater-1.0.0/src/maltsev_repeater/repeater_result.py` & `maltsev_repeater-1.0.1/src/maltsev_repeater/repeater_result.py`

 * *Files identical despite different names*

### Comparing `maltsev_repeater-1.0.0/PKG-INFO` & `maltsev_repeater-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maltsev-repeater
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Home-page: https://github.com/victormaltsev/Maltsev.Repeater
 License: MIT
 Author: Victor Maltsev
 Author-email: git@victormaltsev.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

