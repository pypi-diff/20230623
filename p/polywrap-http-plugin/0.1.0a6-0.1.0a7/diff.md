# Comparing `tmp/polywrap_http_plugin-0.1.0a6.tar.gz` & `tmp/polywrap_http_plugin-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_http_plugin-0.1.0a6.tar", max compression
+gzip compressed data, was "polywrap_http_plugin-0.1.0a7.tar", max compression
```

## Comparing `polywrap_http_plugin-0.1.0a6.tar` & `polywrap_http_plugin-0.1.0a7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1713 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/README.md
--rw-r--r--   0        0        0     3658 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/py.typed
--rw-r--r--   0        0        0      163 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/__init__.py
--rw-r--r--   0        0        0     1322 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/module.py
--rw-r--r--   0        0        0     1527 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/types.py
--rw-r--r--   0        0        0     6044 2023-05-09 18:16:20.636005 polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/wrap_info.py
--rw-r--r--   0        0        0     1369 2023-05-09 18:15:59.859879 polywrap_http_plugin-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1561 2023-06-23 18:09:58.464667 polywrap_http_plugin-0.1.0a7/README.md
+-rw-r--r--   0        0        0     4726 2023-06-23 18:09:58.464667 polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:09:58.464667 polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/py.typed
+-rw-r--r--   0        0        0      163 2023-06-23 18:10:16.689057 polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/wrap/__init__.py
+-rw-r--r--   0        0        0     1247 2023-06-23 18:10:16.689057 polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/wrap/module.py
+-rw-r--r--   0        0        0     1506 2023-06-23 18:10:16.689057 polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/wrap/types.py
+-rw-r--r--   0        0        0     8589 2023-06-23 18:10:16.689057 polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1363 2023-06-23 18:09:58.464667 polywrap_http_plugin-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a7/PKG-INFO
```

### Comparing `polywrap_http_plugin-0.1.0a6/README.md` & `polywrap_http_plugin-0.1.0a7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,48 @@
-# @polywrap/http-plugin-js
+# polywrap-http-plugin
 
 Http plugin currently supports two different methods `GET` and `POST`. Similar to calling axios, when defining request you need to specify a response type. Headers and query parameters may also be defined.
 
 ## Response Types
 
 `TEXT` - The server will respond with text, the HTTP plugin will return the text as-is.
 
 `BINARY` - The server will respond with binary data (_bytes_), the HTTP plugin will encode as a **base64** string and return it.
 
 ## GET request
 
 Below is sample invocation of the `GET` request with custom request headers and query parameters (`urlParams`).
 
 ```python
-result = await client.invoke(
-    InvokerOptions(
-        uri="wrap://ens/http.polywrap.eth",
-        method="get",
-        args={
-            "url": "http://www.example.com/api",
-            "request": {
-                "responseType": "TEXT",
-                "urlParams": [{"key": "query", "value": "foo"}],
-                "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
-            },
+result = client.invoke(
+    uri="wrap://ens/http.polywrap.eth",
+    method="get",
+    args={
+        "url": "http://www.example.com/api",
+        "request": {
+            "responseType": "TEXT",
+            "urlParams": [{"key": "query", "value": "foo"}],
+            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
         },
-    )
+    },
 )
 ```
 
 ## POST request
 
 Below is sample invocation of the `POST` request with custom request headers and query parameters (`urlParams`). It is also possible to set request body as shown below.
 
 ```python
-response = await client.invoke(
-    InvokerOptions(
-        uri="wrap://ens/http.polywrap.eth",
-        method="post",
-        args={
-            "url": "http://www.example.com/api",
-            "request": {
-                "responseType": "TEXT",
-                "urlParams": [{"key": "query", "value": "foo"}],
-                "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
-                "body": "{data: 'test-request'}",
-            }
+response = client.invoke(
+    uri="wrap://ens/http.polywrap.eth",
+    method="post",
+    args={
+        "url": "http://www.example.com/api",
+        "request": {
+            "responseType": "TEXT",
+            "urlParams": [{"key": "query", "value": "foo"}],
+            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
+            "body": "{data: 'test-request'}",
         }
-    )
+    }
 )
 ```
```

### Comparing `polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/__init__.py` & `polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """This package contains the HTTP plugin."""
 import base64
-from typing import Optional, cast
+from typing import List, Optional, cast
 
-from httpx import AsyncClient
+from httpx import Client
 from httpx import Response as HttpxResponse
-from polywrap_core import InvokerClient, UriPackageOrWrapper
+from httpx._types import RequestFiles
+from polywrap_core import InvokerClient
 from polywrap_msgpack import GenericMap
 from polywrap_plugin import PluginPackage
 
-from .wrap import ArgsGet, ArgsPost, Module, Response, ResponseType, manifest
+from .wrap import (
+    ArgsGet,
+    ArgsPost,
+    FormDataEntry,
+    Module,
+    Response,
+    ResponseType,
+    manifest,
+)
 
 
 def _is_response_binary(args: ArgsGet) -> bool:
     if args.get("request") is None:
         return False
     if not args["request"]:
         return False
@@ -27,32 +36,32 @@
 
 class HttpPlugin(Module[None]):
     """HTTP plugin."""
 
     def __init__(self):
         """Initialize the HTTP plugin."""
         super().__init__(None)
-        self.client = AsyncClient()
+        self.client = Client()
 
-    async def get(
-        self, args: ArgsGet, client: InvokerClient[UriPackageOrWrapper], env: None
+    def get(
+        self, args: ArgsGet, client: InvokerClient, env: None
     ) -> Optional[Response]:
         """Make a GET request to the given URL."""
         res: HttpxResponse
         if args.get("request") is None:
-            res = await self.client.get(args["url"])
+            res = self.client.get(args["url"])
         elif args["request"] is not None:
-            res = await self.client.get(
+            res = self.client.get(
                 args["url"],
                 params=args["request"].get("urlParams"),
                 headers=args["request"].get("headers"),
                 timeout=cast(float, args["request"].get("timeout")),
             )
         else:
-            res = await self.client.get(args["url"])
+            res = self.client.get(args["url"])
 
         if _is_response_binary(args):
             return Response(
                 status=res.status_code,
                 statusText=res.reason_phrase,
                 headers=GenericMap(dict(res.headers)),
                 body=base64.b64encode(res.content).decode(),
@@ -61,36 +70,50 @@
         return Response(
             status=res.status_code,
             statusText=res.reason_phrase,
             headers=GenericMap(dict(res.headers)),
             body=res.text,
         )
 
-    async def post(
-        self, args: ArgsPost, client: InvokerClient[UriPackageOrWrapper], env: None
+    def post(
+        self, args: ArgsPost, client: InvokerClient, env: None
     ) -> Optional[Response]:
         """Make a POST request to the given URL."""
         res: HttpxResponse
         if args.get("request") is None:
-            res = await self.client.post(args["url"])
+            res = self.client.post(args["url"])
         elif args["request"] is not None:
             content = (
                 args["request"]["body"].encode()
                 if args["request"]["body"] is not None
                 else None
             )
-            res = await self.client.post(
+
+            files = self._get_files_from_form_data(
+                args["request"].get("formData") or []
+            )
+
+            if args["request"].get("headers"):
+                headers = cast(GenericMap[str, str], args["request"]["headers"])
+                if headers["Content-Type"] == "multipart/form-data":
+                    # Let httpx handle the content type if it's multipart/form-data
+                    # because it will automatically generate the boundary.
+                    del headers["Content-Type"]
+
+            res = self.client.post(
                 args["url"],
                 content=content,
+                files=files,
                 params=args["request"].get("urlParams"),
                 headers=args["request"].get("headers"),
                 timeout=cast(float, args["request"].get("timeout")),
             )
+
         else:
-            res = await self.client.post(args["url"])
+            res = self.client.post(args["url"])
 
         if _is_response_binary(args):
             return Response(
                 status=res.status_code,
                 statusText=res.reason_phrase,
                 headers=GenericMap(dict(res.headers)),
                 body=base64.b64encode(res.content).decode(),
@@ -99,11 +122,24 @@
         return Response(
             status=res.status_code,
             statusText=res.reason_phrase,
             headers=GenericMap(dict(res.headers)),
             body=res.text,
         )
 
+    def _get_files_from_form_data(self, form_data: List[FormDataEntry]) -> RequestFiles:
+        files: RequestFiles = {}
+        for entry in form_data:
+            file_content = cast(str, entry["value"]) if entry.get("value") else ""
+            if entry.get("type"):
+                file_content = (
+                    base64.b64decode(cast(str, entry["value"]).encode())
+                    if entry.get("value")
+                    else bytes()
+                )
+            files[entry["name"]] = file_content
+        return files
+
 
 def http_plugin():
     """Factory function for the HTTP plugin."""
     return PluginPackage(module=HttpPlugin(), manifest=manifest)
```

### Comparing `polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/module.py` & `polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/wrap/module.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TypeVar, Generic, TypedDict, Optional
 
 from .types import *
 
-from polywrap_core import InvokerClient, UriPackageOrWrapper
+from polywrap_core import InvokerClient
 from polywrap_plugin import PluginModule
 from polywrap_msgpack import GenericMap
 
 TConfig = TypeVar("TConfig")
 
 
 ArgsGet = TypedDict("ArgsGet", {
@@ -30,24 +30,24 @@
         # NOTE: This is used to dynamically add WRAP ABI compatible methods to the class
         instance = super().__new__(cls)
         setattr(instance, "get", instance.get)
         setattr(instance, "post", instance.post)
         return instance
 
     @abstractmethod
-    async def get(
+    def get(
         self,
         args: ArgsGet,
-        client: InvokerClient[UriPackageOrWrapper],
+        client: InvokerClient,
         env: None
     ) -> Optional["Response"]:
         pass
 
     @abstractmethod
-    async def post(
+    def post(
         self,
         args: ArgsPost,
-        client: InvokerClient[UriPackageOrWrapper],
+        client: InvokerClient,
         env: None
     ) -> Optional["Response"]:
         pass
```

### Comparing `polywrap_http_plugin-0.1.0a6/polywrap_http_plugin/wrap/types.py` & `polywrap_http_plugin-0.1.0a7/polywrap_http_plugin/wrap/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: This is an auto-generated file. All modifications will be overwritten.
 # type: ignore
 from __future__ import annotations
 
 from typing import TypedDict, Optional
 from enum import IntEnum
 
-from polywrap_core import InvokerClient, Uri, UriPackageOrWrapper
+from polywrap_core import InvokerClient, Uri
 from polywrap_msgpack import GenericMap
 
 
 ### Env START ###
 
 ### Env END ###
```

### Comparing `polywrap_http_plugin-0.1.0a6/PKG-INFO` & `polywrap_http_plugin-0.1.0a7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 Metadata-Version: 2.1
 Name: polywrap-http-plugin
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: 
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: polywrap-core (>=0.1.0a29,<0.2.0)
-Requires-Dist: polywrap-manifest (>=0.1.0a29,<0.2.0)
-Requires-Dist: polywrap-msgpack (>=0.1.0a29,<0.2.0)
-Requires-Dist: polywrap-plugin (==0.1.0a29)
+Requires-Dist: polywrap-core (>=0.1.0a33,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0a33,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0a33,<0.2.0)
+Requires-Dist: polywrap-plugin (==0.1.0a33)
 Description-Content-Type: text/markdown
 
-# @polywrap/http-plugin-js
+# polywrap-http-plugin
 
 Http plugin currently supports two different methods `GET` and `POST`. Similar to calling axios, when defining request you need to specify a response type. Headers and query parameters may also be defined.
 
 ## Response Types
 
 `TEXT` - The server will respond with text, the HTTP plugin will return the text as-is.
 
 `BINARY` - The server will respond with binary data (_bytes_), the HTTP plugin will encode as a **base64** string and return it.
 
 ## GET request
 
 Below is sample invocation of the `GET` request with custom request headers and query parameters (`urlParams`).
 
 ```python
-result = await client.invoke(
-    InvokerOptions(
-        uri="wrap://ens/http.polywrap.eth",
-        method="get",
-        args={
-            "url": "http://www.example.com/api",
-            "request": {
-                "responseType": "TEXT",
-                "urlParams": [{"key": "query", "value": "foo"}],
-                "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
-            },
+result = client.invoke(
+    uri="wrap://ens/http.polywrap.eth",
+    method="get",
+    args={
+        "url": "http://www.example.com/api",
+        "request": {
+            "responseType": "TEXT",
+            "urlParams": [{"key": "query", "value": "foo"}],
+            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
         },
-    )
+    },
 )
 ```
 
 ## POST request
 
 Below is sample invocation of the `POST` request with custom request headers and query parameters (`urlParams`). It is also possible to set request body as shown below.
 
 ```python
-response = await client.invoke(
-    InvokerOptions(
-        uri="wrap://ens/http.polywrap.eth",
-        method="post",
-        args={
-            "url": "http://www.example.com/api",
-            "request": {
-                "responseType": "TEXT",
-                "urlParams": [{"key": "query", "value": "foo"}],
-                "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
-                "body": "{data: 'test-request'}",
-            }
+response = client.invoke(
+    uri="wrap://ens/http.polywrap.eth",
+    method="post",
+    args={
+        "url": "http://www.example.com/api",
+        "request": {
+            "responseType": "TEXT",
+            "urlParams": [{"key": "query", "value": "foo"}],
+            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
+            "body": "{data: 'test-request'}",
         }
-    )
+    }
 )
 ```
```

