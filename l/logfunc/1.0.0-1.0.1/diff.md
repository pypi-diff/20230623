# Comparing `tmp/logfunc-1.0.0.tar.gz` & `tmp/logfunc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-1.0.0.tar", last modified: Fri Jun 23 17:08:44 2023, max compression
+gzip compressed data, was "logfunc-1.0.1.tar", last modified: Fri Jun 23 17:17:40 2023, max compression
```

## Comparing `logfunc-1.0.0.tar` & `logfunc-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 17:08:44.080885 logfunc-1.0.0/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.0.0/LICENSE
--rw-r--r--   0 work       (501) staff       (20)      935 2023-06-23 17:08:44.080763 logfunc-1.0.0/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      148 2023-06-23 16:56:28.000000 logfunc-1.0.0/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 17:08:44.080176 logfunc-1.0.0/logfunc/
--rw-r--r--   0 work       (501) staff       (20)        1 2023-06-23 16:58:26.000000 logfunc-1.0.0/logfunc/__init__.py
--rw-r--r--   0 work       (501) staff       (20)     3017 2023-06-23 17:02:21.000000 logfunc-1.0.0/logfunc/logf.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 17:08:44.080607 logfunc-1.0.0/logfunc.egg-info/
--rw-r--r--   0 work       (501) staff       (20)      935 2023-06-23 17:08:44.000000 logfunc-1.0.0/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      186 2023-06-23 17:08:44.000000 logfunc-1.0.0/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-06-23 17:08:44.000000 logfunc-1.0.0/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-06-23 17:08:44.000000 logfunc-1.0.0/logfunc.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-06-23 17:08:44.080929 logfunc-1.0.0/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)      970 2023-06-23 17:06:54.000000 logfunc-1.0.0/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 17:17:40.868518 logfunc-1.0.1/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.0.1/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)      935 2023-06-23 17:17:40.868373 logfunc-1.0.1/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      148 2023-06-23 16:56:28.000000 logfunc-1.0.1/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 17:17:40.867622 logfunc-1.0.1/logfunc/
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-06-23 16:58:26.000000 logfunc-1.0.1/logfunc/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)     3514 2023-06-23 17:16:26.000000 logfunc-1.0.1/logfunc/logf.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-23 17:17:40.868198 logfunc-1.0.1/logfunc.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)      935 2023-06-23 17:17:40.000000 logfunc-1.0.1/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      186 2023-06-23 17:17:40.000000 logfunc-1.0.1/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-06-23 17:17:40.000000 logfunc-1.0.1/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)        8 2023-06-23 17:17:40.000000 logfunc-1.0.1/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-06-23 17:17:40.868559 logfunc-1.0.1/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)      970 2023-06-23 17:17:37.000000 logfunc-1.0.1/setup.py
```

### Comparing `logfunc-1.0.0/LICENSE` & `logfunc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-1.0.0/PKG-INFO` & `logfunc-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.0.0
+Version: 1.0.1
 Summary: A function decorator/wrapper which allows for logging of args, kwargs, execution time, return value, etc of a func
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `logfunc-1.0.0/logfunc.egg-info/PKG-INFO` & `logfunc-1.0.1/logfunc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.0.0
+Version: 1.0.1
 Summary: A function decorator/wrapper which allows for logging of args, kwargs, execution time, return value, etc of a func
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `logfunc-1.0.0/setup.py` & `logfunc-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='logfunc',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='A function decorator/wrapper which allows for logging of args, kwargs, execution time, return value, etc of a func',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

