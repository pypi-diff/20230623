# Comparing `tmp/django-cache-helper-1.0.2.tar.gz` & `tmp/django-cache-helper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cache-helper-1.0.2.tar", last modified: Thu Nov 10 14:22:28 2022, max compression
+gzip compressed data, was "django-cache-helper-1.0.3.tar", last modified: Thu Nov 10 14:28:29 2022, max compression
```

## Comparing `django-cache-helper-1.0.2.tar` & `django-cache-helper-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2022-11-10 14:22:28.519334 django-cache-helper-1.0.2/
--rw-r--r--   0 kevinfox   (501) wheel        (0)     3444 2022-11-10 14:22:28.518991 django-cache-helper-1.0.2/PKG-INFO
--rw-r--r--   0 kevinfox   (501) wheel        (0)     2862 2022-11-10 14:16:47.000000 django-cache-helper-1.0.2/README.md
-drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2022-11-10 14:22:28.514989 django-cache-helper-1.0.2/cache_helper/
--rw-r--r--   0 kevinfox   (501) wheel        (0)       20 2022-11-10 14:22:11.000000 django-cache-helper-1.0.2/cache_helper/__init__.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)     6393 2022-11-10 14:16:47.000000 django-cache-helper-1.0.2/cache_helper/decorators.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)      110 2022-11-10 14:16:47.000000 django-cache-helper-1.0.2/cache_helper/exceptions.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)      470 2020-01-15 18:19:24.000000 django-cache-helper-1.0.2/cache_helper/interfaces.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)       94 2022-11-10 14:16:47.000000 django-cache-helper-1.0.2/cache_helper/settings.py
--rw-r--r--   0 kevinfox   (501) wheel        (0)     4323 2022-11-10 14:16:47.000000 django-cache-helper-1.0.2/cache_helper/utils.py
-drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2022-11-10 14:22:28.518449 django-cache-helper-1.0.2/django_cache_helper.egg-info/
--rw-r--r--   0 kevinfox   (501) wheel        (0)     3444 2022-11-10 14:22:28.000000 django-cache-helper-1.0.2/django_cache_helper.egg-info/PKG-INFO
--rw-r--r--   0 kevinfox   (501) wheel        (0)      391 2022-11-10 14:22:28.000000 django-cache-helper-1.0.2/django_cache_helper.egg-info/SOURCES.txt
--rw-r--r--   0 kevinfox   (501) wheel        (0)        1 2022-11-10 14:22:28.000000 django-cache-helper-1.0.2/django_cache_helper.egg-info/dependency_links.txt
--rw-r--r--   0 kevinfox   (501) wheel        (0)       19 2022-11-10 14:22:28.000000 django-cache-helper-1.0.2/django_cache_helper.egg-info/requires.txt
--rw-r--r--   0 kevinfox   (501) wheel        (0)       13 2022-11-10 14:22:28.000000 django-cache-helper-1.0.2/django_cache_helper.egg-info/top_level.txt
--rw-r--r--   0 kevinfox   (501) wheel        (0)      870 2022-11-10 14:20:44.000000 django-cache-helper-1.0.2/pyproject.toml
--rw-r--r--   0 kevinfox   (501) wheel        (0)       38 2022-11-10 14:22:28.519485 django-cache-helper-1.0.2/setup.cfg
+drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2022-11-10 14:28:29.548106 django-cache-helper-1.0.3/
+-rw-r--r--   0 kevinfox   (501) wheel        (0)     3417 2022-11-10 14:28:29.547608 django-cache-helper-1.0.3/PKG-INFO
+-rw-r--r--   0 kevinfox   (501) wheel        (0)     2835 2022-11-10 14:26:01.000000 django-cache-helper-1.0.3/README.md
+drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2022-11-10 14:28:29.544960 django-cache-helper-1.0.3/cache_helper/
+-rw-r--r--   0 kevinfox   (501) wheel        (0)       20 2022-11-10 14:26:35.000000 django-cache-helper-1.0.3/cache_helper/__init__.py
+-rw-r--r--   0 kevinfox   (501) wheel        (0)     6393 2022-11-10 14:16:47.000000 django-cache-helper-1.0.3/cache_helper/decorators.py
+-rw-r--r--   0 kevinfox   (501) wheel        (0)      110 2022-11-10 14:16:47.000000 django-cache-helper-1.0.3/cache_helper/exceptions.py
+-rw-r--r--   0 kevinfox   (501) wheel        (0)      470 2020-01-15 18:19:24.000000 django-cache-helper-1.0.3/cache_helper/interfaces.py
+-rw-r--r--   0 kevinfox   (501) wheel        (0)       94 2022-11-10 14:16:47.000000 django-cache-helper-1.0.3/cache_helper/settings.py
+-rw-r--r--   0 kevinfox   (501) wheel        (0)     4323 2022-11-10 14:16:47.000000 django-cache-helper-1.0.3/cache_helper/utils.py
+drwxr-xr-x   0 kevinfox   (501) wheel        (0)        0 2022-11-10 14:28:29.546917 django-cache-helper-1.0.3/django_cache_helper.egg-info/
+-rw-r--r--   0 kevinfox   (501) wheel        (0)     3417 2022-11-10 14:28:29.000000 django-cache-helper-1.0.3/django_cache_helper.egg-info/PKG-INFO
+-rw-r--r--   0 kevinfox   (501) wheel        (0)      349 2022-11-10 14:28:29.000000 django-cache-helper-1.0.3/django_cache_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinfox   (501) wheel        (0)        1 2022-11-10 14:28:29.000000 django-cache-helper-1.0.3/django_cache_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinfox   (501) wheel        (0)       13 2022-11-10 14:28:29.000000 django-cache-helper-1.0.3/django_cache_helper.egg-info/top_level.txt
+-rw-r--r--   0 kevinfox   (501) wheel        (0)      841 2022-11-10 14:26:01.000000 django-cache-helper-1.0.3/pyproject.toml
+-rw-r--r--   0 kevinfox   (501) wheel        (0)       38 2022-11-10 14:28:29.548278 django-cache-helper-1.0.3/setup.cfg
```

### Comparing `django-cache-helper-1.0.2/PKG-INFO` & `django-cache-helper-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cache-helper
-Version: 1.0.2
+Version: 1.0.3
 Summary: a simple tool for making caching functions, methods, and class methods a little bit easier.
 Author-email: YCharts <developers@ycharts.com>
 Project-URL: Homepage, https://github.com/ycharts/django_cache_helper
 Keywords: cache,django
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -25,17 +25,17 @@
 django-cache-helper is a simple tool for making caching functions, methods, and class methods a little bit easier.
 It is largely based off of django-cache-utils, however, since cache-utils did not support caching model methods by instance and carried other features I didn't need, django-cache-helper was created.
 
 In order to cache and invalidate a function/method/class_method/static_method:
 
 ## Support
 
-| Python | Django |
-|--------|--------|
-|  3.7, 3.8, 3.9, 3.10      | 3.2    |
+| Python |
+|--------|
+|  3.7, 3.8, 3.9, 3.10      |
 
 
 #### How to Cache
 
 ```python
 # Caching a function
 @cached(60*60)  # 60 Minutes
```

### Comparing `django-cache-helper-1.0.2/README.md` & `django-cache-helper-1.0.3/django_cache_helper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: django-cache-helper
+Version: 1.0.3
+Summary: a simple tool for making caching functions, methods, and class methods a little bit easier.
+Author-email: YCharts <developers@ycharts.com>
+Project-URL: Homepage, https://github.com/ycharts/django_cache_helper
+Keywords: cache,django
+Classifier: Programming Language :: Python :: 3
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 django-cache-helper
 ===================
 
 &nbsp;
 ![PyPI](https://img.shields.io/pypi/v/django-cache-helper?color=green)
 [![Test Suite](https://github.com/ycharts/django_cache_helper/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/ycharts/django_cache_helper/actions/workflows/main.yml)
 [![Coverage Status](https://coveralls.io/repos/github/ycharts/django_cache_helper/badge.svg?branch=master)](https://coveralls.io/github/ycharts/django_cache_helper?branch=master)
@@ -10,17 +25,17 @@
 django-cache-helper is a simple tool for making caching functions, methods, and class methods a little bit easier.
 It is largely based off of django-cache-utils, however, since cache-utils did not support caching model methods by instance and carried other features I didn't need, django-cache-helper was created.
 
 In order to cache and invalidate a function/method/class_method/static_method:
 
 ## Support
 
-| Python | Django |
-|--------|--------|
-|  3.7, 3.8, 3.9, 3.10      | 3.2    |
+| Python |
+|--------|
+|  3.7, 3.8, 3.9, 3.10      |
 
 
 #### How to Cache
 
 ```python
 # Caching a function
 @cached(60*60)  # 60 Minutes
```

### Comparing `django-cache-helper-1.0.2/cache_helper/decorators.py` & `django-cache-helper-1.0.3/cache_helper/decorators.py`

 * *Files identical despite different names*

### Comparing `django-cache-helper-1.0.2/cache_helper/utils.py` & `django-cache-helper-1.0.3/cache_helper/utils.py`

 * *Files identical despite different names*

### Comparing `django-cache-helper-1.0.2/django_cache_helper.egg-info/PKG-INFO` & `django-cache-helper-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: django-cache-helper
-Version: 1.0.2
-Summary: a simple tool for making caching functions, methods, and class methods a little bit easier.
-Author-email: YCharts <developers@ycharts.com>
-Project-URL: Homepage, https://github.com/ycharts/django_cache_helper
-Keywords: cache,django
-Classifier: Programming Language :: Python :: 3
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 django-cache-helper
 ===================
 
 &nbsp;
 ![PyPI](https://img.shields.io/pypi/v/django-cache-helper?color=green)
 [![Test Suite](https://github.com/ycharts/django_cache_helper/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/ycharts/django_cache_helper/actions/workflows/main.yml)
 [![Coverage Status](https://coveralls.io/repos/github/ycharts/django_cache_helper/badge.svg?branch=master)](https://coveralls.io/github/ycharts/django_cache_helper?branch=master)
@@ -25,17 +10,17 @@
 django-cache-helper is a simple tool for making caching functions, methods, and class methods a little bit easier.
 It is largely based off of django-cache-utils, however, since cache-utils did not support caching model methods by instance and carried other features I didn't need, django-cache-helper was created.
 
 In order to cache and invalidate a function/method/class_method/static_method:
 
 ## Support
 
-| Python | Django |
-|--------|--------|
-|  3.7, 3.8, 3.9, 3.10      | 3.2    |
+| Python |
+|--------|
+|  3.7, 3.8, 3.9, 3.10      |
 
 
 #### How to Cache
 
 ```python
 # Caching a function
 @cached(60*60)  # 60 Minutes
```

### Comparing `django-cache-helper-1.0.2/pyproject.toml` & `django-cache-helper-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Framework :: Django",
 ]
-dependencies = [
-    "Django >=3.2.*, <4.0",
-]
+dependencies = []
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/ycharts/django_cache_helper"
 
 [tool.setuptools]
 packages = [
```

