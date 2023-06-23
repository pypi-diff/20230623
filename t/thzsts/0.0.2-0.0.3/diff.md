# Comparing `tmp/thzsts-0.0.2.tar.gz` & `tmp/thzsts-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thzsts-0.0.2.tar", last modified: Fri Jun 23 20:10:09 2023, max compression
+gzip compressed data, was "thzsts-0.0.3.tar", last modified: Fri Jun 23 20:39:58 2023, max compression
```

## Comparing `thzsts-0.0.2.tar` & `thzsts-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 20:10:09.781861 thzsts-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-06-23 18:17:52.000000 thzsts-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      842 2023-06-23 20:10:09.780218 thzsts-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-23 19:13:47.000000 thzsts-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 20:10:09.781861 thzsts-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-06-23 20:10:06.000000 thzsts-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 20:10:09.775242 thzsts-0.0.2/src/
--rw-rw-rw-   0        0        0     3132 2023-06-23 20:06:13.000000 thzsts-0.0.2/src/thzccsim.py
-drwxrwxrwx   0        0        0        0 2023-06-23 20:10:09.780218 thzsts-0.0.2/src/thzsts.egg-info/
--rw-rw-rw-   0        0        0      842 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-23 20:10:09.000000 thzsts-0.0.2/src/thzsts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5424 2023-06-23 20:06:32.000000 thzsts-0.0.2/src/thzstsalgorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:39:58.953144 thzsts-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-06-23 18:17:52.000000 thzsts-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      929 2023-06-23 20:39:58.952446 thzsts-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-23 19:13:47.000000 thzsts-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:39:58.953144 thzsts-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-23 20:38:43.000000 thzsts-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:39:58.941599 thzsts-0.0.3/thzsts/
+drwxrwxrwx   0        0        0        0 2023-06-23 20:39:58.951411 thzsts-0.0.3/thzsts/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 20:39:58.950120 thzsts-0.0.3/thzsts/src/thzsts.egg-info/
+-rw-rw-rw-   0        0        0      929 2023-06-23 20:39:58.000000 thzsts-0.0.3/thzsts/src/thzsts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-23 20:39:58.000000 thzsts-0.0.3/thzsts/src/thzsts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:39:58.000000 thzsts-0.0.3/thzsts/src/thzsts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-23 20:39:58.000000 thzsts-0.0.3/thzsts/src/thzsts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 20:39:58.000000 thzsts-0.0.3/thzsts/src/thzsts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8273 2023-06-23 20:38:16.000000 thzsts-0.0.3/thzsts/src/thzsts.py
```

### Comparing `thzsts-0.0.2/LICENSE.txt` & `thzsts-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thzsts-0.0.2/PKG-INFO` & `thzsts-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: thzsts
-Version: 0.0.2
+Version: 0.0.3
 Summary: Function to perform THz STS algorithm and simulate measurements.
 Home-page: https://github.com/NanoTHzCoding/THz_STS_Algorithm
 Author: Stefanie Adams
 Author-email: nanothz.coding@gmail.com
-License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # THz-STS-Algorithm
 A compilation of functions to perform the steady-state terahertz scanning tunneling spectroscopy (THz-STS) algorithm described in Ammerman, S.E. et al. Nat Commun 12, 6794 (2021). https://doi.org/10.1038/s41467-021-26656-3 and functions to determine a true waveform from THz cross-correlation measurements described in ...
 
 ## Installation
```

### Comparing `thzsts-0.0.2/setup.py` & `thzsts-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from setuptools import setup, find_packages
+import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-setup(
+setuptools.setup(
     name='thzsts',
-    version='0.0.2',
+    version='0.0.3',
+    author="Stefanie Adams",
+    author_email="nanothz.coding@gmail.com",
     description='Function to perform THz STS algorithm and simulate measurements.',
-    license='MIT',
-    py_modules=['thzstsalgorithm', 'thzccsim'],
-    package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type="text/markdown",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+    ], 
+    py_modules=['thzsts'],
+    package_dir={'': 'thzsts/src'},
     url="https://github.com/NanoTHzCoding/THz_STS_Algorithm",
-    author="Stefanie Adams",
-    author_email="nanothz.coding@gmail.com",
     install_requires=[
         "numpy",
         "scipy",
         "matplotlib",
         "scikit-learn"
     ],
 )
```

### Comparing `thzsts-0.0.2/src/thzsts.egg-info/PKG-INFO` & `thzsts-0.0.3/thzsts/src/thzsts.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: thzsts
-Version: 0.0.2
+Version: 0.0.3
 Summary: Function to perform THz STS algorithm and simulate measurements.
 Home-page: https://github.com/NanoTHzCoding/THz_STS_Algorithm
 Author: Stefanie Adams
 Author-email: nanothz.coding@gmail.com
-License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # THz-STS-Algorithm
 A compilation of functions to perform the steady-state terahertz scanning tunneling spectroscopy (THz-STS) algorithm described in Ammerman, S.E. et al. Nat Commun 12, 6794 (2021). https://doi.org/10.1038/s41467-021-26656-3 and functions to determine a true waveform from THz cross-correlation measurements described in ...
 
 ## Installation
```

