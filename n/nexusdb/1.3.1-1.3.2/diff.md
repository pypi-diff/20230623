# Comparing `tmp/nexusdb-1.3.1.tar.gz` & `tmp/nexusdb-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexusdb-1.3.1.tar", last modified: Fri Jun 23 09:34:00 2023, max compression
+gzip compressed data, was "nexusdb-1.3.2.tar", last modified: Fri Jun 23 10:28:30 2023, max compression
```

## Comparing `nexusdb-1.3.1.tar` & `nexusdb-1.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 09:34:00.723641 nexusdb-1.3.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 09:34:00.723641 nexusdb-1.3.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.3.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 09:34:00.723641 nexusdb-1.3.1/nexusdb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-23 09:34:00.000000 nexusdb-1.3.1/nexusdb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 09:34:00.723641 nexusdb-1.3.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-06-23 09:31:10.000000 nexusdb-1.3.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:28:30.744611 nexusdb-1.3.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:28:30.744611 nexusdb-1.3.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.3.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:28:30.744611 nexusdb-1.3.2/nexusdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 10:28:30.744611 nexusdb-1.3.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1088 2023-06-23 10:28:02.000000 nexusdb-1.3.2/setup.py
```

### Comparing `nexusdb-1.3.1/PKG-INFO` & `nexusdb-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.3.1
+Version: 1.3.2
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.3.1/nexusdb.egg-info/PKG-INFO` & `nexusdb-1.3.2/nexusdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.3.1
+Version: 1.3.2
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.3.1/setup.py` & `nexusdb-1.3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nexusdb",
-    version="1.3.1",
+    version="1.3.2",
     author="Pawan kumar",
     author_email="control@vvfin.in",
+    include_package_data=True,
     description="A lightweight JSON-based database system for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/nexusdb",
     packages=find_packages(),
     py_modules=['nexusdb'],
-        install_requires=[
+    install_requires=[
         "uuid"
     ],
     entry_points={
     'console_scripts': [
     'nexus = nexus:main',
         ],
     },
```

