# Comparing `tmp/s2and-0.22.tar.gz` & `tmp/s2and-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2and-0.22.tar", last modified: Thu Jun 22 13:49:27 2023, max compression
+gzip compressed data, was "s2and-0.23.tar", last modified: Fri Jun 23 01:27:13 2023, max compression
```

## Comparing `s2and-0.22.tar` & `s2and-0.23.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-22 13:49:27.227338 s2and-0.22/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.22/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-22 13:49:27.227200 s2and-0.22/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10741 2023-06-21 14:47:32.000000 s2and-0.22/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-22 13:49:27.224758 s2and-0.22/s2and/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.22/s2and/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1751 2023-06-22 13:43:50.000000 s2and-0.22/s2and/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.22/s2and/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    42587 2023-06-20 21:51:56.000000 s2and-0.22/s2and/eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-21 21:37:38.000000 s2and-0.22/s2and/featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.22/s2and/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1132 2023-06-22 13:45:23.000000 s2and-0.22/s2and/inference.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    48439 2023-06-21 20:44:19.000000 s2and-0.22/s2and/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.22/s2and/plotting_utils.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.22/s2and/s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.22/s2and/sampling.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.22/s2and/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-22 13:49:27.225377 s2and-0.22/s2and.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-22 13:49:27.000000 s2and-0.22/s2and.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-22 13:49:27.000000 s2and-0.22/s2and.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-22 13:49:27.000000 s2and-0.22/s2and.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-22 13:49:27.000000 s2and-0.22/s2and.egg-info/top_level.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-22 13:49:27.227376 s2and-0.22/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-22 13:49:15.000000 s2and-0.22/setup.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-22 13:49:27.226998 s2and-0.22/tests/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.22/tests/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_cluster.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_cluster_incremental.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_cluster_incremental_incompatible.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.22/tests/test_text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-23 01:27:13.686077 s2and-0.23/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.23/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-23 01:27:13.685934 s2and-0.23/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10741 2023-06-21 14:47:32.000000 s2and-0.23/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-23 01:27:13.682454 s2and-0.23/s2and/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.23/s2and/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1751 2023-06-23 01:22:30.000000 s2and-0.23/s2and/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    63270 2023-06-23 01:26:19.000000 s2and-0.23/s2and/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    42587 2023-06-20 21:51:56.000000 s2and-0.23/s2and/eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-21 21:37:38.000000 s2and-0.23/s2and/featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.23/s2and/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1133 2023-06-23 01:21:53.000000 s2and-0.23/s2and/inference.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    48439 2023-06-21 20:44:19.000000 s2and-0.23/s2and/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.23/s2and/plotting_utils.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.23/s2and/s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.23/s2and/sampling.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.23/s2and/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-23 01:27:13.683674 s2and-0.23/s2and.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-23 01:27:13.000000 s2and-0.23/s2and.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-23 01:27:13.000000 s2and-0.23/s2and.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-23 01:27:13.000000 s2and-0.23/s2and.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-23 01:27:13.000000 s2and-0.23/s2and.egg-info/top_level.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-23 01:27:13.686138 s2and-0.23/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-23 01:22:53.000000 s2and-0.23/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-23 01:27:13.685725 s2and-0.23/tests/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.23/tests/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_cluster.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_cluster_incremental.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_cluster_incremental_incompatible.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.23/tests/test_text.py
```

### Comparing `s2and-0.22/LICENSE` & `s2and-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `s2and-0.22/README.md` & `s2and-0.23/README.md`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/consts.py` & `s2and-0.23/s2and/consts.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/data.py` & `s2and-0.23/s2and/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Union, Dict, List, Any, Tuple, Set, NamedTuple
-
+import time
 import os
 import json
 import numpy as np
 import pandas as pd
 import logging
 import pickle
 import multiprocessing
@@ -355,21 +355,26 @@
             self.first_dict = load_name_counts["first_dict"]
             self.last_dict = load_name_counts["last_dict"]
             self.first_last_dict = load_name_counts["first_last_dict"]
             self.last_first_initial_dict = load_name_counts["last_first_initial_dict"]
             name_counts_loaded = True
         elif load_name_counts:
             logger.info("loading name counts")
-            with open(cached_path(NAME_COUNTS_PATH), "rb") as f:
-                (
-                    first_dict,
-                    last_dict,
-                    first_last_dict,
-                    last_first_initial_dict,
-                ) = pickle.load(f)
+            while True:
+                try:
+                    with open(cached_path(NAME_COUNTS_PATH), "rb") as f:
+                        (
+                            first_dict,
+                            last_dict,
+                            first_last_dict,
+                            last_first_initial_dict,
+                        ) = pickle.load(f)
+                    break
+                except:
+                    time.sleep(1)
             self.first_dict = first_dict
             self.last_dict = last_dict
             self.first_last_dict = first_last_dict
             self.last_first_initial_dict = last_first_initial_dict
             name_counts_loaded = True
             logger.info("loaded name counts")
```

### Comparing `s2and-0.22/s2and/eval.py` & `s2and-0.23/s2and/eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/featurizer.py` & `s2and-0.23/s2and/featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/file_cache.py` & `s2and-0.23/s2and/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/inference.py` & `s2and-0.23/s2and/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os.path import join
 import pickle
 import pprint
 from s2and.data import ANDData
 
 
-def run(signatures, path_to_data, dataset_name="pubmed", batch_size=100000000, use_cache=True, n_jobs=64):
+def run(signatures, path_to_data, dataset_name="pubmed", batch_size=100000000, use_cache=False, n_jobs=64):
     parent_dir = join(path_to_data, dataset_name)
 
     #signatures = join(parent_dir, f"{dataset_name}_signatures.json")
     papers = join(parent_dir, f"{dataset_name}_papers.json")
 
     with open(join(path_to_data, "production_model.pickle"), "rb") as _pkl_file:
         clusterer = pickle.load(_pkl_file)['clusterer']
```

### Comparing `s2and-0.22/s2and/model.py` & `s2and-0.23/s2and/model.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/plotting_utils.py` & `s2and-0.23/s2and/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/s2_funcs.py` & `s2and-0.23/s2and/s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/sampling.py` & `s2and-0.23/s2and/sampling.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and/text.py` & `s2and-0.23/s2and/text.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/s2and.egg-info/SOURCES.txt` & `s2and-0.23/s2and.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_cluster.py` & `s2and-0.23/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_cluster_incremental.py` & `s2and-0.23/tests/test_cluster_incremental.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_cluster_incremental_incompatible.py` & `s2and-0.23/tests/test_cluster_incremental_incompatible.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_data.py` & `s2and-0.23/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_eval.py` & `s2and-0.23/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_featurizer.py` & `s2and-0.23/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_s2_funcs.py` & `s2and-0.23/tests/test_s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.22/tests/test_text.py` & `s2and-0.23/tests/test_text.py`

 * *Files identical despite different names*

