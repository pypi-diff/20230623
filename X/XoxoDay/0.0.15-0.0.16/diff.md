# Comparing `tmp/XoxoDay-0.0.15.tar.gz` & `tmp/XoxoDay-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XoxoDay-0.0.15.tar", last modified: Thu Jun 22 09:49:28 2023, max compression
+gzip compressed data, was "XoxoDay-0.0.16.tar", last modified: Thu Jun 22 16:03:13 2023, max compression
```

## Comparing `XoxoDay-0.0.15.tar` & `XoxoDay-0.0.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.676327 XoxoDay-0.0.15/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.15/LICENSE
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-22 09:49:28.676194 XoxoDay-0.0.15/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.15/README.md
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.673283 XoxoDay-0.0.15/XoxoDay/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-22 09:49:17.000000 XoxoDay-0.0.15/XoxoDay/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.15/XoxoDay/exception.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.674525 XoxoDay-0.0.15/XoxoDay/helper/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.15/XoxoDay/helper/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.15/XoxoDay/helper/sqlite.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.15/XoxoDay/helper/token.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.15/XoxoDay/serializer.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.675862 XoxoDay-0.0.15/XoxoDay/service/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.15/XoxoDay/service/__init__.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1121 2023-06-14 18:07:04.000000 XoxoDay-0.0.15/XoxoDay/service/http_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.15/XoxoDay/service/placeOrder.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     1850 2023-06-15 17:52:44.000000 XoxoDay-0.0.15/XoxoDay/service/token_service.py
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.15/XoxoDay/service/voucher.json
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.15/XoxoDay/service/xoxoday_service.py
-drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 09:49:28.674052 XoxoDay-0.0.15/XoxoDay.egg-info/
--rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/PKG-INFO
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/SOURCES.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/dependency_links.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/requires.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-22 09:49:28.000000 XoxoDay-0.0.15/XoxoDay.egg-info/top_level.txt
--rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-22 09:49:28.676368 XoxoDay-0.0.15/setup.cfg
--rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-22 09:49:08.000000 XoxoDay-0.0.15/setup.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 16:03:13.835999 XoxoDay-0.0.16/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1071 2022-10-16 19:39:29.000000 XoxoDay-0.0.16/LICENSE
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-22 16:03:13.835779 XoxoDay-0.0.16/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1789 2023-06-15 17:58:41.000000 XoxoDay-0.0.16/README.md
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 16:03:13.831910 XoxoDay-0.0.16/XoxoDay/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      163 2023-06-22 16:03:00.000000 XoxoDay-0.0.16/XoxoDay/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      577 2023-06-15 17:06:19.000000 XoxoDay-0.0.16/XoxoDay/exception.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 16:03:13.833263 XoxoDay-0.0.16/XoxoDay/helper/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:06:04.000000 XoxoDay-0.0.16/XoxoDay/helper/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      469 2023-06-14 18:27:10.000000 XoxoDay-0.0.16/XoxoDay/helper/sqlite.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      947 2023-06-14 18:27:04.000000 XoxoDay-0.0.16/XoxoDay/helper/token.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      499 2023-06-14 18:06:04.000000 XoxoDay-0.0.16/XoxoDay/serializer.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 16:03:13.835204 XoxoDay-0.0.16/XoxoDay/service/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        0 2023-06-14 18:26:05.000000 XoxoDay-0.0.16/XoxoDay/service/__init__.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1143 2023-06-22 16:02:54.000000 XoxoDay-0.0.16/XoxoDay/service/http_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      286 2023-06-14 21:15:51.000000 XoxoDay-0.0.16/XoxoDay/service/placeOrder.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     1850 2023-06-15 17:52:44.000000 XoxoDay-0.0.16/XoxoDay/service/token_service.py
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      300 2023-06-14 20:56:15.000000 XoxoDay-0.0.16/XoxoDay/service/voucher.json
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     4607 2023-06-22 09:49:08.000000 XoxoDay-0.0.16/XoxoDay/service/xoxoday_service.py
+drwxr-xr-x   0 yasarozyurt   (501) staff       (20)        0 2023-06-22 16:03:13.832742 XoxoDay-0.0.16/XoxoDay.egg-info/
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)     2294 2023-06-22 16:03:13.000000 XoxoDay-0.0.16/XoxoDay.egg-info/PKG-INFO
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      508 2023-06-22 16:03:13.000000 XoxoDay-0.0.16/XoxoDay.egg-info/SOURCES.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        1 2023-06-22 16:03:13.000000 XoxoDay-0.0.16/XoxoDay.egg-info/dependency_links.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       23 2023-06-22 16:03:13.000000 XoxoDay-0.0.16/XoxoDay.egg-info/requires.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)        8 2023-06-22 16:03:13.000000 XoxoDay-0.0.16/XoxoDay.egg-info/top_level.txt
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)       38 2023-06-22 16:03:13.836049 XoxoDay-0.0.16/setup.cfg
+-rw-r--r--   0 yasarozyurt   (501) staff       (20)      945 2023-06-22 16:03:04.000000 XoxoDay-0.0.16/setup.py
```

### Comparing `XoxoDay-0.0.15/LICENSE` & `XoxoDay-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.15/PKG-INFO` & `XoxoDay-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.15
+Version: 0.0.16
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `XoxoDay-0.0.15/README.md` & `XoxoDay-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.15/XoxoDay/exception.py` & `XoxoDay-0.0.16/XoxoDay/exception.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.15/XoxoDay/helper/token.py` & `XoxoDay-0.0.16/XoxoDay/helper/token.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.15/XoxoDay/service/http_service.py` & `XoxoDay-0.0.16/XoxoDay/service/http_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             raise XoxoDayException(ErrorCodes.BASE_URL_ERROR)
         self.REST_URL = REST_URL
 
     @staticmethod
     def parse_result(r):
         res = r.text.encode('utf-8')
         res = Serializer.loads(res)
-        if 'errors' in res:
+        if 'errors' in res and 'data' not in res:
             raise XoxoDayException(res['errors']['message'])
         return res
 
     def post_request(self, url, request_body, headers):
         request_body = Serializer.dumps(request_body)
         r = requests.post(url, data=request_body, headers=headers)
         return self.parse_result(r)
```

### Comparing `XoxoDay-0.0.15/XoxoDay/service/token_service.py` & `XoxoDay-0.0.16/XoxoDay/service/token_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.15/XoxoDay/service/xoxoday_service.py` & `XoxoDay-0.0.16/XoxoDay/service/xoxoday_service.py`

 * *Files identical despite different names*

### Comparing `XoxoDay-0.0.15/XoxoDay.egg-info/PKG-INFO` & `XoxoDay-0.0.16/XoxoDay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XoxoDay
-Version: 0.0.15
+Version: 0.0.16
 Summary: XoxoDay Api Client For Python
 Home-page: https://github.com/blueromans/XoxoDay.git
 Author: Yaşar Özyurt
 Author-email: blueromans@gmail.com
 Project-URL: Bug Tracker, https://github.com/blueromans/XoxoDay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

