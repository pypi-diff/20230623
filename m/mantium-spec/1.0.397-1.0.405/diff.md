# Comparing `tmp/mantium_spec-1.0.397.tar.gz` & `tmp/mantium_spec-1.0.405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantium_spec-1.0.397.tar", max compression
+gzip compressed data, was "mantium_spec-1.0.405.tar", max compression
```

## Comparing `mantium_spec-1.0.397.tar` & `mantium_spec-1.0.405.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     4957 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/README.md
--rw-r--r--   0        0        0     3182 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/__init__.py
--rw-r--r--   0        0        0      149 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/api/__init__.py
--rw-r--r--   0        0        0    22155 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/api/applications_api.py
--rw-r--r--   0        0        0    27708 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/api_client.py
--rw-r--r--   0        0        0    16324 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/configuration.py
--rw-r--r--   0        0        0     5056 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/exceptions.py
--rw-r--r--   0        0        0     2644 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/__init__.py
--rw-r--r--   0        0        0     8042 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/answer.py
--rw-r--r--   0        0        0     3647 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/answer_meta.py
--rw-r--r--   0        0        0     4604 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/application_credential.py
--rw-r--r--   0        0        0    11526 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/application_detail_response.py
--rw-r--r--   0        0        0     5447 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/application_query_request.py
--rw-r--r--   0        0        0     7110 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/application_query_response.py
--rw-r--r--   0        0        0     8424 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/application_response.py
--rw-r--r--   0        0        0     3160 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/application_status.py
--rw-r--r--   0        0        0    22875 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/chat_gpt_plugin_application_detail_response.py
--rw-r--r--   0        0        0     5758 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/content_creation_template_options.py
--rw-r--r--   0        0        0     3109 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/content_type.py
--rw-r--r--   0        0        0     3370 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/credential_type.py
--rw-r--r--   0        0        0     8288 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/custom_template_options.py
--rw-r--r--   0        0        0     5758 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/customer_support_template_options.py
--rw-r--r--   0        0        0     7156 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/datamodel_page_application_response.py
--rw-r--r--   0        0        0     6152 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/document.py
--rw-r--r--   0        0        0     3899 2023-06-22 19:52:22.000000 mantium_spec-1.0.397/mantium_spec/models/document_metadata.py
--rw-r--r--   0        0        0     5722 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/event_planning_template_options.py
--rw-r--r--   0        0        0     3689 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/http_validation_error.py
--rw-r--r--   0        0        0     5740 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/legal_documents_template_options.py
--rw-r--r--   0        0        0     2959 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/location_inner.py
--rw-r--r--   0        0        0     5686 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/meeting_info_template_options.py
--rw-r--r--   0        0        0     5976 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/personal_knowledge_management_template_options.py
--rw-r--r--   0        0        0     5848 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/product_documentation_template_options.py
--rw-r--r--   0        0        0     5776 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/recipe_management_template_options.py
--rw-r--r--   0        0        0    22115 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/response_get_application_detail.py
--rw-r--r--   0        0        0     5612 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/shopify_template_options.py
--rw-r--r--   0        0        0     4331 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/span.py
--rw-r--r--   0        0        0     7924 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/template.py
--rw-r--r--   0        0        0     5215 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/models/validation_error.py
--rw-r--r--   0        0        0    12585 2023-06-22 19:52:23.000000 mantium_spec-1.0.397/mantium_spec/rest.py
--rw-r--r--   0        0        0      368 2023-06-22 19:52:38.827779 mantium_spec-1.0.397/pyproject.toml
--rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 mantium_spec-1.0.397/setup.py
--rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 mantium_spec-1.0.397/PKG-INFO
+-rw-r--r--   0        0        0     4957 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/README.md
+-rw-r--r--   0        0        0     3182 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/__init__.py
+-rw-r--r--   0        0        0      149 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/api/__init__.py
+-rw-r--r--   0        0        0    22155 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/api/applications_api.py
+-rw-r--r--   0        0        0    27708 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/api_client.py
+-rw-r--r--   0        0        0    16324 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/configuration.py
+-rw-r--r--   0        0        0     5056 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/exceptions.py
+-rw-r--r--   0        0        0     2644 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/__init__.py
+-rw-r--r--   0        0        0     8042 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/answer.py
+-rw-r--r--   0        0        0     3647 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/answer_meta.py
+-rw-r--r--   0        0        0     4604 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/application_credential.py
+-rw-r--r--   0        0        0    11526 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/application_detail_response.py
+-rw-r--r--   0        0        0     5447 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/application_query_request.py
+-rw-r--r--   0        0        0     7110 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/application_query_response.py
+-rw-r--r--   0        0        0     8424 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/application_response.py
+-rw-r--r--   0        0        0     3160 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/application_status.py
+-rw-r--r--   0        0        0    22875 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/chat_gpt_plugin_application_detail_response.py
+-rw-r--r--   0        0        0     5758 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/content_creation_template_options.py
+-rw-r--r--   0        0        0     3109 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/content_type.py
+-rw-r--r--   0        0        0     3370 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/credential_type.py
+-rw-r--r--   0        0        0     8288 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/custom_template_options.py
+-rw-r--r--   0        0        0     5758 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/customer_support_template_options.py
+-rw-r--r--   0        0        0     7156 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/datamodel_page_application_response.py
+-rw-r--r--   0        0        0     6152 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/document.py
+-rw-r--r--   0        0        0     3899 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/document_metadata.py
+-rw-r--r--   0        0        0     5722 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/event_planning_template_options.py
+-rw-r--r--   0        0        0     3689 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/http_validation_error.py
+-rw-r--r--   0        0        0     5740 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/legal_documents_template_options.py
+-rw-r--r--   0        0        0     2959 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/location_inner.py
+-rw-r--r--   0        0        0     5686 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/meeting_info_template_options.py
+-rw-r--r--   0        0        0     5976 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/personal_knowledge_management_template_options.py
+-rw-r--r--   0        0        0     5848 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/product_documentation_template_options.py
+-rw-r--r--   0        0        0     5776 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/recipe_management_template_options.py
+-rw-r--r--   0        0        0    22115 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/response_get_application_detail.py
+-rw-r--r--   0        0        0     5612 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/shopify_template_options.py
+-rw-r--r--   0        0        0     4331 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/span.py
+-rw-r--r--   0        0        0     7924 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/template.py
+-rw-r--r--   0        0        0     5215 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/models/validation_error.py
+-rw-r--r--   0        0        0    12585 2023-06-23 20:41:58.000000 mantium_spec-1.0.405/mantium_spec/rest.py
+-rw-r--r--   0        0        0      368 2023-06-23 20:43:16.002443 mantium_spec-1.0.405/pyproject.toml
+-rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 mantium_spec-1.0.405/setup.py
+-rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 mantium_spec-1.0.405/PKG-INFO
```

### Comparing `mantium_spec-1.0.397/README.md` & `mantium_spec-1.0.405/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # mantium-spec
 Mantium API Documentation
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.397
+- API version: 1.0.405
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `mantium_spec-1.0.397/mantium_spec/__init__.py` & `mantium_spec-1.0.405/mantium_spec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 __version__ = "1.0.0"
```

### Comparing `mantium_spec-1.0.397/mantium_spec/api/applications_api.py` & `mantium_spec-1.0.405/mantium_spec/api/applications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `mantium_spec-1.0.397/mantium_spec/api_client.py` & `mantium_spec-1.0.405/mantium_spec/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
```

### Comparing `mantium_spec-1.0.397/mantium_spec/configuration.py` & `mantium_spec-1.0.405/mantium_spec/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -384,15 +384,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.397\n"\
+               "Version of the API: 1.0.405\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `mantium_spec-1.0.397/mantium_spec/exceptions.py` & `mantium_spec-1.0.405/mantium_spec/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/__init__.py` & `mantium_spec-1.0.405/mantium_spec/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/answer.py` & `mantium_spec-1.0.405/mantium_spec/models/answer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/answer_meta.py` & `mantium_spec-1.0.405/mantium_spec/models/answer_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/application_credential.py` & `mantium_spec-1.0.405/mantium_spec/models/application_credential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/application_detail_response.py` & `mantium_spec-1.0.405/mantium_spec/models/application_detail_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/application_query_request.py` & `mantium_spec-1.0.405/mantium_spec/models/application_query_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/application_query_response.py` & `mantium_spec-1.0.405/mantium_spec/models/application_query_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/application_response.py` & `mantium_spec-1.0.405/mantium_spec/models/application_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/application_status.py` & `mantium_spec-1.0.405/mantium_spec/models/application_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/chat_gpt_plugin_application_detail_response.py` & `mantium_spec-1.0.405/mantium_spec/models/chat_gpt_plugin_application_detail_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/content_creation_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/content_creation_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/content_type.py` & `mantium_spec-1.0.405/mantium_spec/models/content_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/credential_type.py` & `mantium_spec-1.0.405/mantium_spec/models/credential_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/custom_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/custom_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/customer_support_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/customer_support_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/datamodel_page_application_response.py` & `mantium_spec-1.0.405/mantium_spec/models/datamodel_page_application_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/document.py` & `mantium_spec-1.0.405/mantium_spec/models/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/document_metadata.py` & `mantium_spec-1.0.405/mantium_spec/models/document_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/event_planning_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/event_planning_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/http_validation_error.py` & `mantium_spec-1.0.405/mantium_spec/models/http_validation_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/legal_documents_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/legal_documents_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/location_inner.py` & `mantium_spec-1.0.405/mantium_spec/models/location_inner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/meeting_info_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/meeting_info_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/personal_knowledge_management_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/personal_knowledge_management_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/product_documentation_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/product_documentation_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/recipe_management_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/recipe_management_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/response_get_application_detail.py` & `mantium_spec-1.0.405/mantium_spec/models/response_get_application_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/shopify_template_options.py` & `mantium_spec-1.0.405/mantium_spec/models/shopify_template_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/span.py` & `mantium_spec-1.0.405/mantium_spec/models/span.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/template.py` & `mantium_spec-1.0.405/mantium_spec/models/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/models/validation_error.py` & `mantium_spec-1.0.405/mantium_spec/models/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.397/mantium_spec/rest.py` & `mantium_spec-1.0.405/mantium_spec/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.397
+    The version of the OpenAPI document: 1.0.405
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `mantium_spec-1.0.397/setup.py` & `mantium_spec-1.0.405/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['openapi-client>=1.1.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'mantium-spec',
-    'version': '1.0.397',
+    'version': '1.0.405',
     'description': 'OpenAPI-generated Python client',
-    'long_description': '# mantium-spec\nMantium API Documentation\n\nThis Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:\n\n- API version: 1.0.397\n- Package version: 1.0.0\n- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen\n\n## Requirements.\n\nPython 2.7 and 3.4+\n\n## Installation & Usage\n### pip install\n\nIf the python package is hosted on a repository, you can install directly using:\n\n```sh\npip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git\n```\n(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n### Setuptools\n\nInstall via [Setuptools](http://pypi.python.org/pypi/setuptools).\n\n```sh\npython setup.py install --user\n```\n(or `sudo python setup.py install` to install the package for all users)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n## Getting Started\n\nPlease follow the [installation procedure](#installation--usage) and then run the following:\n\n```python\nfrom __future__ import print_function\n\nimport time\nimport mantium_spec\nfrom mantium_spec.rest import ApiException\nfrom pprint import pprint\n\n# Defining the host is optional and defaults to http://localhost\n# See configuration.py for a list of all supported configuration parameters.\nconfiguration = mantium_spec.Configuration(\n    host = "http://localhost"\n)\n\n# The client must configure the authentication and authorization parameters\n# in accordance with the API server security policy.\n# Examples for each auth method are provided below, use the example that\n# satisfies your auth use case.\n\n# Configure Bearer authorization: HTTPBearer\nconfiguration = mantium_spec.Configuration(\n    access_token = \'YOUR_BEARER_TOKEN\'\n)\n\n\n# Enter a context with an instance of the API client\nwith mantium_spec.ApiClient(configuration) as api_client:\n    # Create an instance of the API class\n    api_instance = mantium_spec.ApplicationsApi(api_client)\n    application_id = \'application_id_example\' # str | \nbody = None # object |  (optional)\n\n    try:\n        # Get application detail.\n        api_response = api_instance.get_application_detail(application_id, body=body)\n        pprint(api_response)\n    except ApiException as e:\n        print("Exception when calling ApplicationsApi->get_application_detail: %s\\n" % e)\n    \n```\n\n## Documentation for API Endpoints\n\nAll URIs are relative to *http://localhost*\n\nClass | Method | HTTP request | Description\n------------ | ------------- | ------------- | -------------\n*ApplicationsApi* | [**get_application_detail**](docs/ApplicationsApi.md#get_application_detail) | **GET** /applications/{application_id} | Get application detail.\n*ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /applications/ | List applications.\n*ApplicationsApi* | [**query_application**](docs/ApplicationsApi.md#query_application) | **POST** /applications/{application_id}/query | Interact with an application.\n\n\n## Documentation For Models\n\n - [Answer](docs/Answer.md)\n - [AnswerMeta](docs/AnswerMeta.md)\n - [ApplicationCredential](docs/ApplicationCredential.md)\n - [ApplicationDetailResponse](docs/ApplicationDetailResponse.md)\n - [ApplicationQueryRequest](docs/ApplicationQueryRequest.md)\n - [ApplicationQueryResponse](docs/ApplicationQueryResponse.md)\n - [ApplicationResponse](docs/ApplicationResponse.md)\n - [ApplicationStatus](docs/ApplicationStatus.md)\n - [ChatGPTPluginApplicationDetailResponse](docs/ChatGPTPluginApplicationDetailResponse.md)\n - [ContentCreationTemplateOptions](docs/ContentCreationTemplateOptions.md)\n - [ContentType](docs/ContentType.md)\n - [CredentialType](docs/CredentialType.md)\n - [CustomTemplateOptions](docs/CustomTemplateOptions.md)\n - [CustomerSupportTemplateOptions](docs/CustomerSupportTemplateOptions.md)\n - [DatamodelPageApplicationResponse](docs/DatamodelPageApplicationResponse.md)\n - [Document](docs/Document.md)\n - [DocumentMetadata](docs/DocumentMetadata.md)\n - [EventPlanningTemplateOptions](docs/EventPlanningTemplateOptions.md)\n - [HTTPValidationError](docs/HTTPValidationError.md)\n - [LegalDocumentsTemplateOptions](docs/LegalDocumentsTemplateOptions.md)\n - [LocationInner](docs/LocationInner.md)\n - [MeetingInfoTemplateOptions](docs/MeetingInfoTemplateOptions.md)\n - [PersonalKnowledgeManagementTemplateOptions](docs/PersonalKnowledgeManagementTemplateOptions.md)\n - [ProductDocumentationTemplateOptions](docs/ProductDocumentationTemplateOptions.md)\n - [RecipeManagementTemplateOptions](docs/RecipeManagementTemplateOptions.md)\n - [ResponseGetApplicationDetail](docs/ResponseGetApplicationDetail.md)\n - [ShopifyTemplateOptions](docs/ShopifyTemplateOptions.md)\n - [Span](docs/Span.md)\n - [Template](docs/Template.md)\n - [ValidationError](docs/ValidationError.md)\n\n\n## Documentation For Authorization\n\n\n## HTTPBearer\n\n- **Type**: Bearer authentication\n\n\n## Author\n\n\n\n\n',
+    'long_description': '# mantium-spec\nMantium API Documentation\n\nThis Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:\n\n- API version: 1.0.405\n- Package version: 1.0.0\n- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen\n\n## Requirements.\n\nPython 2.7 and 3.4+\n\n## Installation & Usage\n### pip install\n\nIf the python package is hosted on a repository, you can install directly using:\n\n```sh\npip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git\n```\n(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n### Setuptools\n\nInstall via [Setuptools](http://pypi.python.org/pypi/setuptools).\n\n```sh\npython setup.py install --user\n```\n(or `sudo python setup.py install` to install the package for all users)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n## Getting Started\n\nPlease follow the [installation procedure](#installation--usage) and then run the following:\n\n```python\nfrom __future__ import print_function\n\nimport time\nimport mantium_spec\nfrom mantium_spec.rest import ApiException\nfrom pprint import pprint\n\n# Defining the host is optional and defaults to http://localhost\n# See configuration.py for a list of all supported configuration parameters.\nconfiguration = mantium_spec.Configuration(\n    host = "http://localhost"\n)\n\n# The client must configure the authentication and authorization parameters\n# in accordance with the API server security policy.\n# Examples for each auth method are provided below, use the example that\n# satisfies your auth use case.\n\n# Configure Bearer authorization: HTTPBearer\nconfiguration = mantium_spec.Configuration(\n    access_token = \'YOUR_BEARER_TOKEN\'\n)\n\n\n# Enter a context with an instance of the API client\nwith mantium_spec.ApiClient(configuration) as api_client:\n    # Create an instance of the API class\n    api_instance = mantium_spec.ApplicationsApi(api_client)\n    application_id = \'application_id_example\' # str | \nbody = None # object |  (optional)\n\n    try:\n        # Get application detail.\n        api_response = api_instance.get_application_detail(application_id, body=body)\n        pprint(api_response)\n    except ApiException as e:\n        print("Exception when calling ApplicationsApi->get_application_detail: %s\\n" % e)\n    \n```\n\n## Documentation for API Endpoints\n\nAll URIs are relative to *http://localhost*\n\nClass | Method | HTTP request | Description\n------------ | ------------- | ------------- | -------------\n*ApplicationsApi* | [**get_application_detail**](docs/ApplicationsApi.md#get_application_detail) | **GET** /applications/{application_id} | Get application detail.\n*ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /applications/ | List applications.\n*ApplicationsApi* | [**query_application**](docs/ApplicationsApi.md#query_application) | **POST** /applications/{application_id}/query | Interact with an application.\n\n\n## Documentation For Models\n\n - [Answer](docs/Answer.md)\n - [AnswerMeta](docs/AnswerMeta.md)\n - [ApplicationCredential](docs/ApplicationCredential.md)\n - [ApplicationDetailResponse](docs/ApplicationDetailResponse.md)\n - [ApplicationQueryRequest](docs/ApplicationQueryRequest.md)\n - [ApplicationQueryResponse](docs/ApplicationQueryResponse.md)\n - [ApplicationResponse](docs/ApplicationResponse.md)\n - [ApplicationStatus](docs/ApplicationStatus.md)\n - [ChatGPTPluginApplicationDetailResponse](docs/ChatGPTPluginApplicationDetailResponse.md)\n - [ContentCreationTemplateOptions](docs/ContentCreationTemplateOptions.md)\n - [ContentType](docs/ContentType.md)\n - [CredentialType](docs/CredentialType.md)\n - [CustomTemplateOptions](docs/CustomTemplateOptions.md)\n - [CustomerSupportTemplateOptions](docs/CustomerSupportTemplateOptions.md)\n - [DatamodelPageApplicationResponse](docs/DatamodelPageApplicationResponse.md)\n - [Document](docs/Document.md)\n - [DocumentMetadata](docs/DocumentMetadata.md)\n - [EventPlanningTemplateOptions](docs/EventPlanningTemplateOptions.md)\n - [HTTPValidationError](docs/HTTPValidationError.md)\n - [LegalDocumentsTemplateOptions](docs/LegalDocumentsTemplateOptions.md)\n - [LocationInner](docs/LocationInner.md)\n - [MeetingInfoTemplateOptions](docs/MeetingInfoTemplateOptions.md)\n - [PersonalKnowledgeManagementTemplateOptions](docs/PersonalKnowledgeManagementTemplateOptions.md)\n - [ProductDocumentationTemplateOptions](docs/ProductDocumentationTemplateOptions.md)\n - [RecipeManagementTemplateOptions](docs/RecipeManagementTemplateOptions.md)\n - [ResponseGetApplicationDetail](docs/ResponseGetApplicationDetail.md)\n - [ShopifyTemplateOptions](docs/ShopifyTemplateOptions.md)\n - [Span](docs/Span.md)\n - [Template](docs/Template.md)\n - [ValidationError](docs/ValidationError.md)\n\n\n## Documentation For Authorization\n\n\n## HTTPBearer\n\n- **Type**: Bearer authentication\n\n\n## Author\n\n\n\n\n',
     'author': 'Mantium',
     'author_email': 'support@mantiumai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mantium_spec-1.0.397/PKG-INFO` & `mantium_spec-1.0.405/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantium-spec
-Version: 1.0.397
+Version: 1.0.405
 Summary: OpenAPI-generated Python client
 Author: Mantium
 Author-email: support@mantiumai.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 
 # mantium-spec
 Mantium API Documentation
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.397
+- API version: 1.0.405
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

