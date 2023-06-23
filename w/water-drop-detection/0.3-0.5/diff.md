# Comparing `tmp/water_drop_detection-0.3.tar.gz` & `tmp/water_drop_detection-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "water_drop_detection-0.3.tar", last modified: Fri Jun 23 14:29:35 2023, max compression
+gzip compressed data, was "water_drop_detection-0.5.tar", last modified: Fri Jun 23 14:39:41 2023, max compression
```

## Comparing `water_drop_detection-0.3.tar` & `water_drop_detection-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:35.968643 water_drop_detection-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:29:35.968643 water_drop_detection-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-23 14:29:23.000000 water_drop_detection-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:29:35.968643 water_drop_detection-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 14:29:23.000000 water_drop_detection-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:35.968643 water_drop_detection-0.3/water_drop_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:25.000000 water_drop_detection-0.3/water_drop_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 14:29:25.000000 water_drop_detection-0.3/water_drop_detection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:29:35.968643 water_drop_detection-0.3/water_drop_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:29:35.000000 water_drop_detection-0.3/water_drop_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:41.389487 water_drop_detection-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:39:41.389487 water_drop_detection-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-23 14:39:27.000000 water_drop_detection-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:39:41.389487 water_drop_detection-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 14:39:27.000000 water_drop_detection-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:41.389487 water_drop_detection-0.5/water_drop_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:29.000000 water_drop_detection-0.5/water_drop_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 14:39:29.000000 water_drop_detection-0.5/water_drop_detection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:41.389487 water_drop_detection-0.5/water_drop_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 14:39:41.000000 water_drop_detection-0.5/water_drop_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 14:39:41.000000 water_drop_detection-0.5/water_drop_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:39:41.000000 water_drop_detection-0.5/water_drop_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 14:39:41.000000 water_drop_detection-0.5/water_drop_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:39:41.000000 water_drop_detection-0.5/water_drop_detection.egg-info/top_level.txt
```

### Comparing `water_drop_detection-0.3/PKG-INFO` & `water_drop_detection-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: water_drop_detection
-Version: 0.3
+Version: 0.5
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
```

### Comparing `water_drop_detection-0.3/README.md` & `water_drop_detection-0.5/README.md`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.3/setup.py` & `water_drop_detection-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     read_me = file.read()
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setuptools.setup(
     name = "water_drop_detection",
-    version = "0.3",
+    version = "0.5",
     author = "Aleksandr Leisle, Sofia Volodina, Alina Shitenko",
     author_email = "a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru",
     description = "A neural network that detects water drops on the surface from an image.",
     long_description = read_me,
     long_description_content_type = "text/markdown",
     project_urls = {
         'Documentation': 'https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf',
```

### Comparing `water_drop_detection-0.3/water_drop_detection.egg-info/PKG-INFO` & `water_drop_detection-0.5/water_drop_detection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: water-drop-detection
-Version: 0.3
+Version: 0.5
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
```

