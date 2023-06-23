# Comparing `tmp/webcam-1.3.tar.gz` & `tmp/webcam-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-1.3.tar", last modified: Fri Jun 23 12:38:46 2023, max compression
+gzip compressed data, was "webcam-1.4.tar", last modified: Fri Jun 23 12:39:54 2023, max compression
```

## Comparing `webcam-1.3.tar` & `webcam-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 12:38:46.938822 webcam-1.3/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.3/LICENSE
--rw-rw-rw-   0        0        0     4224 2023-06-23 12:38:46.937762 webcam-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 12:38:46.938822 webcam-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-06-23 12:36:27.000000 webcam-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:38:46.905465 webcam-1.3/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.3/webcam/__init__.py
--rw-rw-rw-   0        0        0    10127 2023-06-23 12:36:27.000000 webcam-1.3/webcam/_perspective_manager.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.3/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.3/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    18641 2023-06-23 12:38:38.000000 webcam-1.3/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:38:46.933008 webcam-1.3/webcam.egg-info/
--rw-rw-rw-   0        0        0     4224 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 12:38:46.000000 webcam-1.3/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 12:39:54.080841 webcam-1.4/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.4/LICENSE
+-rw-rw-rw-   0        0        0     4224 2023-06-23 12:39:54.079793 webcam-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 12:39:54.081807 webcam-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-06-23 12:39:51.000000 webcam-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:39:54.057762 webcam-1.4/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.4/webcam/__init__.py
+-rw-rw-rw-   0        0        0    10127 2023-06-23 12:36:27.000000 webcam-1.4/webcam/_perspective_manager.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.4/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.4/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    18641 2023-06-23 12:38:38.000000 webcam-1.4/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:39:54.078558 webcam-1.4/webcam.egg-info/
+-rw-rw-rw-   0        0        0     4224 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 12:39:53.000000 webcam-1.4/webcam.egg-info/top_level.txt
```

### Comparing `webcam-1.3/LICENSE` & `webcam-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-1.3/PKG-INFO` & `webcam-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.3
+Version: 1.4
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `webcam-1.3/README.md` & `webcam-1.4/README.md`

 * *Files identical despite different names*

### Comparing `webcam-1.3/setup.py` & `webcam-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='1.3',
+    version='1.4',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-1.3/webcam/_perspective_manager.py` & `webcam-1.4/webcam/_perspective_manager.py`

 * *Files identical despite different names*

### Comparing `webcam-1.3/webcam/_video_webcam.py` & `webcam-1.4/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-1.3/webcam/_webcam_background.py` & `webcam-1.4/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-1.3/webcam/webcam.py` & `webcam-1.4/webcam/webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-1.3/webcam.egg-info/PKG-INFO` & `webcam-1.4/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.3
+Version: 1.4
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

