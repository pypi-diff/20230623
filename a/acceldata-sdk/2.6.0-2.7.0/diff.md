# Comparing `tmp/acceldata_sdk-2.6.0.tar.gz` & `tmp/acceldata_sdk-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_sdk-2.6.0.tar", last modified: Mon Mar  6 08:20:11 2023, max compression
+gzip compressed data, was "acceldata_sdk-2.7.0.tar", last modified: Fri Jun 23 12:29:15 2023, max compression
```

## Comparing `acceldata_sdk-2.6.0.tar` & `acceldata_sdk-2.7.0.tar`

### file list

```diff
@@ -1,87 +1,69 @@
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.393297 acceldata_sdk-2.6.0/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      140 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/CHANGELOG.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3952 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/DATASOURCE_README.md
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1082 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/LICENCE.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       31 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/MANIFEST.in
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    23249 2023-03-06 08:20:11.392941 acceldata_sdk-2.6.0/PKG-INFO
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    18634 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/README.md
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      196 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/README.txt
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.378541 acceldata_sdk-2.6.0/acceldata_sdk/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        0 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1227 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/client.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     8561 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/common.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1966 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/constants.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      172 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/errors.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.380646 acceldata_sdk-2.6.0/acceldata_sdk/events/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        0 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/events/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      373 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/events/generic_event.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1016 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/events/job_events.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      455 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/events/log_events.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1061 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/events/span_event.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      328 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/initialiser.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.384445 acceldata_sdk-2.6.0/acceldata_sdk/models/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      162 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     6504 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/asset.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      664 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/assetType.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     9991 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/connection.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3523 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/create_asset.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     9033 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/datasource.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    10010 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/dqrule.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     4157 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/job.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1136 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/notifications.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    22692 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/pipeline.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2782 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/profile.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    11289 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/reconcillationrule.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     5929 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/rule.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     7453 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/ruleExecutionResult.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2254 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/span.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     8048 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/span_context.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3810 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/models/tags.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    15627 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/torch_client.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    42521 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/acceldata_sdk/torch_http_client.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.379728 acceldata_sdk-2.6.0/acceldata_sdk.egg-info/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)    23249 2023-03-06 08:20:11.000000 acceldata_sdk-2.6.0/acceldata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2302 2023-03-06 08:20:11.000000 acceldata_sdk-2.6.0/acceldata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        1 2023-03-06 08:20:11.000000 acceldata_sdk-2.6.0/acceldata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      117 2023-03-06 08:20:11.000000 acceldata_sdk-2.6.0/acceldata_sdk.egg-info/requires.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       23 2023-03-06 08:20:11.000000 acceldata_sdk-2.6.0/acceldata_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.384739 acceldata_sdk-2.6.0/docs/
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.375236 acceldata_sdk-2.6.0/docs/_build/
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.375307 acceldata_sdk-2.6.0/docs/_build/html/
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.386728 acceldata_sdk-2.6.0/docs/_build/html/_sources/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      491 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       72 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       54 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/readme.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       45 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/readme_datasource.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       34 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/readme_pipeline.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      921 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1731 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1070 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/_build/html/_sources/torch_sdk.rst.txt
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1946 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/docs/conf.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.391512 acceldata_sdk-2.6.0/examples/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)        0 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/__init__.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3684 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/a17_pipeline_bug_2.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3682 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/a17_pipeline_bug_27_10.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1901 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/airflow_cust_trans.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     6779 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/bank_data.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2896 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/child_spans.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     5340 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/demo_sdk.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1723 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/demo_sdk_2.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     8775 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/etl_by_sdk.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3352 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/example_1_pipeline.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3792 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/example_2_pipeline.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2486 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/example_3_1_pipeline.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2726 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/example_3_2_pipeline.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2459 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/example_datasource_workflow.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2392 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/example_datasource_workflow_2.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     8309 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/example_sdk.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     9909 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/pipeline_demo.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     2809 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/sso_demo.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1381 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/examples/test_gcs.py
-drwxr-xr-x   0 jeevanpaul   (501) staff       (20)        0 2023-03-06 08:20:11.392482 acceldata_sdk-2.6.0/integration_tests/
--rw-r--r--   0 jeevanpaul   (501) staff       (20)      887 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/integration_tests/test_constants.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3791 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/integration_tests/test_ds_assets.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     4488 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/integration_tests/test_pipelines.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     3945 2023-01-30 07:20:37.000000 acceldata_sdk-2.6.0/integration_tests/test_policy.py
--rw-r--r--   0 jeevanpaul   (501) staff       (20)       38 2023-03-06 08:20:11.393364 acceldata_sdk-2.6.0/setup.cfg
--rw-r--r--   0 jeevanpaul   (501) staff       (20)     1238 2023-03-06 08:18:27.000000 acceldata_sdk-2.6.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.992984 acceldata_sdk-2.7.0/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      140 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/DATASOURCE_README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23249 2023-06-23 12:29:15.992819 acceldata_sdk-2.7.0/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    18634 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.984760 acceldata_sdk-2.7.0/acceldata_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     8561 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/common.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1966 2023-06-14 05:09:30.000000 acceldata_sdk-2.7.0/acceldata_sdk/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/errors.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.986852 acceldata_sdk-2.7.0/acceldata_sdk/events/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      373 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/generic_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/job_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      455 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/log_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1061 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/span_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.989860 acceldata_sdk-2.7.0/acceldata_sdk/models/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6504 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/assetType.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     9991 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/connection.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3523 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/create_asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     9033 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/datasource.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10010 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/dqrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4157 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1136 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/notifications.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    22692 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/pipeline.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2782 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/profile.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11289 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/reconcillationrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/rule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7453 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/ruleExecutionResult.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2254 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     8048 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/span_context.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/tags.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15627 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    42521 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/torch_http_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.985734 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23249 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1811 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.990033 acceldata_sdk-2.7.0/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.981385 acceldata_sdk-2.7.0/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.981437 acceldata_sdk-2.7.0/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.991553 acceldata_sdk-2.7.0/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/readme.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/readme_datasource.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/readme_pipeline.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2023-06-14 05:00:44.000000 acceldata_sdk-2.7.0/docs/conf.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.992265 acceldata_sdk-2.7.0/integration_tests/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.992416 acceldata_sdk-2.7.0/integration_tests/.pytest_cache/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      302 2023-06-14 11:07:12.000000 acceldata_sdk-2.7.0/integration_tests/.pytest_cache/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/integration_tests/test_constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3791 2023-06-14 05:00:44.000000 acceldata_sdk-2.7.0/integration_tests/test_ds_assets.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/integration_tests/test_pipelines.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3945 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/integration_tests/test_policy.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2023-06-23 12:29:15.993020 acceldata_sdk-2.7.0/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2023-06-23 05:58:49.000000 acceldata_sdk-2.7.0/setup.py
```

### Comparing `acceldata_sdk-2.6.0/DATASOURCE_README.md` & `acceldata_sdk-2.7.0/DATASOURCE_README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/LICENCE.txt` & `acceldata_sdk-2.7.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/PKG-INFO` & `acceldata_sdk-2.7.0/acceldata_sdk.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: acceldata_sdk
-Version: 2.6.0
+Name: acceldata-sdk
+Version: 2.7.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acceldata_sdk-2.6.0/README.md` & `acceldata_sdk-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/client.py` & `acceldata_sdk-2.7.0/acceldata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/common.py` & `acceldata_sdk-2.7.0/acceldata_sdk/common.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/constants.py` & `acceldata_sdk-2.7.0/acceldata_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/events/job_events.py` & `acceldata_sdk-2.7.0/acceldata_sdk/events/job_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/events/span_event.py` & `acceldata_sdk-2.7.0/acceldata_sdk/events/span_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/asset.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/assetType.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/assetType.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/connection.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/connection.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/create_asset.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/create_asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/datasource.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/datasource.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/dqrule.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/dqrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/job.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/notifications.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/notifications.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/pipeline.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/profile.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/profile.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/reconcillationrule.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/reconcillationrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/rule.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/rule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/ruleExecutionResult.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/ruleExecutionResult.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/span.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/span_context.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/span_context.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/models/tags.py` & `acceldata_sdk-2.7.0/acceldata_sdk/models/tags.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/torch_client.py` & `acceldata_sdk-2.7.0/acceldata_sdk/torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk/torch_http_client.py` & `acceldata_sdk-2.7.0/acceldata_sdk/torch_http_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk.egg-info/PKG-INFO` & `acceldata_sdk-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: acceldata-sdk
-Version: 2.6.0
+Name: acceldata_sdk
+Version: 2.7.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acceldata_sdk-2.6.0/acceldata_sdk.egg-info/SOURCES.txt` & `acceldata_sdk-2.7.0/acceldata_sdk.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -45,30 +45,12 @@
 docs/_build/html/_sources/modules.rst.txt
 docs/_build/html/_sources/readme.rst.txt
 docs/_build/html/_sources/readme_datasource.rst.txt
 docs/_build/html/_sources/readme_pipeline.rst.txt
 docs/_build/html/_sources/torch_sdk.events.rst.txt
 docs/_build/html/_sources/torch_sdk.models.rst.txt
 docs/_build/html/_sources/torch_sdk.rst.txt
-examples/__init__.py
-examples/a17_pipeline_bug_2.py
-examples/a17_pipeline_bug_27_10.py
-examples/airflow_cust_trans.py
-examples/bank_data.py
-examples/child_spans.py
-examples/demo_sdk.py
-examples/demo_sdk_2.py
-examples/etl_by_sdk.py
-examples/example_1_pipeline.py
-examples/example_2_pipeline.py
-examples/example_3_1_pipeline.py
-examples/example_3_2_pipeline.py
-examples/example_datasource_workflow.py
-examples/example_datasource_workflow_2.py
-examples/example_sdk.py
-examples/pipeline_demo.py
-examples/sso_demo.py
-examples/test_gcs.py
 integration_tests/test_constants.py
 integration_tests/test_ds_assets.py
 integration_tests/test_pipelines.py
-integration_tests/test_policy.py
+integration_tests/test_policy.py
+integration_tests/.pytest_cache/README.md
```

### Comparing `acceldata_sdk-2.6.0/docs/_build/html/_sources/torch_sdk.events.rst.txt` & `acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.events.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/docs/_build/html/_sources/torch_sdk.models.rst.txt` & `acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.models.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/docs/_build/html/_sources/torch_sdk.rst.txt` & `acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/docs/conf.py` & `acceldata_sdk-2.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/integration_tests/test_constants.py` & `acceldata_sdk-2.7.0/integration_tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/integration_tests/test_ds_assets.py` & `acceldata_sdk-2.7.0/integration_tests/test_ds_assets.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/integration_tests/test_pipelines.py` & `acceldata_sdk-2.7.0/integration_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/integration_tests/test_policy.py` & `acceldata_sdk-2.7.0/integration_tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.6.0/setup.py` & `acceldata_sdk-2.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # except (IOError, ImportError):
 #     description = open('README.md').read()
 
 # Change MIN_TORCH_BACKEND_VERSION_SUPPORTED in constants as well if needed while updating version here
 
 setup(
     name='acceldata_sdk',
-    version='2.6.0',
+    version='2.7.0',
     description='Acceldata SDK.' + '\n\n' + open('README.txt').read(),
     long_description=open('README.md').read() + '\n\n' + open('DATASOURCE_README.md').read() + '\n\n'  + open('CHANGELOG.txt').read(),
     long_description_content_type="text/markdown",
     url='',
     author='acceldata',
     author_email='apisupport@acceldata.io',
     license='MIT License',
```

