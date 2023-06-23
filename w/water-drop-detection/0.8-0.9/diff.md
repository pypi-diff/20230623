# Comparing `tmp/water_drop_detection-0.8.tar.gz` & `tmp/water_drop_detection-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "water_drop_detection-0.8.tar", last modified: Fri Jun 23 15:45:48 2023, max compression
+gzip compressed data, was "water_drop_detection-0.9.tar", last modified: Fri Jun 23 15:51:17 2023, max compression
```

## Comparing `water_drop_detection-0.8.tar` & `water_drop_detection-0.9.tar`

### file list

```diff
@@ -1,14 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:45:48.349949 water_drop_detection-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 15:45:48.349949 water_drop_detection-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-23 15:45:34.000000 water_drop_detection-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:45:48.349949 water_drop_detection-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 15:45:34.000000 water_drop_detection-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:45:48.349949 water_drop_detection-0.8/water_drop_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:45:36.000000 water_drop_detection-0.8/water_drop_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 15:45:36.000000 water_drop_detection-0.8/water_drop_detection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:45:48.349949 water_drop_detection-0.8/water_drop_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 15:45:48.000000 water_drop_detection-0.8/water_drop_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 15:45:48.000000 water_drop_detection-0.8/water_drop_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:45:48.000000 water_drop_detection-0.8/water_drop_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 15:45:48.000000 water_drop_detection-0.8/water_drop_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:45:48.000000 water_drop_detection-0.8/water_drop_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.022420 water_drop_detection-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 15:51:17.022420 water_drop_detection-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-23 15:51:02.000000 water_drop_detection-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:51:17.022420 water_drop_detection-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-23 15:51:02.000000 water_drop_detection-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/NN/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/BatchManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/SaveBatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/SaveLoadModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/TestNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/NN/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/NN/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:03.000000 water_drop_detection-0.9/water_drop_detection/NN/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/NN/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:04.000000 water_drop_detection-0.9/water_drop_detection/NN/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:04.000000 water_drop_detection-0.9/water_drop_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 15:51:04.000000 water_drop_detection-0.9/water_drop_detection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-06-23 15:51:04.000000 water_drop_detection-0.9/water_drop_detection/ui/GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:04.000000 water_drop_detection-0.9/water_drop_detection/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/ui/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:04.000000 water_drop_detection-0.9/water_drop_detection/ui/logo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection/ui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:04.000000 water_drop_detection-0.9/water_drop_detection/ui/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:17.018420 water_drop_detection-0.9/water_drop_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-23 15:51:16.000000 water_drop_detection-0.9/water_drop_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-23 15:51:16.000000 water_drop_detection-0.9/water_drop_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:51:16.000000 water_drop_detection-0.9/water_drop_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 15:51:16.000000 water_drop_detection-0.9/water_drop_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-23 15:51:16.000000 water_drop_detection-0.9/water_drop_detection.egg-info/top_level.txt
```

### Comparing `water_drop_detection-0.8/PKG-INFO` & `water_drop_detection-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: water_drop_detection
-Version: 0.8
+Version: 0.9
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
```

### Comparing `water_drop_detection-0.8/README.md` & `water_drop_detection-0.9/README.md`

 * *Files identical despite different names*

### Comparing `water_drop_detection-0.8/water_drop_detection.egg-info/PKG-INFO` & `water_drop_detection-0.9/water_drop_detection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: water-drop-detection
-Version: 0.8
+Version: 0.9
 Summary: A neural network that detects water drops on the surface from an image.
 Home-page: UNKNOWN
 Author: Aleksandr Leisle, Sofia Volodina, Alina Shitenko
 Author-email: a.leisle@g.nsu.ru, s.volodina@g.nsu.ru, a.shitenko@g.nsu.ru
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/HerrPhoton/Water_drop_detection/blob/master/Documentation.pdf
 Project-URL: Bug Tracker, https://github.com/HerrPhoton/Water_drop_detection/issues
```

