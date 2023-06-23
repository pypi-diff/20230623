# Comparing `tmp/salesforce-tools-0.1.8.tar.gz` & `tmp/salesforce-tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-tools-0.1.8.tar", max compression
+gzip compressed data, was "salesforce-tools-0.1.9.tar", max compression
```

## Comparing `salesforce-tools-0.1.8.tar` & `salesforce-tools-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      821 2022-09-25 00:36:26.412070 salesforce-tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      548 2022-09-05 02:32:41.928723 salesforce-tools-0.1.8/salesforce_tools/__init__.py
--rw-r--r--   0        0        0     6460 2022-09-06 00:27:08.955178 salesforce-tools-0.1.8/salesforce_tools/auth.py
--rw-r--r--   0        0        0     6280 2022-09-03 22:52:28.858802 salesforce-tools-0.1.8/salesforce_tools/bulk.py
--rw-r--r--   0        0        0     5879 2022-09-05 02:34:33.026876 salesforce-tools-0.1.8/salesforce_tools/bulk_models.py
--rw-r--r--   0        0        0     1519 2022-08-28 19:09:24.339050 salesforce-tools-0.1.8/salesforce_tools/oauth_server.py
--rw-r--r--   0        0        0    81520 2022-09-25 00:35:32.399290 salesforce-tools-0.1.8/salesforce_tools/salesforce.py
--rw-r--r--   0        0        0     1511 2022-09-03 22:40:31.857193 salesforce-tools-0.1.8/salesforce_tools/util.py
--rw-r--r--   0        0        0      895 2022-09-25 00:40:47.998514 salesforce-tools-0.1.8/setup.py
--rw-r--r--   0        0        0      844 2022-09-25 00:40:47.998679 salesforce-tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      821 2022-09-25 00:51:07.339524 salesforce-tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      545 2022-09-25 00:50:43.720137 salesforce-tools-0.1.9/salesforce_tools/__init__.py
+-rw-r--r--   0        0        0     6460 2022-09-06 00:27:08.955178 salesforce-tools-0.1.9/salesforce_tools/auth.py
+-rw-r--r--   0        0        0     6280 2022-09-03 22:52:28.858802 salesforce-tools-0.1.9/salesforce_tools/bulk.py
+-rw-r--r--   0        0        0     5879 2022-09-05 02:34:33.026876 salesforce-tools-0.1.9/salesforce_tools/bulk_models.py
+-rw-r--r--   0        0        0     1519 2022-08-28 19:09:24.339050 salesforce-tools-0.1.9/salesforce_tools/oauth_server.py
+-rw-r--r--   0        0        0    81520 2022-09-25 00:35:32.399290 salesforce-tools-0.1.9/salesforce_tools/salesforce.py
+-rw-r--r--   0        0        0     1511 2022-09-03 22:40:31.857193 salesforce-tools-0.1.9/salesforce_tools/util.py
+-rw-r--r--   0        0        0      895 2022-09-25 00:51:17.260267 salesforce-tools-0.1.9/setup.py
+-rw-r--r--   0        0        0      844 2022-09-25 00:51:17.260443 salesforce-tools-0.1.9/PKG-INFO
```

### Comparing `salesforce-tools-0.1.8/pyproject.toml` & `salesforce-tools-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salesforce-tools"
-version = "0.1.8"
+version = "0.1.9"
 description = "Salesforce API tools"
 authors = ["David Manuel <david@dcmanjr.com>"]
 license = "MIT"
 homepage = "https://github.com/dacmanj/salesforce-tools"
 repository = "https://github.com/dacmanj/salesforce-tools"
 
 [tool.poetry.dependencies]
```

### Comparing `salesforce-tools-0.1.8/salesforce_tools/__init__.py` & `salesforce-tools-0.1.9/salesforce_tools/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-from salesforce_tools.salesforce import SalesforceAPI, SalesforceModelFactory, SalesforceServicesData
+from salesforce_tools.salesforce import SalesforceAPI, SalesforceModelFactory, RestAPI, ToolingAPI
 from salesforce_tools.auth import login, SalesforceOAuthClient, SalesforceJWTClient
 from salesforce_tools.bulk import SalesforceBulkAPI, SalesforceBulkJobException
 from salesforce_tools.bulk_models import JobInfo, JobInfoList, JobTypeEnum, JobStateEnum, OperationEnum, ContentTypeEnum
 from salesforce_tools.oauth_server import CallbackServer, OAuthCallbackHandler
 from salesforce_tools.util import SFDateTime, EmailValidator, EMAIL_ADDRESS_REGEX
```

### Comparing `salesforce-tools-0.1.8/salesforce_tools/auth.py` & `salesforce-tools-0.1.9/salesforce_tools/auth.py`

 * *Files identical despite different names*

### Comparing `salesforce-tools-0.1.8/salesforce_tools/bulk.py` & `salesforce-tools-0.1.9/salesforce_tools/bulk.py`

 * *Files identical despite different names*

### Comparing `salesforce-tools-0.1.8/salesforce_tools/bulk_models.py` & `salesforce-tools-0.1.9/salesforce_tools/bulk_models.py`

 * *Files identical despite different names*

### Comparing `salesforce-tools-0.1.8/salesforce_tools/oauth_server.py` & `salesforce-tools-0.1.9/salesforce_tools/oauth_server.py`

 * *Files identical despite different names*

### Comparing `salesforce-tools-0.1.8/salesforce_tools/salesforce.py` & `salesforce-tools-0.1.9/salesforce_tools/salesforce.py`

 * *Files identical despite different names*

### Comparing `salesforce-tools-0.1.8/salesforce_tools/util.py` & `salesforce-tools-0.1.9/salesforce_tools/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-tools-0.1.8/setup.py` & `salesforce-tools-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pydantic>=1.9.2,<2.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'salesforce-tools',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Salesforce API tools',
     'long_description': None,
     'author': 'David Manuel',
     'author_email': 'david@dcmanjr.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/dacmanj/salesforce-tools',
```

### Comparing `salesforce-tools-0.1.8/PKG-INFO` & `salesforce-tools-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Salesforce API tools
 Home-page: https://github.com/dacmanj/salesforce-tools
 License: MIT
 Author: David Manuel
 Author-email: david@dcmanjr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

