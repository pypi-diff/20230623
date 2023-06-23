# Comparing `tmp/tissue-detection-0.0.1.tar.gz` & `tmp/tissue-detection-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tissue-detection-0.0.1.tar", last modified: Fri Jun 23 18:58:18 2023, max compression
+gzip compressed data, was "tissue-detection-0.0.2.tar", last modified: Fri Jun 23 19:03:54 2023, max compression
```

## Comparing `tissue-detection-0.0.1.tar` & `tissue-detection-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-06-23 18:58:18.881508 tissue-detection-0.0.1/
--rw-r--r--   0 finsberg   (501) staff       (20)     1055 2023-06-07 08:22:16.000000 tissue-detection-0.0.1/LICENSE
--rw-r--r--   0 finsberg   (501) staff       (20)     1277 2023-06-23 18:58:18.881350 tissue-detection-0.0.1/PKG-INFO
--rw-r--r--   0 finsberg   (501) staff       (20)      547 2023-06-07 20:34:30.000000 tissue-detection-0.0.1/README.md
--rw-r--r--   0 finsberg   (501) staff       (20)     2478 2023-06-20 07:05:48.000000 tissue-detection-0.0.1/pyproject.toml
--rw-r--r--   0 finsberg   (501) staff       (20)       38 2023-06-23 18:58:18.881544 tissue-detection-0.0.1/setup.cfg
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-06-23 18:58:18.870965 tissue-detection-0.0.1/src/
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-06-23 18:58:18.871990 tissue-detection-0.0.1/src/tissue_detection/
--rw-r--r--   0 finsberg   (501) staff       (20)      105 2023-06-16 07:04:16.000000 tissue-detection-0.0.1/src/tissue_detection/__init__.py
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-06-23 18:58:18.874662 tissue-detection-0.0.1/src/tissue_detection/examples/
--rw-r--r--   0 finsberg   (501) staff       (20)   576954 2023-06-07 20:03:39.000000 tissue-detection-0.0.1/src/tissue_detection/examples/A13_firstframe.tif
--rw-r--r--   0 finsberg   (501) staff       (20)      180 2023-06-07 20:23:17.000000 tissue-detection-0.0.1/src/tissue_detection/examples/__init__.py
--rw-r--r--   0 finsberg   (501) staff       (20)     5091 2023-06-23 18:58:02.000000 tissue-detection-0.0.1/src/tissue_detection/template.py
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-06-23 18:58:18.875114 tissue-detection-0.0.1/src/tissue_detection/templates/
--rw-r--r--   0 finsberg   (501) staff       (20)      172 2023-06-07 20:32:57.000000 tissue-detection-0.0.1/src/tissue_detection/templates/__init__.py
--rw-r--r--   0 finsberg   (501) staff       (20)   894860 2023-06-07 09:04:58.000000 tissue-detection-0.0.1/src/tissue_detection/templates/tpe1_template.tif
--rw-r--r--   0 finsberg   (501) staff       (20)     3091 2023-06-20 07:05:48.000000 tissue-detection-0.0.1/src/tissue_detection/tpe.py
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-06-23 18:58:18.872592 tissue-detection-0.0.1/src/tissue_detection.egg-info/
--rw-r--r--   0 finsberg   (501) staff       (20)     1277 2023-06-23 18:58:18.000000 tissue-detection-0.0.1/src/tissue_detection.egg-info/PKG-INFO
--rw-r--r--   0 finsberg   (501) staff       (20)      580 2023-06-23 18:58:18.000000 tissue-detection-0.0.1/src/tissue_detection.egg-info/SOURCES.txt
--rw-r--r--   0 finsberg   (501) staff       (20)        1 2023-06-23 18:58:18.000000 tissue-detection-0.0.1/src/tissue_detection.egg-info/dependency_links.txt
--rw-r--r--   0 finsberg   (501) staff       (20)      285 2023-06-23 18:58:18.000000 tissue-detection-0.0.1/src/tissue_detection.egg-info/requires.txt
--rw-r--r--   0 finsberg   (501) staff       (20)       17 2023-06-23 18:58:18.000000 tissue-detection-0.0.1/src/tissue_detection.egg-info/top_level.txt
-drwxr-xr-x   0 finsberg   (501) staff       (20)        0 2023-06-23 18:58:18.881136 tissue-detection-0.0.1/tests/
--rw-r--r--   0 finsberg   (501) staff       (20)      615 2023-06-20 07:05:48.000000 tissue-detection-0.0.1/tests/test_demos.py
--rw-r--r--   0 finsberg   (501) staff       (20)     3170 2023-06-16 08:25:35.000000 tissue-detection-0.0.1/tests/test_template_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:54.853122 tissue-detection-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-23 19:03:54.853122 tissue-detection-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:03:54.853122 tissue-detection-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:54.849122 tissue-detection-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:54.849122 tissue-detection-0.0.2/src/tissue_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/src/tissue_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:54.849122 tissue-detection-0.0.2/src/tissue_detection/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   576954 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/src/tissue_detection/examples/A13_firstframe.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/src/tissue_detection/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/src/tissue_detection/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:54.849122 tissue-detection-0.0.2/src/tissue_detection/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/src/tissue_detection/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   894860 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/src/tissue_detection/templates/tpe1_template.tif
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/src/tissue_detection/tpe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:54.849122 tissue-detection-0.0.2/src/tissue_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-23 19:03:54.000000 tissue-detection-0.0.2/src/tissue_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 19:03:54.000000 tissue-detection-0.0.2/src/tissue_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:03:54.000000 tissue-detection-0.0.2/src/tissue_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-23 19:03:54.000000 tissue-detection-0.0.2/src/tissue_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 19:03:54.000000 tissue-detection-0.0.2/src/tissue_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:03:54.853122 tissue-detection-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-23 19:03:27.000000 tissue-detection-0.0.2/tests/test_template_matching.py
```

### Comparing `tissue-detection-0.0.1/LICENSE` & `tissue-detection-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tissue-detection-0.0.1/PKG-INFO` & `tissue-detection-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tissue-detection
-Version: 0.0.1
+Version: 0.0.2
 Summary: General suite of ODE solvers
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://computationalphysiology.github.io/tissue-detection
 Project-URL: Documentation, https://computationalphysiology.github.io/tissue-detection
 Project-URL: Source, https://github.com/ComputationalPhysiology/tissue-detection
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/tissue-detection/issues
@@ -23,16 +23,17 @@
 Library for detecting tissue in cardiac TPE and MPS systems.
 
 - Source code: https://github.com/ComputationalPhysiology/tissue-detection
 - Documentation: https://computationalphysiology.github.io/tissue-detection
 
 ## Install
 You can install the library with pip
+
 ```
-python3 -m pip install git+https://github.com/ComputationalPhysiology/tissue-detection.git
+python3 -m pip install tissue-detection
 ```
 
 
 ## Getting started
 
 TBW
```

### Comparing `tissue-detection-0.0.1/pyproject.toml` & `tissue-detection-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "tissue-detection"
-version = "0.0.1"
+version = "0.0.2"
 description = "General suite of ODE solvers"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["cardiac", "ecg", "electrophysiology"]
 dependencies = [
```

### Comparing `tissue-detection-0.0.1/src/tissue_detection/examples/A13_firstframe.tif` & `tissue-detection-0.0.2/src/tissue_detection/examples/A13_firstframe.tif`

 * *Files identical despite different names*

### Comparing `tissue-detection-0.0.1/src/tissue_detection/template.py` & `tissue-detection-0.0.2/src/tissue_detection/template.py`

 * *Files identical despite different names*

### Comparing `tissue-detection-0.0.1/src/tissue_detection/templates/tpe1_template.tif` & `tissue-detection-0.0.2/src/tissue_detection/templates/tpe1_template.tif`

 * *Files identical despite different names*

### Comparing `tissue-detection-0.0.1/src/tissue_detection/tpe.py` & `tissue-detection-0.0.2/src/tissue_detection/tpe.py`

 * *Files identical despite different names*

### Comparing `tissue-detection-0.0.1/src/tissue_detection.egg-info/PKG-INFO` & `tissue-detection-0.0.2/src/tissue_detection.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tissue-detection
-Version: 0.0.1
+Version: 0.0.2
 Summary: General suite of ODE solvers
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://computationalphysiology.github.io/tissue-detection
 Project-URL: Documentation, https://computationalphysiology.github.io/tissue-detection
 Project-URL: Source, https://github.com/ComputationalPhysiology/tissue-detection
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/tissue-detection/issues
@@ -23,16 +23,17 @@
 Library for detecting tissue in cardiac TPE and MPS systems.
 
 - Source code: https://github.com/ComputationalPhysiology/tissue-detection
 - Documentation: https://computationalphysiology.github.io/tissue-detection
 
 ## Install
 You can install the library with pip
+
 ```
-python3 -m pip install git+https://github.com/ComputationalPhysiology/tissue-detection.git
+python3 -m pip install tissue-detection
 ```
 
 
 ## Getting started
 
 TBW
```

### Comparing `tissue-detection-0.0.1/src/tissue_detection.egg-info/SOURCES.txt` & `tissue-detection-0.0.2/src/tissue_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tissue-detection-0.0.1/tests/test_demos.py` & `tissue-detection-0.0.2/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `tissue-detection-0.0.1/tests/test_template_matching.py` & `tissue-detection-0.0.2/tests/test_template_matching.py`

 * *Files identical despite different names*

