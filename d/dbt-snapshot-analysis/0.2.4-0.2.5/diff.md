# Comparing `tmp/dbt_snapshot_analysis-0.2.4.tar.gz` & `tmp/dbt_snapshot_analysis-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.2.4.tar", last modified: Fri Jun 23 16:02:24 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.2.5.tar", last modified: Fri Jun 23 16:07:11 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.2.4.tar` & `dbt_snapshot_analysis-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:02:24.546652 dbt_snapshot_analysis-0.2.4/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 16:02:24.546519 dbt_snapshot_analysis-0.2.4/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      928 2023-06-23 13:57:34.000000 dbt_snapshot_analysis-0.2.4/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:02:24.545478 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/data_validation.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     5949 2023-06-23 15:59:28.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/dbt_snapshot_analysis.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-23 15:03:50.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/snapshot_utils.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/streamlit_entry_point.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:02:24.546297 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 16:02:24.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 16:02:24.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 16:02:24.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 16:02:24.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 16:02:24.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 16:02:24.000000 dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 16:02:24.546705 dbt_snapshot_analysis-0.2.4/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      851 2023-06-23 16:02:13.000000 dbt_snapshot_analysis-0.2.4/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:07:11.503872 dbt_snapshot_analysis-0.2.5/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 16:07:11.503744 dbt_snapshot_analysis-0.2.5/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      928 2023-06-23 13:57:34.000000 dbt_snapshot_analysis-0.2.5/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:07:11.502762 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/data_validation.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     5917 2023-06-23 16:05:25.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/dbt_snapshot_analysis.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-23 15:03:50.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/snapshot_utils.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/streamlit_entry_point.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 16:07:11.503555 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1347 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       24 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 16:07:11.000000 dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 16:07:11.503920 dbt_snapshot_analysis-0.2.5/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      847 2023-06-23 16:06:39.000000 dbt_snapshot_analysis-0.2.5/setup.py
```

### Comparing `dbt_snapshot_analysis-0.2.4/PKG-INFO` & `dbt_snapshot_analysis-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_snapshot_analysis
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_2o3scylj_/tmpqp2xor7d_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_2o3scylj_/tmpqp2xor7d_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.4 Summary: A
+Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.5 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
```

### Comparing `dbt_snapshot_analysis-0.2.4/README.md` & `dbt_snapshot_analysis-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/data_validation.py` & `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/data_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/dbt_snapshot_analysis.py` & `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/dbt_snapshot_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import plotly.graph_objects as go
 
 
 from snapshot_utils import (
     get_metric_by_month,
     get_snapshot_as_of_date,
 )
-import matplotlib.pyplot as plt
 
 
 @st.cache_data()
 def compute_all_metric_day_by_day(df: pd.DataFrame, date_range: List[str]):
     print("Computing metric day by day...")
     all_results = pd.DataFrame()
     progress_text = "Operation in progress. Please wait."
```

### Comparing `dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis/snapshot_utils.py` & `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.4/dbt_snapshot_analysis.egg-info/PKG-INFO` & `dbt_snapshot_analysis-0.2.5/dbt_snapshot_analysis.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snapshot-analysis
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_2o3scylj_/tmpqp2xor7d_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_2o3scylj_/tmpqp2xor7d_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.4 Summary: A
+Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.5 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
```

### Comparing `dbt_snapshot_analysis-0.2.4/setup.py` & `dbt_snapshot_analysis-0.2.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     py_modules=["dbt_snapshot_analysis"],
-    install_requires=["pandas", "matplotlib", "streamlit"],
+    install_requires=["pandas", "plotly", "streamlit"],
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "dbt_snapshot_analysis=dbt_snapshot_analysis.streamlit_entry_point:main"
         ]
     },
```

