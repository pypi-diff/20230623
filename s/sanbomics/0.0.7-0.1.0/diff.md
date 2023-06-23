# Comparing `tmp/sanbomics-0.0.7.tar.gz` & `tmp/sanbomics-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanbomics-0.0.7.tar", last modified: Mon Nov 28 00:36:21 2022, max compression
+gzip compressed data, was "sanbomics-0.1.0.tar", last modified: Fri Jun 23 15:51:41 2023, max compression
```

## Comparing `sanbomics-0.0.7.tar` & `sanbomics-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2022-11-28 00:36:21.420964 sanbomics-0.0.7/
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)     1073 2022-10-07 04:09:06.000000 sanbomics-0.0.7/LICENSE
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       18 2022-11-28 00:31:48.000000 sanbomics-0.0.7/MANIFEST.in
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      701 2022-11-28 00:36:21.420964 sanbomics-0.0.7/PKG-INFO
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      183 2022-11-27 23:56:11.000000 sanbomics-0.0.7/README.md
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      755 2022-11-28 00:36:15.000000 sanbomics-0.0.7/pyproject.toml
-drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2022-11-28 00:36:21.416964 sanbomics-0.0.7/sanbomics/
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)        0 2022-10-04 03:27:01.000000 sanbomics-0.0.7/sanbomics/__init__.py
-drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2022-11-28 00:36:21.416964 sanbomics-0.0.7/sanbomics/data/
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)  2024851 2022-11-27 22:56:35.000000 sanbomics-0.0.7/sanbomics/data/human_ids.csv
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)  1607953 2022-11-27 22:56:58.000000 sanbomics-0.0.7/sanbomics/data/mouse_ids.csv
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)     8884 2022-10-07 03:39:55.000000 sanbomics-0.0.7/sanbomics/plots.py
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)     2955 2022-11-28 00:15:37.000000 sanbomics-0.0.7/sanbomics/tools.py
-drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2022-11-28 00:36:21.416964 sanbomics-0.0.7/sanbomics.egg-info/
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      701 2022-11-28 00:36:21.000000 sanbomics-0.0.7/sanbomics.egg-info/PKG-INFO
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      326 2022-11-28 00:36:21.000000 sanbomics-0.0.7/sanbomics.egg-info/SOURCES.txt
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)        1 2022-11-28 00:36:21.000000 sanbomics-0.0.7/sanbomics.egg-info/dependency_links.txt
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       68 2022-11-28 00:36:21.000000 sanbomics-0.0.7/sanbomics.egg-info/requires.txt
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       10 2022-11-28 00:36:21.000000 sanbomics-0.0.7/sanbomics.egg-info/top_level.txt
--rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       38 2022-11-28 00:36:21.420964 sanbomics-0.0.7/setup.cfg
+drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2023-06-23 15:51:41.279955 sanbomics-0.1.0/
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)     1073 2022-10-07 04:09:06.000000 sanbomics-0.1.0/LICENSE
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       18 2022-11-28 00:31:48.000000 sanbomics-0.1.0/MANIFEST.in
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      701 2023-06-23 15:51:41.279955 sanbomics-0.1.0/PKG-INFO
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      183 2022-11-27 23:56:11.000000 sanbomics-0.1.0/README.md
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      771 2023-06-23 15:48:30.000000 sanbomics-0.1.0/pyproject.toml
+drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2023-06-23 15:51:41.275955 sanbomics-0.1.0/sanbomics/
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)        0 2022-10-04 03:27:01.000000 sanbomics-0.1.0/sanbomics/__init__.py
+drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2023-06-23 15:51:41.279955 sanbomics-0.1.0/sanbomics/data/
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)  2024851 2022-11-27 22:56:35.000000 sanbomics-0.1.0/sanbomics/data/human_ids.csv
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)  1607953 2022-11-27 22:56:58.000000 sanbomics-0.1.0/sanbomics/data/mouse_ids.csv
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)     8884 2022-10-07 03:39:55.000000 sanbomics-0.1.0/sanbomics/plots.py
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)     7497 2023-06-23 15:41:06.000000 sanbomics-0.1.0/sanbomics/tools.py
+drwxr-xr-x   0 sanbomics  (1000) jrlab2019  (1000)        0 2023-06-23 15:51:41.275955 sanbomics-0.1.0/sanbomics.egg-info/
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      701 2023-06-23 15:51:41.000000 sanbomics-0.1.0/sanbomics.egg-info/PKG-INFO
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)      326 2023-06-23 15:51:41.000000 sanbomics-0.1.0/sanbomics.egg-info/SOURCES.txt
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)        1 2023-06-23 15:51:41.000000 sanbomics-0.1.0/sanbomics.egg-info/dependency_links.txt
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       81 2023-06-23 15:51:41.000000 sanbomics-0.1.0/sanbomics.egg-info/requires.txt
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       10 2023-06-23 15:51:41.000000 sanbomics-0.1.0/sanbomics.egg-info/top_level.txt
+-rw-r--r--   0 sanbomics  (1000) jrlab2019  (1000)       38 2023-06-23 15:51:41.279955 sanbomics-0.1.0/setup.cfg
```

### Comparing `sanbomics-0.0.7/LICENSE` & `sanbomics-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanbomics-0.0.7/PKG-INFO` & `sanbomics-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanbomics
-Version: 0.0.7
+Version: 0.1.0
 Summary: bioinformatics plots and tools for python
 Author-email: Mark Sanborn <mark.email24@gmail.com>
 Project-URL: Homepage, https://github.com/mousepixels/sanbomic
 Project-URL: Bug Tracker, https://github.com/mousepixels/sanbomic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sanbomics-0.0.7/pyproject.toml` & `sanbomics-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sanbomics"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="Mark Sanborn", email="mark.email24@gmail.com" },
 ]
 description = "bioinformatics plots and tools for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-"pandas>=1.0", "numpy>=1.17.0", "matplotlib>=3.4", "seaborn", "adjustText>=0.7.3"
+"pandas>=1.0", "numpy>=1.17.0", "matplotlib>=3.4", "seaborn", "adjustText>=0.7.3", "scipy>=1.9.1"
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/mousepixels/sanbomic"
 "Bug Tracker" = "https://github.com/mousepixels/sanbomic"
```

### Comparing `sanbomics-0.0.7/sanbomics/data/human_ids.csv` & `sanbomics-0.1.0/sanbomics/data/human_ids.csv`

 * *Files identical despite different names*

### Comparing `sanbomics-0.0.7/sanbomics/data/mouse_ids.csv` & `sanbomics-0.1.0/sanbomics/data/mouse_ids.csv`

 * *Files identical despite different names*

### Comparing `sanbomics-0.0.7/sanbomics/plots.py` & `sanbomics-0.1.0/sanbomics/plots.py`

 * *Files identical despite different names*

### Comparing `sanbomics-0.0.7/sanbomics.egg-info/PKG-INFO` & `sanbomics-0.1.0/sanbomics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanbomics
-Version: 0.0.7
+Version: 0.1.0
 Summary: bioinformatics plots and tools for python
 Author-email: Mark Sanborn <mark.email24@gmail.com>
 Project-URL: Homepage, https://github.com/mousepixels/sanbomic
 Project-URL: Bug Tracker, https://github.com/mousepixels/sanbomic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

