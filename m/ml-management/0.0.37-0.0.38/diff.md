# Comparing `tmp/ml-management-0.0.37.tar.gz` & `tmp/ml-management-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.37.tar", last modified: Thu Jun 22 14:46:10 2023, max compression
+gzip compressed data, was "ml-management-0.0.38.tar", last modified: Fri Jun 23 12:33:17 2023, max compression
```

## Comparing `ml-management-0.0.37.tar` & `ml-management-0.0.38.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.843464 ml-management-0.0.37/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       18 2023-02-15 13:35:59.000000 ml-management-0.0.37/MANIFEST.in
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      120 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1092 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      456 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1318 2023-06-01 12:44:21.000000 ml-management-0.0.37/ML_management/collectors/collectors.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/dummy/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      463 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/s3/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10609 2023-06-19 11:21:46.000000 ml-management-0.0.37/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/topic_markers/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)   331440 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3167 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/dataset_loader_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2407 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/executor_template/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/executor_template/default_executors/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      895 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      843 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      869 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4566 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      402 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      334 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/mlmanagement/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      581 2023-03-13 10:54:54.000000 ml-management-0.0.37/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3392 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5054 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    13550 2023-06-22 14:43:51.000000 ml-management-0.0.37/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10262 2023-06-02 13:31:58.000000 ml-management-0.0.37/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      201 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5001 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      316 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/models/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/models/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      949 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/models/patterns/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4202 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      561 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      445 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/registry/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/registry/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2566 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/registry/exceptions.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     7556 2023-06-13 13:01:13.000000 ml-management-0.0.37/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/tests/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/tests/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3361 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9275 2023-06-19 11:21:46.000000 ml-management-0.0.37/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/uploader_data/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1694 2023-06-19 11:21:46.000000 ml-management-0.0.37/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-06-22 14:46:10.839464 ml-management-0.0.37/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       56 2023-02-15 13:35:59.000000 ml-management-0.0.37/README.md
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        7 2023-06-22 14:45:56.000000 ml-management-0.0.37/VERSION
-drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ml_management.egg-info/
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2449 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        1 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      154 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/requires.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       14 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       38 2023-06-22 14:46:10.843464 ml-management-0.0.37/setup.cfg
--rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1053 2023-06-01 12:44:21.000000 ml-management-0.0.37/setup.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-06-06 09:18:11.000000 ml-management-0.0.38/MANIFEST.in
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/collectors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      120 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1092 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      456 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1318 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/collectors.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/collectors/dummy/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      463 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/collectors/s3/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10609 2023-06-20 12:45:17.000000 ml-management-0.0.38/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)   331440 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3167 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/dataset_loader_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2407 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/executor_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4566 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      402 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/mlmanagement/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      581 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    13677 2023-06-23 12:19:15.000000 ml-management-0.0.38/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10260 2023-06-23 12:16:04.000000 ml-management-0.0.38/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      201 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5001 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      316 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/models/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/models/patterns/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4202 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/registry/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/registry/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2566 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/registry/exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     7556 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/tests/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/tests/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9275 2023-06-20 12:45:17.000000 ml-management-0.0.38/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/uploader_data/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1694 2023-06-20 12:45:17.000000 ml-management-0.0.38/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-06-23 12:33:17.977694 ml-management-0.0.38/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-06-06 09:18:11.000000 ml-management-0.0.38/README.md
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-06-23 12:16:14.000000 ml-management-0.0.38/VERSION
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ml_management.egg-info/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2449 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      153 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-06-23 12:33:17.977694 ml-management-0.0.38/setup.cfg
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1052 2023-06-23 12:18:15.000000 ml-management-0.0.38/setup.py
```

### Comparing `ml-management-0.0.37/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.38/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/collectors/collectors.py` & `ml-management-0.0.38/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.38/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.38/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.38/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.38/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.38/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.38/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.38/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.38/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.38/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.38/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.38/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.38/ML_management/mlmanagement/mlmanagement.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 import inspect
 import io
 import os
 import tempfile
 import zipfile
 from typing import Any, Dict, List, Optional, Union
 
+import numpy
 import pandas
-from ML_management.executor_template.upload_model_mode import UploadModelMode
 from ML_management.mlmanagement import utils
 from ML_management.mlmanagement.mlmanager import request_for_function
 from ML_management.mlmanagement.utils import active_run_stack, is_server
-from mlflow.entities import Experiment, Run, RunStatus, ViewType
+from mlflow.entities import Experiment, Run, RunStatus
 from mlflow.entities.model_registry import ModelVersion, RegisteredModel
-from mlflow.models import ModelInputExample, ModelSignature
+from mlflow.models import Model
 from mlflow.pyfunc import PyFuncModel
 from mlflow.store.entities import PagedList
-from mlflow.tracking._model_registry import DEFAULT_AWAIT_MAX_SLEEP_SECONDS
-from mlflow.tracking.fluent import _RUN_ID_ENV_VAR, SEARCH_MAX_RESULTS_PANDAS
+from mlflow.tracking.fluent import _RUN_ID_ENV_VAR
 from mlflow.utils import env
+from scipy.sparse import csc_matrix, csr_matrix
 
 import mlflow
 from mlflow import ActiveRun
 
 
 def monkey_patching_exit(self, exc_type, exc_val, exc_tb):
     """Redefine __exit__ function of class ActiveRun."""
@@ -43,15 +43,15 @@
 
 def start_run_if_not_exist():
     """If run doesn't exist call start_run() function."""
     if len(active_run_stack) == 0:
         start_run()
 
 
-def set_experiment(experiment_name: str) -> None:
+def set_experiment(experiment_name: Optional[str] = None, experiment_id: Optional[str] = None) -> Experiment:
     """
     Set the given experiment as the active experiment.
 
     The experiment must either be specified by name via
     experiment_name or by ID via experiment_id. The experiment name and ID cannot both be specified.
     Set global variable active_experiment_name to that experiment_name.
     """
@@ -63,29 +63,32 @@
     """Retrieve an experiment by experiment name from the backend store."""
     return request_for_function(inspect.currentframe())
 
 
 def search_runs(
     experiment_ids: Optional[List[str]] = None,
     filter_string: str = "",
-    run_view_type: int = ViewType.ACTIVE_ONLY,
-    max_results: int = SEARCH_MAX_RESULTS_PANDAS,
+    run_view_type: int = 1,
+    max_results: int = 100000,
     order_by: Optional[List[str]] = None,
     output_format: str = "pandas",
+    search_all_experiments: bool = False,
+    experiment_names: Optional[List[str]] = None,
 ) -> Union[List[Run], "pandas.DataFrame"]:
     """Search experiments that fit the search criteria."""
     return request_for_function(inspect.currentframe())
 
 
 def start_run(
-    run_id: str = None,
+    run_id: Optional[str] = None,
     experiment_id: Optional[str] = None,
     run_name: Optional[str] = None,
     nested: bool = False,
     tags: Optional[Dict[str, Any]] = None,
+    description: Optional[str] = None,
 ) -> ActiveRun:
     """
     Start a new MLflow run, setting it as the active run under which metrics and parameters will be logged.
 
     The return value can be used as a context manager within a with block; otherwise, you must call end_run() to
     terminate the current run.
     If you pass a run_id or the MLFLOW_RUN_ID environment variable is set, start_run attempts to resume a run with
@@ -155,29 +158,30 @@
 ):
     """Add job metainfo on execution fail. For internal use only."""
     return request_for_function(inspect.currentframe())
 
 
 def log_model(
     artifact_path,
-    upload_model_mode: Optional[UploadModelMode] = None,
     loader_module=None,
     data_path=None,
     code_path=None,
     conda_env=None,
     python_model=None,
     artifacts=None,
-    registered_model_name="default_name",  # TODO maybe raise if no name?
-    signature: ModelSignature = None,
-    input_example: ModelInputExample = None,
-    await_registration_for=DEFAULT_AWAIT_MAX_SLEEP_SECONDS,
+    registered_model_name="default_name",
+    signature: mlflow.models.signature.ModelSignature = None,
+    input_example: Union[pandas.core.frame.DataFrame, numpy.ndarray, dict, list, csr_matrix, csc_matrix, str, bytes] = None,
+    await_registration_for=300,
     pip_requirements=None,
     extra_pip_requirements=None,
+    metadata=None,
     source_model_name=None,
     source_model_version=None,
+    upload_model_mode=None,
 ):
     """
     Log a Pyfunc model with custom inference logic and optional data dependencies as an MLflow artifact.
 
     Current run is using.
     You cannot specify the parameters: loader_module, data_path and the parameters: python_model, artifacts together.
     """
@@ -215,47 +219,42 @@
     """Set a tag under the current run. If no run is active, this method will create a new active run."""
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe())
 
 
 def autolog(
     log_every_n_epoch=1,
+    log_every_n_step=None,
     log_models=True,
+    log_datasets=True,
     disable=False,
     exclusive=False,
     disable_for_unsupported_versions=False,
     silent=False,
+    registered_model_name=None,
 ) -> None:
     """
     Enable (or disable) and configure autologging for all supported integrations.
 
     The parameters are passed to any autologging integrations that support them.
     """
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe(), ["pytorch"])
 
 
-def load_model(model_uri: str, suppress_warnings: bool = True) -> PyFuncModel:
+def load_model(model_uri: str, suppress_warnings: bool = False, dst_path: Optional[str] = None) -> PyFuncModel:
     """Load a model stored in Python function format."""
     return request_for_function(inspect.currentframe(), ["pyfunc"])
 
 
+default_model = Model()
+
+
 def save_model(
-    path,
-    loader_module=None,
-    data_path=None,
-    code_path=None,
-    conda_env=None,
-    mlflow_model=None,
-    python_model=None,
-    artifacts=None,
-    signature: ModelSignature = None,
-    input_example: ModelInputExample = None,
-    pip_requirements=None,
-    extra_pip_requirements=None,
+    path, loader_module=None, data_path=None, code_path=None, conda_env=None, mlflow_model=default_model, python_model=None, artifacts=None
 ):
     """
     Save a Pyfunc model with custom inference logic and optional data dependencies to a path on the local filesystem.
 
     You cannot specify the parameters: loader_module, data_path and the parameters: python_model, artifacts together.
     """
     return request_for_function(inspect.currentframe(), ["pyfunc"])
@@ -307,15 +306,17 @@
     def __init__(self, registry_uri: Optional[str] = None):
         self.extra_attrs = ["tracking"]
         self.for_class = {
             "class_name": self.__class__.__name__,
             "class_kwargs": {"registry_uri": registry_uri},
         }
 
-    def set_model_version_tag(self, name: str, version: str, key: str, value: Any) -> None:
+    def set_model_version_tag(
+        self, name: str, version: Optional[str] = None, key: Optional[str] = None, value: Optional[Any] = None, stage: Optional[str] = None
+    ) -> None:
         """Set model version tag."""
         return request_for_function(
             inspect.currentframe(),
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
 
@@ -331,18 +332,23 @@
         """Get registered model by name."""
         return request_for_function(
             inspect.currentframe(),
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
 
-    # MlflowClient.search_model_versions always returns all versions in single page with no token
-    # as it uses SqlAlchemyStore on mlflow server pod based on helm Values.mlflow.backendUri
-    # which starts with "postgres". See mlflow/store/model_registry/sqlalchemy_store.py:732
-    def search_model_versions(self, filter_string: str) -> PagedList[ModelVersion]:
+    # TODO after updating to a new version, the result is paginated
+    # and needs to be converted to pagination scheme of our project.
+    def search_model_versions(
+        self,
+        filter_string: Optional[str] = None,
+        max_results: int = 10000,
+        order_by: Optional[List[str]] = None,
+        page_token: Optional[str] = None,
+    ) -> PagedList[ModelVersion]:
         """Search for model versions in backend that satisfy the filter criteria."""
         return request_for_function(
             inspect.currentframe(),
             extra_attrs=self.extra_attrs,
             for_class=self.for_class,
         )
```

### Comparing `ml-management-0.0.37/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.38/ML_management/mlmanagement/mlmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 if utils.active_experiment_name != EXPERIMENT_NAME_FOR_DATASET_LOADER:
                     raise InvalidExperimentName(kwargs["model_type"].value, utils.active_experiment_name)
             else:
                 raise ModelTypeIsNotFound()
 
             # now we need to infer schemas for methods.
             methods_schema = {}
-            for (model_type, methods_name_to_schema_map) in model_to_methods.items():
+            for model_type, methods_name_to_schema_map in model_to_methods.items():
                 if isinstance(python_model, model_type):
                     for method_name_to_schema in methods_name_to_schema_map:
                         model_method = getattr(python_model, method_name_to_schema.name, None)
                         model_method_schema = infer_jsonschema(model_method)
                         methods_schema[method_name_to_schema.value] = model_method_schema
             kwargs["model_methods_schema"] = json.dumps(methods_schema)
```

### Comparing `ml-management-0.0.37/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.38/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.38/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.38/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.38/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/registry/exceptions.py` & `ml-management-0.0.38/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/registry/registry_manager.py` & `ml-management-0.0.38/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.38/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.38/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.38/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.38/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.37/setup.py` & `ml-management-0.0.38/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     author_email="modis@ispras.ru",
     maintainer="Maxim Ryndin",
     packages=find_packages(include=["ML_management", "ML_management.*"]),
     include_package_data=True,
     # jsonschema 2.6.0 is the last one to support python 3.6
     install_requires=[
         "sgqlc==16.1",
-        "mlflow==1.21.0",
+        "mlflow==2.4.0",
         "pandas>=0.20.1,<=1.5.2",
         "numpy>=1.8.1,<=1.23.5",
         "jsonschema==2.6.0",
         "requests_toolbelt>=0.9.1,<=0.10.1",
         "boto3==1.21.21",
         "protobuf<4.0.0",
     ],
     data_files=[("", ["VERSION"])],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
 )
```

