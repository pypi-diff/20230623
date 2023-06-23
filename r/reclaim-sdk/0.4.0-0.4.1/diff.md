# Comparing `tmp/reclaim-sdk-0.4.0.tar.gz` & `tmp/reclaim-sdk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reclaim-sdk-0.4.0.tar", last modified: Sun Oct  9 10:10:21 2022, max compression
+gzip compressed data, was "reclaim-sdk-0.4.1.tar", last modified: Fri Jun 23 15:13:07 2023, max compression
```

## Comparing `reclaim-sdk-0.4.0.tar` & `reclaim-sdk-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 llabusch  (1000) llabusch  (1000)        0 2022-10-09 10:10:21.558486 reclaim-sdk-0.4.0/
--rw-r--r--   0 llabusch  (1000) llabusch  (1000)     1073 2022-10-04 12:33:05.000000 reclaim-sdk-0.4.0/LICENSE
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)     5712 2022-10-09 10:10:21.558486 reclaim-sdk-0.4.0/PKG-INFO
--rw-r--r--   0 llabusch  (1000) llabusch  (1000)     5418 2022-10-09 10:10:06.000000 reclaim-sdk-0.4.0/README.md
-drwxrwxr-x   0 llabusch  (1000) llabusch  (1000)        0 2022-10-09 10:10:21.554486 reclaim-sdk-0.4.0/reclaim_sdk/
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)      132 2022-10-06 08:22:22.000000 reclaim-sdk-0.4.0/reclaim_sdk/__init__.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)     2831 2022-10-07 07:53:17.000000 reclaim-sdk-0.4.0/reclaim_sdk/client.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)      310 2022-10-07 06:32:30.000000 reclaim-sdk-0.4.0/reclaim_sdk/exceptions.py
-drwxrwxr-x   0 llabusch  (1000) llabusch  (1000)        0 2022-10-09 10:10:21.558486 reclaim-sdk-0.4.0/reclaim_sdk/models/
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)        0 2022-10-05 08:10:16.000000 reclaim-sdk-0.4.0/reclaim_sdk/models/__init__.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)     5170 2022-10-09 09:58:11.000000 reclaim-sdk-0.4.0/reclaim_sdk/models/model.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)     8192 2022-10-09 09:58:11.000000 reclaim-sdk-0.4.0/reclaim_sdk/models/task.py
--rw-r--r--   0 llabusch  (1000) llabusch  (1000)     2046 2022-10-09 09:58:11.000000 reclaim-sdk-0.4.0/reclaim_sdk/models/task_event.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)      582 2022-10-07 06:17:28.000000 reclaim-sdk-0.4.0/reclaim_sdk/utils.py
-drwxrwxr-x   0 llabusch  (1000) llabusch  (1000)        0 2022-10-09 10:10:21.558486 reclaim-sdk-0.4.0/reclaim_sdk.egg-info/
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)     5712 2022-10-09 10:10:21.000000 reclaim-sdk-0.4.0/reclaim_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)      595 2022-10-09 10:10:21.000000 reclaim-sdk-0.4.0/reclaim_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)        1 2022-10-09 10:10:21.000000 reclaim-sdk-0.4.0/reclaim_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)        1 2022-10-09 10:00:24.000000 reclaim-sdk-0.4.0/reclaim_sdk.egg-info/not-zip-safe
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)       34 2022-10-09 10:10:21.000000 reclaim-sdk-0.4.0/reclaim_sdk.egg-info/requires.txt
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)       29 2022-10-09 10:10:21.000000 reclaim-sdk-0.4.0/reclaim_sdk.egg-info/top_level.txt
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)       38 2022-10-09 10:10:21.558486 reclaim-sdk-0.4.0/setup.cfg
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)      801 2022-10-09 10:10:06.000000 reclaim-sdk-0.4.0/setup.py
-drwxrwxr-x   0 llabusch  (1000) llabusch  (1000)        0 2022-10-09 10:10:21.558486 reclaim-sdk-0.4.0/tests/
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)        0 2022-10-05 09:14:39.000000 reclaim-sdk-0.4.0/tests/__init__.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)      648 2022-10-07 07:36:32.000000 reclaim-sdk-0.4.0/tests/common.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)     1615 2022-10-09 09:58:11.000000 reclaim-sdk-0.4.0/tests/test_task_crud.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)     1400 2022-10-07 07:34:16.000000 reclaim-sdk-0.4.0/tests/test_task_crud_exceptions.py
--rw-r--r--   0 llabusch  (1000) llabusch  (1000)     1641 2022-10-09 09:58:11.000000 reclaim-sdk-0.4.0/tests/test_task_event_crud.py
--rw-rw-r--   0 llabusch  (1000) llabusch  (1000)      535 2022-10-05 13:42:11.000000 reclaim-sdk-0.4.0/tests/test_task_search.py
+drwxr-xr-x   0 llabusch  (1000) llabusch  (1000)        0 2023-06-23 15:13:07.181694 reclaim-sdk-0.4.1/
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     1073 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/LICENSE
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     5610 2023-06-23 15:13:07.181694 reclaim-sdk-0.4.1/PKG-INFO
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     5316 2023-06-23 15:09:48.000000 reclaim-sdk-0.4.1/README.md
+drwxr-xr-x   0 llabusch  (1000) llabusch  (1000)        0 2023-06-23 15:13:07.178361 reclaim-sdk-0.4.1/reclaim_sdk/
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)      132 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/reclaim_sdk/__init__.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     2824 2023-06-23 15:09:48.000000 reclaim-sdk-0.4.1/reclaim_sdk/client.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)      310 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/reclaim_sdk/exceptions.py
+drwxr-xr-x   0 llabusch  (1000) llabusch  (1000)        0 2023-06-23 15:13:07.181694 reclaim-sdk-0.4.1/reclaim_sdk/models/
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)        0 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/reclaim_sdk/models/__init__.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     5170 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/reclaim_sdk/models/model.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     8192 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/reclaim_sdk/models/task.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     2046 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/reclaim_sdk/models/task_event.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)      582 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/reclaim_sdk/utils.py
+drwxr-xr-x   0 llabusch  (1000) llabusch  (1000)        0 2023-06-23 15:13:07.181694 reclaim-sdk-0.4.1/reclaim_sdk.egg-info/
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     5610 2023-06-23 15:13:07.000000 reclaim-sdk-0.4.1/reclaim_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)      595 2023-06-23 15:13:07.000000 reclaim-sdk-0.4.1/reclaim_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)        1 2023-06-23 15:13:07.000000 reclaim-sdk-0.4.1/reclaim_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)        1 2023-06-23 15:13:07.000000 reclaim-sdk-0.4.1/reclaim_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)       34 2023-06-23 15:13:07.000000 reclaim-sdk-0.4.1/reclaim_sdk.egg-info/requires.txt
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)       18 2023-06-23 15:13:07.000000 reclaim-sdk-0.4.1/reclaim_sdk.egg-info/top_level.txt
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)       38 2023-06-23 15:13:07.181694 reclaim-sdk-0.4.1/setup.cfg
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)      801 2023-06-23 15:09:48.000000 reclaim-sdk-0.4.1/setup.py
+drwxr-xr-x   0 llabusch  (1000) llabusch  (1000)        0 2023-06-23 15:13:07.181694 reclaim-sdk-0.4.1/tests/
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)        0 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/tests/__init__.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)      648 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/tests/common.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     1615 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/tests/test_task_crud.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     1400 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/tests/test_task_crud_exceptions.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)     1641 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/tests/test_task_event_crud.py
+-rw-r--r--   0 llabusch  (1000) llabusch  (1000)      535 2023-06-23 14:45:26.000000 reclaim-sdk-0.4.1/tests/test_task_search.py
```

### Comparing `reclaim-sdk-0.4.0/LICENSE` & `reclaim-sdk-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/PKG-INFO` & `reclaim-sdk-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reclaim-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: Unofficial Reclaim.ai Python API
 Home-page: https://github.com/llabusch93/reclaim-sdk
 Author: Laurence Lars Labusch
 Author-email: llabusch@labusch-it.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,15 +20,15 @@
 ## Installation
 
 ```bash
 pip install reclaim-sdk
 ```
 
 ## Configuration
-The only configuration needed is the token. You can get it from the Reclaim.ai web app, by copying it from the browser's developer tools. It's stored in the cookie named `RECLAIM`.
+You can get an API key from [here](https://app.reclaim.ai/settings/developer).
 
 There are 3 ways to configure the token:
 
 1. You can initiate the `ReclaimClient` class with the token as the `token` argument. As `ReclaimClient` is a singleton, you should initiate this class at the beginning of your script / program. It will be used for all subsequent calls.
 2. You can set the environment variable `RECLAIM_TOKEN` to the token.
 3. You can store the token in a toml file named `.reclaim.toml` in your home directory. It should look like this:
```

### Comparing `reclaim-sdk-0.4.0/README.md` & `reclaim-sdk-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ## Installation
 
 ```bash
 pip install reclaim-sdk
 ```
 
 ## Configuration
-The only configuration needed is the token. You can get it from the Reclaim.ai web app, by copying it from the browser's developer tools. It's stored in the cookie named `RECLAIM`.
+You can get an API key from [here](https://app.reclaim.ai/settings/developer).
 
 There are 3 ways to configure the token:
 
 1. You can initiate the `ReclaimClient` class with the token as the `token` argument. As `ReclaimClient` is a singleton, you should initiate this class at the beginning of your script / program. It will be used for all subsequent calls.
 2. You can set the environment variable `RECLAIM_TOKEN` to the token.
 3. You can store the token in a toml file named `.reclaim.toml` in your home directory. It should look like this:
```

### Comparing `reclaim-sdk-0.4.0/reclaim_sdk/client.py` & `reclaim-sdk-0.4.1/reclaim_sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         if self._token:
             self.authenticate(self._token)
 
         else:
             raise ValueError("No Reclaim.ai token provided.")
 
-    def authenticate(self, token):
+    def authenticate(self):
         """
         Authenticate the client with the given token.
         """
         self.cookies.set("RECLAIM", self._token)
 
 
 class ReclaimAPICall(object):
```

### Comparing `reclaim-sdk-0.4.0/reclaim_sdk/models/model.py` & `reclaim-sdk-0.4.1/reclaim_sdk/models/model.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/reclaim_sdk/models/task.py` & `reclaim-sdk-0.4.1/reclaim_sdk/models/task.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/reclaim_sdk/models/task_event.py` & `reclaim-sdk-0.4.1/reclaim_sdk/models/task_event.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/reclaim_sdk/utils.py` & `reclaim-sdk-0.4.1/reclaim_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/reclaim_sdk.egg-info/PKG-INFO` & `reclaim-sdk-0.4.1/reclaim_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reclaim-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: Unofficial Reclaim.ai Python API
 Home-page: https://github.com/llabusch93/reclaim-sdk
 Author: Laurence Lars Labusch
 Author-email: llabusch@labusch-it.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,15 +20,15 @@
 ## Installation
 
 ```bash
 pip install reclaim-sdk
 ```
 
 ## Configuration
-The only configuration needed is the token. You can get it from the Reclaim.ai web app, by copying it from the browser's developer tools. It's stored in the cookie named `RECLAIM`.
+You can get an API key from [here](https://app.reclaim.ai/settings/developer).
 
 There are 3 ways to configure the token:
 
 1. You can initiate the `ReclaimClient` class with the token as the `token` argument. As `ReclaimClient` is a singleton, you should initiate this class at the beginning of your script / program. It will be used for all subsequent calls.
 2. You can set the environment variable `RECLAIM_TOKEN` to the token.
 3. You can store the token in a toml file named `.reclaim.toml` in your home directory. It should look like this:
```

### Comparing `reclaim-sdk-0.4.0/reclaim_sdk.egg-info/SOURCES.txt` & `reclaim-sdk-0.4.1/reclaim_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/setup.py` & `reclaim-sdk-0.4.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Read the README.md file for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="reclaim-sdk",
-    version="0.4.0",
+    version="0.4.1",
     description="Unofficial Reclaim.ai Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/llabusch93/reclaim-sdk",
     author="Laurence Lars Labusch",
     author_email="llabusch@labusch-it.com",
     license="MIT",
```

### Comparing `reclaim-sdk-0.4.0/tests/common.py` & `reclaim-sdk-0.4.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/tests/test_task_crud.py` & `reclaim-sdk-0.4.1/tests/test_task_crud.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/tests/test_task_crud_exceptions.py` & `reclaim-sdk-0.4.1/tests/test_task_crud_exceptions.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/tests/test_task_event_crud.py` & `reclaim-sdk-0.4.1/tests/test_task_event_crud.py`

 * *Files identical despite different names*

### Comparing `reclaim-sdk-0.4.0/tests/test_task_search.py` & `reclaim-sdk-0.4.1/tests/test_task_search.py`

 * *Files identical despite different names*

