# Comparing `tmp/thzsts-0.0.1.tar.gz` & `tmp/thzsts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thzsts-0.0.1.tar", last modified: Fri Jun 23 19:15:05 2023, max compression
+gzip compressed data, was "thzsts-0.0.2.tar", last modified: Fri Jun 23 20:10:09 2023, max compression
```

## Comparing `thzsts-0.0.1.tar` & `thzsts-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:15:05.008577 thzsts-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-23 18:17:52.000000 thzsts-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      767 2023-06-23 19:15:05.008577 thzsts-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-23 19:13:47.000000 thzsts-0.0.1/README.md
--rw-rw-rw-   0        0        0      115 2023-06-23 19:15:05.008577 thzsts-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-06-23 19:13:20.000000 thzsts-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:15:05.000016 thzsts-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 19:15:05.007572 thzsts-0.0.1/src/thzsts.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-23 19:15:04.000000 thzsts-0.0.1/src/thzsts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-06-23 19:15:04.000000 thzsts-0.0.1/src/thzsts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:15:04.000000 thzsts-0.0.1/src/thzsts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-23 19:15:04.000000 thzsts-0.0.1/src/thzsts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:15:04.000000 thzsts-0.0.1/src/thzsts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 20:10:09.781861 thzsts-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-23 18:17:52.000000 thzsts-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      842 2023-06-23 20:10:09.780218 thzsts-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-23 19:13:47.000000 thzsts-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:10:09.781861 thzsts-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-06-23 20:10:06.000000 thzsts-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:10:09.775242 thzsts-0.0.2/src/
+-rw-rw-rw-   0        0        0     3132 2023-06-23 20:06:13.000000 thzsts-0.0.2/src/thzccsim.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:10:09.780218 thzsts-0.0.2/src/thzsts.egg-info/
+-rw-rw-rw-   0        0        0      842 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5424 2023-06-23 20:06:32.000000 thzsts-0.0.2/src/thzstsalgorithm.py
```

### Comparing `thzsts-0.0.1/LICENSE.txt` & `thzsts-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thzsts-0.0.1/PKG-INFO` & `thzsts-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: thzsts
-Version: 0.0.1
+Version: 0.0.2
+Summary: Function to perform THz STS algorithm and simulate measurements.
 Home-page: https://github.com/NanoTHzCoding/THz_STS_Algorithm
 Author: Stefanie Adams
 Author-email: nanothz.coding@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `thzsts-0.0.1/src/thzsts.egg-info/PKG-INFO` & `thzsts-0.0.2/src/thzsts.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: thzsts
-Version: 0.0.1
+Version: 0.0.2
+Summary: Function to perform THz STS algorithm and simulate measurements.
 Home-page: https://github.com/NanoTHzCoding/THz_STS_Algorithm
 Author: Stefanie Adams
 Author-email: nanothz.coding@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

