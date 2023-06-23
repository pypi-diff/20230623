# Comparing `tmp/dipense-0.1.3.tar.gz` & `tmp/dipense-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipense-0.1.3.tar", last modified: Fri Jun 23 14:18:28 2023, max compression
+gzip compressed data, was "dipense-0.1.4.tar", last modified: Fri Jun 23 14:27:31 2023, max compression
```

## Comparing `dipense-0.1.3.tar` & `dipense-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:18:28.089391 dipense-0.1.3/
--rw-rw-r--   0 usman     (1000) usman     (1000)      187 2023-06-23 14:17:59.000000 dipense-0.1.3/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-06-23 13:56:36.000000 dipense-0.1.3/LICENSE
--rw-r--r--   0 usman     (1000) usman     (1000)       64 2023-06-20 05:06:50.000000 dipense-0.1.3/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     3806 2023-06-23 14:18:28.081391 dipense-0.1.3/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     2317 2023-06-23 14:17:59.000000 dipense-0.1.3/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:18:28.073391 dipense-0.1.3/dipense/
--rw-rw-r--   0 usman     (1000) usman     (1000)     2626 2023-06-23 14:17:59.000000 dipense-0.1.3/dipense/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1351 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/default.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     9288 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/drone.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     4601 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/icheckp.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1750 2023-06-23 13:56:36.000000 dipense-0.1.3/dipense/structure.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:18:28.081391 dipense-0.1.3/dipense.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3806 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)      298 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       90 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        8 2023-06-23 14:18:27.000000 dipense-0.1.3/dipense.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-23 14:18:28.089391 dipense-0.1.3/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     2269 2023-06-23 14:17:59.000000 dipense-0.1.3/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:27:31.652712 dipense-0.1.4/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      176 2023-06-23 14:27:07.000000 dipense-0.1.4/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-06-23 13:56:36.000000 dipense-0.1.4/LICENSE
+-rw-r--r--   0 usman     (1000) usman     (1000)       64 2023-06-20 05:06:50.000000 dipense-0.1.4/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3836 2023-06-23 14:27:31.644707 dipense-0.1.4/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2358 2023-06-23 14:27:07.000000 dipense-0.1.4/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:27:31.636702 dipense-0.1.4/dipense/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2626 2023-06-23 14:27:07.000000 dipense-0.1.4/dipense/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1351 2023-06-23 13:56:36.000000 dipense-0.1.4/dipense/default.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     9288 2023-06-23 13:56:36.000000 dipense-0.1.4/dipense/drone.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4601 2023-06-23 13:56:36.000000 dipense-0.1.4/dipense/icheckp.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1750 2023-06-23 13:56:36.000000 dipense-0.1.4/dipense/structure.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-23 14:27:31.640704 dipense-0.1.4/dipense.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3836 2023-06-23 14:27:31.000000 dipense-0.1.4/dipense.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)      298 2023-06-23 14:27:31.000000 dipense-0.1.4/dipense.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-23 14:27:31.000000 dipense-0.1.4/dipense.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       90 2023-06-23 14:27:31.000000 dipense-0.1.4/dipense.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        8 2023-06-23 14:27:31.000000 dipense-0.1.4/dipense.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-23 14:27:31.652712 dipense-0.1.4/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2269 2023-06-23 14:27:07.000000 dipense-0.1.4/setup.py
```

### Comparing `dipense-0.1.3/LICENSE` & `dipense-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dipense-0.1.3/PKG-INFO` & `dipense-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipense
-Version: 0.1.3
+Version: 0.1.4
 Summary: An OSINT tool for IT ninjas
 Home-page: https://dipense.readthedocs.io
 Download-URL: https://pypi.org/project/dipense
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
 Project-URL: Documentation, https://dipense.readthedocs.io
@@ -116,39 +116,41 @@
 
 To see positional argument and flags available run the file without any flag or positional argument like:
 
 ```
 python route.py
 ```
 
+## Version Status
+
+- version 0.1.4
+
 ## Useful links
 
 - Documentation: https://dipense.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/dipense
 - Docker-hub Release: https://hub.docker.com/r/usmanmusa/dipense
 
 ## DiPense at a glance (docker)
 
 [![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 ## DiPense at a glance (pypi)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/dipense-terminal.png)](https://dipense.readthedocs.io)
 
 
 Change Log
 ==========
 
-0.1.3 (23/june/2023)
+0.1.4 (23/june/2023)
 --------------------
 
-- Fourth (0.1.3) Release
+- Fifth (0.1.4) Release
 
-OS compatibility
+- Fourth (0.1.3) Release
 
 - Third (0.1.2) Release
 
-OS compatibility
-
 - Second Release
 
 - First Release
```

### Comparing `dipense-0.1.3/README.md` & `dipense-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,20 +81,24 @@
 
 To see positional argument and flags available run the file without any flag or positional argument like:
 
 ```
 python route.py
 ```
 
+## Version Status
+
+- version 0.1.4
+
 ## Useful links
 
 - Documentation: https://dipense.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/dipense
 - Docker-hub Release: https://hub.docker.com/r/usmanmusa/dipense
 
 ## DiPense at a glance (docker)
 
 [![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 ## DiPense at a glance (pypi)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/dipense-terminal.png)](https://dipense.readthedocs.io)
```

### Comparing `dipense-0.1.3/dipense/__init__.py` & `dipense-0.1.4/dipense/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   your webbrowser, e.g
     _______________________________________________
     ICHECKP(autoOpenMap=True).icheckp('197.3.11.7')
     
 """
 
 __title__ = 'dipense'
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 __author__ = 'Usman Musa'
 __author_email__ = 'usmanmusa1920@gmail.com'
 __author_website__ = 'https://usmanmusa1920.github.io'
 __repository__ = 'https://github.com/usmanmusa1920/dipense'
 __url__ = 'https://dipense.readthedocs.io'
 __copyright__ = 'Copyright (C) 2022 - 2023 Usman Musa'
```

### Comparing `dipense-0.1.3/dipense/default.py` & `dipense-0.1.4/dipense/default.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.3/dipense/drone.py` & `dipense-0.1.4/dipense/drone.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.3/dipense/icheckp.py` & `dipense-0.1.4/dipense/icheckp.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.3/dipense/structure.py` & `dipense-0.1.4/dipense/structure.py`

 * *Files identical despite different names*

### Comparing `dipense-0.1.3/dipense.egg-info/PKG-INFO` & `dipense-0.1.4/dipense.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipense
-Version: 0.1.3
+Version: 0.1.4
 Summary: An OSINT tool for IT ninjas
 Home-page: https://dipense.readthedocs.io
 Download-URL: https://pypi.org/project/dipense
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
 Project-URL: Documentation, https://dipense.readthedocs.io
@@ -116,39 +116,41 @@
 
 To see positional argument and flags available run the file without any flag or positional argument like:
 
 ```
 python route.py
 ```
 
+## Version Status
+
+- version 0.1.4
+
 ## Useful links
 
 - Documentation: https://dipense.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/dipense
 - Docker-hub Release: https://hub.docker.com/r/usmanmusa/dipense
 
 ## DiPense at a glance (docker)
 
 [![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
 
 ## DiPense at a glance (pypi)
 
-[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/screen-shot.png)](https://dipense.readthedocs.io)
+[![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/v0.1.3/docs/library/media/dipense-terminal.png)](https://dipense.readthedocs.io)
 
 
 Change Log
 ==========
 
-0.1.3 (23/june/2023)
+0.1.4 (23/june/2023)
 --------------------
 
-- Fourth (0.1.3) Release
+- Fifth (0.1.4) Release
 
-OS compatibility
+- Fourth (0.1.3) Release
 
 - Third (0.1.2) Release
 
-OS compatibility
-
 - Second Release
 
 - First Release
```

### Comparing `dipense-0.1.3/setup.py` & `dipense-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
   name = 'dipense', # name of the main package (base folder i.e dipense)
-  version = '0.1.3',
+  version = '0.1.4',
   description = 'An OSINT tool for IT ninjas',
   long_description = open('README.md').read() + '\n\n' + open('CHANGELOG').read(),
   long_description_content_type='text/markdown',
   python_requires = '>=3.7',
   platforms='any',
   
   url = 'https://dipense.readthedocs.io',
```
