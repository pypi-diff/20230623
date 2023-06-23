# Comparing `tmp/nexusdb-1.2.0.tar.gz` & `tmp/nexusdb-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexusdb-1.2.0.tar", last modified: Sun Jun 18 10:03:58 2023, max compression
+gzip compressed data, was "nexusdb-1.3.1.tar", last modified: Fri Jun 23 09:34:00 2023, max compression
```

## Comparing `nexusdb-1.2.0.tar` & `nexusdb-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 10:03:58.412605 nexusdb-1.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-18 10:03:58.412605 nexusdb-1.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.2.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 10:03:58.412605 nexusdb-1.2.0/nexusdb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      183 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13905 2023-06-18 10:02:05.000000 nexusdb-1.2.0/nexusdb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-18 10:03:58.412605 nexusdb-1.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      990 2023-06-18 10:02:10.000000 nexusdb-1.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 09:34:00.723641 nexusdb-1.3.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 09:34:00.723641 nexusdb-1.3.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.3.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 09:34:00.723641 nexusdb-1.3.1/nexusdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 09:34:00.723641 nexusdb-1.3.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-06-23 09:31:10.000000 nexusdb-1.3.1/setup.py
```

### Comparing `nexusdb-1.2.0/PKG-INFO` & `nexusdb-1.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.2.0
+Version: 1.3.1
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.2.0/nexusdb.egg-info/PKG-INFO` & `nexusdb-1.3.1/nexusdb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.2.0
+Version: 1.3.1
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.2.0/setup.py` & `nexusdb-1.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nexusdb",
-    version="1.2.0",
+    version="1.3.1",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     description="A lightweight JSON-based database system for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/nexusdb",
     packages=find_packages(),
     py_modules=['nexusdb'],
         install_requires=[
-        "uuid",
-        "pytz",
+        "uuid"
     ],
+    entry_points={
+    'console_scripts': [
+    'nexus = nexus:main',
+        ],
+    },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

