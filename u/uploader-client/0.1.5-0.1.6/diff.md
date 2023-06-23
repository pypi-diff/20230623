# Comparing `tmp/uploader-client-0.1.5.tar.gz` & `tmp/uploader-client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploader-client-0.1.5.tar", last modified: Tue Jun 20 12:28:19 2023, max compression
+gzip compressed data, was "uploader-client-0.1.6.tar", last modified: Fri Jun 23 12:40:12 2023, max compression
```

## Comparing `uploader-client-0.1.5.tar` & `uploader-client-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.573946 uploader-client-0.1.5/
--rw-r--r--   0 root         (0) root         (0)      290 2023-01-23 10:33:53.000000 uploader-client-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2688 2023-06-20 12:28:19.572945 uploader-client-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1782 2023-03-20 10:09:04.000000 uploader-client-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.540946 uploader-client-0.1.5/requirements/
--rw-r--r--   0 root         (0) root         (0)       87 2023-01-23 10:33:53.000000 uploader-client-0.1.5/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-23 10:33:53.000000 uploader-client-0.1.5/requirements/prod.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 12:28:19.573946 uploader-client-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2427 2023-01-23 10:33:53.000000 uploader-client-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.534946 uploader-client-0.1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.548946 uploader-client-0.1.5/src/uploader_client/
--rw-r--r--   0 root         (0) root         (0)      658 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1151 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/adapters.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-03-20 10:09:04.000000 uploader-client-0.1.5/src/uploader_client/configurations.py
--rw-r--r--   0 root         (0) root         (0)      340 2023-03-20 10:09:04.000000 uploader-client-0.1.5/src/uploader_client/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.551946 uploader-client-0.1.5/src/uploader_client/contrib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.552945 uploader-client-0.1.5/src/uploader_client/contrib/rdm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/contrib/rdm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.557946 uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/configurations.py
--rw-r--r--   0 root         (0) root         (0)     3841 2023-06-20 12:28:06.000000 uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/rdm.json
--rw-r--r--   0 root         (0) root         (0)     2258 2023-03-20 10:09:04.000000 uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/rest.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/utils.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-03-21 07:37:04.000000 uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.564946 uploader-client-0.1.5/src/uploader_client/interfaces/
--rw-r--r--   0 root         (0) root         (0)      274 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/interfaces/base.py
--rw-r--r--   0 root         (0) root         (0)     6035 2023-03-20 10:09:04.000000 uploader-client-0.1.5/src/uploader_client/interfaces/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.569945 uploader-client-0.1.5/src/uploader_client/logging/
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/logging/base.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/logging/db.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/logging/stdlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.572945 uploader-client-0.1.5/src/uploader_client/migrations/
--rw-r--r--   0 root         (0) root         (0)     1194 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/models.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-01-23 10:33:53.000000 uploader-client-0.1.5/src/uploader_client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 12:28:19.551946 uploader-client-0.1.5/src/uploader_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2688 2023-06-20 12:28:19.000000 uploader-client-0.1.5/src/uploader_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1262 2023-06-20 12:28:19.000000 uploader-client-0.1.5/src/uploader_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-20 12:28:19.000000 uploader-client-0.1.5/src/uploader_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-20 12:28:19.000000 uploader-client-0.1.5/src/uploader_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-20 12:28:19.000000 uploader-client-0.1.5/src/uploader_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-20 12:28:19.000000 uploader-client-0.1.5/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.858312 uploader-client-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-01-23 10:33:53.000000 uploader-client-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-06-23 12:40:12.858312 uploader-client-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-03-20 10:09:04.000000 uploader-client-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.827312 uploader-client-0.1.6/requirements/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-01-23 10:33:53.000000 uploader-client-0.1.6/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-01-23 10:33:53.000000 uploader-client-0.1.6/requirements/prod.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 12:40:12.858312 uploader-client-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-01-23 10:33:53.000000 uploader-client-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.824312 uploader-client-0.1.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.836311 uploader-client-0.1.6/src/uploader_client/
+-rw-r--r--   0 root         (0) root         (0)      658 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/adapters.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-03-20 10:09:04.000000 uploader-client-0.1.6/src/uploader_client/configurations.py
+-rw-r--r--   0 root         (0) root         (0)      340 2023-03-20 10:09:04.000000 uploader-client-0.1.6/src/uploader_client/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.839311 uploader-client-0.1.6/src/uploader_client/contrib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.839311 uploader-client-0.1.6/src/uploader_client/contrib/rdm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/contrib/rdm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.843311 uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/configurations.py
+-rw-r--r--   0 root         (0) root         (0)     3825 2023-06-23 12:39:59.000000 uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/rdm.json
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-03-20 10:09:04.000000 uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/rest.py
+-rw-r--r--   0 root         (0) root         (0)      898 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-23 12:39:59.000000 uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.849311 uploader-client-0.1.6/src/uploader_client/interfaces/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/interfaces/base.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2023-03-20 10:09:04.000000 uploader-client-0.1.6/src/uploader_client/interfaces/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.854312 uploader-client-0.1.6/src/uploader_client/logging/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/logging/base.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/logging/db.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/logging/stdlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.857312 uploader-client-0.1.6/src/uploader_client/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/models.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-01-23 10:33:53.000000 uploader-client-0.1.6/src/uploader_client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:40:12.839311 uploader-client-0.1.6/src/uploader_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2688 2023-06-23 12:40:12.000000 uploader-client-0.1.6/src/uploader_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-06-23 12:40:12.000000 uploader-client-0.1.6/src/uploader_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-23 12:40:12.000000 uploader-client-0.1.6/src/uploader_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-23 12:40:12.000000 uploader-client-0.1.6/src/uploader_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 12:40:12.000000 uploader-client-0.1.6/src/uploader_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-23 12:40:12.000000 uploader-client-0.1.6/version.conf
```

### Comparing `uploader-client-0.1.5/PKG-INFO` & `uploader-client-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uploader-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Клиент для взаимодействия с Загрузчиком данных в витрину
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `uploader-client-0.1.5/README.md` & `uploader-client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/setup.py` & `uploader-client-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/__init__.py` & `uploader-client-0.1.6/src/uploader_client/__init__.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/adapters.py` & `uploader-client-0.1.6/src/uploader_client/adapters.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/configurations.py` & `uploader-client-0.1.6/src/uploader_client/configurations.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/configurations.py` & `uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/configurations.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/rdm.json` & `uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/rdm.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998914930555555%*

 * *Differences: {"'paths'": "{'/{version}/datamarts/{datamart_name}/tables/{table_name}/upload': {'post': "*

 * *            "{'requestBody': {'content': {replace: OrderedDict([('text/csv', "*

 * *            "OrderedDict([('schema', OrderedDict([('type', 'string')]))]))])}}}}}"}*

```diff
@@ -35,15 +35,15 @@
                         "schema": {
                             "type": "string"
                         }
                     }
                 ],
                 "requestBody": {
                     "content": {
-                        "application/octet-stream": {
+                        "text/csv": {
                             "schema": {
                                 "type": "string"
                             }
                         }
                     },
                     "required": true
                 },
```

### Comparing `uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/rest.py` & `uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/utils.py` & `uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/contrib/rdm/interfaces/validation.py` & `uploader-client-0.1.6/src/uploader_client/contrib/rdm/interfaces/validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     media_type_finder_cls = MediaTypeFinder
 
     def __init__(
         self, *args, custom_media_type_deserializers=None, **kwargs
     ):
         custom_media_type_deserializers: dict = custom_media_type_deserializers or {}
         custom_media_type_deserializers.update({
-            'application/octet-stream': utils.try_decode_csv,
+            'text/csv': utils.try_decode_csv,
             'multipart/form-data': utils.try_decode_multipart
         })
         super().__init__(
             *args, custom_media_type_deserializers=custom_media_type_deserializers
         )
 
     def _get_media_type(self, content, request_or_response):
```

### Comparing `uploader-client-0.1.5/src/uploader_client/interfaces/base.py` & `uploader-client-0.1.6/src/uploader_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/interfaces/rest.py` & `uploader-client-0.1.6/src/uploader_client/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/logging/base.py` & `uploader-client-0.1.6/src/uploader_client/logging/base.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/migrations/0001_initial.py` & `uploader-client-0.1.6/src/uploader_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/models.py` & `uploader-client-0.1.6/src/uploader_client/models.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client/utils.py` & `uploader-client-0.1.6/src/uploader_client/utils.py`

 * *Files identical despite different names*

### Comparing `uploader-client-0.1.5/src/uploader_client.egg-info/PKG-INFO` & `uploader-client-0.1.6/src/uploader_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uploader-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Клиент для взаимодействия с Загрузчиком данных в витрину
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `uploader-client-0.1.5/src/uploader_client.egg-info/SOURCES.txt` & `uploader-client-0.1.6/src/uploader_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

