# Comparing `tmp/osint-python-starter-service-2.1.1.tar.gz` & `tmp/osint-python-starter-service-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.1.1.tar", last modified: Sat Jun 17 00:50:27 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.2.0.tar", last modified: Fri Jun 23 01:28:42 2023, max compression
```

## Comparing `osint-python-starter-service-2.1.1.tar` & `osint-python-starter-service-2.2.0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.029231 osint-python-starter-service-2.1.1/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.1.1/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-17 00:50:27.029231 osint-python-starter-service-2.1.1/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.1.1/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      942 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-06-17 00:50:27.000000 osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-17 00:50:27.029231 osint-python-starter-service-2.1.1/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-06-17 00:46:37.000000 osint-python-starter-service-2.1.1/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.1.1/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.1.1/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6176 2023-06-17 00:42:50.000000 osint-python-starter-service-2.1.1/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.1.1/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3931 2023-06-16 19:55:26.000000 osint-python-starter-service-2.1.1/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.1/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.1.1/starter_service/examples/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      594 2023-06-07 19:05:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1587 2023-06-16 20:48:31.000000 osint-python-starter-service-2.1.1/starter_service/examples/manual_api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1274 2023-06-07 20:59:38.000000 osint-python-starter-service-2.1.1/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1212 2023-06-07 19:05:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1324 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/offset_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1156 2023-06-07 19:08:41.000000 osint-python-starter-service-2.1.1/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5722 2023-06-17 00:50:00.000000 osint-python-starter-service-2.1.1/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.1.1/starter_service/schemas.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:50:27.025897 osint-python-starter-service-2.1.1/starter_service/tests/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.1.1/starter_service/tests/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.1.1/starter_service/tests/employee.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.1.1/starter_service/tests/teet.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.1.1/starter_service/tests/test_avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.1.1/starter_service/tests/tst.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.2.0/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.2.0/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-22 23:18:15.000000 osint-python-starter-service-2.2.0/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2841 2023-06-22 23:23:47.000000 osint-python-starter-service-2.2.0/classes/article_raw_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      909 2023-06-22 23:23:46.000000 osint-python-starter-service-2.2.0/classes/metadata_item_ner_en.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1051 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       24 2023-06-23 01:28:42.000000 osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-06-23 00:55:50.000000 osint-python-starter-service-2.2.0/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.2.0/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.2.0/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6309 2023-06-23 01:20:47.000000 osint-python-starter-service-2.2.0/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.2.0/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3999 2023-06-23 01:22:59.000000 osint-python-starter-service-2.2.0/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.2.0/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.2.0/starter_service/examples/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      602 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1595 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/manual_api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1282 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1220 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1332 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/offset_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1164 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.0/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6117 2023-06-23 01:28:24.000000 osint-python-starter-service-2.2.0/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.2.0/starter_service/schemas.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      788 2023-06-23 00:39:02.000000 osint-python-starter-service-2.2.0/starter_service/sub_process.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 01:28:42.180339 osint-python-starter-service-2.2.0/starter_service/tests/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.2.0/starter_service/tests/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.2.0/starter_service/tests/employee.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.2.0/starter_service/tests/teet.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.2.0/starter_service/tests/test_avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.2.0/starter_service/tests/tst.py
```

### Comparing `osint-python-starter-service-2.1.1/LICENSE` & `osint-python-starter-service-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/PKG-INFO` & `osint-python-starter-service-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.1.1
+Version: 2.2.0
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.1.1/README.md` & `osint-python-starter-service-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.1.1
+Version: 2.2.0
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.1.1/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.2.0/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 LICENSE
 README.md
 setup.py
+classes/__init__.py
+classes/article_raw_en.py
+classes/metadata_item_ner_en.py
 osint_python_starter_service.egg-info/PKG-INFO
 osint_python_starter_service.egg-info/SOURCES.txt
 osint_python_starter_service.egg-info/dependency_links.txt
 osint_python_starter_service.egg-info/requires.txt
 osint_python_starter_service.egg-info/top_level.txt
 starter_service/__init__.py
 starter_service/api.py
 starter_service/api_server.py
 starter_service/avro_parser.py
 starter_service/base_service.py
 starter_service/env.py
 starter_service/kafka_adapter.py
 starter_service/schemas.py
+starter_service/sub_process.py
 starter_service/examples/__init__.py
 starter_service/examples/error.py
 starter_service/examples/manual_api.py
 starter_service/examples/manual_kafka.py
 starter_service/examples/multi.py
 starter_service/examples/offset_kafka.py
 starter_service/examples/single.py
```

### Comparing `osint-python-starter-service-2.1.1/setup.py` & `osint-python-starter-service-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.1.1",
+    version="2.2.0",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/api.py` & `osint-python-starter-service-2.2.0/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/starter_service/api_server.py` & `osint-python-starter-service-2.2.0/starter_service/api_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,74 @@
 import datetime
 import logging
-import threading
 
+import uvicorn
 from fastapi import FastAPI, APIRouter
 from fastapi.encoders import jsonable_encoder
 from pydantic import ValidationError
 from starlette.responses import Response, JSONResponse
 from starlette.status import HTTP_200_OK
-
 from starter_service.api import API
 from starter_service.env import ENV
-from starter_service.schemas import SchemaRegistry
+from starter_service.sub_process import SubProcess
+from uvicorn import Config
 
 
-class APIServer:
+class APIServer(SubProcess):
 
-    def __init__(self, name=None, ready: callable = None, health: callable = None, kafka_status: str = None,
-                 base_service=None, callback=None, **kwargs):
+    def __init__(self, name=None, ready: callable = None, health: callable = None, **kwargs):
+        super().__init__()
         self.name = name
+        self.server = None
+        self.logger = logging.getLogger(__name__)
+
         self._validated()
         self._fast_api = FastAPI(title=self.name)
         self._router = APIRouter()
-        self.callback = callback
 
         @self._fast_api.exception_handler(Exception)
         async def validation_exception_handler(request, err):
             base_error_message = f"Failed to execute: {request.method}: {request.url}"
             # Change here to LOGGER
             return JSONResponse(status_code=400, content={"message": f"{base_error_message}. Detail: {err}"})
 
         @self._fast_api.exception_handler(ValidationError)
         async def validation_exception_handler(request, err):
             base_error_message = f"Failed to execute: {request.method}: {request.url}"
             # Change here to LOGGER
             return JSONResponse(status_code=400, content={"message": f"{base_error_message}. Detail: {err}"})
 
-        self.host = ENV.REST_API_HOST
-        self.port = ENV.REST_API_PORT
-        self._logger = logging.getLogger(__name__)
-
+        # service
         self._ready = ready
         self._health = health
-        self._kafka_status = kafka_status
 
-        self._thread = None
         self._uptime = None
-        self._running = False
-        self._base_service = base_service
-
-        self._register_static_routes()
-        self._register_dynamic_routes()
-        self._fast_api.include_router(self._router)
 
     @property
     def fast_api(self):
         return self._fast_api
 
     @property
     def router(self):
         return self._router
 
     def _register_static_routes(self):
-        self._logger.info("Registering static routes")
+        self.logger.info("Registering static routes")
 
         @self._router.get("/")
         def root():
+            from starter_service.schemas import SchemaRegistry
             return {
                 "client_id": ENV.CLIENT_ID,
                 "uptime": self._uptime,
                 "docs": "/docs",
                 "redoc": "/redoc",
                 "openapi": "/openapi.json",
-                "kafka": {"error": self._kafka_status} if self._kafka_status != "ok" else {
+                "kafka": {
+                    "error": self.base_service.kafka_error} if self.base_service and self.base_service.kafka_error else {
                     "status": "ok",
                     "host": ENV.KAFKA_HOST,
                     "schema_registry": ENV.SCHEMA_REGISTRY,
                     "partitioner": ENV.PARTITIONER,
                     "message_max_bytes": ENV.MESSAGE_MAX_BYTES,
                     "heartbeat_interval": ENV.HEARTBEAT_INTERVAL,
                     "offset_type": ENV.OFFSET_TYPE,
@@ -109,49 +102,57 @@
             """Return 200 OK if server is ready"""
             response = self._ready()
             if response:
                 return Response(status_code=HTTP_200_OK)
             else:
                 return Response(status_code=503)
 
-    def start(self):
+    def run(self):
         """Start the server"""
-        self._logger.info("Starting API server")
+        self.logger.info("Starting API server")
+
+        self._register_static_routes()
+        self._register_dynamic_routes()
+        self._fast_api.include_router(self._router)
+
         self._running = True
         self._uptime = datetime.datetime.now().isoformat()
-        self._thread = threading.Thread(target=self._run)
-        self._thread.start()
-        self.callback()
+        if self.callback:
+            self.callback()
+        try:
+            self.logger.info(f"Starting API server on {ENV.REST_API_HOST}:{ENV.REST_API_PORT}")
+            server = uvicorn.Server(config=Config(self._fast_api, host=ENV.REST_API_HOST, port=ENV.REST_API_PORT))
+            server.run()
+        except Exception as e:
+            self.logger.error(f"Failed to start API server: {e}")
+            self.stop()
 
     def stop(self):
-        self._logger.info("Stopping API server")
-        self._running = False
-        self._thread.join()
-
-    def _run(self):
-        import uvicorn
-        uvicorn.run(self._fast_api, host=ENV.REST_API_HOST, port=ENV.REST_API_PORT)
+        self.logger.info("Stopping API server")
+        self.running = False
+        self.server.stop()
 
     def _validated(self):
         """Validate that the server is configured correctly"""
         if ENV.REST_API_ENABLED is False:
             raise Exception("REST API is disabled. To enable REST API set REST_API_ENABLED to true")
 
     def _register_dynamic_routes(self):
         """Register routes that are dynamically added by the user"""
-        self._logger.info("Registering dynamic routes")
+        self.logger.info("Registering dynamic routes")
         for consumer, producer, doc, func, _type in API.functions:
             self._register_route(consumer, producer, doc, func, _type)
 
     def _register_route(self, consumer, producer, doc, func, _type):
         """Register a route"""
+        from starter_service.schemas import SchemaRegistry
         consumer_class = SchemaRegistry.get_schema(consumer)
         producer_class = SchemaRegistry.get_schema(producer)
 
-        self._logger.info(f"Registering route {consumer}:{consumer_class} -> {producer}:{producer_class} ({doc})")
-        func_wrapper = lambda message: func(self._base_service, message) \
-            if isinstance(message, str) else func(self._base_service, jsonable_encoder(message))
+        self.logger.info(f"Registering route {consumer}:{consumer_class} -> {producer}:{producer_class} ({doc})")
+        func_wrapper = lambda message: func(self.base_service, message) \
+            if isinstance(message, str) else func(self.base_service, jsonable_encoder(message))
         path = f"/api{f'/{consumer}' if consumer else ''}{f'/{producer}' if producer else ''}"
 
         func_wrapper.__annotations__ = {'message': consumer_class, 'return': producer_class}
         self._router.add_api_route(path, func_wrapper, methods=[_type], response_model=producer_class, tags=["topics"],
                                    summary=doc)
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/avro_parser.py` & `osint-python-starter-service-2.2.0/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/starter_service/env.py` & `osint-python-starter-service-2.2.0/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/starter_service/examples/error.py` & `osint-python-starter-service-2.2.0/starter_service/examples/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
     @API.post(consumer=ENV.CONSUME, producer=ENV.PRODUCE, doc="Process raw article and return metadata")
     def handle_message(self, message: dict):
         raise Exception("Bad request")
 
 
 if __name__ == '__main__':
-    SingleRoute()
+    SingleRoute().start()
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/examples/manual_api.py` & `osint-python-starter-service-2.2.0/starter_service/examples/manual_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,8 +49,8 @@
             data['language'] = 'en'
             return data
 
         self.api.fast_api.add_api_route('/test_manual', post_test, methods=['POST'])
 
 
 if __name__ == '__main__':
-    ManualKafka()
+    ManualKafka().start()
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.2.0/starter_service/examples/manual_kafka.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 
         message['language'] = 'lt'
         self.send_message(message, 'article_raw_lt')
         return {}
 
 
 if __name__ == '__main__':
-    ManualKafka()
+    ManualKafka().start()
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/examples/multi.py` & `osint-python-starter-service-2.2.0/starter_service/examples/multi.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,8 +35,8 @@
               doc="Process article_raw_xx and posts article_raw_nl")
     def handle_message_nl(self, message: dict):
         message['language'] = 'nl'
         return message
 
 
 if __name__ == '__main__':
-    MultiRoutes()
+    MultiRoutes().start()
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/examples/offset_kafka.py` & `osint-python-starter-service-2.2.0/starter_service/examples/offset_kafka.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 
         message['language'] = 'lt'
         self.send_message(message, 'article_raw_lt')
         return {}
 
 
 if __name__ == '__main__':
-    ManualKafka()
+    ManualKafka().start()
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/examples/single.py` & `osint-python-starter-service-2.2.0/starter_service/examples/single.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,8 +39,8 @@
                     }
                 }
             ]
         }
 
 
 if __name__ == '__main__':
-    SingleRoute()
+    SingleRoute().start()
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.2.0/starter_service/kafka_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 import logging
-import threading
-import time
-import traceback
-from threading import Thread
+from time import sleep
 
+from starter_service.api import API
+from starter_service.env import ENV
+from starter_service.schemas import SchemaRegistry
+from starter_service.sub_process import SubProcess
 from test_bed_adapter import TestBedOptions, TestBedAdapter
 from test_bed_adapter.kafka.consumer_manager import ConsumerManager
 from test_bed_adapter.kafka.log_manager import LogManager
 from test_bed_adapter.kafka.producer_manager import ProducerManager
 
-from starter_service.api import API
-from starter_service.env import ENV
-from starter_service.schemas import SchemaRegistry
-
 logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s %(message)s')
 
 
-class KafkaAdapter(Thread):
+class KafkaAdapter(SubProcess):
     """Kafka adapter"""
 
-    def __init__(self, callback=None, base_service=None) -> None:
+    def __init__(self) -> None:
         super().__init__()
-        self.daemon = True
-        # Initialize logger
-        self.logger = None
         # Initialize test bed adapter
         self._test_bed_adapter = None
         # Initialize test bed options
         self._test_bed_options = None
-
         # Validate environment variables
         self._validate_params()
         # Initialize test bed options
         self._init_options()
         # Initialize producers and consumers
         self._producers = {}
         self._consumers = {}
 
-        self._callback = callback
-        self._base_service = base_service
-
-    def start(self):
+    def run(self):
         """Start the service"""
         self._init_producers()
         self._test_bed_adapter.initialize()
-
+        self._init_logger()
         # Create threads for each consume topic
         for topic in ENV.CONSUME.split(','):
             topic = topic.strip()
             if not topic:
                 self.logger.warning("Empty topic, skipping")
                 continue
-            _consumer = ConsumerManager(
-                options=self._test_bed_options,
-                kafka_topic=topic,
-                handle_message=self._handle_message
-            )
-            _consumer.start()
-            self.logger.info(f"Registering schema from kafka for {topic}")
-            SchemaRegistry.register_schema(_consumer.schema_str, topic)
-            self.logger.info(f"Initializing listener for topic {topic}")
+            try:
+                _consumer = ConsumerManager(
+                    options=self._test_bed_options,
+                    kafka_topic=topic,
+                    handle_message=self._handle_message
+                )
+                self._consumers[topic] = _consumer
+                self.logger.info(f"Registering schema from kafka for {topic}")
+                SchemaRegistry.register_schema(_consumer.schema_str, topic)
+            except:
+                self.logger.error(f"Could not initialize consumer for topic {topic}")
 
         if self._callback:
             self._callback()
 
+        # Start listening for messages
+        for consumer in self._consumers.values():
+            try:
+                consumer.start()
+                self.logger.info(f"Initializing listener for topic {topic}")
+            except:
+                self.logger.error("Could not start consumer")
+
+        while self.running:
+            sleep(1)
+
+        for consumer in self._consumers.values():
+            consumer.stop()
+            consumer.join()
 
     def send_message(self, message, topics=None, testing=False):
         """Send message to kafka topic"""
         if testing:
             self.logger.info(f"Sending test message to {topics}\n{message}")
             return
 
@@ -104,14 +110,20 @@
             _producer = ProducerManager(
                 options=self._test_bed_options,
                 kafka_topic=topic
             )
             self._producers[topic] = _producer
             SchemaRegistry.register_schema(_producer.schema_str, topic)
 
+    def _init_logger(self):
+        try:
+            self.base_service.logger = self.logger
+        except:
+            pass
+
     def _init_options(self):
         _options = {
             "kafka_host": ENV.KAFKA_HOST,
             "schema_registry": ENV.SCHEMA_REGISTRY,
             "partitioner": ENV.PARTITIONER,
             "consumer_group": ENV.CLIENT_ID,
             "message_max_bytes": ENV.MESSAGE_MAX_BYTES,
@@ -131,16 +143,14 @@
     def _handle_message(self, message, topic):
         self.logger.info(f"Received message for topic {topic}")
         if ENV.DEBUG:
             self.logger.info(f"Message {message}")
 
         funcs = API.get_func_by_consumer(topic)
         for consumer, producer, doc, func, _type in funcs:
-            # self.logger.info(f'Found function form {consumer}, to {producer}')
             try:
                 response = func(self._base_service, message)
                 if producer and response:
                     self.logger.info(f"Sending response: {producer}, {str(response)[:100]}")
                     self.send_message(response, topics=producer)
             except Exception as e:
-                traceback.print_exc()
-                self.logger.error(e)
+                self.logger.error(e)
```

### Comparing `osint-python-starter-service-2.1.1/starter_service/schemas.py` & `osint-python-starter-service-2.2.0/starter_service/schemas.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/starter_service/tests/employee.py` & `osint-python-starter-service-2.2.0/starter_service/tests/employee.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/starter_service/tests/teet.py` & `osint-python-starter-service-2.2.0/starter_service/tests/teet.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.1.1/starter_service/tests/test_avro_parser.py` & `osint-python-starter-service-2.2.0/starter_service/tests/test_avro_parser.py`

 * *Files identical despite different names*

