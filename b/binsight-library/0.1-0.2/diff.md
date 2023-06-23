# Comparing `tmp/binsight_library-0.1.tar.gz` & `tmp/binsight_library-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binsight_library-0.1.tar", last modified: Thu Jun 22 20:13:54 2023, max compression
+gzip compressed data, was "binsight_library-0.2.tar", last modified: Fri Jun 23 20:47:42 2023, max compression
```

## Comparing `binsight_library-0.1.tar` & `binsight_library-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:13:54.210876 binsight_library-0.1/
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-22 20:13:54.210876 binsight_library-0.1/PKG-INFO
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:06:37.000000 binsight_library-0.1/README.md
-drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:13:54.210876 binsight_library-0.1/binsight_library/
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:05:58.000000 binsight_library-0.1/binsight_library/__init__.py
-drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:13:54.210876 binsight_library-0.1/binsight_library.egg-info/
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-22 20:13:54.000000 binsight_library-0.1/binsight_library.egg-info/PKG-INFO
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      207 2023-06-22 20:13:54.000000 binsight_library-0.1/binsight_library.egg-info/SOURCES.txt
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)        1 2023-06-22 20:13:54.000000 binsight_library-0.1/binsight_library.egg-info/dependency_links.txt
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)       17 2023-06-22 20:13:54.000000 binsight_library-0.1/binsight_library.egg-info/top_level.txt
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)       38 2023-06-22 20:13:54.210876 binsight_library-0.1/setup.cfg
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      571 2023-06-22 20:08:01.000000 binsight_library-0.1/setup.py
+drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 20:47:42.633085 binsight_library-0.2/
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-23 20:47:42.633085 binsight_library-0.2/PKG-INFO
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:06:37.000000 binsight_library-0.2/README.md
+drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 20:47:42.633085 binsight_library-0.2/binsight_library/
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:05:58.000000 binsight_library-0.2/binsight_library/__init__.py
+drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 20:47:42.633085 binsight_library-0.2/binsight_library.egg-info/
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-23 20:47:42.000000 binsight_library-0.2/binsight_library.egg-info/PKG-INFO
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      207 2023-06-23 20:47:42.000000 binsight_library-0.2/binsight_library.egg-info/SOURCES.txt
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)        1 2023-06-23 20:47:42.000000 binsight_library-0.2/binsight_library.egg-info/dependency_links.txt
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)       17 2023-06-23 20:47:42.000000 binsight_library-0.2/binsight_library.egg-info/top_level.txt
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)       38 2023-06-23 20:47:42.633085 binsight_library-0.2/setup.cfg
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      571 2023-06-23 20:46:13.000000 binsight_library-0.2/setup.py
```

### Comparing `binsight_library-0.1/setup.py` & `binsight_library-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='binsight_library',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='Binsight library for data processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Daniel Blanc',
     author_email='dblanc@binsight.app',
     url='https://github.com/username/my-package',
```

