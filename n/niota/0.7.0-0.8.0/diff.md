# Comparing `tmp/niota-0.7.0.tar.gz` & `tmp/niota-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niota-0.7.0.tar", last modified: Tue Jan 25 16:33:57 2022, max compression
+gzip compressed data, was "niota-0.8.0.tar", last modified: Fri Jun 23 10:46:35 2023, max compression
```

## Comparing `niota-0.7.0.tar` & `niota-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:57.728109 niota-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-01-25 16:33:57.724109 niota-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-01-25 16:33:48.000000 niota-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:57.724109 niota-0.7.0/niota/
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-01-25 16:33:48.000000 niota-0.7.0/niota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-01-25 16:33:48.000000 niota-0.7.0/niota/chrysalis.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-01-25 16:33:48.000000 niota-0.7.0/niota/encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-01-25 16:33:48.000000 niota-0.7.0/niota/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-01-25 16:33:48.000000 niota-0.7.0/niota/iota_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-01-25 16:33:48.000000 niota-0.7.0/niota/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2022-01-25 16:33:48.000000 niota-0.7.0/niota/niota.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-01-25 16:33:48.000000 niota-0.7.0/niota/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:57.724109 niota-0.7.0/niota.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-01-25 16:33:57.000000 niota-0.7.0/niota.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-01-25 16:33:57.000000 niota-0.7.0/niota.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 16:33:57.000000 niota-0.7.0/niota.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-01-25 16:33:57.000000 niota-0.7.0/niota.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-25 16:33:57.000000 niota-0.7.0/niota.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-25 16:33:57.728109 niota-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-01-25 16:33:48.000000 niota-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:57.724109 niota-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:48.000000 niota-0.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:57.724109 niota-0.7.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:48.000000 niota-0.7.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-01-25 16:33:48.000000 niota-0.7.0/tests/integration/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-25 16:33:48.000000 niota-0.7.0/tests/integration/test_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:57.724109 niota-0.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:48.000000 niota-0.7.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-01-25 16:33:48.000000 niota-0.7.0/tests/unit/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-01-25 16:33:48.000000 niota-0.7.0/tests/unit/test_iota_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:57.724109 niota-0.7.0/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 16:33:48.000000 niota-0.7.0/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-01-25 16:33:48.000000 niota-0.7.0/utils/hello_iota_storage_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:46:35.025562 niota-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-23 10:46:35.025562 niota-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-23 10:46:24.000000 niota-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 10:46:24.000000 niota-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-23 10:46:35.025562 niota-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 10:46:24.000000 niota-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:46:35.017562 niota-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:46:35.021562 niota-0.8.0/src/niota/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-23 10:46:24.000000 niota-0.8.0/src/niota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 10:46:24.000000 niota-0.8.0/src/niota/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-23 10:46:24.000000 niota-0.8.0/src/niota/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-23 10:46:24.000000 niota-0.8.0/src/niota/iota_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-23 10:46:24.000000 niota-0.8.0/src/niota/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-23 10:46:24.000000 niota-0.8.0/src/niota/niota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-23 10:46:24.000000 niota-0.8.0/src/niota/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:46:35.025562 niota-0.8.0/src/niota.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-23 10:46:34.000000 niota-0.8.0/src/niota.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-23 10:46:34.000000 niota-0.8.0/src/niota.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:46:34.000000 niota-0.8.0/src/niota.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 10:46:34.000000 niota-0.8.0/src/niota.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 10:46:34.000000 niota-0.8.0/src/niota.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:46:34.000000 niota-0.8.0/src/niota.egg-info/zip-safe
```

### Comparing `niota-0.7.0/README.md` & `niota-0.8.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,25 @@
 # NIOTA
 
 Make IOTA to be an integrity chain.
 
 Niota registers Asset history records to the integrity chain.
 
-# Installation
+## Installation
 
-The Python binding of [iota.rs](https://github.com/iotaledger/iota.rs/releases). You can download the latest version from the official [nightly.link service](https://nightly.link/iotaledger/iota.rs/workflows/python_binding_publish/dev).
+```shell
+python3 -m pip install niota
+ ```
 
-Two ways to install niota:
+## Unit Testing
 
-1. Insatll by using PyPI (stable versoin)
-
-    ```
-    $ python3 -m pip install niota
-    ```
-
-2. Install manually (latest version)
-
-    ```
-    $ python3 setup.py bdist_wheel
-    $ python3 -m pip install dist/niota-<version>-py3-none-any.whl
-    ```
-
-# Unit Testing
-
-```
-$ pytest -m unit
-```
-
-# Integration Testing
-
-```
-$ pytest -m integration
-```
-
-Known issue: the legacy Chrysalis client which uses the official IOTA Client sometimes raises the error:
-
-```
-niota/chrysalis.py:18: PanicException
----------------------------------------------------------------- Captured stderr call -----------------------------------------------------------------
-thread '<unnamed>' panicked at 'called `Result::unwrap()` on an `Err` value: ReqwestError(reqwest::Error { kind: Request, url: Url { scheme: "https", username: "", password: None, host: Some(Domain("chrysalis-nodes.iota.org")), port: None, path: "/api/v1/info", query: None, fragment: None }, source: TimedOut })', src/client/mod.rs:146:80
-note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
+```shell
+make test
 ```
 
-Rerun the test again and it should work.
-
-
 ## Usage
 
 ### Iota Client
 
 The `IotaClient` class is a client to interact with [IOTA REST API](https://editor.swagger.io/?url=https://raw.githubusercontent.com/rufsam/protocol-rfcs/master/text/0026-rest-api/0026-rest-api.yaml).
 
 Below is a minimal example for connecting to an IOTA hornet node with JWT authentication enabled, and create a message.
```

### Comparing `niota-0.7.0/niota/iota_client.py` & `niota-0.8.0/src/niota/iota_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import requests
 
 from niota import exceptions
 from niota.encoder import hexstr_to_str, str_to_hexstr
-from niota.models import CreateMessageResp, MessageResp, Payload, PayloadContent, SearchMessageResp
-
+from niota.models import (
+    CreateMessageResp,
+    MessageResp,
+    Payload,
+    PayloadContent,
+    SearchMessageResp,
+)
 
 INDEXATION_MESSAGE_TYPE = 2
 
 
 class IotaClient():
     DEFAULT_BASE_URL = 'https://chrysalis-nodes.iota.org'
 
@@ -18,26 +23,26 @@
 
     def _raise_for_error(self, resp: requests.Response):
         try:
             resp.raise_for_status()
         except requests.exceptions.HTTPError as e:
             if resp.status_code >= 500:
                 raise exceptions.NodeInternalServerError(e.response.text) from None
-            elif 'missing or malformed jwt' in resp.text:
+            if 'missing or malformed jwt' in resp.text:
                 raise exceptions.InvalidJWT(e.response.text) from None
-            elif 'message not found' in resp.text:
+            if 'message not found' in resp.text:
                 raise exceptions.MessageNotFound(e.response.text) from None
             raise exceptions.UnknownError(e.response.text)
 
     def health(self):
         resp = self.session.get(f'{self.base_url}/health', headers=self.headers)
         try:
             resp.raise_for_status()
-        except requests.exceptions.HTTPError:
-            raise exceptions.NodeUnhealthy
+        except requests.exceptions.HTTPError as e:
+            raise exceptions.NodeUnhealthy from e
 
     def info(self):
         resp = self.session.get(f'{self.base_url}/api/v1/info', headers=self.headers)
         self._raise_for_error(resp)
         return resp.json()
 
     def create_message(self, index: str, data: str):
```

### Comparing `niota-0.7.0/niota/models.py` & `niota-0.8.0/src/niota/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List
 
 from pydantic import BaseModel
 
-
 hexstr = str
 
 
 class Payload(BaseModel):
     type: int
     index: hexstr
     data: hexstr
@@ -30,23 +29,23 @@
 
 
 class MessageResp(BaseModel):
     data: MessageData
 
 
 class CreateMessageData(BaseModel):
-    messageId: hexstr
+    messageId: str
 
 
 class CreateMessageResp(BaseModel):
     data: CreateMessageData
 
 
 class SearchMessageData(BaseModel):
     index: hexstr
     maxResults: int
     count: int
-    messageIds: List[hexstr]
+    messageIds: List[str]
 
 
 class SearchMessageResp(BaseModel):
     data: SearchMessageData
```

### Comparing `niota-0.7.0/niota/signature.py` & `niota-0.8.0/src/niota/signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
+from typing import Union
+
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
-from typing import Union
 
 
 def load_private_key(pem_private_key: str) -> rsa.RSAPrivateKeyWithSerialization:
     pem_private_key_bytes = pem_private_key.encode('utf-8')
     return serialization.load_pem_private_key(pem_private_key_bytes, password=None)
 
 
@@ -21,50 +22,44 @@
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.TraditionalOpenSSL,
         encryption_algorithm=serialization.NoEncryption(),
     )
     return pem.decode('utf-8')
 
 
-def export_public_key(private_key: rsa.RSAPrivateKeyWithSerialization) -> str:
-    pem = private_key.public_bytes(
+def export_public_key(public_key: rsa.RSAPublicKeyWithSerialization) -> str:
+    pem = public_key.public_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PublicFormat.SubjectPublicKeyInfo,
     )
     return pem.decode('utf-8')
 
 
 def get_pem_public_key(pem_private_key):
     private_key = load_private_key(pem_private_key)
     public_key = private_key.public_key()
     pem_public_key = export_public_key(public_key)
     return pem_public_key
 
 
 def generate_key_pair():
-    private_key = rsa.generate_private_key(
-        public_exponent=65537,
-        key_size=2048,
-        backend=default_backend()
-    )
+    private_key = rsa.generate_private_key(public_exponent=65537, key_size=2048, backend=default_backend())
     return private_key, private_key.public_key()
 
 
-def sign_message(
-    private_key: Union[str, rsa.RSAPrivateKeyWithSerialization],
-    message: str
-):
+def generate_key_pair_in_pem():
+    private_key, public_key = generate_key_pair()
+    return export_private_key(private_key), export_public_key(public_key)
+
+
+def sign_message(private_key: Union[str, rsa.RSAPrivateKeyWithSerialization], message: str):
     if isinstance(private_key, str):
         private_key = load_private_key(private_key)
     signature = private_key.sign(
-        message.encode('utf-8'),
-        padding.PSS(
-            mgf=padding.MGF1(hashes.SHA256()),
-            salt_length=padding.PSS.MAX_LENGTH
-        ),
+        message.encode('utf-8'), padding.PSS(mgf=padding.MGF1(hashes.SHA256()), salt_length=padding.PSS.MAX_LENGTH),
         hashes.SHA256()
     )
     base64_signature = base64.b64encode(signature).decode('utf-8')
     return base64_signature
 
 
 def verify_signature(
@@ -74,21 +69,15 @@
     raise_exception=True,
 ):
     if isinstance(public_key, str):
         public_key = load_public_key(public_key)
     signature = base64.b64decode(base64_signature.encode('utf-8'))
     try:
         public_key.verify(
-            signature,
-            message.encode('utf-8'),
-            padding.PSS(
-                mgf=padding.MGF1(hashes.SHA256()),
-                salt_length=padding.PSS.MAX_LENGTH
-            ),
-            hashes.SHA256()
+            signature, message.encode('utf-8'),
+            padding.PSS(mgf=padding.MGF1(hashes.SHA256()), salt_length=padding.PSS.MAX_LENGTH), hashes.SHA256()
         )
     except InvalidSignature:
         if raise_exception:
             raise
         return False
-    else:
-        return True
+    return True
```

