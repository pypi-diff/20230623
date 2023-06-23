# Comparing `tmp/django-sso-client-0.0.7.tar.gz` & `tmp/django-sso-client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-0.0.7.tar", last modified: Wed Jun  7 13:18:50 2023, max compression
+gzip compressed data, was "django-sso-client-0.0.8.tar", last modified: Fri Jun 23 20:06:18 2023, max compression
```

## Comparing `django-sso-client-0.0.7.tar` & `django-sso-client-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-07 13:18:50.408554 django-sso-client-0.0.7/
--rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.7/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      958 2023-06-07 13:18:50.408554 django-sso-client-0.0.7/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)     1663 2023-06-07 13:14:46.000000 django-sso-client-0.0.7/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-07 13:18:50.408554 django-sso-client-0.0.7/django_client_sso/
--rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.7/django_client_sso/__init__.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1741 2023-06-02 19:03:13.000000 django-sso-client-0.0.7/django_client_sso/client_base.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      386 2023-06-07 13:12:36.000000 django-sso-client-0.0.7/django_client_sso/client_office365.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1592 2023-06-02 19:32:28.000000 django-sso-client-0.0.7/django_client_sso/decorators.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      361 2023-06-02 19:33:03.000000 django-sso-client-0.0.7/django_client_sso/exceptions.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      700 2023-06-02 19:35:23.000000 django-sso-client-0.0.7/django_client_sso/handlers.py
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-07 13:18:50.408554 django-sso-client-0.0.7/django_sso_client.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      958 2023-06-07 13:18:50.000000 django-sso-client-0.0.7/django_sso_client.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      399 2023-06-07 13:18:50.000000 django-sso-client-0.0.7/django_sso_client.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-07 13:18:50.000000 django-sso-client-0.0.7/django_sso_client.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-07 13:18:50.000000 django-sso-client-0.0.7/django_sso_client.egg-info/top_level.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-07 13:18:50.408554 django-sso-client-0.0.7/setup.cfg
--rw-rw-r--   0 israel    (1000) israel    (1000)     1076 2023-06-07 13:12:57.000000 django-sso-client-0.0.7/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.8/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      958 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1663 2023-06-07 13:14:46.000000 django-sso-client-0.0.8/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/django_client_sso/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.8/django_client_sso/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1741 2023-06-02 19:03:13.000000 django-sso-client-0.0.8/django_client_sso/client_base.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      386 2023-06-07 13:12:36.000000 django-sso-client-0.0.8/django_client_sso/client_office365.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     2356 2023-06-23 20:05:23.000000 django-sso-client-0.0.8/django_client_sso/decorators.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      361 2023-06-02 19:33:03.000000 django-sso-client-0.0.8/django_client_sso/exceptions.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      700 2023-06-02 19:35:23.000000 django-sso-client-0.0.8/django_client_sso/handlers.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/django_sso_client.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)      958 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      399 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/top_level.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/setup.cfg
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1076 2023-06-23 20:05:45.000000 django-sso-client-0.0.8/setup.py
```

### Comparing `django-sso-client-0.0.7/PKG-INFO` & `django-sso-client-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/DJANGO_CLIENT
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.7/README.md` & `django-sso-client-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.7/django_client_sso/client_base.py` & `django-sso-client-0.0.8/django_client_sso/client_base.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.7/django_client_sso/decorators.py` & `django-sso-client-0.0.8/django_client_sso/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,40 @@
             raise Exception403()
     
         return wrapper
 
     return decorator_func
 
 
+def validator_with_args_kwargs(permissions):
+    def decorator_func(func):
+        @wraps(func)
+        def wrapper(self, request, *args, **kwargs):
+            client = ClientBase()
+            token = request.META.get('HTTP_AUTHORIZATION')
+            
+            if not token:
+                raise Exception401()
+            
+            token = token.replace('Bearer ', '')
+            token_decode = client.decode_token(token)
+            
+            required = str(permissions).split()
+            scope = token_decode['scope']
+
+            for r in required:
+                if r in scope:
+                    return func(self,request, *args, **kwargs)
+           
+            raise Exception403()
+    
+        return wrapper
+
+    return decorator_func
+
 def validator_without_request(permissions):
     def decorator_func(func):
         @wraps(func)
         def wrapper(self):
             client = ClientBase()
             token = self.request.META.get('HTTP_AUTHORIZATION')
```

### Comparing `django-sso-client-0.0.7/django_client_sso/handlers.py` & `django-sso-client-0.0.8/django_client_sso/handlers.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.7/django_sso_client.egg-info/PKG-INFO` & `django-sso-client-0.0.8/django_sso_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Client for Django Apps - SSO TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/DJANGO_CLIENT
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
```

### Comparing `django-sso-client-0.0.7/setup.py` & `django-sso-client-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-sso-client',
-    version='0.0.7',
+    version='0.0.8',
     author='TIT CS',
     author_email='contato@titcs.com.br',
     packages=['django_client_sso'],
     description='Client for Django Apps - SSO TIT/Hyper by P&D',
     long_description='Client for Django Apps - SSO TIT/Hyper by P&D',
     url='https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/DJANGO_CLIENT',
     project_urls={
```

