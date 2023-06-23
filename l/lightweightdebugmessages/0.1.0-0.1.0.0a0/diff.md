# Comparing `tmp/lightweightdebugmessages-0.1.0.tar.gz` & `tmp/lightweightdebugmessages-0.1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweightdebugmessages-0.1.0.tar", max compression
+gzip compressed data, was "lightweightdebugmessages-0.1.0.0a0.tar", max compression
```

## Comparing `lightweightdebugmessages-0.1.0.tar` & `lightweightdebugmessages-0.1.0.0a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      732 2023-06-23 04:52:57.821341 lightweightdebugmessages-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-05-31 03:25:27.620372 lightweightdebugmessages-0.1.0/LICENSE
--rw-r--r--   0        0        0     1054 2023-06-23 05:03:31.380099 lightweightdebugmessages-0.1.0/README.md
--rw-r--r--   0        0        0     1626 2023-06-23 05:12:58.778271 lightweightdebugmessages-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5591 2023-06-12 05:18:44.899304 lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/LightweightDebugMessages.py
--rw-r--r--   0        0        0     2461 2023-06-23 04:52:57.821341 lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/__init__.py
--rw-r--r--   0        0        0      158 2023-04-26 02:30:20.708024 lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/unittests/__init__.py
--rw-r--r--   0        0        0     2163 2023-06-12 05:19:41.849282 lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/unittests/common.py
--rw-r--r--   0        0        0     5998 2023-06-12 05:21:56.179243 lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py
--rw-r--r--   0        0        0     2460 2023-06-12 05:17:52.439303 lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/version.py
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 lightweightdebugmessages-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      732 2023-06-23 04:52:57.821341 lightweightdebugmessages-0.1.0.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-05-31 03:25:27.620372 lightweightdebugmessages-0.1.0.0a0/LICENSE
+-rw-r--r--   0        0        0     1054 2023-06-23 05:03:31.380099 lightweightdebugmessages-0.1.0.0a0/README.md
+-rw-r--r--   0        0        0     1629 2023-06-23 05:11:06.415713 lightweightdebugmessages-0.1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5591 2023-06-12 05:18:44.899304 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/LightweightDebugMessages.py
+-rw-r--r--   0        0        0     2461 2023-06-23 04:52:57.821341 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-26 02:30:20.708024 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/__init__.py
+-rw-r--r--   0        0        0     2163 2023-06-12 05:19:41.849282 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/common.py
+-rw-r--r--   0        0        0     5998 2023-06-12 05:21:56.179243 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py
+-rw-r--r--   0        0        0     2460 2023-06-12 05:17:52.439303 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/version.py
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 lightweightdebugmessages-0.1.0.0a0/PKG-INFO
```

### Comparing `lightweightdebugmessages-0.1.0/CHANGELOG.md` & `lightweightdebugmessages-0.1.0.0a0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/LICENSE` & `lightweightdebugmessages-0.1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/README.md` & `lightweightdebugmessages-0.1.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/pyproject.toml` & `lightweightdebugmessages-0.1.0.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "lightweightdebugmessages"
 description = "Helper class for exception handling"
-version = "0.1.0"
+version = "0.1.0.0a"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Debugging",
     "Logging"
 ]
 repository = "https://gitlab.com/semantik-software/code/python/LightweightDebugMessages"
```

### Comparing `lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/LightweightDebugMessages.py` & `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/LightweightDebugMessages.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/__init__.py` & `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/__init__.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/unittests/common.py` & `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/common.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py` & `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/src/lightweightdebugmessages/version.py` & `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/version.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0/PKG-INFO` & `lightweightdebugmessages-0.1.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweightdebugmessages
-Version: 0.1.0
+Version: 0.1.0.0a0
 Summary: Helper class for exception handling
 Home-page: https://gitlab.com/semantik-software/code/python/LightweightDebugMessages
 License: LICENSE
 Keywords: Debugging,Logging
 Author: William McLendon
 Author-email: wcmclen@hotmail.com
 Maintainer: William McLendon
```

