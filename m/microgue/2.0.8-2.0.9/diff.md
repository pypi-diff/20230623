# Comparing `tmp/microgue-2.0.8.tar.gz` & `tmp/microgue-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microgue-2.0.8.tar", last modified: Thu May 25 19:39:35 2023, max compression
+gzip compressed data, was "microgue-2.0.9.tar", last modified: Fri May 26 13:37:38 2023, max compression
```

## Comparing `microgue-2.0.8.tar` & `microgue-2.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.369383 microgue-2.0.8/
--rw-r--r--   0 michael    (501) staff       (20)     2240 2023-05-25 19:39:35.369154 microgue-2.0.8/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1945 2023-05-16 02:02:44.000000 microgue-2.0.8/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.363639 microgue-2.0.8/microgue/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5664 2023-05-12 01:21:19.000000 microgue-2.0.8/microgue/abstract_app.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.364679 microgue-2.0.8/microgue/caches/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/caches/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3289 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/caches/abstract_cache.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.365171 microgue-2.0.8/microgue/constants/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/constants/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      378 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/constants/error_constants.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.365599 microgue-2.0.8/microgue/events/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/events/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     2150 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/events/abstract_event_bus.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.365879 microgue-2.0.8/microgue/loggers/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/loggers/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1412 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/loggers/logger.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.366340 microgue-2.0.8/microgue/models/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/models/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10735 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/models/abstract_model.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.367241 microgue-2.0.8/microgue/objects/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/objects/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1483 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/objects/abstract_expiring_model_object.py
--rw-r--r--   0 michael    (501) staff       (20)     8817 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/objects/abstract_model_object.py
--rw-r--r--   0 michael    (501) staff       (20)     2707 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/objects/object.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.367507 microgue-2.0.8/microgue/queues/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/queues/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3335 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/queues/abstract_queue.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.367770 microgue-2.0.8/microgue/secrets/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/secrets/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1065 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/secrets/secrets.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.368025 microgue-2.0.8/microgue/security/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/security/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      334 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/security/generic.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.368350 microgue-2.0.8/microgue/services/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/services/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4270 2023-05-25 19:36:57.000000 microgue-2.0.8/microgue/services/service.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.368785 microgue-2.0.8/microgue/storages/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/storages/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     3886 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/storages/abstract_storage.py
--rw-r--r--   0 michael    (501) staff       (20)     2737 2023-05-10 14:52:59.000000 microgue-2.0.8/microgue/utils.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-25 19:39:35.364482 microgue-2.0.8/microgue.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     2240 2023-05-25 19:39:35.000000 microgue-2.0.8/microgue.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1010 2023-05-25 19:39:35.000000 microgue-2.0.8/microgue.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-25 19:39:35.000000 microgue-2.0.8/microgue.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       42 2023-05-25 19:39:35.000000 microgue-2.0.8/microgue.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2023-05-25 19:39:35.000000 microgue-2.0.8/microgue.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-25 19:39:35.369436 microgue-2.0.8/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      640 2023-05-25 19:37:36.000000 microgue-2.0.8/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.701565 microgue-2.0.9/
+-rw-r--r--   0 michael    (501) staff       (20)     2240 2023-05-26 13:37:38.701318 microgue-2.0.9/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1945 2023-05-16 02:02:44.000000 microgue-2.0.9/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.696433 microgue-2.0.9/microgue/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     5664 2023-05-12 01:21:19.000000 microgue-2.0.9/microgue/abstract_app.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.697304 microgue-2.0.9/microgue/caches/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/caches/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3289 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/caches/abstract_cache.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.697658 microgue-2.0.9/microgue/constants/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/constants/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      378 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/constants/error_constants.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.697978 microgue-2.0.9/microgue/events/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/events/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     2150 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/events/abstract_event_bus.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.698310 microgue-2.0.9/microgue/loggers/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/loggers/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1412 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/loggers/logger.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.698629 microgue-2.0.9/microgue/models/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/models/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10735 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/models/abstract_model.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.699565 microgue-2.0.9/microgue/objects/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/objects/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1483 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/objects/abstract_expiring_model_object.py
+-rw-r--r--   0 michael    (501) staff       (20)     8817 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/objects/abstract_model_object.py
+-rw-r--r--   0 michael    (501) staff       (20)     2707 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/objects/object.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.699861 microgue-2.0.9/microgue/queues/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/queues/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3335 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/queues/abstract_queue.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.700142 microgue-2.0.9/microgue/secrets/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/secrets/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1065 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/secrets/secrets.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.700421 microgue-2.0.9/microgue/security/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/security/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      334 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/security/generic.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.700689 microgue-2.0.9/microgue/services/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/services/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     4492 2023-05-26 13:31:22.000000 microgue-2.0.9/microgue/services/service.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.701040 microgue-2.0.9/microgue/storages/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/storages/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     3886 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/storages/abstract_storage.py
+-rw-r--r--   0 michael    (501) staff       (20)     2737 2023-05-10 14:52:59.000000 microgue-2.0.9/microgue/utils.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 13:37:38.697099 microgue-2.0.9/microgue.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     2240 2023-05-26 13:37:38.000000 microgue-2.0.9/microgue.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1010 2023-05-26 13:37:38.000000 microgue-2.0.9/microgue.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-26 13:37:38.000000 microgue-2.0.9/microgue.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       42 2023-05-26 13:37:38.000000 microgue-2.0.9/microgue.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2023-05-26 13:37:38.000000 microgue-2.0.9/microgue.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-26 13:37:38.701645 microgue-2.0.9/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      640 2023-05-26 13:36:13.000000 microgue-2.0.9/setup.py
```

### Comparing `microgue-2.0.8/PKG-INFO` & `microgue-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.8
+Version: 2.0.9
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `microgue-2.0.8/README.md` & `microgue-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/abstract_app.py` & `microgue-2.0.9/microgue/abstract_app.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/caches/abstract_cache.py` & `microgue-2.0.9/microgue/caches/abstract_cache.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/events/abstract_event_bus.py` & `microgue-2.0.9/microgue/events/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/loggers/logger.py` & `microgue-2.0.9/microgue/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/models/abstract_model.py` & `microgue-2.0.9/microgue/models/abstract_model.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/objects/abstract_expiring_model_object.py` & `microgue-2.0.9/microgue/objects/abstract_expiring_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/objects/abstract_model_object.py` & `microgue-2.0.9/microgue/objects/abstract_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/objects/object.py` & `microgue-2.0.9/microgue/objects/object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/queues/abstract_queue.py` & `microgue-2.0.9/microgue/queues/abstract_queue.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/secrets/secrets.py` & `microgue-2.0.9/microgue/secrets/secrets.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/services/service.py` & `microgue-2.0.9/microgue/services/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,30 +13,38 @@
     request_base_url = ""
     mask_request_headers_fields = []
     mask_request_data_fields = []
     mask_response_headers_fields = []
     mask_response_data_fields = []
 
     class Request:
+        # extension optional
+        default_headers = {}
+        default_data = {}
+
         def __init__(
             self,
             url="",
             parameters=None,
             method="GET",
             headers=None,
             cookies=None,
             data=None,
             files=None,
             verify_ssl=True
         ):
+            # apply default headers and data
+            self.headers = self.default_headers
+            self.data = self.default_data
+
             # defaults
             self.parameters = {} if parameters is None else parameters
-            self.headers = {} if headers is None else headers
+            self.headers.update({} if headers is None else headers)
             self.cookies = {} if cookies is None else cookies
-            self.data = {} if data is None else data
+            self.data.update({} if data is None else data)
             self.files = {} if files is None else files
 
             self.url = url
             self.method = method
             self.verify_ssl = verify_ssl
 
     class Response:
@@ -58,15 +66,15 @@
         pass
 
     def request(self, *args, **kwargs):
         return self.invoke(Service.Request(*args, **kwargs))
 
     def invoke(self, request):
         logger.debug(f"{self.__class__.__name__}.invoke", priority=2)
-        logger.debug(f"request url: {request.url}")
+        logger.debug(f"request url: {self.request_base_url + request.url}")
         logger.debug(f"request method: {request.method}")
         logger.debug(f"request headers: {mask_fields_in_data(request.headers, self.mask_request_headers_fields)}")
         logger.debug(f"request cookies: {request.cookies}")
         logger.debug(f"request data: {mask_fields_in_data(request.data, self.mask_request_data_fields)}")
 
         # open all files before sending them
         opened_request_files = OrderedDict()
@@ -77,15 +85,14 @@
             requests_response = requests.request(
                 url=self.request_base_url + request.url,
                 params=request.parameters,
                 method=request.method,
                 headers=request.headers,
                 cookies=request.cookies,
                 data=request.data,
-                json=request.data,
                 files=opened_request_files,
                 verify=request.verify_ssl
             )
 
             response_status_code = requests_response.status_code
             response_headers = dict(requests_response.headers)
             response_cookies = dict(requests_response.cookies)
```

### Comparing `microgue-2.0.8/microgue/storages/abstract_storage.py` & `microgue-2.0.9/microgue/storages/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue/utils.py` & `microgue-2.0.9/microgue/utils.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/microgue.egg-info/PKG-INFO` & `microgue-2.0.9/microgue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.8
+Version: 2.0.9
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `microgue-2.0.8/microgue.egg-info/SOURCES.txt` & `microgue-2.0.9/microgue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microgue-2.0.8/setup.py` & `microgue-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="microgue",
-    version="2.0.8",
+    version="2.0.9",
     author="Michael Hudelson",
     author_email="michaelhudelson@gmail.com",
     description="This project contains bootstrap code to speed up the development of AWS based microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
```

