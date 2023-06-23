# Comparing `tmp/tellosync-0.0.1.tar.gz` & `tmp/tellosync-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellosync-0.0.1.tar", last modified: Fri Jun 23 04:29:18 2023, max compression
+gzip compressed data, was "tellosync-0.0.2.tar", last modified: Fri Jun 23 13:13:42 2023, max compression
```

## Comparing `tellosync-0.0.1.tar` & `tellosync-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 04:29:18.841836 tellosync-0.0.1/
--rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2132 2023-06-23 04:29:18.841836 tellosync-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2023-06-22 13:01:38.000000 tellosync-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 04:29:18.794731 tellosync-0.0.1/easytello/
--rw-rw-rw-   0        0        0      223 2023-06-22 13:01:38.000000 tellosync-0.0.1/easytello/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-06-22 13:01:38.000000 tellosync-0.0.1/easytello/stats.py
--rw-rw-rw-   0        0        0      496 2023-06-23 03:31:30.000000 tellosync-0.0.1/easytello/synchro.py
--rw-rw-rw-   0        0        0     7136 2023-06-23 03:31:30.000000 tellosync-0.0.1/easytello/tello.py
--rw-rw-rw-   0        0        0       42 2023-06-23 04:29:18.841836 tellosync-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-06-23 04:29:03.000000 tellosync-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:29:18.834816 tellosync-0.0.1/tellosync.egg-info/
--rw-rw-rw-   0        0        0     2132 2023-06-23 04:29:18.000000 tellosync-0.0.1/tellosync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-23 04:29:18.000000 tellosync-0.0.1/tellosync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 04:29:18.000000 tellosync-0.0.1/tellosync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-23 04:29:18.000000 tellosync-0.0.1/tellosync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 04:29:18.000000 tellosync-0.0.1/tellosync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 13:13:42.712084 tellosync-0.0.2/
+-rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2132 2023-06-23 13:13:42.709105 tellosync-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1557 2023-06-22 13:01:38.000000 tellosync-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 13:13:42.712084 tellosync-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-23 13:13:14.000000 tellosync-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:13:42.645219 tellosync-0.0.2/tellosync/
+-rw-rw-rw-   0        0        0      223 2023-06-22 13:01:38.000000 tellosync-0.0.2/tellosync/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-06-22 13:01:38.000000 tellosync-0.0.2/tellosync/stats.py
+-rw-rw-rw-   0        0        0      495 2023-06-23 13:10:28.000000 tellosync-0.0.2/tellosync/synchro.py
+-rw-rw-rw-   0        0        0     7136 2023-06-23 13:10:30.000000 tellosync-0.0.2/tellosync/tello.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:13:42.702664 tellosync-0.0.2/tellosync.egg-info/
+-rw-rw-rw-   0        0        0     2132 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/top_level.txt
```

### Comparing `tellosync-0.0.1/LICENSE` & `tellosync-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.1/PKG-INFO` & `tellosync-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tellosync-0.0.1/README.md` & `tellosync-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.1/easytello/stats.py` & `tellosync-0.0.2/tellosync/stats.py`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.1/easytello/tello.py` & `tellosync-0.0.2/tellosync/tello.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import socket
 import threading
 import time
 import cv2
-from easytello.stats import Stats
-from easytello.synchro import Synchro
+from tellosync.stats import Stats
+from tellosync.synchro import Synchro
 
 class Tello:
     def __init__(self, tello_ip: str='192.168.10.1', debug: bool=True, sync: Synchro=None):
         # Opening local UDP port on 8889 for Tello communication
         self.local_ip = ''
         self.local_port = 8889
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
```

### Comparing `tellosync-0.0.1/setup.py` & `tellosync-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tellosync',
-    version='0.0.1',
+    version='0.0.2',
     author='Ezra Fielding, Vincent Wu',
     author_email='ezra.fielding@gmail.com, vwu1888@gmail.com',
     description='An easy framework to support DJI Tello scripting in Python 3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vwu1888/easyTello',
     packages=setuptools.find_packages(),
     install_requires=[
         'opencv-python'
+        'pyserial'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

### Comparing `tellosync-0.0.1/tellosync.egg-info/PKG-INFO` & `tellosync-0.0.2/tellosync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

