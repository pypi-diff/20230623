# Comparing `tmp/pillar1-0.1.7.tar.gz` & `tmp/pillar1-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.7.tar", last modified: Fri Jun 23 13:36:45 2023, max compression
+gzip compressed data, was "pillar1-0.1.7.1.tar", last modified: Fri Jun 23 13:48:46 2023, max compression
```

## Comparing `pillar1-0.1.7.tar` & `pillar1-0.1.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:36:45.276310 pillar1-0.1.7/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-23 13:36:45.276177 pillar1-0.1.7/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:36:45.275278 pillar1-0.1.7/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3675 2023-06-23 13:33:48.000000 pillar1-0.1.7/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:36:45.275899 pillar1-0.1.7/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      202 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 13:36:45.276355 pillar1-0.1.7/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      619 2023-06-23 13:36:35.000000 pillar1-0.1.7/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:48:46.083391 pillar1-0.1.7.1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 13:48:46.083182 pillar1-0.1.7.1/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.1/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:48:46.081529 pillar1-0.1.7.1/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.1/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.1/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 13:48:37.000000 pillar1-0.1.7.1/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:48:46.082192 pillar1-0.1.7.1/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 13:48:46.000000 pillar1-0.1.7.1/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      202 2023-06-23 13:48:46.000000 pillar1-0.1.7.1/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 13:48:46.000000 pillar1-0.1.7.1/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 13:48:46.000000 pillar1-0.1.7.1/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 13:48:46.083463 pillar1-0.1.7.1/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 13:48:42.000000 pillar1-0.1.7.1/setup.py
```

### Comparing `pillar1-0.1.7/PKG-INFO` & `pillar1-0.1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7/README.md` & `pillar1-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7/pillar1/constants.py` & `pillar1-0.1.7.1/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7/pillar1/pillar1.py` & `pillar1-0.1.7.1/pillar1/pillar1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import boto3
 import ipywidgets as widgets
 from IPython.display import display
 from pyspark.sql import SparkSession
-import constants as cn
+import pillar1.constants as cn
 
 MODELS_META = {
     'pillar1-f40b-instruct': {
         'context': '',
         'stop_token': '<|endoftext|>'
     },
     'starcoder-beta': {
```

### Comparing `pillar1-0.1.7/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.7.1/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7/setup.py` & `pillar1-0.1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.7',
+    version='0.1.7.1',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

