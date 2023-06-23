# Comparing `tmp/plemmy-0.2.2.tar.gz` & `tmp/plemmy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.2.2.tar", last modified: Wed Jun 21 17:46:16 2023, max compression
+gzip compressed data, was "plemmy-0.2.3.tar", last modified: Fri Jun 23 19:25:50 2023, max compression
```

## Comparing `plemmy-0.2.2.tar` & `plemmy-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-21 17:46:16.201411 plemmy-0.2.2/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.2/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-21 17:46:16.201255 plemmy-0.2.2/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.2/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-21 17:46:16.200144 plemmy-0.2.2/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.2/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    30174 2023-06-21 17:41:59.000000 plemmy-0.2.2/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     1592 2023-06-21 17:42:05.000000 plemmy-0.2.2/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-21 17:41:42.000000 plemmy-0.2.2/plemmy/version.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-21 17:46:16.201024 plemmy-0.2.2/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-21 17:46:16.000000 plemmy-0.2.2/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-21 17:46:16.201457 plemmy-0.2.2/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.2/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-23 19:25:50.818475 plemmy-0.2.3/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.2.3/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-23 19:25:50.818292 plemmy-0.2.3/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1675 2023-06-20 22:25:52.000000 plemmy-0.2.3/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-23 19:25:50.817187 plemmy-0.2.3/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      140 2023-06-20 19:47:16.000000 plemmy-0.2.3/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    70944 2023-06-23 19:23:23.000000 plemmy-0.2.3/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2803 2023-06-23 18:44:09.000000 plemmy-0.2.3/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-06-23 19:24:36.000000 plemmy-0.2.3/plemmy/version.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-06-23 19:25:50.818067 plemmy-0.2.3/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     1961 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      277 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-06-23 19:25:50.000000 plemmy-0.2.3/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-06-23 19:25:50.818524 plemmy-0.2.3/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.2.3/setup.py
```

### Comparing `plemmy-0.2.2/LICENSE` & `plemmy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.2/PKG-INFO` & `plemmy-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.2/README.md` & `plemmy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `plemmy-0.2.2/plemmy/utils.py` & `plemmy-0.2.3/plemmy/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,88 @@
 import logging
 import requests
 
 
 def post_handler(url: str, headers: dict, json: dict) -> requests.Response:
+    """ post_handler: handles all POST operations for Plemmy
+
+    Args:
+        url (str): Lemmy API URL
+        headers (dict): optional headers
+        json (dict): json/form data to be posted
+
+    Returns:
+        requests.Response: server response for POST operation
+    """
 
     logger = logging.getLogger(__name__)
     try:
         re = requests.post(url, headers=headers, json=json)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"POST error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
 
 
 def put_handler(url: str, headers: dict, json: dict) -> requests.Response:
+    """ put_handler: handles all PUT operations for Plemmy
+
+    Args:
+        url (str): Lemmy API URL
+        headers (dict): optional headers
+        json (dict): json/form data being supplied
+
+    Returns:
+        requests.Response: server response for PUT operation
+    """
 
     logger = logging.getLogger(__name__)
     try:
         re = requests.put(url, headers=headers, json=json)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"PUT error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
 
 
 def get_handler(url: str, headers: dict, json: dict,
                 params: dict = None) -> requests.Response:
+    """ get_handler: handles all GET operations for Plemmy
+
+    Args:
+        url (str): Lemmy API URL
+        headers (dict): optional headers
+        json (dict): json/form data
+        params (dict): parameters for GET operation
+
+    Returns:
+        requests.Response: server response for GET operation
+    """
 
     logger = logging.getLogger(__name__)
     try:
         re = requests.get(url, headers=headers, json=json, params=params)
         logger.debug(f"Code: {re.status_code}")
     except requests.exceptions.RequestException as ex:
         logger.error(f"GET error: {ex}\n\nURL: {url}" +
                      f"\nheaders: {headers}\njson: {json}")
         return None
     return re
 
 
 def create_form(arguments: dict) -> dict:
+    """ create_form: creates a dictionary out of supplied arguments (derived
+    from locals()); resulting dict is in form {"arg1", arg1, ... "argN", argN}
+
+    Args:
+        arguments (dict): function arguments supplied with locals()
+
+    Returns:
+        dict: constructed dictionary/form
+    """
 
     return {k: v for k, v in arguments.items()
             if v is not None and k != "self"}
```

### Comparing `plemmy-0.2.2/plemmy.egg-info/PKG-INFO` & `plemmy-0.2.3/plemmy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `plemmy-0.2.2/setup.py` & `plemmy-0.2.3/setup.py`

 * *Files identical despite different names*

