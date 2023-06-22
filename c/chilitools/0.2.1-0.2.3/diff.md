# Comparing `tmp/chilitools-0.2.1.tar.gz` & `tmp/chilitools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chilitools-0.2.1.tar", max compression
+gzip compressed data, was "chilitools-0.2.3.tar", max compression
```

## Comparing `chilitools-0.2.1.tar` & `chilitools-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     3655 2023-06-22 15:55:36.494990 chilitools-0.2.1/chilitools/__init__.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.2.1/chilitools/api/__init__.py
--rw-r--r--   0        0        0     7160 2023-03-20 16:14:22.242821 chilitools-0.2.1/chilitools/api/connector.py
--rw-r--r--   0        0        0    20888 2023-06-22 02:56:00.106030 chilitools-0.2.1/chilitools/api/endpoints.py
--rw-r--r--   0        0        0     3728 2023-03-21 14:29:37.670561 chilitools-0.2.1/chilitools/api/mycp.py
--rw-r--r--   0        0        0     3114 2022-09-20 16:25:32.069762 chilitools-0.2.1/chilitools/api/response.py
--rw-r--r--   0        0        0        0 2023-06-20 02:25:18.519289 chilitools-0.2.1/chilitools/grafx/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 19:59:39.899564 chilitools-0.2.1/chilitools/grafx/api/__init__.py
--rw-r--r--   0        0        0     1517 2023-06-22 03:37:59.463934 chilitools-0.2.1/chilitools/grafx/api/environment.py
--rw-r--r--   0        0        0     2232 2023-06-20 04:20:59.710105 chilitools-0.2.1/chilitools/grafx/auth.py
--rw-r--r--   0        0        0     1796 2023-06-22 02:21:13.595697 chilitools-0.2.1/chilitools/grafx/connector.py
--rw-r--r--   0        0        0     1558 2023-06-22 15:29:58.303948 chilitools-0.2.1/chilitools/grafx/document.py
--rw-r--r--   0        0        0      661 2023-06-20 20:56:54.535362 chilitools-0.2.1/chilitools/grafx/environment.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.2.1/chilitools/settings/__init__.py
--rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.2.1/chilitools/settings/config.py
--rw-r--r--   0        0        0    12468 2022-09-27 16:58:06.159255 chilitools-0.2.1/chilitools/utilities/ServerMigration.py
--rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.2.1/chilitools/utilities/__init__.py
--rw-r--r--   0        0        0     2104 2022-10-28 20:09:34.951802 chilitools-0.2.1/chilitools/utilities/backoffice.py
--rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.2.1/chilitools/utilities/defaults.py
--rw-r--r--   0        0        0     2069 2023-06-13 15:46:56.759605 chilitools-0.2.1/chilitools/utilities/document.py
--rw-r--r--   0        0        0      897 2022-07-21 19:16:13.652722 chilitools-0.2.1/chilitools/utilities/errors.py
--rw-r--r--   0        0        0     6022 2022-10-28 20:05:22.841538 chilitools-0.2.1/chilitools/utilities/file.py
--rw-r--r--   0        0        0      807 2023-06-20 15:02:52.753030 chilitools-0.2.1/chilitools/utilities/logger.py
--rw-r--r--   0        0        0      509 2022-06-29 19:01:07.878458 chilitools-0.2.1/chilitools/utilities/strings.py
--rw-r--r--   0        0        0     3831 2023-03-21 15:07:48.139637 chilitools-0.2.1/chilitools/utilities/xmltools.py
--rw-r--r--   0        0        0      505 2023-06-22 15:55:30.180729 chilitools-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 chilitools-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3655 2023-06-22 22:39:37.123359 chilitools-0.2.3/chilitools/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257043 chilitools-0.2.3/chilitools/api/__init__.py
+-rw-r--r--   0        0        0     7160 2023-03-20 16:14:22.242821 chilitools-0.2.3/chilitools/api/connector.py
+-rw-r--r--   0        0        0    20998 2023-06-22 22:35:35.839958 chilitools-0.2.3/chilitools/api/endpoints.py
+-rw-r--r--   0        0        0     3728 2023-03-21 14:29:37.670561 chilitools-0.2.3/chilitools/api/mycp.py
+-rw-r--r--   0        0        0     3114 2022-09-20 16:25:32.069762 chilitools-0.2.3/chilitools/api/response.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:25:18.519289 chilitools-0.2.3/chilitools/grafx/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:59:39.899564 chilitools-0.2.3/chilitools/grafx/api/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-22 21:44:25.944416 chilitools-0.2.3/chilitools/grafx/api/environment.py
+-rw-r--r--   0        0        0      513 2023-06-22 22:42:14.136612 chilitools-0.2.3/chilitools/grafx/api/platform.py
+-rw-r--r--   0        0        0     2232 2023-06-20 04:20:59.710105 chilitools-0.2.3/chilitools/grafx/auth.py
+-rw-r--r--   0        0        0     1999 2023-06-22 22:41:24.669863 chilitools-0.2.3/chilitools/grafx/connector.py
+-rw-r--r--   0        0        0     2099 2023-06-22 21:08:30.949881 chilitools-0.2.3/chilitools/grafx/document.py
+-rw-r--r--   0        0        0      662 2023-06-22 22:26:48.267393 chilitools-0.2.3/chilitools/grafx/environment.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257581 chilitools-0.2.3/chilitools/settings/__init__.py
+-rw-r--r--   0        0        0      199 2022-04-15 23:48:49.570757 chilitools-0.2.3/chilitools/settings/config.py
+-rw-r--r--   0        0        0    12468 2022-09-27 16:58:06.159255 chilitools-0.2.3/chilitools/utilities/ServerMigration.py
+-rw-r--r--   0        0        0        0 2022-04-15 01:52:44.257751 chilitools-0.2.3/chilitools/utilities/__init__.py
+-rw-r--r--   0        0        0     2104 2022-10-28 20:09:34.951802 chilitools-0.2.3/chilitools/utilities/backoffice.py
+-rw-r--r--   0        0        0      602 2022-04-15 23:48:53.626324 chilitools-0.2.3/chilitools/utilities/defaults.py
+-rw-r--r--   0        0        0     2069 2023-06-13 15:46:56.759605 chilitools-0.2.3/chilitools/utilities/document.py
+-rw-r--r--   0        0        0      897 2022-07-21 19:16:13.652722 chilitools-0.2.3/chilitools/utilities/errors.py
+-rw-r--r--   0        0        0     6022 2022-10-28 20:05:22.841538 chilitools-0.2.3/chilitools/utilities/file.py
+-rw-r--r--   0        0        0      807 2023-06-20 15:02:52.753030 chilitools-0.2.3/chilitools/utilities/logger.py
+-rw-r--r--   0        0        0      509 2022-06-29 19:01:07.878458 chilitools-0.2.3/chilitools/utilities/strings.py
+-rw-r--r--   0        0        0     3831 2023-03-21 15:07:48.139637 chilitools-0.2.3/chilitools/utilities/xmltools.py
+-rw-r--r--   0        0        0      505 2023-06-22 22:39:25.392049 chilitools-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 chilitools-0.2.3/PKG-INFO
```

### Comparing `chilitools-0.2.1/chilitools/__init__.py` & `chilitools-0.2.3/chilitools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.1'
+__version__ = '0.2.3'
 
 import pyperclip as pc
 from chilitools.utilities.backoffice import backofficeURLInput
 from chilitools.api.connector import ChiliConnector
 from chilitools.api.mycp import generateLoginTokenForURL, generateOAuthTokenFromCredentials, setUserType, deleteLoginFile
 from chilitools.utilities.defaults import STAFF_TYPE
```

### Comparing `chilitools-0.2.1/chilitools/api/connector.py` & `chilitools-0.2.3/chilitools/api/connector.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/api/endpoints.py` & `chilitools-0.2.3/chilitools/api/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,17 @@
       return False
     return True
 
   def get_name_if_exists(self, resourceType: str, itemID: str):
     res = self.ResourceItemGetDefinitionXML(resourceType, itemID)
     if res.statusCode == 404:
       return False
+    if resourceType.lower() == "fonts":
+      return res.content["item"]["@relativePath"].split("\\")[-1]
+
     return res.content["item"]["@name"]
 
   def getDownloadURL(self, resourceType: str, itemID: str, downloadType: str = "original", pageNum: int = 1) -> ChiliResponse:
     return f"{self.connector.baseURL}{self.connector.enviroment}/download.aspx?type={downloadType}&resourceName={resourceType}&id={itemID}&apiKey={self.connector.getAPIKey()}&pageNum={pageNum}"
 
   def getFullResourceTree(self, resourceType: str, folder: str = '') -> dict:
     items = dict()
```

### Comparing `chilitools-0.2.1/chilitools/api/mycp.py` & `chilitools-0.2.3/chilitools/api/mycp.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/api/response.py` & `chilitools-0.2.3/chilitools/api/response.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/grafx/auth.py` & `chilitools-0.2.3/chilitools/grafx/auth.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/grafx/connector.py` & `chilitools-0.2.3/chilitools/grafx/connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 import json
 from chilitools.grafx.auth import GraFxAuth
 from chilitools.grafx.environment import GraFxEnvironment
 from chilitools.grafx.api.environment import Templates
+from chilitools.grafx.api.platform import Platform
 
 
 #Todo(austin): Make some like exception handling thing where you just check_response(resp) and it throws for the usual 401 stuff, etc.
 
 # Gonna embrace the class madness I guess.
 class GraFxConnector:
     def __init__(self, environment: str, environment_type: str = "production", email: str = None, password: str = None, client_id: str = None, client_secret: str = None, logger = None, api_version: str = "1"):
@@ -14,19 +15,23 @@
         self.auth = GraFxAuth(email, password, client_id, client_secret)
         self.environment = GraFxEnvironment(
             environment_name=environment,
             environment_type=environment_type,
             api_version=api_version
         )
         self.logger = logger
-        self.templates = Templates(self) 
+        self.templates = Templates(self)
+        self.platform = Platform(self)
 
-    def make_request(self, method: str, endpoint: str, headers: dict = None, query_params: dict = None, body: dict = None):
+    def make_request(self, api: str, method: str, endpoint: str, headers: dict = None, query_params: dict = None, body: dict = None):
 
-        req_url = self.environment.base_url + endpoint
+        if api == "platform":
+            req_url = self.platform_base_url + endpoint
+        else:
+            req_url = self.environment.base_url + endpoint
 
         req_headers = {
             "content-type": "application/json",
             "Authorization": f"Bearer {self.auth.token}"
         }
 
         # If additional headers were supplied, merge them
```

### Comparing `chilitools-0.2.1/chilitools/grafx/document.py` & `chilitools-0.2.3/chilitools/grafx/document.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 import json
 
+class DocumentFont:
+    def __init__(self, id: str, name: str, family: str, style: str):
+        self.id = id
+        self.name = name
+        self.family = family
+        self.style = style
+
 class GraFxDocument:
     def __init__(self, doc: str, id: str = None, name: str = None):
         try:
             # We were passed a parsed JSON document
             if isinstance(doc, dict):
                 self.doc = doc
             # We were passed the raw JSON string of the document
@@ -31,11 +38,21 @@
                         image_frames.append(frame)
                     # Image is is a variable
                     if frame["src"].get("variableId"):
                         # Find and get the asset Id from the variable
                         for var in self.doc["variables"]:
                             if var.get("id") == frame["src"].get("variableId"):
                                 frame["src"]["assetId"] = var["src"]["assetId"]
+                                image_frames.append(frame)
       return image_frames
 
+    @property
+    def fonts(self):
+        fonts = []
+        for font in self.doc["styleKit"]["fonts"]:
+            #TODO(austin) Fix this when they break me
+            fonts.append(DocumentFont(font["fontId"], font["name"], font["fontFamily"], font["fontStyle"]))
+        return fonts
+
+
     def __str__(self): return json.dumps(self.doc)
     def __repr__(self): return self.doc
```

### Comparing `chilitools-0.2.1/chilitools/grafx/environment.py` & `chilitools-0.2.3/chilitools/grafx/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
         self.type = environment_type
         self.version = api_version
 
     @property
     def base_url(self):
         return f"https://{self.name}.{self._get_host()}.online/grafx/api/v{self.version}/environment/{self.name}"
 
+
     @property
     def publisher_url(self):
         return f"https://{self.name}.{self._get_host()}.online/{self.name}/interface.aspx"
 
     def _get_host(self):
         if self.type == "sandbox":
             return "chili-publish-sandbox"
```

### Comparing `chilitools-0.2.1/chilitools/utilities/ServerMigration.py` & `chilitools-0.2.3/chilitools/utilities/ServerMigration.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/utilities/backoffice.py` & `chilitools-0.2.3/chilitools/utilities/backoffice.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/utilities/defaults.py` & `chilitools-0.2.3/chilitools/utilities/defaults.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/utilities/document.py` & `chilitools-0.2.3/chilitools/utilities/document.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/utilities/errors.py` & `chilitools-0.2.3/chilitools/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/utilities/file.py` & `chilitools-0.2.3/chilitools/utilities/file.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/utilities/logger.py` & `chilitools-0.2.3/chilitools/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/chilitools/utilities/xmltools.py` & `chilitools-0.2.3/chilitools/utilities/xmltools.py`

 * *Files identical despite different names*

### Comparing `chilitools-0.2.1/PKG-INFO` & `chilitools-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chilitools
-Version: 0.2.1
+Version: 0.2.3
 Summary: A collection of tools for working with CHILI products
 Author: Austin
 Author-email: austin.meier@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

