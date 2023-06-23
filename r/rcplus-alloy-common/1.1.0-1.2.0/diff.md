# Comparing `tmp/rcplus_alloy_common-1.1.0.tar.gz` & `tmp/rcplus_alloy_common-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-1.1.0.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-1.2.0.tar", max compression
```

## Comparing `rcplus_alloy_common-1.1.0.tar` & `rcplus_alloy_common-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       77 2023-05-31 23:19:44.177259 rcplus_alloy_common-1.1.0/LICENSE
--rw-r--r--   0        0        0      571 2023-05-31 23:19:44.177259 rcplus_alloy_common-1.1.0/README.md
--rw-r--r--   0        0        0     1930 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2881 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0      567 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     1652 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0     7448 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0    10104 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0     2611 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     2799 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0     2279 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0     3866 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6388 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     3925 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2023-05-31 23:19:44.181259 rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-06-23 20:29:48.979650 rcplus_alloy_common-1.2.0/LICENSE
+-rw-r--r--   0        0        0      571 2023-06-23 20:29:48.979650 rcplus_alloy_common-1.2.0/README.md
+-rw-r--r--   0        0        0     1951 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2881 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0      567 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     1179 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     1681 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0      703 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/hooks.py
+-rw-r--r--   0        0        0     7448 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    18818 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0     2611 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     2799 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0     2279 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0     3866 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6388 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     3925 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.2.0/PKG-INFO
```

### Comparing `rcplus_alloy_common-1.1.0/README.md` & `rcplus_alloy_common-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.1.0**
+Current version: **v1.2.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-1.1.0/pyproject.toml` & `rcplus_alloy_common-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "1.1.0"
+version = "1.2.0"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
@@ -43,14 +43,15 @@
 black = ">=22.10.0"
 pytest = ">=7.2.0"
 pytest-asyncio = ">=0.10.0"
 pylint-quotes = ">=0.2.0"
 moto = "^4.1.10"
 coverage = "^7.2.6"
 bumpsemver = "*"
+pyparsing = "^3.1.0"
 
 [tool.pylint]
 max-line-length = 120
 
 [tool.pylint.main]
 string-quote = "double"
 triple-quote = "double"
```

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,27 +16,27 @@
         class AlloyBashOperator(BashOperator):
             pass
         ```
     """
     orig_init = cls.__init__
     orig_execute = cls.execute
 
-    def new_init(self, *args, default_args=None, **kwargs):
+    def new_init(self, *args, default_args=None, project_depth=4, **kwargs):
         if default_args is None:
             default_args = {}
         default_args = set_default_callbacks(default_args)
         orig_init(self, *args, default_args=default_args, **kwargs)
 
         # add default outlet if not already added
         dag_id = self.get_dag().dag_id
         dataset_uri = f"{dag_id}-{self.task_id}"
         outlets = any(
             True for outlet in self.get_outlet_defs() if isinstance(outlet, Dataset) and Dataset.uri == dataset_uri
         )
-        self.project = AlloyProject(4)  # __init__, _load_project_config, new_init, apply_defaults, dag_fun
+        self.project = AlloyProject(project_depth)  # __init__, _load_project_config, new_init, apply_defaults, dag_fun
         if not outlets:
             self.add_outlets([Dataset(dataset_uri)])
 
     def new_execute(self, *args, **kwargs):
         self.log.info(f"Running task `{self.task_id}` of dag `{self.dag_id}` with `rcplus_alloy_common@{head_ref}`")
         return orig_execute(self, *args, **kwargs)
```

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/airflow/utils.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/logging.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/logging.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.1.0/PKG-INFO` & `rcplus_alloy_common-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcplus-alloy-common
-Version: 1.1.0
+Version: 1.2.0
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
@@ -29,15 +29,15 @@
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.1.0**
+Current version: **v1.2.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

