# Comparing `tmp/cluster_experiments-0.9.0.tar.gz` & `tmp/cluster_experiments-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluster_experiments-0.9.0.tar", last modified: Fri May 26 08:05:02 2023, max compression
+gzip compressed data, was "cluster_experiments-0.9.1.tar", last modified: Fri May 26 12:22:54 2023, max compression
```

## Comparing `cluster_experiments-0.9.0.tar` & `cluster_experiments-0.9.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.590408 cluster_experiments-0.9.0/cluster_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/cupac.py
--rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29720 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/perturbator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/power_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/power_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/random_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/washover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/cluster_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/analysis/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/cupac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/cupac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/cupac/test_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/perturbator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/perturbator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/power_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_time_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_washover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/test_non_clustered.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.973332 cluster_experiments-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-26 12:22:54.973332 cluster_experiments-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.965332 cluster_experiments-0.9.1/cluster_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/cupac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29780 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/perturbator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/power_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/random_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/cluster_experiments/washover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.969332 cluster_experiments-0.9.1/cluster_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-26 12:22:54.000000 cluster_experiments-0.9.1/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-26 12:22:54.000000 cluster_experiments-0.9.1/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:22:54.000000 cluster_experiments-0.9.1/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-26 12:22:54.000000 cluster_experiments-0.9.1/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 12:22:54.000000 cluster_experiments-0.9.1/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:22:54.973332 cluster_experiments-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.969332 cluster_experiments-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.969332 cluster_experiments-0.9.1/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/analysis/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.969332 cluster_experiments-0.9.1/tests/cupac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/cupac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/cupac/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.969332 cluster_experiments-0.9.1/tests/perturbator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/perturbator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.973332 cluster_experiments-0.9.1/tests/power_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:22:54.973332 cluster_experiments-0.9.1/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/splitter/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/splitter/test_time_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/splitter/test_washover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/test_non_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-26 12:21:35.000000 cluster_experiments-0.9.1/tests/utils.py
```

### Comparing `cluster_experiments-0.9.0/LICENSE` & `cluster_experiments-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/PKG-INFO` & `cluster_experiments-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster_experiments
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.9.0/README.md` & `cluster_experiments-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments/__init__.py` & `cluster_experiments-0.9.1/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments/cupac.py` & `cluster_experiments-0.9.1/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.9.1/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments/perturbator.py` & `cluster_experiments-0.9.1/cluster_experiments/perturbator.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,22 +413,22 @@
     def __init__(
         self,
         average_effect: Optional[float] = None,
         target_col: str = "target",
         treatment_col: str = "treatment",
         treatment: str = "B",
         scale: Optional[float] = None,
-        range_min: float = -0.8,
-        range_max: float = 4,
+        range_min: Optional[float] = None,
+        range_max: Optional[float] = None,
         reduce_variance: Optional[bool] = None,
     ):
         self._check_range(range_min, range_max)
         super().__init__(average_effect, target_col, treatment_col, treatment, scale)
-        self._range_min = range_min
-        self._range_max = range_max
+        self._range_min = range_min or -0.8
+        self._range_max = range_max or 4
         self._reduce_variance = reduce_variance or True
 
     def perturbate(
         self, df: pd.DataFrame, average_effect: Optional[float] = None
     ) -> pd.DataFrame:
         """
         Usage:
@@ -559,20 +559,20 @@
         self,
         segment_cols: List[str],
         average_effect: Optional[float] = None,
         target_col: str = "target",
         treatment_col: str = "treatment",
         treatment: str = "B",
         scale: Optional[float] = None,
-        range_min: float = -0.8,
-        range_max: float = 4,
+        range_min: Optional[float] = None,
+        range_max: Optional[float] = None,
     ):
         super().__init__(average_effect, target_col, treatment_col, treatment, scale)
-        self._range_min = range_min
-        self._range_max = range_max
+        self._range_min = range_min or -0.8
+        self._range_max = range_max or 4
         self._segment_cols = segment_cols
         self.segment_col = self._get_segment_col_name(segment_cols)
 
     @staticmethod
     def _get_segment_col_name(segment_cols: List[str]):
         if not isinstance(segment_cols, list):
             raise ValueError(
@@ -644,15 +644,15 @@
             average_effect=config.average_effect,
             target_col=config.target_col,
             treatment_col=config.treatment_col,
             treatment=config.treatment,
             scale=config.scale,
             range_min=config.range_min,
             range_max=config.range_max,
-            segment_cols=config.segment_cols_perturbator,
+            segment_cols=config.segment_cols,
         )
 
 
 class BinaryPerturbator(Perturbator):
     """
     BinaryPerturbator is a Perturbator that adds is used to deal with binary outcome variables.
     It randomly selects some treated instances and flips their outcome from 0 to 1 or 1 to 0, depending on the effect being positive or negative
```

### Comparing `cluster_experiments-0.9.0/cluster_experiments/power_analysis.py` & `cluster_experiments-0.9.1/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments/power_config.py` & `cluster_experiments-0.9.1/cluster_experiments/power_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,23 +147,23 @@
             if self._are_different(self.time_col, None):
                 self._set_and_log("time_col", None, "splitter")
 
         if self.perturbator not in {"normal", "beta_relative_positive"}:
             if self._are_different(self.scale, None):
                 self._set_and_log("scale", None, "perturbator")
 
-        if self.perturbator not in {"beta_relative", "clustered_beta_relative"}:
+        if self.perturbator not in {"beta_relative", "segmented_beta_relative"}:
             if self._are_different(self.range_min, None):
                 self._set_and_log("range_min", None, "perturbator")
             if self._are_different(self.range_max, None):
                 self._set_and_log("range_max", None, "perturbator")
             if self._are_different(self.reduce_variance, None):
                 self._set_and_log("reduce_variance", None, "perturbator")
 
-        if self.perturbator not in {"clustered_beta_relative"}:
+        if self.perturbator not in {"segmented_beta_relative"}:
             if self._are_different(self.segment_cols, None):
                 self._set_and_log("segment_cols", None, "perturbator")
 
         if "stratified" not in self.splitter and "paired_ttest" not in self.analysis:
             if self._are_different(self.strata_cols, None):
                 self._set_and_log("strata_cols", None, "splitter")
 
@@ -210,15 +210,15 @@
     "clustered": ClusteredSplitter,
     "clustered_balance": BalancedClusteredSplitter,
     "non_clustered": NonClusteredSplitter,
     "clustered_stratified": StratifiedClusteredSplitter,
     "switchback": SwitchbackSplitter,
     "switchback_balance": BalancedSwitchbackSplitter,
     "switchback_stratified": StratifiedSwitchbackSplitter,
-    "backtest": RepeatedSampler,
+    "repeated_sampler": RepeatedSampler,
 }
 
 analysis_mapping = {
     "gee": GeeExperimentAnalysis,
     "ols_non_clustered": OLSAnalysis,
     "ols_clustered": ClusteredOLSAnalysis,
     "ttest_clustered": TTestClusteredAnalysis,
```

### Comparing `cluster_experiments-0.9.0/cluster_experiments/random_splitter.py` & `cluster_experiments-0.9.1/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments/washover.py` & `cluster_experiments-0.9.1/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments.egg-info/PKG-INFO` & `cluster_experiments-0.9.1/cluster_experiments.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-experiments
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.9.0/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.9.1/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.9.1/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/setup.py` & `cluster_experiments-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.9.0",
+    version="0.9.1",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.9.0/tests/analysis/test_analysis.py` & `cluster_experiments-0.9.1/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/cupac/test_aggregator.py` & `cluster_experiments-0.9.1/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.9.1/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/examples.py` & `cluster_experiments-0.9.1/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.9.1/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/conftest.py` & `cluster_experiments-0.9.1/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.9.1/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.9.1/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.9.1/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.9.1/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.9.1/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/test_seed.py` & `cluster_experiments-0.9.1/tests/power_analysis/test_seed.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.9.1/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/splitter/conftest.py` & `cluster_experiments-0.9.1/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/splitter/test_splitter.py` & `cluster_experiments-0.9.1/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.9.1/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/splitter/test_time_col.py` & `cluster_experiments-0.9.1/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/splitter/test_washover.py` & `cluster_experiments-0.9.1/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/test_docs.py` & `cluster_experiments-0.9.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/test_non_clustered.py` & `cluster_experiments-0.9.1/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.9.0/tests/utils.py` & `cluster_experiments-0.9.1/tests/utils.py`

 * *Files identical despite different names*

