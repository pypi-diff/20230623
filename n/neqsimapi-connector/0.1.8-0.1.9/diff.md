# Comparing `tmp/neqsimapi_connector-0.1.8.tar.gz` & `tmp/neqsimapi_connector-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neqsimapi_connector-0.1.8.tar", max compression
+gzip compressed data, was "neqsimapi_connector-0.1.9.tar", max compression
```

## Comparing `neqsimapi_connector-0.1.8.tar` & `neqsimapi_connector-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1039 2023-05-26 10:31:57.077727 neqsimapi_connector-0.1.8/README.md
--rw-r--r--   0        0        0     4620 2023-06-14 13:33:15.881449 neqsimapi_connector-0.1.8/neqsimapi_connector/BearerAuth.py
--rw-r--r--   0        0        0     4138 2023-06-14 13:24:22.875049 neqsimapi_connector-0.1.8/neqsimapi_connector/Connector.py
--rw-r--r--   0        0        0      597 2023-06-15 12:02:06.013980 neqsimapi_connector-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 neqsimapi_connector-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1047 2023-06-23 20:20:45.259978 neqsimapi_connector-0.1.9/README.md
+-rw-r--r--   0        0        0     4620 2023-06-14 13:33:15.881449 neqsimapi_connector-0.1.9/neqsimapi_connector/BearerAuth.py
+-rw-r--r--   0        0        0     4951 2023-06-23 20:20:13.482421 neqsimapi_connector-0.1.9/neqsimapi_connector/Connector.py
+-rw-r--r--   0        0        0      606 2023-06-23 20:21:04.763585 neqsimapi_connector-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1985 1970-01-01 00:00:00.000000 neqsimapi_connector-0.1.9/PKG-INFO
```

### Comparing `neqsimapi_connector-0.1.8/README.md` & `neqsimapi_connector-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 c = neqsim_api_connector()
 res = c.post("DEMO/demo-process/simulate", data=data)
 print(res)
 ```
 
 # Install using pip
 Usage of NeqSimAPI is limited to equinor users, but the package is available on pip.  
-```python -m pip neqsimapi_connector```
+```python -m pip install neqsimapi_connector```
```

### Comparing `neqsimapi_connector-0.1.8/neqsimapi_connector/BearerAuth.py` & `neqsimapi_connector-0.1.9/neqsimapi_connector/BearerAuth.py`

 * *Files identical despite different names*

### Comparing `neqsimapi_connector-0.1.8/neqsimapi_connector/Connector.py` & `neqsimapi_connector-0.1.9/neqsimapi_connector/Connector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from urllib.parse import urljoin
 
 import requests
 
 from neqsimapi_connector.BearerAuth import BearerAuth
 
 
@@ -50,15 +51,15 @@
 
         if auth is None:
             auth = get_auth_NeqSimAPI()
         elif isinstance(auth, str):
             auth = BearerAuth(str)
         elif isinstance(auth, dict) and "access_result" in auth:
             auth = BearerAuth(auth["access_result"])
-        
+
         self.session = requests.Session()
         self.session.auth = auth
         if verifySSL is False:
             requests.packages.urllib3.disable_warnings(
                 requests.packages.urllib3.exceptions.InsecureRequestWarning
             )
         self.session.verify = verifySSL
@@ -71,20 +72,20 @@
             a_sync (bool, optional): Set False to loop internally while waiting for a reply from the calculation. Defaults to True.
 
         Returns:
             dict: Results when finished or dictionary with status.
         """
         url = urljoin(self.base_url, f"results/{calculation_id}")
         res = self.session.get(url)
-
-        res = res.json()
+        res.raise_for_status()
 
         if a_sync:
-            return res
+            return res.json()
         else:
+            res = res.json()
             while isinstance(res, dict) and 'status' in res.keys() and res['status'] == 'working':
                 res = self.get_results(calculation_id=calculation_id)
 
             if isinstance(res, dict) and 'result' in res.keys():
                 res = res['result']
 
             return res
@@ -100,14 +101,25 @@
             dict: Result or status dict from end point.
         """
 
         if self.base_url not in url:
             url = urljoin(self.base_url, url)
         res = self.session.post(url, json=data)
 
+        if res.status_code == 422:
+            try:
+                d = json.loads(res.text)
+                property = d["detail"][0]["loc"][1]
+                msg = d["detail"][0]["loc"][1]
+            except:
+                pass # Failed failing
+            
+            raise ValueError(
+                    f"Failed getting result input {property} is out of range, {msg}")
+
         res.raise_for_status()
 
         return res.json()
 
     def post_async(self, url: str, data: dict) -> dict:
         """Start async calculation and get status result.
         NB! Results must be gotten with get_results()
@@ -119,14 +131,25 @@
         Returns:
             dict: Status dict or None if endpoint is not async. 
         """
         if self.base_url not in url:
             url = urljoin(self.base_url, url)
         res = self.session.post(url, json=data)
 
+        if res.status_code == 422:
+            try:
+                d = json.loads(res.text)
+                property = d["detail"][0]["loc"][1]
+                msg = d["detail"][0]["loc"][1]
+            except:
+                pass # Failed failing
+            
+            raise ValueError(
+                    f"Failed getting result input {property} is out of range, {msg}")
+        
         res.raise_for_status()
 
         if isinstance(res.json(), dict) and 'id' in res.json().keys():
             id = res.json()
             status = id['status']
             id = id['id']
             return id, status
```

### Comparing `neqsimapi_connector-0.1.8/pyproject.toml` & `neqsimapi_connector-0.1.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neqsimapi-connector"
-version = "0.1.8"
+version = "0.1.9"
 description = "A python package to simplify calling NeqSimAPI for end-users."
 authors = ["Åsmund Våge Fannemel <asmf@equinor.com>"]
 readme = "README.md"
 packages = [{include = "neqsimapi_connector"}]
 license = "MIT"
 repository = "https://github.com/equinor/NeqSimAPI-connector"
 
@@ -12,11 +12,12 @@
 python = "^3.6"
 msal = "^1.20.0"
 msal-extensions = "^1.0.0"
 requests = "^2.27.1"
 
 # [tool.poetry.group.dev.dependencies]
 # autopep8 = "^2.0.2"
+# pytest
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `neqsimapi_connector-0.1.8/PKG-INFO` & `neqsimapi_connector-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neqsimapi-connector
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package to simplify calling NeqSimAPI for end-users.
 Home-page: https://github.com/equinor/NeqSimAPI-connector
 License: MIT
 Author: Åsmund Våge Fannemel
 Author-email: asmf@equinor.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -49,8 +49,8 @@
 c = neqsim_api_connector()
 res = c.post("DEMO/demo-process/simulate", data=data)
 print(res)
 ```
 
 # Install using pip
 Usage of NeqSimAPI is limited to equinor users, but the package is available on pip.  
-```python -m pip neqsimapi_connector```
+```python -m pip install neqsimapi_connector```
```

