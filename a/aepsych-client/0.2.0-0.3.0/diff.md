# Comparing `tmp/aepsych_client-0.2.0.tar.gz` & `tmp/aepsych_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepsych_client-0.2.0.tar", last modified: Wed Dec  7 19:47:42 2022, max compression
+gzip compressed data, was "aepsych_client-0.3.0.tar", last modified: Fri Jun 23 15:25:01 2023, max compression
```

## Comparing `aepsych_client-0.2.0.tar` & `aepsych_client-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 19:47:42.607452 aepsych_client-0.2.0/
--rw-r--r--   0 craigsanders   (501) staff       (20)     2114 2022-12-07 19:47:42.603628 aepsych_client-0.2.0/PKG-INFO
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 19:47:42.484746 aepsych_client-0.2.0/aepsych_client/
--rw-r--r--   0 craigsanders   (501) staff       (20)      264 2022-12-07 17:18:11.000000 aepsych_client-0.2.0/aepsych_client/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6901 2022-12-07 17:18:11.000000 aepsych_client-0.2.0/aepsych_client/client.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 19:47:42.544695 aepsych_client-0.2.0/aepsych_client.egg-info/
--rw-r--r--   0 craigsanders   (501) staff       (20)     2114 2022-12-07 19:47:42.000000 aepsych_client-0.2.0/aepsych_client.egg-info/PKG-INFO
--rw-r--r--   0 craigsanders   (501) staff       (20)      251 2022-12-07 19:47:42.000000 aepsych_client-0.2.0/aepsych_client.egg-info/SOURCES.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)        1 2022-12-07 19:47:42.000000 aepsych_client-0.2.0/aepsych_client.egg-info/dependency_links.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)       21 2022-12-07 19:47:42.000000 aepsych_client-0.2.0/aepsych_client.egg-info/top_level.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)       38 2022-12-07 19:47:42.613356 aepsych_client-0.2.0/setup.cfg
--rw-r--r--   0 craigsanders   (501) staff       (20)      605 2022-12-07 19:42:11.000000 aepsych_client-0.2.0/setup.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2022-12-07 19:47:42.558918 aepsych_client-0.2.0/tests/
--rw-r--r--   0 craigsanders   (501) staff       (20)        0 2022-12-07 17:18:11.000000 aepsych_client-0.2.0/tests/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4160 2022-12-07 17:18:11.000000 aepsych_client-0.2.0/tests/test_client.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-23 15:25:01.444046 aepsych_client-0.3.0/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2116 2023-06-23 15:25:01.441600 aepsych_client-0.3.0/PKG-INFO
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-23 15:25:01.299617 aepsych_client-0.3.0/aepsych_client/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      264 2023-06-22 19:54:40.000000 aepsych_client-0.3.0/aepsych_client/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     8707 2023-06-22 19:54:40.000000 aepsych_client-0.3.0/aepsych_client/client.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-23 15:25:01.356785 aepsych_client-0.3.0/aepsych_client.egg-info/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2116 2023-06-23 15:25:00.000000 aepsych_client-0.3.0/aepsych_client.egg-info/PKG-INFO
+-rw-r--r--   0 craigsanders   (501) staff       (20)      251 2023-06-23 15:25:00.000000 aepsych_client-0.3.0/aepsych_client.egg-info/SOURCES.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)        1 2023-06-23 15:25:00.000000 aepsych_client-0.3.0/aepsych_client.egg-info/dependency_links.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)       21 2023-06-23 15:25:00.000000 aepsych_client-0.3.0/aepsych_client.egg-info/top_level.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)       38 2023-06-23 15:25:01.445787 aepsych_client-0.3.0/setup.cfg
+-rw-r--r--   0 craigsanders   (501) staff       (20)      605 2023-06-23 15:09:49.000000 aepsych_client-0.3.0/setup.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-23 15:25:01.398628 aepsych_client-0.3.0/tests/
+-rw-r--r--   0 craigsanders   (501) staff       (20)        0 2023-06-22 19:54:40.000000 aepsych_client-0.3.0/tests/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4160 2023-06-22 19:54:40.000000 aepsych_client-0.3.0/tests/test_client.py
```

### Comparing `aepsych_client-0.2.0/PKG-INFO` & `aepsych_client-0.3.0/aepsych_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: aepsych_client
-Version: 0.2.0
+Name: aepsych-client
+Version: 0.3.0
 Description-Content-Type: text/markdown
 
-# AEPsych Python client v0.1
+# AEPsych Python client v0.2.0
 
 This lets you use Python to interface with the AEPsych server to do model-based adaptive experimentation.
 
 ## Installation
 We recommend installing the client under a virtual environment like
 [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 Once you've created a virtual environment for `AEPsychClient` and activated it, you can install through pip:
```

### Comparing `aepsych_client-0.2.0/aepsych_client.egg-info/PKG-INFO` & `aepsych_client-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: aepsych-client
-Version: 0.2.0
+Name: aepsych_client
+Version: 0.3.0
 Description-Content-Type: text/markdown
 
-# AEPsych Python client v0.1
+# AEPsych Python client v0.2.0
 
 This lets you use Python to interface with the AEPsych server to do model-based adaptive experimentation.
 
 ## Installation
 We recommend installing the client under a virtual environment like
 [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
 Once you've created a virtual environment for `AEPsychClient` and activated it, you can install through pip:
```

### Comparing `aepsych_client-0.2.0/setup.py` & `aepsych_client-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "Readme.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="aepsych_client",
-    version="0.2.0",
+    version="0.3.0",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `aepsych_client-0.2.0/tests/test_client.py` & `aepsych_client-0.3.0/tests/test_client.py`

 * *Files identical despite different names*

