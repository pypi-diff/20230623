# Comparing `tmp/nexusdb-1.3.2.tar.gz` & `tmp/nexusdb-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexusdb-1.3.2.tar", last modified: Fri Jun 23 10:28:30 2023, max compression
+gzip compressed data, was "nexusdb-1.3.5.tar", last modified: Fri Jun 23 10:34:48 2023, max compression
```

## Comparing `nexusdb-1.3.2.tar` & `nexusdb-1.3.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:28:30.744611 nexusdb-1.3.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:28:30.744611 nexusdb-1.3.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.3.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:28:30.744611 nexusdb-1.3.2/nexusdb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-23 10:28:30.000000 nexusdb-1.3.2/nexusdb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 10:28:30.744611 nexusdb-1.3.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1088 2023-06-23 10:28:02.000000 nexusdb-1.3.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:34:48.410111 nexusdb-1.3.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:34:48.410111 nexusdb-1.3.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.3.5/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:34:48.406110 nexusdb-1.3.5/nexus/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2023-06-23 10:33:24.000000 nexusdb-1.3.5/nexus/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26311 2023-06-23 09:25:03.000000 nexusdb-1.3.5/nexus/main.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:34:48.410111 nexusdb-1.3.5/nexusdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 10:34:48.410111 nexusdb-1.3.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1088 2023-06-23 10:34:43.000000 nexusdb-1.3.5/setup.py
```

### Comparing `nexusdb-1.3.2/PKG-INFO` & `nexusdb-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.3.2
+Version: 1.3.5
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.3.2/nexusdb.egg-info/PKG-INFO` & `nexusdb-1.3.5/nexusdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.3.2
+Version: 1.3.5
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.3.2/setup.py` & `nexusdb-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nexusdb",
-    version="1.3.2",
+    version="1.3.5",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight JSON-based database system for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/nexusdb",
```

