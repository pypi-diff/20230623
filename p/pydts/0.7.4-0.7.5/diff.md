# Comparing `tmp/pydts-0.7.4.tar.gz` & `tmp/pydts-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydts-0.7.4.tar", max compression
+gzip compressed data, was "pydts-0.7.5.tar", max compression
```

## Comparing `pydts-0.7.4.tar` & `pydts-0.7.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.4/LICENSE
--rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.4/README.md
--rw-r--r--   0        0        0     1418 2023-06-23 19:40:20.475297 pydts-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.4/src/pydts/.DS_Store
--rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.4/src/pydts/__init__.py
--rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.4/src/pydts/base_fitters.py
--rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.4/src/pydts/config.py
--rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.4/src/pydts/cross_validation.py
--rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.4/src/pydts/data_generation.py
--rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.4/src/pydts/datasets/.DS_Store
--rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.4/src/pydts/datasets/LOS_simulated_data.csv
--rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.4/src/pydts/evaluation.py
--rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.4/src/pydts/examples_utils/__init__.py
--rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.4/src/pydts/examples_utils/datasets.py
--rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.4/src/pydts/examples_utils/generate_simulations_data.py
--rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.7.4/src/pydts/examples_utils/mimic_consts.py
--rw-r--r--   0        0        0    33784 2023-06-23 19:40:20.486964 pydts-0.7.4/src/pydts/examples_utils/plots.py
--rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.4/src/pydts/examples_utils/simulations_data_config.py
--rw-r--r--   0        0        0    31476 2023-06-23 19:40:20.471655 pydts-0.7.4/src/pydts/fitters.py
--rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.4/src/pydts/model_selection.py
--rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.4/src/pydts/utils.py
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 pydts-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.5/LICENSE
+-rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.5/README.md
+-rw-r--r--   0        0        0     1441 2023-06-23 20:29:16.430266 pydts-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.5/src/pydts/.DS_Store
+-rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.5/src/pydts/__init__.py
+-rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.5/src/pydts/base_fitters.py
+-rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.5/src/pydts/config.py
+-rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.5/src/pydts/cross_validation.py
+-rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.5/src/pydts/data_generation.py
+-rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.5/src/pydts/datasets/.DS_Store
+-rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.5/src/pydts/datasets/LOS_simulated_data.csv
+-rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.5/src/pydts/evaluation.py
+-rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.5/src/pydts/examples_utils/__init__.py
+-rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.5/src/pydts/examples_utils/datasets.py
+-rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.5/src/pydts/examples_utils/generate_simulations_data.py
+-rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.7.5/src/pydts/examples_utils/mimic_consts.py
+-rw-r--r--   0        0        0    33784 2023-06-23 19:40:20.486964 pydts-0.7.5/src/pydts/examples_utils/plots.py
+-rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.5/src/pydts/examples_utils/simulations_data_config.py
+-rw-r--r--   0        0        0    31476 2023-06-23 19:40:20.471655 pydts-0.7.5/src/pydts/fitters.py
+-rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.5/src/pydts/model_selection.py
+-rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.5/src/pydts/utils.py
+-rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 pydts-0.7.5/PKG-INFO
```

### Comparing `pydts-0.7.4/LICENSE` & `pydts-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/README.md` & `pydts-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/pyproject.toml` & `pydts-0.7.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydts"
-version = "0.7.4"
+version = "0.7.5"
 description = "Discrete time survival analysis with competing risks"
 authors = ["Tomer Meir <tomer1812@gmail.com>", "Rom Gutman <rom.gutman1@gmail.com>", "Malka Gorfine <malkago12@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/tomer1812/pydts"
 repository = "https://github.com/tomer1812/pydts"
 keywords = ["Discrete Time", "Time to Event" ,"Survival Analysis", "Competing Events"]
@@ -22,14 +22,15 @@
 scikit-learn = "^1.0.2"
 tqdm = "^4.63.0"
 statsmodels = "^0.13.2"
 pandarallel = "^1.5.7"
 ipython = "^8.2.0"
 numpy = ">=1.23.4"
 psutil = "^5.9.4"
+setuptools = "^68.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 coverage = {extras = ["toml"], version = "^6.3.2"}
 pytest-cov = "^3.0.0"
 mkdocs = "^1.2.3"
 mkdocs-material = "^8.2.4"
```

### Comparing `pydts-0.7.4/src/pydts/.DS_Store` & `pydts-0.7.5/src/pydts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/base_fitters.py` & `pydts-0.7.5/src/pydts/base_fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/cross_validation.py` & `pydts-0.7.5/src/pydts/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/data_generation.py` & `pydts-0.7.5/src/pydts/data_generation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/datasets/.DS_Store` & `pydts-0.7.5/src/pydts/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/datasets/LOS_simulated_data.csv` & `pydts-0.7.5/src/pydts/datasets/LOS_simulated_data.csv`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/evaluation.py` & `pydts-0.7.5/src/pydts/evaluation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/examples_utils/generate_simulations_data.py` & `pydts-0.7.5/src/pydts/examples_utils/generate_simulations_data.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/examples_utils/mimic_consts.py` & `pydts-0.7.5/src/pydts/examples_utils/mimic_consts.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/examples_utils/plots.py` & `pydts-0.7.5/src/pydts/examples_utils/plots.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/examples_utils/simulations_data_config.py` & `pydts-0.7.5/src/pydts/examples_utils/simulations_data_config.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/fitters.py` & `pydts-0.7.5/src/pydts/fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/model_selection.py` & `pydts-0.7.5/src/pydts/model_selection.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/src/pydts/utils.py` & `pydts-0.7.5/src/pydts/utils.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.4/PKG-INFO` & `pydts-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydts
-Version: 0.7.4
+Version: 0.7.5
 Summary: Discrete time survival analysis with competing risks
 Home-page: https://github.com/tomer1812/pydts
 License: GNU GPLv3
 Keywords: Discrete Time,Time to Event,Survival Analysis,Competing Events
 Author: Tomer Meir
 Author-email: tomer1812@gmail.com
 Requires-Python: >=3.8,<3.11
@@ -21,14 +21,15 @@
 Requires-Dist: mknotebooks (>=0.7.1,<0.8.0)
 Requires-Dist: numpy (>=1.23.4)
 Requires-Dist: pandarallel (>=1.5.7,<2.0.0)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Requires-Dist: setuptools (>=68.0.0,<69.0.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: tqdm (>=4.63.0,<5.0.0)
 Project-URL: Documentation, https://tomer1812.github.io/pydts
 Project-URL: Repository, https://github.com/tomer1812/pydts
 Description-Content-Type: text/markdown
 
 [![pypi version](https://img.shields.io/pypi/v/pydts)](https://pypi.org/project/pydts/)
```

