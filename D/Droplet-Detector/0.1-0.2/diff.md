# Comparing `tmp/Droplet-Detector-0.1.tar.gz` & `tmp/Droplet-Detector-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Droplet-Detector-0.1.tar", last modified: Fri Jun 23 17:02:43 2023, max compression
+gzip compressed data, was "Droplet-Detector-0.2.tar", last modified: Fri Jun 23 18:34:29 2023, max compression
```

## Comparing `Droplet-Detector-0.1.tar` & `Droplet-Detector-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 17:02:43.671149 Droplet-Detector-0.1/
-drwxrwxrwx   0        0        0        0 2023-06-23 17:02:43.637545 Droplet-Detector-0.1/Droplet-Detector/
--rw-rw-rw-   0        0        0     7192 2023-06-21 22:35:57.000000 Droplet-Detector-0.1/Droplet-Detector/Bot.py
--rw-rw-rw-   0        0        0      281 2023-06-23 16:56:01.000000 Droplet-Detector-0.1/Droplet-Detector/__init__.py
--rw-rw-rw-   0        0        0      407 2023-06-21 12:37:46.000000 Droplet-Detector-0.1/Droplet-Detector/calculate.py
--rw-rw-rw-   0        0        0     1207 2023-06-21 22:37:50.000000 Droplet-Detector-0.1/Droplet-Detector/do_xslx.py
--rw-rw-rw-   0        0        0     2306 2023-06-21 22:47:13.000000 Droplet-Detector-0.1/Droplet-Detector/draw.py
--rw-rw-rw-   0        0        0     1782 2023-06-21 22:44:54.000000 Droplet-Detector-0.1/Droplet-Detector/get_contours.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:02:43.671149 Droplet-Detector-0.1/Droplet_Detector.egg-info/
--rw-rw-rw-   0        0        0     6425 2023-06-23 17:02:43.000000 Droplet-Detector-0.1/Droplet_Detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-23 17:02:43.000000 Droplet-Detector-0.1/Droplet_Detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 17:02:43.000000 Droplet-Detector-0.1/Droplet_Detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      190 2023-06-23 17:02:43.000000 Droplet-Detector-0.1/Droplet_Detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-23 17:02:43.000000 Droplet-Detector-0.1/Droplet_Detector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6425 2023-06-23 17:02:43.671149 Droplet-Detector-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5818 2023-06-23 17:00:22.000000 Droplet-Detector-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 17:02:43.671149 Droplet-Detector-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-06-23 16:55:51.000000 Droplet-Detector-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:34:29.180449 Droplet-Detector-0.2/
+drwxrwxrwx   0        0        0        0 2023-06-23 18:34:29.132896 Droplet-Detector-0.2/Droplet-Detector/
+-rw-rw-rw-   0        0        0     7192 2023-06-21 22:35:57.000000 Droplet-Detector-0.2/Droplet-Detector/Bot.py
+-rw-rw-rw-   0        0        0      281 2023-06-23 16:56:01.000000 Droplet-Detector-0.2/Droplet-Detector/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-06-21 12:37:46.000000 Droplet-Detector-0.2/Droplet-Detector/calculate.py
+-rw-rw-rw-   0        0        0     1207 2023-06-21 22:37:50.000000 Droplet-Detector-0.2/Droplet-Detector/do_xslx.py
+-rw-rw-rw-   0        0        0     2306 2023-06-21 22:47:13.000000 Droplet-Detector-0.2/Droplet-Detector/draw.py
+-rw-rw-rw-   0        0        0     1782 2023-06-21 22:44:54.000000 Droplet-Detector-0.2/Droplet-Detector/get_contours.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:34:29.180449 Droplet-Detector-0.2/Droplet_Detector.egg-info/
+-rw-rw-rw-   0        0        0     6425 2023-06-23 18:34:28.000000 Droplet-Detector-0.2/Droplet_Detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-23 18:34:28.000000 Droplet-Detector-0.2/Droplet_Detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 18:34:28.000000 Droplet-Detector-0.2/Droplet_Detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2023-06-23 18:34:28.000000 Droplet-Detector-0.2/Droplet_Detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-23 18:34:28.000000 Droplet-Detector-0.2/Droplet_Detector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6425 2023-06-23 18:34:29.180449 Droplet-Detector-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5818 2023-06-23 17:00:22.000000 Droplet-Detector-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 18:34:29.192430 Droplet-Detector-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-06-23 18:33:56.000000 Droplet-Detector-0.2/setup.py
```

### Comparing `Droplet-Detector-0.1/Droplet-Detector/Bot.py` & `Droplet-Detector-0.2/Droplet-Detector/Bot.py`

 * *Files identical despite different names*

### Comparing `Droplet-Detector-0.1/Droplet-Detector/do_xslx.py` & `Droplet-Detector-0.2/Droplet-Detector/do_xslx.py`

 * *Files identical despite different names*

### Comparing `Droplet-Detector-0.1/Droplet-Detector/draw.py` & `Droplet-Detector-0.2/Droplet-Detector/draw.py`

 * *Files identical despite different names*

### Comparing `Droplet-Detector-0.1/Droplet-Detector/get_contours.py` & `Droplet-Detector-0.2/Droplet-Detector/get_contours.py`

 * *Files identical despite different names*

### Comparing `Droplet-Detector-0.1/Droplet_Detector.egg-info/PKG-INFO` & `Droplet-Detector-0.2/Droplet_Detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Droplet-Detector
-Version: 0.1
+Version: 0.2
 Summary: Telegram bot that draws the outlines of drips on a photo 
 Home-page: https://github.com/kvasik3000/Droplet-Detector
 Author: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 Author-email: superadrenoline3000@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Droplet-Detector-0.1/PKG-INFO` & `Droplet-Detector-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Droplet-Detector
-Version: 0.1
+Version: 0.2
 Summary: Telegram bot that draws the outlines of drips on a photo 
 Home-page: https://github.com/kvasik3000/Droplet-Detector
 Author: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 Author-email: superadrenoline3000@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Droplet-Detector-0.1/README.md` & `Droplet-Detector-0.2/README.md`

 * *Files identical despite different names*

### Comparing `Droplet-Detector-0.1/setup.py` & `Droplet-Detector-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 :authors: Kvas Andrey, Belkova Ksenia, Nekrasova Anna
 :license: Apache License, Version 2.0, see LICENSE file
 :copyright: (c) 2023 kvasik3000
 """
 
-version = '0.1'
+version = '0.2'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
```

