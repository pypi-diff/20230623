# Comparing `tmp/dbt_snapshot_analysis-0.1.0.tar.gz` & `tmp/dbt_snapshot_analysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.1.0.tar", last modified: Fri Jun 23 12:03:20 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.1.1.tar", last modified: Fri Jun 23 12:31:22 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.1.0.tar` & `dbt_snapshot_analysis-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 12:03:20.018817 dbt_snapshot_analysis-0.1.0/
--rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 12:03:20.018651 dbt_snapshot_analysis-0.1.0/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      820 2023-06-23 12:01:45.000000 dbt_snapshot_analysis-0.1.0/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 12:03:20.018372 dbt_snapshot_analysis-0.1.0/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 12:03:19.000000 dbt_snapshot_analysis-0.1.0/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      290 2023-06-23 12:03:19.000000 dbt_snapshot_analysis-0.1.0/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 12:03:19.000000 dbt_snapshot_analysis-0.1.0/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       69 2023-06-23 12:03:19.000000 dbt_snapshot_analysis-0.1.0/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 12:03:19.000000 dbt_snapshot_analysis-0.1.0/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 12:03:19.000000 dbt_snapshot_analysis-0.1.0/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 12:03:20.018876 dbt_snapshot_analysis-0.1.0/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      662 2023-06-23 12:03:18.000000 dbt_snapshot_analysis-0.1.0/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 12:31:22.934044 dbt_snapshot_analysis-0.1.1/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 12:31:22.933902 dbt_snapshot_analysis-0.1.1/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      820 2023-06-23 12:01:45.000000 dbt_snapshot_analysis-0.1.1/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-23 12:31:22.933702 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      378 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      290 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       69 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       28 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-23 12:31:22.000000 dbt_snapshot_analysis-0.1.1/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-23 12:31:22.934087 dbt_snapshot_analysis-0.1.1/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      662 2023-06-23 12:31:20.000000 dbt_snapshot_analysis-0.1.1/setup.py
```

### Comparing `dbt_snapshot_analysis-0.1.0/README.md` & `dbt_snapshot_analysis-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.1.0/setup.py` & `dbt_snapshot_analysis-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=["pandas", "matplotlib", "streamlit"],
     entry_points={
         "console_scripts": ["dbt_snapshot_analysis=dbt_snapshot_analysis:main"]
     },
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
```

