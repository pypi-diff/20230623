# Comparing `tmp/django-splint-kovs-0.0.9.1.tar.gz` & `tmp/django-splint-kovs-0.0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-splint-kovs-0.0.9.1.tar", last modified: Wed May 25 15:56:13 2022, max compression
+gzip compressed data, was "django-splint-kovs-0.0.9.2.tar", last modified: Wed May 25 16:40:48 2022, max compression
```

## Comparing `django-splint-kovs-0.0.9.1.tar` & `django-splint-kovs-0.0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 15:56:13.730458 django-splint-kovs-0.0.9.1/
--rw-r--r--   0 fialho     (502) staff       (20)     1073 2022-03-13 20:29:51.000000 django-splint-kovs-0.0.9.1/LICENSE
--rw-r--r--   0 fialho     (502) staff       (20)     4548 2022-05-25 15:56:13.730832 django-splint-kovs-0.0.9.1/PKG-INFO
--rw-r--r--   0 fialho     (502) staff       (20)     4114 2022-05-25 13:48:52.000000 django-splint-kovs-0.0.9.1/README.md
--rw-r--r--   0 fialho     (502) staff       (20)      232 2022-05-25 14:13:34.000000 django-splint-kovs-0.0.9.1/pyproject.toml
--rw-r--r--   0 fialho     (502) staff       (20)      690 2022-05-25 15:56:13.731509 django-splint-kovs-0.0.9.1/setup.cfg
-drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 15:56:13.648300 django-splint-kovs-0.0.9.1/src/
-drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 15:56:13.688559 django-splint-kovs-0.0.9.1/src/django_splint/
--rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 19:04:24.000000 django-splint-kovs-0.0.9.1/src/django_splint/__init__.py
--rw-r--r--   0 fialho     (502) staff       (20)     4073 2022-03-28 03:55:31.000000 django-splint-kovs-0.0.9.1/src/django_splint/admin.py
-drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 15:56:13.708261 django-splint-kovs-0.0.9.1/src/django_splint/api/
--rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 20:17:48.000000 django-splint-kovs-0.0.9.1/src/django_splint/api/__init__.py
--rw-r--r--   0 fialho     (502) staff       (20)      433 2022-03-13 19:46:53.000000 django-splint-kovs-0.0.9.1/src/django_splint/api/authentication.py
--rw-r--r--   0 fialho     (502) staff       (20)     1261 2022-05-25 14:11:58.000000 django-splint-kovs-0.0.9.1/src/django_splint/api/filters.py
--rw-r--r--   0 fialho     (502) staff       (20)     1215 2022-05-25 14:54:32.000000 django-splint-kovs-0.0.9.1/src/django_splint/api/permissions.py
--rw-r--r--   0 fialho     (502) staff       (20)     3957 2022-05-25 15:55:37.000000 django-splint-kovs-0.0.9.1/src/django_splint/api/serializers.py
--rw-r--r--   0 fialho     (502) staff       (20)     2036 2022-03-31 16:48:20.000000 django-splint-kovs-0.0.9.1/src/django_splint/api/views.py
-drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 15:56:13.713831 django-splint-kovs-0.0.9.1/src/django_splint/db/
--rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 20:17:57.000000 django-splint-kovs-0.0.9.1/src/django_splint/db/__init__.py
--rw-r--r--   0 fialho     (502) staff       (20)     3039 2022-05-25 15:55:39.000000 django-splint-kovs-0.0.9.1/src/django_splint/db/fields.py
--rw-r--r--   0 fialho     (502) staff       (20)     5558 2022-05-24 15:58:07.000000 django-splint-kovs-0.0.9.1/src/django_splint/db/models.py
-drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 15:56:13.720862 django-splint-kovs-0.0.9.1/src/django_splint/utils/
--rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 20:13:52.000000 django-splint-kovs-0.0.9.1/src/django_splint/utils/__init__.py
--rw-r--r--   0 fialho     (502) staff       (20)     4120 2022-03-31 16:48:20.000000 django-splint-kovs-0.0.9.1/src/django_splint/utils/decorators.py
-drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 15:56:13.729740 django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/
--rw-r--r--   0 fialho     (502) staff       (20)     4548 2022-05-25 15:56:12.000000 django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/PKG-INFO
--rw-r--r--   0 fialho     (502) staff       (20)      709 2022-05-25 15:56:13.000000 django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/SOURCES.txt
--rw-r--r--   0 fialho     (502) staff       (20)        1 2022-05-25 15:56:13.000000 django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/dependency_links.txt
--rw-r--r--   0 fialho     (502) staff       (20)      106 2022-05-25 15:56:13.000000 django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/requires.txt
--rw-r--r--   0 fialho     (502) staff       (20)       14 2022-05-25 15:56:13.000000 django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/top_level.txt
+drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 16:40:48.216297 django-splint-kovs-0.0.9.2/
+-rw-r--r--   0 fialho     (502) staff       (20)     1073 2022-03-13 20:29:51.000000 django-splint-kovs-0.0.9.2/LICENSE
+-rw-r--r--   0 fialho     (502) staff       (20)     4548 2022-05-25 16:40:48.217088 django-splint-kovs-0.0.9.2/PKG-INFO
+-rw-r--r--   0 fialho     (502) staff       (20)     4114 2022-05-25 13:48:52.000000 django-splint-kovs-0.0.9.2/README.md
+-rw-r--r--   0 fialho     (502) staff       (20)      232 2022-05-25 14:13:34.000000 django-splint-kovs-0.0.9.2/pyproject.toml
+-rw-r--r--   0 fialho     (502) staff       (20)      690 2022-05-25 16:40:48.218851 django-splint-kovs-0.0.9.2/setup.cfg
+drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 16:40:48.118386 django-splint-kovs-0.0.9.2/src/
+drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 16:40:48.149261 django-splint-kovs-0.0.9.2/src/django_splint/
+-rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 19:04:24.000000 django-splint-kovs-0.0.9.2/src/django_splint/__init__.py
+-rw-r--r--   0 fialho     (502) staff       (20)     4087 2022-05-25 16:39:12.000000 django-splint-kovs-0.0.9.2/src/django_splint/admin.py
+drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 16:40:48.180540 django-splint-kovs-0.0.9.2/src/django_splint/api/
+-rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 20:17:48.000000 django-splint-kovs-0.0.9.2/src/django_splint/api/__init__.py
+-rw-r--r--   0 fialho     (502) staff       (20)      433 2022-03-13 19:46:53.000000 django-splint-kovs-0.0.9.2/src/django_splint/api/authentication.py
+-rw-r--r--   0 fialho     (502) staff       (20)     1261 2022-05-25 14:11:58.000000 django-splint-kovs-0.0.9.2/src/django_splint/api/filters.py
+-rw-r--r--   0 fialho     (502) staff       (20)     1215 2022-05-25 14:54:32.000000 django-splint-kovs-0.0.9.2/src/django_splint/api/permissions.py
+-rw-r--r--   0 fialho     (502) staff       (20)     3957 2022-05-25 15:55:37.000000 django-splint-kovs-0.0.9.2/src/django_splint/api/serializers.py
+-rw-r--r--   0 fialho     (502) staff       (20)     2036 2022-03-31 16:48:20.000000 django-splint-kovs-0.0.9.2/src/django_splint/api/views.py
+drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 16:40:48.185098 django-splint-kovs-0.0.9.2/src/django_splint/db/
+-rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 20:17:57.000000 django-splint-kovs-0.0.9.2/src/django_splint/db/__init__.py
+-rw-r--r--   0 fialho     (502) staff       (20)     3039 2022-05-25 15:55:39.000000 django-splint-kovs-0.0.9.2/src/django_splint/db/fields.py
+-rw-r--r--   0 fialho     (502) staff       (20)     5558 2022-05-24 15:58:07.000000 django-splint-kovs-0.0.9.2/src/django_splint/db/models.py
+drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 16:40:48.196914 django-splint-kovs-0.0.9.2/src/django_splint/utils/
+-rw-r--r--   0 fialho     (502) staff       (20)        0 2022-03-13 20:13:52.000000 django-splint-kovs-0.0.9.2/src/django_splint/utils/__init__.py
+-rw-r--r--   0 fialho     (502) staff       (20)     4120 2022-03-31 16:48:20.000000 django-splint-kovs-0.0.9.2/src/django_splint/utils/decorators.py
+drwxr-xr-x   0 fialho     (502) staff       (20)        0 2022-05-25 16:40:48.215805 django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/
+-rw-r--r--   0 fialho     (502) staff       (20)     4548 2022-05-25 16:40:47.000000 django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/PKG-INFO
+-rw-r--r--   0 fialho     (502) staff       (20)      709 2022-05-25 16:40:48.000000 django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/SOURCES.txt
+-rw-r--r--   0 fialho     (502) staff       (20)        1 2022-05-25 16:40:47.000000 django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/dependency_links.txt
+-rw-r--r--   0 fialho     (502) staff       (20)      106 2022-05-25 16:40:47.000000 django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/requires.txt
+-rw-r--r--   0 fialho     (502) staff       (20)       14 2022-05-25 16:40:47.000000 django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/top_level.txt
```

### Comparing `django-splint-kovs-0.0.9.1/LICENSE` & `django-splint-kovs-0.0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/PKG-INFO` & `django-splint-kovs-0.0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-splint-kovs
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: Simple package with utilities for projects with Django Framework
 Author: Silvio Moreto
 Author-email: silvio.moreto@medway.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `django-splint-kovs-0.0.9.1/README.md` & `django-splint-kovs-0.0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/setup.cfg` & `django-splint-kovs-0.0.9.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-splint-kovs
-version = 0.0.9.1
+version = 0.0.9.2
 author = Silvio Moreto
 author_email = silvio.moreto@medway.com.br
 description = Simple package with utilities for projects with Django Framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/admin.py` & `django-splint-kovs-0.0.9.2/src/django_splint/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from django.conf import settings
 from django.contrib import admin
 from django.core.exceptions import FieldError
 
 from import_export.admin import ExportActionMixin
 
-from db.models import SplintModel
+from django_splint.db.models import SplintModel
 
 
 try:
     EXTRA_CSS = settings.EXTRA_CSS
 except AttributeError:
     EXTRA_CSS = '/static/css/custom_admin.css'
```

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/api/filters.py` & `django-splint-kovs-0.0.9.2/src/django_splint/api/filters.py`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/api/permissions.py` & `django-splint-kovs-0.0.9.2/src/django_splint/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/api/serializers.py` & `django-splint-kovs-0.0.9.2/src/django_splint/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/api/views.py` & `django-splint-kovs-0.0.9.2/src/django_splint/api/views.py`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/db/fields.py` & `django-splint-kovs-0.0.9.2/src/django_splint/db/fields.py`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/db/models.py` & `django-splint-kovs-0.0.9.2/src/django_splint/db/models.py`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint/utils/decorators.py` & `django-splint-kovs-0.0.9.2/src/django_splint/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/PKG-INFO` & `django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-splint-kovs
-Version: 0.0.9.1
+Version: 0.0.9.2
 Summary: Simple package with utilities for projects with Django Framework
 Author: Silvio Moreto
 Author-email: silvio.moreto@medway.com.br
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `django-splint-kovs-0.0.9.1/src/django_splint_kovs.egg-info/SOURCES.txt` & `django-splint-kovs-0.0.9.2/src/django_splint_kovs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

