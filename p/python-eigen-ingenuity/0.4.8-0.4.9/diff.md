# Comparing `tmp/python-eigen-ingenuity-0.4.8.tar.gz` & `tmp/python-eigen-ingenuity-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-eigen-ingenuity-0.4.8.tar", last modified: Wed Jun  7 12:12:42 2023, max compression
+gzip compressed data, was "python-eigen-ingenuity-0.4.9.tar", last modified: Thu Jun  8 12:21:51 2023, max compression
```

## Comparing `python-eigen-ingenuity-0.4.8.tar` & `python-eigen-ingenuity-0.4.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.729014 python-eigen-ingenuity-0.4.8/
--rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/LICENSE
--rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.8/MANIFEST.in
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-07 12:12:42.728734 python-eigen-ingenuity-0.4.8/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/README.md
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.727292 python-eigen-ingenuity-0.4.8/eigeningenuity/
--rw-r--r--   0 berhic     (501) staff       (20)     1205 2023-05-23 15:38:30.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/assetmodel.py
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.727647 python-eigen-ingenuity-0.4.8/eigeningenuity/core/
--rw-r--r--   0 berhic     (501) staff       (20)     7741 2023-05-23 15:25:59.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/core/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/core/debug.py
--rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/elastic.py
--rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/events.py
--rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-24 08:12:38.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/historian.py
--rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/smartdash.py
--rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/sql.py
--rw-r--r--   0 berhic     (501) staff       (20)    15067 2023-06-07 12:09:52.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/util.py
--rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/pyproject.toml
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.728508 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)      551 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/SOURCES.txt
--rw-r--r--   0 berhic     (501) staff       (20)        1 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/dependency_links.txt
--rw-r--r--   0 berhic     (501) staff       (20)       24 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/requires.txt
--rw-r--r--   0 berhic     (501) staff       (20)       15 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/top_level.txt
--rw-r--r--   0 berhic     (501) staff       (20)       38 2023-06-07 12:12:42.729074 python-eigen-ingenuity-0.4.8/setup.cfg
--rw-r--r--   0 berhic     (501) staff       (20)      689 2023-06-07 12:12:34.000000 python-eigen-ingenuity-0.4.8/setup.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 12:21:51.098888 python-eigen-ingenuity-0.4.9/
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.9/LICENSE
+-rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.9/MANIFEST.in
+-rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-08 12:21:51.098634 python-eigen-ingenuity-0.4.9/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.9/README.md
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 12:21:51.097034 python-eigen-ingenuity-0.4.9/eigeningenuity/
+-rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-06-08 09:07:24.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/assetmodel.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 12:21:51.097511 python-eigen-ingenuity-0.4.9/eigeningenuity/core/
+-rw-r--r--   0 berhic     (501) staff       (20)     7741 2023-05-23 15:25:59.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/core/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/core/debug.py
+-rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/elastic.py
+-rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/events.py
+-rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-24 08:12:38.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/historian.py
+-rw-r--r--   0 berhic     (501) staff       (20)      124 2023-06-08 12:21:31.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/settings.py
+-rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/smartdash.py
+-rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/sql.py
+-rw-r--r--   0 berhic     (501) staff       (20)    15930 2023-06-08 12:15:08.000000 python-eigen-ingenuity-0.4.9/eigeningenuity/util.py
+-rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.9/pyproject.toml
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 12:21:51.098394 python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/
+-rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-08 12:21:51.000000 python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2023-06-08 12:21:51.000000 python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/SOURCES.txt
+-rw-r--r--   0 berhic     (501) staff       (20)        1 2023-06-08 12:21:51.000000 python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/dependency_links.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       37 2023-06-08 12:21:51.000000 python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/requires.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       15 2023-06-08 12:21:51.000000 python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/top_level.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       38 2023-06-08 12:21:51.098942 python-eigen-ingenuity-0.4.9/setup.cfg
+-rw-r--r--   0 berhic     (501) staff       (20)      748 2023-06-08 12:21:44.000000 python-eigen-ingenuity-0.4.9/setup.py
```

### Comparing `python-eigen-ingenuity-0.4.8/LICENSE` & `python-eigen-ingenuity-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/PKG-INFO` & `python-eigen-ingenuity-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.8/README.md` & `python-eigen-ingenuity-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/__init__.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 from eigeningenuity.assetmodel import get_assetmodel
 from eigeningenuity.smartdash import get_smartdash
 from eigeningenuity.sql import get_sql
 
 from eigeningenuity.core import *
 
 __all__ = ["get_historian", "get_assetmodel", "get_elastic", "get_sql", "get_eventlog", "get_smartdash", "list_historians", "get_default_historian_name", "EigenServer"]
-# __version__ = pkg_resources.require("python-eigen-ingenuity")[0].version
+__version__ = pkg_resources.require("python-eigen-ingenuity")[0].version
```

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/assetmodel.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/assetmodel.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/core/__init__.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/core/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/core/debug.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/core/debug.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/elastic.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/elastic.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/events.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/events.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/historian.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/historian.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/smartdash.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/smartdash.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/sql.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/sql.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/util.py` & `python-eigen-ingenuity-0.4.9/eigeningenuity/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 
-import sys, os, json, time, requests, csv, msal, atexit
+import sys, os, json, time, requests, csv, msal, atexit, keyring
 from datetime import datetime
 import pandas as pd
 from collections import ChainMap
 from urllib.parse import urlsplit, quote as urlquote
+from cryptography.fernet import Fernet
 
 from requests.exceptions import ConnectionError
-
 from eigeningenuity.core.debug import _debug
+import eigeningenuity.settings as settings
 
-def _authenticate_azure_user(baseurl):
-    cache = msal.SerializableTokenCache()
+cache = msal.SerializableTokenCache()
 
-    if not os.path.exists(os.path.dirname(__file__) + '/.azure'):
-        os.mkdir(os.path.dirname(__file__) + "/.azure")
-    if os.path.exists(os.path.dirname(__file__) + "/.azure/token_cache.bin"):
-        cache.deserialize(open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "r").read())
-    atexit.register(lambda:
-        open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "w").write(cache.serialize())
-        if cache.has_state_changed else None
-        )
+def encrypt(data,key):
+        cipher_suite = Fernet(key)
+        encrypted_data = cipher_suite.encrypt(data.encode())
+        return encrypted_data
+
+def decrypt(data,key):
+    cipher_suite = Fernet(key)
+    decrypted_data = cipher_suite.decrypt(data).decode()
+    return decrypted_data
+
+def _authenticate_azure_user(baseurl):
+    if settings._token_cache_enabled_:
+        global cache
+        try:
+            encryptionKey = keyring.get_password("eigeningenuity","python")
+        except:
+            pass
+
+        if not os.path.exists(os.path.dirname(__file__) + '/.azure'):
+            os.mkdir(os.path.dirname(__file__) + "/.azure")
+
+        if os.path.exists(os.path.dirname(__file__) + "/.azure/token_cache.bin"):
+            encryptedToken = open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "rb").read()
+            if encryptedToken != b'':
+                cache.deserialize(decrypt(encryptedToken,encryptionKey))
+        
+        encryptionKey = Fernet.generate_key().decode('utf-8')
+
+
+        atexit.register(lambda:
+            open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "wb").write(encrypt(cache.serialize(),encryptionKey)) and keyring.set_password("eigeningenuity","python",encryptionKey)
+            if cache.has_state_changed else None
+            )
 
     client_id = os.environ["CLIENTID"]
     tenant_id = os.environ["TENANTID"]
     authority = f'https://login.microsoftonline.com/{tenant_id}'
     scope=[f"{baseurl}/user_impersonation"]
 
     app = msal.PublicClientApplication(
```

### Comparing `python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/PKG-INFO` & `python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/SOURCES.txt` & `python-eigen-ingenuity-0.4.9/python_eigen_ingenuity.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.py
 eigeningenuity/__init__.py
 eigeningenuity/assetmodel.py
 eigeningenuity/elastic.py
 eigeningenuity/events.py
 eigeningenuity/historian.py
+eigeningenuity/settings.py
 eigeningenuity/smartdash.py
 eigeningenuity/sql.py
 eigeningenuity/util.py
 eigeningenuity/core/__init__.py
 eigeningenuity/core/debug.py
 python_eigen_ingenuity.egg-info/PKG-INFO
 python_eigen_ingenuity.egg-info/SOURCES.txt
```

### Comparing `python-eigen-ingenuity-0.4.8/setup.py` & `python-eigen-ingenuity-0.4.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 README = (HERE / "README.md").read_text()
 
 pkgname = 'python-eigen-ingenuity'
 
 # Invoke setup
 setup(
     name=pkgname,
-    version='0.4.8',
+    version='0.4.9',
     author='Murray Callander',
     author_email='info@eigen.co',
     url='https://www.eigen.co/',
     description="A python library used to query data from the Eigen Ingenuity system",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages("."),
     license='Apache License 2.0',
     install_requires=["pandas",
                     "requests",
-                    "urllib3"],
+                    "urllib3",
+                    "msal",
+                    "keyring"],
 )
```

