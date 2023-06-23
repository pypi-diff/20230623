# Comparing `tmp/dbt_snapshot_analysis-0.2.2.tar.gz` & `tmp/dbt_snapshot_analysis-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.2.2.tar", last modified: Fri Jun 23 13:54:59 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.2.3.tar", last modified: Fri Jun 23 13:58:12 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.2.2.tar` & `dbt_snapshot_analysis-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:54:59.281787 dbt_snapshot_analysis-0.2.2/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1346 2023-06-23 13:54:59.281658 dbt_snapshot_analysis-0.2.2/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      927 2023-06-23 13:52:21.000000 dbt_snapshot_analysis-0.2.2/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:54:59.280377 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/data_validation.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3175 2023-06-23 13:39:09.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/dbt_snapshot_analysis.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-22 13:32:52.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/snapshot_utils.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/streamlit_entry_point.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:54:59.281350 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1346 2023-06-23 13:54:59.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 13:54:59.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 13:54:59.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 13:54:59.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 13:54:59.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 13:54:59.000000 dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 13:54:59.281834 dbt_snapshot_analysis-0.2.2/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      851 2023-06-23 13:54:06.000000 dbt_snapshot_analysis-0.2.2/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:58:12.321709 dbt_snapshot_analysis-0.2.3/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 13:58:12.321585 dbt_snapshot_analysis-0.2.3/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      928 2023-06-23 13:57:34.000000 dbt_snapshot_analysis-0.2.3/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:58:12.320531 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/data_validation.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3175 2023-06-23 13:39:09.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/dbt_snapshot_analysis.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-22 13:32:52.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/snapshot_utils.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/streamlit_entry_point.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:58:12.321352 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 13:58:12.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 13:58:12.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 13:58:12.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 13:58:12.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 13:58:12.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 13:58:12.000000 dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 13:58:12.321761 dbt_snapshot_analysis-0.2.3/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      851 2023-06-23 13:58:03.000000 dbt_snapshot_analysis-0.2.3/setup.py
```

### Comparing `dbt_snapshot_analysis-0.2.2/PKG-INFO` & `dbt_snapshot_analysis-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_snapshot_analysis
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
   </a>
 </p>
 
 <h2 align="center" >A Changelog for Data</h3>
 <p align="center">Git-Based. Data-Consumer-Friendly.</p>
 
 <p align="center"><a href="https://data-drift.io">Website</a> · <a href="https://www.data-drift.io/blog">Blog</a></p>
+
 # DBT Snapshot Analysis
 
 [![PyPI version](https://badge.fury.io/py/dbt-snapshot-analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis)
 
 This project is developped by the DataDrift team.
 
 DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_4r_wa3p7_/tmptrg4dgsu_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_4r_wa3p7_/tmptrg4dgsu_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.2 Summary: A
+Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.3 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
```

### Comparing `dbt_snapshot_analysis-0.2.2/README.md` & `dbt_snapshot_analysis-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
   </a>
 </p>
 
 <h2 align="center" >A Changelog for Data</h3>
 <p align="center">Git-Based. Data-Consumer-Friendly.</p>
 
 <p align="center"><a href="https://data-drift.io">Website</a> · <a href="https://www.data-drift.io/blog">Blog</a></p>
+
 # DBT Snapshot Analysis
 
 [![PyPI version](https://badge.fury.io/py/dbt-snapshot-analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis)
 
 This project is developped by the DataDrift team.
 
 DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
```

### Comparing `dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/data_validation.py` & `dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/data_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/dbt_snapshot_analysis.py` & `dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/dbt_snapshot_analysis.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis/snapshot_utils.py` & `dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.2/dbt_snapshot_analysis.egg-info/PKG-INFO` & `dbt_snapshot_analysis-0.2.3/dbt_snapshot_analysis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snapshot-analysis
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
   </a>
 </p>
 
 <h2 align="center" >A Changelog for Data</h3>
 <p align="center">Git-Based. Data-Consumer-Friendly.</p>
 
 <p align="center"><a href="https://data-drift.io">Website</a> · <a href="https://www.data-drift.io/blog">Blog</a></p>
+
 # DBT Snapshot Analysis
 
 [![PyPI version](https://badge.fury.io/py/dbt-snapshot-analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis)
 
 This project is developped by the DataDrift team.
 
 DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_4r_wa3p7_/tmptrg4dgsu_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_4r_wa3p7_/tmptrg4dgsu_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.2 Summary: A
+Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.3 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
```

### Comparing `dbt_snapshot_analysis-0.2.2/setup.py` & `dbt_snapshot_analysis-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     py_modules=["dbt_snapshot_analysis"],
     install_requires=["pandas", "matplotlib", "streamlit"],
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
```

