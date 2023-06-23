# Comparing `tmp/acceldata_airflow_sdk-2.6.0.tar.gz` & `tmp/acceldata_airflow_sdk-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_airflow_sdk-2.6.0.tar", last modified: Mon Mar  6 08:22:39 2023, max compression
+gzip compressed data, was "acceldata_airflow_sdk-2.7.0.tar", last modified: Fri Jun 23 12:48:05 2023, max compression
```

## Comparing `acceldata_airflow_sdk-2.6.0.tar` & `acceldata_airflow_sdk-2.7.0.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.565693 acceldata_airflow_sdk-2.6.0/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      335 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/CHANGELOG.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1082 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/LICENCE.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       31 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/MANIFEST.in
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    23391 2023-03-06 08:22:39.565393 acceldata_airflow_sdk-2.6.0/PKG-INFO
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    22515 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/README.md
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      196 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/README.txt
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.558978 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        0 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3065 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/dag.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.560722 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        0 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1100 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/handle_callback.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3935 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/job.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     4254 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/span.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1297 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/initialiser.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.561757 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        0 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     4229 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/execute_policy_operator.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     6446 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/job_operator.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     6143 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/span_operator.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     7017 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.562533 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        0 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2270 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/callback.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3477 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/constants.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3812 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/torch_client.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.559953 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk.egg-info/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    23391 2023-03-06 08:22:39.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1405 2023-03-06 08:22:39.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        1 2023-03-06 08:22:39.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       82 2023-03-06 08:22:39.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk.egg-info/requires.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       22 2023-03-06 08:22:39.000000 acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.562739 acceldata_airflow_sdk-2.6.0/docs/
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.557131 acceldata_airflow_sdk-2.6.0/docs/_build/
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.557207 acceldata_airflow_sdk-2.6.0/docs/_build/html/
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.564347 acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      492 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       96 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      858 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      720 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      707 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      623 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1950 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/docs/conf.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.557378 acceldata_airflow_sdk-2.6.0/examples/
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:22:39.565088 acceldata_airflow_sdk-2.6.0/examples/dags/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     8071 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/examples/dags/dag_1.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2937 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/examples/dags/dag_2.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3062 2023-01-30 07:20:37.000000 acceldata_airflow_sdk-2.6.0/examples/dags/simple_test_dag.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       38 2023-03-06 08:22:39.565768 acceldata_airflow_sdk-2.6.0/setup.cfg
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      842 2023-03-06 08:18:17.000000 acceldata_airflow_sdk-2.6.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.656618 acceldata_airflow_sdk-2.7.0/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      335 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23391 2023-06-23 12:48:05.656444 acceldata_airflow_sdk-2.7.0/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    22515 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.649641 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3065 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/dag.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.651432 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1100 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/handle_callback.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3935 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4254 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1297 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.652348 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4229 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/execute_policy_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6446 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/job_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6143 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/span_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7017 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.653055 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2270 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/callback.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3477 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3812 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/torch_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.650496 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23391 2023-06-23 12:48:05.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1651 2023-06-23 12:48:05.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2023-06-23 12:48:05.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       82 2023-06-23 12:48:05.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       22 2023-06-23 12:48:05.000000 acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.653263 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2086 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/README.md
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.653669 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/__init__.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.654490 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/listener/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/listener/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      847 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/listener/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     5215 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/listener/events_listener.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    18118 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/listener/utils.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1215 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/adoc_listener_plugin/plugins/listener_plugin.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.654829 acceldata_airflow_sdk-2.7.0/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.647931 acceldata_airflow_sdk-2.7.0/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.647984 acceldata_airflow_sdk-2.7.0/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:48:05.656142 acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      492 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       96 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      858 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      720 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      707 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      623 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1950 2023-06-14 05:00:44.000000 acceldata_airflow_sdk-2.7.0/docs/conf.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2023-06-23 12:48:05.656653 acceldata_airflow_sdk-2.7.0/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      842 2023-06-23 05:58:49.000000 acceldata_airflow_sdk-2.7.0/setup.py
```

### Comparing `acceldata_airflow_sdk-2.6.0/LICENCE.txt` & `acceldata_airflow_sdk-2.7.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/PKG-INFO` & `acceldata_airflow_sdk-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_airflow_sdk
-Version: 2.6.0
+Version: 2.7.0
 Summary: Acceldata Airflow SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-airflow
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acceldata_airflow_sdk-2.6.0/README.md` & `acceldata_airflow_sdk-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/dag.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/dag.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/handle_callback.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/handle_callback.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/job.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/decorators/span.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/decorators/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/initialiser.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/initialiser.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/execute_policy_operator.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/execute_policy_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/job_operator.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/job_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/span_operator.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/span_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/callback.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/callback.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/constants.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk/utils/torch_client.py` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk/utils/torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/acceldata_airflow_sdk.egg-info/PKG-INFO` & `acceldata_airflow_sdk-2.7.0/acceldata_airflow_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata-airflow-sdk
-Version: 2.6.0
+Version: 2.7.0
 Summary: Acceldata Airflow SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-airflow
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt` & `acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt` & `acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt` & `acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt` & `acceldata_airflow_sdk-2.7.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/docs/conf.py` & `acceldata_airflow_sdk-2.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-2.6.0/setup.py` & `acceldata_airflow_sdk-2.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: Apache Software License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='acceldata_airflow_sdk',
-  version='2.6.0',
+  version='2.7.0',
   description='Acceldata Airflow SDK.' + '\n\n' + open('README.txt').read(),
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type="text/markdown",
   url='',
   author='acceldata',
   author_email='apisupport@acceldata.io',
   license='MIT License',
```

