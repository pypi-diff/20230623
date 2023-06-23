# Comparing `tmp/dbt_snapshot_analysis-0.2.0.tar.gz` & `tmp/dbt_snapshot_analysis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.2.0.tar", last modified: Fri Jun 23 13:40:59 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.2.1.tar", last modified: Fri Jun 23 13:45:03 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.2.0.tar` & `dbt_snapshot_analysis-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:40:59.000213 dbt_snapshot_analysis-0.2.0/
--rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 13:40:59.000090 dbt_snapshot_analysis-0.2.0/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      820 2023-06-23 12:01:45.000000 dbt_snapshot_analysis-0.2.0/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:40:58.998936 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/data_validation.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3175 2023-06-23 13:39:09.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/dbt_snapshot_analysis.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-22 13:32:52.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/snapshot_utils.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/streamlit_entry_point.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:40:58.999853 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 13:40:59.000275 dbt_snapshot_analysis-0.2.0/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      748 2023-06-23 13:40:39.000000 dbt_snapshot_analysis-0.2.0/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:45:03.228187 dbt_snapshot_analysis-0.2.1/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1241 2023-06-23 13:45:03.228062 dbt_snapshot_analysis-0.2.1/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      822 2023-06-23 13:43:39.000000 dbt_snapshot_analysis-0.2.1/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:45:03.226938 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/data_validation.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3175 2023-06-23 13:39:09.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/dbt_snapshot_analysis.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-22 13:32:52.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/snapshot_utils.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/streamlit_entry_point.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:45:03.227848 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1241 2023-06-23 13:45:03.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 13:45:03.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 13:45:03.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 13:45:03.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 13:45:03.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 13:45:03.000000 dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 13:45:03.228231 dbt_snapshot_analysis-0.2.1/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      851 2023-06-23 13:44:51.000000 dbt_snapshot_analysis-0.2.1/setup.py
```

### Comparing `dbt_snapshot_analysis-0.2.0/README.md` & `dbt_snapshot_analysis-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <h2 align="center" >A Changelog for Data</h3>
 <p align="center">Git-Based. Data-Consumer-Friendly.</p>
 
 <p align="center"><a href="https://data-drift.io">Website</a> · <a href="https://www.data-drift.io/blog">Blog</a></p>
 
 # DBT Snapshot Analysis
 
-[![PyPI version](https://badge.fury.io/py/dbt-snaphot-analysis.svg)](https://badge.fury.io/py/dbt-snaphot-analysis)
+[![PyPI version](https://badge.fury.io/py/dbt-snapshot-analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis)
 
 DBT Snapshot Analysis is a Python package for analyzing snapshots. It provides a set of tools for visualizing and exploring data in a variety of ways.
 
 ## Installation
 
 You can install Plot Analysis using `pip`:
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_q_h4urwq_/tmp6ktndmb5_TarContainer/0/2.md", line 9, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_q_h4urwq_/tmp6ktndmb5_TarContainer/0/2.md", line 9, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,10 +1,10 @@
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
                       Git-Based. Data-Consumer-Friendly.
                                 Website Â· Blog
-# DBT Snapshot Analysis [![PyPI version](https://badge.fury.io/py/dbt-snaphot-
-analysis.svg)](https://badge.fury.io/py/dbt-snaphot-analysis) DBT Snapshot
+# DBT Snapshot Analysis [![PyPI version](https://badge.fury.io/py/dbt-snapshot-
+analysis.svg)](https://badge.fury.io/py/dbt-snapshot-analysis) DBT Snapshot
 Analysis is a Python package for analyzing snapshots. It provides a set of
 tools for visualizing and exploring data in a variety of ways. ## Installation
 You can install Plot Analysis using `pip`: ```sh pip install dbt-snapshot-
 analysis ``` ## Usage ```sh dbt-snapshot-analysis -- ```
```

### Comparing `dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/data_validation.py` & `dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/data_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/dbt_snapshot_analysis.py` & `dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/dbt_snapshot_analysis.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/snapshot_utils.py` & `dbt_snapshot_analysis-0.2.1/dbt_snapshot_analysis/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.0/setup.py` & `dbt_snapshot_analysis-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     py_modules=["dbt_snapshot_analysis"],
     install_requires=["pandas", "matplotlib", "streamlit"],
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "dbt_snapshot_analysis=dbt_snapshot_analysis.streamlit_entry_point:main"
         ]
     },
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
```

