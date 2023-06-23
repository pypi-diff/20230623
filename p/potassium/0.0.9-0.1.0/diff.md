# Comparing `tmp/potassium-0.0.9.tar.gz` & `tmp/potassium-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potassium-0.0.9.tar", last modified: Thu May 25 22:30:00 2023, max compression
+gzip compressed data, was "potassium-0.1.0.tar", last modified: Fri Jun 23 18:01:49 2023, max compression
```

## Comparing `potassium-0.0.9.tar` & `potassium-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:30:00.474604 potassium-0.0.9/
--rw-r--r--   0 erik       (501) staff       (20)    11357 2023-04-24 01:09:41.000000 potassium-0.0.9/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)     7939 2023-05-25 22:30:00.474489 potassium-0.0.9/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     7273 2023-05-12 03:11:03.000000 potassium-0.0.9/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:30:00.473780 potassium-0.0.9/potassium/
--rw-r--r--   0 erik       (501) staff       (20)       83 2023-04-28 20:13:33.000000 potassium-0.0.9/potassium/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)      221 2023-04-24 01:09:41.000000 potassium-0.0.9/potassium/hooks.py
--rw-r--r--   0 erik       (501) staff       (20)     6946 2023-05-25 22:13:36.000000 potassium-0.0.9/potassium/potassium.py
--rw-r--r--   0 erik       (501) staff       (20)     4063 2023-04-28 21:55:56.000000 potassium-0.0.9/potassium/store.py
--rw-r--r--   0 erik       (501) staff       (20)     1305 2023-04-28 21:46:28.000000 potassium-0.0.9/potassium/store_test.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:30:00.474332 potassium-0.0.9/potassium.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     7939 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      297 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       31 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       10 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       38 2023-05-25 22:30:00.474636 potassium-0.0.9/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1258 2023-05-25 22:27:50.000000 potassium-0.0.9/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 18:01:49.967061 potassium-0.1.0/
+-rw-r--r--   0 erik       (501) staff       (20)    11357 2023-04-24 01:09:41.000000 potassium-0.1.0/LICENSE
+-rw-r--r--   0 erik       (501) staff       (20)     7116 2023-06-23 18:01:49.966940 potassium-0.1.0/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     6450 2023-06-23 18:01:41.000000 potassium-0.1.0/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 18:01:49.966274 potassium-0.1.0/potassium/
+-rw-r--r--   0 erik       (501) staff       (20)       83 2023-06-06 23:50:04.000000 potassium-0.1.0/potassium/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)      221 2023-04-24 01:09:41.000000 potassium-0.1.0/potassium/hooks.py
+-rw-r--r--   0 erik       (501) staff       (20)     6323 2023-06-23 18:01:41.000000 potassium-0.1.0/potassium/potassium.py
+-rw-r--r--   0 erik       (501) staff       (20)     5500 2023-06-23 18:01:41.000000 potassium-0.1.0/potassium/store.py
+-rw-r--r--   0 erik       (501) staff       (20)     2397 2023-06-23 18:01:41.000000 potassium-0.1.0/potassium/store_test.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 18:01:49.966778 potassium-0.1.0/potassium.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     7116 2023-06-23 18:01:49.000000 potassium-0.1.0/potassium.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      297 2023-06-23 18:01:49.000000 potassium-0.1.0/potassium.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-06-23 18:01:49.000000 potassium-0.1.0/potassium.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)       37 2023-06-23 18:01:49.000000 potassium-0.1.0/potassium.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       10 2023-06-23 18:01:49.000000 potassium-0.1.0/potassium.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       38 2023-06-23 18:01:49.967104 potassium-0.1.0/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1275 2023-06-23 18:01:41.000000 potassium-0.1.0/setup.py
```

### Comparing `potassium-0.0.9/LICENSE` & `potassium-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `potassium-0.0.9/PKG-INFO` & `potassium-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potassium
-Version: 0.0.9
+Version: 0.1.0
 Summary: The potassium package is a flask-like HTTP server for serving large AI models
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: Apache License 2.0
 Keywords: Banana server,HTTP server,Banana,Framework
 Classifier: Development Status :: 3 - Alpha
@@ -51,17 +51,18 @@
 This downloads boilerplate for your potassium app, and automatically installs potassium into the venv.
 
 2. Create a new project directory with 
 ```bash
 banana init my-app
 cd my-app
 ```
-3. Start the hot-reload dev server
+3. Start the dev server
 ```bash
-banana dev
+. ./venv/bin/activate
+python3 app.py
 ```
 
 4. Call your API (from a separate terminal)
 ```bash
 curl -X POST -H "Content-Type: application/json" -d '{"prompt": "Hello I am a [MASK] model."}' http://localhost:8000/
 ``` 
 
@@ -175,15 +176,15 @@
 There may only be one `@app.init` function.
 
 ---
 
 ## @app.handler()
 
 ```python
-@app.handler("/", gpu=True)
+@app.handler("/")
 def handler(context: dict, request: Request) -> Response:
     
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     return Response(
@@ -192,19 +193,19 @@
     )
 ```
 
 The `@app.handler` decorated function runs for every http call, and is used to run inference or training workloads against your model(s).
 
 You may configure as many `@app.handler` functions as you'd like, with unique API routes.
 
-The `gpu=True` argument allows the handler to access the prewarmed context value, and runs the handler as blocking. While the handler is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
+The context dict passed in is a mutable reference, so you can modify it in-place to persist objects between warm handlers.
 
 ---
 
-## @app.background(path="/background", gpu=True)
+## @app.background(path="/background")
 
 ```python
 @app.background("/background")
 def handler(context: dict, request: Request) -> Response:
 
     prompt = request.json.get("prompt")
     model = context.get("model")
@@ -213,31 +214,31 @@
     send_webhook(url="http://localhost:8001", json={"outputs": outputs})
 
     return
 ```
 
 The `@app.background()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
 
-When invoked, the client immediately returns a `{"success": true}` message.
+When invoked, the server immediately returns a `{"success": true}` message.
 
 You may configure as many `@app.background` functions as you'd like, with unique API routes.
 
-The `gpu=True` argument allows the background handler to access the prewarmed context value, and runs the child background thread as blocking. While the child thread is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
----
+The context dict passed in is a mutable reference, so you can modify it in-place to persist objects between warm handlers.
 
+---
 ## app.serve()
 
 `app.serve` runs the server, and is a blocking operation.
 
 
 ---
 
 # Store
-Potassium includes a key-value storage primative, to help users persist data between calls. This is often used to implement patterns such as an async-worker queue where one background task runs inference and saves the result to the Store, with another handler set to `gpu=False` built to fetch the result.
+Potassium includes a key-value storage primative, to help users persist data between calls.
 
 Example usage: your own Redis backend (encouraged)
 ```
 from potassium.store import Store, RedisConfig
 
 store = Store(
     backend="redis",
```

### Comparing `potassium-0.0.9/README.md` & `potassium-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 This downloads boilerplate for your potassium app, and automatically installs potassium into the venv.
 
 2. Create a new project directory with 
 ```bash
 banana init my-app
 cd my-app
 ```
-3. Start the hot-reload dev server
+3. Start the dev server
 ```bash
-banana dev
+. ./venv/bin/activate
+python3 app.py
 ```
 
 4. Call your API (from a separate terminal)
 ```bash
 curl -X POST -H "Content-Type: application/json" -d '{"prompt": "Hello I am a [MASK] model."}' http://localhost:8000/
 ``` 
 
@@ -157,15 +158,15 @@
 There may only be one `@app.init` function.
 
 ---
 
 ## @app.handler()
 
 ```python
-@app.handler("/", gpu=True)
+@app.handler("/")
 def handler(context: dict, request: Request) -> Response:
     
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     return Response(
@@ -174,19 +175,19 @@
     )
 ```
 
 The `@app.handler` decorated function runs for every http call, and is used to run inference or training workloads against your model(s).
 
 You may configure as many `@app.handler` functions as you'd like, with unique API routes.
 
-The `gpu=True` argument allows the handler to access the prewarmed context value, and runs the handler as blocking. While the handler is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
+The context dict passed in is a mutable reference, so you can modify it in-place to persist objects between warm handlers.
 
 ---
 
-## @app.background(path="/background", gpu=True)
+## @app.background(path="/background")
 
 ```python
 @app.background("/background")
 def handler(context: dict, request: Request) -> Response:
 
     prompt = request.json.get("prompt")
     model = context.get("model")
@@ -195,31 +196,31 @@
     send_webhook(url="http://localhost:8001", json={"outputs": outputs})
 
     return
 ```
 
 The `@app.background()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
 
-When invoked, the client immediately returns a `{"success": true}` message.
+When invoked, the server immediately returns a `{"success": true}` message.
 
 You may configure as many `@app.background` functions as you'd like, with unique API routes.
 
-The `gpu=True` argument allows the background handler to access the prewarmed context value, and runs the child background thread as blocking. While the child thread is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
----
+The context dict passed in is a mutable reference, so you can modify it in-place to persist objects between warm handlers.
 
+---
 ## app.serve()
 
 `app.serve` runs the server, and is a blocking operation.
 
 
 ---
 
 # Store
-Potassium includes a key-value storage primative, to help users persist data between calls. This is often used to implement patterns such as an async-worker queue where one background task runs inference and saves the result to the Store, with another handler set to `gpu=False` built to fetch the result.
+Potassium includes a key-value storage primative, to help users persist data between calls.
 
 Example usage: your own Redis backend (encouraged)
 ```
 from potassium.store import Store, RedisConfig
 
 store = Store(
     backend="redis",
```

### Comparing `potassium-0.0.9/potassium/store.py` & `potassium-0.1.0/potassium/store.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,124 @@
-import time, os
+import time
+import os
 from typing import Union
 import shelve
 from threading import Thread, Lock
 import atexit
 import redis
+import boto3
 import pickle
 import json
 
 
 class Entry():
     def __init__(self, value, expiration):
         self.value = value
         self.expiration = expiration
+
+
 class RedisConfig():
-    def __init__(self, host:str, port:str, username:str = None, password:str = None, db:int = 0, encoding:str = "json"):
+    def __init__(self, host: str, port: str, username: str = None, password: str = None, db: int = 0, encoding: str = "json"):
         "encoding can be 'json' or 'pickle'. JSON is default.\nPickle has better support for arbitrary python types, but using pickle with a remote redis introduces a large security risk, see https://stackoverflow.com/questions/2259270/pickle-or-json/2259351#2259351"
         # validate args
         encodings = ["json", "pickle"]
         if encoding not in encodings:
-            raise ValueError("redis config encoding must be one of the following:", encodings)
-        
+            raise ValueError(
+                "redis config encoding must be one of the following:", encodings)
+
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.db = db
         self.encoding = encoding
+
+
+class S3Config():
+    def __init__(self, aws_access_key_id, aws_secret_access_key, bucket, encoding: str = "json"):
+        "encoding can be 'json' or 'pickle'. JSON is default.\nPickle has better support for arbitrary python types, but using pickle across the network to s3 introduces a large security risk, see https://stackoverflow.com/questions/2259270/pickle-or-json/2259351#2259351"
+        # validate args
+        encodings = ["json", "pickle"]
+        if encoding not in encodings:
+            raise ValueError(
+                "s3 config encoding must be one of the following:", encodings)
+
+        if aws_access_key_id is None:
+            raise ValueError(
+                "aws_access_key_id must be provided. It is a sensitive key, so ensure it is scoped to the bucket you want to use and not hardcoded in any open source repos.")
+        if aws_secret_access_key is None:
+            raise ValueError(
+                "aws_secret_access_key must be provided. It is a sensitive key, so ensure it is scoped to the bucket you want to use and not hardcoded in any open source repos.")
+
+        self.access_key = aws_access_key_id
+        self.secret_access_key = aws_secret_access_key
+        self.bucket = bucket
+        self.encoding = encoding
+
+
 class Store():
-    def __init__(self, backend: str ="local", config: Union[None, RedisConfig] = None):
+    def __init__(self, backend: str = "redis", config: Union[None, RedisConfig, S3Config] = None):
         # validate args
-        backends = ["local", "redis"]
+        backends = ["redis", "s3"]
         if backend not in backends:
             raise ValueError("backend must be one of the following:", backends)
-        
+
         self.backend = backend
         self.config = config
-         
-        if self.backend == "local": 
-            self._local_store = shelve.open(".localstore")
-            self._lock = Lock()
-            
-            # run TTL gc as thread
-            thread = Thread(target=self._gc)
-            thread.daemon = True
-            thread.start()
-
-            # delete store at exit, to avoid side effects
-            def exit_handler():
-                os.remove(".localstore")
-            atexit.register(exit_handler)
 
         if self.backend == "redis":
             if not isinstance(config, RedisConfig):
                 raise ValueError("redis backends require users to bring their own redis, and configure the potassium store to use it with the config argument. For example, to use a local redis, create store with:\n\nfrom potassium.store import Store, RedisConfig\nstore = Store(backend = 'redis', config = RedisConfig(host = 'localhost', port = 6379))")
-            self._redis_store = redis.Redis(
-                host=config.host, 
+            self._redis_client = redis.Redis(
+                host=config.host,
                 port=config.port,
                 username=config.username,
                 password=config.password,
                 db=config.db,
             )
 
-    def _gc(self):
-        if self.backend == "local":
-            while True:
-                time.sleep(1)
-                with self._lock:
-                    try:
-                        for k, v in self._local_store.items():
-                            if v.expiration < time.time():
-                                del self._local_store[k]
-                    except:
-                        pass
+        if self.backend == "s3":
+            if not isinstance(config, S3Config):
+                raise ValueError("s3 backends require users to bring their own s3 bucket, and configure the potassium store to use it with the config argument. For example, create store with:\n\nfrom potassium.store import Store, S3Config\nstore = Store(backend = 's3', config = S3Config(access_key, secret_access_key, bucket)")
+            session = boto3.Session(
+                aws_access_key_id=config.access_key,
+                aws_secret_access_key=config.secret_access_key
+            )
+            self._s3_client = session.client('s3')
+            self._s3_bucket = config.bucket
 
     def get(self, key: str):
-        if self.backend == "local":
-            with self._lock:
-                entry = self._local_store.get(key)
-            if entry == None:
-                return None
-            return entry.value
-        
         if self.backend == "redis":
-            encoded = self._redis_store.get(key)
+            encoded = self._redis_client.get(key)
             if encoded == None:
                 return None
             if self.config.encoding == "json":
                 return json.loads(encoded)
             if self.config.encoding == "pickle":
                 return pickle.loads(encoded)
-    
-    def set(self, key, value, ttl=600):
-        if self.backend == "local":
-            with self._lock:
-                self._local_store[key] = Entry(
-                    value=value,
-                    expiration=time.time()+ttl
-                )
 
+        if self.backend == "s3":
+            response = self._s3_client.get_object(
+                Bucket=self._s3_bucket, Key=key)
+            encoded = response['Body'].read()
+            if encoded == None:
+                return None
+            if self.config.encoding == "json":
+                return json.loads(encoded.decode('utf-8'))
+            if self.config.encoding == "pickle":
+                return pickle.loads(encoded)
+
+    def set(self, key, value, ttl=600):
         if self.backend == "redis":
             if self.config.encoding == "json":
                 encoded = json.dumps(value)
             if self.config.encoding == "pickle":
                 encoded = pickle.dumps(value)
-            self._redis_store.set(key, encoded, ex=ttl)
+            self._redis_client.set(key, encoded, ex=ttl)
+
+        if self.backend == "s3":
+            if self.config.encoding == "json":
+                encoded = json.dumps(value)
+            if self.config.encoding == "pickle":
+                encoded = pickle.dumps(value)
+            self._s3_client.put_object(
+                Body=encoded, Bucket=self._s3_bucket, Key=key)
```

### Comparing `potassium-0.0.9/potassium.egg-info/PKG-INFO` & `potassium-0.1.0/potassium.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potassium
-Version: 0.0.9
+Version: 0.1.0
 Summary: The potassium package is a flask-like HTTP server for serving large AI models
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: Apache License 2.0
 Keywords: Banana server,HTTP server,Banana,Framework
 Classifier: Development Status :: 3 - Alpha
@@ -51,17 +51,18 @@
 This downloads boilerplate for your potassium app, and automatically installs potassium into the venv.
 
 2. Create a new project directory with 
 ```bash
 banana init my-app
 cd my-app
 ```
-3. Start the hot-reload dev server
+3. Start the dev server
 ```bash
-banana dev
+. ./venv/bin/activate
+python3 app.py
 ```
 
 4. Call your API (from a separate terminal)
 ```bash
 curl -X POST -H "Content-Type: application/json" -d '{"prompt": "Hello I am a [MASK] model."}' http://localhost:8000/
 ``` 
 
@@ -175,15 +176,15 @@
 There may only be one `@app.init` function.
 
 ---
 
 ## @app.handler()
 
 ```python
-@app.handler("/", gpu=True)
+@app.handler("/")
 def handler(context: dict, request: Request) -> Response:
     
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     return Response(
@@ -192,19 +193,19 @@
     )
 ```
 
 The `@app.handler` decorated function runs for every http call, and is used to run inference or training workloads against your model(s).
 
 You may configure as many `@app.handler` functions as you'd like, with unique API routes.
 
-The `gpu=True` argument allows the handler to access the prewarmed context value, and runs the handler as blocking. While the handler is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
+The context dict passed in is a mutable reference, so you can modify it in-place to persist objects between warm handlers.
 
 ---
 
-## @app.background(path="/background", gpu=True)
+## @app.background(path="/background")
 
 ```python
 @app.background("/background")
 def handler(context: dict, request: Request) -> Response:
 
     prompt = request.json.get("prompt")
     model = context.get("model")
@@ -213,31 +214,31 @@
     send_webhook(url="http://localhost:8001", json={"outputs": outputs})
 
     return
 ```
 
 The `@app.background()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
 
-When invoked, the client immediately returns a `{"success": true}` message.
+When invoked, the server immediately returns a `{"success": true}` message.
 
 You may configure as many `@app.background` functions as you'd like, with unique API routes.
 
-The `gpu=True` argument allows the background handler to access the prewarmed context value, and runs the child background thread as blocking. While the child thread is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
----
+The context dict passed in is a mutable reference, so you can modify it in-place to persist objects between warm handlers.
 
+---
 ## app.serve()
 
 `app.serve` runs the server, and is a blocking operation.
 
 
 ---
 
 # Store
-Potassium includes a key-value storage primative, to help users persist data between calls. This is often used to implement patterns such as an async-worker queue where one background task runs inference and saves the result to the Store, with another handler set to `gpu=False` built to fetch the result.
+Potassium includes a key-value storage primative, to help users persist data between calls.
 
 Example usage: your own Redis backend (encouraged)
 ```
 from potassium.store import Store, RedisConfig
 
 store = Store(
     backend="redis",
```

### Comparing `potassium-0.0.9/setup.py` & `potassium-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='potassium',
     packages=['potassium'],
-    version='0.0.9',
+    version='0.1.0',
     license='Apache License 2.0',
     # Give a short description about your library
     description='The potassium package is a flask-like HTTP server for serving large AI models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
     url='https://www.banana.dev',
     keywords=['Banana server', 'HTTP server', 'Banana', 'Framework'],
     setup_requires=['wheel'],
     install_requires=[
         "Flask",
         "requests",
         "termcolor",
-        "redis"
+        "redis",
+        "boto3"
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
```

