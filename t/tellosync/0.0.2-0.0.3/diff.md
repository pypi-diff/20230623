# Comparing `tmp/tellosync-0.0.2.tar.gz` & `tmp/tellosync-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellosync-0.0.2.tar", last modified: Fri Jun 23 13:13:42 2023, max compression
+gzip compressed data, was "tellosync-0.0.3.tar", last modified: Fri Jun 23 16:26:33 2023, max compression
```

## Comparing `tellosync-0.0.2.tar` & `tellosync-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:13:42.712084 tellosync-0.0.2/
--rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2132 2023-06-23 13:13:42.709105 tellosync-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2023-06-22 13:01:38.000000 tellosync-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 13:13:42.712084 tellosync-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-23 13:13:14.000000 tellosync-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:13:42.645219 tellosync-0.0.2/tellosync/
--rw-rw-rw-   0        0        0      223 2023-06-22 13:01:38.000000 tellosync-0.0.2/tellosync/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-06-22 13:01:38.000000 tellosync-0.0.2/tellosync/stats.py
--rw-rw-rw-   0        0        0      495 2023-06-23 13:10:28.000000 tellosync-0.0.2/tellosync/synchro.py
--rw-rw-rw-   0        0        0     7136 2023-06-23 13:10:30.000000 tellosync-0.0.2/tellosync/tello.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:13:42.702664 tellosync-0.0.2/tellosync.egg-info/
--rw-rw-rw-   0        0        0     2132 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 13:13:42.000000 tellosync-0.0.2/tellosync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 16:26:33.073251 tellosync-0.0.3/
+-rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2132 2023-06-23 16:26:33.064229 tellosync-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1557 2023-06-22 13:01:38.000000 tellosync-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 16:26:33.073251 tellosync-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-23 16:26:18.000000 tellosync-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:26:33.016042 tellosync-0.0.3/tellosync/
+-rw-rw-rw-   0        0        0      223 2023-06-22 13:01:38.000000 tellosync-0.0.3/tellosync/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-06-22 13:01:38.000000 tellosync-0.0.3/tellosync/stats.py
+-rw-rw-rw-   0        0        0      503 2023-06-23 16:15:24.000000 tellosync-0.0.3/tellosync/synchro.py
+-rw-rw-rw-   0        0        0     7136 2023-06-23 13:10:30.000000 tellosync-0.0.3/tellosync/tello.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:26:33.064229 tellosync-0.0.3/tellosync.egg-info/
+-rw-rw-rw-   0        0        0     2132 2023-06-23 16:26:32.000000 tellosync-0.0.3/tellosync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-23 16:26:32.000000 tellosync-0.0.3/tellosync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:26:32.000000 tellosync-0.0.3/tellosync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-23 16:26:32.000000 tellosync-0.0.3/tellosync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 16:26:32.000000 tellosync-0.0.3/tellosync.egg-info/top_level.txt
```

### Comparing `tellosync-0.0.2/LICENSE` & `tellosync-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.2/PKG-INFO` & `tellosync-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tellosync-0.0.2/README.md` & `tellosync-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.2/setup.py` & `tellosync-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tellosync',
-    version='0.0.2',
+    version='0.0.3',
     author='Ezra Fielding, Vincent Wu',
     author_email='ezra.fielding@gmail.com, vwu1888@gmail.com',
     description='An easy framework to support DJI Tello scripting in Python 3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vwu1888/easyTello',
     packages=setuptools.find_packages(),
     install_requires=[
-        'opencv-python'
+        'opencv-python',
         'pyserial'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `tellosync-0.0.2/tellosync/stats.py` & `tellosync-0.0.3/tellosync/stats.py`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.2/tellosync/tello.py` & `tellosync-0.0.3/tellosync/tello.py`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.2/tellosync.egg-info/PKG-INFO` & `tellosync-0.0.3/tellosync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

