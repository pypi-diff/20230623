# Comparing `tmp/XoxoDay-0.0.21.tar.gz` & `tmp/XoxoDay-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.21.tar", last modified: Fri Jun 23 21:29:01 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.22.tar", last modified: Fri Jun 23 21:46:17 2023, max compression
```

## Comparing `XoxoDay-0.0.21.tar` & `XoxoDay-0.0.22.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:29:01.713235 XoxoDay-0.0.21/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.21/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 21:29:01.713101 XoxoDay-0.0.21/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.21/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:29:01.709992 XoxoDay-0.0.21/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-23 21:28:52.000000 XoxoDay-0.0.21/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.21/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:29:01.711450 XoxoDay-0.0.21/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.21/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.21/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1020 2023-06-23 21:25:40.000000 XoxoDay-0.0.21/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)    16384 2023-06-23 21:24:26.000000 XoxoDay-0.0.21/XoxoDay/helper/xoxo.sqlite
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.21/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:29:01.712796 XoxoDay-0.0.21/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.21/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.21/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.21/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3087 2023-06-23 21:25:40.000000 XoxoDay-0.0.21/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.21/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.21/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:29:01.710737 XoxoDay-0.0.21/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 21:29:01.000000 XoxoDay-0.0.21/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      535 2023-06-23 21:29:01.000000 XoxoDay-0.0.21/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-23 21:29:01.000000 XoxoDay-0.0.21/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-23 21:29:01.000000 XoxoDay-0.0.21/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-23 21:29:01.000000 XoxoDay-0.0.21/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-23 21:29:01.713281 XoxoDay-0.0.21/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      957 2023-06-23 21:28:49.000000 XoxoDay-0.0.21/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:46:17.406751 XoxoDay-0.0.22/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.22/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 21:46:17.406525 XoxoDay-0.0.22/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.22/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:46:17.401464 XoxoDay-0.0.22/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-23 21:46:09.000000 XoxoDay-0.0.22/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.22/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:46:17.402854 XoxoDay-0.0.22/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.22/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.22/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1020 2023-06-23 21:25:40.000000 XoxoDay-0.0.22/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.22/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:46:17.405858 XoxoDay-0.0.22/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.22/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.22/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.22/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3087 2023-06-23 21:25:40.000000 XoxoDay-0.0.22/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.22/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.22/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 21:46:17.402257 XoxoDay-0.0.22/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 21:46:17.000000 XoxoDay-0.0.22/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-23 21:46:17.000000 XoxoDay-0.0.22/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-23 21:46:17.000000 XoxoDay-0.0.22/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-23 21:46:17.000000 XoxoDay-0.0.22/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-23 21:46:17.000000 XoxoDay-0.0.22/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-23 21:46:17.407103 XoxoDay-0.0.22/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-23 21:46:05.000000 XoxoDay-0.0.22/setup.py
```

### Comparing `XoxoDay-0.0.21/LICENSE` & `XoxoDay-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/PKG-INFO` & `XoxoDay-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.21
+Version: 0.0.22
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.21/README.md` & `XoxoDay-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/XoxoDay/exception.py` & `XoxoDay-0.0.22/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/XoxoDay/helper/sqlite.py` & `XoxoDay-0.0.22/XoxoDay/helper/sqlite.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/XoxoDay/helper/token.py` & `XoxoDay-0.0.22/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/XoxoDay/service/http_service.py` & `XoxoDay-0.0.22/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/XoxoDay/service/token_service.py` & `XoxoDay-0.0.22/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.22/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.21/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.22/XoxoDay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.21
+Version: 0.0.22
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

