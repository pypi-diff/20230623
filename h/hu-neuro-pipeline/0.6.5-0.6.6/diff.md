# Comparing `tmp/hu-neuro-pipeline-0.6.5.tar.gz` & `tmp/hu-neuro-pipeline-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hu-neuro-pipeline-0.6.5.tar", last modified: Sat May 20 06:48:11 2023, max compression
+gzip compressed data, was "hu-neuro-pipeline-0.6.6.tar", last modified: Fri Jun 23 09:05:02 2023, max compression
```

## Comparing `hu-neuro-pipeline-0.6.5.tar` & `hu-neuro-pipeline-0.6.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/.github/workflows/build_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/docs/flowchart.odp
--rw-r--r--   0 runner    (1001) docker     (123)    30937 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/docs/inputs.md
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/docs/outputs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 06:48:11.000000 hu-neuro-pipeline-0.6.5/pipeline/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/averaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/boilerplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/pipeline/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/datasets/ucap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/epoching.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/perm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pipeline/tfr.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:48:11.843191 hu-neuro-pipeline-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-20 06:48:00.000000 hu-neuro-pipeline-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/.github/workflows/build_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/docs/flowchart.odp
+-rw-r--r--   0 runner    (1001) docker     (123)    30937 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/docs/inputs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/docs/outputs.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.915692 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:05:02.000000 hu-neuro-pipeline-0.6.6/pipeline/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/averaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/boilerplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/pipeline/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/datasets/ucap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/epoching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/perm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pipeline/tfr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:05:02.919692 hu-neuro-pipeline-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-23 09:04:55.000000 hu-neuro-pipeline-0.6.6/setup.py
```

### Comparing `hu-neuro-pipeline-0.6.5/.github/workflows/build_publish.yml` & `hu-neuro-pipeline-0.6.6/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/LICENSE` & `hu-neuro-pipeline-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/PKG-INFO` & `hu-neuro-pipeline-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.6.5
+Version: 0.6.6
 Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hu-neuro-pipeline-0.6.5/README.md` & `hu-neuro-pipeline-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/docs/flowchart.odp` & `hu-neuro-pipeline-0.6.6/docs/flowchart.odp`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/docs/inputs.md` & `hu-neuro-pipeline-0.6.6/docs/inputs.md`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/docs/outputs.md` & `hu-neuro-pipeline-0.6.6/docs/outputs.md`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/PKG-INFO` & `hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.6.5
+Version: 0.6.6
 Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hu-neuro-pipeline-0.6.5/hu_neuro_pipeline.egg-info/SOURCES.txt` & `hu-neuro-pipeline-0.6.6/hu_neuro_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/__init__.py` & `hu-neuro-pipeline-0.6.6/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/averaging.py` & `hu-neuro-pipeline-0.6.6/pipeline/averaging.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,13 +264,13 @@
     first_grouping_ix = 1  # Column 0 is participant_id (to average over)
     last_grouping_col = 'freq' if 'freq' in evokeds_df.columns else 'time'
     last_grouping_ix = evokeds_df.columns.get_loc(last_grouping_col)
     grouping_ixs = range(first_grouping_ix, last_grouping_ix + 1)
 
     # Average by grouping columns
     group_cols = list(evokeds_df.columns[grouping_ixs])
-    grands_df = evokeds_df.groupby(group_cols, dropna=False).mean()
+    grands_df = evokeds_df.groupby(group_cols, dropna=False).mean(numeric_only=True)
 
     # Convert conditions from index back to columns
     grands_df = grands_df.reset_index()
 
     return grands_df
```

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/boilerplate.py` & `hu-neuro-pipeline-0.6.6/pipeline/boilerplate.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/datasets/ucap.py` & `hu-neuro-pipeline-0.6.6/pipeline/datasets/ucap.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/epoching.py` & `hu-neuro-pipeline-0.6.6/pipeline/epoching.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/group.py` & `hu-neuro-pipeline-0.6.6/pipeline/group.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/io.py` & `hu-neuro-pipeline-0.6.6/pipeline/io.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/participant.py` & `hu-neuro-pipeline-0.6.6/pipeline/participant.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/perm.py` & `hu-neuro-pipeline-0.6.6/pipeline/perm.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/preprocessing.py` & `hu-neuro-pipeline-0.6.6/pipeline/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/report.py` & `hu-neuro-pipeline-0.6.6/pipeline/report.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/pipeline/tfr.py` & `hu-neuro-pipeline-0.6.6/pipeline/tfr.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.6.5/setup.py` & `hu-neuro-pipeline-0.6.6/setup.py`

 * *Files identical despite different names*

