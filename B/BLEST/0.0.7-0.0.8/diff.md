# Comparing `tmp/BLEST-0.0.7.tar.gz` & `tmp/BLEST-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLEST-0.0.7.tar", last modified: Fri Jun 23 01:26:19 2023, max compression
+gzip compressed data, was "BLEST-0.0.8.tar", last modified: Fri Jun 23 02:28:03 2023, max compression
```

## Comparing `BLEST-0.0.7.tar` & `BLEST-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 01:26:19.250604 BLEST-0.0.7/
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 01:26:19.249598 BLEST-0.0.7/BLEST.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)       37 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.7/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 01:26:19.250124 BLEST-0.0.7/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     3369 2023-06-23 01:13:48.000000 BLEST-0.0.7/README.md
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-23 01:26:19.250715 BLEST-0.0.7/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)     1134 2023-06-23 01:24:58.000000 BLEST-0.0.7/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 02:28:03.968040 BLEST-0.0.8/
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 02:28:03.966377 BLEST-0.0.8/BLEST.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 02:28:03.000000 BLEST-0.0.8/BLEST.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-23 02:28:03.000000 BLEST-0.0.8/BLEST.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 02:28:03.000000 BLEST-0.0.8/BLEST.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        8 2023-06-23 02:28:03.000000 BLEST-0.0.8/BLEST.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 02:28:03.000000 BLEST-0.0.8/BLEST.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.8/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 02:28:03.967270 BLEST-0.0.8/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     3369 2023-06-23 01:13:48.000000 BLEST-0.0.8/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-23 02:28:03.968240 BLEST-0.0.8/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)     1039 2023-06-23 02:25:45.000000 BLEST-0.0.8/setup.py
```

### Comparing `BLEST-0.0.7/BLEST.egg-info/PKG-INFO` & `BLEST-0.0.8/BLEST.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BLEST
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `BLEST-0.0.7/LICENSE` & `BLEST-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BLEST-0.0.7/PKG-INFO` & `BLEST-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BLEST
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `BLEST-0.0.7/README.md` & `BLEST-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `BLEST-0.0.7/setup.py` & `BLEST-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="BLEST",
-    version="0.0.7",
+    version="0.0.8",
     author="JHunt",
     author_email="blest@jhunt.dev",
     description="The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/jhuntdev/blest-py",
     packages=find_packages(),
@@ -17,18 +17,12 @@
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "asyncio",
-        "aiohttp",
-        "uuid",
-        "json",
-        "copy",
-        "os",
-        "re"
+        "aiohttp"
     ],
     python_requires=">=3.6",
     platforms="any",
 )
```

