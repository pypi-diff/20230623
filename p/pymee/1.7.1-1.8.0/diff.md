# Comparing `tmp/pymee-1.7.1.tar.gz` & `tmp/pymee-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymee-1.7.1.tar", last modified: Sun Jun 11 20:05:50 2023, max compression
+gzip compressed data, was "pymee-1.8.0.tar", last modified: Fri Jun 23 14:51:43 2023, max compression
```

## Comparing `pymee-1.7.1.tar` & `pymee-1.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 20:05:50.986852 pymee-1.7.1/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-06-11 20:05:47.000000 pymee-1.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6037 2023-06-11 20:05:50.986852 pymee-1.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5627 2023-06-11 20:05:47.000000 pymee-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 20:05:50.986852 pymee-1.7.1/pymee/
--rw-r--r--   0 root         (0) root         (0)    16494 2023-06-11 20:05:47.000000 pymee-1.7.1/pymee/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26751 2023-06-11 20:05:47.000000 pymee-1.7.1/pymee/const.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-06-11 20:05:47.000000 pymee-1.7.1/pymee/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 20:05:50.986852 pymee-1.7.1/pymee.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6037 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-11 20:05:50.000000 pymee-1.7.1/pymee.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-11 20:05:50.986852 pymee-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      647 2023-06-11 20:05:48.000000 pymee-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:51:43.164933 pymee-1.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-06-23 14:51:39.000000 pymee-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-06-23 14:51:43.164933 pymee-1.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5627 2023-06-23 14:51:39.000000 pymee-1.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:51:43.160933 pymee-1.8.0/pymee/
+-rw-r--r--   0 root         (0) root         (0)    16494 2023-06-23 14:51:39.000000 pymee-1.8.0/pymee/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26751 2023-06-23 14:51:39.000000 pymee-1.8.0/pymee/const.py
+-rw-r--r--   0 root         (0) root         (0)    12787 2023-06-23 14:51:39.000000 pymee-1.8.0/pymee/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:51:43.164933 pymee-1.8.0/pymee.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-06-23 14:51:43.000000 pymee-1.8.0/pymee.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-23 14:51:43.000000 pymee-1.8.0/pymee.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:51:43.000000 pymee-1.8.0/pymee.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 14:51:43.000000 pymee-1.8.0/pymee.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-23 14:51:43.164933 pymee-1.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      647 2023-06-23 14:51:40.000000 pymee-1.8.0/setup.py
```

### Comparing `pymee-1.7.1/LICENSE` & `pymee-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymee-1.7.1/PKG-INFO` & `pymee-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymee
-Version: 1.7.1
+Version: 1.8.0
 Summary: a python library to interact with homee
 Home-page: https://github.com/FreshlyBrewedCode/pymee
 Author: FreshlyBrewedCode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pymee-1.7.1/README.md` & `pymee-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pymee-1.7.1/pymee/__init__.py` & `pymee-1.8.0/pymee/__init__.py`

 * *Files identical despite different names*

### Comparing `pymee-1.7.1/pymee/const.py` & `pymee-1.8.0/pymee/const.py`

 * *Files identical despite different names*

### Comparing `pymee-1.7.1/pymee/model.py` & `pymee-1.8.0/pymee/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,63 @@
 from typing import Callable, List
 from urllib.parse import unquote
 
 
+class HomeeAttributeOptions:
+    def __init__(self, attributeOptions):
+        self._data = attributeOptions
+
+    @property
+    def can_observe(self) -> list:
+        """List (int) of attribute types that this attribute can observe."""
+        if "can_observe" in self._data:
+            return self._data["can_observe"]
+        else:
+            return []
+
+    @property
+    def observes(self) -> list:
+        """List (int) of attribute ids that this attribute observes."""
+        if "observes" in self._data:
+            return self._data["observes"]
+        else:
+            return []
+
+    @property
+    def observed_by(self) -> list:
+        """List (int) of attribute ids that observe this attribute."""
+        if "observed_by" in self._data:
+            return self._data["observed_by"]
+        else:
+            return []
+
+    @property
+    def automations(self) -> list:
+        """List (str) of automations for thie attribute."""
+        if "automations" in self._data:
+            return self._data["automations"]
+        else:
+            return []
+
+    @property
+    def history(self) -> List[dict]:
+        """History data for the attribute. {'day': int, 'week': int, 'month': int, 'stepped': bool}"""
+        if "history" in self._data:
+            return self._data["history"]
+        else:
+            return {}
+
+    @property
+    def reverse_control_ui(self) -> bool:
+        """Do up/down controls work in opposite direction?"""
+        if "reverse_control_ui" in self._data:
+            return self._data["reverse_control_ui"]
+        else:
+            return False
+
 class HomeeAttribute:
     def __init__(self, data: dict) -> None:
         self._data = data
 
     @property
     def id(self) -> int:
         """The unique id of the attribute."""
@@ -97,14 +149,19 @@
         return unquote(self._data["name"])
 
     @property
     def data(self) -> str:
         """The data string of the attribute. Note that the data may be uri encoded."""
         return self._data["data"]
 
+    @property
+    def options(self) -> HomeeAttributeOptions:
+        """The options collection of the attribute. Optional, not on every attribute."""
+        return HomeeAttributeOptions(self._data["options"])
+
 
 class HomeeNode:
     def __init__(self, data: dict) -> None:
         self._data = data
         self.attributes: List[HomeeAttribute] = []
         for a in self.attributes_raw:
             self.attributes.append(HomeeAttribute(a))
@@ -434,8 +491,8 @@
     @property
     def order(self) -> int:
         return self._data["order"]
 
 
 # JSON to Python regex:
 # Match: "([^"]*)":[^,]*,
-# Replace: @property\ndef $1(self):\n\treturn self._data["$1"]\n
+# Replace: @property\ndef $1(self):\n\treturn self._data["$1"]\n
```

### Comparing `pymee-1.7.1/pymee.egg-info/PKG-INFO` & `pymee-1.8.0/pymee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymee
-Version: 1.7.1
+Version: 1.8.0
 Summary: a python library to interact with homee
 Home-page: https://github.com/FreshlyBrewedCode/pymee
 Author: FreshlyBrewedCode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pymee-1.7.1/setup.py` & `pymee-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "1.7.1"
+__version__ = "1.8.0"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymee",
     version=__version__,
```

