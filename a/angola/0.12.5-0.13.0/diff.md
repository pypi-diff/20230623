# Comparing `tmp/angola-0.12.5.tar.gz` & `tmp/angola-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.12.5.tar", last modified: Sun Jun 18 07:27:57 2023, max compression
+gzip compressed data, was "angola-0.13.0.tar", last modified: Fri Jun 23 04:35:40 2023, max compression
```

## Comparing `angola-0.12.5.tar` & `angola-0.13.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.959443 angola-0.12.5/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.5/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.5/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:27:57.959529 angola-0.12.5/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.5/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-18 07:27:57.959814 angola-0.12.5/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-18 07:27:51.000000 angola-0.12.5/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.951307 angola-0.12.5/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.955516 angola-0.12.5/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.5/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-11 22:47:22.000000 angola-0.12.5/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.5/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.5/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.5/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    20046 2023-06-18 07:26:19.000000 angola-0.12.5/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.957184 angola-0.12.5/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.959319 angola-0.12.5/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.5/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.5/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.5/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.5/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.5/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.852900 angola-0.13.0/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.13.0/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.13.0/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 04:35:40.852969 angola-0.13.0/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.13.0/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-23 04:35:40.853207 angola-0.13.0/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      793 2023-06-23 04:35:13.000000 angola-0.13.0/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.847959 angola-0.13.0/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.850616 angola-0.13.0/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.13.0/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-23 04:30:25.000000 angola-0.13.0/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.13.0/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.13.0/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17512 2023-06-23 04:30:25.000000 angola-0.13.0/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.13.0/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.851390 angola-0.13.0/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       53 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.852797 angola-0.13.0/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.13.0/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.13.0/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.13.0/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.13.0/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.13.0/tests/test_query.py
```

### Comparing `angola-0.12.5/LICENSE` & `angola-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.12.5/PKG-INFO` & `angola-0.13.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.5
+Version: 0.13.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.5/README.md` & `angola-0.13.0/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.12.5/setup.py` & `angola-0.13.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.12.5"
+VERSION = "0.13.0"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
@@ -21,13 +21,13 @@
         'Topic :: Database',
     ],
     python_requires='>=3.8.0',
     install_requires = [
         "Jinja2 >= 3.0",
         "python-slugify",
         "arrow",
-        "python3-xid",
+        "uuid7",
         "python-arango"
     ],
     packages=['angola'],
     package_dir={'':'src'}
 )
```

### Comparing `angola-0.12.5/src/angola/database.py` & `angola-0.13.0/src/angola/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1582,26 +1582,26 @@
 
 #------------------------------------------------------------------------------
 
 def _create_edge_name(from_name, to_name):
     return "edge--%s-%s" % (from_name, to_name)
 
 def _create_document_item(data:dict={}) -> dict:
-    _key = data["_key"] if "_key" in data else lib.gen_key()
+    _key = data["_key"] if "_key" in data else lib.gen_xid()
 
     return {
         "_key": _key,
         "_created_at:$datetime": True,
         "_modified_at": None,
         "__ttl": None,
         **data,
     }
 
 def _create_subdocument_item(data:dict={}) -> dict:
-    _key = data["_key"] if "_key" in data else lib.gen_key()
+    _key = data["_key"] if "_key" in data else lib.gen_xid()
 
     return {
         "_key": _key,
         "_created_at:$datetime": True,
         "_modified_at": None,
         **data,
     }
```

### Comparing `angola-0.12.5/src/angola/dict_mutator.py` & `angola-0.13.0/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.5/src/angola/dict_query.py` & `angola-0.13.0/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.5/src/angola/lib.py` & `angola-0.13.0/src/angola/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # -- Angola --
 #-----------------------------
 
 import os
 import re
 import sys
 import json
-import xid
 import math
 import uuid
 import time
 import arrow
 import string
 import random
 import secrets
 import hashlib
 import datetime
 from slugify import slugify
 from jinja2 import Template
 from functools import reduce
 from operator import itemgetter
 from typing import Iterator, Any
+from uuid_extensions import uuid7
 
 # Date format
 FORMAT_ISO_DATE = "YYYY-MM-DD"
 FORMAT_ISO_TIME = "HH:mm:ss"
 FORMAT_ISO_DATETIME = "YYYY-MM-DD HH:mm:ss"
 
 DATES_FORMAT = {
@@ -60,21 +60,21 @@
     """
     pattern = re.compile(r"^[a-z][a-z0-9\_]{2,64}$")
     return bool(pattern.match(name)) 
 
 
 def gen_xid() -> str:
     """
-    Return XID. 26 Chars
+    Return UUID7. 32 Chars
     """
-    return str(xid.Xid())
+    return str(uuid7()).replace("-", "")
 
 def gen_key() -> str:
     """
-    Return XID. 26 Chars
+    Return UUID7. 32 Chars
     """
     return gen_xid()
     
 def gen_uuid() -> str:
     """
     Return a UUID4 key. 32 chars
     """
```

### Comparing `angola-0.12.5/src/angola/lib_xql.py` & `angola-0.13.0/src/angola/lib_xql.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,16 @@
         k, operator = k.split(":", 2)
         operator = operator.upper()
 
     # literal values starts with `#`
     # it indicates the value should not be converted, but rather return as is without `#`
     # ie:
     # - {k: "@parent.key"} -> k == parent.key
-    # - {k: '$@params_value'} -> k == @params_value
+    # - {k: "#parent.key"} -> k == parent.key
+    # - {k: '#@params_value'} -> k == @params_value
     #
     dlit = isinstance(value, str) and value.startswith("#")
 
     # gen a unique number to make sure values generated are unique
     num_ = lib.gen_number(6)
     ukey = slugify("%s_%s" % (k, num_), separator="_")
     stmt = ""
@@ -405,15 +406,15 @@
     r = {k.upper(): v for k, v in _defaults.items()}
     if r.get("FETCH"):
         r["FROM"] = r.get("FETCH")
     if r.get("AS") :
         r["ALIAS"] = r.get("AS")
     if r.get("SUBQUERIES"):
         r["JOIN"] = r.get("SUBQUERIES")
-        
+
     if r["RETURN"] is None:
         r["RETURN"] = r["ALIAS"]
     return r
 
 
 def xql_take_skip_page(xql: dict, max_limit=100) -> tuple:
     """
```

### Comparing `angola-0.12.5/src/angola.egg-info/PKG-INFO` & `angola-0.13.0/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.5
+Version: 0.13.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.5/tests/test_database.py` & `angola-0.13.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.5/tests/test_dict_mutator.py` & `angola-0.13.0/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.5/tests/test_lib.py` & `angola-0.13.0/tests/test_lib.py`

 * *Files identical despite different names*

