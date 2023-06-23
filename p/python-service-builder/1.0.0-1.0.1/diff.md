# Comparing `tmp/python-service-builder-1.0.0.tar.gz` & `tmp/python-service-builder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-service-builder-1.0.0.tar", last modified: Wed Jun 21 15:43:50 2023, max compression
+gzip compressed data, was "python-service-builder-1.0.1.tar", last modified: Fri Jun 23 14:05:04 2023, max compression
```

## Comparing `python-service-builder-1.0.0.tar` & `python-service-builder-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3278 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2758 2023-06-20 19:07:05.000000 python-service-builder-1.0.0/README.md
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1180 2023-06-07 19:47:23.000000 python-service-builder-1.0.0/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/python_service_builder.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3278 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      453 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      328 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       18 2023-06-21 15:43:50.000000 python-service-builder-1.0.0/python_service_builder.egg-info/top_level.txt
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/service_framework/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3630 2023-06-20 15:29:24.000000 python-service-builder-1.0.0/service_framework/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3743 2023-06-15 20:04:02.000000 python-service-builder-1.0.0/service_framework/__init_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1687 2023-06-20 15:06:26.000000 python-service-builder-1.0.0/service_framework/list_services.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3941 2023-06-20 16:02:27.000000 python-service-builder-1.0.0/service_framework/service_builder.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    14358 2023-06-20 15:33:57.000000 python-service-builder-1.0.0/service_framework/services.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1270 2023-06-20 15:45:57.000000 python-service-builder-1.0.0/service_framework/services_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-21 15:43:50.512979 python-service-builder-1.0.0/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-23 14:05:04.445899 python-service-builder-1.0.1/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3278 2023-06-23 14:05:04.445899 python-service-builder-1.0.1/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2758 2023-06-20 19:07:05.000000 python-service-builder-1.0.1/README.md
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1180 2023-06-23 13:57:56.000000 python-service-builder-1.0.1/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-23 14:05:04.445899 python-service-builder-1.0.1/python_service_builder.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3278 2023-06-23 14:05:04.000000 python-service-builder-1.0.1/python_service_builder.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      453 2023-06-23 14:05:04.000000 python-service-builder-1.0.1/python_service_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-23 14:05:04.000000 python-service-builder-1.0.1/python_service_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      328 2023-06-23 14:05:04.000000 python-service-builder-1.0.1/python_service_builder.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       18 2023-06-23 14:05:04.000000 python-service-builder-1.0.1/python_service_builder.egg-info/top_level.txt
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-23 14:05:04.445899 python-service-builder-1.0.1/service_framework/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3630 2023-06-20 15:29:24.000000 python-service-builder-1.0.1/service_framework/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3743 2023-06-15 20:04:02.000000 python-service-builder-1.0.1/service_framework/__init_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1687 2023-06-20 15:06:26.000000 python-service-builder-1.0.1/service_framework/list_services.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     3468 2023-06-23 13:56:51.000000 python-service-builder-1.0.1/service_framework/service_builder.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)    14358 2023-06-20 15:33:57.000000 python-service-builder-1.0.1/service_framework/services.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1270 2023-06-20 15:45:57.000000 python-service-builder-1.0.1/service_framework/services_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-23 14:05:04.445899 python-service-builder-1.0.1/setup.cfg
```

### Comparing `python-service-builder-1.0.0/PKG-INFO` & `python-service-builder-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-service-builder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper library for easier creation of Google services.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/google/python-service-builder
 Project-URL: Bug Tracker, https://github.com/google/python-service-builder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-service-builder-1.0.0/README.md` & `python-service-builder-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-service-builder-1.0.0/pyproject.toml` & `python-service-builder-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "python-service-builder"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "David Harcombe", email = "david.harcombe@gmail.com" }]
 description = "Helper library for easier creation of Google services."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
  "Programming Language :: Python :: 3",
  "Operating System :: OS Independent",
```

### Comparing `python-service-builder-1.0.0/python_service_builder.egg-info/PKG-INFO` & `python-service-builder-1.0.1/python_service_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-service-builder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helper library for easier creation of Google services.
 Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/google/python-service-builder
 Project-URL: Bug Tracker, https://github.com/google/python-service-builder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `python-service-builder-1.0.0/service_framework/__init__.py` & `python-service-builder-1.0.1/service_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `python-service-builder-1.0.0/service_framework/__init_test.py` & `python-service-builder-1.0.1/service_framework/__init_test.py`

 * *Files identical despite different names*

### Comparing `python-service-builder-1.0.0/service_framework/list_services.py` & `python-service-builder-1.0.1/service_framework/list_services.py`

 * *Files identical despite different names*

### Comparing `python-service-builder-1.0.0/service_framework/service_builder.py` & `python-service-builder-1.0.1/service_framework/service_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 import dataclasses_json
 import google_auth_httplib2
 from apiclient import discovery
 from google.auth import exceptions
 from google.oauth2 import credentials as oauth
 from httplib2 import Http
 from oauth2client import service_account
+from oauth2client import client
 
 from service_framework.services import Service
 from service_framework import snake_field
 
 
-@dataclasses_json.dataclass_json
+@dataclasses_json.dataclass_json(undefined=dataclasses_json.Undefined.EXCLUDE)
 @dataclasses.dataclass
 class OAuthKey(object):
   """Dataclass from the json key.
 
   NOTE: This is by no means the entire key; just the fields neccessary for OAuth.
   """
   access_token: Optional[str] = snake_field(field_name='token')
@@ -71,59 +72,40 @@
   definition = service.definition
 
   if isinstance(key, OAuthKey):
     kwargs = key.to_dict()
     if extra_scopes:
       kwargs['scopes'] = extra_scopes
 
-    try:
-      credentials = oauth.Credentials(**kwargs)
-      https = google_auth_httplib2.AuthorizedHttp(credentials)
-
-    except KeyError:
-      logging.exception(
-          'Invalid credentials received: missing a part of the credentials')
-      raise
-
-    except exceptions.RefreshError as error:
-      logging.exception('Invalid credentials received')
-      raise
+    credentials = oauth.Credentials(**kwargs)
 
   elif isinstance(key, oauth.Credentials):
     credentials = key
-    https = google_auth_httplib2.AuthorizedHttp(credentials)
 
   elif isinstance(key, str):
     kwargs = {
         'filename': key,
     }
     if extra_scopes:
       kwargs['scopes'] = extra_scopes
 
-    credentials = \
-        service_account.ServiceAccountCredentials.from_json_keyfile_name(
-            **kwargs)
-    https = credentials.authorize(Http())
+    credentials = oauth.Credentials.from_authorized_user_file(**kwargs)
 
   elif isinstance(key, Mapping):
-    kwargs = {
-        'keyfile_dict': key,
-    }
+    kwargs = OAuthKey(**key).to_dict()
 
     if extra_scopes:
       kwargs['scopes'] = extra_scopes
 
-    credentials = \
-        service_account.ServiceAccountCredentials.from_json_keyfile_dict(
-            key, scopes=extra_scopes)
-    https = credentials.authorize(Http())
+    credentials = oauth.Credentials(**kwargs)
 
   else:
     raise Exception('No valid credentials provided.')
 
+  https = google_auth_httplib2.AuthorizedHttp(credentials)
   discovery_args = {
       'http': https,
       'developerKey': api_key,
       'cache_discovery': False,
       **definition.to_dict()
   }
```

### Comparing `python-service-builder-1.0.0/service_framework/services.py` & `python-service-builder-1.0.1/service_framework/services.py`

 * *Files identical despite different names*

### Comparing `python-service-builder-1.0.0/service_framework/services_test.py` & `python-service-builder-1.0.1/service_framework/services_test.py`

 * *Files identical despite different names*

