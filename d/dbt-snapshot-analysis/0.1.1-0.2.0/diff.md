# Comparing `tmp/dbt_snapshot_analysis-0.1.1.tar.gz` & `tmp/dbt_snapshot_analysis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.1.1.tar", last modified: Fri Jun 23 12:31:22 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.2.0.tar", last modified: Fri Jun 23 13:40:59 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.1.1.tar` & `dbt_snapshot_analysis-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 12:31:22.934044 dbt_snapshot_analysis-0.1.1/
--rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 12:31:22.933902 dbt_snapshot_analysis-0.1.1/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      820 2023-06-23 12:01:45.000000 dbt_snapshot_analysis-0.1.1/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 12:31:22.933702 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      290 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       69 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 12:31:22.934087 dbt_snapshot_analysis-0.1.1/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      662 2023-06-23 12:31:20.000000 dbt_snapshot_analysis-0.1.1/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:40:59.000213 dbt_snapshot_analysis-0.2.0/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 13:40:59.000090 dbt_snapshot_analysis-0.2.0/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      820 2023-06-23 12:01:45.000000 dbt_snapshot_analysis-0.2.0/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:40:58.998936 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/data_validation.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3175 2023-06-23 13:39:09.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/dbt_snapshot_analysis.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1449 2023-06-22 13:32:52.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/snapshot_utils.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis/streamlit_entry_point.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:40:58.999853 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-23 13:40:58.000000 dbt_snapshot_analysis-0.2.0/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 13:40:59.000275 dbt_snapshot_analysis-0.2.0/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      748 2023-06-23 13:40:39.000000 dbt_snapshot_analysis-0.2.0/setup.py
```

### Comparing `dbt_snapshot_analysis-0.1.1/README.md` & `dbt_snapshot_analysis-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.1.1/setup.py` & `dbt_snapshot_analysis-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.1.1",
+    version="0.2.0",
     packages=find_packages(),
+    py_modules=["dbt_snapshot_analysis"],
     install_requires=["pandas", "matplotlib", "streamlit"],
     entry_points={
-        "console_scripts": ["dbt_snapshot_analysis=dbt_snapshot_analysis:main"]
+        "console_scripts": [
+            "dbt_snapshot_analysis=dbt_snapshot_analysis.streamlit_entry_point:main"
+        ]
     },
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
     description="A package for analyzing snapshots",
     url="https://github.com/data-drift/dbt-snapshot-analytics",
     classifiers=[
         "Programming Language :: Python :: 3",
```

