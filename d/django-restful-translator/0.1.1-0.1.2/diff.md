# Comparing `tmp/django_restful_translator-0.1.1.tar.gz` & `tmp/django_restful_translator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restful_translator-0.1.1.tar", last modified: Fri Jun 23 10:03:39 2023, max compression
+gzip compressed data, was "django_restful_translator-0.1.2.tar", last modified: Fri Jun 23 10:13:33 2023, max compression
```

## Comparing `django_restful_translator-0.1.1.tar` & `django_restful_translator-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:03:39.914157 django_restful_translator-0.1.1/
--rw-r--r--   0 alex       (501) staff       (20)     8196 2023-06-23 09:58:00.000000 django_restful_translator-0.1.1/.DS_Store
--rw-r--r--   0 alex       (501) staff       (20)     1188 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/.gitignore
--rw-r--r--   0 alex       (501) staff       (20)     1075 2023-06-23 08:32:22.000000 django_restful_translator-0.1.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       56 2023-06-23 09:57:36.000000 django_restful_translator-0.1.1/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-23 10:03:39.914036 django_restful_translator-0.1.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4396 2023-06-23 09:55:35.000000 django_restful_translator-0.1.1/README.md
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2191 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/admin.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:03:39.912630 django_restful_translator-0.1.1/django_restful_translator.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-23 10:03:39.000000 django_restful_translator-0.1.1/django_restful_translator.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      605 2023-06-23 10:03:39.000000 django_restful_translator-0.1.1/django_restful_translator.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-23 10:03:39.000000 django_restful_translator-0.1.1/django_restful_translator.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       49 2023-06-23 10:03:39.000000 django_restful_translator-0.1.1/django_restful_translator.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       26 2023-06-23 10:03:39.000000 django_restful_translator-0.1.1/django_restful_translator.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:03:39.913026 django_restful_translator-0.1.1/drf/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/drf/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      432 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/drf/fields.py
--rw-r--r--   0 alex       (501) staff       (20)     2296 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/drf/serializers.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:03:39.913178 django_restful_translator-0.1.1/management/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:08.000000 django_restful_translator-0.1.1/management/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:03:39.913556 django_restful_translator-0.1.1/management/commands/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:15.000000 django_restful_translator-0.1.1/management/commands/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2663 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/management/commands/generatelocales.py
--rw-r--r--   0 alex       (501) staff       (20)     2685 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/management/commands/update_database_translations.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:03:39.913860 django_restful_translator-0.1.1/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     1218 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1041 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/models.py
--rw-r--r--   0 alex       (501) staff       (20)       49 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/requirements.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-23 10:03:39.914201 django_restful_translator-0.1.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      916 2023-06-23 10:03:18.000000 django_restful_translator-0.1.1/setup.py
--rw-r--r--   0 alex       (501) staff       (20)      641 2023-06-23 08:31:59.000000 django_restful_translator-0.1.1/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:13:33.492323 django_restful_translator-0.1.2/
+-rw-r--r--   0 alex       (501) staff       (20)     1075 2023-06-23 08:32:22.000000 django_restful_translator-0.1.2/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-23 10:13:33.492206 django_restful_translator-0.1.2/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4396 2023-06-23 09:55:35.000000 django_restful_translator-0.1.2/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:13:33.490121 django_restful_translator-0.1.2/django_resful_translator/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2191 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/admin.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:13:33.490563 django_restful_translator-0.1.2/django_resful_translator/drf/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/drf/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      432 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/drf/fields.py
+-rw-r--r--   0 alex       (501) staff       (20)     2296 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/drf/serializers.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:13:33.490714 django_restful_translator-0.1.2/django_resful_translator/management/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:08.000000 django_restful_translator-0.1.2/django_resful_translator/management/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:13:33.491114 django_restful_translator-0.1.2/django_resful_translator/management/commands/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 09:56:15.000000 django_restful_translator-0.1.2/django_resful_translator/management/commands/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2663 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/management/commands/generatelocales.py
+-rw-r--r--   0 alex       (501) staff       (20)     2685 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/management/commands/update_database_translations.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:13:33.491419 django_restful_translator-0.1.2/django_resful_translator/migrations/
+-rw-r--r--   0 alex       (501) staff       (20)     1218 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/migrations/0001_initial.py
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/migrations/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1041 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/models.py
+-rw-r--r--   0 alex       (501) staff       (20)      641 2023-06-23 08:31:59.000000 django_restful_translator-0.1.2/django_resful_translator/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-23 10:13:33.492024 django_restful_translator-0.1.2/django_restful_translator.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     5030 2023-06-23 10:13:33.000000 django_restful_translator-0.1.2/django_restful_translator.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      880 2023-06-23 10:13:33.000000 django_restful_translator-0.1.2/django_restful_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-23 10:13:33.000000 django_restful_translator-0.1.2/django_restful_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       49 2023-06-23 10:13:33.000000 django_restful_translator-0.1.2/django_restful_translator.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       25 2023-06-23 10:13:33.000000 django_restful_translator-0.1.2/django_restful_translator.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-23 10:13:33.492364 django_restful_translator-0.1.2/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      916 2023-06-23 10:13:13.000000 django_restful_translator-0.1.2/setup.py
```

### Comparing `django_restful_translator-0.1.1/LICENSE` & `django_restful_translator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/PKG-INFO` & `django_restful_translator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_restful_translator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django application providing translation functionalities for Django Rest Framework
 Home-page: https://github.com/AlexIvanchyk/django_restful_translator
 Author: Alex Ivanchyk
 Author-email: alexander.ivanchik@gmail.com
 License: MIT
 Keywords: django rest-framework translation i18n
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django_restful_translator-0.1.1/README.md` & `django_restful_translator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/admin.py` & `django_restful_translator-0.1.2/django_resful_translator/admin.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/django_restful_translator.egg-info/PKG-INFO` & `django_restful_translator-0.1.2/django_restful_translator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restful-translator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django application providing translation functionalities for Django Rest Framework
 Home-page: https://github.com/AlexIvanchyk/django_restful_translator
 Author: Alex Ivanchyk
 Author-email: alexander.ivanchik@gmail.com
 License: MIT
 Keywords: django rest-framework translation i18n
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django_restful_translator-0.1.1/drf/serializers.py` & `django_restful_translator-0.1.2/django_resful_translator/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/management/commands/generatelocales.py` & `django_restful_translator-0.1.2/django_resful_translator/management/commands/generatelocales.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/management/commands/update_database_translations.py` & `django_restful_translator-0.1.2/django_resful_translator/management/commands/update_database_translations.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/migrations/0001_initial.py` & `django_restful_translator-0.1.2/django_resful_translator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/models.py` & `django_restful_translator-0.1.2/django_resful_translator/models.py`

 * *Files identical despite different names*

### Comparing `django_restful_translator-0.1.1/setup.py` & `django_restful_translator-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django_restful_translator',
-    version='0.1.1',
+    version='0.1.2',
     author='Alex Ivanchyk',
     author_email='alexander.ivanchik@gmail.com',
     description='A Django application providing translation functionalities for Django Rest Framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AlexIvanchyk/django_restful_translator',
     packages=find_packages(),
```

### Comparing `django_restful_translator-0.1.1/utils.py` & `django_restful_translator-0.1.2/django_resful_translator/utils.py`

 * *Files identical despite different names*

