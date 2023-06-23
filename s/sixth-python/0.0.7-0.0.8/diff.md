# Comparing `tmp/sixth-python-0.0.7.tar.gz` & `tmp/sixth-python-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.0.7.tar", last modified: Mon Jun 19 19:58:09 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.0.8.tar", last modified: Fri Jun 23 11:51:07 2023, max compression
```

## Comparing `sixth-python-0.0.7.tar` & `sixth-python-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/
--rw-r--r--   0 mac        (501) staff       (20)     3117 2023-06-19 19:58:09.000000 sixth-python-0.0.7/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1909 2023-06-19 18:09:44.000000 sixth-python-0.0.7/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-19 19:58:09.000000 sixth-python-0.0.7/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3776 2023-06-19 19:57:52.000000 sixth-python-0.0.7/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       32 2023-06-17 23:23:30.000000 sixth-python-0.0.7/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.0.7/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.0.7/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     4392 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.0.7/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.0.7/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      850 2023-06-19 15:54:59.000000 sixth-python-0.0.7/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4165 2023-06-19 19:50:08.000000 sixth-python-0.0.7/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.0.7/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.0.7/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.0.7/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3117 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-19 19:58:09.000000 sixth-python-0.0.7/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/
+-rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 11:51:07.000000 sixth-python-0.0.8/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.0.8/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-23 11:51:07.000000 sixth-python-0.0.8/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3773 2023-06-23 11:49:27.000000 sixth-python-0.0.8/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       32 2023-06-17 23:23:30.000000 sixth-python-0.0.8/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.0.8/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-06-19 19:50:08.000000 sixth-python-0.0.8/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.0.8/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-06-19 19:50:08.000000 sixth-python-0.0.8/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     5026 2023-06-22 10:58:05.000000 sixth-python-0.0.8/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.0.8/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      165 2023-06-14 20:44:10.000000 sixth-python-0.0.8/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      850 2023-06-19 15:54:59.000000 sixth-python-0.0.8/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4160 2023-06-23 02:36:25.000000 sixth-python-0.0.8/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.0.8/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.0.8/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.0.8/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3114 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-23 11:51:07.000000 sixth-python-0.0.8/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.0.7/PKG-INFO` & `sixth-python-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.7
+Version: 0.0.8
 Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
@@ -31,29 +31,29 @@
         ## **Installation and usage**
         ### Python
         Sixth SDK is currently only available for [fasiapi](https://fastapi.tiangolo.com/lo/) and can be installed as followed.
         
         #### _Installation_
         
         ```sh
-        pip install six-python
+        pip install sixth-python
         ```
         
         #### _usage_
         ```python
         #import sixth SDK
         from sixth.sdk import SixthSense
         from fastapi import FastAPI
         
         app = FastAPI()
         # initalize app, add routes, middleware, exception handlers etc
         
         
         #....
-        SixthSense(apikey="api key", app=app).init()
+        Sixth(apikey="api key", app=app).init()
         if __name__ == "__main__":
             uvicorn.run(app, host=host, port=PORT)
         
         ```
         
         ### Javascript
         Sixth SDK is currently only available for [express](https://expressjs.com/) and can be installed as followed.
```

### Comparing `sixth-python-0.0.7/README.md` & `sixth-python-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 ```sh
 pip install six-python
 ```
 
 #### _usage_
 ```python
 #import sixth SDK
-from sixth.sdk import SixthSense
+from sixth.sdk import Sixth
 from fastapi import FastAPI
 
 app = FastAPI()
 # initalize app, add routes, middleware, exception handlers etc
 
 
 #....
-SixthSense(apikey="api key", app=app).init()
+Sixth(apikey="api key", app=app).init()
 if __name__ == "__main__":
     uvicorn.run(app, host=host, port=PORT)
 
 ```
 
 ### Javascript
 Sixth SDK is currently only available for [express](https://expressjs.com/) and can be installed as followed.
```

### Comparing `sixth-python-0.0.7/setup.py` & `sixth-python-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Six offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
 
@@ -31,29 +31,29 @@
 ## **Installation and usage**
 ### Python
 Sixth SDK is currently only available for [fasiapi](https://fastapi.tiangolo.com/lo/) and can be installed as followed.
 
 #### _Installation_
 
 ```sh
-pip install six-python
+pip install sixth-python
 ```
 
 #### _usage_
 ```python
 #import sixth SDK
 from sixth.sdk import SixthSense
 from fastapi import FastAPI
 
 app = FastAPI()
 # initalize app, add routes, middleware, exception handlers etc
 
 
 #....
-SixthSense(apikey="api key", app=app).init()
+Sixth(apikey="api key", app=app).init()
 if __name__ == "__main__":
     uvicorn.run(app, host=host, port=PORT)
 
 ```
 
 ### Javascript
 Sixth SDK is currently only available for [express](https://expressjs.com/) and can be installed as followed.
```

### Comparing `sixth-python-0.0.7/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.0.8/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.7/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.0.8/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.7/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.0.8/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.7/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.0.8/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -69,31 +69,42 @@
         out=ast.literal_eval(string)
         return out
         
     async def dispatch(self,request: Request,call_next) -> None:
         host = request.client.host
         route = request.scope["path"]
         route = re.sub(r'\W+', '~', route)
-        rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
-        if rate_limit_resp.status_code == 200:
-            rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
-            self._config.rate_limiter[route] = rate_limit
-            preferred_id = host if self._config.rate_limiter[route].unique_id == "" or self._config.rate_limiter[route].unique_id == "host" else self._config.rate_limiter[route].unique_id
-            _response = await call_next(request)
-            if self._is_rate_limit_reached(preferred_id, route): 
-                return _response
+        #fail safe if there is an internal server error our servers are currenly in maintnance
+        try:
+            rate_limit_resp = requests.get("https://backend.withsix.co/project-config/config/get-route-rate-limit/"+self._apikey+"/"+route)
+            body = await request.body()
+            await self.set_body(request, body)
+            body = await self._parse_bools(body)
+            if rate_limit_resp.status_code == 200:
+                try:
+                    rate_limit = schemas.RateLimiter.parse_obj(rate_limit_resp.json())
+                    self._config.rate_limiter[route] = rate_limit
+                    preferred_id = host if self._config.rate_limiter[route].unique_id == "" or self._config.rate_limiter[route].unique_id == "host" else body[self._config.rate_limiter[route].unique_id]
+                    print("preferred id is ", preferred_id)
+                    _response = await call_next(request)
+                    if self._is_rate_limit_reached(preferred_id, route): 
+                        return _response
+                    else:
+                        temp_payload = rate_limit.error_payload.values()
+                        final = {}
+                        for c in temp_payload:
+                            for keys in c:
+                                if keys != "uid":
+                                    final[keys] = c[keys]
+                        output= final
+                        _response.headers["content-length"]= str(len(str(output).encode()))
+                        return Response(json.dumps(output), status_code=401, headers=_response.headers)
+                except:
+                    _response = await call_next(request)
+                    return _response
             else:
-                temp_payload = rate_limit.error_payload.values()
-                final = {}
-                for c in temp_payload:
-                    for keys in c:
-                        if keys != "uid":
-                            final[keys] = c[keys]
-                output= final
-                _response.headers["content-length"]= str(len(str(output).encode()))
-                return Response(json.dumps(output), status_code=401, headers=_response.headers)
-        else:
-            output={
-                    "message": "something went wrong"
-                }
-            _response.headers["content-length"]= str(len(str(output).encode()))
-            return Response(json.dumps(output), status_code=500)
+                #fail safe if there is an internal server error our servers are currenly in maintnance
+                _response = await call_next(request)
+                return _response
+        except:
+            _response = await call_next(request)
+            return _response
```

### Comparing `sixth-python-0.0.7/sixth/schemas.py` & `sixth-python-0.0.8/sixth/schemas.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.7/sixth/sdk.py` & `sixth-python-0.0.8/sixth/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import json
 import re
 from pydantic.error_wrappers import ValidationError
 
 load_dotenv()
 
 
-class SixthSense():
+class Sixth():
     def __init__(self, apikey: str, app: FastAPI):
         self._apikey = apikey
         self._app = app 
 
     def init(self):
         _base_url = "https://backend.withsix.co"
         _project_config_resp = requests.get(_base_url+"/project-config/config/"+self._apikey)
```

### Comparing `sixth-python-0.0.7/sixth/utils/encryption_utils.py` & `sixth-python-0.0.8/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.7/sixth/utils/time_utils.py` & `sixth-python-0.0.8/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.7/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.0.8/sixth_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.0.7
+Version: 0.0.8
 Summary: Six offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
@@ -31,29 +31,29 @@
         ## **Installation and usage**
         ### Python
         Sixth SDK is currently only available for [fasiapi](https://fastapi.tiangolo.com/lo/) and can be installed as followed.
         
         #### _Installation_
         
         ```sh
-        pip install six-python
+        pip install sixth-python
         ```
         
         #### _usage_
         ```python
         #import sixth SDK
         from sixth.sdk import SixthSense
         from fastapi import FastAPI
         
         app = FastAPI()
         # initalize app, add routes, middleware, exception handlers etc
         
         
         #....
-        SixthSense(apikey="api key", app=app).init()
+        Sixth(apikey="api key", app=app).init()
         if __name__ == "__main__":
             uvicorn.run(app, host=host, port=PORT)
         
         ```
         
         ### Javascript
         Sixth SDK is currently only available for [express](https://expressjs.com/) and can be installed as followed.
```

### Comparing `sixth-python-0.0.7/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.0.8/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.0.7/sixth_python.egg-info/requires.txt` & `sixth-python-0.0.8/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*

