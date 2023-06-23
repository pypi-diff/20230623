# Comparing `tmp/dj-jwt-auth-1.0.0.tar.gz` & `tmp/dj-jwt-auth-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-jwt-auth-1.0.0.tar", last modified: Mon Jun 19 09:03:45 2023, max compression
+gzip compressed data, was "dj-jwt-auth-1.0.1.tar", last modified: Fri Jun 23 16:11:14 2023, max compression
```

## Comparing `dj-jwt-auth-1.0.0.tar` & `dj-jwt-auth-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.184073 dj-jwt-auth-1.0.0/
--rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-06-19 09:03:45.184255 dj-jwt-auth-1.0.0/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) 1002642239     1779 2023-06-16 14:04:30.000000 dj-jwt-auth-1.0.0/README.md
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.175979 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/
--rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 seleznevk (984925890) 1002642239      409 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 seleznevk (984925890) 1002642239        1 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 seleznevk (984925890) 1002642239       63 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 seleznevk (984925890) 1002642239       17 2023-06-19 09:03:45.000000 dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/top_level.txt
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.180122 dj-jwt-auth-1.0.0/django_jwt/
--rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 11:25:09.000000 dj-jwt-auth-1.0.0/django_jwt/__init__.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     1092 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.0/django_jwt/middleware.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      981 2023-06-16 14:04:30.000000 dj-jwt-auth-1.0.0/django_jwt/settings.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     3064 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.0/django_jwt/user.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     1482 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.0/django_jwt/utils.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      200 2022-12-07 14:39:32.000000 dj-jwt-auth-1.0.0/django_jwt/views.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      221 2022-10-24 09:36:12.000000 dj-jwt-auth-1.0.0/pyproject.toml
--rw-r--r--   0 seleznevk (984925890) 1002642239      991 2023-06-19 09:03:45.185038 dj-jwt-auth-1.0.0/setup.cfg
--rw-r--r--   0 seleznevk (984925890) 1002642239       90 2022-10-24 09:36:32.000000 dj-jwt-auth-1.0.0/setup.py
-drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-19 09:03:45.183215 dj-jwt-auth-1.0.0/tests/
--rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 13:02:24.000000 dj-jwt-auth-1.0.0/tests/__init__.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      251 2023-06-19 08:33:20.000000 dj-jwt-auth-1.0.0/tests/models.py
--rw-r--r--   0 seleznevk (984925890) 1002642239     5139 2023-06-19 08:55:20.000000 dj-jwt-auth-1.0.0/tests/test.py
--rw-r--r--   0 seleznevk (984925890) 1002642239      212 2022-10-14 10:04:40.000000 dj-jwt-auth-1.0.0/tests/urls.py
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-23 16:11:14.206956 dj-jwt-auth-1.0.1/
+-rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-06-23 16:11:14.207231 dj-jwt-auth-1.0.1/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) 1002642239     1779 2023-06-16 14:04:30.000000 dj-jwt-auth-1.0.1/README.md
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-23 16:11:14.196572 dj-jwt-auth-1.0.1/dj_jwt_auth.egg-info/
+-rw-r--r--   0 seleznevk (984925890) 1002642239     2720 2023-06-23 16:11:14.000000 dj-jwt-auth-1.0.1/dj_jwt_auth.egg-info/PKG-INFO
+-rw-r--r--   0 seleznevk (984925890) 1002642239      409 2023-06-23 16:11:14.000000 dj-jwt-auth-1.0.1/dj_jwt_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 seleznevk (984925890) 1002642239        1 2023-06-23 16:11:14.000000 dj-jwt-auth-1.0.1/dj_jwt_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 seleznevk (984925890) 1002642239       63 2023-06-23 16:11:14.000000 dj-jwt-auth-1.0.1/dj_jwt_auth.egg-info/requires.txt
+-rw-r--r--   0 seleznevk (984925890) 1002642239       17 2023-06-23 16:11:14.000000 dj-jwt-auth-1.0.1/dj_jwt_auth.egg-info/top_level.txt
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-23 16:11:14.202337 dj-jwt-auth-1.0.1/django_jwt/
+-rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 11:25:09.000000 dj-jwt-auth-1.0.1/django_jwt/__init__.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     1092 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.1/django_jwt/middleware.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      981 2023-06-19 09:22:31.000000 dj-jwt-auth-1.0.1/django_jwt/settings.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     3420 2023-06-23 16:06:11.000000 dj-jwt-auth-1.0.1/django_jwt/user.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     1482 2023-06-19 08:56:53.000000 dj-jwt-auth-1.0.1/django_jwt/utils.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      200 2022-12-07 14:39:32.000000 dj-jwt-auth-1.0.1/django_jwt/views.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      221 2022-10-24 09:36:12.000000 dj-jwt-auth-1.0.1/pyproject.toml
+-rw-r--r--   0 seleznevk (984925890) 1002642239      991 2023-06-23 16:11:14.208535 dj-jwt-auth-1.0.1/setup.cfg
+-rw-r--r--   0 seleznevk (984925890) 1002642239       90 2022-10-24 09:36:32.000000 dj-jwt-auth-1.0.1/setup.py
+drwxr-xr-x   0 seleznevk (984925890) 1002642239        0 2023-06-23 16:11:14.206129 dj-jwt-auth-1.0.1/tests/
+-rw-r--r--   0 seleznevk (984925890) 1002642239        0 2022-10-13 13:02:24.000000 dj-jwt-auth-1.0.1/tests/__init__.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      251 2023-06-19 08:33:20.000000 dj-jwt-auth-1.0.1/tests/models.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239     5123 2023-06-23 16:01:33.000000 dj-jwt-auth-1.0.1/tests/test.py
+-rw-r--r--   0 seleznevk (984925890) 1002642239      212 2022-10-14 10:04:40.000000 dj-jwt-auth-1.0.1/tests/urls.py
```

### Comparing `dj-jwt-auth-1.0.0/PKG-INFO` & `dj-jwt-auth-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-jwt-auth-1.0.0/README.md` & `dj-jwt-auth-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.0.0/dj_jwt_auth.egg-info/PKG-INFO` & `dj-jwt-auth-1.0.1/dj_jwt_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-jwt-auth-1.0.0/django_jwt/middleware.py` & `dj-jwt-auth-1.0.1/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.0.0/django_jwt/settings.py` & `dj-jwt-auth-1.0.1/django_jwt/settings.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.0.0/django_jwt/user.py` & `dj-jwt-auth-1.0.1/django_jwt/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
+from datetime import datetime
+from logging import getLogger
+
 import pytz
-from dateutil import parser
 from django.contrib.auth import get_user_model
 from django.http.request import HttpRequest
 
 from django_jwt import settings
 from django_jwt.utils import oidc_handler
 
 utc = pytz.UTC
+log = getLogger(__name__)
 
 
 class UserHandler:
+    modified_at = None
+
     def __init__(self, payload: dict, request: HttpRequest, access_token: str):
         # payload of access token without user info
         # auth0_id should be available if auth0 added in Client Scopes in KeyCloak admin
         self.kwargs = settings.OIDC_USER_DEFAULTS.copy()
         self.kwargs[settings.OIDC_USER_UID] = payload.get("auth0_id", payload["sub"])
+
         modified_at = payload.get(settings.OIDC_TOKEN_MODIFIED_FIELD, None)
-        self.modified_at = utc.normalize(parser.parse(modified_at)) if modified_at else None
+        if modified_at and isinstance(modified_at, int):
+            self.modified_at = utc.localize(datetime.fromtimestamp(modified_at))
 
         self.on_create = settings.OIDC_USER_ON_CREATE
         self.on_update = settings.OIDC_USER_ON_UPDATE
         self.request = request
         self.access_token = access_token
 
     def _collect_user_data(self):
@@ -65,15 +72,22 @@
             except model.DoesNotExist:
                 # or just create new user
                 user = model.objects.create(**self.kwargs)
                 if self.on_create:
                     self.on_create(user, self.request)
                 return user
 
+        if not settings.OIDC_USER_UPDATE:
+            return user
+
         # update user fields if they are changed in KeyCloak
-        user_modified_at = getattr(user, settings.OIDC_USER_MODIFIED_FIELD)
+        user_modified_at = getattr(user, settings.OIDC_USER_MODIFIED_FIELD, None)
+        if not user_modified_at:
+            log.error("User model does not have field '%s'", settings.OIDC_USER_MODIFIED_FIELD)
+            return user
+
         if self.modified_at and utc.localize(user_modified_at) < self.modified_at:
             self._collect_user_data()
             self._update_user(user)
             if self.on_update:
                 self.on_update(user, self.request)
         return user
```

### Comparing `dj-jwt-auth-1.0.0/django_jwt/utils.py` & `dj-jwt-auth-1.0.1/django_jwt/utils.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.0.0/setup.cfg` & `dj-jwt-auth-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-jwt-auth
-version = 1.0.0
+version = 1.0.1
 description = A Django package for JSON Web Token validation and verification. Using PyJWT.
 long_description = file: README.md
 url = https://www.example.com/
 author = Konstantin Seleznev
 author_email = k.seleznev@elsevier.com
 license = MIT
 classifiers =
```

### Comparing `dj-jwt-auth-1.0.0/tests/test.py` & `dj-jwt-auth-1.0.1/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from django_jwt import settings
 from django_jwt.middleware import JWTAuthMiddleware
 
 access_token_payload = {
     "sub": "12345",
     "auth0_id": "1234",
-    "updated_at": "2050-01-01T00:00:00.000Z",
+    "updated_at": 2687276498,
 }
 user_info_payload = {
     "sub": "12345",
     "auth0_id": "1234",
     "email": "example@bk.com",
     "name": "UserName",
     "given_name": "1st name",
```

