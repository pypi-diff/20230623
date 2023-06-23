# Comparing `tmp/django-guardian-queryset-1.0.8.tar.gz` & `tmp/django-guardian-queryset-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-guardian-queryset-1.0.8.tar", last modified: Thu Jun  2 01:44:33 2022, max compression
+gzip compressed data, was "dist/django-guardian-queryset-1.0.9.tar", last modified: Fri Jun 10 21:39:22 2022, max compression
```

## Comparing `django-guardian-queryset-1.0.8.tar` & `django-guardian-queryset-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/
--rw-r--r--   0 Sam        (501) staff       (20)     1212 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/PKG-INFO
--rw-r--r--   0 Sam        (501) staff       (20)      274 2020-10-04 02:16:03.000000 django-guardian-queryset-1.0.8/README.md
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/
--rw-r--r--   0 Sam        (501) staff       (20)     1212 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/PKG-INFO
--rw-r--r--   0 Sam        (501) staff       (20)      626 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/SOURCES.txt
--rw-r--r--   0 Sam        (501) staff       (20)        1 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/dependency_links.txt
--rw-r--r--   0 Sam        (501) staff       (20)      106 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/requires.txt
--rw-r--r--   0 Sam        (501) staff       (20)       18 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/top_level.txt
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/guardian_queryset/
--rw-r--r--   0 Sam        (501) staff       (20)        0 2020-10-04 02:14:38.000000 django-guardian-queryset-1.0.8/guardian_queryset/__init__.py
--rw-r--r--   0 Sam        (501) staff       (20)     1460 2021-08-12 01:42:29.000000 django-guardian-queryset-1.0.8/guardian_queryset/admin.py
--rwxr-xr-x   0 Sam        (501) staff       (20)      108 2020-10-04 02:21:57.000000 django-guardian-queryset-1.0.8/guardian_queryset/apps.py
--rw-r--r--   0 Sam        (501) staff       (20)      362 2020-10-06 22:27:23.000000 django-guardian-queryset-1.0.8/guardian_queryset/decorators.py
--rw-r--r--   0 Sam        (501) staff       (20)      306 2020-10-06 22:22:48.000000 django-guardian-queryset-1.0.8/guardian_queryset/filters.py
--rw-r--r--   0 Sam        (501) staff       (20)      230 2020-10-05 21:28:31.000000 django-guardian-queryset-1.0.8/guardian_queryset/manager.py
-drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/guardian_queryset/migrations/
--rw-r--r--   0 Sam        (501) staff       (20)        0 2019-12-09 20:56:55.000000 django-guardian-queryset-1.0.8/guardian_queryset/migrations/__init__.py
--rw-r--r--   0 Sam        (501) staff       (20)     5278 2020-10-06 04:54:23.000000 django-guardian-queryset-1.0.8/guardian_queryset/models.py
--rw-r--r--   0 Sam        (501) staff       (20)     5331 2020-10-12 20:52:43.000000 django-guardian-queryset-1.0.8/guardian_queryset/queryset.py
--rw-r--r--   0 Sam        (501) staff       (20)     3330 2021-08-22 02:10:08.000000 django-guardian-queryset-1.0.8/guardian_queryset/serializers.py
--rw-r--r--   0 Sam        (501) staff       (20)     2766 2022-06-01 17:21:49.000000 django-guardian-queryset-1.0.8/guardian_queryset/utils.py
--rw-r--r--   0 Sam        (501) staff       (20)        0 2020-05-23 17:44:20.000000 django-guardian-queryset-1.0.8/guardian_queryset/views.py
--rw-r--r--   0 Sam        (501) staff       (20)      952 2022-06-02 01:44:33.000000 django-guardian-queryset-1.0.8/setup.cfg
--rw-r--r--   0 Sam        (501) staff       (20)       94 2020-10-04 00:37:39.000000 django-guardian-queryset-1.0.8/setup.py
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/
+-rw-r--r--   0 Sam        (501) staff       (20)     1212 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/PKG-INFO
+-rw-r--r--   0 Sam        (501) staff       (20)      274 2020-10-04 02:16:03.000000 django-guardian-queryset-1.0.9/README.md
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/
+-rw-r--r--   0 Sam        (501) staff       (20)     1212 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/PKG-INFO
+-rw-r--r--   0 Sam        (501) staff       (20)      626 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/SOURCES.txt
+-rw-r--r--   0 Sam        (501) staff       (20)        1 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/dependency_links.txt
+-rw-r--r--   0 Sam        (501) staff       (20)      106 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/requires.txt
+-rw-r--r--   0 Sam        (501) staff       (20)       18 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/top_level.txt
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/guardian_queryset/
+-rw-r--r--   0 Sam        (501) staff       (20)        0 2020-10-04 02:14:38.000000 django-guardian-queryset-1.0.9/guardian_queryset/__init__.py
+-rw-r--r--   0 Sam        (501) staff       (20)     1460 2021-08-12 01:42:29.000000 django-guardian-queryset-1.0.9/guardian_queryset/admin.py
+-rwxr-xr-x   0 Sam        (501) staff       (20)      108 2020-10-04 02:21:57.000000 django-guardian-queryset-1.0.9/guardian_queryset/apps.py
+-rw-r--r--   0 Sam        (501) staff       (20)      362 2020-10-06 22:27:23.000000 django-guardian-queryset-1.0.9/guardian_queryset/decorators.py
+-rw-r--r--   0 Sam        (501) staff       (20)      306 2020-10-06 22:22:48.000000 django-guardian-queryset-1.0.9/guardian_queryset/filters.py
+-rw-r--r--   0 Sam        (501) staff       (20)      230 2020-10-05 21:28:31.000000 django-guardian-queryset-1.0.9/guardian_queryset/manager.py
+drwxr-xr-x   0 Sam        (501) staff       (20)        0 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/guardian_queryset/migrations/
+-rw-r--r--   0 Sam        (501) staff       (20)        0 2019-12-09 20:56:55.000000 django-guardian-queryset-1.0.9/guardian_queryset/migrations/__init__.py
+-rw-r--r--   0 Sam        (501) staff       (20)     5278 2020-10-06 04:54:23.000000 django-guardian-queryset-1.0.9/guardian_queryset/models.py
+-rw-r--r--   0 Sam        (501) staff       (20)     5360 2022-06-05 01:58:31.000000 django-guardian-queryset-1.0.9/guardian_queryset/queryset.py
+-rw-r--r--   0 Sam        (501) staff       (20)     3330 2021-08-22 02:10:08.000000 django-guardian-queryset-1.0.9/guardian_queryset/serializers.py
+-rw-r--r--   0 Sam        (501) staff       (20)     2766 2022-06-01 17:21:49.000000 django-guardian-queryset-1.0.9/guardian_queryset/utils.py
+-rw-r--r--   0 Sam        (501) staff       (20)        0 2020-05-23 17:44:20.000000 django-guardian-queryset-1.0.9/guardian_queryset/views.py
+-rw-r--r--   0 Sam        (501) staff       (20)      952 2022-06-10 21:39:22.000000 django-guardian-queryset-1.0.9/setup.cfg
+-rw-r--r--   0 Sam        (501) staff       (20)       94 2020-10-04 00:37:39.000000 django-guardian-queryset-1.0.9/setup.py
```

### Comparing `django-guardian-queryset-1.0.8/PKG-INFO` & `django-guardian-queryset-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-guardian-queryset
-Version: 1.0.8
+Version: 1.0.9
 Summary: Protected querysets in Django
 Home-page: UNKNOWN
 License: MIT
 Description: # Django Global Requests
         
         Allows for global request objects in your django project
```

### Comparing `django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/PKG-INFO` & `django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-guardian-queryset
-Version: 1.0.8
+Version: 1.0.9
 Summary: Protected querysets in Django
 Home-page: UNKNOWN
 License: MIT
 Description: # Django Global Requests
         
         Allows for global request objects in your django project
```

### Comparing `django-guardian-queryset-1.0.8/django_guardian_queryset.egg-info/SOURCES.txt` & `django-guardian-queryset-1.0.9/django_guardian_queryset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-guardian-queryset-1.0.8/guardian_queryset/admin.py` & `django-guardian-queryset-1.0.9/guardian_queryset/admin.py`

 * *Files identical despite different names*

### Comparing `django-guardian-queryset-1.0.8/guardian_queryset/models.py` & `django-guardian-queryset-1.0.9/guardian_queryset/models.py`

 * *Files identical despite different names*

### Comparing `django-guardian-queryset-1.0.8/guardian_queryset/queryset.py` & `django-guardian-queryset-1.0.9/guardian_queryset/queryset.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,28 +43,29 @@
 
     def select_for_update(self, *args, **kwargs):
         obj = super().select_for_update(*args, **kwargs)
         obj.can_change()
         obj.force_validate_oper("view")
         return obj
 
-    def create(self, with_user=True, **kwargs):
+    def create(self, with_user=True, user=None, **kwargs):
+        user = user or self.user
         if with_user:
             obj = super().create(**{
-                'user': self.user,
+                'user': user,
                 **kwargs,
             })
         else:
             obj = super().create(**kwargs)
         try:
-            validate_foreign_keys(self.user, obj)
+            validate_foreign_keys(user, obj)
         except ValidationError as e:
             obj.delete()
             raise e
-        assign_default_permissions(self.user, obj)
+        assign_default_permissions(user, obj)
         return obj
 
 
     def _reset_validation(self):
         self._validated_opers = {
             "view": False,
             "change": False,
```

### Comparing `django-guardian-queryset-1.0.8/guardian_queryset/serializers.py` & `django-guardian-queryset-1.0.9/guardian_queryset/serializers.py`

 * *Files identical despite different names*

### Comparing `django-guardian-queryset-1.0.8/guardian_queryset/utils.py` & `django-guardian-queryset-1.0.9/guardian_queryset/utils.py`

 * *Files identical despite different names*

### Comparing `django-guardian-queryset-1.0.8/setup.cfg` & `django-guardian-queryset-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-guardian-queryset
-version = 1.0.8
+version = 1.0.9
 description = Protected querysets in Django
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

