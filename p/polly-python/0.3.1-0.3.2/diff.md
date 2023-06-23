# Comparing `tmp/polly-python-0.3.1.tar.gz` & `tmp/polly-python-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polly-python-0.3.1.tar", last modified: Thu May 18 06:31:08 2023, max compression
+gzip compressed data, was "polly-python-0.3.2.tar", last modified: Fri Jun 23 05:14:37 2023, max compression
```

## Comparing `polly-python-0.3.1.tar` & `polly-python-0.3.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.262608 polly-python-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-18 06:29:34.000000 polly-python-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 06:29:34.000000 polly-python-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-18 06:31:08.262608 polly-python-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-18 06:29:34.000000 polly-python-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.258608 polly-python-0.3.1/polly/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/application_error_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/bridge_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/core_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    34051 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/http_response_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/index_schema_level_conversion_const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)   193661 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    67169 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/omixatlas_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/validation_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-05-18 06:29:34.000000 polly-python-0.3.1/polly/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.262608 polly-python-0.3.1/polly_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 06:31:08.000000 polly-python-0.3.1/polly_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 06:29:34.000000 polly-python-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-18 06:31:08.266608 polly-python-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:29:34.000000 polly-python-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:31:08.262608 polly-python-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    90818 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_schema_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-18 06:29:34.000000 polly-python-0.3.1/tests/test_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.420019 polly-python-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-06-23 05:13:10.000000 polly-python-0.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 05:13:10.000000 polly-python-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 05:14:37.420019 polly-python-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-23 05:13:10.000000 polly-python-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.416018 polly-python-0.3.2/polly/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/application_error_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/bridge_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31214 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/core_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20886 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35626 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/http_response_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/index_schema_level_conversion_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198255 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73864 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/omixatlas_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/validation_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-06-23 05:13:10.000000 polly-python-0.3.2/polly/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.420019 polly-python-0.3.2/polly_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 05:14:37.000000 polly-python-0.3.2/polly_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 05:13:10.000000 polly-python-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-23 05:14:37.420019 polly-python-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 05:13:10.000000 polly-python-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:14:37.420019 polly-python-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98539 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_schema_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-23 05:13:10.000000 polly-python-0.3.2/tests/test_workspaces.py
```

### Comparing `polly-python-0.3.1/LICENSE.md` & `polly-python-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/PKG-INFO` & `polly-python-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.3.1
+Version: 0.3.2
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
-Requires-Python: >=3.6
+Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 ![code-coverage](https://github.com/ElucidataInc/polly-python-code/blob/badges_do_not_delete/badges/badge.svg)
 ![Linting](https://img.shields.io/badge/Linting-Black-green)
```

### Comparing `polly-python-0.3.1/README.md` & `polly-python-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/application_error_info.py` & `polly-python-0.3.2/polly/application_error_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,8 +112,11 @@
 000006f0: 746f 7269 6e67 2064 6173 6862 6f61 7264  toring dashboard
 00000700: 2066 6f72 2076 6973 6962 696c 6974 7920   for visibility 
 00000710: 6f6e 2074 6869 7320 7072 6f63 6573 732e  on this process.
 00000720: 2022 0a20 2020 202b 2022 4f6e 6365 2063   ".    + "Once c
 00000730: 6f6d 706c 6574 6564 2c20 796f 7520 6361  ompleted, you ca
 00000740: 6e20 6564 6974 2079 6f75 7220 6461 7461  n edit your data
 00000750: 7365 7473 206f 7220 7363 6865 6d61 2e20  sets or schema. 
-00000760: 220a 290a                                ".).
+00000760: 220a 290a 0a50 4159 4c4f 4144 5f4d 4158  ".)..PAYLOAD_MAX
+00000770: 5f4f 5554 5f54 4954 4c45 203d 2022 5061  _OUT_TITLE = "Pa
+00000780: 796c 6f61 6420 746f 6f20 6c61 7267 6522  yload too large"
+00000790: 0a                                       .
```

### Comparing `polly-python-0.3.1/polly/auth.py` & `polly-python-0.3.2/polly/auth.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/bridge_cohort.py` & `polly-python-0.3.2/polly/bridge_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/cohort.py` & `polly-python-0.3.2/polly/cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/constants.py` & `polly-python-0.3.2/polly/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,25 @@
                 {"name": "tcga", "header_mapping": {}},
             ],
         }
     ]
 }
 COHORT_SUPPORTED_DATATYPES = ["Raw Counts Transcriptomics"]
 COHORT_SUPPORTED_DATASOURCES = ["GEO"]
+COHORT_LIST_COLS_TO_DROP = [
+    "sample_characteristics",
+    "timestamp_",
+    "curated_control",
+    "curated_cohort_id",
+    "curated_cohort_name",
+    "curated_is_control",
+    "curated_max_age",
+    "curated_min_age",
+    "curated_age_unit",
+]
 
 # validation flow files url github
 VALIDATION_FLOW_FILES_URL = (
     "https://raw.githubusercontent.com/ElucidataInc/PublicAssets/master/"
     + "internal-user/validation_full_flow_files"
 )
 
@@ -118,14 +129,16 @@
 
 FILES_PATH_FORMAT = {"metadata": "<metadata_path>", "data": "<data_path>"}
 
 INGESTION_FILES_PATH_DIR_NAMES = ["metadata", "data"]
 
 SCHEMA_CONFIG_KEY_NAMES = ["source", "datatype"]
 
+VALIDATION_SCOPE_CONSTANTS = ["basic", "advanced"]
+
 SCHEMA_CONFIG_FORMAT = {"source": "<source_name", "datatype": "<datatype_name>"}
 
 FORMATTED_METADATA = {"id": "", "type": "", "attributes": {}}
 
 FILE_FORMAT_CONSTANTS_URL = (
     "https://elucidatainc.github.io/PublicAssets/file_format_constants.txt"
 )
@@ -559,21 +572,39 @@
         "gpuxlarge": "8 GPU, 96 vCPU, 760GB RAM",
     },
 )
 
 DATA_LOG_MODES = ["latest", "all"]
 MIXPANEL_KEY = "91fa77fcf07f7b672b5c5c6c09d8a14c"
 
+PROD_ENV_NAME = "polly"
+
 POLLY_PYTHON_PYPI_URL = "https://pypi.python.org/pypi/polly-python/json"
 ERROR_MSG_GET_METADATA = "Argument 'table_name' not valid, please query 'SHOW TABLES IN repo_name' \
 using query_metadata function and pick the appropriate table name you want the metadata \
 for Example: samples, features, samples_singlecell etc. \
 Currently, get_metadata works only for sample level table of gct and h5ad files. \
 If you want to get metadata for other tables, please contact polly.support@elucidata.io"
 
 TABLE_NAME_SAMPLE_LEVEL_INDEX_MAP = {
     "samples": "gct_col_metadata",
     "samples_singlecell": "h5ad_col_metadata",
 }
 POLLY_PYTHON_LATEST_VERSION_FILE = (
     "https://elucidatainc.github.io/PublicAssets/polly_python_latest_version.txt"
 )
+
+QUERY_MAX_RECORD_SIZE = 20000
+# this control lever is for testing as data is less on testpolly
+DEFAULT_PAGE_SIZE_LIST_FILES = 2600
+
+DEFAULT_PAGE_SIZE_LIST_FILES_KEY_NAME = "default_page_size_list_files"
+
+PAGE_REDUCTION_PERCENTAGE_LIST_FILES = 20
+
+PAGE_REDUCTION_PERCENTAGE_LIST_FILES_KEY_NAME = "page_reduction_percentage_list_files"
+
+LIST_FILE_API_CONTROL_LEVER_LINK = (
+    "https://elucidatainc.github.io/PublicAssets/list_files_api_control_lever/"
+    + "list_files_control_lever.json"
+)
+QUERY_API_V2 = "v2"
```

### Comparing `polly-python-0.3.1/polly/core_cohort.py` & `polly-python-0.3.2/polly/core_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/curation.py` & `polly-python-0.3.2/polly/curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/errors.py` & `polly-python-0.3.2/polly/errors.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/help.py` & `polly-python-0.3.2/polly/help.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/helpers.py` & `polly-python-0.3.2/polly/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from polly.constants import COHORT_CONSTANTS_URL, REPORT_FIELDS_URL, ELUCIDATA_LOGO_URL
 from bs4 import BeautifulSoup
 import contextlib
 import joblib
 import urllib
 import pandas as pd
 import polly.http_response_codes as http_codes
+from polly.tracking import Track
+import polly.constants as const
 
 
 def get_platform_value_from_env(
     variable: str, default_val: str, passed_val: str
 ) -> str:
     """
     Get variable value of passed variable
@@ -55,14 +57,40 @@
     if not prefix:
         raise InvalidParameterException("prefix")
     if not postfix:
         raise InvalidParameterException("postfix")
     return os.path.normpath(f"{prefix}/{postfix}")
 
 
+def debug_print(self, val: str):
+    """Helper function to show prints in test and dev environment
+
+    Args:
+        self (polly_session_object): polly_session
+        val (str): value to be printed
+    """
+    if self.session.env != const.PROD_ENV_NAME:
+        print(val)
+
+
+@Track.track_decorator
+def debug_logger(self, properties: dict):
+    """Track an event but calling the debug logger with properties
+    that needs to be tracked
+    For Example :-
+    If I need to track the Crash of an API and properties related to it
+    like which API is crashing, for which page size it crashed and other
+    relevant details
+
+    Args:
+        properties (dict): Properties of the event which is tracked
+    """
+    return properties
+
+
 def get_sts_creds(sts_dict: dict) -> dict:
     """
     Function to check and return temporary sts creds
     """
     if sts_dict and isinstance(sts_dict, dict):
         if "data" in sts_dict:
             data = sts_dict.get("data")
@@ -1027,7 +1055,31 @@
     """
     Function to remove prefix from text.
     """
     if text.startswith(prefix):
         slice_obj = slice(len(prefix), len(text))
         return text[slice_obj]
     return text
+
+
+def find_between(s, first, last) -> str:
+    """Function to find the elements between first and last boundary elements
+    Using this function, a substring can be extract which is between two elements
+    first and last
+    Reference
+    https://stackoverflow.com/questions/3368969/find-string-between-two-substrings
+
+    Args:
+        s (str): main string from
+        first (str): first boundary elements
+        last (str): last boundary elements
+
+    Returns:
+        str: substring b/w boundary elements
+    """
+    try:
+        start = s.index(first) + len(first)
+        end = s.index(last, start)
+        return s[start:end]
+    except ValueError:
+        # write proper error message here
+        raise Exception("Error extracting substring. Please contact admin")
```

### Comparing `polly-python-0.3.1/polly/http_response_codes.py` & `polly-python-0.3.2/polly/http_response_codes.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/jobs.py` & `polly-python-0.3.2/polly/jobs.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/omixatlas.py` & `polly-python-0.3.2/polly/omixatlas.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import platform
 import tempfile
 import boto3
 from boto3.s3.transfer import TransferConfig
 from boto3.exceptions import S3UploadFailedError
 from tempfile import TemporaryDirectory as TempDir
 from pathlib import Path
-from typing import Union, Dict
+from typing import Dict, Generator, Union
 from collections import namedtuple
 import xml.etree.ElementTree as ET
 import pandas as pd
 import time
 from joblib import Parallel, delayed
 import requests
 from retrying import retry
@@ -63,17 +63,14 @@
 
 import polly.omixatlas_hlpr as omix_hlpr
 
 import polly.http_response_codes as http_codes
 from polly.schema import check_schema_for_errors
 from polly.tracking import Track
 
-QUERY_API_V1 = "v1"
-QUERY_API_V2 = "v2"
-
 
 class OmixAtlas:
     """
     OmixAtlas class enables users to interact with functional properties of the omixatlas such as \
     create and update an Omixatlas, get summary of it's contents, add, insert, update the schema, \
     add, update or delete datasets, query metadata, download data, save data to workspace etc.\
 
@@ -271,92 +268,117 @@
             )
 
     @Track.track_decorator
     def query_metadata(
         self,
         query: str,
         experimental_features=None,
-        query_api_version=QUERY_API_V2,
-        page_size=None,  # Note: do not increase page size more than 999
-    ):
+    ) -> pd.DataFrame:
         """
         This function will return a dataframe containing the SQL response.
+        In cases of data intensive queries, the data returned can be very large to process and it might lead to kernel failure\
+        , where in the runtime memory is exhausted and the process haults.
+        In order to access the data, there are two options in this case, either increase the kernel memory, \
+        or use the function query_metadata_iterator() that returns an iterator.
+        The function usage can be looked up in the documentation mentioned here under the \
+        Polly Python section - "https://docs.elucidata.io/index.html".
 
         Args:
-           query (str) : sql query  on  omixatlas.
+           query (str): sql query  on  omixatlas.
            experimental_features : this section includes in querying metadata <target>.
-           query_api_version (str) : v1 or v2.
-           page_size (int): page size for query.
 
         Returns:
             It will return a dataframe that contains the query response.
 
         Raises:
             UnfinishedQueryException: when query has not finised the execution.
             QueryFailedException: when query failed to execute.
         """
+        query_id = self._get_query_id(query, experimental_features)
+        iterator_function = False
+        return self._process_query_to_completion(query_id, iterator_function)
 
-        max_page_size = 999
-        if page_size is not None and page_size > max_page_size:
-            raise ValueError(
-                f"The maximum permitted value for page_size is {max_page_size}"
-            )
-        elif page_size is None and query_api_version != QUERY_API_V2:
-            page_size = 500
+    @Track.track_decorator
+    def query_metadata_iterator(
+        self,
+        query: str,
+        experimental_features=None,
+    ) -> Generator[dict, None, None]:
+        """
+        This function will return a Generator object containing the SQL response.
+
+        Args:
+           query (str) : sql query  on  omixatlas.
+           experimental_features : this section includes in querying metadata <target>.
+
+        Returns:
+            It will return a generator object having the SQL response.
 
+        Raises:
+            UnfinishedQueryException: when query has not finised the execution.
+            QueryFailedException: when query failed to execute.
+        """
+        query_id = self._get_query_id(query, experimental_features)
+        iterator_function = True
+        return self._process_query_to_completion(query_id, iterator_function)
+
+    def _get_query_id(self, query, experimental_features) -> str:
+        """
+        Function to return query_id for the respective SQL query.
+        """
         queries_url = f"{self.resource_url}/queries"
         queries_payload = {
             "data": {
                 "type": "queries",
                 "attributes": {
                     "query": query,
-                    "query_api_version": query_api_version,
+                    "query_api_version": const.QUERY_API_V2,
                     "query_results_format": "JSON",
                 },
             }
         }
         if experimental_features is not None:
             queries_payload.update({"experimental_features": experimental_features})
 
         response = self.session.post(queries_url, json=queries_payload)
         error_handler(response)
 
         query_data = response.json().get("data")
         query_id = query_data.get("id")
-        return self._process_query_to_completion(query_id, query_api_version, page_size)
+        return query_id
 
     @retry(
         retry_on_exception=is_unfinished_query_error,
         wait_exponential_multiplier=500,  # Exponential back-off starting 500ms
         wait_exponential_max=10000,  # After 10s, retry every 10s
         stop_max_delay=900000,  # Stop retrying after 900s (15m)
     )
     def _process_query_to_completion(
-        self, query_id: str, query_api_version: str, page_size: Union[int, None]
-    ):
+        self, query_id: str, iterator_function: bool
+    ) -> Union[pd.DataFrame, Generator[dict, None, None]]:
         queries_url = f"{self.resource_url}/queries/{query_id}"
         response = self.session.get(queries_url)
         error_handler(response)
 
         query_data = response.json().get("data")
         query_status = query_data.get("attributes", {}).get("status")
         if query_status == "succeeded":
-            return self._handle_query_success(query_data, query_api_version, page_size)
+            return self._handle_query_success(query_data, iterator_function)
         elif query_status == "failed":
             self._handle_query_failure(query_data)
         else:
             raise UnfinishedQueryException(query_id)
 
     def _handle_query_failure(self, query_data: dict):
         fail_msg = query_data.get("attributes").get("failure_reason")
         raise QueryFailedException(fail_msg)
 
     def _handle_query_success(
-        self, query_data: dict, query_api_version: str, page_size: Union[int, None]
-    ) -> pd.DataFrame:
+        self, query_data: dict, iterator_function: bool
+    ) -> Union[pd.DataFrame, Generator[dict, None, None]]:
         query_id = query_data.get("id")
 
         details = []
         time_taken_in_ms = query_data.get("attributes").get("exec_time_ms")
         if isinstance(time_taken_in_ms, int):
             details.append("time taken: {:.2f} seconds".format(time_taken_in_ms / 1000))
         data_scanned_in_bytes = query_data.get("attributes").get("data_scanned_bytes")
@@ -367,20 +389,51 @@
 
         if details:
             detail_str = ", ".join(details)
             print("Query execution succeeded " f"({detail_str})")
         else:
             print("Query execution succeeded")
 
-        if query_api_version != QUERY_API_V2 or page_size is not None:
-            return self._fetch_results_as_pages(query_id, page_size)
-        else:
-            return self._fetch_results_as_file(query_id)
+        return self._fetch_results_as_file(query_id, iterator_function)
 
-    def _fetch_results_as_pages(self, query_id, page_size):
+    def _fetch_iterator_as_pages(
+        self, query_id, page_size
+    ) -> Generator[dict, None, None]:
+        """
+        Function to return generator for SHOW/DESC queries that is only possible using page_size.
+        """
+        first_page_url = (
+            f"{self.resource_url}/queries/{query_id}" f"/results?page[size]={page_size}"
+        )
+        response = self.session.get(first_page_url)
+        error_handler(response)
+        result_data = response.json()
+        rows = [row_data.get("attributes") for row_data in result_data.get("data")]
+        # yielding data for the first time call
+        for row in rows:
+            yield row
+
+        while (
+            result_data.get("links") is not None
+            and result_data.get("links").get("next") is not None
+            and result_data.get("links").get("next") != "null"
+        ):
+            # subsequent call for next paginated data, if any
+            next_page_url = self.base_url + result_data.get("links").get("next")
+            response = self.session.get(next_page_url)
+            error_handler(response)
+            result_data = response.json()
+            if result_data.get("data"):
+                rows = [
+                    row_data.get("attributes") for row_data in result_data.get("data")
+                ]
+                for row in rows:
+                    yield row
+
+    def _fetch_results_as_pages(self, query_id, page_size) -> pd.DataFrame:
         first_page_url = (
             f"{self.resource_url}/queries/{query_id}" f"/results?page[size]={page_size}"
         )
         response = self.session.get(first_page_url)
         error_handler(response)
         result_data = response.json()
         rows = [row_data.get("attributes") for row_data in result_data.get("data")]
@@ -428,50 +481,89 @@
 
         temp_file_path = os.path.join(temp_dir, filename)
         if Path(temp_file_path).exists():
             os.remove(temp_file_path)
 
         return temp_file_path
 
-    def _extract_results_from_download_urls(self, download_urls):
+    def _extract_results_from_download_urls(self, download_urls) -> pd.DataFrame:
         # Function to pull out & combine results from the list of Download URLS
-        results = []
-        for url in download_urls:
-            r = requests.get(url, allow_redirects=True)
-            name = self._get_root_loc_from_url(url)
-            filename = self._local_temp_file_path(name)
-            with open(filename, "wb") as f:
-                f.write(r.content)
+        query_metadata_df = pd.DataFrame()
+        files = Parallel(n_jobs=-1, require="sharedmem")(
+            delayed(self._write_single_gzip_file)(url) for url in download_urls
+        )
+        temp_records = []
+        for filename in files:
             with gzip.open(filename, "rt", encoding="utf-8") as fgz:
                 for line in fgz:
-                    results.append(json.loads(line))
-
-        df = pd.DataFrame.from_records(results)
-        print(f"Fetched {len(df.index)} rows")
-        return df
+                    data = json.loads(line)
+                    temp_records.append(data)
+                    if len(temp_records) == const.QUERY_MAX_RECORD_SIZE:
+                        new_df = pd.DataFrame.from_records(temp_records)
+                        query_metadata_df = pd.concat(
+                            [query_metadata_df, new_df], ignore_index=True
+                        )
+                        temp_records.clear()
+        df = pd.DataFrame.from_records(temp_records)
+        query_metadata_df = pd.concat([query_metadata_df, df], ignore_index=True)
+        print(f"Fetched {len(query_metadata_df.index)} rows")
+        return query_metadata_df
+
+    def _write_single_gzip_file(self, url) -> str:
+        """
+        Function that writes content of a file and returns the filename.
+        """
+        r = requests.get(url, allow_redirects=True)
+        name = self._get_root_loc_from_url(url)
+        filename = self._local_temp_file_path(name)
+        with open(filename, "wb") as f:
+            f.write(r.content)
+        return filename
+
+    def _generator_function_for_download_urls(
+        self, download_urls: list
+    ) -> Generator[dict, None, None]:
+        """
+        Function to return an iterable object, that yields files one line at a time downloaded from the list of download_urls.
+        """
+        files = Parallel(n_jobs=-1, require="sharedmem")(
+            delayed(self._write_single_gzip_file)(url) for url in download_urls
+        )
+        for filename in files:
+            with gzip.open(filename, "rt", encoding="utf-8") as fgz:
+                for line in fgz:
+                    sorted_json = omix_hlpr.return_sorted_dict(json.loads(line))
+                    yield sorted_json
 
-    def _fetch_results_as_file(self, query_id):
+    def _fetch_results_as_file(
+        self, query_id: str, iterator_function: bool
+    ) -> Union[pd.DataFrame, Generator[dict, None, None]]:
         results_file_req_url = (
             f"{self.resource_url}/queries/{query_id}/results?action=download"
         )
         response = self.session.get(results_file_req_url)
         error_handler(response)
         result_data = response.json()
 
         results_file_download_url = result_data.get("data", {}).get("download_url")
-        if (
-            results_file_download_url is None
-            or results_file_download_url == "Not available"
-        ):
+        if results_file_download_url in [None, "Not available"]:
             # The user is probably executing SHOW TABLES or DESCRIBE query
-            return self._fetch_results_as_pages(query_id, 100)
+            if iterator_function:
+                return self._fetch_iterator_as_pages(query_id, 100)
+            else:
+                return self._fetch_results_as_pages(query_id, 100)
         else:
             pd.set_option("display.max_columns", None)
-            df = self._extract_results_from_download_urls(results_file_download_url)
-            return self._get_sorted_col_df(df)
+            if iterator_function:
+                return self._generator_function_for_download_urls(
+                    results_file_download_url
+                )
+            else:
+                df = self._extract_results_from_download_urls(results_file_download_url)
+                return self._get_sorted_col_df(df)
 
     def _get_sorted_col_df(self, results_dataframe):
         """
         Function to sort a dataframe columnwise. Primarily being used before returning the
         query_metadata result dataframe.
 
         ``Args:``
@@ -1578,14 +1670,15 @@
         Link a workspace ID given by the user to an OmixAtlas. Called by the update() function.
         Args:
             repo_key (str): repo_name/repo_id for that Omixatlas
             workspace_id (str): ID of the Workspace to be linked to the Omixatlas
         """
         url = f"{self.discover_url}/repositories/{repo_key}"
         get_response = self.session.get(url)
+        error_handler(get_response)
         get_response = get_response.json()
         get_response["data"]["attributes"]["linked_workspace_id"] = workspace_id
         get_response["data"]["attributes"].pop("repo_name")
         patch_response = self.session.patch(url, data=json.dumps(get_response))
         error_handler(patch_response)
         if patch_response.status_code != const.OK:
             raise Exception(patch_response.text)
@@ -2217,41 +2310,44 @@
                 data_source_folder_path,
                 destination_folder_path,
                 file_status_dict,
                 data_metadata_mapping,
             )
             # iterating the status dict
             # generating appropriate messages
-            result_list = self._generating_response_from_status_dict(
-                file_status_dict, result_list
-            )
+            data_upload_results_df = pd.DataFrame()
 
-            # printing the dataframe
-            data_upload_results_df = pd.DataFrame(
-                result_list, columns=["File Name", "Message"]
-            )
-
-            # print message before delay
-            print(const.WAIT_FOR_COMMIT)
-            # delay added after the files are uploaded
-            # before commit API is hit
-            time.sleep(30)
-
-            # informing infra to commit the uploaded data in the repository
-            self._commit_data_to_repo(repo_id)
-
-            with pd.option_context(
-                "display.max_rows",
-                800,
-                "display.max_columns",
-                800,
-                "display.width",
-                1200,
-            ):
-                print("\n", data_upload_results_df)
+            if file_status_dict:
+                result_list = self._generating_response_from_status_dict(
+                    file_status_dict, result_list
+                )
+
+                # printing the dataframe
+                data_upload_results_df = pd.DataFrame(
+                    result_list, columns=["File Name", "Message"]
+                )
+
+                # print message before delay
+                print(const.WAIT_FOR_COMMIT)
+                # delay added after the files are uploaded
+                # before commit API is hit
+                time.sleep(30)
+
+                # informing infra to commit the uploaded data in the repository
+                self._commit_data_to_repo(repo_id)
+
+                with pd.option_context(
+                    "display.max_rows",
+                    800,
+                    "display.max_columns",
+                    800,
+                    "display.width",
+                    1200,
+                ):
+                    print("\n", data_upload_results_df)
 
             if validation:
                 print("\n")
                 print("-----Files which are Not Validated-------")
                 helpers.display_df_from_list(
                     omix_hlpr.dataset_level_metadata_files_not_uploaded,
                     "Invalid Metadata Files",
@@ -2368,14 +2464,17 @@
                 priority,
                 final_data_metadata_mapping_dict,
                 validation_dataset_lvl,
             )
         except Exception as err:
             raise err
 
+        # intialising empty df
+        data_upload_results_df = pd.DataFrame()
+
         if file_status_dict:
             result_list = self._generating_response_from_status_dict(
                 file_status_dict, result_list
             )
 
             # printing the dataframe
             data_upload_results_df = pd.DataFrame(
@@ -2393,33 +2492,33 @@
             self._commit_data_to_repo(repo_id)
 
             with pd.option_context(
                 "display.max_rows", None, "display.max_columns", None
             ):
                 print("\n", data_upload_results_df)
 
-            if validation:
-                print("\n")
-                print("-----Files which are Not Validated-------")
-                helpers.display_df_from_list(
-                    omix_hlpr.dataset_level_metadata_files_not_uploaded,
-                    "Invalid Metadata Files",
-                )
-                print("\n")
-                helpers.display_df_from_list(
-                    omix_hlpr.data_files_whose_metadata_failed_validation,
-                    "Invalid Data Files",
-                )
-
-            # reset global variables storing validation results
-            # flushes out the previous state of variables and creates
-            # new state
-            omix_hlpr.reset_global_variables_with_validation_results()
+        if validation:
+            print("\n")
+            print("-----Files which are Not Validated-------")
+            helpers.display_df_from_list(
+                omix_hlpr.dataset_level_metadata_files_not_uploaded,
+                "Invalid Metadata Files",
+            )
+            print("\n")
+            helpers.display_df_from_list(
+                omix_hlpr.data_files_whose_metadata_failed_validation,
+                "Invalid Data Files",
+            )
+
+        # reset global variables storing validation results
+        # flushes out the previous state of variables and creates
+        # new state
+        omix_hlpr.reset_global_variables_with_validation_results()
 
-            return data_upload_results_df
+        return data_upload_results_df
 
     def _check_destination_folder(self, destination_folder_path: str, repo_id: str):
         """Check if the destination folder passed in the parameter, if that is valid destination
         folder.
         Destination folder is a valid destination folder
         When it is returned as a response of list files API in OA in the file_id key
         Merely being a folder present in the s3 bucket of the OA does not make it valid
@@ -2978,16 +3077,18 @@
         # For these files deletion will be skipped
         # This is to ease out the process of Bulk Delete
 
         # iterating over list_files_resp_list to get all the list of files
         for list_files_resp in list_files_resp_list:
             if list_files_resp.status_code != const.OK and internal_call:
                 if list_files_resp.status_code == http_codes.NOT_FOUND:
-                    error_msg = omix_hlpr.extract_error_message(list_files_resp.text)
-                    return error_msg
+                    error_msg_dict = omix_hlpr.extract_error_message(
+                        list_files_resp.text
+                    )
+                    return error_msg_dict.get("detail", "")
             elif list_files_resp.status_code != const.OK:
                 error_handler(list_files_resp)
             else:
                 list_files_resp = list_files_resp.json()
                 list_files_resp_data = list_files_resp.get("data", [])
                 for file_data in list_files_resp_data:
                     file_metadata = file_data.get("attributes", {}).get("metadata", {})
```

### Comparing `polly-python-0.3.1/polly/omixatlas_hlpr.py` & `polly-python-0.3.2/polly/omixatlas_hlpr.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,44 @@
     if not (dataset_id and isinstance(dataset_id, str)):
         raise paramException(
             title="Param Error",
             detail="Argument 'dataset_id' is either empty or invalid. It should be a string. Please try again.",
         )
 
 
+def parameter_check_for_list_dataset_ids(dataset_ids):
+    """Checking for validity of repo id
+    Args:
+        dataset_id (): Dataset Id of the dataset
+
+    Raises:
+        paramException: Error if dataset id is empty or is not str
+    """
+    if not (dataset_ids and isinstance(dataset_ids, list)):
+        raise paramException(
+            title="Param Error",
+            detail="dataset_ids should be list of strings",
+        )
+
+
+def str_params_check(str_params: list):
+    """Checking if string parameters are of valid format
+    Args:
+        str_params (list): list of string parameters
+
+    Raises:
+        paramException: Error if any of string parameters are empty or is not str
+    """
+    for param in str_params:
+        if not isinstance(param, str):
+            raise paramException(
+                title="Param Error", detail=f"{param} should be a string"
+            )
+
+
 def make_repo_id_string(repo_id: int) -> str:
     """If repo id is int, change to string
 
     Args:
         repo_id (int/str): repo_id of the omixatlas
 
     Returns:
@@ -754,19 +784,15 @@
         dataset_ids (list): List of dataset ids
         priority (str): priority of the operation
     """
     try:
         parameter_check_for_repo_id(src_repo_key)
         parameter_check_for_repo_id(dest_repo_key)
         parameter_check_for_priority(priority)
-        if not dataset_ids or not isinstance(dataset_ids, list):
-            raise paramException(
-                title="param error",
-                detail="dataset_ids should not be empty and dataset_ids should be in list format.",
-            )
+        parameter_check_for_list_dataset_ids(dataset_ids)
     except Exception as err:
         raise err
 
 
 def metadata_files_for_upload(source_metadata_path: str) -> list:
     """Find List of all the metadata files to be uploaded
 
@@ -947,19 +973,15 @@
         components (list): components to be added in the omixatlas
         category (str): category definition of the omixatlas
         data_type(str): datatype of the omixatlas. By default it is None
         org_id(str): org id of the Organisation. By default it is empty
     """
     try:
         str_params = [display_name, description, repo_name, image_url]
-        for param in str_params:
-            if not isinstance(param, str):
-                raise paramException(
-                    title="Param Error", detail=f"{param} should be a string"
-                )
+        str_params_check(str_params)
         check_components_parameter(components)
 
         if not isinstance(category, str) or (
             category not in const.OMIXATLAS_CATEGORY_VALS
         ):
             raise paramException(
                 title="Param Error",
@@ -1050,19 +1072,15 @@
                 detail=(
                     "No parameters passed to update, please pass at least one of the following"
                     + " params [display_name, description, image_url, components, workspace_id, data_type]."
                 ),
             )
 
         str_params = [display_name, description, image_url, workspace_id]
-        for param in str_params:
-            if not isinstance(param, str):
-                raise paramException(
-                    title="Param Error", detail=f"{param} should be a string"
-                )
+        str_params_check(str_params)
         check_components_parameter(components)
     except Exception as err:
         raise err
 
 
 def verify_repo_identifier(repo_identifier: str):
     """Verify if the repository_idenfier is repo_id for a repo
@@ -1090,39 +1108,36 @@
         raise paramException(
             title="Param Error",
             detail="Value of repo_id key and id key is not same in the payload. "
             + "Please correct it. ",
         )
 
 
+# TODO -> can we remove this function altogether
+# and use extract_error_message_details in errors module
+# to follow the DRY principle
+# extract_error_message should be at only 1 place and should be generic enough
+# to handle all the cases
 def extract_error_message(error_msg) -> str:
     """
     Extract error message from the error
     """
     error_msg = json.loads(error_msg)
     error = error_msg.get("error")
     if error is None:
         error = error_msg.get("errors")[0]
     if "detail" in error:
         detail = error.get("detail")
 
-    return detail
-
+    if "title" in error:
+        title = error.get("title")
 
-def dataset_id_type_check_in_delete_datasets(dataset_ids: list):
-    """Dataset Id type check in delete datasets
+    error_msg_dict = {"title": title, "detail": detail}
 
-    Args:
-        dataset_id (list): dataset ids list
-    """
-    if not (dataset_ids and isinstance(dataset_ids, list)):
-        raise paramException(
-            title="Param Error",
-            detail="dataset_ids should be list of strings",
-        )
+    return error_msg_dict
 
 
 def dataset_file_path_dict_type_check_in_delete_datasets(dataset_file_path_dict: dict):
     """dataset_file_path_dict type check in delete datasets
 
     Args:
         dataset_file_path_dict (dict): dict of dataset_file_path_dict
@@ -1158,15 +1173,15 @@
     repo_id: int, dataset_ids: list, dataset_file_path_dict: dict
 ):
     """
     Sanity check for all the parameters of delete datasets
     """
     try:
         parameter_check_for_repo_id(repo_id)
-        dataset_id_type_check_in_delete_datasets(dataset_ids)
+        parameter_check_for_list_dataset_ids(dataset_ids)
         dataset_file_path_dict_type_check_in_delete_datasets(dataset_file_path_dict)
     except Exception as err:
         raise err
 
 
 def dataset_file_path_is_subset_dataset_id(
     dataset_ids: list, dataset_file_path_dict: dict
@@ -1215,63 +1230,196 @@
             + "these are not present in dataset_ids list. "
             + "For any questions, please reach out to polly.support@elucidata.io. "
         )
         # break line added -> for better UX
         print("\n")
 
 
+def fetch_list_api_control_levers() -> str:
+    """Fetch List Files API control Levers"""
+    response = requests.get(const.LIST_FILE_API_CONTROL_LEVER_LINK)
+    error_handler(response)
+    control_levers_dict = json.loads(response.text)
+    default_page_size = control_levers_dict.get(
+        const.DEFAULT_PAGE_SIZE_LIST_FILES_KEY_NAME
+    )
+    page_reduction_percentage = control_levers_dict.get(
+        const.PAGE_REDUCTION_PERCENTAGE_LIST_FILES_KEY_NAME
+    )
+    return default_page_size, page_reduction_percentage
+
+
+def reduce_page_size(default_page_size: int, reduction_percentage: int) -> int:
+    """Reduce the page size based on the current reduction percentage
+
+    Args:
+        default_page_size (int): current page size
+
+    Returns:
+        int: reduced page size
+    """
+    # error_msg_dict = extract_error_message(response.text)
+    # reduce the default page size
+
+    # reduce page size by PAGE_REDUCTION_PERCENTAGE_LIST_FILES
+    # reduction_multiplier = (100 - const.PAGE_REDUCTION_PERCENTAGE_LIST_FILES) / 100
+
+    reduction_multiplier = (100 - reduction_percentage) / 100
+
+    default_page_size = reduction_multiplier * default_page_size
+
+    # TODO -> Put tracking to see how many times API is crashing
+    # with the current default page size -> the tracking will help
+    # to optimise the control lever
+
+    # give nearest rounded integer value -> so that decimal does not come
+    return round(default_page_size)
+
+
+def extract_page_after_from_next_link(next_link: str) -> int:
+    """Extract page[after] from next_link
+
+    Args:
+        next_link (str): next_link given by the API in pagination
+
+    Returns:
+        int: page_after
+    """
+    # next link format ->
+    # /repositories/1643016586529/files
+    # ?page[size]=2500&page[after]=2500&version=latest&include_metadata=True
+
+    # if page[after] exists in next_link then the page[after] value will be b/w
+    # `page[after]=` and `&`
+
+    if "page[after]" in next_link:
+        page_after_str = helpers.find_between(next_link, "page[after]=", "&")
+        # typecast the page[after] value to int and return
+        return int(page_after_str)
+    else:
+        # return 0 as default page_size if "page[after]" does not exist
+        # in the next_link -> this is an extreme case where the API is broken
+        # in normal cases this error may never come
+        return 0
+
+
 # cached for the cases when this function is called internally when same
 # result is needed multiple times
 @lru_cache(maxsize=None)
 def list_files(
-    self: dict, repo_id: str, metadata="true", data="true", version="current"
+    self, repo_id: str, metadata="true", data="true", version="current"
 ) -> list:
     """helper function to integrate list files API response
 
     Args:
-        self (dict): dictionary storing session vara
+        self (polly_session_object): polly_session
         repo_id (str): repo id of the omixatlas
     Returns:
         list_files_resp -> list of objects with requests type
     """
-    # page_size -> for paginating the API
+    # endpoints for list files API
     files_api_endpoint = f"{self.discover_url}/repositories/{repo_id}/files"
-    # initialising an empty value of next link
+
+    # initialising an empty string of next link
     next_link = ""
     responses_list = []
-    # once the pages will end -> next_link will be
-    # set to None by the API
+
+    # page_size -> for paginating the API
+    # set to the default page size mentioned in the constants
+    # if the API crashes then -> it will reduced
+    # default_page_size = const.DEFAULT_PAGE_SIZE_LIST_FILES
+    default_page_size, reduction_percentage = fetch_list_api_control_levers()
+
+    # initially set to 0, but will be updated
+    # as the API request crashes request is called on next link
+    # in that next_link will be set to empty string and page_after
+    # will be updated to current page_after in the next_link
+    page_after = 0
+
+    # initially next_link will be empty string
+    # once the pages will end -> next_link will be set to None by the API
     while next_link is not None:
         if next_link:
             next_endpoint = f"{self.discover_url}{next_link}"
             response = self.session.get(next_endpoint)
+
+            if response.status_code == http_codes.PAYLOAD_TOO_LARGE:
+                page_after = extract_page_after_from_next_link(next_link)
+                list_api_crash_messaging_tracking(self, page_after, default_page_size)
+
+                default_page_size = reduce_page_size(
+                    default_page_size, reduction_percentage
+                )
+                helpers.debug_print(
+                    self, f"--reduced page size---: {default_page_size}"
+                )
+                # intialise next_link to empty str so that query_params
+                # dict is intialised again with new default_page_size and page_after
+                next_link = ""
+                # go to the next iteation
+                continue
         else:
-            # getting the response for the first 100 pages initially
-            # 100 page is set for now -> so that data does not max out
-            # TODO -> need to be optimised for page size and time
             query_params = {
-                "page[size]": 100,
-                "page[after]": 0,
+                "page[size]": default_page_size,
+                "page[after]": page_after,
                 "include_metadata": f"{metadata}",
                 "data": f"{data}",
                 "version": f"{version}",
             }
+
             response = self.session.get(files_api_endpoint, params=query_params)
-        response.raise_for_status()
+            # in case of payload too large error, reduce the page size
+            if response.status_code == http_codes.PAYLOAD_TOO_LARGE:
+                list_api_crash_messaging_tracking(self, page_after, default_page_size)
+
+                default_page_size = reduce_page_size(
+                    default_page_size, reduction_percentage
+                )
+
+                helpers.debug_print(
+                    self, f"--reduced page size---: {default_page_size}"
+                )
+                # go to the next iteation
+                continue
+
+        error_handler(response)
         response_json = response.json()
         # list of request objects
-        # request object having both status and data of the response
+        # reponse object having both status and data of the response
         responses_list.append(response)
         # seeing after 1000 pages whose response is already fetched
         # if there are more pages
         next_link = response_json.get("links").get("next")
-
+        helpers.debug_print(self, f"next link--: {next_link}")
     return responses_list
 
 
+def list_api_crash_messaging_tracking(self, page_after: int, default_page_size: int):
+    """Function to print API crashing and log events for tracking
+
+    Args:
+        page_after (int): page_after value after which API crashed
+        default_page_size (int): page_size for which API crashed
+    """
+    helpers.debug_print(self, "------API crashed-------")
+    helpers.debug_print(self, f"----current page[after] value: {page_after}")
+
+    helpers.debug_print(self, f"--current_page_size: {default_page_size}")
+
+    # tracking metadata
+    # what parameters need to be shown on tracking dashboard
+    # put in the properties dict and pass it
+    properties_dict = {}
+    properties_dict["api_name"] = "list_file_api"
+    properties_dict["crashed_page_size"] = default_page_size
+    properties_dict["current_page_after"] = page_after
+
+    helpers.debug_logger(self, properties_dict)
+
+
 def normalize_file_paths(dataset_file_path_dict: dict):
     """Normalise all the file paths in the dataset_file_path_dict
 
     Args:
         dataset_file_path_dict (dict): key is dataset id and value is the file_path
     """
     # iterating over the dictionary containing dataset_id and list of file paths
@@ -1438,19 +1586,15 @@
 
     Args:
         repo_id (int): repo_id of the repo of the Omixatlas
         dataset_id (str): dataset id passed by the user
     """
     try:
         parameter_check_for_repo_id(repo_id)
-        if not (dataset_id and isinstance(dataset_id, str)):
-            raise paramException(
-                title="Param Error",
-                detail="dataset_ids should be a string",
-            )
+        parameter_check_for_dataset_id(dataset_id)
     except Exception as err:
         raise err
 
 
 def warning_message_for_wrong_destination_folder(
     corresponding_data_file_names: list,
     required_file_name: str,
@@ -1624,24 +1768,20 @@
             detail=const.ERROR_MSG_GET_METADATA,
         )
 
 
 def param_check_download_dataset(
     repo_key: str, dataset_ids: list, folder_path: str
 ) -> None:
+    parameter_check_for_list_dataset_ids(dataset_ids)
     if not (repo_key and isinstance(repo_key, str)):
         raise paramException(
             title="Param Error",
             detail="repo_key (either id or name) is required and should be a string",
         )
-    if not (dataset_ids and isinstance(dataset_ids, list)):
-        raise paramException(
-            title="Param Error",
-            detail="dataset_ids is required and should be a list of dataset_ids as strings",
-        )
     if (not isinstance(folder_path, str)) or (not os.path.isdir(folder_path)):
         raise paramException(
             title="Param Error",
             detail="folder_path if provided should be a string and a valid folder path.",
         )
 
 
@@ -1724,7 +1864,42 @@
 It should either be a string or an integer. Please try again.",
         )
     if not (dataset_id and isinstance(dataset_id, str)):
         raise paramException(
             title="Param Error",
             detail="Argument 'dataset_id' is either empty or invalid. It should be a string. Please try again.",
         )
+
+
+def return_sorted_dict(single_dict: dict) -> dict:
+    """
+    Function that takes in a dictionary and returns an alphabetically sorted dictionary,
+    except for keys - dataset_id and src_dataset_id.
+    If either/both of the two keys are present,it will get inserted in the beginning of the dictionary.
+    """
+    # checking presence of either of the dataset_id related cols in the df
+    id_cols_present = set.intersection(
+        set(["dataset_id", "src_dataset_id"]), set(single_dict.keys())
+    )
+    final_dict = {}
+    if len(id_cols_present) == 0:
+        # None of the two keys present, sort the dictionary
+        final_dict = dict(sorted(single_dict.items()))
+    elif len(id_cols_present) == 1:
+        # Sort the dictionary except for the key that is present,
+        # insert the key after the rest of the dict is sorted
+        key = id_cols_present.pop()
+        col_data = single_dict.pop(key)
+        sorted_dict = dict(sorted(single_dict.items()))
+        final_dict[key] = col_data
+        # updating the dictionary to append the dataset keys first
+        final_dict.update(sorted_dict)
+    else:
+        # Both the keys present, sort the rest of the dict and insert the keys at the beginning of the sorted dictionary.
+        dataset_id_data = single_dict.pop("dataset_id")
+        src_dataset_id_data = single_dict.pop("src_dataset_id")
+        sorted_dict = dict(sorted(single_dict.items()))
+        final_dict["dataset_id"] = dataset_id_data
+        final_dict["src_dataset_id"] = src_dataset_id_data
+        # updating the dictionary to append the dataset keys first
+        final_dict.update(sorted_dict)
+    return final_dict
```

### Comparing `polly-python-0.3.1/polly/schema.py` & `polly-python-0.3.2/polly/schema.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/session.py` & `polly-python-0.3.2/polly/session.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly/tracking.py` & `polly-python-0.3.2/polly/tracking.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from functools import wraps
 from mixpanel import Mixpanel
+import time
+from polly.__init__ import __version__
 from polly.constants import MIXPANEL_KEY
 
 
 class Track:
     """
     This class is used for tracking polly-python services using mixpanel.
     This class will have a unidirectional association relationship with the class which wants to use the tracking service.
@@ -35,14 +37,23 @@
             if kwargs:
                 for key, value in kwargs.items():
                     properties[key] = value
             # tracking the execution status (True/False) of the function
             properties["execution_status"] = execution_flag
             # tracking the env (dev/test/prod) in which this function was called
             properties["tracking_env"] = tracking_env
+            # current polly py version
+            properties["pollypy_version"] = __version__
+
+            # current timestamp
+            # reference link
+            # https://stackoverflow.com/questions/16755394/
+            # what-is-the-easiest-way-to-get-current-gmt-time-in-unix-timestamp-format
+            properties["current_timestamp"] = time.time()
+
             mp = Mixpanel(MIXPANEL_KEY)
             mp.track(email_id, function.__name__, properties)
             if execution_flag:
                 if result is not None:
                     return result
             else:
                 raise returned_err
```

### Comparing `polly-python-0.3.1/polly/validation.py` & `polly-python-0.3.2/polly/validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,66 @@
         # if COMPUTE_ENV_VARIABLE, give priority
         env = helpers.get_platform_value_from_env(
             const.COMPUTE_ENV_VARIABLE, default_env, env
         )
         self.session = Polly.get_session(token, env=env)
 
     @Track.track_decorator
+    def get_ingestion_configs(
+        self, indexing_configs=True, validation_configs=True
+    ) -> dict:
+        """Return the ingestion configs in dictionary which contain two sections
+        i) indexing_configs
+        {
+            "file_metadata": true/false
+            "col_metadata": true/false,
+            "row_metadata": true/false,
+            "data_required": true/false
+        }
+
+
+        ii) validation_configs
+        "validation_check": {
+            "dataset": {
+                "validate": false/true,
+                "scope": "advanced"/"basic",
+                "force_ingest": false/true
+            },
+            "sample": {
+                "validate": false/true,
+                "scope": "advanced"/"basic",
+                "force_ingest": false/true
+            }
+        }
+
+        Args:
+            indexing_configs (bool, optional): Optional parameter(True/False)
+            validation_configs (bool, optional): Optional parameter(True/False)
+
+
+        Returns:
+            dict: dictionary returning the ingestion configs in a dictionary
+        """
+
+        ingestion_configs = {}
+
+        if indexing_configs:
+            indexing_configs_dict = validation_hlpr.get_indexing_configs()
+            ingestion_configs.update(indexing_configs_dict)
+
+        if validation_configs:
+            dataset_config_dict = validation_hlpr.get_dataset_level_validation_config()
+            sample_config_dict = validation_hlpr.get_sample_level_validation_configs()
+            ingestion_configs["validation_check"] = {}
+            ingestion_configs["validation_check"]["dataset"] = dataset_config_dict
+            ingestion_configs["validation_check"]["sample"] = sample_config_dict
+
+        return ingestion_configs
+
+    @Track.track_decorator
     def validate_datasets(
         self, repo_id: int, source_folder_path: dict, schema_config={}
     ) -> pd.DataFrame:
         """Validate the dataset level metadata for datasets to be Ingested
         Args:
             repo_id(int/string): Repo id of OmixAtlas
             source_folder_path(dict): Source folder path of data and metadata files.
```

### Comparing `polly-python-0.3.1/polly/validation_hlpr.py` & `polly-python-0.3.2/polly/validation_hlpr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import copy
 import requests
+import warnings
 import json
 from pathlib import Path
 from polly.errors import paramException, error_handler
 from tqdm import tqdm
 from polly.omixatlas import OmixAtlas
 from polly_validator.validators import dataset_metadata_validator
 
@@ -189,51 +190,153 @@
             # skip hidden files and validation status file
             # if not file.startswith(".") and file != const.VALIDATION_STATUS_FILE_NAME:
             file_path = str(Path(metadata_path) / Path(os.fsdecode(file)))
             with open(file_path, "r") as file_to_upload:
                 res_dict = json.load(file_to_upload)
                 # only put a file for validation
                 # if validate is True in the metadata dict
-                if (
+                validate_val = (
                     res_dict.get("__index__", {})
                     .get("validation_check", {})
                     .get("dataset", {})
                     .get("validate", "")
-                ):
+                )
+                check_for_validate_key_val(validate_val, file)
+                if validate_val:
                     # validation level needed for grouping
                     # metadata dicts with same validation level
-                    validation_level_val = (
+                    scope = (
                         res_dict.get("__index__", {})
                         .get("validation_check", {})
                         .get("dataset", {})
                         .get("scope", "")
                     )
-                    validate_on_val = compute_validate_on_param(validation_level_val)
-                    if validate_on_val in combined_metadata_dict_list:
-                        combined_metadata_dict_list.get(validate_on_val).append(
-                            res_dict
-                        )
+                    if scope:
+                        check_for_scope_key_val(scope, file)
+                        # converting scope to validate_on param that needs to
+                        # passed to validation library
+                        validate_on_val = compute_validate_on_param(scope)
+                        if validate_on_val in combined_metadata_dict_list:
+                            combined_metadata_dict_list.get(validate_on_val).append(
+                                res_dict
+                            )
+                        else:
+                            combined_metadata_dict_list[validate_on_val] = []
+                            combined_metadata_dict_list.get(validate_on_val).append(
+                                res_dict
+                            )
                     else:
-                        combined_metadata_dict_list[validate_on_val] = []
-                        combined_metadata_dict_list.get(validate_on_val).append(
-                            res_dict
-                        )
+                        # raise warning and skip
+                        # validation config does not have scope defined for validation
+                        warning_validation_scope_not_defined(file)
+                else:
+                    # raise warning -> validation config not correctly defined
+                    # validation skipped for the file
+                    warning_validation_config_incorrectly_defined(file)
 
         return combined_metadata_dict_list
     except Exception as err:
         raise err
 
 
+def check_for_validate_key_val(validate_val, file):
+    """check validate_val is of correct type
+
+    Args:
+        validate_val (): validate key val
+        file : file where value defined
+    """
+    if not isinstance(validate_val, bool):
+        raise paramException(
+            title="Param Error",
+            detail=f"validate key is set to incorrect type in {file}. Only boolean allowed",
+        )
+
+
+def check_for_scope_key_val(scope_val, file):
+    """check for scope key correct type
+
+    Args:
+        scope_val (): scope key val
+        file : file where value defined
+    """
+    if scope_val not in const.VALIDATION_SCOPE_CONSTANTS:
+        raise paramException(
+            title="Param Error",
+            detail=f"scope key is set to incorrect type/val in {file}. "
+            + f"Only {const.VALIDATION_SCOPE_CONSTANTS} allowed.",
+        )
+
+
+def get_indexing_configs():
+    """Get Indexing Configs default value"""
+    indexing_configs_dict = {}
+    indexing_configs_dict["file_metadata"] = True
+    indexing_configs_dict["col_metadata"] = True
+    indexing_configs_dict["row_metadata"] = True
+    indexing_configs_dict["data_required"] = True
+    return indexing_configs_dict
+
+
+def get_dataset_level_validation_config():
+    """Get dataset level validation config"""
+    dataset = {}
+    dataset["validate"] = True
+    dataset["scope"] = "advanced"
+    dataset["force_ingest"] = False
+    return dataset
+
+
+def get_sample_level_validation_configs():
+    """Get sample level validation config"""
+    sample = {}
+    sample["validate"] = True
+    sample["scope"] = "advanced"
+    sample["force_ingest"] = False
+    return sample
+
+
+def warning_validation_scope_not_defined(file: str):
+    """Warning to show when validation scope is not present in validation config
+    Args:
+        file (str): file that needs to be validated
+    """
+    warnings.formatwarning = lambda msg, *args, **kwargs: f"WARNING: {msg}\n"
+    warnings.warn(
+        f"Unable to validate metadata file: {file} "
+        + " because the validation_config key did not have scope defined for dataset level. "
+        + "Please use `get_ingestion_configs` to get ingestion_configs in the right format. "
+        + "For any questions, please reach out to polly.support@elucidata.io. "
+    )
+    print("\n")
+
+
+def warning_validation_config_incorrectly_defined(file: str):
+    """Warning to show when validation config is incorrect in the
+    file
+    Args:
+        file(str): file that needs to be validated
+    """
+    warnings.formatwarning = lambda msg, *args, **kwargs: f"WARNING: {msg}\n"
+    warnings.warn(
+        f"Unable to validate metadata file: {file} "
+        + " because the validation_config keys were not present in the right format. "
+        + "Please use `get_ingestion_configs` to get ingestion_configs in the right format. "
+        + "For any questions, please reach out to polly.support@elucidata.io. "
+    )
+    print("\n")
+
+
 def validate_datasets(repo_id: str, schema_dict: dict, combined_metadata: dict):
     """Validate datasets one metadata file at a time
 
     Args:
-        repo_id (str): _description_
-        schema_dict (dict): _description_
-        combined_metadata (dict): _description_
+        repo_id (str): repo_id of the omixatlas
+        schema_dict (dict): schema dict of the omixatlas
+        combined_metadata (dict): combined metadata dict
     """
     # key1 -> "error" & val -> list of error DFs
     # key2 -> "status" & val -> list of status dicts
     validation_lib_res = {}
     validation_lib_res["error"] = []
     validation_lib_res["status"] = []
     for validate_on_val, metadata_list_of_dicts in combined_metadata.items():
```

### Comparing `polly-python-0.3.1/polly/workspaces.py` & `polly-python-0.3.2/polly/workspaces.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/polly_python.egg-info/PKG-INFO` & `polly-python-0.3.2/polly_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: polly-python
-Version: 0.3.1
+Version: 0.3.2
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
-Requires-Python: >=3.6
+Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 ![code-coverage](https://github.com/ElucidataInc/polly-python-code/blob/badges_do_not_delete/badges/badge.svg)
 ![Linting](https://img.shields.io/badge/Linting-Black-green)
```

### Comparing `polly-python-0.3.1/polly_python.egg-info/SOURCES.txt` & `polly-python-0.3.2/polly_python.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -32,10 +32,11 @@
 polly_python.egg-info/dependency_links.txt
 polly_python.egg-info/requires.txt
 polly_python.egg-info/top_level.txt
 tests/test_cohort.py
 tests/test_constants.py
 tests/test_curation.py
 tests/test_helpers.py
+tests/test_jobs.py
 tests/test_omixatlas.py
 tests/test_schema_ux.py
 tests/test_workspaces.py
```

### Comparing `polly-python-0.3.1/tests/test_cohort.py` & `polly-python-0.3.2/tests/test_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/tests/test_constants.py` & `polly-python-0.3.2/tests/test_constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -94,7 +94,9 @@
         "created_timestamp": 1679564893,
         "modified_timestamp": 1679564894,
         "type": "file",
     }
 }
 
 WORKSPACE_RESPONSE_JSON = [{"key": "value"}]
+
+SAMPLE_QUERY = "SELECT * FROM sc_data_lake.features_singlecell LIMIT 100"
```

### Comparing `polly-python-0.3.1/tests/test_curation.py` & `polly-python-0.3.2/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/tests/test_helpers.py` & `polly-python-0.3.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/tests/test_omixatlas.py` & `polly-python-0.3.2/tests/test_omixatlas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from polly import omixatlas
 import polly
 from polly.auth import Polly
 import os
-import csv
 from polly.errors import (
     RequestException,
     apiErrorException,
     InvalidPathException,
     paramException,
     UnauthorizedException,
     InvalidParameterException,
@@ -28,16 +27,18 @@
 from polly_validator.validators import dataset_metadata_validator
 
 # from botocore.exceptions import ClientError
 
 
 key = "POLLY_REFRESH_TOKEN"
 token = os.getenv(key)
+
 test_key = "TEST_POLLY_REFRESH_TOKEN"
 testpolly_token = os.getenv(test_key)
+
 dev_key = "DEV_POLLY_REFRESH_TOKEN"
 devpolly_token = os.getenv(dev_key)
 
 
 def test_obj_initialised():
     Polly.auth(token)
     assert omixatlas.OmixAtlas() is not None
@@ -536,42 +537,165 @@
     repo_id = ""
     dataset_ids = ["GSE100009_GPL11154"]
 
     with pytest.raises(paramException, match=r".*repo_id should not be empty.*"):
         omix_obj.delete_datasets(repo_id, dataset_ids)
 
 
-def test_query_metadata():
+@pytest.fixture()
+def get_query_metadata_fixture():
+    """Get success response for query_metadata enpoint from github"""
+    base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
+
+    data_file = f"{base_polly_py_test_url}/query_metadata_success_response.json"
+    data = requests.get(data_file)
+    error_handler(data)
+    return data
+
+
+@pytest.fixture()
+def get_download_url_fixture():
+    """Get success response of dummy urls from github"""
+    base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
+
+    data_file = f"{base_polly_py_test_url}/download_urls_response.json"
+    data = requests.get(data_file)
+    error_handler(data)
+    return data
+
+
+def test_query_metadata(mocker):
+    """
+    Mock function for query_metadata().
+    """
+    Polly.auth(token)
+    obj = omixatlas.OmixAtlas()
+    query = test_const.SAMPLE_QUERY
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._get_query_id",
+        return_value="query_id",
+    )
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._process_query_to_completion",
+        return_value=pd.DataFrame(),
+    )
+    assert type(obj.query_metadata(query)) is pd.DataFrame
+
+
+def test_query_metadata_iterator(mocker, generator_function):
+    """
+    Mock function for query_metadata_iterator().
+    """
+    Polly.auth(token)
+    query = test_const.SAMPLE_QUERY
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._get_query_id",
+        return_value="query_id",
+    )
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._process_query_to_completion",
+        return_value=generator_function,
+    )
+    obj = omixatlas.OmixAtlas(token)
+    gen = obj.query_metadata(query)
+    assert gen is not None
+
+
+@pytest.fixture()
+def generator_function():
+    """
+    A dummy generator function for mocking a generator
+    """
+    dummy_list = [{"key": "value"}]
+    for i in dummy_list:
+        yield i
+
+
+def test_process_query_to_completion_iterator(
+    mocker, generator_function, get_query_metadata_fixture
+):
+    """
+    Mock function for _process_query_to_completion() with iterator.
+    """
+    Polly.auth(token)
+    obj = omixatlas.OmixAtlas()
+    mocked_response = get_query_metadata_fixture
+    response = mocker.patch.object(obj.session, "get")
+    response.return_value.status_code = 200
+    response.return_value = mocked_response
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._fetch_results_as_file",
+        return_value=generator_function,
+    )
+    query_id = "query_id"
+    iterator_function = True
+    gen = obj._process_query_to_completion(query_id, iterator_function)
+    assert gen is not None
+
+
+def test_process_query_to_completion(mocker, get_query_metadata_fixture):
+    """
+    Mock function for _process_query_to_completion() without iterator.
+    """
+    Polly.auth(token)
+    obj = omixatlas.OmixAtlas()
+    mocked_response = get_query_metadata_fixture
+    response = mocker.patch.object(obj.session, "get")
+    response.return_value.status_code = 200
+    response.return_value = mocked_response
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._fetch_results_as_file",
+        return_value=pd.DataFrame(),
+    )
+    query_id = "query_id"
+    iterator_function = False
+    df = obj._process_query_to_completion(query_id, iterator_function)
+    assert type(df) is pd.DataFrame
+
+
+def test_fetch_results_as_file(mocker, get_download_url_fixture):
+    """
+    Mock function for _fetch_results_as_file() without iterator.
+    """
     Polly.auth(token)
-    nobj3 = omixatlas.OmixAtlas()
-    obj3 = omixatlas.OmixAtlas(token)
-    query_dict = {}
-    with open("tests/query.csv") as csv_file:
-        csv_reader = csv.reader(csv_file, delimiter=",")
-        line_count = 0
-        for row in csv_reader:
-            if line_count == 0:
-                line_count += 1
-            else:
-                query_dict[row[0]] = row[1]
-    query_dataset_level = query_dict["query_dataset_level"]
-    query_sample_level = query_dict["query_sample_level"]
-    query_feature_level = query_dict["query_feature_level"]
-    query_singlecell_sample = query_dict["query_singlecell_sample"]
-    query_singlecell_feature = query_dict["query_singlecell_feature"]
-    assert dict(obj3.query_metadata(query_feature_level)) is not None
-    assert dict(obj3.query_metadata(query_sample_level)) is not None
-    assert dict(obj3.query_metadata(query_dataset_level)) is not None
-    assert dict(obj3.query_metadata(query_singlecell_sample)) is not None
-    assert dict(obj3.query_metadata(query_singlecell_feature)) is not None
-    assert dict(nobj3.query_metadata(query_feature_level)) is not None
-    assert dict(nobj3.query_metadata(query_sample_level)) is not None
-    assert dict(nobj3.query_metadata(query_dataset_level)) is not None
-    assert dict(nobj3.query_metadata(query_singlecell_sample)) is not None
-    assert dict(nobj3.query_metadata(query_singlecell_feature)) is not None
+    obj = omixatlas.OmixAtlas()
+    mocked_response = get_download_url_fixture
+    response = mocker.patch.object(obj.session, "get")
+    response.return_value.status_code = 200
+    response.return_value = mocked_response
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._extract_results_from_download_urls",
+        return_value=pd.DataFrame(),
+    )
+    query_id = "query_id"
+    iterator_function = False
+    df = obj._fetch_results_as_file(query_id, iterator_function)
+    assert type(df) is pd.DataFrame
+
+
+def test_fetch_results_as_file_iterator(
+    mocker, generator_function, get_download_url_fixture
+):
+    """
+    Mock function for _fetch_results_as_file() with iterator.
+    """
+    Polly.auth(token)
+    obj = omixatlas.OmixAtlas()
+    mocked_response = get_download_url_fixture
+    response = mocker.patch.object(obj.session, "get")
+    response.return_value.status_code = 200
+    response.return_value = mocked_response
+    mocker.patch(
+        polly.omixatlas.__name__ + ".OmixAtlas._extract_results_from_download_urls",
+        return_value=generator_function,
+    )
+    query_id = "query_id"
+    iterator_function = True
+    gen = obj._fetch_results_as_file(query_id, iterator_function)
+    assert gen is not None
 
 
 def test_generate_report():
     invalid_repo_key = 9
     valid_repo_key = "9"
     invalid_dataset_id = 9
     valid_dataset_id = "9"
@@ -591,30 +715,101 @@
     with pytest.raises(
         InvalidParameterException,
         match=r".* Invalid Parameters .*",
     ):
         obj.generate_report(valid_repo_key, valid_dataset_id, invalid_workspace_id)
 
 
-'''def test_update_function_by_updating_description():
-    # Either value will be updated to the current value
-    # Or it will be the current value
-    # If value is not equal to the current value means
-    # update is not working
+# update omixatlas tests
 
-    description = "updated description ingestion_test_1 omixatlas"
-    # ingestion_test_1
-    repo_key = "1654268055800"
+
+# Test 1 -> pass no parameters to update -> will raise an error
+def test_update_oa_no_params_passed():
+    Polly.auth(testpolly_token, env="testpolly")
+    omix_obj = omixatlas.OmixAtlas()
+    # ingestion_test_1 repo
+    repo_id = "1654268055800"
+    with pytest.raises(
+        paramException,
+        match=r".* parameters passed to update, please pass at least one of the following .*",
+    ):
+        omix_obj.update(repo_key=repo_id)
+
+
+# Test 2 -> wrong description type
+def test_update_oa_wrong_description_type():
     Polly.auth(testpolly_token, env="testpolly")
     omix_obj = omixatlas.OmixAtlas()
-    res = omix_obj.update(repo_key, description=description)
+    # ingestion_test_1 repo
+    repo_id = "1654268055800"
+    with pytest.raises(
+        paramException,
+        match=r".* should be a string.*",
+    ):
+        omix_obj.update(
+            repo_key=repo_id, description=["Created Omixatlas to test description"]
+        )
+
+
+# Test 3 -> wrong display name type
+def test_update_oa_wrong_display_name_type():
+    Polly.auth(testpolly_token, env="testpolly")
+    omix_obj = omixatlas.OmixAtlas()
+    # ingestion_test_1 repo
+    repo_id = "1654268055800"
+    with pytest.raises(
+        paramException,
+        match=r".* should be a string.*",
+    ):
+        omix_obj.update(repo_key=repo_id, display_name=1234)
+
+
+@pytest.fixture()
+def update_default_patch_req_fixture():
+    # put the response in a json
+    # and do json.loads to load it into a dictionary
+    base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
+    parent_dir = os.getcwd()
+    test_dir = "tests"
+    test_path = os.path.join(parent_dir, test_dir)
+    if not os.path.isdir(test_path):
+        os.makedirs(test_path)
+
+    create_response_file = f"{base_polly_py_test_url}/update_pos_response.json"
+    create_post_response_json = requests.get(create_response_file)
+
+    error_handler(create_post_response_json)
+    fake_create_post_response_json_dict = json.loads(create_post_response_json.text)
+    return fake_create_post_response_json_dict
+
+
+# Test 4 -> positive case -> update description
+def test_update_function_by_updating_description(
+    mocker, update_default_patch_req_fixture
+):
+    # updated description value
+    description_val = "updated description of lib repo dev v1"
+    # ingestion_test_1
+    repo_key_val = "1654268055800"
+    Polly.auth(testpolly_token, env="testpolly")
+    nobj = omixatlas.OmixAtlas()
+    # mocked response with status and no specific value
+    # as no specific response is mocked -> generic message will be printed
+    response = mocker.patch.object(nobj.session, "patch")
+    # http create response code -> 201
+    response.return_value.status_code = 200
+    response.return_value.json.return_value = update_default_patch_req_fixture
+
+    res = nobj.update(repo_key=repo_key_val, description=description_val)
+
     description_value = res.iloc[0, 4]
-    assert description_value == "updated description ingestion_test_1 omixatlas"'''
+    assert description_value == description_val
 
 
+# create omixatlas tests
 def test_create_oa_wrong_category_value():
     # Passing wrong value of category -> will throw error
     Polly.auth(testpolly_token, env="testpolly")
     omix_obj = omixatlas.OmixAtlas()
     with pytest.raises(
         paramException,
         match=r".* should be a string and its value must be one of .*",
@@ -658,14 +853,68 @@
         omix_obj.create(
             "omix_desc_test_12",
             "Created Omixatlas to test description",
             image_url=["/a/c/img.png"],
         )
 
 
+@pytest.fixture()
+def create_default_param_res_fixture_df():
+    Polly.auth(testpolly_token, env="testpolly")
+    res_dict = {}
+    res_dict["Repository Id"] = "1684738195734"
+    res_dict["Repository Name"] = "doing_test_for_mocking_v5"
+    res_dict["Category"] = "private"
+    res_dict["Display Name"] = "doing_test_for_mocking_v5"
+    res_dict["Description"] = "testing locally create for mocking v5"
+    df = pd.DataFrame([res_dict])
+    return df
+
+
+@pytest.fixture()
+def create_default_post_req_fixture():
+    # put the response in a json
+    # and do json.loads to load it into a dictionary
+    base_polly_py_test_url = test_const.POLLY_PY_TEST_FILES_URL
+    parent_dir = os.getcwd()
+    test_dir = "tests"
+    test_path = os.path.join(parent_dir, test_dir)
+    if not os.path.isdir(test_path):
+        os.makedirs(test_path)
+
+    create_response_file = f"{base_polly_py_test_url}/create_pos_response.json"
+    create_post_response_json = requests.get(create_response_file)
+
+    error_handler(create_post_response_json)
+    fake_create_post_response_json_dict = json.loads(create_post_response_json.text)
+    return fake_create_post_response_json_dict
+
+
+def test_create_default_params(
+    mocker, create_default_param_res_fixture_df, create_default_post_req_fixture
+):
+    # then mocking the response of PATCH API CALL for Update Schema
+    Polly.auth(testpolly_token, env="testpolly")
+    nobj = omixatlas.OmixAtlas()
+    # mocked response with status and no specific value
+    # as no specific response is mocked -> generic message will be printed
+    response = mocker.patch.object(nobj.session, "post")
+    # http create response code -> 201
+    response.return_value.status_code = 201
+    response.return_value.json.return_value = create_default_post_req_fixture
+
+    # create default params
+    display_name = "doing_test_for_mocking_v5"
+    description = "testing locally create for mocking v5"
+
+    res = nobj.create(display_name, description)
+
+    pd.testing.assert_frame_equal(res, create_default_param_res_fixture_df)
+
+
 def test_validate_schema_function_empty_repo_id():
     # load data
     response = requests.get(const.SCHEMA_VALIDATION.get("empty_repo_id"))
     error_handler(response)
     test_data = json.loads(response.text)
     Polly.auth(testpolly_token, env="testpolly")
     omix_obj = omixatlas.OmixAtlas()
@@ -1326,60 +1575,61 @@
 #     assert isinstance(res, pd.DataFrame)
 
 #     # number of rows should be 6 in the df -> 5 data files listed above
 #     # And 1 combined metadata file
 #     num_of_rows = len(res.index)
 #     assert num_of_rows == 2
 
+# TODO: need to revert commented code
+# def test_update_dataset_update_metadata_with_no_dataset_in_oa():
+#     """
+#     updating a metadata with no data in the oa
+#     shall throw a warning and skip the update
+#     """
+#     Polly.auth(testpolly_token, env="testpolly")
+#     omix_obj = omixatlas.OmixAtlas()
+#     # ingestion_test_1
+#     repo_id = "1654268055800"
+#     base_add_metadata_test_file_path = BASE_TEST_FORMAT_CONSTANTS_URL
 
-def test_update_dataset_update_metadata_with_no_dataset_in_oa():
-    """
-    updating a metadata with no data in the oa
-    shall throw a warning and skip the update
-    """
-    Polly.auth(testpolly_token, env="testpolly")
-    omix_obj = omixatlas.OmixAtlas()
-    # ingestion_test_1
-    repo_id = "1654268055800"
-    base_add_metadata_test_file_path = BASE_TEST_FORMAT_CONSTANTS_URL
-
-    # creating directory
-    parent_dir = os.getcwd()
-    metadata_dir = "metadata_name_new"
-    metadata_path = os.path.join(parent_dir, metadata_dir)
+#     # creating directory
+#     parent_dir = os.getcwd()
+#     metadata_dir = "metadata_name_new"
+#     metadata_path = os.path.join(parent_dir, metadata_dir)
 
-    # metadata directory
-    if not os.path.isdir(metadata_path):
-        os.makedirs(metadata_path)
-    metadata_file_folder_path = (
-        f"{base_add_metadata_test_file_path}/metadata_name_ext_checks"
-    )
-    # metadata file such that corresponding data file is not present in OA
-    metadata_file_1 = (
-        f"{metadata_file_folder_path}/"
-        + "DLS_BB057_CV244_AML_BMMC_ATAC088_ATAC089_GEX062_GEX063_MTDNA073_MTDNA074_0.05rnaclustres_0.05corr.json"
-    )
-    metadata_resp_1 = requests.get(metadata_file_1)
-    error_handler(metadata_resp_1)
+#     # metadata directory
+#     if not os.path.isdir(metadata_path):
+#         os.makedirs(metadata_path)
+#     metadata_file_folder_path = (
+#         f"{base_add_metadata_test_file_path}/metadata_name_ext_checks"
+#     )
+#     # metadata file such that corresponding data file is not present in OA
+#     metadata_file_1 = (
+#         f"{metadata_file_folder_path}/"
+#         + "DLS_BB057_CV244_AML_BMMC_ATAC088_ATAC089_GEX062_GEX063_MTDNA073_MTDNA074_0.05rnaclustres_0.05corr.json"
+#     )
+#     metadata_resp_1 = requests.get(metadata_file_1)
+#     error_handler(metadata_resp_1)
 
-    meta_file_1_nam = "DLS_BB057_CV244_AML_BMMC_ATAC088_ATAC089_GEX062_GEX063_MTDNA073_MTDNA074_0.05rnaclustres_0.05corrN.json"
+#     meta_file_1_nam = "DLS_BB057_CV244_AML_BMMC_ATAC088_ATAC089_GEX062_GEX063_
+#     MTDNA073_MTDNA074_0.05rnaclustres_0.05corrN.json"
 
-    # creating files in metadata path
-    with open(os.path.join(metadata_path, meta_file_1_nam), "w") as m_file_1:
-        metadata_1_content = metadata_resp_1.text
-        m_file_1.write(metadata_1_content)
-    source_folder_path = {"metadata": metadata_path}
-    destination_folder = "transcriptomics_75"
+#     # creating files in metadata path
+#     with open(os.path.join(metadata_path, meta_file_1_nam), "w") as m_file_1:
+#         metadata_1_content = metadata_resp_1.text
+#         m_file_1.write(metadata_1_content)
+#     source_folder_path = {"metadata": metadata_path}
+#     destination_folder = "transcriptomics_75"
 
-    with pytest.warns(Warning) as record:
-        omix_obj.update_datasets(repo_id, source_folder_path, destination_folder)
-        if not record:
-            pytest.fail("Expected a warning!")
-    print(record)
-    assert len(record) >= 1
+#     with pytest.warns(Warning) as record:
+#         omix_obj.update_datasets(repo_id, source_folder_path, destination_folder)
+#         if not record:
+#             pytest.fail("Expected a warning!")
+#     print(record)
+#     assert len(record) >= 1
 
 
 # these files are there in s3 but not ingested in infra
 # that is why it is not showing in the list files API
 # that is why a warning is getting raised because system shows that these files
 # are present in it from before -> so this test is failing
 # needs to be discussed with shilpa once
@@ -2473,15 +2723,15 @@
         paramException,
         match=r"paramException \(parameter error\): repo_key \(either id or name\) is required and should be a string",
     ):
         obj.download_dataset(invalid_repo_key_type, dataset_id, folder_path)
 
     with pytest.raises(
         paramException,
-        match=r"paramException \(parameter error\): dataset_ids is required and should be a list of dataset_ids as strings*",
+        match=r"paramException \(parameter error\): dataset_ids should be list of strings*",
     ):
         obj.download_dataset(repo_key, invalid_dataset_id_type, folder_path)
 
     with pytest.raises(
         paramException,
         match=r"paramException \(parameter error\): folder_path if provided should be a string and a valid folder path.*",
     ):
```

### Comparing `polly-python-0.3.1/tests/test_schema_ux.py` & `polly-python-0.3.2/tests/test_schema_ux.py`

 * *Files identical despite different names*

### Comparing `polly-python-0.3.1/tests/test_workspaces.py` & `polly-python-0.3.2/tests/test_workspaces.py`

 * *Files identical despite different names*

