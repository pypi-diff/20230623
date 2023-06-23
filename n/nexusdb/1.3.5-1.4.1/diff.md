# Comparing `tmp/nexusdb-1.3.5.tar.gz` & `tmp/nexusdb-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexusdb-1.3.5.tar", last modified: Fri Jun 23 10:34:48 2023, max compression
+gzip compressed data, was "nexusdb-1.4.1.tar", last modified: Fri Jun 23 10:42:49 2023, max compression
```

## Comparing `nexusdb-1.3.5.tar` & `nexusdb-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:34:48.410111 nexusdb-1.3.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:34:48.410111 nexusdb-1.3.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.3.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:34:48.406110 nexusdb-1.3.5/nexus/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2023-06-23 10:33:24.000000 nexusdb-1.3.5/nexus/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26311 2023-06-23 09:25:03.000000 nexusdb-1.3.5/nexus/main.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:34:48.410111 nexusdb-1.3.5/nexusdb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-23 10:34:48.000000 nexusdb-1.3.5/nexusdb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 10:34:48.410111 nexusdb-1.3.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1088 2023-06-23 10:34:43.000000 nexusdb-1.3.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:42:49.975408 nexusdb-1.4.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:42:49.975408 nexusdb-1.4.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.4.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:42:49.975408 nexusdb-1.4.1/nexus/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2023-06-23 10:33:24.000000 nexusdb-1.4.1/nexus/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26342 2023-06-23 10:41:36.000000 nexusdb-1.4.1/nexus/main.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 10:42:49.975408 nexusdb-1.4.1/nexusdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       37 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-23 10:42:49.000000 nexusdb-1.4.1/nexusdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 10:42:49.975408 nexusdb-1.4.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1088 2023-06-23 10:42:28.000000 nexusdb-1.4.1/setup.py
```

### Comparing `nexusdb-1.3.5/PKG-INFO` & `nexusdb-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.3.5
+Version: 1.4.1
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.3.5/nexus/main.py` & `nexusdb-1.4.1/nexus/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 class NexusClient:
     def __init__(self, db_folder):
         self.db_folder = db_folder
         self.authenticated = False
         self.db_path = os.path.join('database', self.db_folder)
         if not os.path.exists(self.db_path):
             os.makedirs(self.db_path)
+        
         self.logs_path = os.path.join(self.db_path, 'logs', 'logs.json')
-        if not os.path.exists(self.logs_path):
-            os.makedirs(os.path.join(self.db_path, 'logs'))
+        logs_dir = os.path.join(self.db_path, 'logs')
+        if not os.path.exists(logs_dir):
+            os.makedirs(logs_dir)
 
         self.config = {}
        
     def set_app_mode(self, mode):
         BOLD_RED = "\033[91m"
         RESET_COLOR = "\033[0m"
         if mode.lower() not in ["production", "development"]:
```

### Comparing `nexusdb-1.3.5/nexusdb.egg-info/PKG-INFO` & `nexusdb-1.4.1/nexusdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.3.5
+Version: 1.4.1
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.3.5/setup.py` & `nexusdb-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nexusdb",
-    version="1.3.5",
+    version="1.4.1",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight JSON-based database system for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/nexusdb",
```

