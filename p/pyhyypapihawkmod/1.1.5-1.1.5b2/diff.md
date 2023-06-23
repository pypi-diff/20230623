# Comparing `tmp/pyhyypapihawkmod-1.1.5.tar.gz` & `tmp/pyhyypapihawkmod-1.1.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.5.tar", last modified: Fri Jun 23 17:38:27 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.5b2.tar", last modified: Tue Jun 20 10:40:42 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.5.tar` & `pyhyypapihawkmod-1.1.5b2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 17:38:27.135450 pyhyypapihawkmod-1.1.5/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-06-23 17:38:27.134439 pyhyypapihawkmod-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2152 2023-06-23 16:59:10.000000 pyhyypapihawkmod-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 17:38:27.122802 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     8139 2023-06-23 16:58:28.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27863 2023-06-23 16:58:28.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:38:27.132418 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-23 17:38:27.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-06-23 17:38:27.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 17:38:27.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-23 17:38:27.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-23 17:38:27.000000 pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 17:38:27.135450 pyhyypapihawkmod-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-06-23 16:58:51.000000 pyhyypapihawkmod-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:40:42.034148 pyhyypapihawkmod-1.1.5b2/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-06-20 10:40:42.033639 pyhyypapihawkmod-1.1.5b2/PKG-INFO
+-rw-rw-rw-   0        0        0     2126 2023-06-20 10:39:09.000000 pyhyypapihawkmod-1.1.5b2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:40:42.021409 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     8139 2023-06-20 10:38:34.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27863 2023-06-20 10:21:52.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:40:42.031614 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:40:42.034148 pyhyypapihawkmod-1.1.5b2/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-06-20 10:38:42.000000 pyhyypapihawkmod-1.1.5b2/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.5/LICENSE.md` & `pyhyypapihawkmod-1.1.5b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/PKG-INFO` & `pyhyypapihawkmod-1.1.5b2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.5
+Version: 1.1.5b2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.5/README.md` & `pyhyypapihawkmod-1.1.5b2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 - Capture panic api...for obvious reasons.
 - What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
 
 
 Changelog 
 
 1.1.5
-- Added functions to supply notifications for debugging when specifically called.
+- Added functions to supply notifications for debugging
 
 1.1.4
 - Bugfix: When no "triggers" exist a blank key is now returned instead of nothing. This caused a KeyError in home assistant.
 
 1.1.3
 - Bugfix: Fixes a bug when calling notifications
```

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.5
+Version: 1.1.5b2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.5/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.5/setup.py` & `pyhyypapihawkmod-1.1.5b2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.5",
+    version="1.1.5b2",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

