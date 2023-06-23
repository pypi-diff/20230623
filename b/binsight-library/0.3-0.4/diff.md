# Comparing `tmp/binsight_library-0.3.tar.gz` & `tmp/binsight_library-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binsight_library-0.3.tar", last modified: Fri Jun 23 20:57:39 2023, max compression
+gzip compressed data, was "binsight_library-0.4.tar", last modified: Fri Jun 23 21:04:35 2023, max compression
```

## Comparing `binsight_library-0.3.tar` & `binsight_library-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 20:57:39.004155 binsight_library-0.3/
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-23 20:57:39.004155 binsight_library-0.3/PKG-INFO
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:06:37.000000 binsight_library-0.3/README.md
-drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 20:57:39.004155 binsight_library-0.3/binsight_library/
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:05:58.000000 binsight_library-0.3/binsight_library/__init__.py
-drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 20:57:39.004155 binsight_library-0.3/binsight_library.egg-info/
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-23 20:57:38.000000 binsight_library-0.3/binsight_library.egg-info/PKG-INFO
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      246 2023-06-23 20:57:38.000000 binsight_library-0.3/binsight_library.egg-info/SOURCES.txt
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)        1 2023-06-23 20:57:38.000000 binsight_library-0.3/binsight_library.egg-info/dependency_links.txt
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)       26 2023-06-23 20:57:38.000000 binsight_library-0.3/binsight_library.egg-info/requires.txt
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)       17 2023-06-23 20:57:38.000000 binsight_library-0.3/binsight_library.egg-info/top_level.txt
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)       38 2023-06-23 20:57:39.004155 binsight_library-0.3/setup.cfg
--rw-r--r--   0 dblanc    (1000) dblanc    (1000)      677 2023-06-23 20:57:35.000000 binsight_library-0.3/setup.py
+drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 21:04:35.288474 binsight_library-0.4/
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-23 21:04:35.288474 binsight_library-0.4/PKG-INFO
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:06:37.000000 binsight_library-0.4/README.md
+drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 21:04:35.288474 binsight_library-0.4/binsight_library/
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)        0 2023-06-22 20:05:58.000000 binsight_library-0.4/binsight_library/__init__.py
+drwxr-xr-x   0 dblanc    (1000) dblanc    (1000)        0 2023-06-23 21:04:35.288474 binsight_library-0.4/binsight_library.egg-info/
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      395 2023-06-23 21:04:35.000000 binsight_library-0.4/binsight_library.egg-info/PKG-INFO
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      246 2023-06-23 21:04:35.000000 binsight_library-0.4/binsight_library.egg-info/SOURCES.txt
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)        1 2023-06-23 21:04:35.000000 binsight_library-0.4/binsight_library.egg-info/dependency_links.txt
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)       13 2023-06-23 21:04:35.000000 binsight_library-0.4/binsight_library.egg-info/requires.txt
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)       17 2023-06-23 21:04:35.000000 binsight_library-0.4/binsight_library.egg-info/top_level.txt
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)       38 2023-06-23 21:04:35.288474 binsight_library-0.4/setup.cfg
+-rw-r--r--   0 dblanc    (1000) dblanc    (1000)      634 2023-06-23 21:04:18.000000 binsight_library-0.4/setup.py
```

### Comparing `binsight_library-0.3/setup.py` & `binsight_library-0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='binsight_library',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     description='Binsight library for data processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Daniel Blanc',
     author_email='dblanc@binsight.app',
     url='https://github.com/username/my-package',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-       'pickle',
        'boto3',
        'pandas',
-       'io',
-       'os',
     ],
 )
```

