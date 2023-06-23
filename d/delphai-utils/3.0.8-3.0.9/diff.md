# Comparing `tmp/delphai-utils-3.0.8.tar.gz` & `tmp/delphai-utils-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai-utils-3.0.8.tar", max compression
+gzip compressed data, was "delphai-utils-3.0.9.tar", max compression
```

## Comparing `delphai-utils-3.0.8.tar` & `delphai-utils-3.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       22 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/__init__.py
--rw-r--r--   0        0        0     3842 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/authorization.py
--rw-r--r--   0        0        0      495 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/authorization_test.py
--rw-r--r--   0        0        0     2069 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/caching.py
--rw-r--r--   0        0        0     3392 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/config.py
--rw-r--r--   0        0        0     1347 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/db.py
--rw-r--r--   0        0        0      549 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/elasticsearch.py
--rw-r--r--   0        0        0    11285 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/faust.py
--rw-r--r--   0        0        0      481 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/formatting.py
--rw-r--r--   0        0        0     7063 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/gateway.py
--rw-r--r--   0        0        0     4796 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/grpc_client.py
--rw-r--r--   0        0        0     3630 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/grpc_server.py
--rw-r--r--   0        0        0     1532 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/interceptors/authentication.py
--rw-r--r--   0        0        0     5228 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/interceptors/metrics.py
--rw-r--r--   0        0        0     1482 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/keycloak.py
--rw-r--r--   0        0        0     2336 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/logging.py
--rw-r--r--   0        0        0     2499 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/patches.py
--rw-r--r--   0        0        0     3435 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/users.py
--rw-r--r--   0        0        0     2608 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/utils.py
--rw-r--r--   0        0        0      435 2022-11-01 15:55:04.763624 delphai-utils-3.0.8/delphai_utils/validation.py
--rw-r--r--   0        0        0    43882 2022-11-01 15:55:04.767624 delphai-utils-3.0.8/delphai_utils/validator.py
--rw-r--r--   0        0        0     3218 2022-11-01 15:55:44.263636 delphai-utils-3.0.8/pyproject.toml
--rw-r--r--   0        0        0     2303 2022-11-01 15:55:46.463638 delphai-utils-3.0.8/setup.py
--rw-r--r--   0        0        0     2757 2022-11-01 15:55:46.464138 delphai-utils-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/__init__.py
+-rw-r--r--   0        0        0     3842 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/authorization.py
+-rw-r--r--   0        0        0      495 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/authorization_test.py
+-rw-r--r--   0        0        0     2069 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/caching.py
+-rw-r--r--   0        0        0     3392 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/config.py
+-rw-r--r--   0        0        0     1347 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/db.py
+-rw-r--r--   0        0        0      549 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/elasticsearch.py
+-rw-r--r--   0        0        0    11285 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/faust.py
+-rw-r--r--   0        0        0      481 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/formatting.py
+-rw-r--r--   0        0        0     7063 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/gateway.py
+-rw-r--r--   0        0        0     4796 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/grpc_client.py
+-rw-r--r--   0        0        0     3630 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/grpc_server.py
+-rw-r--r--   0        0        0     1532 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/interceptors/authentication.py
+-rw-r--r--   0        0        0     5218 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/interceptors/metrics.py
+-rw-r--r--   0        0        0     1482 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/keycloak.py
+-rw-r--r--   0        0        0     2336 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/logging.py
+-rw-r--r--   0        0        0     2499 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/patches.py
+-rw-r--r--   0        0        0     3435 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/users.py
+-rw-r--r--   0        0        0     2608 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/utils.py
+-rw-r--r--   0        0        0      435 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/validation.py
+-rw-r--r--   0        0        0    43882 2022-11-10 10:16:35.271632 delphai-utils-3.0.9/delphai_utils/validator.py
+-rw-r--r--   0        0        0     3218 2022-11-10 10:17:10.011103 delphai-utils-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2303 2022-11-10 10:17:13.201829 delphai-utils-3.0.9/setup.py
+-rw-r--r--   0        0        0     2757 2022-11-10 10:17:13.202185 delphai-utils-3.0.9/PKG-INFO
```

### Comparing `delphai-utils-3.0.8/delphai_utils/authorization.py` & `delphai-utils-3.0.9/delphai_utils/authorization.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/caching.py` & `delphai-utils-3.0.9/delphai_utils/caching.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/config.py` & `delphai-utils-3.0.9/delphai_utils/config.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/db.py` & `delphai-utils-3.0.9/delphai_utils/db.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/elasticsearch.py` & `delphai-utils-3.0.9/delphai_utils/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/faust.py` & `delphai-utils-3.0.9/delphai_utils/faust.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/gateway.py` & `delphai-utils-3.0.9/delphai_utils/gateway.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/grpc_client.py` & `delphai-utils-3.0.9/delphai_utils/grpc_client.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/grpc_server.py` & `delphai-utils-3.0.9/delphai_utils/grpc_server.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/interceptors/authentication.py` & `delphai-utils-3.0.9/delphai_utils/interceptors/authentication.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/interceptors/metrics.py` & `delphai-utils-3.0.9/delphai_utils/interceptors/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         try:
             yield
             grpc_code = StatusCode.OK
         except grpc.aio.AbortError as error:
             grpc_code = STATUS_CODE_BY_INT_VALUE.get(
                 servicer_context.code(), StatusCode.UNKNOWN
             )
-            logger.error(f"[{grpc_code}] {error.details()}")
+            logger.error(f"[{grpc_code}] {error}")
             raise error
 
         finally:
             end_time = time.perf_counter()
             elapsed = max(end_time - start_time, 0)
 
             logger.info(
```

### Comparing `delphai-utils-3.0.8/delphai_utils/keycloak.py` & `delphai-utils-3.0.9/delphai_utils/keycloak.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/logging.py` & `delphai-utils-3.0.9/delphai_utils/logging.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/patches.py` & `delphai-utils-3.0.9/delphai_utils/patches.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/users.py` & `delphai-utils-3.0.9/delphai_utils/users.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/utils.py` & `delphai-utils-3.0.9/delphai_utils/utils.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/delphai_utils/validator.py` & `delphai-utils-3.0.9/delphai_utils/validator.py`

 * *Files identical despite different names*

### Comparing `delphai-utils-3.0.8/pyproject.toml` & `delphai-utils-3.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delphai-utils"
-version = "3.0.8"
+version = "3.0.9"
 description = "delphai backend utilities"
 authors = ["Barath Kumar <barath@delphai.com>"]
 homepage = "https://github.com/delphai/delphai-utils"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 omegaconf = { version = "^2.1.0", optional = true}
```

### Comparing `delphai-utils-3.0.8/setup.py` & `delphai-utils-3.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                'faust-streaming>=0.6.9,<0.7.0',
                'confluent-kafka>=1.7.0,<2.0.0',
                'betterproto[compiler]==2.0.0b3',
                'aioprometheus[aiohttp]==21.8.0']}
 
 setup_kwargs = {
     'name': 'delphai-utils',
-    'version': '3.0.8',
+    'version': '3.0.9',
     'description': 'delphai backend utilities',
     'long_description': None,
     'author': 'Barath Kumar',
     'author_email': 'barath@delphai.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/delphai/delphai-utils',
```

### Comparing `delphai-utils-3.0.8/PKG-INFO` & `delphai-utils-3.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-utils
-Version: 3.0.8
+Version: 3.0.9
 Summary: delphai backend utilities
 Home-page: https://github.com/delphai/delphai-utils
 Author: Barath Kumar
 Author-email: barath@delphai.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

