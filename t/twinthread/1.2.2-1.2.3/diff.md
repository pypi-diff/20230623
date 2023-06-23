# Comparing `tmp/twinthread-1.2.2.tar.gz` & `tmp/twinthread-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinthread-1.2.2.tar", max compression
+gzip compressed data, was "twinthread-1.2.3.tar", max compression
```

## Comparing `twinthread-1.2.2.tar` & `twinthread-1.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      457 2023-03-02 17:34:26.368862 twinthread-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    12469 2023-03-02 17:35:43.413090 twinthread-1.2.2/twinthread/__init__.py
--rw-r--r--   0        0        0      660 2022-01-18 16:12:09.250822 twinthread-1.2.2/twinthread/exec_task.py
--rw-r--r--   0        0        0     3247 2022-01-18 16:12:09.251027 twinthread-1.2.2/twinthread/jupyter.py
--rw-r--r--   0        0        0      725 2022-01-18 16:12:09.251186 twinthread-1.2.2/twinthread/string.py
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 twinthread-1.2.2/setup.py
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 twinthread-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-06-23 20:58:04.570400 twinthread-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    12520 2023-06-23 20:58:04.570855 twinthread-1.2.3/twinthread/__init__.py
+-rw-r--r--   0        0        0      660 2023-06-20 21:09:20.015296 twinthread-1.2.3/twinthread/exec_task.py
+-rw-r--r--   0        0        0     3247 2023-06-20 21:09:20.015428 twinthread-1.2.3/twinthread/jupyter.py
+-rw-r--r--   0        0        0      725 2023-06-20 21:09:20.015543 twinthread-1.2.3/twinthread/string.py
+-rw-r--r--   0        0        0      296 2023-06-22 15:31:37.239496 twinthread-1.2.3/twinthread/testing.py
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 twinthread-1.2.3/PKG-INFO
```

### Comparing `twinthread-1.2.2/twinthread/__init__.py` & `twinthread-1.2.3/twinthread/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from _plotly_utils.utils import PlotlyJSONEncoder
 
 from .jupyter import register_jupyter
 from .string import task_string_to_context
 
 __author__ = """Brad Johnson"""
 __email__ = "brad.johnson@twinthread.com"
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 import re
 import json
 import simplejson
 import requests
 import pandas as pd
 from io import StringIO
@@ -27,21 +27,22 @@
     fig = plt.figure()
     fig.axes.append(subplot)
     return fig
 
 
 def do_login(base_url, username):
     import getpass
-
-    password = getpass.getpass("Password?")
+    bi_key = getpass.getpass(f"Enter Active BI Key from {base_url}/settings: ")
     response = requests.post(
-        f"{base_url}/Token",
-        {"grant_type": "password", "username": username, "password": password},
+        f"{base_url}/Account/TokenExchange",
+        {
+            "username": username,
+            "key": bi_key
+        },
     )
-
     if response.status_code != 200:
         raise Exception("Invalid credentials")
 
     print("Login succeeded")
 
     return response.json()["access_token"]
```

### Comparing `twinthread-1.2.2/twinthread/exec_task.py` & `twinthread-1.2.3/twinthread/exec_task.py`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.2/twinthread/jupyter.py` & `twinthread-1.2.3/twinthread/jupyter.py`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.2/twinthread/string.py` & `twinthread-1.2.3/twinthread/string.py`

 * *Files identical despite different names*

### Comparing `twinthread-1.2.2/PKG-INFO` & `twinthread-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinthread
-Version: 1.2.2
+Version: 1.2.3
 Summary: 
 Author: Brent Baumgartner
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

