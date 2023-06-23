# Comparing `tmp/Digital_Forming_Solution-0.1.12.tar.gz` & `tmp/Digital_Forming_Solution-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Forming_Solution-0.1.12.tar", last modified: Wed Jun 21 12:02:51 2023, max compression
+gzip compressed data, was "Digital_Forming_Solution-0.1.13.tar", last modified: Fri Jun 23 10:20:04 2023, max compression
```

## Comparing `Digital_Forming_Solution-0.1.12.tar` & `Digital_Forming_Solution-0.1.13.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 12:02:51.826826 Digital_Forming_Solution-0.1.12/
-drwxrwxrwx   0        0        0        0 2023-06-21 12:02:51.744047 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution/
--rw-rw-rw-   0        0        0     2496 2023-06-21 10:18:31.000000 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution/Select_Operations.py
--rw-rw-rw-   0        0        0        0 2023-06-13 09:25:58.000000 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 12:02:51.810869 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution.egg-info/
--rw-rw-rw-   0        0        0      387 2023-06-21 12:02:51.000000 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-21 12:02:51.000000 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 12:02:51.000000 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-21 12:02:51.000000 Digital_Forming_Solution-0.1.12/Digital_Forming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      387 2023-06-21 12:02:51.822840 Digital_Forming_Solution-0.1.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-21 12:02:51.827824 Digital_Forming_Solution-0.1.12/setup.cfg
--rw-rw-rw-   0        0        0      515 2023-06-21 10:20:25.000000 Digital_Forming_Solution-0.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:20:04.761522 Digital_Forming_Solution-0.1.13/
+drwxrwxrwx   0        0        0        0 2023-06-23 10:20:04.701681 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution/
+-rw-rw-rw-   0        0        0     2496 2023-06-21 10:18:31.000000 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution/Select_Operations.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 09:25:58.000000 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:20:04.753544 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      387 2023-06-23 10:20:03.000000 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-23 10:20:04.000000 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 10:20:03.000000 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-23 10:20:03.000000 Digital_Forming_Solution-0.1.13/Digital_Forming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      387 2023-06-23 10:20:04.760526 Digital_Forming_Solution-0.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-23 10:20:04.763517 Digital_Forming_Solution-0.1.13/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-06-23 10:19:49.000000 Digital_Forming_Solution-0.1.13/setup.py
```

### Comparing `Digital_Forming_Solution-0.1.12/Digital_Forming_Solution/Select_Operations.py` & `Digital_Forming_Solution-0.1.13/Digital_Forming_Solution/Select_Operations.py`

 * *Files identical despite different names*

### Comparing `Digital_Forming_Solution-0.1.12/setup.py` & `Digital_Forming_Solution-0.1.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Forming_Solution",
-    version="0.1.12",
+    version="0.1.13",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description="DFS Projects Some of the Packages it help to perform task easily",
     packages=["Digital_Forming_Solution"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

