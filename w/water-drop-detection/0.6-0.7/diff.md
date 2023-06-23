# Comparing `tmp/water_drop_detection-0.6.tar.gz` & `tmp/water_drop_detection-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "water_drop_detection-0.6.tar", last modified: Fri Jun 23 14:47:12 2023, max compression
+gzip compressed data, was "water_drop_detection-0.7.tar", last modified: Fri Jun 23 14:53:33 2023, max compression
```

## Comparing `water_drop_detection-0.6.tar` & `water_drop_detection-0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:12.096735 water_drop_detection-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:47:12.096735 water_drop_detection-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-23 14:47:00.000000 water_drop_detection-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:47:12.096735 water_drop_detection-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-23 14:47:00.000000 water_drop_detection-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:12.096735 water_drop_detection-0.6/water_drop_detection/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:12.096735 water_drop_detection-0.6/water_drop_detection/NN/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-23 14:47:00.000000 water_drop_detection-0.6/water_drop_detection/NN/BatchManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-23 14:47:00.000000 water_drop_detection-0.6/water_drop_detection/NN/SaveBatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-23 14:47:00.000000 water_drop_detection-0.6/water_drop_detection/NN/SaveLoadModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-23 14:47:00.000000 water_drop_detection-0.6/water_drop_detection/NN/TestNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:00.000000 water_drop_detection-0.6/water_drop_detection/NN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-23 14:47:00.000000 water_drop_detection-0.6/water_drop_detection/NN/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:01.000000 water_drop_detection-0.6/water_drop_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 14:47:01.000000 water_drop_detection-0.6/water_drop_detection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:12.096735 water_drop_detection-0.6/water_drop_detection/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-23 14:47:01.000000 water_drop_detection-0.6/water_drop_detection/ui/GUI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:01.000000 water_drop_detection-0.6/water_drop_detection/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:47:12.096735 water_drop_detection-0.6/water_drop_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:47:12.000000 water_drop_detection-0.6/water_drop_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-23 14:47:12.000000 water_drop_detection-0.6/water_drop_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:47:12.000000 water_drop_detection-0.6/water_drop_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 14:47:12.000000 water_drop_detection-0.6/water_drop_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:47:12.000000 water_drop_detection-0.6/water_drop_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:33.210625 water_drop_detection-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:53:33.210625 water_drop_detection-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-23 14:53:19.000000 water_drop_detection-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:53:33.210625 water_drop_detection-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-23 14:53:19.000000 water_drop_detection-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:33.206625 water_drop_detection-0.7/water_drop_detection/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:33.206625 water_drop_detection-0.7/water_drop_detection/NN/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-23 14:53:19.000000 water_drop_detection-0.7/water_drop_detection/NN/BatchManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-23 14:53:19.000000 water_drop_detection-0.7/water_drop_detection/NN/SaveBatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-23 14:53:19.000000 water_drop_detection-0.7/water_drop_detection/NN/SaveLoadModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-23 14:53:19.000000 water_drop_detection-0.7/water_drop_detection/NN/TestNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:19.000000 water_drop_detection-0.7/water_drop_detection/NN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-23 14:53:19.000000 water_drop_detection-0.7/water_drop_detection/NN/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:20.000000 water_drop_detection-0.7/water_drop_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 14:53:20.000000 water_drop_detection-0.7/water_drop_detection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:33.210625 water_drop_detection-0.7/water_drop_detection/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-23 14:53:20.000000 water_drop_detection-0.7/water_drop_detection/ui/GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:20.000000 water_drop_detection-0.7/water_drop_detection/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:33.206625 water_drop_detection-0.7/water_drop_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:53:33.000000 water_drop_detection-0.7/water_drop_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-23 14:53:33.000000 water_drop_detection-0.7/water_drop_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:53:33.000000 water_drop_detection-0.7/water_drop_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 14:53:33.000000 water_drop_detection-0.7/water_drop_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 14:53:33.000000 water_drop_detection-0.7/water_drop_detection.egg-info/top_level.txt
```

### Comparing `water_drop_detection-0.6/PKG-INFO` & `water_drop_detection-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: water_drop_detection
-Version: 0.6
+Version: 0.7
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
```

### Comparing `water_drop_detection-0.6/README.md` & `water_drop_detection-0.7/README.md`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.6/setup.py` & `water_drop_detection-0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,26 @@
     read_me = file.read()
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setuptools.setup(
     name = "water_drop_detection",
-    version = "0.6",
+    version = "0.7",
     author = "Aleksandr Leisle, Sofia Volodina, Alina Shitenko",
     author_email = "a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru",
     description = "A neural network that detects water drops on the surface from an image.",
     long_description = read_me,
     long_description_content_type = "text/markdown",
     project_urls = {
         'Documentation': 'https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf',
         'Bug Tracker': 'https://github.com/HerrPhoton/Water_drop_detection/issues',
         'Homepage': 'https://github.com/HerrPhoton/Water_drop_detection',
     },
-    packages = setuptools.find_packages(),
+    packages = ['water_drop_detection', 'water_drop_detection/NN', 'water_drop_detection/ui'],
     install_requires = requirements,
     classifiers = [
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     python_requires = '==3.9.*',
 )
```

### Comparing `water_drop_detection-0.6/water_drop_detection/NN/BatchManager.py` & `water_drop_detection-0.7/water_drop_detection/NN/BatchManager.py`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.6/water_drop_detection/NN/SaveBatch.py` & `water_drop_detection-0.7/water_drop_detection/NN/SaveBatch.py`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.6/water_drop_detection/NN/SaveLoadModel.py` & `water_drop_detection-0.7/water_drop_detection/NN/SaveLoadModel.py`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.6/water_drop_detection/NN/TestNetwork.py` & `water_drop_detection-0.7/water_drop_detection/NN/TestNetwork.py`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.6/water_drop_detection/NN/main.py` & `water_drop_detection-0.7/water_drop_detection/NN/main.py`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.6/water_drop_detection/ui/GUI.py` & `water_drop_detection-0.7/water_drop_detection/ui/GUI.py`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.6/water_drop_detection.egg-info/PKG-INFO` & `water_drop_detection-0.7/water_drop_detection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: water-drop-detection
-Version: 0.6
+Version: 0.7
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
```

### Comparing `water_drop_detection-0.6/water_drop_detection.egg-info/SOURCES.txt` & `water_drop_detection-0.7/water_drop_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

