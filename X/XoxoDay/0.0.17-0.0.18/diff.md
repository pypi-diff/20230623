# Comparing `tmp/XoxoDay-0.0.17.tar.gz` & `tmp/XoxoDay-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.17.tar", last modified: Fri Jun 23 20:32:40 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.18.tar", last modified: Fri Jun 23 20:35:48 2023, max compression
```

## Comparing `XoxoDay-0.0.17.tar` & `XoxoDay-0.0.18.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:32:40.554107 XoxoDay-0.0.17/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.17/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:32:40.553948 XoxoDay-0.0.17/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.17/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:32:40.549897 XoxoDay-0.0.17/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-23 20:30:02.000000 XoxoDay-0.0.17/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.17/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:32:40.551269 XoxoDay-0.0.17/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.17/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.17/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.17/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.17/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:32:40.553575 XoxoDay-0.0.17/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.17/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.17/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.17/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3049 2023-06-23 20:32:05.000000 XoxoDay-0.0.17/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.17/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.17/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:32:40.550704 XoxoDay-0.0.17/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:32:40.000000 XoxoDay-0.0.17/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-23 20:32:40.000000 XoxoDay-0.0.17/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-23 20:32:40.000000 XoxoDay-0.0.17/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-23 20:32:40.000000 XoxoDay-0.0.17/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-23 20:32:40.000000 XoxoDay-0.0.17/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-23 20:32:40.554148 XoxoDay-0.0.17/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-23 20:29:44.000000 XoxoDay-0.0.17/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.421892 XoxoDay-0.0.18/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.18/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:35:48.421673 XoxoDay-0.0.18/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.18/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.418016 XoxoDay-0.0.18/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-23 20:35:39.000000 XoxoDay-0.0.18/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.18/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.419247 XoxoDay-0.0.18/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.18/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.18/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      942 2023-06-23 20:35:32.000000 XoxoDay-0.0.18/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.18/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.421142 XoxoDay-0.0.18/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.18/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.18/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.18/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3049 2023-06-23 20:32:05.000000 XoxoDay-0.0.18/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.18/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.18/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.418744 XoxoDay-0.0.18/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-23 20:35:48.421946 XoxoDay-0.0.18/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-23 20:35:35.000000 XoxoDay-0.0.18/setup.py
```

### Comparing `XoxoDay-0.0.17/LICENSE` & `XoxoDay-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.17/PKG-INFO` & `XoxoDay-0.0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.17
+Version: 0.0.18
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.17/README.md` & `XoxoDay-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.17/XoxoDay/exception.py` & `XoxoDay-0.0.18/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.17/XoxoDay/helper/sqlite.py` & `XoxoDay-0.0.18/XoxoDay/helper/sqlite.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.17/XoxoDay/helper/token.py` & `XoxoDay-0.0.18/XoxoDay/helper/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sqlite3 as lite
 
 from XoxoDay.exception import XoxoDayException
 from XoxoDay.serializer import Serializer
 
-sql_path = f'{os.path.dirname(os.path.abspath(__file__))}/logo_rest.sqlite'
+sql_path = f'{os.path.dirname(os.path.abspath(__file__))}/xoxo.sqlite'
 
 
 def get_token():
     try:
         with lite.connect(sql_path) as sqlite:
             cursor = sqlite.cursor()
             query = """SELECT token FROM jwt"""
```

### Comparing `XoxoDay-0.0.17/XoxoDay/service/http_service.py` & `XoxoDay-0.0.18/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.17/XoxoDay/service/token_service.py` & `XoxoDay-0.0.18/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.17/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.18/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.17/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.18/XoxoDay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.17
+Version: 0.0.18
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.17/setup.py` & `XoxoDay-0.0.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.17",
+    version="0.0.18",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

