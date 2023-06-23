# Comparing `tmp/dipense-0.1.2.tar.gz` & `tmp/dipense-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipense-0.1.2.tar", last modified: Fri Jun 23 14:01:47 2023, max compression
+gzip compressed data, was "dipense-0.1.3.tar", last modified: Fri Jun 23 14:18:28 2023, max compression
```

## Comparing `dipense-0.1.2.tar` & `dipense-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:01:47.012213 dipense-0.1.2/
--rw-rw-r--   0 usman     (1000) usman     (1000)      221 2023-06-23 13:56:36.000000 dipense-0.1.2/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-06-23 13:56:36.000000 dipense-0.1.2/LICENSE
--rw-r--r--   0 usman     (1000) usman     (1000)       64 2023-06-20 05:06:50.000000 dipense-0.1.2/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     3829 2023-06-23 14:01:47.000213 dipense-0.1.2/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     2306 2023-06-23 13:56:36.000000 dipense-0.1.2/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:01:46.988212 dipense-0.1.2/dipense/
--rw-rw-r--   0 usman     (1000) usman     (1000)     2626 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1351 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/default.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     9288 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/drone.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     4601 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/icheckp.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1750 2023-06-23 13:56:36.000000 dipense-0.1.2/dipense/structure.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:01:46.996213 dipense-0.1.2/dipense.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3829 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)      298 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       90 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        8 2023-06-23 14:01:46.000000 dipense-0.1.2/dipense.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-23 14:01:47.012213 dipense-0.1.2/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     2269 2023-06-23 14:01:37.000000 dipense-0.1.2/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:18:28.089391 dipense-0.1.3/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      187 2023-06-23 14:17:59.000000 dipense-0.1.3/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-06-23 13:56:36.000000 dipense-0.1.3/LICENSE
+-rw-r--r--   0 usman     (1000) usman     (1000)       64 2023-06-20 05:06:50.000000 dipense-0.1.3/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3806 2023-06-23 14:18:28.081391 dipense-0.1.3/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2317 2023-06-23 14:17:59.000000 dipense-0.1.3/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:18:28.073391 dipense-0.1.3/dipense/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2626 2023-06-23 14:17:59.000000 dipense-0.1.3/dipense/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1351 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/default.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     9288 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/drone.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4601 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/icheckp.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1750 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/structure.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:18:28.081391 dipense-0.1.3/dipense.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3806 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)      298 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       90 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        8 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-23 14:18:28.089391 dipense-0.1.3/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2269 2023-06-23 14:17:59.000000 dipense-0.1.3/setup.py
```

### Comparing `dipense-0.1.2/LICENSE` & `dipense-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dipense-0.1.2/PKG-INFO` & `dipense-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipense
-Version: 0.1.2
+Version: 0.1.3
 Summary: An OSINT tool for IT ninjas
 Home-page: https://dipense.readthedocs.io
 Download-URL: https://pypi.org/project/dipense
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
 Project-URL: Documentation, https://dipense.readthedocs.io
@@ -124,30 +124,31 @@
 
 - Documentation: https://dipense.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/dipense
 - Docker-hub Release: https://hub.docker.com/r/usmanmusa/dipense
 
 ## DiPense at a glance (docker)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/screen-shot.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 ## DiPense at a glance (pypi)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/dipense-terminal.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 
 Change Log
 ==========
 
-0.1.2 (23/june/2023)
-------------------
+0.1.3 (23/june/2023)
+--------------------
+
+- Fourth (0.1.3) Release
+
+OS compatibility
+
 - Third (0.1.2) Release
 
 OS compatibility
 
-0.1.1 (28/may/2023)
-------------------
 - Second Release
 
-0.1 (13/november/2022)
-------------------
 - First Release
```

### Comparing `dipense-0.1.2/README.md` & `dipense-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -89,12 +89,12 @@
 
 - Documentation: https://dipense.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/dipense
 - Docker-hub Release: https://hub.docker.com/r/usmanmusa/dipense
 
 ## DiPense at a glance (docker)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/screen-shot.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 ## DiPense at a glance (pypi)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/dipense-terminal.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
```

### Comparing `dipense-0.1.2/dipense/__init__.py` & `dipense-0.1.3/dipense/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   your webbrowser, e.g
     _______________________________________________
     ICHECKP(autoOpenMap=True).icheckp('197.3.11.7')
     
 """
 
 __title__ = 'dipense'
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 __author__ = 'Usman Musa'
 __author_email__ = 'usmanmusa1920@gmail.com'
 __author_website__ = 'https://usmanmusa1920.github.io'
 __repository__ = 'https://github.com/usmanmusa1920/dipense'
 __url__ = 'https://dipense.readthedocs.io'
 __copyright__ = 'Copyright (C) 2022 - 2023 Usman Musa'
```

### Comparing `dipense-0.1.2/dipense/default.py` & `dipense-0.1.3/dipense/default.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.2/dipense/drone.py` & `dipense-0.1.3/dipense/drone.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.2/dipense/icheckp.py` & `dipense-0.1.3/dipense/icheckp.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.2/dipense/structure.py` & `dipense-0.1.3/dipense/structure.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.2/dipense.egg-info/PKG-INFO` & `dipense-0.1.3/dipense.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipense
-Version: 0.1.2
+Version: 0.1.3
 Summary: An OSINT tool for IT ninjas
 Home-page: https://dipense.readthedocs.io
 Download-URL: https://pypi.org/project/dipense
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
 Project-URL: Documentation, https://dipense.readthedocs.io
@@ -124,30 +124,31 @@
 
 - Documentation: https://dipense.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/dipense
 - Docker-hub Release: https://hub.docker.com/r/usmanmusa/dipense
 
 ## DiPense at a glance (docker)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/screen-shot.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 ## DiPense at a glance (pypi)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.2/docs/media/dipense-terminal.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 
 Change Log
 ==========
 
-0.1.2 (23/june/2023)
-------------------
+0.1.3 (23/june/2023)
+--------------------
+
+- Fourth (0.1.3) Release
+
+OS compatibility
+
 - Third (0.1.2) Release
 
 OS compatibility
 
-0.1.1 (28/may/2023)
-------------------
 - Second Release
 
-0.1 (13/november/2022)
-------------------
 - First Release
```

### Comparing `dipense-0.1.2/setup.py` & `dipense-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
   name = 'dipense', # name of the main package (base folder i.e dipense)
-  version = '0.1.2',
+  version = '0.1.3',
   description = 'An OSINT tool for IT ninjas',
   long_description = open('README.md').read() + '\n\n' + open('CHANGELOG').read(),
   long_description_content_type='text/markdown',
   python_requires = '>=3.7',
   platforms='any',
   
   url = 'https://dipense.readthedocs.io',
```

