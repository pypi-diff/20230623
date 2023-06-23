# Comparing `tmp/XoxoDay-0.0.18.tar.gz` & `tmp/XoxoDay-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.18.tar", last modified: Fri Jun 23 20:35:48 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.19.tar", last modified: Fri Jun 23 20:39:53 2023, max compression
```

## Comparing `XoxoDay-0.0.18.tar` & `XoxoDay-0.0.19.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.421892 XoxoDay-0.0.18/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.18/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:35:48.421673 XoxoDay-0.0.18/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.18/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.418016 XoxoDay-0.0.18/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-23 20:35:39.000000 XoxoDay-0.0.18/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.18/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.419247 XoxoDay-0.0.18/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.18/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.18/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      942 2023-06-23 20:35:32.000000 XoxoDay-0.0.18/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.18/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.421142 XoxoDay-0.0.18/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.18/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.18/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.18/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     3049 2023-06-23 20:32:05.000000 XoxoDay-0.0.18/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.18/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.18/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:35:48.418744 XoxoDay-0.0.18/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-23 20:35:48.000000 XoxoDay-0.0.18/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-23 20:35:48.421946 XoxoDay-0.0.18/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-23 20:35:35.000000 XoxoDay-0.0.18/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:39:53.827062 XoxoDay-0.0.19/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.19/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:39:53.826896 XoxoDay-0.0.19/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.19/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:39:53.823613 XoxoDay-0.0.19/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-23 20:39:39.000000 XoxoDay-0.0.19/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.19/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:39:53.824883 XoxoDay-0.0.19/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.19/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      618 2023-06-23 20:29:54.000000 XoxoDay-0.0.19/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      942 2023-06-23 20:35:32.000000 XoxoDay-0.0.19/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.19/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:39:53.826501 XoxoDay-0.0.19/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.19/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1205 2023-06-23 20:31:24.000000 XoxoDay-0.0.19/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.19/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     3052 2023-06-23 20:39:39.000000 XoxoDay-0.0.19/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.19/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.19/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-23 20:39:53.824385 XoxoDay-0.0.19/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-23 20:39:53.000000 XoxoDay-0.0.19/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-23 20:39:53.000000 XoxoDay-0.0.19/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-23 20:39:53.000000 XoxoDay-0.0.19/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-23 20:39:53.000000 XoxoDay-0.0.19/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-23 20:39:53.000000 XoxoDay-0.0.19/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-23 20:39:53.827120 XoxoDay-0.0.19/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-23 20:39:43.000000 XoxoDay-0.0.19/setup.py
```

### Comparing `XoxoDay-0.0.18/LICENSE` & `XoxoDay-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.18/PKG-INFO` & `XoxoDay-0.0.19/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.18
+Version: 0.0.19
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.18/README.md` & `XoxoDay-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.18/XoxoDay/exception.py` & `XoxoDay-0.0.19/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.18/XoxoDay/helper/sqlite.py` & `XoxoDay-0.0.19/XoxoDay/helper/sqlite.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.18/XoxoDay/helper/token.py` & `XoxoDay-0.0.19/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.18/XoxoDay/service/http_service.py` & `XoxoDay-0.0.19/XoxoDay/service/http_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.18/XoxoDay/service/token_service.py` & `XoxoDay-0.0.19/XoxoDay/service/token_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         result = {
             "access_token": data['access_token'],
             "token_type": data['token_type'],
             "expires_in": data['expires_in'],
             "refresh_token": data['refresh_token']
         }
         update_token(result)
-        return res
+        return result
 
     def create_access_token(self, payloads, headers):
         res = self.connect('POST', '/v1/oauth/token/user', payloads, headers)
         if 'error' in res:
             raise XoxoDayException(res['error'] + ' ' + res['error_description'])
         update_token(res)
         return res
```

### Comparing `XoxoDay-0.0.18/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.19/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.18/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.19/XoxoDay.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.18
+Version: 0.0.19
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.18/setup.py` & `XoxoDay-0.0.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='XoxoDay',
-    version="0.0.18",
+    version="0.0.19",
     author="Yaşar Özyurt",
     author_email="blueromans@gmail.com",
     description='XoxoDay Api Client For Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blueromans/XoxoDay.git',
     project_urls={
```

