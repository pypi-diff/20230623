# Comparing `tmp/bluecast-0.2.tar.gz` & `tmp/bluecast-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-0.2.tar", max compression
+gzip compressed data, was "bluecast-0.3.tar", max compression
```

## Comparing `bluecast-0.2.tar` & `bluecast-0.3.tar`

### file list

```diff
@@ -1,81 +1,103 @@
--rw-r--r--   0        0        0     1076 2023-06-09 18:08:15.669820 bluecast-0.2/LICENSE
--rw-r--r--   0        0        0    14338 2023-06-20 20:04:49.529175 bluecast-0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.514815 bluecast-0.2/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515058 bluecast-0.2/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      168 2023-06-07 04:56:37.021684 bluecast-0.2/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7764 2023-06-08 18:49:56.097612 bluecast-0.2/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0    12209 2023-06-20 20:04:49.529837 bluecast-0.2/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515460 bluecast-0.2/bluecast/config/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:56:37.023862 bluecast-0.2/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3462 2023-06-08 18:49:56.099991 bluecast-0.2/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     2792 2023-06-15 02:48:46.492822 bluecast-0.2/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.515862 bluecast-0.2/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      168 2023-06-07 04:56:37.055926 bluecast-0.2/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1598 2023-06-08 18:49:56.584677 bluecast-0.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     1418 2023-06-08 18:50:02.325344 bluecast-0.2/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1979 2023-06-07 20:39:31.701364 bluecast-0.2/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     1389 2023-06-09 18:08:15.671080 bluecast-0.2/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-06-07 20:14:40.570845 bluecast-0.2/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      171 2023-06-08 18:50:02.038695 bluecast-0.2/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2440 2023-06-08 18:50:02.041457 bluecast-0.2/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2248 2023-06-07 20:39:31.698812 bluecast-0.2/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.516548 bluecast-0.2/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      170 2023-06-07 04:56:37.978742 bluecast-0.2/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1440 2023-06-08 18:50:12.014936 bluecast-0.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     8492 2023-06-08 18:50:09.692583 bluecast-0.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0      982 2023-06-07 20:39:31.678131 bluecast-0.2/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    12506 2023-06-08 18:43:33.722773 bluecast-0.2/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.517425 bluecast-0.2/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      171 2023-06-07 04:56:37.505605 bluecast-0.2/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1428 2023-06-08 18:50:12.016504 bluecast-0.2/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1543 2023-06-08 18:50:12.017272 bluecast-0.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     3675 2023-06-08 18:50:12.018392 bluecast-0.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     4584 2023-06-08 18:50:12.019409 bluecast-0.2/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     6527 2023-06-07 04:56:37.506887 bluecast-0.2/bluecast/preprocessing/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-06-08 18:50:12.020042 bluecast-0.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1957 2023-06-08 18:50:12.020557 bluecast-0.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     4940 2023-06-08 18:50:12.021396 bluecast-0.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     1823 2023-06-08 18:50:12.961492 bluecast-0.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0     1402 2023-06-20 20:04:49.530190 bluecast-0.2/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1424 2023-06-07 20:39:31.712452 bluecast-0.2/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3122 2023-06-07 20:39:31.689572 bluecast-0.2/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     6190 2023-06-20 20:04:49.530725 bluecast-0.2/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      862 2023-06-07 20:39:31.683729 bluecast-0.2/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     1452 2023-06-08 18:43:33.723008 bluecast-0.2/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4561 2023-06-07 20:39:31.709912 bluecast-0.2/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     2871 2023-06-20 20:04:49.531175 bluecast-0.2/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.518803 bluecast-0.2/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      163 2023-06-07 04:56:36.657919 bluecast-0.2/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3729 2023-06-08 18:49:52.784669 bluecast-0.2/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3165 2023-06-08 18:50:12.966095 bluecast-0.2/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1146 2023-06-07 04:56:38.295009 bluecast-0.2/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2401 2023-06-07 04:56:38.296223 bluecast-0.2/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4812 2023-06-08 18:50:12.971333 bluecast-0.2/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1702 2023-06-08 18:50:12.972854 bluecast-0.2/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4598 2023-06-07 04:56:38.302111 bluecast-0.2/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2057 2023-06-08 18:50:12.974781 bluecast-0.2/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2108 2023-06-08 18:50:12.976223 bluecast-0.2/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1528 2023-06-07 04:56:38.303245 bluecast-0.2/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1886 2023-06-07 04:56:38.304347 bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1458 2023-06-07 04:56:38.305381 bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2157 2023-06-07 04:56:38.307410 bluecast-0.2/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:56:12.519076 bluecast-0.2/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      173 2023-06-07 04:56:38.291659 bluecast-0.2/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1132 2023-06-07 04:56:38.292287 bluecast-0.2/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2023-06-07 04:56:12.519593 bluecast-0.2/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     4333 2023-06-20 04:25:58.592640 bluecast-0.2/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     1328 2023-06-07 20:14:40.740928 bluecast-0.2/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     1789 2023-06-09 18:08:15.671451 bluecast-0.2/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     1097 2023-06-07 04:56:12.520160 bluecast-0.2/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:56:12.520372 bluecast-0.2/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     2608 2023-06-07 20:14:40.770936 bluecast-0.2/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     1482 2023-06-08 19:05:45.011986 bluecast-0.2/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:56:12.521016 bluecast-0.2/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1020 2023-06-08 19:13:52.772067 bluecast-0.2/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 18:43:33.723332 bluecast-0.2/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     2204 2023-06-09 18:08:15.671913 bluecast-0.2/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:56:12.521411 bluecast-0.2/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      735 2023-06-07 04:56:12.521599 bluecast-0.2/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:56:12.521767 bluecast-0.2/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1457 2023-06-15 02:48:46.497087 bluecast-0.2/pyproject.toml
--rw-r--r--   0        0        0    15454 1970-01-01 00:00:00.000000 bluecast-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.3/LICENSE
+-rw-r--r--   0        0        0    16212 2023-06-23 13:29:21.676523 bluecast-0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.3/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.3/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.3/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8992 2023-06-23 12:59:49.535433 bluecast-0.3/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0     7485 2023-06-08 04:50:54.090183 bluecast-0.3/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
+-rw-r--r--   0        0        0    13297 2023-06-23 12:59:43.723338 bluecast-0.3/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.3/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.3/bluecast/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4476 2023-06-23 11:38:00.335361 bluecast-0.3/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3347 2023-06-08 04:35:46.974972 bluecast-0.3/bluecast/config/__pycache__/training_config.cpython-38.pyc
+-rw-r--r--   0        0        0     3469 2023-06-23 11:37:59.119340 bluecast-0.3/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.3/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.3/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.3/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2037 2023-06-23 04:30:50.713477 bluecast-0.3/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     1585 2023-06-08 04:35:46.978972 bluecast-0.3/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.3/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1407 2023-06-08 04:35:46.978972 bluecast-0.3/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
+-rw-r--r--   0        0        0     2478 2023-06-23 04:30:45.253379 bluecast-0.3/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.3/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.3/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.3/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.3/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.3/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.3/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.3/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.3/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.3/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.3/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.3/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0     9011 2023-06-23 11:28:59.858174 bluecast-0.3/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0     8279 2023-06-08 04:35:46.978972 bluecast-0.3/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.3/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    13556 2023-06-23 10:39:10.188195 bluecast-0.3/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.3/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.3/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.3/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.3/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.3/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.3/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
+-rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.3/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.3/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     1374 2023-06-23 13:01:03.812637 bluecast-0.3/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.3/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     4561 2023-06-08 04:35:46.982972 bluecast-0.3/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.3/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.3/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
+-rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.3/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     1929 2023-06-08 04:53:15.604550 bluecast-0.3/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
+-rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.3/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.3/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
+-rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.3/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     1790 2023-06-08 04:35:46.982972 bluecast-0.3/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
+-rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.3/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.3/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.3/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     1354 2023-06-23 13:12:42.063930 bluecast-0.3/bluecast/preprocessing/feature_selection.py
+-rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.3/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.3/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.3/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.3/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.3/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.3/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.3/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7699 2023-06-23 12:59:49.139426 bluecast-0.3/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.3/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.3/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.3/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.3/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.3/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.3/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.3/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.3/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.3/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3994 2023-06-09 12:37:48.738873 bluecast-0.3/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.3/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.3/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.3/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.3/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.3/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.3/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.3/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     5855 2023-06-23 12:58:15.485905 bluecast-0.3/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.3/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.3/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.3/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.3/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.3/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.3/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.3/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.3/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.3/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     2204 2023-06-09 12:36:14.185320 bluecast-0.3/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.3/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.3/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.3/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1457 2023-06-23 04:18:51.254539 bluecast-0.3/pyproject.toml
+-rw-r--r--   0        0        0    17328 1970-01-01 00:00:00.000000 bluecast-0.3/PKG-INFO
```

### Comparing `bluecast-0.2/LICENSE` & `bluecast-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/README.md` & `bluecast-0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 A lightweight and fast auto-ml library. This is the successor of the
 e2eml automl library. While e2eml tried to cover many model
 architectures and a lot of different preprocessing options,
 BlueCast focuses on a few model architectures (on default Xgboost
 only) and a few preprocessing options (only what is
 needed for Xgboost). This allows for a much faster development
 cycle and a much more stable codebase while also having as few dependencies
-as possible for the library.
+as possible for the library. Despite being lightweight in its core BlueCast
+offers high customization options for advanced users.
 
 <!-- toc -->
 
 * [Installation](#installation)
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
     * [Custom training configuration](#custom--training-configuration)
     * [Custom preprocessing](#custom-preprocessing)
+    * [Custom feature selection](#custom-feature-selection)
     * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
 * [Meta](#meta)
 
@@ -233,14 +235,61 @@
         custom_last_mile_computation=custom_last_mile_computation, # last step before model training/prediction
     )
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
+#### Custom feature selection
+
+As of version 0.3 BlueCast added automated feature selection. Also this
+step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
+Otherwise the pipeline will fail. To disable feature selection set `execute_selection`
+to `False`. To surpass the `RFECV` limitation a custom feature selection algorithm
+can also be passed as part of a custom last mile computation.
+
+```sh
+from bluecast.config.training_config import FeatureSelectionConfig
+from sklearn.feature_selection import RFECV
+from sklearn.metrics import make_scorer, matthews_corrcoef
+from sklearn.model_selection import StratifiedKFold
+
+# add custom feature selection
+custom_feat_sel = FeatureSelectionConfig()
+# custom_feat_sel.execute_selection = False
+custom_feat_sel.selection_strategy = RFECV(
+    estimator=xgb.XGBClassifier(),
+    step=1,
+    cv=StratifiedKFold(10, random_state=0, shuffle=True),
+    min_features_to_select=1,
+    scoring=make_scorer(matthews_corrcoef),
+    n_jobs=1,
+)
+
+# Create an instance of the BlueCast class with the custom model
+bluecast = BlueCast(
+    class_problem="binary",
+    target_column="target",
+    conf_feature_selection=custom_feat_sel,
+
+# Create some sample data for testing
+x_train = pd.DataFrame(
+    {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
+)
+y_train = pd.Series([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
+x_test = pd.DataFrame(
+    {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
+
+x_train["target"] = y_trai
+# Fit the BlueCast model using the custom model
+bluecast.fit(x_train, "target"
+# Predict on the test data using the custom model
+predicted_probas, predicted_classes = bluecast.predict(x_test)
+```
+
 #### Custom ML model
 
 For some users it might just be convenient to use the BlueCast class to
 enjoy convenience features (details see below), but use a custom ML model.
 This is possible by passing a custom model to the BlueCast class. The needed properties
 are defined via the BaseClassMlModel class. Here is an example:
 
@@ -359,15 +408,15 @@
 * Push your changes and create a pull request
 
 If library or dev dependencies have to be changed, adjust the pyproject.toml.
 For readthedocs it is also requited to update the
 `docs/srtd_requirements.txt` file. Simply run:
 
 ```sh
-poetry export --with doc -f requirements.txt --output docs/rtd_requirements.txt
+poetry export --with dev -f requirements.txt --output docs/rtd_requirements.txt
 ```
 
 If readthedocs will be able to create the documentation can be tested via:
 
 ```sh
 poetry run sphinx-autobuild docs/source docs/build/html
 ```
```

### Comparing `bluecast-0.2/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-0.3/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 18:43:33 2023 UTC, .py size: 10420 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,486 +1,562 @@
-00000000: 6f0d 0d0a 0000 0000 5521 8264 b428 0000  o.......U!.d.(..
+00000000: 6f0d 0d0a 0000 0000 3f97 9564 f133 0000  o.......?..d.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 f600 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 0201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 0100 6401 6403 6c09 5a0a 6401  m.Z...d.d.l.Z.d.
 00000060: 6403 6c0b 5a0c 6401 6404 6c0d 6d0e 5a0e  d.l.Z.d.d.l.m.Z.
-00000070: 6d0f 5a0f 6d10 5a10 0100 6401 6405 6c11  m.Z.m.Z...d.d.l.
-00000080: 6d12 5a12 0100 6401 6406 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
-00000090: 0100 6401 6407 6c15 6d16 5a16 0100 6401  ..d.d.l.m.Z...d.
-000000a0: 6408 6c17 6d18 5a18 0100 6401 6409 6c19  d.l.m.Z...d.d.l.
-000000b0: 6d1a 5a1a 0100 6401 640a 6c1b 6d1c 5a1c  m.Z...d.d.l.m.Z.
-000000c0: 0100 6401 640b 6c1d 6d1e 5a1e 0100 6401  ..d.d.l.m.Z...d.
-000000d0: 640c 6c1f 6d20 5a20 0100 6401 640d 6c21  d.l.m Z ..d.d.l!
-000000e0: 6d22 5a22 0100 6401 640e 6c23 6d24 5a24  m"Z"..d.d.l#m$Z$
-000000f0: 0100 6401 640f 6c25 6d26 5a26 6d27 5a27  ..d.d.l%m&Z&m'Z'
+00000070: 6d0f 5a0f 6d10 5a10 6d11 5a11 0100 6401  m.Z.m.Z.m.Z...d.
+00000080: 6405 6c12 6d13 5a13 0100 6401 6406 6c14  d.l.m.Z...d.d.l.
+00000090: 6d15 5a15 0100 6401 6407 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
+000000a0: 0100 6401 6408 6c18 6d19 5a19 0100 6401  ..d.d.l.m.Z...d.
+000000b0: 6409 6c1a 6d1b 5a1b 0100 6401 640a 6c1c  d.l.m.Z...d.d.l.
+000000c0: 6d1d 5a1d 0100 6401 640b 6c1e 6d1f 5a1f  m.Z...d.d.l.m.Z.
+000000d0: 0100 6401 640c 6c20 6d21 5a21 0100 6401  ..d.d.l m!Z!..d.
+000000e0: 640d 6c22 6d23 5a23 0100 6401 640e 6c24  d.l"m#Z#..d.d.l$
+000000f0: 6d25 5a25 0100 6401 640f 6c26 6d27 5a27  m%Z%..d.d.l&m'Z'
 00000100: 0100 6401 6410 6c28 6d29 5a29 6d2a 5a2a  ..d.d.l(m)Z)m*Z*
-00000110: 0100 4700 6411 6412 8400 6412 8302 5a2b  ..G.d.d...d...Z+
-00000120: 6403 5300 2913 61f9 0100 0052 756e 2066  d.S.).a....Run f
-00000130: 756c 6c79 2063 6f6e 6669 6775 7265 6420  ully configured 
-00000140: 636c 6173 7369 6669 6361 7469 6f6e 2062  classification b
-00000150: 6c75 6570 7269 6e74 2e0a 0a43 7573 746f  lueprint...Custo
-00000160: 6d69 7a61 7469 6f6e 2076 6961 2063 6c61  mization via cla
-00000170: 7373 2061 7474 7269 6275 7465 7320 6973  ss attributes is
-00000180: 2070 6f73 7369 626c 652e 2043 6f6e 6669   possible. Confi
-00000190: 6773 2063 616e 2062 6520 696e 7374 616e  gs can be instan
-000001a0: 7469 6174 6564 2061 6e64 2070 726f 7669  tiated and provi
-000001b0: 6465 6420 746f 2063 6861 6e67 6520 5867  ded to change Xg
-000001c0: 626f 6f73 7420 7472 6169 6e69 6e67 2e0a  boost training..
-000001d0: 4465 6661 756c 7420 6879 7065 7270 6172  Default hyperpar
-000001e0: 616d 6574 6572 2073 6561 7263 6820 7370  ameter search sp
-000001f0: 6163 6520 6973 2072 656c 6174 6976 656c  ace is relativel
-00000200: 7920 6c69 6768 742d 7765 6967 6874 2074  y light-weight t
-00000210: 6f20 7370 6565 6420 7570 2074 6865 2070  o speed up the p
-00000220: 726f 746f 7479 7069 6e67 2e0a 4361 6e20  rototyping..Can 
-00000230: 6465 616c 2077 6974 6820 6269 6e61 7279  deal with binary
-00000240: 2061 6e64 206d 756c 7469 2d63 6c61 7373   and multi-class
-00000250: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
-00000260: 7072 6f62 6c65 6d73 2e0a 4879 7065 7270  problems..Hyperp
-00000270: 6172 616d 6574 6572 2074 756e 696e 6720  arameter tuning 
-00000280: 6361 6e20 6265 2073 7769 7463 6865 6420  can be switched 
-00000290: 6f66 6620 6f72 2065 7665 6e20 7374 7265  off or even stre
-000002a0: 6e67 7468 656e 6564 2076 6961 2063 726f  ngthened via cro
-000002b0: 7373 2d76 616c 6964 6174 696f 6e2e 2054  ss-validation. T
-000002c0: 6869 7320 6265 6861 7669 6f75 7220 6361  his behaviour ca
-000002d0: 6e20 6265 2063 6f6e 7472 6f6c 6c65 640a  n be controlled.
-000002e0: 7669 6120 7468 6520 636f 6e66 6967 2063  via the config c
-000002f0: 6c61 7373 2061 7474 7269 6275 7465 7320  lass attributes 
-00000300: 6672 6f6d 2063 6f6e 6669 672e 7472 6169  from config.trai
-00000310: 6e69 6e67 5f63 6f6e 6669 6720 6d6f 6475  ning_config modu
-00000320: 6c65 2e0a e900 0000 0029 07da 0341 6e79  le.......)...Any
-00000330: da04 4469 6374 da04 4c69 7374 da07 4c69  ..Dict..List..Li
-00000340: 7465 7261 6cda 084f 7074 696f 6e61 6cda  teral..Optional.
-00000350: 0554 7570 6c65 da05 556e 696f 6e4e 2903  .Tuple..UnionN).
-00000360: da0e 5472 6169 6e69 6e67 436f 6e66 6967  ..TrainingConfig
-00000370: da17 5867 626f 6f73 7446 696e 616c 5061  ..XgboostFinalPa
-00000380: 7261 6d43 6f6e 6669 67da 1758 6762 6f6f  ramConfig..Xgboo
-00000390: 7374 5475 6e65 5061 7261 6d73 436f 6e66  stTuneParamsConf
-000003a0: 6967 2901 da0f 6576 616c 5f63 6c61 7373  ig)...eval_class
-000003b0: 6966 6965 7229 01da 1173 6861 705f 6578  ifier)...shap_ex
-000003c0: 706c 616e 6174 696f 6e73 2901 da11 6368  planations)...ch
-000003d0: 6563 6b5f 6770 755f 7375 7070 6f72 7429  eck_gpu_support)
-000003e0: 01da 0c58 6762 6f6f 7374 4d6f 6465 6c29  ...XgboostModel)
-000003f0: 01da 1343 7573 746f 6d50 7265 7072 6f63  ...CustomPreproc
-00000400: 6573 7369 6e67 2901 da0e 6461 7465 5f63  essing)...date_c
-00000410: 6f6e 7665 7274 6572 2901 da12 5461 7267  onverter)...Targ
-00000420: 6574 4c61 6265 6c45 6e63 6f64 6572 2901  etLabelEncoder).
-00000430: da13 4665 6174 7572 6554 7970 6544 6574  ..FeatureTypeDet
-00000440: 6563 746f 7229 01da 1466 696c 6c5f 696e  ector)...fill_in
-00000450: 6669 6e69 7465 5f76 616c 7565 7329 01da  finite_values)..
-00000460: 0e53 6368 656d 6144 6574 6563 746f 7229  .SchemaDetector)
-00000470: 02da 1842 696e 6172 7943 6c61 7373 5461  ...BinaryClassTa
-00000480: 7267 6574 456e 636f 6465 72da 174d 756c  rgetEncoder..Mul
-00000490: 7469 436c 6173 7354 6172 6765 7445 6e63  tiClassTargetEnc
-000004a0: 6f64 6572 2902 da16 7472 6169 6e5f 7465  oder)...train_te
-000004b0: 7374 5f73 706c 6974 5f63 726f 7373 da15  st_split_cross..
-000004c0: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
-000004d0: 5f74 696d 6563 0000 0000 0000 0000 0000  _timec..........
-000004e0: 0000 0000 0000 1600 0000 4000 0000 7318  ..........@...s.
-000004f0: 0100 0065 005a 0164 005a 0264 015a 0309  ...e.Z.d.Z.d.Z..
-00000500: 0209 0209 0209 0209 0209 0209 0209 0264  ...............d
-00000510: 1d64 0365 0464 0419 0064 0565 0565 0665  .d.e.d...d.e.e.e
-00000520: 0765 0866 0319 0064 0665 0965 0a65 0565  .e.f...d.e.e.e.e
-00000530: 0665 0765 0866 0319 0019 0019 0064 0765  .e.e.f.......d.e
-00000540: 0965 0a65 0565 0665 0765 0866 0319 0019  .e.e.e.e.e.f....
-00000550: 0019 0064 0865 0965 0619 0064 0965 0965  ...d.e.e...d.e.e
-00000560: 0b19 0064 0a65 0965 0c19 0064 0b65 0965  ...d.e.e...d.e.e
-00000570: 0d19 0064 0c65 0965 0e19 0064 0d65 0965  ...d.e.e...d.e.e
-00000580: 0f19 0066 1464 0e64 0f84 055a 1064 1065  ...f.d.d...Z.d.e
-00000590: 116a 1264 1165 0664 1264 0266 0664 1364  .j.d.e.d.d.f.d.d
-000005a0: 1484 045a 1364 1065 116a 1264 1565 116a  ...Z.d.e.j.d.e.j
-000005b0: 1264 1665 116a 1464 1165 0664 1265 1565  .d.e.j.d.e.d.e.e
-000005c0: 0665 1666 0219 0066 0a64 1764 1884 045a  .e.f...f.d.d...Z
-000005d0: 1764 1065 116a 1264 1265 116a 1266 0464  .d.e.j.d.e.j.f.d
-000005e0: 1964 1a84 045a 1864 1065 116a 1264 1265  .d...Z.d.e.j.d.e
-000005f0: 1965 1a6a 1b65 1a6a 1b66 0219 0066 0464  .e.j.e.j.f...f.d
-00000600: 1b64 1c84 045a 1c64 0253 0029 1eda 0842  .d...Z.d.S.)...B
-00000610: 6c75 6543 6173 7461 a504 0000 5275 6e20  lueCasta....Run 
-00000620: 6675 6c6c 7920 636f 6e66 6967 7572 6564  fully configured
-00000630: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
-00000640: 626c 7565 7072 696e 742e 0a0a 2020 2020  blueprint...    
-00000650: 4375 7374 6f6d 697a 6174 696f 6e20 7669  Customization vi
-00000660: 6120 636c 6173 7320 6174 7472 6962 7574  a class attribut
-00000670: 6573 2069 7320 706f 7373 6962 6c65 2e20  es is possible. 
-00000680: 436f 6e66 6967 7320 6361 6e20 6265 2069  Configs can be i
-00000690: 6e73 7461 6e74 6961 7465 6420 616e 6420  nstantiated and 
-000006a0: 7072 6f76 6964 6564 2074 6f20 6368 616e  provided to chan
-000006b0: 6765 2058 6762 6f6f 7374 2074 7261 696e  ge Xgboost train
-000006c0: 696e 672e 0a20 2020 2044 6566 6175 6c74  ing..    Default
-000006d0: 2068 7970 6572 7061 7261 6d65 7465 7220   hyperparameter 
-000006e0: 7365 6172 6368 2073 7061 6365 2069 7320  search space is 
-000006f0: 7265 6c61 7469 7665 6c79 206c 6967 6874  relatively light
-00000700: 2d77 6569 6768 7420 746f 2073 7065 6564  -weight to speed
-00000710: 2075 7020 7468 6520 7072 6f74 6f74 7970   up the prototyp
-00000720: 696e 672e 0a20 2020 203a 7061 7261 6d20  ing..    :param 
-00000730: 3a63 6c61 7373 5f70 726f 626c 656d 3a20  :class_problem: 
-00000740: 5461 6b65 7320 6120 7374 7269 6e67 2063  Takes a string c
-00000750: 6f6e 7461 696e 696e 6720 7468 6520 636c  ontaining the cl
-00000760: 6173 7320 7072 6f62 6c65 6d20 7479 7065  ass problem type
-00000770: 2e20 4569 7468 6572 2022 6269 6e61 7279  . Either "binary
-00000780: 2220 6f72 2022 6d75 6c74 6963 6c61 7373  " or "multiclass
-00000790: 222e 0a20 2020 203a 7061 7261 6d20 3a74  "..    :param :t
-000007a0: 6172 6765 745f 636f 6c75 6d6e 3a20 5461  arget_column: Ta
-000007b0: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
-000007c0: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
-000007d0: 206f 6620 7468 6520 7461 7267 6574 2063   of the target c
-000007e0: 6f6c 756d 6e2e 0a20 2020 203a 7061 7261  olumn..    :para
-000007f0: 6d20 3a63 6174 5f63 6f6c 756d 6e73 3a20  m :cat_columns: 
-00000800: 5461 6b65 7320 6120 6c69 7374 206f 6620  Takes a list of 
-00000810: 7374 7269 6e67 7320 636f 6e74 6169 6e69  strings containi
-00000820: 6e67 2074 6865 206e 616d 6573 206f 6620  ng the names of 
-00000830: 7468 6520 6361 7465 676f 7269 6361 6c20  the categorical 
-00000840: 636f 6c75 6d6e 732e 2049 6620 6e6f 7420  columns. If not 
-00000850: 7072 6f76 6964 6564 2c0a 2020 2020 426c  provided,.    Bl
-00000860: 7565 4361 7374 2077 696c 6c20 696e 6665  ueCast will infe
-00000870: 7220 7468 6573 6520 6175 746f 6d61 6963  r these automaic
-00000880: 616c 6c79 2e0a 2020 2020 3a70 6172 616d  ally..    :param
-00000890: 203a 6461 7465 5f63 6f6c 756d 6e73 3a20   :date_columns: 
-000008a0: 5461 6b65 7320 6120 6c69 7374 206f 6620  Takes a list of 
-000008b0: 7374 7269 6e67 7320 636f 6e74 6169 6e69  strings containi
-000008c0: 6e67 2074 6865 206e 616d 6573 206f 6620  ng the names of 
-000008d0: 7468 6520 6461 7465 2063 6f6c 756d 6e73  the date columns
-000008e0: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
-000008f0: 642c 0a20 2020 2042 6c75 6543 6173 7420  d,.    BlueCast 
-00000900: 7769 6c6c 2069 6e66 6572 2074 6865 7365  will infer these
-00000910: 2061 7574 6f6d 6169 6361 6c6c 792e 0a20   automaically.. 
-00000920: 2020 203a 7061 7261 6d20 3a74 696d 655f     :param :time_
-00000930: 7370 6c69 745f 636f 6c75 6d6e 3a20 5461  split_column: Ta
-00000940: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
-00000950: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
-00000960: 206f 6620 7468 6520 7469 6d65 2073 706c   of the time spl
-00000970: 6974 2063 6f6c 756d 6e2e 2049 6620 6e6f  it column. If no
-00000980: 7420 7072 6f76 6964 6564 2c0a 2020 2020  t provided,.    
-00000990: 426c 7565 4361 7374 2077 696c 6c20 6e6f  BlueCast will no
-000009a0: 7420 7370 6c69 7420 7468 6520 6461 7461  t split the data
-000009b0: 2062 7920 7469 6d65 206f 7220 6f72 6465   by time or orde
-000009c0: 722c 2062 7574 2064 6f20 6120 7261 6e64  r, but do a rand
-000009d0: 6f6d 2073 706c 6974 2069 6e73 7465 6164  om split instead
-000009e0: 2e0a 2020 2020 3a70 6172 616d 203a 6d6c  ..    :param :ml
-000009f0: 5f6d 6f64 656c 3a20 5461 6b65 7320 616e  _model: Takes an
-00000a00: 2069 6e73 7461 6e63 6520 6f66 2061 2058   instance of a X
-00000a10: 6762 6f6f 7374 4d6f 6465 6c20 636c 6173  gboostModel clas
-00000a20: 732e 2049 6620 6e6f 7420 7072 6f76 6964  s. If not provid
-00000a30: 6564 2c20 426c 7565 4361 7374 2077 696c  ed, BlueCast wil
-00000a40: 6c20 696e 7374 616e 7469 6174 6520 6f6e  l instantiate on
-00000a50: 652e 0a20 2020 2054 6869 7320 6973 2061  e..    This is a
-00000a60: 6e20 4150 4920 746f 2070 6173 7320 616e  n API to pass an
-00000a70: 7920 6d6f 6465 6c20 636c 6173 732e 2049  y model class. I
-00000a80: 6e68 6572 6974 2074 6865 2062 6173 6563  nherit the basec
-00000a90: 6c61 7373 2066 726f 6d20 6d6c 5f6d 6f64  lass from ml_mod
-00000aa0: 656c 6c69 6e67 2e62 6173 655f 6d6f 6465  elling.base_mode
-00000ab0: 6c2e 4261 7365 4d6f 6465 6c2e 0a20 2020  l.BaseModel..   
-00000ac0: 204e da0d 636c 6173 735f 7072 6f62 6c65   N..class_proble
-00000ad0: 6d29 02da 0662 696e 6172 79da 0a6d 756c  m)...binary..mul
-00000ae0: 7469 636c 6173 73da 0d74 6172 6765 745f  ticlass..target_
-00000af0: 636f 6c75 6d6e da0b 6361 745f 636f 6c75  column..cat_colu
-00000b00: 6d6e 73da 0c64 6174 655f 636f 6c75 6d6e  mns..date_column
-00000b10: 73da 1174 696d 655f 7370 6c69 745f 636f  s..time_split_co
-00000b20: 6c75 6d6e da08 6d6c 5f6d 6f64 656c da13  lumn..ml_model..
-00000b30: 6375 7374 6f6d 5f70 7265 7072 6f63 6573  custom_preproces
-00000b40: 736f 72da 0d63 6f6e 665f 7472 6169 6e69  sor..conf_traini
-00000b50: 6e67 da0c 636f 6e66 5f78 6762 6f6f 7374  ng..conf_xgboost
-00000b60: da13 636f 6e66 5f70 6172 616d 735f 7867  ..conf_params_xg
-00000b70: 626f 6f73 7463 0b00 0000 0000 0000 0000  boostc..........
-00000b80: 0000 0b00 0000 0200 0000 4300 0000 7364  ..........C...sd
-00000b90: 0000 007c 017c 005f 0064 017c 005f 017c  ...|.|._.d.|._.|
-00000ba0: 037c 005f 027c 047c 005f 037c 057c 005f  .|._.|.|._.|.|._
-00000bb0: 047c 027c 005f 057c 087c 005f 067c 097c  .|.|._.|.|._.|.|
-00000bc0: 005f 077c 0a7c 005f 0864 007c 005f 0964  ._.|.|._.d.|._.d
-00000bd0: 007c 005f 0a64 007c 005f 0b64 007c 005f  .|._.d.|._.d.|._
-00000be0: 0c7c 067c 005f 0d7c 077c 005f 0e64 007c  .|.|._.|.|._.d.|
-00000bf0: 005f 0f64 0053 0029 024e 4629 1072 1b00  ._.d.S.).NF).r..
-00000c00: 0000 da0f 7072 6564 6963 7469 6f6e 5f6d  ....prediction_m
-00000c10: 6f64 6572 1f00 0000 7220 0000 0072 2100  oder....r ...r!.
-00000c20: 0000 721e 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
-00000c30: 0072 2600 0000 da12 6665 6174 5f74 7970  .r&.....feat_typ
-00000c40: 655f 6465 7465 6374 6f72 da0b 6361 745f  e_detector..cat_
-00000c50: 656e 636f 6465 72da 1474 6172 6765 745f  encoder..target_
-00000c60: 6c61 6265 6c5f 656e 636f 6465 72da 0f73  label_encoder..s
-00000c70: 6368 656d 615f 6465 7465 6374 6f72 7222  chema_detectorr"
-00000c80: 0000 0072 2300 0000 da0b 7368 6170 5f76  ...r#.....shap_v
-00000c90: 616c 7565 7329 0bda 0473 656c 6672 1b00  alues)...selfr..
-00000ca0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000cb0: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-00000cc0: 7224 0000 0072 2500 0000 7226 0000 00a9  r$...r%...r&....
-00000cd0: 0072 2e00 0000 fa47 2f55 7365 7273 2f74  .r.....G/Users/t
-00000ce0: 686f 6d61 736d 6569 7373 6e65 722f 4964  homasmeissner/Id
-00000cf0: 6561 5072 6f6a 6563 7473 2f42 6c75 6543  eaProjects/BlueC
-00000d00: 6173 742f 626c 7565 6361 7374 2f62 6c75  ast/bluecast/blu
-00000d10: 6570 7269 6e74 732f 6361 7374 2e70 79da  eprints/cast.py.
-00000d20: 085f 5f69 6e69 745f 5f38 0000 0073 2200  .__init__8...s".
-00000d30: 0000 060d 0601 0601 0601 0601 0601 0601  ................
-00000d40: 0601 0601 0601 0203 04fe 0603 0601 0601  ................
-00000d50: 0601 0a01 7a11 426c 7565 4361 7374 2e5f  ....z.BlueCast._
-00000d60: 5f69 6e69 745f 5fda 0264 66da 0a74 6172  _init__..df..tar
-00000d70: 6765 745f 636f 6cda 0672 6574 7572 6e63  get_col..returnc
-00000d80: 0300 0000 0000 0000 0000 0000 0700 0000  ................
-00000d90: 0600 0000 4300 0000 73cc 0100 0074 0083  ....C...s....t..
-00000da0: 0001 0074 0183 007c 005f 027c 006a 02a0  ...t...|._.|.j..
-00000db0: 037c 01a1 017d 017c 006a 026a 0472 287c  .|...}.|.j.j.r(|
-00000dc0: 006a 057c 006a 026a 0476 0072 2874 0683  .j.|.j.j.v.r(t..
-00000dd0: 007c 005f 077c 006a 07a0 087c 017c 006a  .|._.|.j...|.|.j
-00000de0: 0519 00a1 017c 017c 006a 053c 007c 006a  .....|.|.j.<.|.j
-00000df0: 026a 047c 005f 047c 006a 026a 097c 005f  .j.|._.|.j.j.|._
-00000e00: 0974 0a7c 0183 017d 0174 0b7c 017c 006a  .t.|...}.t.|.|.j
-00000e10: 0983 027d 017c 006a 0c64 0175 0172 4d74  ...}.|.j.d.u.rMt
-00000e20: 0d7c 017c 027c 006a 0c83 035c 047d 037d  .|.|.|.j...\.}.}
-00000e30: 047d 057d 066e 0974 0e7c 017c 0283 025c  .}.}.n.t.|.|...\
-00000e40: 047d 037d 047d 057d 0674 0f83 007c 005f  .}.}.}.}.t...|._
-00000e50: 107c 006a 10a0 117c 03a1 0101 007c 006a  .|.j...|.....|.j
-00000e60: 10a0 127c 04a1 017d 047c 006a 0464 0175  ...|...}.|.j.d.u
-00000e70: 0172 847c 006a 1364 026b 0272 8474 147c  .r.|.j.d.k.r.t.|
-00000e80: 006a 0483 017c 005f 157c 006a 15a0 167c  .j...|._.|.j...|
-00000e90: 037c 05a1 027d 037c 006a 15a0 177c 04a1  .|...}.|.j...|..
-00000ea0: 017d 046e 1d7c 006a 0464 0175 0172 a17c  .}.n.|.j.d.u.r.|
-00000eb0: 006a 1364 036b 0272 a174 187c 006a 0483  .j.d.k.r.t.|.j..
-00000ec0: 017c 005f 157c 006a 15a0 197c 037c 05a1  .|._.|.j...|.|..
-00000ed0: 027d 037c 006a 15a0 1a7c 04a1 017d 047c  .}.|.j...|...}.|
-00000ee0: 006a 1b72 b87c 006a 1ba0 1c7c 037c 05a1  .j.r.|.j...|.|..
-00000ef0: 025c 027d 037d 057c 006a 1b6a 127c 047c  .\.}.}.|.j.j.|.|
-00000f00: 0564 0464 058d 035c 027d 047d 067c 006a  .d.d...\.}.}.|.j
-00000f10: 1d73 c874 1e7c 006a 137c 006a 1f7c 006a  .s.t.|.j.|.j.|.j
-00000f20: 207c 006a 2164 068d 047c 005f 1d7c 006a   |.j!d...|._.|.j
-00000f30: 1da0 117c 037c 047c 057c 06a1 0401 007c  ...|.|.|.|.....|
-00000f40: 006a 1f72 e17c 006a 1f6a 2272 e174 237c  .j.r.|.j.j"r.t#|
-00000f50: 006a 1d6a 247c 0464 0783 037c 005f 2564  .j.j$|.d...|._%d
-00000f60: 087c 005f 2664 0153 0029 097a 1954 7261  .|._&d.S.).z.Tra
-00000f70: 696e 2061 2066 756c 6c20 4d4c 2070 6970  in a full ML pip
-00000f80: 656c 696e 652e 4e72 1c00 0000 721d 0000  eline.Nr....r...
-00000f90: 0046 a901 da0e 7072 6564 6963 746f 6e5f  .F....predicton_
-00000fa0: 6d6f 6465 2903 7224 0000 0072 2500 0000  mode).r$...r%...
-00000fb0: 7226 0000 00da 0474 7265 6554 2927 720e  r&.....treeT)'r.
-00000fc0: 0000 0072 1300 0000 7228 0000 005a 1b66  ...r....r(...Z.f
-00000fd0: 6974 5f74 7261 6e73 666f 726d 5f66 6561  it_transform_fea
-00000fe0: 7475 7265 5f74 7970 6573 721f 0000 0072  ture_typesr....r
-00000ff0: 1e00 0000 7212 0000 0072 2a00 0000 5a1b  ....r....r*...Z.
-00001000: 6669 745f 7472 616e 7366 6f72 6d5f 7461  fit_transform_ta
-00001010: 7267 6574 5f6c 6162 656c 7372 2000 0000  rget_labelsr ...
-00001020: 7214 0000 0072 1100 0000 7221 0000 0072  r....r....r!...r
-00001030: 1900 0000 7218 0000 0072 1500 0000 722b  ....r....r....r+
-00001040: 0000 00da 0366 6974 da09 7472 616e 7366  .....fit..transf
-00001050: 6f72 6d72 1b00 0000 7216 0000 0072 2900  ormr....r....r).
-00001060: 0000 5a1e 6669 745f 7461 7267 6574 5f65  ..Z.fit_target_e
-00001070: 6e63 6f64 655f 6269 6e61 7279 5f63 6c61  ncode_binary_cla
-00001080: 7373 da24 7472 616e 7366 6f72 6d5f 7461  ss.$transform_ta
-00001090: 7267 6574 5f65 6e63 6f64 655f 6269 6e61  rget_encode_bina
-000010a0: 7279 5f63 6c61 7373 7217 0000 005a 1c66  ry_classr....Z.f
-000010b0: 6974 5f74 6172 6765 745f 656e 636f 6465  it_target_encode
-000010c0: 5f6d 756c 7469 636c 6173 73da 2274 7261  _multiclass."tra
-000010d0: 6e73 666f 726d 5f74 6172 6765 745f 656e  nsform_target_en
-000010e0: 636f 6465 5f6d 756c 7469 636c 6173 7372  code_multiclassr
-000010f0: 2300 0000 da0d 6669 745f 7472 616e 7366  #.....fit_transf
-00001100: 6f72 6d72 2200 0000 720f 0000 0072 2400  ormr"...r....r$.
-00001110: 0000 7225 0000 0072 2600 0000 5a15 6361  ..r%...r&...Z.ca
-00001120: 6c63 756c 6174 655f 7368 6170 5f76 616c  lculate_shap_val
-00001130: 7565 7372 0d00 0000 da05 6d6f 6465 6c72  uesr......modelr
-00001140: 2c00 0000 7227 0000 0029 0772 2d00 0000  ,...r'...).r-...
-00001150: 7231 0000 0072 3200 0000 5a07 785f 7472  r1...r2...Z.x_tr
-00001160: 6169 6e5a 0678 5f74 6573 745a 0779 5f74  ainZ.x_testZ.y_t
-00001170: 7261 696e 5a06 795f 7465 7374 722e 0000  rainZ.y_testr...
-00001180: 0072 2e00 0000 722f 0000 0072 3700 0000  .r....r/...r7...
-00001190: 5800 0000 7360 0000 0006 0208 010c 0108  X...s`..........
-000011a0: 020e 0108 0106 0308 0102 ff02 fe04 0102  ................
-000011b0: ff0a 060a 0108 020c 010a 0202 0108 010e  ................
-000011c0: ff12 0408 020c 010c 0114 020c 010e 010e  ................
-000011d0: 0114 010c 010e 010c 0106 0212 0106 0106  ................
-000011e0: 010a ff06 0402 0104 0104 0104 0104 0108  ................
-000011f0: fc12 060e 0112 010a 017a 0c42 6c75 6543  .........z.BlueC
-00001200: 6173 742e 6669 74da 0764 665f 6576 616c  ast.fit..df_eval
-00001210: da0b 7461 7267 6574 5f65 7661 6c63 0500  ..target_evalc..
-00001220: 0000 0000 0000 0000 0000 0800 0000 0400  ................
-00001230: 0000 4300 0000 732a 0000 007c 00a0 007c  ..C...s*...|...|
-00001240: 017c 04a1 0201 007c 00a0 017c 02a1 015c  .|.....|...|...\
-00001250: 027d 057d 0674 027c 036a 037c 0683 027d  .}.}.t.|.j.|...}
-00001260: 077c 0753 0029 0161 8e02 0000 5472 6169  .|.S.).a....Trai
-00001270: 6e20 6120 6675 6c6c 204d 4c20 7069 7065  n a full ML pipe
-00001280: 6c69 6e65 2061 6e64 2065 7661 6c75 6174  line and evaluat
-00001290: 6520 6f6e 2061 2068 6f6c 646f 7574 2073  e on a holdout s
-000012a0: 6574 2e0a 0a20 2020 2020 2020 2054 6869  et...        Thi
-000012b0: 7320 6973 2061 2063 6f6e 7665 6e69 656e  s is a convenien
-000012c0: 6365 2066 756e 6374 696f 6e20 746f 2074  ce function to t
-000012d0: 7261 696e 2061 6e64 2065 7661 6c75 6174  rain and evaluat
-000012e0: 6520 6f6e 2061 2068 6f6c 646f 7574 2073  e on a holdout s
-000012f0: 6574 2e20 4974 2069 7320 7265 636f 6d6d  et. It is recomm
-00001300: 656e 6465 6420 746f 2075 7365 2074 6869  ended to use thi
-00001310: 7320 666f 7220 6d6f 6465 6c0a 2020 2020  s for model.    
-00001320: 2020 2020 6578 706c 6f72 6174 696f 6e2e      exploration.
-00001330: 204f 6e20 7072 6f64 7563 7469 6f6e 2074   On production t
-00001340: 6865 2073 696d 706c 6520 6669 7428 2920  he simple fit() 
-00001350: 6675 6e63 7469 6f6e 2073 686f 756c 6420  function should 
-00001360: 6265 2075 7365 642e 0a20 2020 2020 2020  be used..       
-00001370: 203a 7061 7261 6d20 3a64 663a 2054 616b   :param :df: Tak
-00001380: 6573 2061 2070 616e 6461 7320 4461 7461  es a pandas Data
-00001390: 4672 616d 6520 636f 6e74 6169 6e69 6e67  Frame containing
-000013a0: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
-000013b0: 7461 2061 6e64 2074 6865 2074 6172 6765  ta and the targe
-000013c0: 7473 2e0a 2020 2020 2020 2020 3a70 6172  ts..        :par
-000013d0: 616d 203a 6466 5f65 7661 6c3a 2054 616b  am :df_eval: Tak
-000013e0: 6573 2061 2070 616e 6461 7320 4461 7461  es a pandas Data
-000013f0: 4672 616d 6520 636f 6e74 6169 6e69 6e67  Frame containing
-00001400: 2074 6865 2065 7661 6c75 6174 696f 6e20   the evaluation 
-00001410: 6461 7461 2c20 6275 7420 6e6f 7420 7468  data, but not th
-00001420: 6520 7461 7267 6574 732e 0a20 2020 2020  e targets..     
-00001430: 2020 203a 7061 7261 6d20 3a74 6172 6765     :param :targe
-00001440: 745f 6576 616c 3a20 5461 6b65 7320 6120  t_eval: Takes a 
-00001450: 7061 6e64 6173 2053 6572 6965 7320 636f  pandas Series co
-00001460: 6e74 6169 6e69 6e67 2074 6865 2065 7661  ntaining the eva
-00001470: 6c75 6174 696f 6e20 7461 7267 6574 732e  luation targets.
-00001480: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001490: 3a74 6172 6765 745f 636f 6c3a 2054 616b  :target_col: Tak
-000014a0: 6573 2061 2073 7472 696e 6720 636f 6e74  es a string cont
-000014b0: 6169 6e69 6e67 2074 6865 206e 616d 6520  aining the name 
-000014c0: 6f66 2074 6865 2074 6172 6765 7420 636f  of the target co
-000014d0: 6c75 6d6e 2069 6e73 6964 6520 7468 6520  lumn inside the 
-000014e0: 7472 6169 6e69 6e67 2064 6174 6120 6466  training data df
-000014f0: 2e0a 2020 2020 2020 2020 2904 7237 0000  ..        ).r7..
-00001500: 00da 0770 7265 6469 6374 720c 0000 00da  ...predictr.....
-00001510: 0676 616c 7565 7329 0872 2d00 0000 7231  .values).r-...r1
-00001520: 0000 0072 3d00 0000 723e 0000 0072 3200  ...r=...r>...r2.
-00001530: 0000 da07 795f 7072 6f62 73da 0979 5f63  ....y_probs..y_c
-00001540: 6c61 7373 6573 5a09 6576 616c 5f64 6963  lassesZ.eval_dic
-00001550: 7472 2e00 0000 722e 0000 0072 2f00 0000  tr....r....r/...
-00001560: da08 6669 745f 6576 616c 9300 0000 7308  ..fit_eval....s.
-00001570: 0000 000c 100e 010c 0104 017a 1142 6c75  ...........z.Blu
-00001580: 6543 6173 742e 6669 745f 6576 616c 6302  eCast.fit_evalc.
-00001590: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000015a0: 0000 0043 0000 0073 ca00 0000 7400 8300  ...C...s....t...
-000015b0: 0100 7c00 6a01 730a 7402 6401 8301 8201  ..|.j.s.t.d.....
-000015c0: 7c00 6a01 6a03 7c01 7c00 6a04 6701 6402  |.j.j.|.|.j.g.d.
-000015d0: 8d02 7d01 7405 7c01 8301 7d01 7406 7c01  ..}.t.|...}.t.|.
-000015e0: 7c00 6a07 8302 7d01 7c00 6a08 7227 7c00  |.j...}.|.j.r'|.
-000015f0: 6a08 a009 7c01 a101 7d01 7c00 6a0a 723f  j...|...}.|.j.r?
-00001600: 7c00 6a0b 723f 7c00 6a0c 6403 6b02 723f  |.j.r?|.j.d.k.r?
-00001610: 740d 7c00 6a0b 740e 8302 723f 7c00 6a0b  t.|.j.t...r?|.j.
-00001620: a00f 7c01 a101 7d01 6e17 7c00 6a0a 7256  ..|...}.n.|.j.rV
-00001630: 7c00 6a0b 7256 7c00 6a0c 6404 6b02 7256  |.j.rV|.j.d.k.rV
-00001640: 740d 7c00 6a0b 7410 8302 7256 7c00 6a0b  t.|.j.t...rV|.j.
-00001650: a011 7c01 a101 7d01 7c00 6a12 7263 7c00  ..|...}.|.j.rc|.
-00001660: 6a12 6a09 7c01 6405 6406 8d02 5c02 7d01  j.j.|.d.d...\.}.
-00001670: 7d02 7c01 5300 2907 7a37 5472 616e 7366  }.|.S.).z7Transf
-00001680: 6f72 6d20 6e65 7720 6461 7461 2061 6363  orm new data acc
-00001690: 6f72 6469 6e67 2074 6f20 7072 6570 726f  ording to prepro
-000016a0: 6365 7373 696e 6720 7069 7065 6c69 6e65  cessing pipeline
-000016b0: 2efa 2a46 6561 7475 7265 2074 7970 6520  ..*Feature type 
-000016c0: 636f 6e76 6572 7465 7220 636f 756c 6420  converter could 
-000016d0: 6e6f 7420 6265 2066 6f75 6e64 2e29 015a  not be found.).Z
-000016e0: 0b69 676e 6f72 655f 636f 6c73 721c 0000  .ignore_colsr...
-000016f0: 0072 1d00 0000 5472 3400 0000 2913 720e  .r....Tr4...).r.
-00001700: 0000 0072 2800 0000 da09 4578 6365 7074  ...r(.....Except
-00001710: 696f 6e5a 1774 7261 6e73 666f 726d 5f66  ionZ.transform_f
-00001720: 6561 7475 7265 5f74 7970 6573 721e 0000  eature_typesr...
-00001730: 0072 1400 0000 7211 0000 0072 2000 0000  .r....r....r ...
-00001740: 722b 0000 0072 3800 0000 721f 0000 0072  r+...r8...r....r
-00001750: 2900 0000 721b 0000 00da 0a69 7369 6e73  )...r......isins
-00001760: 7461 6e63 6572 1600 0000 7239 0000 0072  tancer....r9...r
-00001770: 1700 0000 723a 0000 0072 2300 0000 2903  ....r:...r#...).
-00001780: 722d 0000 0072 3100 0000 da01 5f72 2e00  r-...r1....._r..
-00001790: 0000 722e 0000 0072 2f00 0000 da12 7472  ..r....r/.....tr
-000017a0: 616e 7366 6f72 6d5f 6e65 775f 6461 7461  ansform_new_data
-000017b0: a800 0000 733a 0000 0006 0206 0108 0106  ....s:..........
-000017c0: 0208 0106 ff08 030c 0106 020c 0104 0302  ................
-000017d0: ff04 0202 fe0a 030a 0102 ff0e 0304 0202  ................
-000017e0: ff04 0202 fe0a 030a 0102 ff0c 0306 0214  ................
-000017f0: 0104 017a 1b42 6c75 6543 6173 742e 7472  ...z.BlueCast.tr
-00001800: 616e 7366 6f72 6d5f 6e65 775f 6461 7461  ansform_new_data
-00001810: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00001820: 0005 0000 0043 0000 0073 8000 0000 7c00  .....C...s....|.
-00001830: 6a00 7307 7401 6401 8301 8201 7c00 6a02  j.s.t.d.....|.j.
-00001840: 730e 7401 6402 8301 8201 7403 8300 0100  s.t.d.....t.....
-00001850: 7c00 a004 7c01 a101 7d01 7405 6403 8301  |...|...}.t.d...
-00001860: 0100 7c00 6a00 a006 7c01 a101 5c02 7d02  ..|.j...|...\.}.
-00001870: 7d03 7c00 6a02 6a07 723c 7c00 6a08 7c00  }.|.j.j.r<|.j.|.
-00001880: 6a02 6a07 7600 723c 7c00 6a09 723c 7c00  j.j.v.r<|.j.r<|.
-00001890: 6a02 723c 7c00 6a09 a00a 740b a00c 7c03  j.r<|.j...t...|.
-000018a0: a101 a101 7d03 7c02 7c03 6602 5300 2904  ....}.|.|.f.S.).
-000018b0: 7a90 5072 6564 6963 7420 6f6e 2075 6e73  z.Predict on uns
-000018c0: 6565 6e20 6461 7461 2e0a 0a20 2020 2020  een data...     
-000018d0: 2020 2052 6574 7572 6e20 7468 6520 7072     Return the pr
-000018e0: 6564 6963 7465 6420 7072 6f62 6162 696c  edicted probabil
-000018f0: 6974 6965 7320 616e 6420 7468 6520 7072  ities and the pr
-00001900: 6564 6963 7465 6420 636c 6173 7365 733a  edicted classes:
-00001910: 0a20 2020 2020 2020 2079 5f70 726f 6273  .        y_probs
-00001920: 2c20 795f 636c 6173 7365 7320 3d20 7072  , y_classes = pr
-00001930: 6564 6963 7428 6466 290a 2020 2020 2020  edict(df).      
-00001940: 2020 7a1b 4d6c 206d 6f64 656c 2063 6f75    z.Ml model cou
-00001950: 6c64 206e 6f74 2062 6520 666f 756e 6472  ld not be foundr
-00001960: 4400 0000 7a0d 5072 6564 6963 7469 6e67  D...z.Predicting
-00001970: 2e2e 2e29 0d72 2200 0000 7245 0000 0072  ...).r"...rE...r
-00001980: 2800 0000 720e 0000 0072 4800 0000 da05  (...r....rH.....
-00001990: 7072 696e 7472 3f00 0000 721f 0000 0072  printr?...r....r
-000019a0: 1e00 0000 722a 0000 005a 1f6c 6162 656c  ....r*...Z.label
-000019b0: 5f65 6e63 6f64 6572 5f72 6576 6572 7365  _encoder_reverse
-000019c0: 5f74 7261 6e73 666f 726d da02 7064 da06  _transform..pd..
-000019d0: 5365 7269 6573 2904 722d 0000 0072 3100  Series).r-...r1.
-000019e0: 0000 7241 0000 0072 4200 0000 722e 0000  ..rA...rB...r...
-000019f0: 0072 2e00 0000 722f 0000 0072 3f00 0000  .r....r/...r?...
-00001a00: ca00 0000 7324 0000 0006 0608 0106 0208  ....s$..........
-00001a10: 0106 020a 0108 0210 0108 020e 0204 0102  ................
-00001a20: ff04 0202 fe06 0408 0104 ff08 047a 1042  .............z.B
-00001a30: 6c75 6543 6173 742e 7072 6564 6963 7429  lueCast.predict)
-00001a40: 084e 4e4e 4e4e 4e4e 4e29 1dda 085f 5f6e  .NNNNNNNN)...__n
-00001a50: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00001a60: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00001a70: 075f 5f64 6f63 5f5f 7205 0000 0072 0800  .__doc__r....r..
-00001a80: 0000 da03 7374 72da 0566 6c6f 6174 da03  ....str..float..
-00001a90: 696e 7472 0600 0000 7204 0000 0072 0f00  intr....r....r..
-00001aa0: 0000 7210 0000 0072 0900 0000 720b 0000  ..r....r....r...
-00001ab0: 0072 0a00 0000 7230 0000 0072 4a00 0000  .r....r0...rJ...
-00001ac0: da09 4461 7461 4672 616d 6572 3700 0000  ..DataFramer7...
-00001ad0: 724b 0000 0072 0300 0000 7202 0000 0072  rK...r....r....r
-00001ae0: 4300 0000 7248 0000 0072 0700 0000 da02  C...rH...r......
-00001af0: 6e70 da07 6e64 6172 7261 7972 3f00 0000  np..ndarrayr?...
-00001b00: 722e 0000 0072 2e00 0000 722e 0000 0072  r....r....r....r
-00001b10: 2f00 0000 721a 0000 0027 0000 0073 5a00  /...r....'...sZ.
-00001b20: 0000 0800 0401 0214 0201 0201 0201 0201  ................
-00001b30: 0201 0201 0201 04f5 0602 02fe 0c03 02fd  ................
-00001b40: 1404 02fc 1405 02fb 0606 02fa 0607 02f9  ................
-00001b50: 0608 02f8 0609 02f7 060a 02f6 060b 0af5  ................
-00001b60: 1820 023b 0402 02fe 0403 02fd 0404 02fc  . .;............
-00001b70: 0205 02fb 0a06 0afa 1615 2422 721a 0000  ..........$"r...
-00001b80: 0029 2c72 4f00 0000 da06 7479 7069 6e67  .),rO.....typing
-00001b90: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-00001ba0: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
-00001bb0: 0000 00da 056e 756d 7079 7254 0000 00da  .....numpyrT....
-00001bc0: 0670 616e 6461 7372 4a00 0000 da1f 626c  .pandasrJ.....bl
-00001bd0: 7565 6361 7374 2e63 6f6e 6669 672e 7472  uecast.config.tr
-00001be0: 6169 6e69 6e67 5f63 6f6e 6669 6772 0900  aining_configr..
-00001bf0: 0000 720a 0000 0072 0b00 0000 5a20 626c  ..r....r....Z bl
-00001c00: 7565 6361 7374 2e65 7661 6c75 6174 696f  uecast.evaluatio
-00001c10: 6e2e 6576 616c 5f6d 6574 7269 6373 720c  n.eval_metricsr.
-00001c20: 0000 005a 1f62 6c75 6563 6173 742e 6576  ...Z.bluecast.ev
-00001c30: 616c 7561 7469 6f6e 2e73 6861 705f 7661  aluation.shap_va
-00001c40: 6c75 6573 720d 0000 005a 2462 6c75 6563  luesr....Z$bluec
-00001c50: 6173 742e 6765 6e65 7261 6c5f 7574 696c  ast.general_util
-00001c60: 732e 6765 6e65 7261 6c5f 7574 696c 7372  s.general_utilsr
-00001c70: 0e00 0000 5a1d 626c 7565 6361 7374 2e6d  ....Z.bluecast.m
-00001c80: 6c5f 6d6f 6465 6c6c 696e 672e 7867 626f  l_modelling.xgbo
-00001c90: 6f73 7472 0f00 0000 da1d 626c 7565 6361  ostr......blueca
-00001ca0: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
-00001cb0: 2e63 7573 746f 6d72 1000 0000 5a28 626c  .customr....Z(bl
-00001cc0: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
-00001cd0: 7369 6e67 2e64 6174 6574 696d 655f 6665  sing.datetime_fe
-00001ce0: 6174 7572 6573 7211 0000 005a 2b62 6c75  aturesr....Z+blu
-00001cf0: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-00001d00: 696e 672e 656e 636f 6465 5f74 6172 6765  ing.encode_targe
-00001d10: 745f 6c61 6265 6c73 7212 0000 005a 2462  t_labelsr....Z$b
-00001d20: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
-00001d30: 7373 696e 672e 6665 6174 7572 655f 7479  ssing.feature_ty
-00001d40: 7065 7372 1300 0000 5a25 626c 7565 6361  pesr....Z%blueca
-00001d50: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
-00001d60: 2e6e 756c 6c73 5f61 6e64 5f69 6e66 7372  .nulls_and_infsr
-00001d70: 1400 0000 5a24 626c 7565 6361 7374 2e70  ....Z$bluecast.p
-00001d80: 7265 7072 6f63 6573 7369 6e67 2e73 6368  reprocessing.sch
-00001d90: 656d 615f 6368 6563 6b73 7215 0000 005a  ema_checksr....Z
-00001da0: 2662 6c75 6563 6173 742e 7072 6570 726f  &bluecast.prepro
-00001db0: 6365 7373 696e 672e 7461 7267 6574 5f65  cessing.target_e
-00001dc0: 6e63 6f64 696e 6772 1600 0000 7217 0000  ncodingr....r...
-00001dd0: 005a 2762 6c75 6563 6173 742e 7072 6570  .Z'bluecast.prep
-00001de0: 726f 6365 7373 696e 672e 7472 6169 6e5f  rocessing.train_
-00001df0: 7465 7374 5f73 706c 6974 7218 0000 0072  test_splitr....r
-00001e00: 1900 0000 721a 0000 0072 2e00 0000 722e  ....r....r....r.
-00001e10: 0000 0072 2e00 0000 722f 0000 00da 083c  ...r....r/.....<
-00001e20: 6d6f 6475 6c65 3e01 0000 0073 2400 0000  module>....s$...
-00001e30: 0400 2408 0802 0801 1402 0c05 0c01 0c01  ..$.............
-00001e40: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 1001  ................
-00001e50: 1004 1206                                ....
+00000110: 0100 6401 6411 6c2b 6d2c 5a2c 0100 4700  ..d.d.l+m,Z,..G.
+00000120: 6412 6413 8400 6413 8302 5a2d 6403 5300  d.d...d...Z-d.S.
+00000130: 2914 61f9 0100 0052 756e 2066 756c 6c79  ).a....Run fully
+00000140: 2063 6f6e 6669 6775 7265 6420 636c 6173   configured clas
+00000150: 7369 6669 6361 7469 6f6e 2062 6c75 6570  sification bluep
+00000160: 7269 6e74 2e0a 0a43 7573 746f 6d69 7a61  rint...Customiza
+00000170: 7469 6f6e 2076 6961 2063 6c61 7373 2061  tion via class a
+00000180: 7474 7269 6275 7465 7320 6973 2070 6f73  ttributes is pos
+00000190: 7369 626c 652e 2043 6f6e 6669 6773 2063  sible. Configs c
+000001a0: 616e 2062 6520 696e 7374 616e 7469 6174  an be instantiat
+000001b0: 6564 2061 6e64 2070 726f 7669 6465 6420  ed and provided 
+000001c0: 746f 2063 6861 6e67 6520 5867 626f 6f73  to change Xgboos
+000001d0: 7420 7472 6169 6e69 6e67 2e0a 4465 6661  t training..Defa
+000001e0: 756c 7420 6879 7065 7270 6172 616d 6574  ult hyperparamet
+000001f0: 6572 2073 6561 7263 6820 7370 6163 6520  er search space 
+00000200: 6973 2072 656c 6174 6976 656c 7920 6c69  is relatively li
+00000210: 6768 742d 7765 6967 6874 2074 6f20 7370  ght-weight to sp
+00000220: 6565 6420 7570 2074 6865 2070 726f 746f  eed up the proto
+00000230: 7479 7069 6e67 2e0a 4361 6e20 6465 616c  typing..Can deal
+00000240: 2077 6974 6820 6269 6e61 7279 2061 6e64   with binary and
+00000250: 206d 756c 7469 2d63 6c61 7373 2063 6c61   multi-class cla
+00000260: 7373 6966 6963 6174 696f 6e20 7072 6f62  ssification prob
+00000270: 6c65 6d73 2e0a 4879 7065 7270 6172 616d  lems..Hyperparam
+00000280: 6574 6572 2074 756e 696e 6720 6361 6e20  eter tuning can 
+00000290: 6265 2073 7769 7463 6865 6420 6f66 6620  be switched off 
+000002a0: 6f72 2065 7665 6e20 7374 7265 6e67 7468  or even strength
+000002b0: 656e 6564 2076 6961 2063 726f 7373 2d76  ened via cross-v
+000002c0: 616c 6964 6174 696f 6e2e 2054 6869 7320  alidation. This 
+000002d0: 6265 6861 7669 6f75 7220 6361 6e20 6265  behaviour can be
+000002e0: 2063 6f6e 7472 6f6c 6c65 640a 7669 6120   controlled.via 
+000002f0: 7468 6520 636f 6e66 6967 2063 6c61 7373  the config class
+00000300: 2061 7474 7269 6275 7465 7320 6672 6f6d   attributes from
+00000310: 2063 6f6e 6669 672e 7472 6169 6e69 6e67   config.training
+00000320: 5f63 6f6e 6669 6720 6d6f 6475 6c65 2e0a  _config module..
+00000330: e900 0000 0029 07da 0341 6e79 da04 4469  .....)...Any..Di
+00000340: 6374 da04 4c69 7374 da07 4c69 7465 7261  ct..List..Litera
+00000350: 6cda 084f 7074 696f 6e61 6cda 0554 7570  l..Optional..Tup
+00000360: 6c65 da05 556e 696f 6e4e 2904 da16 4665  le..UnionN)...Fe
+00000370: 6174 7572 6553 656c 6563 7469 6f6e 436f  atureSelectionCo
+00000380: 6e66 6967 da0e 5472 6169 6e69 6e67 436f  nfig..TrainingCo
+00000390: 6e66 6967 da17 5867 626f 6f73 7446 696e  nfig..XgboostFin
+000003a0: 616c 5061 7261 6d43 6f6e 6669 67da 1758  alParamConfig..X
+000003b0: 6762 6f6f 7374 5475 6e65 5061 7261 6d73  gboostTuneParams
+000003c0: 436f 6e66 6967 2901 da0f 6576 616c 5f63  Config)...eval_c
+000003d0: 6c61 7373 6966 6965 7229 01da 1173 6861  lassifier)...sha
+000003e0: 705f 6578 706c 616e 6174 696f 6e73 2901  p_explanations).
+000003f0: da11 6368 6563 6b5f 6770 755f 7375 7070  ..check_gpu_supp
+00000400: 6f72 7429 01da 0c58 6762 6f6f 7374 4d6f  ort)...XgboostMo
+00000410: 6465 6c29 01da 1343 7573 746f 6d50 7265  del)...CustomPre
+00000420: 7072 6f63 6573 7369 6e67 2901 da0e 6461  processing)...da
+00000430: 7465 5f63 6f6e 7665 7274 6572 2901 da12  te_converter)...
+00000440: 5461 7267 6574 4c61 6265 6c45 6e63 6f64  TargetLabelEncod
+00000450: 6572 2901 da0f 4665 6174 7572 6553 656c  er)...FeatureSel
+00000460: 6563 746f 7229 01da 1346 6561 7475 7265  ector)...Feature
+00000470: 5479 7065 4465 7465 6374 6f72 2901 da14  TypeDetector)...
+00000480: 6669 6c6c 5f69 6e66 696e 6974 655f 7661  fill_infinite_va
+00000490: 6c75 6573 2901 da0e 5363 6865 6d61 4465  lues)...SchemaDe
+000004a0: 7465 6374 6f72 2902 da18 4269 6e61 7279  tector)...Binary
+000004b0: 436c 6173 7354 6172 6765 7445 6e63 6f64  ClassTargetEncod
+000004c0: 6572 da17 4d75 6c74 6943 6c61 7373 5461  er..MultiClassTa
+000004d0: 7267 6574 456e 636f 6465 7229 01da 1074  rgetEncoder)...t
+000004e0: 7261 696e 5f74 6573 745f 7370 6c69 7463  rain_test_splitc
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000500: 1a00 0000 4000 0000 7334 0100 0065 005a  ....@...s4...e.Z
+00000510: 0164 005a 0264 015a 0309 0209 0209 0209  .d.Z.d.Z........
+00000520: 0209 0209 0209 0209 0209 0209 0264 1f64  .............d.d
+00000530: 0365 0464 0419 0064 0565 0565 0665 0765  .e.d...d.e.e.e.e
+00000540: 0866 0319 0064 0665 0965 0a65 0565 0665  .f...d.e.e.e.e.e
+00000550: 0765 0866 0319 0019 0019 0064 0765 0965  .e.f.......d.e.e
+00000560: 0a65 0565 0665 0765 0866 0319 0019 0019  .e.e.e.e.f......
+00000570: 0064 0865 0965 0619 0064 0965 0965 0565  .d.e.e...d.e.e.e
+00000580: 0b65 0c66 0219 0019 0064 0a65 0965 0d19  .e.f.....d.e.e..
+00000590: 0064 0b65 0965 0d19 0064 0c65 0965 0e19  .d.e.e...d.e.e..
+000005a0: 0064 0d65 0965 0f19 0064 0e65 0965 1019  .d.e.e...d.e.e..
+000005b0: 0064 0f65 0965 1119 0066 1864 1064 1184  .d.e.e...f.d.d..
+000005c0: 055a 1264 1265 136a 1464 1365 0664 1464  .Z.d.e.j.d.e.d.d
+000005d0: 0266 0664 1564 1684 045a 1564 1265 136a  .f.d.d...Z.d.e.j
+000005e0: 1464 1765 136a 1464 1865 136a 1664 1365  .d.e.j.d.e.j.d.e
+000005f0: 0664 1465 1765 0665 0c66 0219 0066 0a64  .d.e.e.e.f...f.d
+00000600: 1964 1a84 045a 1864 1265 136a 1464 1465  .d...Z.d.e.j.d.e
+00000610: 136a 1466 0464 1b64 1c84 045a 1964 1265  .j.f.d.d...Z.d.e
+00000620: 136a 1464 1465 1a65 1b6a 1c65 1b6a 1c66  .j.d.e.e.j.e.j.f
+00000630: 0219 0066 0464 1d64 1e84 045a 1d64 0253  ...f.d.d...Z.d.S
+00000640: 0029 20da 0842 6c75 6543 6173 7461 2206  .) ..BlueCasta".
+00000650: 0000 5275 6e20 6675 6c6c 7920 636f 6e66  ..Run fully conf
+00000660: 6967 7572 6564 2063 6c61 7373 6966 6963  igured classific
+00000670: 6174 696f 6e20 626c 7565 7072 696e 742e  ation blueprint.
+00000680: 0a0a 2020 2020 4375 7374 6f6d 697a 6174  ..    Customizat
+00000690: 696f 6e20 7669 6120 636c 6173 7320 6174  ion via class at
+000006a0: 7472 6962 7574 6573 2069 7320 706f 7373  tributes is poss
+000006b0: 6962 6c65 2e20 436f 6e66 6967 7320 6361  ible. Configs ca
+000006c0: 6e20 6265 2069 6e73 7461 6e74 6961 7465  n be instantiate
+000006d0: 6420 616e 6420 7072 6f76 6964 6564 2074  d and provided t
+000006e0: 6f20 6368 616e 6765 2058 6762 6f6f 7374  o change Xgboost
+000006f0: 2074 7261 696e 696e 672e 0a20 2020 2044   training..    D
+00000700: 6566 6175 6c74 2068 7970 6572 7061 7261  efault hyperpara
+00000710: 6d65 7465 7220 7365 6172 6368 2073 7061  meter search spa
+00000720: 6365 2069 7320 7265 6c61 7469 7665 6c79  ce is relatively
+00000730: 206c 6967 6874 2d77 6569 6768 7420 746f   light-weight to
+00000740: 2073 7065 6564 2075 7020 7468 6520 7072   speed up the pr
+00000750: 6f74 6f74 7970 696e 672e 0a20 2020 203a  ototyping..    :
+00000760: 7061 7261 6d20 3a63 6c61 7373 5f70 726f  param :class_pro
+00000770: 626c 656d 3a20 5461 6b65 7320 6120 7374  blem: Takes a st
+00000780: 7269 6e67 2063 6f6e 7461 696e 696e 6720  ring containing 
+00000790: 7468 6520 636c 6173 7320 7072 6f62 6c65  the class proble
+000007a0: 6d20 7479 7065 2e20 4569 7468 6572 2022  m type. Either "
+000007b0: 6269 6e61 7279 2220 6f72 2022 6d75 6c74  binary" or "mult
+000007c0: 6963 6c61 7373 222e 0a20 2020 203a 7061  iclass"..    :pa
+000007d0: 7261 6d20 3a74 6172 6765 745f 636f 6c75  ram :target_colu
+000007e0: 6d6e 3a20 5461 6b65 7320 6120 7374 7269  mn: Takes a stri
+000007f0: 6e67 2063 6f6e 7461 696e 696e 6720 7468  ng containing th
+00000800: 6520 6e61 6d65 206f 6620 7468 6520 7461  e name of the ta
+00000810: 7267 6574 2063 6f6c 756d 6e2e 0a20 2020  rget column..   
+00000820: 203a 7061 7261 6d20 3a63 6174 5f63 6f6c   :param :cat_col
+00000830: 756d 6e73 3a20 5461 6b65 7320 6120 6c69  umns: Takes a li
+00000840: 7374 206f 6620 7374 7269 6e67 7320 636f  st of strings co
+00000850: 6e74 6169 6e69 6e67 2074 6865 206e 616d  ntaining the nam
+00000860: 6573 206f 6620 7468 6520 6361 7465 676f  es of the catego
+00000870: 7269 6361 6c20 636f 6c75 6d6e 732e 2049  rical columns. I
+00000880: 6620 6e6f 7420 7072 6f76 6964 6564 2c0a  f not provided,.
+00000890: 2020 2020 426c 7565 4361 7374 2077 696c      BlueCast wil
+000008a0: 6c20 696e 6665 7220 7468 6573 6520 6175  l infer these au
+000008b0: 746f 6d61 6963 616c 6c79 2e0a 2020 2020  tomaically..    
+000008c0: 3a70 6172 616d 203a 6461 7465 5f63 6f6c  :param :date_col
+000008d0: 756d 6e73 3a20 5461 6b65 7320 6120 6c69  umns: Takes a li
+000008e0: 7374 206f 6620 7374 7269 6e67 7320 636f  st of strings co
+000008f0: 6e74 6169 6e69 6e67 2074 6865 206e 616d  ntaining the nam
+00000900: 6573 206f 6620 7468 6520 6461 7465 2063  es of the date c
+00000910: 6f6c 756d 6e73 2e20 4966 206e 6f74 2070  olumns. If not p
+00000920: 726f 7669 6465 642c 0a20 2020 2042 6c75  rovided,.    Blu
+00000930: 6543 6173 7420 7769 6c6c 2069 6e66 6572  eCast will infer
+00000940: 2074 6865 7365 2061 7574 6f6d 6169 6361   these automaica
+00000950: 6c6c 792e 0a20 2020 203a 7061 7261 6d20  lly..    :param 
+00000960: 3a74 696d 655f 7370 6c69 745f 636f 6c75  :time_split_colu
+00000970: 6d6e 3a20 5461 6b65 7320 6120 7374 7269  mn: Takes a stri
+00000980: 6e67 2063 6f6e 7461 696e 696e 6720 7468  ng containing th
+00000990: 6520 6e61 6d65 206f 6620 7468 6520 7469  e name of the ti
+000009a0: 6d65 2073 706c 6974 2063 6f6c 756d 6e2e  me split column.
+000009b0: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+000009c0: 2c0a 2020 2020 426c 7565 4361 7374 2077  ,.    BlueCast w
+000009d0: 696c 6c20 6e6f 7420 7370 6c69 7420 7468  ill not split th
+000009e0: 6520 6461 7461 2062 7920 7469 6d65 206f  e data by time o
+000009f0: 7220 6f72 6465 722c 2062 7574 2064 6f20  r order, but do 
+00000a00: 6120 7261 6e64 6f6d 2073 706c 6974 2069  a random split i
+00000a10: 6e73 7465 6164 2e0a 2020 2020 3a70 6172  nstead..    :par
+00000a20: 616d 203a 6d6c 5f6d 6f64 656c 3a20 5461  am :ml_model: Ta
+00000a30: 6b65 7320 616e 2069 6e73 7461 6e63 6520  kes an instance 
+00000a40: 6f66 2061 2058 6762 6f6f 7374 4d6f 6465  of a XgboostMode
+00000a50: 6c20 636c 6173 732e 2049 6620 6e6f 7420  l class. If not 
+00000a60: 7072 6f76 6964 6564 2c20 426c 7565 4361  provided, BlueCa
+00000a70: 7374 2077 696c 6c20 696e 7374 616e 7469  st will instanti
+00000a80: 6174 6520 6f6e 652e 0a20 2020 2054 6869  ate one..    Thi
+00000a90: 7320 6973 2061 6e20 4150 4920 746f 2070  s is an API to p
+00000aa0: 6173 7320 616e 7920 6d6f 6465 6c20 636c  ass any model cl
+00000ab0: 6173 732e 2049 6e68 6572 6974 2074 6865  ass. Inherit the
+00000ac0: 2062 6173 6563 6c61 7373 2066 726f 6d20   baseclass from 
+00000ad0: 6d6c 5f6d 6f64 656c 6c69 6e67 2e62 6173  ml_modelling.bas
+00000ae0: 655f 6d6f 6465 6c2e 4261 7365 4d6f 6465  e_model.BaseMode
+00000af0: 6c2e 0a20 2020 203a 7061 7261 6d20 6375  l..    :param cu
+00000b00: 7374 6f6d 5f70 7265 7072 6f63 6573 736f  stom_preprocesso
+00000b10: 723a 2054 616b 6573 2061 6e20 696e 7374  r: Takes an inst
+00000b20: 616e 6365 206f 6620 6120 4375 7374 6f6d  ance of a Custom
+00000b30: 5072 6570 726f 6365 7373 696e 6720 636c  Preprocessing cl
+00000b40: 6173 732e 2041 6c6c 6f77 7320 7573 6572  ass. Allows user
+00000b50: 7320 746f 2069 6e6a 6563 7420 6375 7374  s to inject cust
+00000b60: 6f6d 0a20 2020 2070 7265 7072 6f63 6573  om.    preproces
+00000b70: 7369 6e67 2073 7465 7073 2077 6869 6368  sing steps which
+00000b80: 2074 616b 6520 706c 6163 6520 7269 6768   take place righ
+00000b90: 7420 6166 7465 7220 7468 6520 7472 6169  t after the trai
+00000ba0: 6e20 7465 7374 2073 7069 742e 0a20 2020  n test spit..   
+00000bb0: 203a 7061 7261 6d20 6375 7374 6f6d 5f6c   :param custom_l
+00000bc0: 6173 745f 6d69 6c65 5f63 6f6d 7075 7461  ast_mile_computa
+00000bd0: 7469 6f6e 3a20 5461 6b65 7320 616e 2069  tion: Takes an i
+00000be0: 6e73 7461 6e63 6520 6f66 2061 2043 7573  nstance of a Cus
+00000bf0: 746f 6d50 7265 7072 6f63 6573 7369 6e67  tomPreprocessing
+00000c00: 2063 6c61 7373 2e20 416c 6c6f 7773 2075   class. Allows u
+00000c10: 7365 7273 2074 6f20 696e 6a65 6374 2063  sers to inject c
+00000c20: 7573 746f 6d0a 2020 2020 7072 6570 726f  ustom.    prepro
+00000c30: 6365 7373 696e 6720 7374 6570 7320 7768  cessing steps wh
+00000c40: 6963 6820 7461 6b65 2070 6c61 6365 2072  ich take place r
+00000c50: 6967 6874 2062 6566 6f72 6520 7468 6520  ight before the 
+00000c60: 6d6f 6465 6c20 7472 6169 6e69 6e67 2e0a  model training..
+00000c70: 2020 2020 4eda 0d63 6c61 7373 5f70 726f      N..class_pro
+00000c80: 626c 656d 2902 da06 6269 6e61 7279 da0a  blem)...binary..
+00000c90: 6d75 6c74 6963 6c61 7373 da0d 7461 7267  multiclass..targ
+00000ca0: 6574 5f63 6f6c 756d 6eda 0b63 6174 5f63  et_column..cat_c
+00000cb0: 6f6c 756d 6e73 da0c 6461 7465 5f63 6f6c  olumns..date_col
+00000cc0: 756d 6e73 da11 7469 6d65 5f73 706c 6974  umns..time_split
+00000cd0: 5f63 6f6c 756d 6eda 086d 6c5f 6d6f 6465  _column..ml_mode
+00000ce0: 6cda 1c63 7573 746f 6d5f 6c61 7374 5f6d  l..custom_last_m
+00000cf0: 696c 655f 636f 6d70 7574 6174 696f 6eda  ile_computation.
+00000d00: 1363 7573 746f 6d5f 7072 6570 726f 6365  .custom_preproce
+00000d10: 7373 6f72 da0d 636f 6e66 5f74 7261 696e  ssor..conf_train
+00000d20: 696e 67da 0c63 6f6e 665f 7867 626f 6f73  ing..conf_xgboos
+00000d30: 74da 1363 6f6e 665f 7061 7261 6d73 5f78  t..conf_params_x
+00000d40: 6762 6f6f 7374 da16 636f 6e66 5f66 6561  gboost..conf_fea
+00000d50: 7475 7265 5f73 656c 6563 7469 6f6e 630d  ture_selectionc.
+00000d60: 0000 0000 0000 0000 0000 000d 0000 0002  ................
+00000d70: 0000 0043 0000 0073 7600 0000 7c01 7c00  ...C...sv...|.|.
+00000d80: 5f00 6401 7c00 5f01 7c03 7c00 5f02 7c04  _.d.|._.|.|._.|.
+00000d90: 7c00 5f03 7c05 7c00 5f04 7c02 7c00 5f05  |._.|.|._.|.|._.
+00000da0: 7c09 7c00 5f06 7c0a 7c00 5f07 7c0b 7c00  |.|._.|.|._.|.|.
+00000db0: 5f08 7c0c 7c00 5f09 6400 7c00 5f0a 6400  _.|.|._.d.|._.d.
+00000dc0: 7c00 5f0b 6400 7c00 5f0c 6400 7c00 5f0d  |._.d.|._.d.|._.
+00000dd0: 6400 7c00 5f0e 7c06 7c00 5f0f 7c07 7c00  d.|._.|.|._.|.|.
+00000de0: 5f10 7c08 7c00 5f11 6400 7c00 5f12 6400  _.|.|._.d.|._.d.
+00000df0: 5300 2902 4e46 2913 721c 0000 00da 0f70  S.).NF).r......p
+00000e00: 7265 6469 6374 696f 6e5f 6d6f 6465 7220  rediction_moder 
+00000e10: 0000 0072 2100 0000 7222 0000 0072 1f00  ...r!...r"...r..
+00000e20: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
+00000e30: 0072 2900 0000 da10 6665 6174 7572 655f  .r).....feature_
+00000e40: 7365 6c65 6374 6f72 da12 6665 6174 5f74  selector..feat_t
+00000e50: 7970 655f 6465 7465 6374 6f72 da0b 6361  ype_detector..ca
+00000e60: 745f 656e 636f 6465 72da 1474 6172 6765  t_encoder..targe
+00000e70: 745f 6c61 6265 6c5f 656e 636f 6465 72da  t_label_encoder.
+00000e80: 0f73 6368 656d 615f 6465 7465 6374 6f72  .schema_detector
+00000e90: 7223 0000 0072 2400 0000 7225 0000 00da  r#...r$...r%....
+00000ea0: 0b73 6861 705f 7661 6c75 6573 290d da04  .shap_values)...
+00000eb0: 7365 6c66 721c 0000 0072 1f00 0000 7220  selfr....r....r 
+00000ec0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+00000ed0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+00000ee0: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
+00000ef0: a900 7232 0000 00fa 3e2f 686f 6d65 2f74  ..r2....>/home/t
+00000f00: 686f 6d61 732f 4964 6561 5072 6f6a 6563  homas/IdeaProjec
+00000f10: 7473 2f42 6c75 6543 6173 742f 626c 7565  ts/BlueCast/blue
+00000f20: 6361 7374 2f62 6c75 6570 7269 6e74 732f  cast/blueprints/
+00000f30: 6361 7374 2e70 79da 085f 5f69 6e69 745f  cast.py..__init_
+00000f40: 5f3b 0000 0073 2800 0000 060f 0601 0601  _;...s(.........
+00000f50: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00000f60: 0601 0203 04fe 0603 0601 0601 0601 0601  ................
+00000f70: 0a01 7a11 426c 7565 4361 7374 2e5f 5f69  ..z.BlueCast.__i
+00000f80: 6e69 745f 5fda 0264 66da 0a74 6172 6765  nit__..df..targe
+00000f90: 745f 636f 6cda 0672 6574 7572 6e63 0300  t_col..returnc..
+00000fa0: 0000 0000 0000 0000 0000 0900 0000 0700  ................
+00000fb0: 0000 4300 0000 73ce 0200 0074 0083 0001  ..C...s....t....
+00000fc0: 0074 0183 007d 037c 03a0 027c 01a1 017d  .t...}.|...|...}
+00000fd0: 017c 037c 005f 037c 006a 036a 0472 297c  .|.|._.|.j.j.r)|
+00000fe0: 006a 057c 006a 036a 0476 0072 2974 0683  .j.|.j.j.v.r)t..
+00000ff0: 007c 005f 077c 006a 07a0 087c 017c 006a  .|._.|.j...|.|.j
+00001000: 0519 00a1 017c 017c 006a 053c 007c 006a  .....|.|.j.<.|.j
+00001010: 036a 047c 005f 047c 006a 036a 097c 005f  .j.|._.|.j.j.|._
+00001020: 097c 006a 0a73 3a74 0b83 007c 005f 0a74  .|.j.s:t...|._.t
+00001030: 0c7c 017c 027c 006a 0d7c 006a 0a6a 0e7c  .|.|.|.j.|.j.j.|
+00001040: 006a 0a6a 0f7c 006a 0a6a 1083 065c 047d  .j.j.|.j.j...\.}
+00001050: 047d 057d 067d 077c 006a 1172 927c 006a  .}.}.}.|.j.r.|.j
+00001060: 11a0 127c 047c 06a1 025c 027d 047d 067c  ...|.|...\.}.}.|
+00001070: 006a 116a 137c 057c 0764 0164 028d 035c  .j.j.|.|.d.d...\
+00001080: 027d 057d 0774 0183 007d 037c 03a0 027c  .}.}.t...}.|...|
+00001090: 04a1 017d 087c 046a 1464 0364 048d 017c  ...}.|.j.d.d...|
+000010a0: 066a 1464 0364 048d 0102 027d 047d 067c  .j.d.d.....}.}.|
+000010b0: 056a 1464 0364 048d 017c 076a 1464 0364  .j.d.d...|.j.d.d
+000010c0: 048d 0102 027d 057d 077c 027c 036a 0476  .....}.}.|.|.j.v
+000010d0: 0072 927c 036a 04a0 157c 02a1 0101 0074  .r.|.j...|.....t
+000010e0: 167c 0483 0174 167c 0583 0102 027d 047d  .|...t.|.....}.}
+000010f0: 0574 177c 047c 006a 0983 0274 177c 057c  .t.|.|.j...t.|.|
+00001100: 006a 0983 0202 027d 047d 0574 1883 007c  .j.....}.}.t...|
+00001110: 005f 197c 006a 19a0 1a7c 04a1 0101 007c  ._.|.j...|.....|
+00001120: 006a 19a0 137c 05a1 017d 057c 006a 0464  .j...|...}.|.j.d
+00001130: 0575 0172 d67c 006a 1b64 066b 0272 d674  .u.r.|.j.d.k.r.t
+00001140: 1c7c 036a 0483 017c 005f 1d7c 006a 1da0  .|.j...|._.|.j..
+00001150: 1e7c 047c 06a1 027d 047c 006a 1da0 1f7c  .|.|...}.|.j...|
+00001160: 05a1 017d 056e 1d7c 006a 0464 0575 0172  ...}.n.|.j.d.u.r
+00001170: f37c 006a 1b64 076b 0272 f374 207c 036a  .|.j.d.k.r.t |.j
+00001180: 0483 017c 005f 1d7c 006a 1da0 217c 047c  ...|._.|.j..!|.|
+00001190: 06a1 027d 047c 006a 1da0 227c 05a1 017d  ...}.|.j.."|...}
+000011a0: 057c 006a 2390 0172 0b7c 006a 23a0 127c  .|.j#..r.|.j#..|
+000011b0: 047c 06a1 025c 027d 047d 067c 006a 236a  .|...\.}.}.|.j#j
+000011c0: 137c 057c 0764 0164 028d 035c 027d 057d  .|.|.d.d...\.}.}
+000011d0: 077c 006a 2490 0173 1374 2583 007c 005f  .|.j$..s.t%..|._
+000011e0: 247c 006a 246a 2690 0172 2074 277c 006a  $|.j$j&..r t'|.j
+000011f0: 246a 2864 088d 017c 005f 297c 006a 2990  $j(d...|._)|.j).
+00001200: 0172 367c 006a 246a 2690 0172 367c 006a  .r6|.j$j&..r6|.j
+00001210: 29a0 127c 047c 06a1 027d 047c 006a 29a0  )..|.|...}.|.j).
+00001220: 137c 05a1 017d 057c 006a 2a90 0173 4774  .|...}.|.j*..sGt
+00001230: 2b7c 006a 1b7c 006a 0a7c 006a 2c7c 006a  +|.j.|.j.|.j,|.j
+00001240: 2d64 098d 047c 005f 2a7c 006a 2aa0 1a7c  -d...|._*|.j*..|
+00001250: 047c 057c 067c 07a1 0401 007c 006a 0a90  .|.|.|.....|.j..
+00001260: 0172 627c 006a 0a6a 2e90 0172 6274 2f7c  .rb|.j.j...rbt/|
+00001270: 006a 2a6a 307c 0564 0a83 037c 005f 3164  .j*j0|.d...|._1d
+00001280: 037c 005f 3264 0553 0029 0b7a 1954 7261  .|._2d.S.).z.Tra
+00001290: 696e 2061 2066 756c 6c20 4d4c 2070 6970  in a full ML pip
+000012a0: 656c 696e 652e 46a9 01da 0e70 7265 6469  eline.F....predi
+000012b0: 6374 6f6e 5f6d 6f64 6554 a901 da04 6472  cton_modeT....dr
+000012c0: 6f70 4e72 1d00 0000 721e 0000 0029 01da  opNr....r....)..
+000012d0: 1273 656c 6563 7469 6f6e 5f73 7472 6174  .selection_strat
+000012e0: 6567 7929 0372 2600 0000 7227 0000 0072  egy).r&...r'...r
+000012f0: 2800 0000 da04 7472 6565 2933 720f 0000  (.....tree)3r...
+00001300: 0072 1500 0000 5a1b 6669 745f 7472 616e  .r....Z.fit_tran
+00001310: 7366 6f72 6d5f 6665 6174 7572 655f 7479  sform_feature_ty
+00001320: 7065 7372 2c00 0000 7220 0000 0072 1f00  pesr,...r ...r..
+00001330: 0000 7213 0000 0072 2e00 0000 5a1b 6669  ..r....r....Z.fi
+00001340: 745f 7472 616e 7366 6f72 6d5f 7461 7267  t_transform_targ
+00001350: 6574 5f6c 6162 656c 7372 2100 0000 7226  et_labelsr!...r&
+00001360: 0000 0072 0a00 0000 721a 0000 0072 2200  ...r....r....r".
+00001370: 0000 da0a 7472 6169 6e5f 7369 7a65 5a13  ....train_sizeZ.
+00001380: 676c 6f62 616c 5f72 616e 646f 6d5f 7374  global_random_st
+00001390: 6174 655a 1474 7261 696e 5f73 706c 6974  ateZ.train_split
+000013a0: 5f73 7472 6174 6966 7972 2500 0000 da0d  _stratifyr%.....
+000013b0: 6669 745f 7472 616e 7366 6f72 6dda 0974  fit_transform..t
+000013c0: 7261 6e73 666f 726d da0b 7265 7365 745f  ransform..reset_
+000013d0: 696e 6465 78da 0672 656d 6f76 6572 1600  index..remover..
+000013e0: 0000 7212 0000 0072 1700 0000 722f 0000  ..r....r....r/..
+000013f0: 00da 0366 6974 721c 0000 0072 1800 0000  ...fitr....r....
+00001400: 722d 0000 005a 1e66 6974 5f74 6172 6765  r-...Z.fit_targe
+00001410: 745f 656e 636f 6465 5f62 696e 6172 795f  t_encode_binary_
+00001420: 636c 6173 73da 2474 7261 6e73 666f 726d  class.$transform
+00001430: 5f74 6172 6765 745f 656e 636f 6465 5f62  _target_encode_b
+00001440: 696e 6172 795f 636c 6173 7372 1900 0000  inary_classr....
+00001450: 5a1c 6669 745f 7461 7267 6574 5f65 6e63  Z.fit_target_enc
+00001460: 6f64 655f 6d75 6c74 6963 6c61 7373 da22  ode_multiclass."
+00001470: 7472 616e 7366 6f72 6d5f 7461 7267 6574  transform_target
+00001480: 5f65 6e63 6f64 655f 6d75 6c74 6963 6c61  _encode_multicla
+00001490: 7373 7224 0000 0072 2900 0000 7209 0000  ssr$...r)...r...
+000014a0: 00da 1165 7865 6375 7465 5f73 656c 6563  ...execute_selec
+000014b0: 7469 6f6e 7214 0000 0072 3c00 0000 722b  tionr....r<...r+
+000014c0: 0000 0072 2300 0000 7210 0000 0072 2700  ...r#...r....r'.
+000014d0: 0000 7228 0000 005a 1563 616c 6375 6c61  ..r(...Z.calcula
+000014e0: 7465 5f73 6861 705f 7661 6c75 6573 720e  te_shap_valuesr.
+000014f0: 0000 00da 056d 6f64 656c 7230 0000 0072  .....modelr0...r
+00001500: 2a00 0000 2909 7231 0000 0072 3500 0000  *...).r1...r5...
+00001510: 7236 0000 0072 2c00 0000 da07 785f 7472  r6...r,.....x_tr
+00001520: 6169 6eda 0678 5f74 6573 74da 0779 5f74  ain..x_test..y_t
+00001530: 7261 696e da06 795f 7465 7374 da01 5f72  rain..y_test.._r
+00001540: 3200 0000 7232 0000 0072 3300 0000 7243  2...r2...r3...rC
+00001550: 0000 0060 0000 0073 a400 0000 0602 0601  ...`...s........
+00001560: 0a01 0601 0802 0e01 0801 0603 0801 02ff  ................
+00001570: 02fe 0401 02ff 0a06 0a01 0602 0801 0202  ................
+00001580: 0201 0201 0401 0601 0601 0601 0cfa 0609  ................
+00001590: 1201 0601 0601 0aff 0603 0a01 0e01 0201  ................
+000015a0: 0aff 0e03 0201 0aff 0a03 0c01 1202 0c01  ................
+000015b0: 0601 08ff 0804 0c01 0c01 1402 0c01 0e01  ................
+000015c0: 0e01 1401 0c01 0e01 0c01 0802 0601 0401  ................
+000015d0: 08ff 0603 0601 0aff 0804 0801 0a02 0201  ................
+000015e0: 0601 08ff 1204 0e01 0c01 0802 0201 0401  ................
+000015f0: 0401 0401 0401 08fc 1206 1201 1201 0a01  ................
+00001600: 7a0c 426c 7565 4361 7374 2e66 6974 da07  z.BlueCast.fit..
+00001610: 6466 5f65 7661 6cda 0b74 6172 6765 745f  df_eval..target_
+00001620: 6576 616c 6305 0000 0000 0000 0000 0000  evalc...........
+00001630: 0008 0000 0004 0000 0043 0000 0073 2a00  .........C...s*.
+00001640: 0000 7c00 a000 7c01 7c04 a102 0100 7c00  ..|...|.|.....|.
+00001650: a001 7c02 a101 5c02 7d05 7d06 7402 7c03  ..|...\.}.}.t.|.
+00001660: 6a03 7c06 8302 7d07 7c07 5300 2901 618e  j.|...}.|.S.).a.
+00001670: 0200 0054 7261 696e 2061 2066 756c 6c20  ...Train a full 
+00001680: 4d4c 2070 6970 656c 696e 6520 616e 6420  ML pipeline and 
+00001690: 6576 616c 7561 7465 206f 6e20 6120 686f  evaluate on a ho
+000016a0: 6c64 6f75 7420 7365 742e 0a0a 2020 2020  ldout set...    
+000016b0: 2020 2020 5468 6973 2069 7320 6120 636f      This is a co
+000016c0: 6e76 656e 6965 6e63 6520 6675 6e63 7469  nvenience functi
+000016d0: 6f6e 2074 6f20 7472 6169 6e20 616e 6420  on to train and 
+000016e0: 6576 616c 7561 7465 206f 6e20 6120 686f  evaluate on a ho
+000016f0: 6c64 6f75 7420 7365 742e 2049 7420 6973  ldout set. It is
+00001700: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
+00001710: 7573 6520 7468 6973 2066 6f72 206d 6f64  use this for mod
+00001720: 656c 0a20 2020 2020 2020 2065 7870 6c6f  el.        explo
+00001730: 7261 7469 6f6e 2e20 4f6e 2070 726f 6475  ration. On produ
+00001740: 6374 696f 6e20 7468 6520 7369 6d70 6c65  ction the simple
+00001750: 2066 6974 2829 2066 756e 6374 696f 6e20   fit() function 
+00001760: 7368 6f75 6c64 2062 6520 7573 6564 2e0a  should be used..
+00001770: 2020 2020 2020 2020 3a70 6172 616d 203a          :param :
+00001780: 6466 3a20 5461 6b65 7320 6120 7061 6e64  df: Takes a pand
+00001790: 6173 2044 6174 6146 7261 6d65 2063 6f6e  as DataFrame con
+000017a0: 7461 696e 696e 6720 7468 6520 7472 6169  taining the trai
+000017b0: 6e69 6e67 2064 6174 6120 616e 6420 7468  ning data and th
+000017c0: 6520 7461 7267 6574 732e 0a20 2020 2020  e targets..     
+000017d0: 2020 203a 7061 7261 6d20 3a64 665f 6576     :param :df_ev
+000017e0: 616c 3a20 5461 6b65 7320 6120 7061 6e64  al: Takes a pand
+000017f0: 6173 2044 6174 6146 7261 6d65 2063 6f6e  as DataFrame con
+00001800: 7461 696e 696e 6720 7468 6520 6576 616c  taining the eval
+00001810: 7561 7469 6f6e 2064 6174 612c 2062 7574  uation data, but
+00001820: 206e 6f74 2074 6865 2074 6172 6765 7473   not the targets
+00001830: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001840: 203a 7461 7267 6574 5f65 7661 6c3a 2054   :target_eval: T
+00001850: 616b 6573 2061 2070 616e 6461 7320 5365  akes a pandas Se
+00001860: 7269 6573 2063 6f6e 7461 696e 696e 6720  ries containing 
+00001870: 7468 6520 6576 616c 7561 7469 6f6e 2074  the evaluation t
+00001880: 6172 6765 7473 2e0a 2020 2020 2020 2020  argets..        
+00001890: 3a70 6172 616d 203a 7461 7267 6574 5f63  :param :target_c
+000018a0: 6f6c 3a20 5461 6b65 7320 6120 7374 7269  ol: Takes a stri
+000018b0: 6e67 2063 6f6e 7461 696e 696e 6720 7468  ng containing th
+000018c0: 6520 6e61 6d65 206f 6620 7468 6520 7461  e name of the ta
+000018d0: 7267 6574 2063 6f6c 756d 6e20 696e 7369  rget column insi
+000018e0: 6465 2074 6865 2074 7261 696e 696e 6720  de the training 
+000018f0: 6461 7461 2064 662e 0a20 2020 2020 2020  data df..       
+00001900: 2029 0472 4300 0000 da07 7072 6564 6963   ).rC.....predic
+00001910: 7472 0d00 0000 da06 7661 6c75 6573 2908  tr......values).
+00001920: 7231 0000 0072 3500 0000 724d 0000 0072  r1...r5...rM...r
+00001930: 4e00 0000 7236 0000 00da 0779 5f70 726f  N...r6.....y_pro
+00001940: 6273 da09 795f 636c 6173 7365 735a 0965  bs..y_classesZ.e
+00001950: 7661 6c5f 6469 6374 7232 0000 0072 3200  val_dictr2...r2.
+00001960: 0000 7233 0000 00da 0866 6974 5f65 7661  ..r3.....fit_eva
+00001970: 6cc1 0000 0073 0800 0000 0c10 0e01 0c01  l....s..........
+00001980: 0401 7a11 426c 7565 4361 7374 2e66 6974  ..z.BlueCast.fit
+00001990: 5f65 7661 6c63 0200 0000 0000 0000 0000  _evalc..........
+000019a0: 0000 0300 0000 0400 0000 4300 0000 7318  ..........C...s.
+000019b0: 0100 0074 0083 0001 007c 006a 0173 0a74  ...t.....|.j.s.t
+000019c0: 0264 0183 0182 017c 006a 016a 037c 017c  .d.....|.j.j.|.|
+000019d0: 006a 0467 0164 028d 027d 017c 006a 0572  .j.g.d...}.|.j.r
+000019e0: 277c 006a 056a 067c 0164 0364 048d 025c  '|.j.j.|.d.d...\
+000019f0: 027d 017d 027c 016a 0764 0364 058d 017d  .}.}.|.j.d.d...}
+00001a00: 0174 087c 0183 017d 0174 097c 017c 006a  .t.|...}.t.|.|.j
+00001a10: 0a83 027d 017c 006a 0b72 3a7c 006a 0ba0  ...}.|.j.r:|.j..
+00001a20: 067c 01a1 017d 017c 006a 0c72 527c 006a  .|...}.|.j.rR|.j
+00001a30: 0d72 527c 006a 0e64 066b 0272 5274 0f7c  .rR|.j.d.k.rRt.|
+00001a40: 006a 0d74 1083 0272 527c 006a 0da0 117c  .j.t...rR|.j...|
+00001a50: 01a1 017d 016e 177c 006a 0c72 697c 006a  ...}.n.|.j.ri|.j
+00001a60: 0d72 697c 006a 0e64 076b 0272 6974 0f7c  .ri|.j.d.k.rit.|
+00001a70: 006a 0d74 1283 0272 697c 006a 0da0 137c  .j.t...ri|.j...|
+00001a80: 01a1 017d 017c 006a 1472 767c 006a 146a  ...}.|.j.rv|.j.j
+00001a90: 067c 0164 0364 048d 025c 027d 017d 027c  .|.d.d...\.}.}.|
+00001aa0: 006a 1573 7d74 1683 007c 005f 157c 006a  .j.s}t...|._.|.j
+00001ab0: 1772 8a7c 006a 156a 1872 8a7c 006a 17a0  .r.|.j.j.r.|.j..
+00001ac0: 067c 01a1 017d 017c 0153 0029 087a 3754  .|...}.|.S.).z7T
+00001ad0: 7261 6e73 666f 726d 206e 6577 2064 6174  ransform new dat
+00001ae0: 6120 6163 636f 7264 696e 6720 746f 2070  a according to p
+00001af0: 7265 7072 6f63 6573 7369 6e67 2070 6970  reprocessing pip
+00001b00: 656c 696e 652e fa2a 4665 6174 7572 6520  eline..*Feature 
+00001b10: 7479 7065 2063 6f6e 7665 7274 6572 2063  type converter c
+00001b20: 6f75 6c64 206e 6f74 2062 6520 666f 756e  ould not be foun
+00001b30: 642e 2901 5a0b 6967 6e6f 7265 5f63 6f6c  d.).Z.ignore_col
+00001b40: 7354 7238 0000 0072 3a00 0000 721d 0000  sTr8...r:...r...
+00001b50: 0072 1e00 0000 2919 720f 0000 0072 2c00  .r....).r....r,.
+00001b60: 0000 da09 4578 6365 7074 696f 6e5a 1774  ....ExceptionZ.t
+00001b70: 7261 6e73 666f 726d 5f66 6561 7475 7265  ransform_feature
+00001b80: 5f74 7970 6573 721f 0000 0072 2500 0000  _typesr....r%...
+00001b90: 7240 0000 0072 4100 0000 7216 0000 0072  r@...rA...r....r
+00001ba0: 1200 0000 7221 0000 0072 2f00 0000 7220  ....r!...r/...r 
+00001bb0: 0000 0072 2d00 0000 721c 0000 00da 0a69  ...r-...r......i
+00001bc0: 7369 6e73 7461 6e63 6572 1800 0000 7244  sinstancer....rD
+00001bd0: 0000 0072 1900 0000 7245 0000 0072 2400  ...r....rE...r$.
+00001be0: 0000 7229 0000 0072 0900 0000 722b 0000  ..r)...r....r+..
+00001bf0: 0072 4600 0000 2903 7231 0000 0072 3500  .rF...).r1...r5.
+00001c00: 0000 724c 0000 0072 3200 0000 7232 0000  ..rL...r2...r2..
+00001c10: 0072 3300 0000 da12 7472 616e 7366 6f72  .r3.....transfor
+00001c20: 6d5f 6e65 775f 6461 7461 d600 0000 7348  m_new_data....sH
+00001c30: 0000 0006 0206 0108 0106 0208 0106 ff06  ................
+00001c40: 0414 010c 0108 020c 0106 020c 0104 0302  ................
+00001c50: ff04 0202 fe0a 030a 0102 ff0e 0304 0202  ................
+00001c60: ff04 0202 fe0a 030a 0102 ff0c 0306 0214  ................
+00001c70: 0106 0208 010e 020c 0104 027a 1b42 6c75  ...........z.Blu
+00001c80: 6543 6173 742e 7472 616e 7366 6f72 6d5f  eCast.transform_
+00001c90: 6e65 775f 6461 7461 6302 0000 0000 0000  new_datac.......
+00001ca0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+00001cb0: 0073 8000 0000 7c00 6a00 7307 7401 6401  .s....|.j.s.t.d.
+00001cc0: 8301 8201 7c00 6a02 730e 7401 6402 8301  ....|.j.s.t.d...
+00001cd0: 8201 7403 8300 0100 7c00 a004 7c01 a101  ..t.....|...|...
+00001ce0: 7d01 7405 6403 8301 0100 7c00 6a00 a006  }.t.d.....|.j...
+00001cf0: 7c01 a101 5c02 7d02 7d03 7c00 6a02 6a07  |...\.}.}.|.j.j.
+00001d00: 723c 7c00 6a08 7c00 6a02 6a07 7600 723c  r<|.j.|.j.j.v.r<
+00001d10: 7c00 6a09 723c 7c00 6a02 723c 7c00 6a09  |.j.r<|.j.r<|.j.
+00001d20: a00a 740b a00c 7c03 a101 a101 7d03 7c02  ..t...|.....}.|.
+00001d30: 7c03 6602 5300 2904 7a90 5072 6564 6963  |.f.S.).z.Predic
+00001d40: 7420 6f6e 2075 6e73 6565 6e20 6461 7461  t on unseen data
+00001d50: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00001d60: 6e20 7468 6520 7072 6564 6963 7465 6420  n the predicted 
+00001d70: 7072 6f62 6162 696c 6974 6965 7320 616e  probabilities an
+00001d80: 6420 7468 6520 7072 6564 6963 7465 6420  d the predicted 
+00001d90: 636c 6173 7365 733a 0a20 2020 2020 2020  classes:.       
+00001da0: 2079 5f70 726f 6273 2c20 795f 636c 6173   y_probs, y_clas
+00001db0: 7365 7320 3d20 7072 6564 6963 7428 6466  ses = predict(df
+00001dc0: 290a 2020 2020 2020 2020 7a1b 4d6c 206d  ).        z.Ml m
+00001dd0: 6f64 656c 2063 6f75 6c64 206e 6f74 2062  odel could not b
+00001de0: 6520 666f 756e 6472 5400 0000 7a0d 5072  e foundrT...z.Pr
+00001df0: 6564 6963 7469 6e67 2e2e 2e29 0d72 2300  edicting...).r#.
+00001e00: 0000 7255 0000 0072 2c00 0000 720f 0000  ..rU...r,...r...
+00001e10: 0072 5700 0000 da05 7072 696e 7472 4f00  .rW.....printrO.
+00001e20: 0000 7220 0000 0072 1f00 0000 722e 0000  ..r ...r....r...
+00001e30: 005a 1f6c 6162 656c 5f65 6e63 6f64 6572  .Z.label_encoder
+00001e40: 5f72 6576 6572 7365 5f74 7261 6e73 666f  _reverse_transfo
+00001e50: 726d da02 7064 da06 5365 7269 6573 2904  rm..pd..Series).
+00001e60: 7231 0000 0072 3500 0000 7251 0000 0072  r1...r5...rQ...r
+00001e70: 5200 0000 7232 0000 0072 3200 0000 7233  R...r2...r2...r3
+00001e80: 0000 0072 4f00 0000 0401 0000 7324 0000  ...rO.......s$..
+00001e90: 0006 0608 0106 0208 0106 020a 0108 0210  ................
+00001ea0: 0108 020e 0204 0102 ff04 0202 fe06 0408  ................
+00001eb0: 0104 ff08 047a 1042 6c75 6543 6173 742e  .....z.BlueCast.
+00001ec0: 7072 6564 6963 7429 0a4e 4e4e 4e4e 4e4e  predict).NNNNNNN
+00001ed0: 4e4e 4e29 1eda 085f 5f6e 616d 655f 5fda  NNN)...__name__.
+00001ee0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00001ef0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00001f00: 5f5f 7205 0000 0072 0800 0000 da03 7374  __r....r......st
+00001f10: 72da 0566 6c6f 6174 da03 696e 7472 0600  r..float..intr..
+00001f20: 0000 7204 0000 0072 1000 0000 7202 0000  ..r....r....r...
+00001f30: 0072 1100 0000 720a 0000 0072 0c00 0000  .r....r....r....
+00001f40: 720b 0000 0072 0900 0000 7234 0000 0072  r....r....r4...r
+00001f50: 5900 0000 da09 4461 7461 4672 616d 6572  Y.....DataFramer
+00001f60: 4300 0000 725a 0000 0072 0300 0000 7253  C...rZ...r....rS
+00001f70: 0000 0072 5700 0000 7207 0000 00da 026e  ...rW...r......n
+00001f80: 70da 076e 6461 7272 6179 724f 0000 0072  p..ndarrayrO...r
+00001f90: 3200 0000 7232 0000 0072 3200 0000 7233  2...r2...r2...r3
+00001fa0: 0000 0072 1b00 0000 2600 0000 7366 0000  ...r....&...sf..
+00001fb0: 0008 0004 0102 1802 0102 0102 0102 0102  ................
+00001fc0: 0102 0102 0102 0102 0104 f306 0202 fe0c  ................
+00001fd0: 0302 fd14 0402 fc14 0502 fb06 0602 fa0e  ................
+00001fe0: 0702 f906 0802 f806 0902 f706 0a02 f606  ................
+00001ff0: 0b02 f506 0c02 f406 0d0a f318 2502 6104  ............%.a.
+00002000: 0202 fe04 0302 fd04 0402 fc02 0502 fb0a  ................
+00002010: 060a fa16 1524 2e72 1b00 0000 292e 725e  .....$.r....).r^
+00002020: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
+00002030: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+00002040: 0600 0000 7207 0000 0072 0800 0000 da05  ....r....r......
+00002050: 6e75 6d70 7972 6300 0000 da06 7061 6e64  numpyrc.....pand
+00002060: 6173 7259 0000 00da 1f62 6c75 6563 6173  asrY.....bluecas
+00002070: 742e 636f 6e66 6967 2e74 7261 696e 696e  t.config.trainin
+00002080: 675f 636f 6e66 6967 7209 0000 0072 0a00  g_configr....r..
+00002090: 0000 720b 0000 0072 0c00 0000 5a20 626c  ..r....r....Z bl
+000020a0: 7565 6361 7374 2e65 7661 6c75 6174 696f  uecast.evaluatio
+000020b0: 6e2e 6576 616c 5f6d 6574 7269 6373 720d  n.eval_metricsr.
+000020c0: 0000 005a 1f62 6c75 6563 6173 742e 6576  ...Z.bluecast.ev
+000020d0: 616c 7561 7469 6f6e 2e73 6861 705f 7661  aluation.shap_va
+000020e0: 6c75 6573 720e 0000 005a 2462 6c75 6563  luesr....Z$bluec
+000020f0: 6173 742e 6765 6e65 7261 6c5f 7574 696c  ast.general_util
+00002100: 732e 6765 6e65 7261 6c5f 7574 696c 7372  s.general_utilsr
+00002110: 0f00 0000 5a1d 626c 7565 6361 7374 2e6d  ....Z.bluecast.m
+00002120: 6c5f 6d6f 6465 6c6c 696e 672e 7867 626f  l_modelling.xgbo
+00002130: 6f73 7472 1000 0000 da1d 626c 7565 6361  ostr......blueca
+00002140: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+00002150: 2e63 7573 746f 6d72 1100 0000 5a28 626c  .customr....Z(bl
+00002160: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
+00002170: 7369 6e67 2e64 6174 6574 696d 655f 6665  sing.datetime_fe
+00002180: 6174 7572 6573 7212 0000 005a 2b62 6c75  aturesr....Z+blu
+00002190: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
+000021a0: 696e 672e 656e 636f 6465 5f74 6172 6765  ing.encode_targe
+000021b0: 745f 6c61 6265 6c73 7213 0000 005a 2862  t_labelsr....Z(b
+000021c0: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
+000021d0: 7373 696e 672e 6665 6174 7572 655f 7365  ssing.feature_se
+000021e0: 6c65 6374 696f 6e72 1400 0000 5a24 626c  lectionr....Z$bl
+000021f0: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
+00002200: 7369 6e67 2e66 6561 7475 7265 5f74 7970  sing.feature_typ
+00002210: 6573 7215 0000 005a 2562 6c75 6563 6173  esr....Z%bluecas
+00002220: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
+00002230: 6e75 6c6c 735f 616e 645f 696e 6673 7216  nulls_and_infsr.
+00002240: 0000 005a 2462 6c75 6563 6173 742e 7072  ...Z$bluecast.pr
+00002250: 6570 726f 6365 7373 696e 672e 7363 6865  eprocessing.sche
+00002260: 6d61 5f63 6865 636b 7372 1700 0000 5a26  ma_checksr....Z&
+00002270: 626c 7565 6361 7374 2e70 7265 7072 6f63  bluecast.preproc
+00002280: 6573 7369 6e67 2e74 6172 6765 745f 656e  essing.target_en
+00002290: 636f 6469 6e67 7218 0000 0072 1900 0000  codingr....r....
+000022a0: 5a27 626c 7565 6361 7374 2e70 7265 7072  Z'bluecast.prepr
+000022b0: 6f63 6573 7369 6e67 2e74 7261 696e 5f74  ocessing.train_t
+000022c0: 6573 745f 7370 6c69 7472 1a00 0000 721b  est_splitr....r.
+000022d0: 0000 0072 3200 0000 7232 0000 0072 3200  ...r2...r2...r2.
+000022e0: 0000 7233 0000 00da 083c 6d6f 6475 6c65  ..r3.....<module
+000022f0: 3e01 0000 0073 2600 0000 0400 2408 0802  >....s&.....$...
+00002300: 0801 1802 0c06 0c01 0c01 0c01 0c01 0c01  ................
+00002310: 0c01 0c01 0c01 0c01 0c01 1001 0c04 1203  ................
```

### Comparing `bluecast-0.2/bluecast/blueprints/cast.py` & `bluecast-0.3/bluecast/blueprints/cast.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 """
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from bluecast.config.training_config import (
+    FeatureSelectionConfig,
     TrainingConfig,
     XgboostFinalParamConfig,
     XgboostTuneParamsConfig,
 )
 from bluecast.evaluation.eval_metrics import eval_classifier
 from bluecast.evaluation.shap_values import shap_explanations
 from bluecast.general_utils.general_utils import check_gpu_support
 from bluecast.ml_modelling.xgboost import XgboostModel
 from bluecast.preprocessing.custom import CustomPreprocessing
 from bluecast.preprocessing.datetime_features import date_converter
 from bluecast.preprocessing.encode_target_labels import TargetLabelEncoder
+from bluecast.preprocessing.feature_selection import FeatureSelector
 from bluecast.preprocessing.feature_types import FeatureTypeDetector
 from bluecast.preprocessing.nulls_and_infs import fill_infinite_values
 from bluecast.preprocessing.schema_checks import SchemaDetector
 from bluecast.preprocessing.target_encoding import (
     BinaryClassTargetEncoder,
     MultiClassTargetEncoder,
 )
@@ -63,24 +65,27 @@
         time_split_column: Optional[str] = None,
         ml_model: Optional[Union[XgboostModel, Any]] = None,
         custom_last_mile_computation: Optional[CustomPreprocessing] = None,
         custom_preprocessor: Optional[CustomPreprocessing] = None,
         conf_training: Optional[TrainingConfig] = None,
         conf_xgboost: Optional[XgboostTuneParamsConfig] = None,
         conf_params_xgboost: Optional[XgboostFinalParamConfig] = None,
+        conf_feature_selection: Optional[FeatureSelectionConfig] = None,
     ):
         self.class_problem = class_problem
         self.prediction_mode: bool = False
         self.cat_columns = cat_columns
         self.date_columns = date_columns
         self.time_split_column = time_split_column
         self.target_column = target_column
         self.conf_training = conf_training
         self.conf_xgboost = conf_xgboost
         self.conf_params_xgboost = conf_params_xgboost
+        self.conf_feature_selection = conf_feature_selection
+        self.feature_selector: Optional[FeatureSelector] = None
         self.feat_type_detector: Optional[FeatureTypeDetector] = None
         self.cat_encoder: Optional[
             Union[BinaryClassTargetEncoder, MultiClassTargetEncoder]
         ] = None
         self.target_label_encoder: Optional[TargetLabelEncoder] = None
         self.schema_detector: Optional[SchemaDetector] = None
         self.ml_model: Optional[XgboostModel] = ml_model
@@ -157,14 +162,26 @@
             x_train, y_train = self.custom_last_mile_computation.fit_transform(
                 x_train, y_train
             )
             x_test, y_test = self.custom_last_mile_computation.transform(
                 x_test, y_test, predicton_mode=False
             )
 
+        if not self.conf_feature_selection:
+            self.conf_feature_selection = FeatureSelectionConfig()
+
+        if self.conf_feature_selection.execute_selection:
+            self.feature_selector = FeatureSelector(
+                selection_strategy=self.conf_feature_selection.selection_strategy
+            )
+
+        if self.feature_selector and self.conf_feature_selection.execute_selection:
+            x_train = self.feature_selector.fit_transform(x_train, y_train)
+            x_test = self.feature_selector.transform(x_test)
+
         if not self.ml_model:
             self.ml_model = XgboostModel(
                 self.class_problem,
                 conf_training=self.conf_training,
                 conf_xgboost=self.conf_xgboost,
                 conf_params_xgboost=self.conf_params_xgboost,
             )
@@ -227,14 +244,21 @@
             and self.class_problem == "multiclass"
             and isinstance(self.cat_encoder, MultiClassTargetEncoder)
         ):
             df = self.cat_encoder.transform_target_encode_multiclass(df)
 
         if self.custom_last_mile_computation:
             df, _ = self.custom_last_mile_computation.transform(df, predicton_mode=True)
+
+        if not self.conf_feature_selection:
+            self.conf_feature_selection = FeatureSelectionConfig()
+
+        if self.feature_selector and self.conf_feature_selection.execute_selection:
+            df = self.feature_selector.transform(df)
+
         return df
 
     def predict(self, df: pd.DataFrame) -> Tuple[np.ndarray, np.ndarray]:
         """Predict on unseen data.
 
         Return the predicted probabilities and the predicted classes:
         y_probs, y_classes = predict(df)
```

### Comparing `bluecast-0.2/bluecast/config/__pycache__/training_config.cpython-310.pyc` & `bluecast-0.3/bluecast/config/__pycache__/training_config.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 2726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 a60a 0000  o..........d....
+00000000: 550d 0d0a 0000 0000 f058 8164 a60a 0000  U........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6505  ..d.d.l.m.Z...e.
 00000050: 4700 6404 6405 8400 6405 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 6505 4700 6406 6407 8400 6407 8302 8301  e.G.d.d...d.....
 00000070: 5a07 6505 4700 6408 6409 8400 6409 8302  Z.e.G.d.d...d...
@@ -69,149 +69,142 @@
 00000440: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00000450: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
 00000460: 635f 5f72 0700 0000 da03 696e 74da 0f5f  c__r......int.._
 00000470: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 7208  _annotations__r.
 00000480: 0000 00da 0462 6f6f 6c72 0a00 0000 720b  .....boolr....r.
 00000490: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
 000004a0: 0000 7210 0000 00a9 0072 1800 0000 7218  ..r......r....r.
-000004b0: 0000 00fa 4e2f 5573 6572 732f 7468 6f6d  ....N/Users/thom
-000004c0: 6173 6d65 6973 736e 6572 2f49 6465 6150  asmeissner/IdeaP
-000004d0: 726f 6a65 6374 732f 426c 7565 4361 7374  rojects/BlueCast
-000004e0: 2f62 6c75 6563 6173 742f 636f 6e66 6967  /bluecast/config
-000004f0: 2f74 7261 696e 696e 675f 636f 6e66 6967  /training_config
-00000500: 2e70 7972 0500 0000 0d00 0000 7314 0000  .pyr........s...
-00000510: 000a 0004 020c 020c 010c 010c 010c 010c  ................
-00000520: 010c 0110 0172 0500 0000 6300 0000 0000  .....r....c.....
-00000530: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000540: 0000 0073 4a01 0000 6500 5a01 6400 5a02  ...sJ...e.Z.d.Z.
-00000550: 5500 6401 5a03 6402 5a04 6505 6506 6403  U.d.Z.d.Z.e.e.d.
-00000560: 3c00 6404 5a07 6505 6506 6405 3c00 6406  <.d.Z.e.e.d.<.d.
-00000570: 5a08 6509 6506 6407 3c00 6408 5a0a 6509  Z.e.e.d.<.d.Z.e.
-00000580: 6506 6409 3c00 6406 5a0b 6509 6506 640a  e.d.<.d.Z.e.e.d.
-00000590: 3c00 6408 5a0c 6509 6506 640b 3c00 6402  <.d.Z.e.e.d.<.d.
-000005a0: 5a0d 6505 6506 640c 3c00 640d 5a0e 6505  Z.e.e.d.<.d.Z.e.
-000005b0: 6506 640e 3c00 640f 5a0f 6509 6506 6410  e.d.<.d.Z.e.e.d.
-000005c0: 3c00 6406 5a10 6509 6506 6411 3c00 640f  <.d.Z.e.e.d.<.d.
-000005d0: 5a11 6509 6506 6412 3c00 6406 5a12 6509  Z.e.e.d.<.d.Z.e.
-000005e0: 6506 6413 3c00 640f 5a13 6509 6506 6414  e.d.<.d.Z.e.e.d.
-000005f0: 3c00 6406 5a14 6509 6506 6415 3c00 640f  <.d.Z.e.e.d.<.d.
-00000600: 5a15 6509 6506 6416 3c00 6406 5a16 6509  Z.e.e.d.<.d.Z.e.
-00000610: 6506 6417 3c00 6402 5a17 6505 6506 6418  e.d.<.d.Z.e.e.d.
-00000620: 3c00 6419 5a18 6505 6506 641a 3c00 641b  <.d.Z.e.e.d.<.d.
-00000630: 5a19 6509 6506 641c 3c00 6402 5a1a 6505  Z.e.e.d.<.d.Z.e.
-00000640: 6506 641d 3c00 641e 5a1b 6505 6506 641f  e.d.<.d.Z.e.e.d.
-00000650: 3c00 6420 5a1c 6505 6506 6421 3c00 6404  <.d Z.e.e.d!<.d.
-00000660: 5a1d 6505 6506 6422 3c00 6423 5a1e 6505  Z.e.e.d"<.d#Z.e.
-00000670: 6506 6424 3c00 6425 5a1f 6520 6506 6426  e.d$<.d%Z.e e.d&
-00000680: 3c00 6427 5a21 6520 6506 6428 3c00 6429  <.d'Z!e e.d(<.d)
-00000690: 5300 292a da17 5867 626f 6f73 7454 756e  S.)*..XgboostTun
-000006a0: 6550 6172 616d 7343 6f6e 6669 677a 2a44  eParamsConfigz*D
-000006b0: 6566 696e 6520 6879 7065 7270 6172 616d  efine hyperparam
-000006c0: 6574 6572 2074 756e 696e 6720 7365 6172  eter tuning sear
-000006d0: 6368 2073 7061 6365 2ee9 0200 0000 da0d  ch space........
-000006e0: 6d61 785f 6465 7074 685f 6d69 6ee9 0300  max_depth_min...
-000006f0: 0000 da0d 6d61 785f 6465 7074 685f 6d61  ....max_depth_ma
-00000700: 7867 0000 0000 0000 f03f da09 616c 7068  xg.......?..alph
-00000710: 615f 6d69 6e67 0000 0000 0040 8f40 da09  a_ming.....@.@..
-00000720: 616c 7068 615f 6d61 78da 0a6c 616d 6264  alpha_max..lambd
-00000730: 615f 6d69 6eda 0a6c 616d 6264 615f 6d61  a_min..lambda_ma
-00000740: 78da 0e6e 756d 5f6c 6561 7665 735f 6d69  x..num_leaves_mi
-00000750: 6ee9 4000 0000 da0e 6e75 6d5f 6c65 6176  n.@.....num_leav
-00000760: 6573 5f6d 6178 6733 3333 3333 33d3 3fda  es_maxg333333.?.
-00000770: 0e73 7562 5f73 616d 706c 655f 6d69 6eda  .sub_sample_min.
-00000780: 0e73 7562 5f73 616d 706c 655f 6d61 78da  .sub_sample_max.
-00000790: 1663 6f6c 5f73 616d 706c 655f 6279 5f74  .col_sample_by_t
-000007a0: 7265 655f 6d69 6eda 1663 6f6c 5f73 616d  ree_min..col_sam
-000007b0: 706c 655f 6279 5f74 7265 655f 6d61 78da  ple_by_tree_max.
-000007c0: 1763 6f6c 5f73 616d 706c 655f 6279 5f6c  .col_sample_by_l
-000007d0: 6576 656c 5f6d 696e da17 636f 6c5f 7361  evel_min..col_sa
-000007e0: 6d70 6c65 5f62 795f 6c65 7665 6c5f 6d61  mple_by_level_ma
-000007f0: 78da 1663 6f6c 5f73 616d 706c 655f 6279  x..col_sample_by
-00000800: 5f6e 6f64 655f 6d69 6eda 1663 6f6c 5f73  _node_min..col_s
-00000810: 616d 706c 655f 6279 5f6e 6f64 655f 6d61  ample_by_node_ma
-00000820: 78da 156d 696e 5f63 6869 6c64 5f73 616d  x..min_child_sam
-00000830: 706c 6573 5f6d 696e e9e8 0300 00da 156d  ples_min.......m
-00000840: 696e 5f63 6869 6c64 5f73 616d 706c 6573  in_child_samples
-00000850: 5f6d 6178 e79a 9999 9999 99b9 3fda 0365  _max........?..e
-00000860: 7461 da09 7374 6570 735f 6d69 6e69 50c3  ta..steps_miniP.
-00000870: 0000 da09 7374 6570 735f 6d61 7872 0c00  ....steps_maxr..
-00000880: 0000 da15 6e75 6d5f 7061 7261 6c6c 656c  ....num_parallel
-00000890: 5f74 7265 655f 6d69 6eda 156e 756d 5f70  _tree_min..num_p
-000008a0: 6172 616c 6c65 6c5f 7472 6565 5f6d 6178  arallel_tree_max
-000008b0: 7201 0000 00da 0f6d 6f64 656c 5f76 6572  r......model_ver
-000008c0: 626f 7369 7479 fa0e 6d75 6c74 693a 736f  bosity..multi:so
-000008d0: 6674 7072 6f62 da0f 6d6f 6465 6c5f 6f62  ftprob..model_ob
-000008e0: 6a65 6374 6976 65da 086d 6c6f 676c 6f73  jective..mloglos
-000008f0: 73da 116d 6f64 656c 5f65 7661 6c5f 6d65  s..model_eval_me
-00000900: 7472 6963 4e29 2272 1100 0000 7212 0000  tricN)"r....r...
-00000910: 0072 1300 0000 7214 0000 0072 1c00 0000  .r....r....r....
-00000920: 7215 0000 0072 1600 0000 721e 0000 0072  r....r....r....r
-00000930: 1f00 0000 da05 666c 6f61 7472 2000 0000  ......floatr ...
-00000940: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
-00000950: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
-00000960: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-00000970: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-00000980: 0072 3000 0000 7232 0000 0072 3300 0000  .r0...r2...r3...
-00000990: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
-000009a0: 3700 0000 7239 0000 00da 0373 7472 723b  7...r9.....strr;
-000009b0: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-000009c0: 0000 7219 0000 0072 1a00 0000 1b00 0000  ..r....r........
-000009d0: 7338 0000 000a 0004 020c 020c 010c 010c  s8..............
-000009e0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-000009f0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000a00: 010c 010c 010c 010c 010c 0110 0172 1a00  .............r..
-00000a10: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000a20: 0000 0004 0000 0040 0000 0073 a000 0000  .......@...s....
-00000a30: 6500 5a01 6400 5a02 5500 6401 5a03 6900  e.Z.d.Z.U.d.Z.i.
-00000a40: 6402 6403 9301 6404 6405 9301 6406 6407  d.d...d.d...d.d.
-00000a50: 9301 6408 6409 9301 640a 640b 9301 640c  ..d.d...d.d...d.
-00000a60: 640d 9301 640e 640f 9301 6410 640f 9301  d...d.d...d.d...
-00000a70: 6411 6412 9301 6413 6414 9301 6415 6414  d.d...d.d...d.d.
-00000a80: 9301 6416 6414 9301 6417 6414 9301 6418  ..d.d...d.d...d.
-00000a90: 6419 9301 641a 640f 9301 641b 641c 9301  d...d.d...d.d...
-00000aa0: 641d 641e 9301 5a04 641f 5a05 6506 6507  d.d...Z.d.Z.e.e.
-00000ab0: 6508 6509 6602 1900 1900 650a 6420 3c00  e.e.f.....e.d <.
-00000ac0: 6421 5a0b 6509 650a 6422 3c00 641f 5300  d!Z.e.e.d"<.d.S.
-00000ad0: 2923 da17 5867 626f 6f73 7446 696e 616c  )#..XgboostFinal
-00000ae0: 5061 7261 6d43 6f6e 6669 677a 1e44 6566  ParamConfigz.Def
-00000af0: 696e 6520 6669 6e61 6c20 6879 7065 7220  ine final hyper 
-00000b00: 7061 7261 6d65 7465 7273 2e5a 096f 626a  parameters.Z.obj
-00000b10: 6563 7469 7665 7238 0000 005a 0b65 7661  ectiver8...Z.eva
-00000b20: 6c5f 6d65 7472 6963 723a 0000 00da 0776  l_metricr:.....v
-00000b30: 6572 626f 7365 7201 0000 005a 0b74 7265  erboser....Z.tre
-00000b40: 655f 6d65 7468 6f64 da05 6578 6163 745a  e_method..exactZ
-00000b50: 096e 756d 5f63 6c61 7373 721b 0000 00da  .num_classr.....
-00000b60: 096d 6178 5f64 6570 7468 721d 0000 00da  .max_depthr.....
-00000b70: 0561 6c70 6861 7231 0000 00da 066c 616d  .alphar1.....lam
-00000b80: 6264 615a 0a6e 756d 5f6c 6561 7665 73e9  bdaZ.num_leaves.
-00000b90: 1000 0000 5a09 7375 6273 616d 706c 6567  ....Z.subsampleg
-00000ba0: 9a99 9999 9999 e93f 5a10 636f 6c73 616d  .......?Z.colsam
-00000bb0: 706c 655f 6279 7472 6565 5a11 636f 6c73  ple_bytreeZ.cols
-00000bc0: 616d 706c 655f 6279 6c65 7665 6c5a 1063  ample_bylevelZ.c
-00000bd0: 6f6c 7361 6d70 6c65 5f62 796e 6f64 655a  olsample_bynodeZ
-00000be0: 116d 696e 5f63 6869 6c64 5f73 616d 706c  .min_child_sampl
-00000bf0: 6573 7209 0000 0072 3200 0000 5a05 7374  esr....r2...Z.st
-00000c00: 6570 7372 2f00 0000 5a11 6e75 6d5f 7061  epsr/...Z.num_pa
-00000c10: 7261 6c6c 656c 5f74 7265 6572 0c00 0000  rallel_treer....
-00000c20: 4eda 0d73 616d 706c 655f 7765 6967 6874  N..sample_weight
-00000c30: 6700 0000 0000 00e0 3fda 1863 6c61 7373  g.......?..class
-00000c40: 6966 6963 6174 696f 6e5f 7468 7265 7368  ification_thresh
-00000c50: 6f6c 6429 0c72 1100 0000 7212 0000 0072  old).r....r....r
-00000c60: 1300 0000 7214 0000 00da 0670 6172 616d  ....r......param
-00000c70: 7372 4500 0000 7203 0000 0072 0200 0000  srE...r....r....
-00000c80: 723d 0000 0072 3c00 0000 7216 0000 0072  r=...r<...r....r
-00000c90: 4600 0000 7218 0000 0072 1800 0000 7218  F...r....r....r.
-00000ca0: 0000 0072 1900 0000 723e 0000 003b 0000  ...r....r>...;..
-00000cb0: 0073 4e00 0000 0a00 0402 0202 0401 02ff  .sN.............
-00000cc0: 0402 02fe 0403 02fd 0404 02fc 0405 02fb  ................
-00000cd0: 0406 02fa 0407 02f9 0408 02f8 0409 02f7  ................
-00000ce0: 040a 02f6 040b 02f5 040c 02f4 040d 02f3  ................
-00000cf0: 040e 02f2 040f 02f1 0410 02f0 0411 04ef  ................
-00000d00: 1813 1001 723e 0000 004e 2909 7214 0000  ....r>...N).r...
-00000d10: 00da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
-00000d20: 0000 005a 1470 7964 616e 7469 632e 6461  ...Z.pydantic.da
-00000d30: 7461 636c 6173 7365 7372 0400 0000 7205  taclassesr....r.
-00000d40: 0000 0072 1a00 0000 723e 0000 0072 1800  ...r....r>...r..
-00000d50: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000d60: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000d70: 1200 0000 0400 1007 0c02 0203 1001 020d  ................
-00000d80: 1001 021f 1401                           ......
+000004b0: 0000 00fa 452f 686f 6d65 2f74 686f 6d61  ....E/home/thoma
+000004c0: 732f 4964 6561 5072 6f6a 6563 7473 2f42  s/IdeaProjects/B
+000004d0: 6c75 6543 6173 742f 626c 7565 6361 7374  lueCast/bluecast
+000004e0: 2f63 6f6e 6669 672f 7472 6169 6e69 6e67  /config/training
+000004f0: 5f63 6f6e 6669 672e 7079 7205 0000 000d  _config.pyr.....
+00000500: 0000 0073 1200 0000 0a02 0402 0c01 0c01  ...s............
+00000510: 0c01 0c01 0c01 0c01 0c01 7205 0000 0063  ..........r....c
+00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000530: 0300 0000 4000 0000 734a 0100 0065 005a  ....@...sJ...e.Z
+00000540: 0164 005a 0255 0064 015a 0364 025a 0465  .d.Z.U.d.Z.d.Z.e
+00000550: 0565 0664 033c 0064 045a 0765 0565 0664  .e.d.<.d.Z.e.e.d
+00000560: 053c 0064 065a 0865 0965 0664 073c 0064  .<.d.Z.e.e.d.<.d
+00000570: 085a 0a65 0965 0664 093c 0064 065a 0b65  .Z.e.e.d.<.d.Z.e
+00000580: 0965 0664 0a3c 0064 085a 0c65 0965 0664  .e.d.<.d.Z.e.e.d
+00000590: 0b3c 0064 025a 0d65 0565 0664 0c3c 0064  .<.d.Z.e.e.d.<.d
+000005a0: 0d5a 0e65 0565 0664 0e3c 0064 0f5a 0f65  .Z.e.e.d.<.d.Z.e
+000005b0: 0965 0664 103c 0064 065a 1065 0965 0664  .e.d.<.d.Z.e.e.d
+000005c0: 113c 0064 0f5a 1165 0965 0664 123c 0064  .<.d.Z.e.e.d.<.d
+000005d0: 065a 1265 0965 0664 133c 0064 0f5a 1365  .Z.e.e.d.<.d.Z.e
+000005e0: 0965 0664 143c 0064 065a 1465 0965 0664  .e.d.<.d.Z.e.e.d
+000005f0: 153c 0064 0f5a 1565 0965 0664 163c 0064  .<.d.Z.e.e.d.<.d
+00000600: 065a 1665 0965 0664 173c 0064 025a 1765  .Z.e.e.d.<.d.Z.e
+00000610: 0565 0664 183c 0064 195a 1865 0565 0664  .e.d.<.d.Z.e.e.d
+00000620: 1a3c 0064 1b5a 1965 0965 0664 1c3c 0064  .<.d.Z.e.e.d.<.d
+00000630: 025a 1a65 0565 0664 1d3c 0064 1e5a 1b65  .Z.e.e.d.<.d.Z.e
+00000640: 0565 0664 1f3c 0064 205a 1c65 0565 0664  .e.d.<.d Z.e.e.d
+00000650: 213c 0064 045a 1d65 0565 0664 223c 0064  !<.d.Z.e.e.d"<.d
+00000660: 235a 1e65 0565 0664 243c 0064 255a 1f65  #Z.e.e.d$<.d%Z.e
+00000670: 2065 0664 263c 0064 275a 2165 2065 0664   e.d&<.d'Z!e e.d
+00000680: 283c 0064 2953 0029 2ada 1758 6762 6f6f  (<.d)S.)*..Xgboo
+00000690: 7374 5475 6e65 5061 7261 6d73 436f 6e66  stTuneParamsConf
+000006a0: 6967 7a2a 4465 6669 6e65 2068 7970 6572  igz*Define hyper
+000006b0: 7061 7261 6d65 7465 7220 7475 6e69 6e67  parameter tuning
+000006c0: 2073 6561 7263 6820 7370 6163 652e e902   search space...
+000006d0: 0000 00da 0d6d 6178 5f64 6570 7468 5f6d  .....max_depth_m
+000006e0: 696e e903 0000 00da 0d6d 6178 5f64 6570  in.......max_dep
+000006f0: 7468 5f6d 6178 6700 0000 0000 00f0 3fda  th_maxg.......?.
+00000700: 0961 6c70 6861 5f6d 696e 6700 0000 0000  .alpha_ming.....
+00000710: 408f 40da 0961 6c70 6861 5f6d 6178 da0a  @.@..alpha_max..
+00000720: 6c61 6d62 6461 5f6d 696e da0a 6c61 6d62  lambda_min..lamb
+00000730: 6461 5f6d 6178 da0e 6e75 6d5f 6c65 6176  da_max..num_leav
+00000740: 6573 5f6d 696e e940 0000 00da 0e6e 756d  es_min.@.....num
+00000750: 5f6c 6561 7665 735f 6d61 7867 3333 3333  _leaves_maxg3333
+00000760: 3333 d33f da0e 7375 625f 7361 6d70 6c65  33.?..sub_sample
+00000770: 5f6d 696e da0e 7375 625f 7361 6d70 6c65  _min..sub_sample
+00000780: 5f6d 6178 da16 636f 6c5f 7361 6d70 6c65  _max..col_sample
+00000790: 5f62 795f 7472 6565 5f6d 696e da16 636f  _by_tree_min..co
+000007a0: 6c5f 7361 6d70 6c65 5f62 795f 7472 6565  l_sample_by_tree
+000007b0: 5f6d 6178 da17 636f 6c5f 7361 6d70 6c65  _max..col_sample
+000007c0: 5f62 795f 6c65 7665 6c5f 6d69 6eda 1763  _by_level_min..c
+000007d0: 6f6c 5f73 616d 706c 655f 6279 5f6c 6576  ol_sample_by_lev
+000007e0: 656c 5f6d 6178 da16 636f 6c5f 7361 6d70  el_max..col_samp
+000007f0: 6c65 5f62 795f 6e6f 6465 5f6d 696e da16  le_by_node_min..
+00000800: 636f 6c5f 7361 6d70 6c65 5f62 795f 6e6f  col_sample_by_no
+00000810: 6465 5f6d 6178 da15 6d69 6e5f 6368 696c  de_max..min_chil
+00000820: 645f 7361 6d70 6c65 735f 6d69 6ee9 e803  d_samples_min...
+00000830: 0000 da15 6d69 6e5f 6368 696c 645f 7361  ....min_child_sa
+00000840: 6d70 6c65 735f 6d61 78e7 9a99 9999 9999  mples_max.......
+00000850: b93f da03 6574 61da 0973 7465 7073 5f6d  .?..eta..steps_m
+00000860: 696e 6950 c300 00da 0973 7465 7073 5f6d  iniP.....steps_m
+00000870: 6178 720c 0000 00da 156e 756d 5f70 6172  axr......num_par
+00000880: 616c 6c65 6c5f 7472 6565 5f6d 696e da15  allel_tree_min..
+00000890: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
+000008a0: 655f 6d61 7872 0100 0000 da0f 6d6f 6465  e_maxr......mode
+000008b0: 6c5f 7665 7262 6f73 6974 79fa 0e6d 756c  l_verbosity..mul
+000008c0: 7469 3a73 6f66 7470 726f 62da 0f6d 6f64  ti:softprob..mod
+000008d0: 656c 5f6f 626a 6563 7469 7665 da08 6d6c  el_objective..ml
+000008e0: 6f67 6c6f 7373 da11 6d6f 6465 6c5f 6576  ogloss..model_ev
+000008f0: 616c 5f6d 6574 7269 634e 2922 7211 0000  al_metricN)"r...
+00000900: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000910: 721c 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000920: 1e00 0000 721f 0000 00da 0566 6c6f 6174  ....r......float
+00000930: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
+00000940: 2300 0000 7225 0000 0072 2600 0000 7227  #...r%...r&...r'
+00000950: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
+00000960: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00000970: 0072 2e00 0000 7230 0000 0072 3200 0000  .r....r0...r2...
+00000980: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
+00000990: 3600 0000 7237 0000 0072 3900 0000 da03  6...r7...r9.....
+000009a0: 7374 7272 3b00 0000 7218 0000 0072 1800  strr;...r....r..
+000009b0: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
+000009c0: 001b 0000 0073 3600 0000 0a02 0402 0c01  .....s6.........
+000009d0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000009e0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+000009f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000a00: 721a 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000a10: 0000 0000 0000 1200 0000 4000 0000 735e  ..........@...s^
+00000a20: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00000a30: 0364 0264 0364 0464 0564 0664 0764 0864  .d.d.d.d.d.d.d.d
+00000a40: 0864 0964 0a64 0a64 0a64 0a64 0b64 0864  .d.d.d.d.d.d.d.d
+00000a50: 0c64 0d64 0e9c 115a 0464 0f5a 0565 0665  .d.d...Z.d.Z.e.e
+00000a60: 0765 0865 0966 0219 0019 0065 0a64 103c  .e.e.f.....e.d.<
+00000a70: 0064 115a 0b65 0965 0a64 123c 0064 0f53  .d.Z.e.e.d.<.d.S
+00000a80: 0029 13da 1758 6762 6f6f 7374 4669 6e61  .)...XgboostFina
+00000a90: 6c50 6172 616d 436f 6e66 6967 7a1e 4465  lParamConfigz.De
+00000aa0: 6669 6e65 2066 696e 616c 2068 7970 6572  fine final hyper
+00000ab0: 2070 6172 616d 6574 6572 732e 7238 0000   parameters.r8..
+00000ac0: 0072 3a00 0000 7201 0000 00da 0565 7861  .r:...r......exa
+00000ad0: 6374 721b 0000 0072 1d00 0000 7231 0000  ctr....r....r1..
+00000ae0: 00e9 1000 0000 679a 9999 9999 99e9 3f72  ......g.......?r
+00000af0: 0900 0000 722f 0000 0072 0c00 0000 2911  ....r/...r....).
+00000b00: da09 6f62 6a65 6374 6976 65da 0b65 7661  ..objective..eva
+00000b10: 6c5f 6d65 7472 6963 da07 7665 7262 6f73  l_metric..verbos
+00000b20: 65da 0b74 7265 655f 6d65 7468 6f64 da09  e..tree_method..
+00000b30: 6e75 6d5f 636c 6173 73da 096d 6178 5f64  num_class..max_d
+00000b40: 6570 7468 da05 616c 7068 61da 066c 616d  epth..alpha..lam
+00000b50: 6264 61da 0a6e 756d 5f6c 6561 7665 73da  bda..num_leaves.
+00000b60: 0973 7562 7361 6d70 6c65 da10 636f 6c73  .subsample..cols
+00000b70: 616d 706c 655f 6279 7472 6565 da11 636f  ample_bytree..co
+00000b80: 6c73 616d 706c 655f 6279 6c65 7665 6cda  lsample_bylevel.
+00000b90: 1063 6f6c 7361 6d70 6c65 5f62 796e 6f64  .colsample_bynod
+00000ba0: 65da 116d 696e 5f63 6869 6c64 5f73 616d  e..min_child_sam
+00000bb0: 706c 6573 7232 0000 00da 0573 7465 7073  plesr2.....steps
+00000bc0: da11 6e75 6d5f 7061 7261 6c6c 656c 5f74  ..num_parallel_t
+00000bd0: 7265 654e da0d 7361 6d70 6c65 5f77 6569  reeN..sample_wei
+00000be0: 6768 7467 0000 0000 0000 e03f da18 636c  ghtg.......?..cl
+00000bf0: 6173 7369 6669 6361 7469 6f6e 5f74 6872  assification_thr
+00000c00: 6573 686f 6c64 290c 7211 0000 0072 1200  eshold).r....r..
+00000c10: 0000 7213 0000 0072 1400 0000 da06 7061  ..r....r......pa
+00000c20: 7261 6d73 7251 0000 0072 0300 0000 7202  ramsrQ...r....r.
+00000c30: 0000 0072 3d00 0000 723c 0000 0072 1600  ...r=...r<...r..
+00000c40: 0000 7252 0000 0072 1800 0000 7218 0000  ..rR...r....r...
+00000c50: 0072 1800 0000 7219 0000 0072 3e00 0000  .r....r....r>...
+00000c60: 3b00 0000 732a 0000 000a 0204 0302 0102  ;...s*..........
+00000c70: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000c80: 0102 0102 0102 0102 0102 0102 0102 ef06  ................
+00000c90: 1318 0172 3e00 0000 4e29 0972 1400 0000  ...r>...N).r....
+00000ca0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
+00000cb0: 0000 da14 7079 6461 6e74 6963 2e64 6174  ....pydantic.dat
+00000cc0: 6163 6c61 7373 6573 7204 0000 0072 0500  aclassesr....r..
+00000cd0: 0000 721a 0000 0072 3e00 0000 7218 0000  ..r....r>...r...
+00000ce0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000cf0: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
+00000d00: 0000 0004 0710 020c 0302 0110 0d02 0110  ................
+00000d10: 1f02 01                                  ...
```

### Comparing `bluecast-0.2/bluecast/config/training_config.py` & `bluecast-0.3/bluecast/config/training_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 Pydantic dataclasses are used to define the configuration parameters. This allows for type checking and validation of
 the configuration parameters. The configuration parameters are used in the training pipeline and in the evaluation
 pipeline. Pydantic dataclasses are used to allow users a pythonic way to define the configuration parameters.
 Default configurations can be loaded, adjusted and passed into the blueprints.
 """
 from typing import Dict, Optional
 
+import xgboost as xgb
 from pydantic.dataclasses import dataclass
+from sklearn.feature_selection import RFECV
+from sklearn.metrics import make_scorer, matthews_corrcoef
+from sklearn.model_selection import StratifiedKFold
+
+
+class Config:
+    arbitrary_types_allowed = True
 
 
 @dataclass
 class TrainingConfig:
     """Define general training parameters."""
 
     global_random_state: int = 10
@@ -20,14 +28,30 @@
     hyperparameter_tuning_max_runtime_secs: int = 3600
     hypertuning_cv_folds: int = 1
     early_stopping_rounds: int = 10
     autotune_model: bool = True
     calculate_shap_values: bool = True
     train_size: float = 0.8
     train_split_stratify: bool = True
+    use_full_data_for_final_model: bool = True
+
+
+@dataclass(config=Config)
+class FeatureSelectionConfig:
+    """Define feature selection parameters."""
+
+    execute_selection: bool = True
+    selection_strategy: RFECV = RFECV(
+        estimator=xgb.XGBClassifier(),
+        step=1,
+        cv=StratifiedKFold(5, random_state=0, shuffle=True),
+        min_features_to_select=1,
+        scoring=make_scorer(matthews_corrcoef),
+        n_jobs=4,
+    )
 
 
 @dataclass
 class XgboostTuneParamsConfig:
     """Define hyperparameter tuning search space."""
 
     max_depth_min: int = 2
```

### Comparing `bluecast-0.2/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-0.3/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 1979 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 bb07 0000  o..........d....
+00000000: 550d 0d0a 0000 0000 f058 8164 bb07 0000  U........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
+00000020: 0005 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a05 6401 6404 6c06  ..d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
-00000070: 6d0e 5a0e 0100 6406 6505 6a0f 6407 6505  m.Z...d.e.j.d.e.
-00000080: 6a0f 6408 6503 6510 6502 6602 1900 6606  j.d.e.e.e.f...f.
-00000090: 6409 640a 8404 5a11 6403 5300 290b 7a51  d.d...Z.d.S.).zQ
-000000a0: 4d6f 6475 6c65 2066 6f72 2065 7661 6c75  Module for evalu
-000000b0: 6174 696f 6e20 6d65 7472 6963 732e 0a0a  ation metrics...
-000000c0: 5468 6973 2069 7320 6361 6c6c 6564 2061  This is called a
-000000d0: 7320 7061 7274 206f 6620 7468 6520 6669  s part of the fi
-000000e0: 745f 6576 616c 2066 756e 6374 696f 6e2e  t_eval function.
-000000f0: 0ae9 0000 0000 2902 da03 416e 79da 0444  ......)...Any..D
-00000100: 6963 744e 2906 da0e 6163 6375 7261 6379  ictN)...accuracy
-00000110: 5f73 636f 7265 da15 636c 6173 7369 6669  _score..classifi
-00000120: 6361 7469 6f6e 5f72 6570 6f72 74da 1063  cation_report..c
-00000130: 6f6e 6675 7369 6f6e 5f6d 6174 7269 78da  onfusion_matrix.
-00000140: 0866 315f 7363 6f72 65da 116d 6174 7468  .f1_score..matth
-00000150: 6577 735f 636f 7272 636f 6566 da0c 7265  ews_corrcoef..re
-00000160: 6361 6c6c 5f73 636f 7265 2901 da06 6c6f  call_score)...lo
-00000170: 6767 6572 da06 795f 7472 7565 da09 795f  gger..y_true..y_
-00000180: 636c 6173 7365 73da 0672 6574 7572 6e63  classes..returnc
-00000190: 0200 0000 0000 0000 0000 0000 0a00 0000  ................
-000001a0: 0a00 0000 4300 0000 7334 0100 007a 0774  ....C...s4...z.t
-000001b0: 007c 007c 0183 027d 0257 006e 0b04 0074  .|.|...}.W.n...t
-000001c0: 0179 1201 0001 0001 0064 017d 0259 006e  .y.......d.}.Y.n
-000001d0: 0177 0074 0264 027c 029b 009d 0283 0101  .w.t.d.|........
+00000070: 6d0e 5a0e 0100 6505 6a0f 6505 6a0f 6503  m.Z...e.j.e.j.e.
+00000080: 6510 6502 6602 1900 6406 9c03 6407 6408  e.e.f...d...d.d.
+00000090: 8404 5a11 6403 5300 2909 7a51 4d6f 6475  ..Z.d.S.).zQModu
+000000a0: 6c65 2066 6f72 2065 7661 6c75 6174 696f  le for evaluatio
+000000b0: 6e20 6d65 7472 6963 732e 0a0a 5468 6973  n metrics...This
+000000c0: 2069 7320 6361 6c6c 6564 2061 7320 7061   is called as pa
+000000d0: 7274 206f 6620 7468 6520 6669 745f 6576  rt of the fit_ev
+000000e0: 616c 2066 756e 6374 696f 6e2e 0ae9 0000  al function.....
+000000f0: 0000 2902 da03 416e 79da 0444 6963 744e  ..)...Any..DictN
+00000100: 2906 da0e 6163 6375 7261 6379 5f73 636f  )...accuracy_sco
+00000110: 7265 da15 636c 6173 7369 6669 6361 7469  re..classificati
+00000120: 6f6e 5f72 6570 6f72 74da 1063 6f6e 6675  on_report..confu
+00000130: 7369 6f6e 5f6d 6174 7269 78da 0866 315f  sion_matrix..f1_
+00000140: 7363 6f72 65da 116d 6174 7468 6577 735f  score..matthews_
+00000150: 636f 7272 636f 6566 da0c 7265 6361 6c6c  corrcoef..recall
+00000160: 5f73 636f 7265 2901 da06 6c6f 6767 6572  _score)...logger
+00000170: 2903 da06 795f 7472 7565 da09 795f 636c  )...y_true..y_cl
+00000180: 6173 7365 73da 0672 6574 7572 6e63 0200  asses..returnc..
+00000190: 0000 0000 0000 0000 0000 0a00 0000 0a00  ................
+000001a0: 0000 4300 0000 7336 0100 007a 0e74 007c  ..C...s6...z.t.|
+000001b0: 007c 0183 027d 0257 006e 1804 0074 016b  .|...}.W.n...t.k
+000001c0: 0a72 2601 0001 0001 0064 017d 0259 006e  .r&......d.}.Y.n
+000001d0: 0258 0074 0264 027c 029b 009d 0283 0101  .X.t.d.|........
 000001e0: 0074 0364 027c 029b 009d 0283 0101 0074  .t.d.|.........t
 000001f0: 0264 0383 0101 0074 047c 007c 0183 027d  .d.....t.|.|...}
 00000200: 0374 0264 047c 039b 009d 0283 0101 0074  .t.d.|.........t
 00000210: 057c 007c 0164 0564 068d 037d 0474 0264  .|.|.d.d...}.t.d
 00000220: 077c 049b 009d 0283 0101 0074 067c 007c  .|.........t.|.|
 00000230: 0164 0864 0164 098d 047d 0574 0264 0a7c  .d.d.d...}.t.d.|
 00000240: 059b 009d 0283 0101 0074 0364 0a7c 059b  .........t.d.|..
@@ -47,54 +47,54 @@
 000002e0: 0029 0f4e 7201 0000 007a 1b54 6865 204d  .).Nr....z.The M
 000002f0: 6174 7468 6577 2063 6f72 7265 6c61 7469  atthew correlati
 00000300: 6f6e 2069 7320 7a13 2d2d 2d2d 2d2d 2d2d  on is z.--------
 00000310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7a 1054 6865  -----------z.The
 00000320: 2061 6363 7572 6163 7920 6973 20da 0877   accuracy is ..w
 00000330: 6569 6768 7465 6429 01da 0761 7665 7261  eighted)...avera
 00000340: 6765 7a0e 5468 6520 7265 6361 6c6c 2069  gez.The recall i
-00000350: 7320 5a05 6d61 6372 6f29 0272 0f00 0000  s Z.macro).r....
-00000360: 5a0d 7a65 726f 5f64 6976 6973 696f 6e7a  Z.zero_divisionz
+00000350: 7320 da05 6d61 6372 6f29 0272 0f00 0000  s ..macro).r....
+00000360: da0d 7a65 726f 5f64 6976 6973 696f 6e7a  ..zero_divisionz
 00000370: 1654 6865 206d 6163 726f 2046 3120 7363  .The macro F1 sc
 00000380: 6f72 6520 6973 20da 056d 6963 726f 7a16  ore is ..microz.
 00000390: 5468 6520 6d69 6372 6f20 4631 2073 636f  The micro F1 sco
 000003a0: 7265 2069 7320 7a19 5468 6520 7765 6967  re is z.The weig
 000003b0: 6874 6564 2046 3120 7363 6f72 6520 6973  hted F1 score is
 000003c0: 2029 08da 086d 6174 7468 6577 73da 0861   )...matthews..a
 000003d0: 6363 7572 6163 79da 0672 6563 616c 6cda  ccuracy..recall.
 000003e0: 0e66 315f 7363 6f72 655f 6d61 6372 6fda  .f1_score_macro.
 000003f0: 0e66 315f 7363 6f72 655f 6d69 6372 6fda  .f1_score_micro.
 00000400: 1166 315f 7363 6f72 655f 7765 6967 6874  .f1_score_weight
-00000410: 6564 5a14 636c 6173 7366 6963 6174 696f  edZ.classficatio
+00000410: 6564 da14 636c 6173 7366 6963 6174 696f  ed..classficatio
 00000420: 6e5f 7265 706f 7274 7206 0000 0029 0972  n_reportr....).r
 00000430: 0800 0000 da09 4578 6365 7074 696f 6eda  ......Exception.
 00000440: 0570 7269 6e74 720a 0000 0072 0400 0000  .printr....r....
 00000450: 7209 0000 0072 0700 0000 7205 0000 0072  r....r....r....r
 00000460: 0600 0000 290a 720b 0000 0072 0c00 0000  ....).r....r....
-00000470: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00000480: 1400 0000 7215 0000 0072 1600 0000 5a1a  ....r....r....Z.
+00000470: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000480: 1600 0000 7217 0000 0072 1800 0000 da1a  ....r....r......
 00000490: 6675 6c6c 5f63 6c61 7373 6966 6963 6174  full_classificat
-000004a0: 696f 6e5f 7265 706f 7274 5a11 6576 616c  ion_reportZ.eval
+000004a0: 696f 6e5f 7265 706f 7274 da11 6576 616c  ion_report..eval
 000004b0: 7561 7469 6f6e 5f73 636f 7265 73a9 0072  uation_scores..r
-000004c0: 1900 0000 fa4f 2f55 7365 7273 2f74 686f  .....O/Users/tho
-000004d0: 6d61 736d 6569 7373 6e65 722f 4964 6561  masmeissner/Idea
-000004e0: 5072 6f6a 6563 7473 2f42 6c75 6543 6173  Projects/BlueCas
-000004f0: 742f 626c 7565 6361 7374 2f65 7661 6c75  t/bluecast/evalu
-00000500: 6174 696f 6e2f 6576 616c 5f6d 6574 7269  ation/eval_metri
-00000510: 6373 2e70 79da 0f65 7661 6c5f 636c 6173  cs.py..eval_clas
-00000520: 7369 6669 6572 1400 0000 7342 0000 0002  sifier....sB....
-00000530: 010e 010c 0108 0102 ff0e 030e 0108 010a  ................
-00000540: 010e 010e 010e 0110 010e 010e 0110 010e  ................
-00000550: 010e 0110 010e 010e 010a 0208 0102 0302  ................
-00000560: 0102 0102 0102 0102 0102 0108 0106 f804  ................
-00000570: 0a72 1b00 0000 2912 da07 5f5f 646f 635f  .r....)...__doc_
-00000580: 5fda 0674 7970 696e 6772 0200 0000 7203  _..typingr....r.
-00000590: 0000 00da 056e 756d 7079 da02 6e70 5a0f  .....numpy..npZ.
-000005a0: 736b 6c65 6172 6e2e 6d65 7472 6963 7372  sklearn.metricsr
-000005b0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-000005c0: 0000 0072 0800 0000 7209 0000 00da 2462  ...r....r.....$b
-000005d0: 6c75 6563 6173 742e 6765 6e65 7261 6c5f  luecast.general_
-000005e0: 7574 696c 732e 6765 6e65 7261 6c5f 7574  utils.general_ut
-000005f0: 696c 7372 0a00 0000 da07 6e64 6172 7261  ilsr......ndarra
-00000600: 79da 0373 7472 721b 0000 0072 1900 0000  y..strr....r....
-00000610: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000620: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00000630: 0000 0400 1004 0802 2001 0c09 2603       ........ ...&.
+000004c0: 1e00 0000 fa46 2f68 6f6d 652f 7468 6f6d  .....F/home/thom
+000004d0: 6173 2f49 6465 6150 726f 6a65 6374 732f  as/IdeaProjects/
+000004e0: 426c 7565 4361 7374 2f62 6c75 6563 6173  BlueCast/bluecas
+000004f0: 742f 6576 616c 7561 7469 6f6e 2f65 7661  t/evaluation/eva
+00000500: 6c5f 6d65 7472 6963 732e 7079 da0f 6576  l_metrics.py..ev
+00000510: 616c 5f63 6c61 7373 6966 6965 7214 0000  al_classifier...
+00000520: 0073 4000 0000 0001 0201 0e01 0e01 0a02  .s@.............
+00000530: 0e01 0e01 0801 0a01 0e01 0e01 0e01 1001  ................
+00000540: 0e01 0e01 1001 0e01 0e01 1001 0e01 0e02  ................
+00000550: 0a01 0803 0201 0201 0201 0201 0201 0201  ................
+00000560: 0201 08f8 060a 7220 0000 0029 12da 075f  ......r ...)..._
+00000570: 5f64 6f63 5f5f da06 7479 7069 6e67 7202  _doc__..typingr.
+00000580: 0000 0072 0300 0000 da05 6e75 6d70 79da  ...r......numpy.
+00000590: 026e 70da 0f73 6b6c 6561 726e 2e6d 6574  .np..sklearn.met
+000005a0: 7269 6373 7204 0000 0072 0500 0000 7206  ricsr....r....r.
+000005b0: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
+000005c0: 0000 da24 626c 7565 6361 7374 2e67 656e  ...$bluecast.gen
+000005d0: 6572 616c 5f75 7469 6c73 2e67 656e 6572  eral_utils.gener
+000005e0: 616c 5f75 7469 6c73 720a 0000 00da 076e  al_utilsr......n
+000005f0: 6461 7272 6179 da03 7374 7272 2000 0000  darray..strr ...
+00000600: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+00000610: 1f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000620: 0000 730a 0000 0004 0410 0208 0120 090c  ..s.......... ..
+00000630: 03                                       .
```

### Comparing `bluecast-0.2/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-0.3/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 1486 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,83 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 ce05 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 6d1d 8364 6d05 0000  o.......m..dm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
-00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6402 6c04 5a05 6401 6402 6c06 5a07 6401  d.l.Z.d.d.l.Z.d.
-00000050: 6402 6c08 5a08 6409 6404 6507 6a09 6405  d.l.Z.d.d.e.j.d.
-00000060: 650a 6406 6505 6a0b 6606 6407 6408 8405  e.d.e.j.f.d.d...
-00000070: 5a0c 6402 5300 290a 7ab2 4d6f 6475 6c65  Z.d.S.).z.Module
-00000080: 2074 6f20 6361 6c63 756c 6174 6520 5348   to calculate SH
-00000090: 4150 2076 616c 7565 7320 666f 7220 6120  AP values for a 
-000000a0: 7472 6169 6e65 6420 4d4c 206d 6f64 656c  trained ML model
-000000b0: 2e0a 0a54 6865 2069 6d70 6c65 6d65 6e74  ...The implement
-000000c0: 6174 696f 6e20 6973 2066 6c65 7869 626c  ation is flexibl
-000000d0: 6520 616e 6420 6361 6e20 6265 2075 7365  e and can be use
-000000e0: 6420 666f 7220 616c 6d6f 7374 2061 6e79  d for almost any
-000000f0: 204d 4c20 6d6f 6465 6c2e 2054 6865 2069   ML model. The i
-00000100: 6d70 6c65 6d65 6e74 6174 696f 6e20 6973  mplementation is
-00000110: 2062 6173 6564 206f 6e20 7468 6520 5348   based on the SH
-00000120: 4150 206c 6962 7261 7279 2e0a e900 0000  AP library......
-00000130: 004e da04 7472 6565 da02 6466 da09 6578  .N..tree..df..ex
-00000140: 706c 6169 6e65 72da 0672 6574 7572 6e63  plainer..returnc
-00000150: 0300 0000 0000 0000 0000 0000 0600 0000  ................
-00000160: 0800 0000 4300 0000 73be 0000 0074 00a0  ....C...s....t..
-00000170: 01a1 0001 007c 0264 016b 0272 457a 1a74  .....|.d.k.rEz.t
-00000180: 00a0 027c 00a1 017d 037c 03a0 037c 01a1  ...|...}.|...|..
-00000190: 017d 0474 006a 047c 047c 0164 0264 0364  .}.t.j.|.|.d.d.d
-000001a0: 048d 0401 0074 05a0 06a1 0001 0057 0064  .....t.......W.d
-000001b0: 0653 0004 0074 0779 4401 0001 0001 0074  .S...t.yD......t
-000001c0: 00a0 087c 006a 097c 01a1 027d 057c 05a0  ...|.j.|...}.|..
-000001d0: 037c 01a1 017d 0474 006a 047c 047c 0164  .|...}.t.j.|.|.d
-000001e0: 0364 058d 0301 0074 05a0 06a1 0001 0059  .d.....t.......Y
-000001f0: 0064 0653 0077 0074 00a0 087c 006a 097c  .d.S.w.t...|.j.|
-00000200: 01a1 027d 057c 05a0 037c 01a1 017d 0474  ...}.|...|...}.t
-00000210: 006a 047c 047c 0164 0364 058d 0301 0074  .j.|.|.d.d.....t
-00000220: 05a0 06a1 0001 007c 0453 0029 0761 3d01  .......|.S.).a=.
-00000230: 0000 0a20 2020 2053 6565 2065 7870 6c61  ...    See expla
-00000240: 6e61 7469 6f6e 7320 756e 6465 723a 0a20  nations under:. 
-00000250: 2020 2068 7474 7073 3a2f 2f6d 6564 6975     https://mediu
-00000260: 6d2e 636f 6d2f 7261 7069 6473 2d61 692f  m.com/rapids-ai/
-00000270: 6770 752d 6163 6365 6c65 7261 7465 642d  gpu-accelerated-
-00000280: 7368 6170 2d76 616c 7565 732d 7769 7468  shap-values-with
-00000290: 2d78 6762 6f6f 7374 2d31 2d33 2d61 6e64  -xgboost-1-3-and
-000002a0: 2d72 6170 6964 732d 3538 3766 6164 3638  -rapids-587fad68
-000002b0: 3232 0a20 2020 203a 7061 7261 6d20 6d6f  22.    :param mo
-000002c0: 6465 6c3a 2054 7261 696e 6564 204d 4c20  del: Trained ML 
-000002d0: 6d6f 6465 6c0a 2020 2020 3a70 6172 616d  model.    :param
-000002e0: 2064 663a 2054 6573 7420 6461 7461 2074   df: Test data t
-000002f0: 6f20 7072 6564 6963 7420 6f6e 2e0a 2020  o predict on..  
-00000300: 2020 3a70 6172 616d 2065 7870 6c61 696e    :param explain
-00000310: 6572 3a20 5365 7420 2274 7265 6522 2066  er: Set "tree" f
-00000320: 6f72 2054 7265 6545 7870 6c61 696e 6572  or TreeExplainer
-00000330: 2e20 4f74 6865 7277 6973 6520 7573 6573  . Otherwise uses
-00000340: 204b 6572 6e65 6c45 7870 6c61 696e 6572   KernelExplainer
-00000350: 2e0a 2020 2020 3a72 6574 7572 6e3a 2053  ..    :return: S
-00000360: 6861 7020 7661 6c75 6573 0a20 2020 2072  hap values.    r
-00000370: 0200 0000 da03 6261 7254 2902 da09 706c  ......barT)...pl
-00000380: 6f74 5f74 7970 65da 0473 686f 7729 0172  ot_type..show).r
-00000390: 0800 0000 4e29 0ada 0473 6861 705a 0669  ....N)...shapZ.i
-000003a0: 6e69 746a 735a 0d54 7265 6545 7870 6c61  nitjsZ.TreeExpla
-000003b0: 696e 6572 da0b 7368 6170 5f76 616c 7565  iner..shap_value
-000003c0: 735a 0c73 756d 6d61 7279 5f70 6c6f 74da  sZ.summary_plot.
-000003d0: 0370 6c74 7208 0000 00da 0e41 7373 6572  .pltr......Asser
-000003e0: 7469 6f6e 4572 726f 725a 0f4b 6572 6e65  tionErrorZ.Kerne
-000003f0: 6c45 7870 6c61 696e 6572 da07 7072 6564  lExplainer..pred
-00000400: 6963 7429 06da 056d 6f64 656c 7203 0000  ict)...modelr...
-00000410: 0072 0400 0000 5a0e 7472 6565 5f65 7870  .r....Z.tree_exp
-00000420: 6c61 696e 6572 5a11 6d6f 6465 6c5f 7368  lainerZ.model_sh
-00000430: 6170 5f76 616c 7565 735a 146d 6f64 656c  ap_valuesZ.model
-00000440: 5f73 6861 705f 6578 706c 6169 6e65 72a9  _shap_explainer.
-00000450: 0072 0f00 0000 fa4e 2f55 7365 7273 2f74  .r.....N/Users/t
-00000460: 686f 6d61 736d 6569 7373 6e65 722f 4964  homasmeissner/Id
-00000470: 6561 5072 6f6a 6563 7473 2f42 6c75 6543  eaProjects/BlueC
-00000480: 6173 742f 626c 7565 6361 7374 2f65 7661  ast/bluecast/eva
-00000490: 6c75 6174 696f 6e2f 7368 6170 5f76 616c  luation/shap_val
-000004a0: 7565 732e 7079 da11 7368 6170 5f65 7870  ues.py..shap_exp
-000004b0: 6c61 6e61 7469 6f6e 730b 0000 0073 2400  lanations....s$.
-000004c0: 0000 0809 0801 0201 0a01 0a01 1201 0e01  ................
-000004d0: 0c01 0e01 0a01 1001 0e01 02fc 0e06 0a01  ................
-000004e0: 1001 0801 0401 7211 0000 0029 0172 0200  ......r....).r..
-000004f0: 0000 290d da07 5f5f 646f 635f 5fda 116d  ..)...__doc__..m
-00000500: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
-00000510: da06 7079 706c 6f74 720b 0000 00da 056e  ..pyplotr......n
-00000520: 756d 7079 da02 6e70 da06 7061 6e64 6173  umpy..np..pandas
-00000530: da02 7064 7209 0000 00da 0944 6174 6146  ..pdr......DataF
-00000540: 7261 6d65 da03 7374 72da 076e 6461 7272  rame..str..ndarr
-00000550: 6179 7211 0000 0072 0f00 0000 720f 0000  ayr....r....r...
-00000560: 0072 0f00 0000 7210 0000 00da 083c 6d6f  .r....r......<mo
-00000570: 6475 6c65 3e01 0000 0073 0c00 0000 0400  dule>....s......
-00000580: 0c04 0801 0801 0801 2003                 ........ .
+00000020: 0007 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
+00000040: 5a04 6401 6402 6c05 5a05 6409 6404 6504  Z.d.d.l.Z.d.d.e.
+00000050: 6a06 6405 6507 6406 6502 6a08 6606 6407  j.d.e.d.e.j.f.d.
+00000060: 6408 8405 5a09 6402 5300 290a 7ab2 4d6f  d...Z.d.S.).z.Mo
+00000070: 6475 6c65 2074 6f20 6361 6c63 756c 6174  dule to calculat
+00000080: 6520 5348 4150 2076 616c 7565 7320 666f  e SHAP values fo
+00000090: 7220 6120 7472 6169 6e65 6420 4d4c 206d  r a trained ML m
+000000a0: 6f64 656c 2e0a 0a54 6865 2069 6d70 6c65  odel...The imple
+000000b0: 6d65 6e74 6174 696f 6e20 6973 2066 6c65  mentation is fle
+000000c0: 7869 626c 6520 616e 6420 6361 6e20 6265  xible and can be
+000000d0: 2075 7365 6420 666f 7220 616c 6d6f 7374   used for almost
+000000e0: 2061 6e79 204d 4c20 6d6f 6465 6c2e 2054   any ML model. T
+000000f0: 6865 2069 6d70 6c65 6d65 6e74 6174 696f  he implementatio
+00000100: 6e20 6973 2062 6173 6564 206f 6e20 7468  n is based on th
+00000110: 6520 5348 4150 206c 6962 7261 7279 2e0a  e SHAP library..
+00000120: e900 0000 004e da04 7472 6565 da02 6466  .....N..tree..df
+00000130: da09 6578 706c 6169 6e65 72da 0672 6574  ..explainer..ret
+00000140: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
+00000150: 0600 0000 0800 0000 4300 0000 73a6 0000  ........C...s...
+00000160: 0074 00a0 01a1 0001 007c 0264 016b 0272  .t.......|.d.k.r
+00000170: 3d7a 1674 00a0 027c 00a1 017d 037c 03a0  =z.t...|...}.|..
+00000180: 037c 01a1 017d 0474 006a 047c 047c 0164  .|...}.t.j.|.|.d
+00000190: 0264 0364 048d 0401 0057 0064 0653 0004  .d.d.....W.d.S..
+000001a0: 0074 0579 3c01 0001 0001 0074 00a0 067c  .t.y<......t...|
+000001b0: 006a 077c 01a1 027d 057c 05a0 037c 01a1  .j.|...}.|...|..
+000001c0: 017d 0474 006a 047c 047c 0164 0364 058d  .}.t.j.|.|.d.d..
+000001d0: 0301 0059 0064 0653 0077 0074 00a0 067c  ...Y.d.S.w.t...|
+000001e0: 006a 077c 01a1 027d 057c 05a0 037c 01a1  .j.|...}.|...|..
+000001f0: 017d 0474 006a 047c 047c 0164 0364 058d  .}.t.j.|.|.d.d..
+00000200: 0301 007c 0453 0029 0761 3d01 0000 0a20  ...|.S.).a=.... 
+00000210: 2020 2053 6565 2065 7870 6c61 6e61 7469     See explanati
+00000220: 6f6e 7320 756e 6465 723a 0a20 2020 2068  ons under:.    h
+00000230: 7474 7073 3a2f 2f6d 6564 6975 6d2e 636f  ttps://medium.co
+00000240: 6d2f 7261 7069 6473 2d61 692f 6770 752d  m/rapids-ai/gpu-
+00000250: 6163 6365 6c65 7261 7465 642d 7368 6170  accelerated-shap
+00000260: 2d76 616c 7565 732d 7769 7468 2d78 6762  -values-with-xgb
+00000270: 6f6f 7374 2d31 2d33 2d61 6e64 2d72 6170  oost-1-3-and-rap
+00000280: 6964 732d 3538 3766 6164 3638 3232 0a20  ids-587fad6822. 
+00000290: 2020 203a 7061 7261 6d20 6d6f 6465 6c3a     :param model:
+000002a0: 2054 7261 696e 6564 204d 4c20 6d6f 6465   Trained ML mode
+000002b0: 6c0a 2020 2020 3a70 6172 616d 2064 663a  l.    :param df:
+000002c0: 2054 6573 7420 6461 7461 2074 6f20 7072   Test data to pr
+000002d0: 6564 6963 7420 6f6e 2e0a 2020 2020 3a70  edict on..    :p
+000002e0: 6172 616d 2065 7870 6c61 696e 6572 3a20  aram explainer: 
+000002f0: 5365 7420 2274 7265 6522 2066 6f72 2054  Set "tree" for T
+00000300: 7265 6545 7870 6c61 696e 6572 2e20 4f74  reeExplainer. Ot
+00000310: 6865 7277 6973 6520 7573 6573 204b 6572  herwise uses Ker
+00000320: 6e65 6c45 7870 6c61 696e 6572 2e0a 2020  nelExplainer..  
+00000330: 2020 3a72 6574 7572 6e3a 2053 6861 7020    :return: Shap 
+00000340: 7661 6c75 6573 0a20 2020 2072 0200 0000  values.    r....
+00000350: da03 6261 7254 2902 da09 706c 6f74 5f74  ..barT)...plot_t
+00000360: 7970 65da 0473 686f 7729 0172 0800 0000  ype..show).r....
+00000370: 4e29 08da 0473 6861 705a 0669 6e69 746a  N)...shapZ.initj
+00000380: 735a 0d54 7265 6545 7870 6c61 696e 6572  sZ.TreeExplainer
+00000390: da0b 7368 6170 5f76 616c 7565 735a 0c73  ..shap_valuesZ.s
+000003a0: 756d 6d61 7279 5f70 6c6f 74da 0e41 7373  ummary_plot..Ass
+000003b0: 6572 7469 6f6e 4572 726f 725a 0f4b 6572  ertionErrorZ.Ker
+000003c0: 6e65 6c45 7870 6c61 696e 6572 da07 7072  nelExplainer..pr
+000003d0: 6564 6963 7429 06da 056d 6f64 656c 7203  edict)...modelr.
+000003e0: 0000 0072 0400 0000 5a0e 7472 6565 5f65  ...r....Z.tree_e
+000003f0: 7870 6c61 696e 6572 5a11 6d6f 6465 6c5f  xplainerZ.model_
+00000400: 7368 6170 5f76 616c 7565 735a 146d 6f64  shap_valuesZ.mod
+00000410: 656c 5f73 6861 705f 6578 706c 6169 6e65  el_shap_explaine
+00000420: 72a9 0072 0e00 0000 fa45 2f68 6f6d 652f  r..r.....E/home/
+00000430: 7468 6f6d 6173 2f49 6465 6150 726f 6a65  thomas/IdeaProje
+00000440: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
+00000450: 6563 6173 742f 6576 616c 7561 7469 6f6e  ecast/evaluation
+00000460: 2f73 6861 705f 7661 6c75 6573 2e70 79da  /shap_values.py.
+00000470: 1173 6861 705f 6578 706c 616e 6174 696f  .shap_explanatio
+00000480: 6e73 0a00 0000 731e 0000 0008 0908 0102  ns....s.........
+00000490: 010a 010a 0118 010c 010e 010a 0116 0102  ................
+000004a0: fd0e 050a 0110 0104 0172 1000 0000 2901  .........r....).
+000004b0: 7202 0000 0029 0ada 075f 5f64 6f63 5f5f  r....)...__doc__
+000004c0: da05 6e75 6d70 79da 026e 70da 0670 616e  ..numpy..np..pan
+000004d0: 6461 73da 0270 6472 0900 0000 da09 4461  das..pdr......Da
+000004e0: 7461 4672 616d 65da 0373 7472 da07 6e64  taFrame..str..nd
+000004f0: 6172 7261 7972 1000 0000 720e 0000 0072  arrayr....r....r
+00000500: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
+00000510: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+00000520: 0004 0008 0408 0108 0120 03              ......... .
```

### Comparing `bluecast-0.2/bluecast/evaluation/eval_metrics.py` & `bluecast-0.3/bluecast/evaluation/eval_metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,25 @@
     matthews_corrcoef,
     recall_score,
 )
 
 from bluecast.general_utils.general_utils import logger
 
 
+def balanced_log_loss(y_true, y_pred):
+    assert ((y_true == 0) | (y_true == 1)).all()
+    assert len(y_true) == len(y_pred)
+    assert y_pred.ndim == 1
+    eps = 1e-15
+    y_pred = y_pred.clip(eps, 1 - eps)
+    l0 = -np.log(1 - y_pred[y_true == 0])
+    l1 = -np.log(y_pred[y_true != 0])
+    return (l0.mean() + l1.mean()) / 2
+
+
 def eval_classifier(y_true: np.ndarray, y_classes: np.ndarray) -> Dict[str, Any]:
     try:
         matthews = matthews_corrcoef(y_true, y_classes)
     except Exception:
         matthews = 0
 
     print(f"The Matthew correlation is {matthews}")
@@ -35,22 +46,26 @@
     logger(f"The macro F1 score is {f1_score_macro}")
     f1_score_micro = f1_score(y_true, y_classes, average="micro", zero_division=0)
     print(f"The micro F1 score is {f1_score_micro}")
     logger(f"The micro F1 score is {f1_score_micro}")
     f1_score_weighted = f1_score(y_true, y_classes, average="weighted", zero_division=0)
     print(f"The weighted F1 score is {f1_score_weighted}")
     logger(f"The weighted F1 score is {f1_score_weighted}")
+    bll = balanced_log_loss(y_true, y_classes)
+    print(f"The balanced logloss is {bll}")
+    logger(f"The balanced logloss is {bll}")
 
     full_classification_report = classification_report(y_true, y_classes)
     print(full_classification_report)
 
     evaluation_scores = {
         "matthews": matthews,
         "accuracy": accuracy,
         "recall": recall,
         "f1_score_macro": f1_score_macro,
         "f1_score_micro": f1_score_micro,
         "f1_score_weighted": f1_score_weighted,
+        "balanced_logloss": bll,
         "classfication_report": full_classification_report,
         "confusion_matrix": confusion_matrix(y_true, y_classes),
     }
     return evaluation_scores
```

### Comparing `bluecast-0.2/bluecast/evaluation/shap_values.py` & `bluecast-0.3/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.3/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 2248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 c808 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 f058 8164 c808 0000  o........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6402 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 6401 6402 6c07 5a08 6401 6402 6c09  Z.d.d.l.Z.d.d.l.
 00000060: 5a0a 6404 650b 6602 6405 6406 8404 5a0c  Z.d.e.f.d.d...Z.
 00000070: 6407 650b 6404 6402 6604 6408 6409 8404  d.e.d.d.f.d.d...
@@ -32,122 +32,121 @@
 000001f0: 7420 7573 6573 2043 5055 2eda 0565 7861  t uses CPU...exa
 00000200: 6374 2909 da02 6e70 da06 7261 6e64 6f6d  ct)...np..random
 00000210: da04 7261 6e64 da07 7261 6e64 696e 74da  ..rand..randint.
 00000220: 0378 6762 5a07 444d 6174 7269 785a 0574  .xgbZ.DMatrixZ.t
 00000230: 7261 696e da05 7072 696e 74da 0945 7863  rain..print..Exc
 00000240: 6570 7469 6f6e 2904 da04 6461 7461 7208  eption)...datar.
 00000250: 0000 005a 0764 5f74 7261 696e da06 7061  ...Z.d_train..pa
-00000260: 7261 6d73 a900 7215 0000 00fa 532f 5573  rams..r.....S/Us
-00000270: 6572 732f 7468 6f6d 6173 6d65 6973 736e  ers/thomasmeissn
-00000280: 6572 2f49 6465 6150 726f 6a65 6374 732f  er/IdeaProjects/
-00000290: 426c 7565 4361 7374 2f62 6c75 6563 6173  BlueCast/bluecas
-000002a0: 742f 6765 6e65 7261 6c5f 7574 696c 732f  t/general_utils/
-000002b0: 6765 6e65 7261 6c5f 7574 696c 732e 7079  general_utils.py
-000002c0: da11 6368 6563 6b5f 6770 755f 7375 7070  ..check_gpu_supp
-000002d0: 6f72 740a 0000 0073 1800 0000 0e01 1001  ort....s........
-000002e0: 0e01 0a01 0201 0c01 0801 0601 0c01 0801  ................
-000002f0: 0601 02fe 7217 0000 00da 076d 6573 7361  ....r......messa
-00000300: 6765 6301 0000 0000 0000 0000 0000 0001  gec.............
-00000310: 0000 0003 0000 0043 0000 0073 1600 0000  .......C...s....
-00000320: 7400 a001 7c00 a101 0100 7402 7c00 8301  t...|.....t.|...
-00000330: 0100 6400 5300 2901 4e29 03da 076c 6f67  ..d.S.).N)...log
-00000340: 6769 6e67 da04 696e 666f 7211 0000 0029  ging..infor....)
-00000350: 0172 1800 0000 7215 0000 0072 1500 0000  .r....r....r....
-00000360: 7216 0000 00da 066c 6f67 6765 7218 0000  r......logger...
-00000370: 0073 0400 0000 0a01 0c01 721b 0000 00da  .s........r.....
-00000380: 0f61 7574 6f6d 6c5f 696e 7374 616e 6365  .automl_instance
-00000390: fa04 2e64 6174 da0e 636c 6173 735f 696e  ...dat..class_in
-000003a0: 7374 616e 6365 da09 6669 6c65 5f70 6174  stance..file_pat
-000003b0: 68da 0966 696c 655f 6e61 6d65 da09 6669  h..file_name..fi
-000003c0: 6c65 5f74 7970 6563 0400 0000 0000 0000  le_typec........
-000003d0: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
-000003e0: 733c 0000 007c 0172 097c 017c 0217 007c  s<...|.r.|.|...|
-000003f0: 0317 007d 046e 047c 027c 0317 007d 0474  ...}.n.|.|...}.t
-00000400: 007c 0464 0183 027d 0574 01a0 027c 007c  .|.d...}.t...|.|
-00000410: 05a1 0201 007c 05a0 03a1 0001 0064 0253  .....|.......d.S
-00000420: 0029 0361 5301 0000 0a20 2020 2054 616b  .).aS....    Tak
-00000430: 6573 2061 2070 7265 7472 6169 6e65 6420  es a pretrained 
-00000440: 6d6f 6465 6c20 616e 6420 7361 7665 7320  model and saves 
-00000450: 6974 2076 6961 2064 696c 6c2e 0a20 2020  it via dill..   
-00000460: 203a 7061 7261 6d20 636c 6173 735f 696e   :param class_in
-00000470: 7374 616e 6365 3a20 5461 6b65 7320 696e  stance: Takes in
-00000480: 7374 616e 6365 206f 6620 6120 426c 7565  stance of a Blue
-00000490: 4361 7374 2063 6c61 7373 2e0a 2020 2020  Cast class..    
-000004a0: 3a70 6172 616d 2066 696c 655f 7061 7468  :param file_path
-000004b0: 3a20 5461 6b65 7320 6120 7374 7269 6e67  : Takes a string
-000004c0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-000004d0: 6675 6c6c 2061 6273 6f6c 7574 6520 7061  full absolute pa
-000004e0: 7468 2e0a 2020 2020 3a70 6172 616d 2066  th..    :param f
-000004f0: 696c 655f 6e61 6d65 3a20 5461 6b65 7320  ile_name: Takes 
-00000500: 6120 7374 7269 6e67 2063 6f6e 7461 696e  a string contain
-00000510: 696e 6720 7468 6520 7768 6f6c 6520 6669  ing the whole fi
-00000520: 6c65 206e 616d 652e 0a20 2020 203a 7061  le name..    :pa
-00000530: 7261 6d20 6669 6c65 5f74 7970 653a 2054  ram file_type: T
-00000540: 616b 6573 2074 6865 2065 7870 6563 7465  akes the expecte
-00000550: 6420 7479 7065 206f 6620 6669 6c65 2074  d type of file t
-00000560: 6f20 6578 706f 7274 2e0a 2020 2020 3a72  o export..    :r
-00000570: 6574 7572 6e3a 0a20 2020 20da 0277 624e  eturn:.    ..wbN
-00000580: 2904 da04 6f70 656e da06 7069 636b 6c65  )...open..pickle
-00000590: da04 6475 6d70 da05 636c 6f73 6529 0672  ..dump..close).r
-000005a0: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
-000005b0: 0000 00da 0966 756c 6c5f 7061 7468 da0b  .....full_path..
-000005c0: 6669 6c65 6861 6e64 6c65 7272 1500 0000  filehandlerr....
-000005d0: 7215 0000 0072 1600 0000 da12 7361 7665  r....r......save
-000005e0: 5f74 6f5f 7072 6f64 7563 7469 6f6e 1d00  _to_production..
-000005f0: 0000 730c 0000 0004 0e0e 0108 020a 010c  ..s.............
-00000600: 010c 0172 2900 0000 6303 0000 0000 0000  ...r)...c.......
-00000610: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
-00000620: 0073 5800 0000 7c00 7207 7c00 7c01 1700  .sX...|.r.|.|...
-00000630: 7d03 6e02 7c01 7d03 7a07 7400 7c03 6401  }.n.|.}.z.t.|.d.
-00000640: 8302 7d04 5700 6e10 0400 7401 7920 0100  ..}.W.n...t.y ..
-00000650: 0100 0100 7400 7c03 7c02 1700 6401 8302  ....t.|.|...d...
-00000660: 7d04 5900 6e01 7700 7402 a003 7c04 a101  }.Y.n.w.t...|...
-00000670: 7d05 7c04 a004 a100 0100 7c05 5300 2902  }.|.......|.S.).
-00000680: 619a 0100 000a 2020 2020 4c6f 6164 2069  a.....    Load i
-00000690: 6e20 6120 7072 6574 7261 696e 6564 2061  n a pretrained a
-000006a0: 7574 6f20 6d6c 206d 6f64 656c 2e20 5468  uto ml model. Th
-000006b0: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
-000006c0: 2074 7279 2074 6f20 6c6f 6164 2074 6865   try to load the
-000006d0: 206d 6f64 656c 2061 7320 7072 6f76 6964   model as provid
-000006e0: 6564 2e0a 2020 2020 4974 2068 6173 2061  ed..    It has a
-000006f0: 2066 616c 6c62 6163 6b20 6c6f 6769 6320   fallback logic 
-00000700: 746f 2069 6d70 7574 6520 2e64 6174 2061  to impute .dat a
-00000710: 7320 6669 6c65 5f74 7970 6520 696e 2063  s file_type in c
-00000720: 6173 6520 7468 6520 696d 706f 7274 2066  ase the import f
-00000730: 6169 6c73 2069 6e69 7469 616c 6c79 2e0a  ails initially..
-00000740: 2020 2020 3a70 6172 616d 2066 696c 655f      :param file_
-00000750: 7061 7468 3a20 5461 6b65 7320 6120 7374  path: Takes a st
-00000760: 7269 6e67 2063 6f6e 7461 696e 696e 6720  ring containing 
-00000770: 7468 6520 6675 6c6c 2061 6273 6f6c 7574  the full absolut
-00000780: 6520 7061 7468 2e0a 2020 2020 3a70 6172  e path..    :par
-00000790: 616d 2066 696c 655f 6e61 6d65 3a20 5461  am file_name: Ta
-000007a0: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
-000007b0: 7461 696e 696e 6720 7468 6520 7768 6f6c  taining the whol
-000007c0: 6520 6669 6c65 206e 616d 652e 0a20 2020  e file name..   
-000007d0: 203a 7061 7261 6d20 6669 6c65 5f74 7970   :param file_typ
-000007e0: 653a 2054 616b 6573 2074 6865 2065 7870  e: Takes the exp
-000007f0: 6563 7465 6420 7479 7065 206f 6620 6669  ected type of fi
-00000800: 6c65 2074 6f20 696d 706f 7274 2e0a 2020  le to import..  
-00000810: 2020 3a72 6574 7572 6e3a 0a20 2020 20da    :return:.    .
-00000820: 0272 6229 0572 2300 0000 7212 0000 0072  .rb).r#...r....r
-00000830: 2400 0000 da04 6c6f 6164 7226 0000 0029  $.....loadr&...)
-00000840: 0672 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00000850: 7227 0000 0072 2800 0000 5a0c 6175 746f  r'...r(...Z.auto
-00000860: 6d6c 5f6d 6f64 656c 7215 0000 0072 1500  ml_modelr....r..
-00000870: 0000 7216 0000 00da 136c 6f61 645f 666f  ..r......load_fo
-00000880: 725f 7072 6f64 7563 7469 6f6e 3400 0000  r_production4...
-00000890: 7316 0000 0004 0d0a 0104 0202 010e 010c  s...............
-000008a0: 0112 0102 ff0a 0208 0104 0172 2c00 0000  ...........r,...
-000008b0: 2903 4e72 1c00 0000 721d 0000 0029 10da  ).Nr....r....)..
-000008c0: 075f 5f64 6f63 5f5f 7219 0000 00da 0674  .__doc__r......t
-000008d0: 7970 696e 6772 0200 0000 7203 0000 005a  ypingr....r....Z
-000008e0: 0464 696c 6c72 2400 0000 da05 6e75 6d70  .dillr$.....nump
-000008f0: 7972 0c00 0000 5a07 7867 626f 6f73 7472  yr....Z.xgboostr
-00000900: 1000 0000 da03 7374 7272 1700 0000 721b  ......strr....r.
-00000910: 0000 0072 2900 0000 722c 0000 0072 1500  ...r)...r,...r..
-00000920: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000930: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000940: 4400 0000 0400 0801 1001 0802 0801 0801  D...............
-00000950: 0e03 120e 0207 0201 0201 04fc 0201 02ff  ................
-00000960: 0602 02fe 0203 02fd 0204 02fc 0205 0afb  ................
-00000970: 0218 0201 0201 04fd 0601 02ff 0202 02fe  ................
-00000980: 0203 02fd 0204 0efc                      ........
+00000260: 7261 6d73 a900 7215 0000 00fa 4a2f 686f  rams..r.....J/ho
+00000270: 6d65 2f74 686f 6d61 732f 4964 6561 5072  me/thomas/IdeaPr
+00000280: 6f6a 6563 7473 2f42 6c75 6543 6173 742f  ojects/BlueCast/
+00000290: 626c 7565 6361 7374 2f67 656e 6572 616c  bluecast/general
+000002a0: 5f75 7469 6c73 2f67 656e 6572 616c 5f75  _utils/general_u
+000002b0: 7469 6c73 2e70 79da 1163 6865 636b 5f67  tils.py..check_g
+000002c0: 7075 5f73 7570 706f 7274 0a00 0000 7318  pu_support....s.
+000002d0: 0000 000e 0110 010e 010a 0102 010c 0108  ................
+000002e0: 0106 010c 0108 0106 0102 fe72 1700 0000  ...........r....
+000002f0: da07 6d65 7373 6167 6563 0100 0000 0000  ..messagec......
+00000300: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000310: 0000 7316 0000 0074 00a0 017c 00a1 0101  ..s....t...|....
+00000320: 0074 027c 0083 0101 0064 0053 0029 014e  .t.|.....d.S.).N
+00000330: 2903 da07 6c6f 6767 696e 67da 0469 6e66  )...logging..inf
+00000340: 6f72 1100 0000 2901 7218 0000 0072 1500  or....).r....r..
+00000350: 0000 7215 0000 0072 1600 0000 da06 6c6f  ..r....r......lo
+00000360: 6767 6572 1800 0000 7304 0000 000a 010c  gger....s.......
+00000370: 0172 1b00 0000 da0f 6175 746f 6d6c 5f69  .r......automl_i
+00000380: 6e73 7461 6e63 65fa 042e 6461 74da 0e63  nstance...dat..c
+00000390: 6c61 7373 5f69 6e73 7461 6e63 65da 0966  lass_instance..f
+000003a0: 696c 655f 7061 7468 da09 6669 6c65 5f6e  ile_path..file_n
+000003b0: 616d 65da 0966 696c 655f 7479 7065 6304  ame..file_typec.
+000003c0: 0000 0000 0000 0000 0000 0006 0000 0004  ................
+000003d0: 0000 0043 0000 0073 3c00 0000 7c01 7209  ...C...s<...|.r.
+000003e0: 7c01 7c02 1700 7c03 1700 7d04 6e04 7c02  |.|...|...}.n.|.
+000003f0: 7c03 1700 7d04 7400 7c04 6401 8302 7d05  |...}.t.|.d...}.
+00000400: 7401 a002 7c00 7c05 a102 0100 7c05 a003  t...|.|.....|...
+00000410: a100 0100 6402 5300 2903 6153 0100 000a  ....d.S.).aS....
+00000420: 2020 2020 5461 6b65 7320 6120 7072 6574      Takes a pret
+00000430: 7261 696e 6564 206d 6f64 656c 2061 6e64  rained model and
+00000440: 2073 6176 6573 2069 7420 7669 6120 6469   saves it via di
+00000450: 6c6c 2e0a 2020 2020 3a70 6172 616d 2063  ll..    :param c
+00000460: 6c61 7373 5f69 6e73 7461 6e63 653a 2054  lass_instance: T
+00000470: 616b 6573 2069 6e73 7461 6e63 6520 6f66  akes instance of
+00000480: 2061 2042 6c75 6543 6173 7420 636c 6173   a BlueCast clas
+00000490: 732e 0a20 2020 203a 7061 7261 6d20 6669  s..    :param fi
+000004a0: 6c65 5f70 6174 683a 2054 616b 6573 2061  le_path: Takes a
+000004b0: 2073 7472 696e 6720 636f 6e74 6169 6e69   string containi
+000004c0: 6e67 2074 6865 2066 756c 6c20 6162 736f  ng the full abso
+000004d0: 6c75 7465 2070 6174 682e 0a20 2020 203a  lute path..    :
+000004e0: 7061 7261 6d20 6669 6c65 5f6e 616d 653a  param file_name:
+000004f0: 2054 616b 6573 2061 2073 7472 696e 6720   Takes a string 
+00000500: 636f 6e74 6169 6e69 6e67 2074 6865 2077  containing the w
+00000510: 686f 6c65 2066 696c 6520 6e61 6d65 2e0a  hole file name..
+00000520: 2020 2020 3a70 6172 616d 2066 696c 655f      :param file_
+00000530: 7479 7065 3a20 5461 6b65 7320 7468 6520  type: Takes the 
+00000540: 6578 7065 6374 6564 2074 7970 6520 6f66  expected type of
+00000550: 2066 696c 6520 746f 2065 7870 6f72 742e   file to export.
+00000560: 0a20 2020 203a 7265 7475 726e 3a0a 2020  .    :return:.  
+00000570: 2020 da02 7762 4e29 04da 046f 7065 6eda    ..wbN)...open.
+00000580: 0670 6963 6b6c 65da 0464 756d 70da 0563  .pickle..dump..c
+00000590: 6c6f 7365 2906 721e 0000 0072 1f00 0000  lose).r....r....
+000005a0: 7220 0000 0072 2100 0000 da09 6675 6c6c  r ...r!.....full
+000005b0: 5f70 6174 68da 0b66 696c 6568 616e 646c  _path..filehandl
+000005c0: 6572 7215 0000 0072 1500 0000 7216 0000  err....r....r...
+000005d0: 00da 1273 6176 655f 746f 5f70 726f 6475  ...save_to_produ
+000005e0: 6374 696f 6e1d 0000 0073 0c00 0000 040e  ction....s......
+000005f0: 0e01 0802 0a01 0c01 0c01 7229 0000 0063  ..........r)...c
+00000600: 0300 0000 0000 0000 0000 0000 0600 0000  ................
+00000610: 0800 0000 4300 0000 7358 0000 007c 0072  ....C...sX...|.r
+00000620: 077c 007c 0117 007d 036e 027c 017d 037a  .|.|...}.n.|.}.z
+00000630: 0774 007c 0364 0183 027d 0457 006e 1004  .t.|.d...}.W.n..
+00000640: 0074 0179 2001 0001 0001 0074 007c 037c  .t.y ......t.|.|
+00000650: 0217 0064 0183 027d 0459 006e 0177 0074  ...d...}.Y.n.w.t
+00000660: 02a0 037c 04a1 017d 057c 04a0 04a1 0001  ...|...}.|......
+00000670: 007c 0553 0029 0261 9a01 0000 0a20 2020  .|.S.).a.....   
+00000680: 204c 6f61 6420 696e 2061 2070 7265 7472   Load in a pretr
+00000690: 6169 6e65 6420 6175 746f 206d 6c20 6d6f  ained auto ml mo
+000006a0: 6465 6c2e 2054 6869 7320 6675 6e63 7469  del. This functi
+000006b0: 6f6e 2077 696c 6c20 7472 7920 746f 206c  on will try to l
+000006c0: 6f61 6420 7468 6520 6d6f 6465 6c20 6173  oad the model as
+000006d0: 2070 726f 7669 6465 642e 0a20 2020 2049   provided..    I
+000006e0: 7420 6861 7320 6120 6661 6c6c 6261 636b  t has a fallback
+000006f0: 206c 6f67 6963 2074 6f20 696d 7075 7465   logic to impute
+00000700: 202e 6461 7420 6173 2066 696c 655f 7479   .dat as file_ty
+00000710: 7065 2069 6e20 6361 7365 2074 6865 2069  pe in case the i
+00000720: 6d70 6f72 7420 6661 696c 7320 696e 6974  mport fails init
+00000730: 6961 6c6c 792e 0a20 2020 203a 7061 7261  ially..    :para
+00000740: 6d20 6669 6c65 5f70 6174 683a 2054 616b  m file_path: Tak
+00000750: 6573 2061 2073 7472 696e 6720 636f 6e74  es a string cont
+00000760: 6169 6e69 6e67 2074 6865 2066 756c 6c20  aining the full 
+00000770: 6162 736f 6c75 7465 2070 6174 682e 0a20  absolute path.. 
+00000780: 2020 203a 7061 7261 6d20 6669 6c65 5f6e     :param file_n
+00000790: 616d 653a 2054 616b 6573 2061 2073 7472  ame: Takes a str
+000007a0: 696e 6720 636f 6e74 6169 6e69 6e67 2074  ing containing t
+000007b0: 6865 2077 686f 6c65 2066 696c 6520 6e61  he whole file na
+000007c0: 6d65 2e0a 2020 2020 3a70 6172 616d 2066  me..    :param f
+000007d0: 696c 655f 7479 7065 3a20 5461 6b65 7320  ile_type: Takes 
+000007e0: 7468 6520 6578 7065 6374 6564 2074 7970  the expected typ
+000007f0: 6520 6f66 2066 696c 6520 746f 2069 6d70  e of file to imp
+00000800: 6f72 742e 0a20 2020 203a 7265 7475 726e  ort..    :return
+00000810: 3a0a 2020 2020 da02 7262 2905 7223 0000  :.    ..rb).r#..
+00000820: 0072 1200 0000 7224 0000 00da 046c 6f61  .r....r$.....loa
+00000830: 6472 2600 0000 2906 721f 0000 0072 2000  dr&...).r....r .
+00000840: 0000 7221 0000 0072 2700 0000 7228 0000  ..r!...r'...r(..
+00000850: 005a 0c61 7574 6f6d 6c5f 6d6f 6465 6c72  .Z.automl_modelr
+00000860: 1500 0000 7215 0000 0072 1600 0000 da13  ....r....r......
+00000870: 6c6f 6164 5f66 6f72 5f70 726f 6475 6374  load_for_product
+00000880: 696f 6e34 0000 0073 1600 0000 040d 0a01  ion4...s........
+00000890: 0402 0201 0e01 0c01 1201 02ff 0a02 0801  ................
+000008a0: 0401 722c 0000 0029 034e 721c 0000 0072  ..r,...).Nr....r
+000008b0: 1d00 0000 2910 da07 5f5f 646f 635f 5f72  ....)...__doc__r
+000008c0: 1900 0000 da06 7479 7069 6e67 7202 0000  ......typingr...
+000008d0: 0072 0300 0000 5a04 6469 6c6c 7224 0000  .r....Z.dillr$..
+000008e0: 00da 056e 756d 7079 720c 0000 005a 0778  ...numpyr....Z.x
+000008f0: 6762 6f6f 7374 7210 0000 00da 0373 7472  gboostr......str
+00000900: 7217 0000 0072 1b00 0000 7229 0000 0072  r....r....r)...r
+00000910: 2c00 0000 7215 0000 0072 1500 0000 7215  ,...r....r....r.
+00000920: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000930: 653e 0100 0000 7344 0000 0004 0008 0110  e>....sD........
+00000940: 0108 0208 0108 010e 0312 0e02 0702 0102  ................
+00000950: 0104 fc02 0102 ff06 0202 fe02 0302 fd02  ................
+00000960: 0402 fc02 050a fb02 1802 0102 0104 fd06  ................
+00000970: 0102 ff02 0202 fe02 0302 fd02 040e fc    ...............
```

### Comparing `bluecast-0.2/bluecast/general_utils/general_utils.py` & `bluecast-0.3/bluecast/general_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-0.3/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 982 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 d603 0000  o..........d....
+00000000: 550d 0d0a 0000 0000 f058 8164 d603 0000  U........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6401 6404 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a0a 6401 6404 6c0b 5a0c 6508 6405 650a  Z.d.d.l.Z.e.d.e.
 00000070: 6a0d 650c 6a0e 8303 5a0f 6508 6406 650a  j.e.j...Z.e.d.e.
@@ -13,78 +13,77 @@
 000000c0: 2ee9 0000 0000 2902 da03 4142 43da 0e61  ......)...ABC..a
 000000d0: 6273 7472 6163 746d 6574 686f 6429 04da  bstractmethod)..
 000000e0: 0341 6e79 da08 4f70 7469 6f6e 616c da05  .Any..Optional..
 000000f0: 5475 706c 65da 0754 7970 6556 6172 4eda  Tuple..TypeVarN.
 00000100: 0f50 7265 6469 6374 6564 5072 6f62 6173  .PredictedProbas
 00000110: da10 5072 6564 6963 7465 6443 6c61 7373  ..PredictedClass
 00000120: 6573 6300 0000 0000 0000 0000 0000 0000  esc.............
-00000130: 0000 000c 0000 0040 0000 0073 5e00 0000  .......@...s^...
-00000140: 6500 5a01 6400 5a02 6401 5a03 6504 6402  e.Z.d.Z.d.Z.e.d.
-00000150: 6505 6a06 6403 6505 6a06 6404 6505 6a07  e.j.d.e.j.d.e.j.
-00000160: 6405 6505 6a07 6406 6508 6509 1900 660a  d.e.j.d.e.e...f.
-00000170: 6407 6408 8404 8301 5a0a 6504 6409 6505  d.d.....Z.e.d.e.
-00000180: 6a06 6406 650b 650c 650d 6602 1900 6604  j.d.e.e.e.f...f.
-00000190: 640a 640b 8404 8301 5a0e 640c 5300 290d  d.d.....Z.d.S.).
-000001a0: da10 4261 7365 436c 6173 734d 6c4d 6f64  ..BaseClassMlMod
-000001b0: 656c 7abe 4261 7365 2063 6c61 7373 2066  elz.Base class f
-000001c0: 6f72 2061 6c6c 204d 4c20 6d6f 6465 6c73  or all ML models
-000001d0: 2e0a 0a20 2020 2045 6e66 6f72 6365 7320  ...    Enforces 
-000001e0: 7468 6520 696d 706c 656d 656e 7461 7469  the implementati
-000001f0: 6f6e 206f 6620 7468 6520 6669 7420 616e  on of the fit an
-00000200: 6420 7072 6564 6963 7420 6d65 7468 6f64  d predict method
-00000210: 732e 0a20 2020 2049 6620 6879 7065 7270  s..    If hyperp
-00000220: 6172 616d 6574 6572 2074 756e 696e 6720  arameter tuning 
-00000230: 6973 2072 6571 7569 7265 642c 2074 6865  is required, the
-00000240: 6e20 7468 6520 6669 7420 6d65 7468 6f64  n the fit method
-00000250: 2073 686f 756c 6420 696d 706c 656d 656e   should implemen
-00000260: 7420 7468 6520 7475 6e69 6e67 2e0a 2020  t the tuning..  
-00000270: 2020 da07 785f 7472 6169 6eda 0678 5f74    ..x_train..x_t
-00000280: 6573 74da 0779 5f74 7261 696e da06 795f  est..y_train..y_
-00000290: 7465 7374 da06 7265 7475 726e 6305 0000  test..returnc...
-000002a0: 0000 0000 0000 0000 0005 0000 0001 0000  ................
-000002b0: 0043 0000 0073 0400 0000 6400 5300 2901  .C...s....d.S.).
-000002c0: 4ea9 0029 05da 0473 656c 6672 0b00 0000  N..)...selfr....
-000002d0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-000002e0: 1000 0000 7210 0000 00fa 512f 5573 6572  ....r.....Q/User
-000002f0: 732f 7468 6f6d 6173 6d65 6973 736e 6572  s/thomasmeissner
-00000300: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
-00000310: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
-00000320: 6d6c 5f6d 6f64 656c 6c69 6e67 2f62 6173  ml_modelling/bas
-00000330: 655f 636c 6173 7365 732e 7079 da03 6669  e_classes.py..fi
-00000340: 7413 0000 0073 0200 0000 0408 7a14 4261  t....s......z.Ba
-00000350: 7365 436c 6173 734d 6c4d 6f64 656c 2e66  seClassMlModel.f
-00000360: 6974 da02 6466 6302 0000 0000 0000 0000  it..dfc.........
-00000370: 0000 0002 0000 0001 0000 0043 0000 0073  ...........C...s
-00000380: 0400 0000 6401 5300 2902 7a71 0a20 2020  ....d.S.).zq.   
-00000390: 2020 2020 2050 7265 6469 6374 206f 6e20       Predict on 
-000003a0: 756e 7365 656e 2064 6174 612e 0a0a 2020  unseen data...  
-000003b0: 2020 2020 2020 3a72 6574 7572 6e20 7475        :return tu
-000003c0: 706c 6520 6f66 2070 7265 6469 6374 6564  ple of predicted
-000003d0: 2070 726f 6261 6269 6c69 7469 6573 2061   probabilities a
-000003e0: 6e64 2070 7265 6469 6374 6564 2063 6c61  nd predicted cla
-000003f0: 7373 6573 0a20 2020 2020 2020 204e 7210  sses.        Nr.
-00000400: 0000 0029 0272 1100 0000 7214 0000 0072  ...).r....r....r
-00000410: 1000 0000 7210 0000 0072 1200 0000 da07  ....r....r......
-00000420: 7072 6564 6963 741d 0000 0073 0200 0000  predict....s....
-00000430: 0407 7a18 4261 7365 436c 6173 734d 6c4d  ..z.BaseClassMlM
-00000440: 6f64 656c 2e70 7265 6469 6374 4e29 0fda  odel.predictN)..
-00000450: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000460: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000470: 655f 5fda 075f 5f64 6f63 5f5f 7203 0000  e__..__doc__r...
-00000480: 00da 0270 64da 0944 6174 6146 7261 6d65  ...pd..DataFrame
-00000490: da06 5365 7269 6573 7205 0000 0072 0400  ..Seriesr....r..
-000004a0: 0000 7213 0000 0072 0600 0000 7208 0000  ..r....r....r...
-000004b0: 0072 0900 0000 7215 0000 0072 1000 0000  .r....r....r....
-000004c0: 7210 0000 0072 1000 0000 7212 0000 0072  r....r....r....r
-000004d0: 0a00 0000 0c00 0000 7320 0000 0008 0004  ........s ......
-000004e0: 0102 0602 0104 0202 fe04 0302 fd04 0402  ................
-000004f0: fc04 0502 fb06 060c fa02 0922 0172 0a00  ...........".r..
-00000500: 0000 2912 7219 0000 00da 0361 6263 7202  ..).r......abcr.
-00000510: 0000 0072 0300 0000 da06 7479 7069 6e67  ...r......typing
-00000520: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
-00000530: 0700 0000 da05 6e75 6d70 79da 026e 70da  ......numpy..np.
-00000540: 0670 616e 6461 7372 1a00 0000 da07 6e64  .pandasr......nd
-00000550: 6172 7261 7972 1c00 0000 7208 0000 0072  arrayr....r....r
-00000560: 0900 0000 720a 0000 0072 1000 0000 7210  ....r....r....r.
-00000570: 0000 0072 1000 0000 7212 0000 00da 083c  ...r....r......<
-00000580: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00000590: 0400 1001 1801 0802 0801 1002 1001 1403  ................
+00000130: 0000 0007 0000 0040 0000 0073 5400 0000  .......@...sT...
+00000140: 6500 5a01 6400 5a02 6401 5a03 6504 6505  e.Z.d.Z.d.Z.e.e.
+00000150: 6a06 6505 6a06 6505 6a07 6505 6a07 6508  j.e.j.e.j.e.j.e.
+00000160: 6509 1900 6402 9c05 6403 6404 8404 8301  e...d...d.d.....
+00000170: 5a0a 6504 6505 6a06 650b 650c 650d 6602  Z.e.e.j.e.e.e.f.
+00000180: 1900 6405 9c02 6406 6407 8404 8301 5a0e  ..d...d.d.....Z.
+00000190: 6408 5300 2909 da10 4261 7365 436c 6173  d.S.)...BaseClas
+000001a0: 734d 6c4d 6f64 656c 7abe 4261 7365 2063  sMlModelz.Base c
+000001b0: 6c61 7373 2066 6f72 2061 6c6c 204d 4c20  lass for all ML 
+000001c0: 6d6f 6465 6c73 2e0a 0a20 2020 2045 6e66  models...    Enf
+000001d0: 6f72 6365 7320 7468 6520 696d 706c 656d  orces the implem
+000001e0: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
+000001f0: 6669 7420 616e 6420 7072 6564 6963 7420  fit and predict 
+00000200: 6d65 7468 6f64 732e 0a20 2020 2049 6620  methods..    If 
+00000210: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
+00000220: 756e 696e 6720 6973 2072 6571 7569 7265  uning is require
+00000230: 642c 2074 6865 6e20 7468 6520 6669 7420  d, then the fit 
+00000240: 6d65 7468 6f64 2073 686f 756c 6420 696d  method should im
+00000250: 706c 656d 656e 7420 7468 6520 7475 6e69  plement the tuni
+00000260: 6e67 2e0a 2020 2020 2905 da07 785f 7472  ng..    )...x_tr
+00000270: 6169 6eda 0678 5f74 6573 74da 0779 5f74  ain..x_test..y_t
+00000280: 7261 696e da06 795f 7465 7374 da06 7265  rain..y_test..re
+00000290: 7475 726e 6305 0000 0000 0000 0000 0000  turnc...........
+000002a0: 0005 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+000002b0: 0000 6400 5300 2901 4ea9 0029 05da 0473  ..d.S.).N..)...s
+000002c0: 656c 6672 0b00 0000 720c 0000 0072 0d00  elfr....r....r..
+000002d0: 0000 720e 0000 0072 1000 0000 7210 0000  ..r....r....r...
+000002e0: 00fa 482f 686f 6d65 2f74 686f 6d61 732f  ..H/home/thomas/
+000002f0: 4964 6561 5072 6f6a 6563 7473 2f42 6c75  IdeaProjects/Blu
+00000300: 6543 6173 742f 626c 7565 6361 7374 2f6d  eCast/bluecast/m
+00000310: 6c5f 6d6f 6465 6c6c 696e 672f 6261 7365  l_modelling/base
+00000320: 5f63 6c61 7373 6573 2e70 79da 0366 6974  _classes.py..fit
+00000330: 1300 0000 7302 0000 0000 087a 1442 6173  ....s......z.Bas
+00000340: 6543 6c61 7373 4d6c 4d6f 6465 6c2e 6669  eClassMlModel.fi
+00000350: 7429 02da 0264 6672 0f00 0000 6302 0000  t)...dfr....c...
+00000360: 0000 0000 0000 0000 0002 0000 0001 0000  ................
+00000370: 0043 0000 0073 0400 0000 6401 5300 2902  .C...s....d.S.).
+00000380: 7a71 0a20 2020 2020 2020 2050 7265 6469  zq.        Predi
+00000390: 6374 206f 6e20 756e 7365 656e 2064 6174  ct on unseen dat
+000003a0: 612e 0a0a 2020 2020 2020 2020 3a72 6574  a...        :ret
+000003b0: 7572 6e20 7475 706c 6520 6f66 2070 7265  urn tuple of pre
+000003c0: 6469 6374 6564 2070 726f 6261 6269 6c69  dicted probabili
+000003d0: 7469 6573 2061 6e64 2070 7265 6469 6374  ties and predict
+000003e0: 6564 2063 6c61 7373 6573 0a20 2020 2020  ed classes.     
+000003f0: 2020 204e 7210 0000 0029 0272 1100 0000     Nr....).r....
+00000400: 7214 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+00000410: 1200 0000 da07 7072 6564 6963 741d 0000  ......predict...
+00000420: 0073 0200 0000 0007 7a18 4261 7365 436c  .s......z.BaseCl
+00000430: 6173 734d 6c4d 6f64 656c 2e70 7265 6469  assMlModel.predi
+00000440: 6374 4e29 0fda 085f 5f6e 616d 655f 5fda  ctN)...__name__.
+00000450: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000460: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00000470: 5f5f 7203 0000 00da 0270 64da 0944 6174  __r......pd..Dat
+00000480: 6146 7261 6d65 da06 5365 7269 6573 7205  aFrame..Seriesr.
+00000490: 0000 0072 0400 0000 7213 0000 0072 0600  ...r....r....r..
+000004a0: 0000 7208 0000 0072 0900 0000 7215 0000  ..r....r....r...
+000004b0: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
+000004c0: 7212 0000 0072 0a00 0000 0c00 0000 7314  r....r........s.
+000004d0: 0000 0008 0104 0602 0304 0104 0104 0104  ................
+000004e0: 0106 fa0e 0902 0172 0a00 0000 2912 7219  .......r....).r.
+000004f0: 0000 00da 0361 6263 7202 0000 0072 0300  .....abcr....r..
+00000500: 0000 da06 7479 7069 6e67 7204 0000 0072  ....typingr....r
+00000510: 0500 0000 7206 0000 0072 0700 0000 da05  ....r....r......
+00000520: 6e75 6d70 79da 026e 70da 0670 616e 6461  numpy..np..panda
+00000530: 7372 1a00 0000 da07 6e64 6172 7261 7972  sr......ndarrayr
+00000540: 1c00 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
+00000550: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
+00000560: 0000 7212 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000570: 3e01 0000 0073 0e00 0000 0401 1001 1802  >....s..........
+00000580: 0801 0802 1001 1003                      ........
```

### Comparing `bluecast-0.2/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-0.3/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 18:43:33 2023 UTC, .py size: 12506 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5521 8264 da30 0000  o.......U!.d.0..
+00000000: 6f0d 0d0a 0000 0000 4e76 9564 f434 0000  o.......Nv.d.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -70,462 +70,495 @@
 00000450: 0000 0000 0000 0000 0500 0000 0200 0000  ................
 00000460: 4300 0000 7322 0000 0064 007c 005f 007c  C...s"...d.|._.|
 00000470: 017c 005f 017c 027c 005f 027c 037c 005f  .|._.|.|._.|.|._
 00000480: 037c 047c 005f 0464 0053 0029 014e 2905  .|.|._.d.S.).N).
 00000490: da05 6d6f 6465 6c72 1000 0000 7213 0000  ..modelr....r...
 000004a0: 0072 1400 0000 7215 0000 0029 05da 0473  .r....r....)...s
 000004b0: 656c 6672 1000 0000 7213 0000 0072 1400  elfr....r....r..
-000004c0: 0000 7215 0000 00a9 0072 1800 0000 fa4c  ..r......r.....L
-000004d0: 2f55 7365 7273 2f74 686f 6d61 736d 6569  /Users/thomasmei
-000004e0: 7373 6e65 722f 4964 6561 5072 6f6a 6563  ssner/IdeaProjec
-000004f0: 7473 2f42 6c75 6543 6173 742f 626c 7565  ts/BlueCast/blue
-00000500: 6361 7374 2f6d 6c5f 6d6f 6465 6c6c 696e  cast/ml_modellin
-00000510: 672f 7867 626f 6f73 742e 7079 da08 5f5f  g/xgboost.py..__
-00000520: 696e 6974 5f5f 1d00 0000 730a 0000 0006  init__....s.....
-00000530: 0706 0106 0106 010a 017a 1558 6762 6f6f  .........z.Xgboo
-00000540: 7374 4d6f 6465 6c2e 5f5f 696e 6974 5f5f  stModel.__init__
-00000550: da01 79da 0672 6574 7572 6e63 0200 0000  ..y..returnc....
-00000560: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000570: 4300 0000 7324 0000 0074 0074 01a0 02a1  C...s$...t.t....
-00000580: 009b 0064 019d 0283 0101 0074 036a 0464  ...d.......t.j.d
-00000590: 027c 0164 038d 027d 027c 0253 0029 047a  .|.d...}.|.S.).z
-000005a0: 2943 616c 6375 6c61 7465 2063 6c61 7373  )Calculate class
-000005b0: 2077 6569 6768 7473 206f 6620 7461 7267   weights of targ
-000005c0: 6574 2063 6f6c 756d 6e2e 7a29 3a20 5374  et column.z): St
-000005d0: 6172 7420 6361 6c63 756c 6174 696e 6720  art calculating 
-000005e0: 7461 7267 6574 2063 6c61 7373 2077 6569  target class wei
-000005f0: 6768 7473 2eda 0862 616c 616e 6365 6429  ghts...balanced)
-00000600: 0272 0800 0000 721b 0000 0029 0572 0d00  .r....r....).r..
-00000610: 0000 7202 0000 00da 0675 7463 6e6f 7772  ..r......utcnowr
-00000620: 0800 0000 da15 636f 6d70 7574 655f 7361  ......compute_sa
-00000630: 6d70 6c65 5f77 6569 6768 7429 0372 1700  mple_weight).r..
-00000640: 0000 721b 0000 00da 0f63 6c61 7373 6573  ..r......classes
-00000650: 5f77 6569 6768 7473 7218 0000 0072 1800  _weightsr....r..
-00000660: 0000 7219 0000 00da 1763 616c 6375 6c61  ..r......calcula
-00000670: 7465 5f63 6c61 7373 5f77 6569 6768 7473  te_class_weights
-00000680: 2a00 0000 730a 0000 0012 0204 0104 0106  *...s...........
-00000690: ff04 037a 2458 6762 6f6f 7374 4d6f 6465  ...z$XgboostMode
-000006a0: 6c2e 6361 6c63 756c 6174 655f 636c 6173  l.calculate_clas
-000006b0: 735f 7765 6967 6874 7363 0100 0000 0000  s_weightsc......
-000006c0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000006d0: 0000 737a 0000 0074 0074 01a0 02a1 009b  ..sz...t.t......
-000006e0: 0064 019d 0283 0101 007c 006a 0373 1974  .d.......|.j.s.t
-000006f0: 0483 007c 005f 0374 0074 01a0 02a1 009b  ...|._.t.t......
-00000700: 0064 029d 0283 0101 007c 006a 0573 2974  .d.......|.j.s)t
-00000710: 0683 007c 005f 0574 0074 01a0 02a1 009b  ...|._.t.t......
-00000720: 0064 039d 0283 0101 007c 006a 0773 3b74  .d.......|.j.s;t
-00000730: 0883 007c 005f 0774 0074 01a0 02a1 009b  ...|._.t.t......
-00000740: 0064 049d 0283 0101 0064 0553 0064 0553  .d.......d.S.d.S
-00000750: 0029 067a 364c 6f61 6420 6d75 6c74 6970  .).z6Load multip
-00000760: 6c65 2063 6f6e 6669 6773 206f 7220 6c6f  le configs or lo
-00000770: 6164 2064 6566 6175 6c74 2063 6f6e 6669  ad default confi
-00000780: 6773 2069 6e73 7465 6164 2e7a 323a 2053  gs instead.z2: S
-00000790: 7461 7274 206c 6f61 6469 6e67 2065 7869  tart loading exi
-000007a0: 7374 696e 6720 6f72 2064 6566 6175 6c74  sting or default
-000007b0: 2063 6f6e 6669 6720 6669 6c65 732e 2e7a   config files..z
-000007c0: 1e3a 204c 6f61 6420 6465 6661 756c 7420  .: Load default 
-000007d0: 5472 6169 6e69 6e67 436f 6e66 6967 2e7a  TrainingConfig.z
-000007e0: 273a 204c 6f61 6420 6465 6661 756c 7420  ': Load default 
-000007f0: 5867 626f 6f73 7454 756e 6550 6172 616d  XgboostTuneParam
-00000800: 7343 6f6e 6669 672e 7a27 3a20 4c6f 6164  sConfig.z': Load
-00000810: 2064 6566 6175 6c74 2058 6762 6f6f 7374   default Xgboost
-00000820: 4669 6e61 6c50 6172 616d 436f 6e66 6967  FinalParamConfig
-00000830: 2e4e 2909 720d 0000 0072 0200 0000 721e  .N).r....r....r.
-00000840: 0000 0072 1300 0000 7209 0000 0072 1400  ...r....r....r..
-00000850: 0000 720b 0000 0072 1500 0000 720a 0000  ..r....r....r...
-00000860: 0029 0172 1700 0000 7218 0000 0072 1800  .).r....r....r..
-00000870: 0000 7219 0000 00da 1063 6865 636b 5f6c  ..r......check_l
-00000880: 6f61 645f 636f 6e66 7332 0000 0073 1600  oad_confs2...s..
-00000890: 0000 1202 0601 0801 1201 0602 0801 1201  ................
-000008a0: 0602 0801 1601 04fe 7a1d 5867 626f 6f73  ........z.Xgboos
-000008b0: 744d 6f64 656c 2e63 6865 636b 5f6c 6f61  tModel.check_loa
-000008c0: 645f 636f 6e66 73da 0778 5f74 7261 696e  d_confs..x_train
-000008d0: da06 785f 7465 7374 da07 795f 7472 6169  ..x_test..y_trai
-000008e0: 6eda 0679 5f74 6573 7463 0500 0000 0000  n..y_testc......
-000008f0: 0000 0000 0000 0900 0000 0700 0000 4300  ..............C.
-00000900: 0000 73d2 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
-00000910: 0064 019d 0283 0101 007c 00a0 03a1 0001  .d.......|......
-00000920: 007c 006a 0472 137c 006a 0573 1774 0664  .|.j.r.|.j.s.t.d
-00000930: 0283 0182 017c 006a 056a 0772 237c 00a0  .....|.j.j.r#|..
-00000940: 087c 017c 027c 037c 04a1 0401 0074 0964  .|.|.|.|.....t.d
-00000950: 0383 0101 007c 006a 046a 0a72 397c 00a0  .....|.j.j.r9|..
-00000960: 0b7c 03a1 017d 0574 0c6a 0d7c 017c 037c  .|...}.t.j.|.|.|
-00000970: 0564 048d 037d 066e 0774 0c6a 0d7c 017c  .d...}.n.t.j.|.|
-00000980: 0364 058d 027d 0674 0c6a 0d7c 027c 0464  .d...}.t.j.|.|.d
-00000990: 058d 027d 077c 0664 0666 027c 0764 0766  ...}.|.d.f.|.d.f
-000009a0: 0267 027d 0874 0c6a 0e7c 006a 046a 0f7c  .g.}.t.j.|.j.j.|
-000009b0: 067c 006a 046a 0f64 0819 007c 006a 056a  .|.j.j.d...|.j.j
-000009c0: 107c 0864 098d 057c 005f 1174 0964 0a83  .|.d...|._.t.d..
-000009d0: 0101 007c 006a 1153 0029 0b7a 3f54 7261  ...|.j.S.).z?Tra
-000009e0: 696e 2058 6762 6f6f 7374 206d 6f64 656c  in Xgboost model
-000009f0: 2e20 496e 636c 7564 6573 2068 7970 6572  . Includes hyper
-00000a00: 7061 7261 6d65 7465 7220 7475 6e69 6e67  parameter tuning
-00000a10: 206f 6e20 6465 6661 756c 742e 7a1e 3a20   on default.z.: 
-00000a20: 5374 6172 7420 6669 7474 696e 6720 5867  Start fitting Xg
-00000a30: 626f 6f73 7420 6d6f 6465 6c2e 7a2c 636f  boost model.z,co
-00000a40: 6e66 5f70 6172 616d 735f 7867 626f 6f73  nf_params_xgboos
-00000a50: 7420 6f72 2063 6f6e 665f 7472 6169 6e69  t or conf_traini
-00000a60: 6e67 2069 7320 4e6f 6e65 7a1e 4669 6e69  ng is Nonez.Fini
-00000a70: 7368 6564 2068 7970 6572 7061 7261 6d65  shed hyperparame
-00000a80: 7465 7220 7475 6e69 6e67 a902 da05 6c61  ter tuning....la
-00000a90: 6265 6cda 0677 6569 6768 74a9 0172 2800  bel..weight..r(.
-00000aa0: 0000 da05 7472 6169 6eda 0474 6573 74da  ....train..test.
-00000ab0: 0573 7465 7073 2903 da0f 6e75 6d5f 626f  .steps)...num_bo
-00000ac0: 6f73 745f 726f 756e 64da 1565 6172 6c79  ost_round..early
-00000ad0: 5f73 746f 7070 696e 675f 726f 756e 6473  _stopping_rounds
-00000ae0: da05 6576 616c 737a 1146 696e 6973 6865  ..evalsz.Finishe
-00000af0: 6420 7472 6169 6e69 6e67 2912 720d 0000  d training).r...
-00000b00: 0072 0200 0000 721e 0000 0072 2200 0000  .r....r....r"...
-00000b10: 7215 0000 0072 1300 0000 da0a 5661 6c75  r....r......Valu
-00000b20: 6545 7272 6f72 da0e 6175 746f 7475 6e65  eError..autotune
-00000b30: 5f6d 6f64 656c da08 6175 746f 7475 6e65  _model..autotune
-00000b40: da05 7072 696e 74da 0d73 616d 706c 655f  ..print..sample_
-00000b50: 7765 6967 6874 7221 0000 00da 0378 6762  weightr!.....xgb
-00000b60: da07 444d 6174 7269 7872 2b00 0000 da06  ..DMatrixr+.....
-00000b70: 7061 7261 6d73 722f 0000 0072 1600 0000  paramsr/...r....
-00000b80: 2909 7217 0000 0072 2300 0000 7224 0000  ).r....r#...r$..
-00000b90: 0072 2500 0000 7226 0000 0072 2000 0000  .r%...r&...r ...
-00000ba0: da07 645f 7472 6169 6eda 0664 5f74 6573  ..d_train..d_tes
-00000bb0: 74da 0865 7661 6c5f 7365 7472 1800 0000  t..eval_setr....
-00000bc0: 7218 0000 0072 1900 0000 da03 6669 7441  r....r......fitA
-00000bd0: 0000 0073 2c00 0000 1208 0801 0c02 0801  ...s,...........
-00000be0: 0802 1001 0802 0802 0a01 1201 0e02 0e01  ................
-00000bf0: 1001 0402 0601 0201 0a01 0601 0201 08fb  ................
-00000c00: 0807 0601 7a10 5867 626f 6f73 744d 6f64  ....z.XgboostMod
-00000c10: 656c 2e66 6974 6305 0000 0000 0000 0000  el.fitc.........
-00000c20: 0000 000b 0000 000a 0000 0003 0000 0073  ...............s
-00000c30: c201 0000 7400 7401 a002 a100 9b00 6401  ....t.t.......d.
-00000c40: 9d02 8301 0100 7403 6a04 7c02 8804 6402  ......t.j.|...d.
-00000c50: 8d02 8900 7405 8300 8902 8801 a006 a100  ....t...........
-00000c60: 0100 8801 6a07 7220 8801 6a08 7220 8801  ....j.r ..j.r ..
-00000c70: 6a09 7324 740a 6403 8301 8201 8700 8701  j.s$t.d.........
-00000c80: 8702 8703 8704 8705 6606 6404 6405 8408  ........f.d.d...
-00000c90: 7d05 6406 7d06 740b 6a0c 6a0d 6407 8801  }.d.}.t.j.j.d...
-00000ca0: 6a08 6a0e 6408 8d02 7d07 740b 6a0f 6409  j.j.d...}.t.j.d.
-00000cb0: 7c07 7c06 9b00 640a 9d02 640b 8d03 7d08  |.|...d...d...}.
-00000cc0: 7c08 6a10 7c05 8801 6a08 6a11 8801 6a08  |.j.|...j.j...j.
-00000cd0: 6a12 6407 6407 640c 8d05 0100 7a16 740b  j.d.d.d.....z.t.
-00000ce0: 6a13 a014 7c08 a101 7d09 7c09 a015 a100  j...|...}.|.....
-00000cf0: 0100 740b 6a13 a016 7c08 a101 7d09 7c09  ..t.j...|...}.|.
-00000d00: a015 a100 0100 5700 6e0c 0400 7417 7418  ......W.n...t.t.
-00000d10: 740a 6603 7976 0100 0100 0100 5900 6e01  t.f.yv......Y.n.
-00000d20: 7700 7c08 6a19 6a1a 7d0a 6900 640d 8801  w.|.j.j.}.i.d...
-00000d30: 6a09 6a1b 9301 640e 8801 6a09 6a1c 9301  j.j...d...j.j...
-00000d40: 640f 8801 6a09 6a1d 9301 6410 8802 9301  d...j.j...d.....
-00000d50: 6411 8805 a01e a100 9301 6412 7c0a 6412  d.........d.|.d.
-00000d60: 1900 9301 6413 7c0a 6413 1900 9301 6414  ....d.|.d.....d.
-00000d70: 7c0a 6414 1900 9301 6415 7c0a 6415 1900  |.d.....d.|.d...
-00000d80: 9301 6416 7c0a 6416 1900 9301 6417 7c0a  ..d.|.d.....d.|.
-00000d90: 6417 1900 9301 6418 7c0a 6418 1900 9301  d.....d.|.d.....
-00000da0: 6419 7c0a 6419 1900 9301 641a 7c0a 641a  d.|.d.....d.|.d.
-00000db0: 1900 9301 641b 8801 6a09 6a1f 9301 641c  ....d...j.j...d.
-00000dc0: 7c0a 641c 1900 9301 641d 7c0a 641d 1900  |.d.....d.|.d...
-00000dd0: 9301 8801 6a07 5f1a 7420 641e 8801 6a07  ....j._.t d...j.
-00000de0: 6a1a 8302 0100 7c0a 641f 1900 8801 6a07  j.....|.d.....j.
-00000df0: 5f21 6420 5300 2921 7a7b 5475 6e65 2068  _!d S.)!z{Tune h
-00000e00: 7970 6572 7061 7261 6d65 7465 7273 2e0a  yperparameters..
-00000e10: 0a20 2020 2020 2020 2041 6e20 616c 7465  .        An alte
-00000e20: 726e 6174 6976 6520 636f 6e66 6967 2063  rnative config c
-00000e30: 616e 2062 6520 7072 6f76 6964 6564 2074  an be provided t
-00000e40: 6f20 6f76 6572 7772 6974 6520 7468 6520  o overwrite the 
-00000e50: 6879 7065 7270 6172 616d 6574 6572 2073  hyperparameter s
-00000e60: 6561 7263 6820 7370 6163 652e 0a20 2020  earch space..   
-00000e70: 2020 2020 207a 2f3a 2053 7461 7274 2068       z/: Start h
-00000e80: 7970 6572 7061 7261 6d65 7465 7220 7475  yperparameter tu
-00000e90: 6e69 6e67 206f 6620 5867 626f 6f73 7420  ning of Xgboost 
-00000ea0: 6d6f 6465 6c2e 722a 0000 007a 3941 7420  model.r*...z9At 
-00000eb0: 6c65 6173 7420 6f6e 6520 6f66 2074 6865  least one of the
-00000ec0: 2063 6f6e 6669 6773 2069 7320 4e6f 6e65   configs is None
-00000ed0: 2c20 7768 6963 6820 6973 206e 6f74 2061  , which is not a
-00000ee0: 6c6c 6f77 6564 6301 0000 0000 0000 0000  llowedc.........
-00000ef0: 0000 000c 0000 000b 0000 0013 0000 0073  ...............s
-00000f00: 4202 0000 6900 6401 8801 6a00 6a01 9301  B...i.d...j.j...
-00000f10: 6402 8801 6a00 6a02 9301 6403 8801 6a00  d...j.j...d...j.
-00000f20: 6a03 9301 6404 8802 9301 6405 8805 a004  j...d.....d.....
-00000f30: a100 9301 6406 7c00 a005 6406 8801 6a00  ....d.|...d...j.
-00000f40: 6a06 8801 6a00 6a07 a103 9301 6407 7c00  j...j.j.....d.|.
-00000f50: a008 6407 8801 6a00 6a09 8801 6a00 6a0a  ..d...j.j...j.j.
-00000f60: a103 9301 6408 7c00 a008 6408 8801 6a00  ....d.|...d...j.
-00000f70: 6a0b 8801 6a00 6a0c a103 9301 6409 7c00  j...j.j.....d.|.
-00000f80: a005 6409 8801 6a00 6a0d 8801 6a00 6a0e  ..d...j.j...j.j.
-00000f90: a103 9301 640a 7c00 a008 640a 8801 6a00  ....d.|...d...j.
-00000fa0: 6a0f 8801 6a00 6a10 a103 9301 640b 7c00  j...j.j.....d.|.
-00000fb0: a008 640b 8801 6a00 6a11 8801 6a00 6a12  ..d...j.j...j.j.
-00000fc0: a103 9301 640c 7c00 a008 640c 8801 6a00  ....d.|...d...j.
-00000fd0: 6a13 8801 6a00 6a14 a103 9301 640d 7c00  j...j.j.....d.|.
-00000fe0: a008 640d 8801 6a00 6a15 8801 6a00 6a16  ..d...j.j...j.j.
-00000ff0: a103 9301 640e 7c00 a005 640e 8801 6a00  ....d.|...d...j.
-00001000: 6a17 8801 6a00 6a18 a103 9301 640f 8801  j...j.j.....d...
-00001010: 6a00 6a19 9301 6410 7c00 a005 6410 8801  j.j...d.|...d...
-00001020: 6a00 6a1a 8801 6a00 6a1b a103 9301 6411  j.j...j.j.....d.
-00001030: 7c00 a005 6411 8801 6a00 6a1c 8801 6a00  |...d...j.j...j.
-00001040: 6a1d a103 9301 7d01 7c00 a01e 6412 6413  j.....}.|...d.d.
-00001050: 6414 6702 a102 7d02 7c02 72ba 8801 a01f  d.g...}.|.r.....
-00001060: 8805 a101 7d03 7420 6a21 8803 8805 7c03  ....}.t j!....|.
-00001070: 6415 8d03 7d04 6e07 7420 6a21 8803 8805  d...}.n.t j!....
-00001080: 6416 8d02 7d04 7422 6a23 a024 7c00 6417  d...}.t"j#.$|.d.
-00001090: a102 7d05 8801 6a25 6a26 6418 6b02 9001  ..}...j%j&d.k...
-000010a0: 7202 7c04 6419 6602 8800 641a 6602 6702  r.|.d.f...d.f.g.
-000010b0: 7d06 7420 6a27 7c01 7c04 7c01 6410 1900  }.t j'|.|.|.d...
-000010c0: 8801 6a25 6a28 7c06 7c05 6701 8801 6a00  ..j%j(|.|.g...j.
-000010d0: 6a03 641b 8d07 7d07 7c07 a029 8800 a101  j.d...}.|..)....
-000010e0: 7d08 742a a02b 641c 641d 8400 7c08 4400  }.t*.+d.d...|.D.
-000010f0: 8301 a101 7d09 742c 8804 7c09 8302 641e  ....}.t,..|...d.
-00001100: 1400 7d0a 7c0a 5300 7420 6a2d 7c01 7c04  ..}.|.S.t j-|.|.
-00001110: 7c01 6410 1900 8801 6a25 6a28 8801 6a25  |.d.....j%j(..j%
-00001120: 6a26 6413 8801 6a25 6a2e 7c05 6701 8801  j&d...j%j.|.g...
-00001130: 6a25 6a2f 641f 8d09 7d0b 7c0b 6420 1900  j%j/d...}.|.d ..
-00001140: a030 a100 5300 2921 4eda 096f 626a 6563  .0..S.)!N..objec
-00001150: 7469 7665 da0b 6576 616c 5f6d 6574 7269  tive..eval_metri
-00001160: 63da 0776 6572 626f 7365 da0b 7472 6565  c..verbose..tree
-00001170: 5f6d 6574 686f 64da 096e 756d 5f63 6c61  _method..num_cla
-00001180: 7373 da09 6d61 785f 6465 7074 68da 0561  ss..max_depth..a
-00001190: 6c70 6861 da06 6c61 6d62 6461 da0a 6e75  lpha..lambda..nu
-000011a0: 6d5f 6c65 6176 6573 da09 7375 6273 616d  m_leaves..subsam
-000011b0: 706c 65da 1063 6f6c 7361 6d70 6c65 5f62  ple..colsample_b
-000011c0: 7974 7265 65da 1163 6f6c 7361 6d70 6c65  ytree..colsample
-000011d0: 5f62 796c 6576 656c da10 636f 6c73 616d  _bylevel..colsam
-000011e0: 706c 655f 6279 6e6f 6465 da11 6d69 6e5f  ple_bynode..min_
-000011f0: 6368 696c 645f 7361 6d70 6c65 73da 0365  child_samples..e
-00001200: 7461 722d 0000 00da 116e 756d 5f70 6172  tar-.....num_par
-00001210: 616c 6c65 6c5f 7472 6565 7235 0000 0054  allel_treer5...T
-00001220: 4672 2700 0000 722a 0000 007a 0d74 6573  Fr'...r*...z.tes
-00001230: 742d 6d6c 6f67 6c6f 7373 e901 0000 0072  t-mlogloss.....r
-00001240: 2b00 0000 722c 0000 0029 0572 2e00 0000  +...r,...).r....
-00001250: 722f 0000 0072 3000 0000 da09 6361 6c6c  r/...r0.....call
-00001260: 6261 636b 73da 0c76 6572 626f 7365 5f65  backs..verbose_e
-00001270: 7661 6c63 0100 0000 0000 0000 0000 0000  valc............
-00001280: 0200 0000 0500 0000 5300 0000 f316 0000  ........S.......
-00001290: 0067 007c 005d 077d 0174 00a0 017c 01a1  .g.|.].}.t...|..
-000012a0: 0191 0271 0253 0072 1800 0000 a902 da02  ...q.S.r........
-000012b0: 6e70 da06 6172 676d 6178 a902 da02 2e30  np..argmax.....0
-000012c0: da04 6c69 6e65 7218 0000 0072 1800 0000  ..liner....r....
-000012d0: 7219 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-000012e0: 3ed1 0000 00f3 0200 0000 1600 7a3c 5867  >...........z<Xg
-000012f0: 626f 6f73 744d 6f64 656c 2e61 7574 6f74  boostModel.autot
-00001300: 756e 652e 3c6c 6f63 616c 733e 2e6f 626a  une.<locals>.obj
-00001310: 6563 7469 7665 2e3c 6c6f 6361 6c73 3e2e  ective.<locals>.
-00001320: 3c6c 6973 7463 6f6d 703e e9ff ffff ff29  <listcomp>.....)
-00001330: 0972 3800 0000 da06 6474 7261 696e 722e  .r8.....dtrainr.
-00001340: 0000 0072 2f00 0000 da05 6e66 6f6c 64da  ...r/.....nfold.
-00001350: 0961 735f 7061 6e64 6173 da04 7365 6564  .as_pandas..seed
-00001360: 724e 0000 00da 0773 6875 6666 6c65 7a12  rN.....shufflez.
-00001370: 7465 7374 2d6d 6c6f 676c 6f73 732d 6d65  test-mlogloss-me
-00001380: 616e 2931 7214 0000 00da 0f6d 6f64 656c  an)1r......model
-00001390: 5f6f 626a 6563 7469 7665 da11 6d6f 6465  _objective..mode
-000013a0: 6c5f 6576 616c 5f6d 6574 7269 63da 0f6d  l_eval_metric..m
-000013b0: 6f64 656c 5f76 6572 626f 7369 7479 da07  odel_verbosity..
-000013c0: 6e75 6e69 7175 655a 0b73 7567 6765 7374  nuniqueZ.suggest
-000013d0: 5f69 6e74 da0d 6d61 785f 6465 7074 685f  _int..max_depth_
-000013e0: 6d69 6eda 0d6d 6178 5f64 6570 7468 5f6d  min..max_depth_m
-000013f0: 6178 5a0d 7375 6767 6573 745f 666c 6f61  axZ.suggest_floa
-00001400: 74da 0961 6c70 6861 5f6d 696e da09 616c  t..alpha_min..al
-00001410: 7068 615f 6d61 78da 0a6c 616d 6264 615f  pha_max..lambda_
-00001420: 6d69 6eda 0a6c 616d 6264 615f 6d61 78da  min..lambda_max.
-00001430: 0e6e 756d 5f6c 6561 7665 735f 6d69 6eda  .num_leaves_min.
-00001440: 0e6e 756d 5f6c 6561 7665 735f 6d61 78da  .num_leaves_max.
-00001450: 0e73 7562 5f73 616d 706c 655f 6d69 6eda  .sub_sample_min.
-00001460: 0e73 7562 5f73 616d 706c 655f 6d61 78da  .sub_sample_max.
-00001470: 1663 6f6c 5f73 616d 706c 655f 6279 5f74  .col_sample_by_t
-00001480: 7265 655f 6d69 6eda 1663 6f6c 5f73 616d  ree_min..col_sam
-00001490: 706c 655f 6279 5f74 7265 655f 6d61 78da  ple_by_tree_max.
-000014a0: 1763 6f6c 5f73 616d 706c 655f 6279 5f6c  .col_sample_by_l
-000014b0: 6576 656c 5f6d 696e da17 636f 6c5f 7361  evel_min..col_sa
-000014c0: 6d70 6c65 5f62 795f 6c65 7665 6c5f 6d61  mple_by_level_ma
-000014d0: 78da 1663 6f6c 5f73 616d 706c 655f 6279  x..col_sample_by
-000014e0: 5f6e 6f64 655f 6d69 6eda 1663 6f6c 5f73  _node_min..col_s
-000014f0: 616d 706c 655f 6279 5f6e 6f64 655f 6d61  ample_by_node_ma
-00001500: 78da 156d 696e 5f63 6869 6c64 5f73 616d  x..min_child_sam
-00001510: 706c 6573 5f6d 696e da15 6d69 6e5f 6368  ples_min..min_ch
-00001520: 696c 645f 7361 6d70 6c65 735f 6d61 7872  ild_samples_maxr
-00001530: 4b00 0000 da09 7374 6570 735f 6d69 6eda  K.....steps_min.
-00001540: 0973 7465 7073 5f6d 6178 da15 6e75 6d5f  .steps_max..num_
-00001550: 7061 7261 6c6c 656c 5f74 7265 655f 6d69  parallel_tree_mi
-00001560: 6eda 156e 756d 5f70 6172 616c 6c65 6c5f  n..num_parallel_
-00001570: 7472 6565 5f6d 6178 5a13 7375 6767 6573  tree_maxZ.sugges
-00001580: 745f 6361 7465 676f 7269 6361 6c72 2100  t_categoricalr!.
-00001590: 0000 7236 0000 0072 3700 0000 da06 6f70  ..r6...r7.....op
-000015a0: 7475 6e61 5a0b 696e 7465 6772 6174 696f  tunaZ.integratio
-000015b0: 6e5a 1658 4742 6f6f 7374 5072 756e 696e  nZ.XGBoostPrunin
-000015c0: 6743 616c 6c62 6163 6b72 1300 0000 da14  gCallbackr......
-000015d0: 6879 7065 7274 756e 696e 675f 6376 5f66  hypertuning_cv_f
-000015e0: 6f6c 6473 722b 0000 0072 2f00 0000 da07  oldsr+...r/.....
-000015f0: 7072 6564 6963 7472 5200 0000 da07 6173  predictrR.....as
-00001600: 6172 7261 7972 0700 0000 da02 6376 da13  arrayr......cv..
-00001610: 676c 6f62 616c 5f72 616e 646f 6d5f 7374  global_random_st
-00001620: 6174 65da 1773 6875 6666 6c65 5f64 7572  ate..shuffle_dur
-00001630: 696e 675f 7472 6169 6e69 6e67 da04 6d65  ing_training..me
-00001640: 616e 290c da05 7472 6961 6cda 0570 6172  an)...trial..par
-00001650: 616d 7235 0000 0072 2000 0000 7239 0000  amr5...r ...r9..
-00001660: 005a 1070 7275 6e69 6e67 5f63 616c 6c62  .Z.pruning_callb
-00001670: 6163 6b72 3b00 0000 7216 0000 00da 0570  ackr;...r......p
-00001680: 7265 6473 da0b 7072 6564 5f6c 6162 656c  reds..pred_label
-00001690: 735a 076d 6174 7468 6577 da06 7265 7375  sZ.matthew..resu
-000016a0: 6c74 a906 723a 0000 0072 1700 0000 5a08  lt..r:...r....Z.
-000016b0: 7472 6169 6e5f 6f6e 7223 0000 0072 2600  train_onr#...r&.
-000016c0: 0000 7225 0000 0072 1800 0000 7219 0000  ..r%...r....r...
-000016d0: 0072 3d00 0000 8000 0000 73d8 0000 0002  .r=.......s.....
-000016e0: 0108 0102 ff08 0202 fe08 0302 fd04 0402  ................
-000016f0: fc08 0502 fb06 0602 0106 0106 0102 fd02  ................
-00001700: fa06 0b0e 0102 ff02 f506 0e0e 0102 ff02  ................
-00001710: f206 1102 0106 0106 0102 fd02 ef06 1602  ................
-00001720: 0106 0106 0102 fd02 ea06 1b02 0106 0106  ................
-00001730: 0102 fd02 e506 2002 0106 0106 0102 fd02  ...... .........
-00001740: e006 2502 0106 0106 0102 fd02 db06 2a02  ..%...........*.
-00001750: 0106 0106 0102 fd02 d608 2f02 d106 300e  ........../...0.
-00001760: 0102 ff02 d006 3302 0106 0106 0102 fd04  ......3.........
-00001770: cd10 3904 010a 0112 010e 0206 0204 0104  ..9.............
-00001780: ff0e 0410 0104 0102 0102 0106 0106 0102  ................
-00001790: 0104 0106 0106 f90a 0914 010e 0104 0104  ................
-000017a0: 0202 0102 0106 0106 0106 0102 0106 0104  ................
-000017b0: 0106 0106 f70c 0c7a 2858 6762 6f6f 7374  .......z(Xgboost
-000017c0: 4d6f 6465 6c2e 6175 746f 7475 6e65 2e3c  Model.autotune.<
-000017d0: 6c6f 6361 6c73 3e2e 6f62 6a65 6374 6976  locals>.objectiv
-000017e0: 65da 0778 6762 6f6f 7374 5429 025a 0c6d  e..xgboostT).Z.m
-000017f0: 756c 7469 7661 7269 6174 6572 5d00 0000  ultivariater]...
-00001800: da08 6d69 6e69 6d69 7a65 7a07 2074 756e  ..minimizez. tun
-00001810: 696e 6729 03da 0964 6972 6563 7469 6f6e  ing)...direction
-00001820: da07 7361 6d70 6c65 725a 0a73 7475 6479  ..samplerZ.study
-00001830: 5f6e 616d 6529 04da 086e 5f74 7269 616c  _name)...n_trial
-00001840: 73da 0774 696d 656f 7574 5a0e 6763 5f61  s..timeoutZ.gc_a
-00001850: 6674 6572 5f74 7269 616c 5a11 7368 6f77  fter_trialZ.show
-00001860: 5f70 726f 6772 6573 735f 6261 7272 3d00  _progress_barr=.
-00001870: 0000 723e 0000 0072 3f00 0000 7240 0000  ..r>...r?...r@..
-00001880: 0072 4100 0000 7242 0000 0072 4300 0000  .rA...rB...rC...
-00001890: 7244 0000 0072 4500 0000 7246 0000 0072  rD...rE...rF...r
-000018a0: 4700 0000 7248 0000 0072 4900 0000 724a  G...rH...rI...rJ
-000018b0: 0000 0072 4b00 0000 722d 0000 0072 4c00  ...rK...r-...rL.
-000018c0: 0000 7a0d 4265 7374 2070 6172 616d 733a  ..z.Best params:
-000018d0: 2072 3500 0000 4e29 2272 0d00 0000 7202   r5...N)"r....r.
-000018e0: 0000 0072 1e00 0000 7236 0000 0072 3700  ...r....r6...r7.
-000018f0: 0000 720c 0000 0072 2200 0000 7215 0000  ..r....r"...r...
-00001900: 0072 1300 0000 7214 0000 0072 3100 0000  .r....r....r1...
-00001910: 7279 0000 005a 0873 616d 706c 6572 735a  ry...Z.samplersZ
-00001920: 0a54 5045 5361 6d70 6c65 7272 7e00 0000  .TPESamplerr~...
-00001930: 5a0c 6372 6561 7465 5f73 7475 6479 da08  Z.create_study..
-00001940: 6f70 7469 6d69 7a65 da1c 6879 7065 7270  optimize..hyperp
-00001950: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
-00001960: 726f 756e 6473 da26 6879 7065 7270 6172  rounds.&hyperpar
-00001970: 616d 6574 6572 5f74 756e 696e 675f 6d61  ameter_tuning_ma
-00001980: 785f 7275 6e74 696d 655f 7365 6373 5a0d  x_runtime_secsZ.
-00001990: 7669 7375 616c 697a 6174 696f 6e5a 1970  visualizationZ.p
-000019a0: 6c6f 745f 6f70 7469 6d69 7a61 7469 6f6e  lot_optimization
-000019b0: 5f68 6973 746f 7279 da04 7368 6f77 5a16  _history..showZ.
-000019c0: 706c 6f74 5f70 6172 616d 5f69 6d70 6f72  plot_param_impor
-000019d0: 7461 6e63 6573 da11 5a65 726f 4469 7669  tances..ZeroDivi
-000019e0: 7369 6f6e 4572 726f 72da 0c52 756e 7469  sionError..Runti
-000019f0: 6d65 4572 726f 725a 0a62 6573 745f 7472  meErrorZ.best_tr
-00001a00: 6961 6c72 3800 0000 725f 0000 0072 6000  ialr8...r_...r`.
-00001a10: 0000 7261 0000 0072 6200 0000 724b 0000  ..ra...rb...rK..
-00001a20: 0072 3400 0000 7235 0000 0029 0b72 1700  .r4...r5...).r..
-00001a30: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
-00001a40: 0072 2600 0000 723d 0000 00da 0961 6c67  .r&...r=.....alg
-00001a50: 6f72 6974 686d 728a 0000 005a 0573 7475  orithmr....Z.stu
-00001a60: 6479 da03 6669 675a 1278 6762 6f6f 7374  dy..figZ.xgboost
-00001a70: 5f62 6573 745f 7061 7261 6d72 1800 0000  _best_paramr....
-00001a80: 7286 0000 0072 1900 0000 7233 0000 0066  r....r....r3...f
-00001a90: 0000 0073 9c00 0000 120b 0e01 0601 0802  ...s............
-00001aa0: 0403 02ff 0402 02fe 0403 02fd 0205 0201  ................
-00001ab0: 04ff 1604 0463 0601 0801 06ff 0403 0201  .....c..........
-00001ac0: 0201 0801 06fd 0406 0201 0601 0601 0201  ................
-00001ad0: 0201 06fb 0207 0c01 0801 0c01 0c01 1201  ................
-00001ae0: 0401 02ff 0803 0201 0801 02ff 0802 02fe  ................
-00001af0: 0803 02fd 0404 02fc 0805 02fb 0406 0201  ................
-00001b00: 02ff 02fa 0809 02f7 080a 02f6 080b 02f5  ................
-00001b10: 080c 02f4 080d 02f3 080e 02f2 080f 02f1  ................
-00001b20: 0810 02f0 0811 02ef 0812 02ee 0813 08ed  ................
-00001b30: 0e15 1001 7a15 5867 626f 6f73 744d 6f64  ....z.XgboostMod
-00001b40: 656c 2e61 7574 6f74 756e 65da 0264 6663  el.autotune..dfc
-00001b50: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00001b60: 0400 0000 4300 0000 73a0 0000 0074 0074  ....C...s....t.t
-00001b70: 01a0 02a1 009b 0064 019d 0283 0101 0074  .......d.......t
-00001b80: 0364 0283 0101 0074 04a0 057c 01a1 017d  .d.....t...|...}
-00001b90: 027c 006a 0673 1974 0764 0383 0182 017c  .|.j.s.t.d.....|
-00001ba0: 006a 0873 2074 0764 0483 0182 017c 006a  .j.s t.d.....|.j
-00001bb0: 06a0 097c 02a1 017d 037c 006a 0a64 056b  ...|...}.|.j.d.k
-00001bc0: 0272 3c74 0ba0 0c64 0664 0784 007c 0344  .r<t...d.d...|.D
-00001bd0: 0083 01a1 017d 047c 047c 006a 086a 0d6b  .....}.|.|.j.j.k
-00001be0: 047d 056e 0c7c 037d 0474 0ba0 0c64 0864  .}.n.|.}.t...d.d
-00001bf0: 0784 007c 0344 0083 01a1 017d 0574 0364  ...|.D.....}.t.d
-00001c00: 0983 0101 007c 047c 0566 0253 0029 0a7a  .....|.|.f.S.).z
-00001c10: 1750 7265 6469 6374 206f 6e20 756e 7365  .Predict on unse
-00001c20: 656e 2064 6174 612e 7a33 3a20 5374 6172  en data.z3: Star
-00001c30: 7420 7072 6564 6963 7469 6e67 206f 6e20  t predicting on 
-00001c40: 6e65 7720 6461 7461 2075 7369 6e67 2058  new data using X
-00001c50: 6762 6f6f 7374 206d 6f64 656c 2e7a 1c2b  gboost model.z.+
-00001c60: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
-00001c70: 2b2b 2b2b 2b2b 2b2b 2b2b 2b7a 204e 6f20  +++++++++++z No 
-00001c80: 7472 6169 6e65 6420 6d6f 6465 6c20 6861  trained model ha
-00001c90: 7320 6265 656e 2066 6f75 6e64 2e7a 2b4e  s been found.z+N
-00001ca0: 6f20 6d6f 6465 6c20 636f 6e66 6967 7572  o model configur
-00001cb0: 6174 696f 6e20 6669 6c65 2068 6173 2062  ation file has b
-00001cc0: 6565 6e20 666f 756e 642e 7211 0000 0063  een found.r....c
-00001cd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001ce0: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00001cf0: 005d 067d 017c 0164 0019 0091 0271 0253  .].}.|.d.....q.S
-00001d00: 0029 0172 4d00 0000 7218 0000 0072 5400  .).rM...r....rT.
-00001d10: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00001d20: 0072 5700 0000 2401 0000 7302 0000 0014  .rW...$...s.....
-00001d30: 007a 2858 6762 6f6f 7374 4d6f 6465 6c2e  .z(XgboostModel.
-00001d40: 7072 6564 6963 742e 3c6c 6f63 616c 733e  predict.<locals>
-00001d50: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
-00001d60: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00001d70: 5300 0000 7250 0000 0072 1800 0000 7251  S...rP...r....rQ
-00001d80: 0000 0072 5400 0000 7218 0000 0072 1800  ...rT...r....r..
-00001d90: 0000 7219 0000 0072 5700 0000 2a01 0000  ..r....rW...*...
-00001da0: 7258 0000 007a 1346 696e 6973 6865 6420  rX...z.Finished 
-00001db0: 7072 6564 6963 7469 6e67 290e 720d 0000  predicting).r...
-00001dc0: 0072 0200 0000 721e 0000 0072 3400 0000  .r....r....r4...
-00001dd0: 7236 0000 0072 3700 0000 7216 0000 00da  r6...r7...r.....
-00001de0: 0945 7863 6570 7469 6f6e 7215 0000 0072  .Exceptionr....r
-00001df0: 7b00 0000 7210 0000 0072 5200 0000 727c  {...r....rR...r|
-00001e00: 0000 00da 1863 6c61 7373 6966 6963 6174  .....classificat
-00001e10: 696f 6e5f 7468 7265 7368 6f6c 6429 0672  ion_threshold).r
-00001e20: 1700 0000 7295 0000 0072 3a00 0000 5a0d  ....r....r:...Z.
-00001e30: 7061 7274 6961 6c5f 7072 6f62 735a 0f70  partial_probsZ.p
-00001e40: 7265 6469 6374 6564 5f70 726f 6273 5a11  redicted_probsZ.
-00001e50: 7072 6564 6963 7465 645f 636c 6173 7365  predicted_classe
-00001e60: 7372 1800 0000 7218 0000 0072 1900 0000  sr....r....r....
-00001e70: 727b 0000 0015 0100 0073 2400 0000 0202  r{.......s$.....
-00001e80: 0c01 04ff 0803 0a01 0601 0801 0602 0801  ................
-00001e90: 0c02 0a01 1401 0a02 04ff 0404 1401 0801  ................
-00001ea0: 0801 7a14 5867 626f 6f73 744d 6f64 656c  ..z.XgboostModel
-00001eb0: 2e70 7265 6469 6374 2903 4e4e 4e29 1ada  .predict).NNN)..
-00001ec0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00001ed0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00001ee0: 655f 5fda 075f 5f64 6f63 5f5f 7204 0000  e__..__doc__r...
-00001ef0: 0072 0500 0000 7209 0000 0072 0b00 0000  .r....r....r....
-00001f00: 720a 0000 0072 1a00 0000 da02 7064 da06  r....r......pd..
-00001f10: 5365 7269 6573 7203 0000 00da 0373 7472  Seriesr......str
-00001f20: da05 666c 6f61 7472 2100 0000 7222 0000  ..floatr!...r"..
-00001f30: 00da 0944 6174 6146 7261 6d65 7236 0000  ...DataFramer6..
-00001f40: 00da 0742 6f6f 7374 6572 723c 0000 0072  ...Boosterr<...r
-00001f50: 3300 0000 7206 0000 0072 5200 0000 da07  3...r....rR.....
-00001f60: 6e64 6172 7261 7972 7b00 0000 7218 0000  ndarrayr{...r...
-00001f70: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001f80: 720f 0000 001a 0000 0073 5000 0000 0800  r........sP.....
-00001f90: 0401 0205 0201 0201 04fb 0602 02fe 0603  ................
-00001fa0: 02fd 0604 02fc 0605 0afb 1c0d 0808 020f  ................
-00001fb0: 0402 02fe 0403 02fd 0404 02fc 0405 02fb  ................
-00001fc0: 0406 0afa 0225 0402 02fe 0403 02fd 0404  .....%..........
-00001fd0: 02fc 0405 02fb 0206 0afa 007f 2430 720f  ............$0r.
-00001fe0: 0000 0029 1c72 9b00 0000 7202 0000 00da  ...).r....r.....
-00001ff0: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
-00002000: 0072 0500 0000 7206 0000 00da 056e 756d  .r....r......num
-00002010: 7079 7252 0000 0072 7900 0000 da06 7061  pyrR...ry.....pa
-00002020: 6e64 6173 729c 0000 0072 8700 0000 7236  ndasr....r....r6
-00002030: 0000 00da 0f73 6b6c 6561 726e 2e6d 6574  .....sklearn.met
-00002040: 7269 6373 7207 0000 00da 0d73 6b6c 6561  ricsr......sklea
-00002050: 726e 2e75 7469 6c73 7208 0000 00da 1f62  rn.utilsr......b
-00002060: 6c75 6563 6173 742e 636f 6e66 6967 2e74  luecast.config.t
-00002070: 7261 696e 696e 675f 636f 6e66 6967 7209  raining_configr.
-00002080: 0000 0072 0a00 0000 720b 0000 00da 2462  ...r....r.....$b
-00002090: 6c75 6563 6173 742e 6765 6e65 7261 6c5f  luecast.general_
-000020a0: 7574 696c 732e 6765 6e65 7261 6c5f 7574  utils.general_ut
-000020b0: 696c 7372 0c00 0000 720d 0000 005a 2262  ilsr....r....Z"b
-000020c0: 6c75 6563 6173 742e 6d6c 5f6d 6f64 656c  luecast.ml_model
-000020d0: 6c69 6e67 2e62 6173 655f 636c 6173 7365  ling.base_classe
-000020e0: 7372 0e00 0000 720f 0000 0072 1800 0000  sr....r....r....
-000020f0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00002100: 083c 6d6f 6475 6c65 3e01 0000 0073 1a00  .<module>....s..
-00002110: 0000 0400 0c06 1801 0802 0801 0801 0801  ................
-00002120: 0c01 0c01 1402 1005 0c01 1403            ............
+000004c0: 0000 7215 0000 00a9 0072 1800 0000 fa43  ..r......r.....C
+000004d0: 2f68 6f6d 652f 7468 6f6d 6173 2f49 6465  /home/thomas/Ide
+000004e0: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
+000004f0: 7374 2f62 6c75 6563 6173 742f 6d6c 5f6d  st/bluecast/ml_m
+00000500: 6f64 656c 6c69 6e67 2f78 6762 6f6f 7374  odelling/xgboost
+00000510: 2e70 79da 085f 5f69 6e69 745f 5f1d 0000  .py..__init__...
+00000520: 0073 0a00 0000 0607 0601 0601 0601 0a01  .s..............
+00000530: 7a15 5867 626f 6f73 744d 6f64 656c 2e5f  z.XgboostModel._
+00000540: 5f69 6e69 745f 5fda 0179 da06 7265 7475  _init__..y..retu
+00000550: 726e 6302 0000 0000 0000 0000 0000 0003  rnc.............
+00000560: 0000 0004 0000 0043 0000 0073 2400 0000  .......C...s$...
+00000570: 7400 7401 a002 a100 9b00 6401 9d02 8301  t.t.......d.....
+00000580: 0100 7403 6a04 6402 7c01 6403 8d02 7d02  ..t.j.d.|.d...}.
+00000590: 7c02 5300 2904 7a29 4361 6c63 756c 6174  |.S.).z)Calculat
+000005a0: 6520 636c 6173 7320 7765 6967 6874 7320  e class weights 
+000005b0: 6f66 2074 6172 6765 7420 636f 6c75 6d6e  of target column
+000005c0: 2e7a 293a 2053 7461 7274 2063 616c 6375  .z): Start calcu
+000005d0: 6c61 7469 6e67 2074 6172 6765 7420 636c  lating target cl
+000005e0: 6173 7320 7765 6967 6874 732e da08 6261  ass weights...ba
+000005f0: 6c61 6e63 6564 2902 7208 0000 0072 1b00  lanced).r....r..
+00000600: 0000 2905 720d 0000 0072 0200 0000 da06  ..).r....r......
+00000610: 7574 636e 6f77 7208 0000 00da 1563 6f6d  utcnowr......com
+00000620: 7075 7465 5f73 616d 706c 655f 7765 6967  pute_sample_weig
+00000630: 6874 2903 7217 0000 0072 1b00 0000 da0f  ht).r....r......
+00000640: 636c 6173 7365 735f 7765 6967 6874 7372  classes_weightsr
+00000650: 1800 0000 7218 0000 0072 1900 0000 da17  ....r....r......
+00000660: 6361 6c63 756c 6174 655f 636c 6173 735f  calculate_class_
+00000670: 7765 6967 6874 732a 0000 0073 0a00 0000  weights*...s....
+00000680: 1202 0401 0401 06ff 0403 7a24 5867 626f  ..........z$Xgbo
+00000690: 6f73 744d 6f64 656c 2e63 616c 6375 6c61  ostModel.calcula
+000006a0: 7465 5f63 6c61 7373 5f77 6569 6768 7473  te_class_weights
+000006b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000006c0: 0003 0000 0043 0000 0073 b400 0000 7400  .....C...s....t.
+000006d0: 7401 a002 a100 9b00 6401 9d02 8301 0100  t.......d.......
+000006e0: 7c00 6a03 731a 7404 8300 7c00 5f03 7400  |.j.s.t...|._.t.
+000006f0: 7401 a002 a100 9b00 6402 9d02 8301 0100  t.......d.......
+00000700: 6e09 7400 7401 a002 a100 9b00 6403 9d02  n.t.t.......d...
+00000710: 8301 0100 7c00 6a05 7334 7406 8300 7c00  ....|.j.s4t...|.
+00000720: 5f05 7400 7401 a002 a100 9b00 6404 9d02  _.t.t.......d...
+00000730: 8301 0100 6e09 7400 7401 a002 a100 9b00  ....n.t.t.......
+00000740: 6405 9d02 8301 0100 7c00 6a07 734f 7408  d.......|.j.sOt.
+00000750: 8300 7c00 5f07 7400 7401 a002 a100 9b00  ..|._.t.t.......
+00000760: 6406 9d02 8301 0100 6408 5300 7400 7401  d.......d.S.t.t.
+00000770: a002 a100 9b00 6407 9d02 8301 0100 6408  ......d.......d.
+00000780: 5300 2909 7a36 4c6f 6164 206d 756c 7469  S.).z6Load multi
+00000790: 706c 6520 636f 6e66 6967 7320 6f72 206c  ple configs or l
+000007a0: 6f61 6420 6465 6661 756c 7420 636f 6e66  oad default conf
+000007b0: 6967 7320 696e 7374 6561 642e 7a32 3a20  igs instead.z2: 
+000007c0: 5374 6172 7420 6c6f 6164 696e 6720 6578  Start loading ex
+000007d0: 6973 7469 6e67 206f 7220 6465 6661 756c  isting or defaul
+000007e0: 7420 636f 6e66 6967 2066 696c 6573 2e2e  t config files..
+000007f0: 7a1e 3a20 4c6f 6164 2064 6566 6175 6c74  z.: Load default
+00000800: 2054 7261 696e 696e 6743 6f6e 6669 672e   TrainingConfig.
+00000810: 7a20 3a20 466f 756e 6420 7072 6f76 6964  z : Found provid
+00000820: 6564 2054 7261 696e 696e 6743 6f6e 6669  ed TrainingConfi
+00000830: 672e 7a27 3a20 4c6f 6164 2064 6566 6175  g.z': Load defau
+00000840: 6c74 2058 6762 6f6f 7374 5475 6e65 5061  lt XgboostTunePa
+00000850: 7261 6d73 436f 6e66 6967 2e7a 293a 2046  ramsConfig.z): F
+00000860: 6f75 6e64 2070 726f 7669 6465 6420 5867  ound provided Xg
+00000870: 626f 6f73 7454 756e 6550 6172 616d 7343  boostTuneParamsC
+00000880: 6f6e 6669 672e 7a27 3a20 4c6f 6164 2064  onfig.z': Load d
+00000890: 6566 6175 6c74 2058 6762 6f6f 7374 4669  efault XgboostFi
+000008a0: 6e61 6c50 6172 616d 436f 6e66 6967 2e7a  nalParamConfig.z
+000008b0: 293a 2046 6f75 6e64 2070 726f 7669 6465  ): Found provide
+000008c0: 6420 5867 626f 6f73 7446 696e 616c 5061  d XgboostFinalPa
+000008d0: 7261 6d43 6f6e 6669 672e 4e29 0972 0d00  ramConfig.N).r..
+000008e0: 0000 7202 0000 0072 1e00 0000 7213 0000  ..r....r....r...
+000008f0: 0072 0900 0000 7214 0000 0072 0b00 0000  .r....r....r....
+00000900: 7215 0000 0072 0a00 0000 2901 7217 0000  r....r....).r...
+00000910: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000920: da10 6368 6563 6b5f 6c6f 6164 5f63 6f6e  ..check_load_con
+00000930: 6673 3200 0000 731a 0000 0012 0206 0108  fs2...s.........
+00000940: 0114 0112 0206 0208 0114 0112 0206 0208  ................
+00000950: 0116 0116 027a 1d58 6762 6f6f 7374 4d6f  .....z.XgboostMo
+00000960: 6465 6c2e 6368 6563 6b5f 6c6f 6164 5f63  del.check_load_c
+00000970: 6f6e 6673 da07 785f 7472 6169 6eda 0678  onfs..x_train..x
+00000980: 5f74 6573 74da 0779 5f74 7261 696e da06  _test..y_train..
+00000990: 795f 7465 7374 6305 0000 0000 0000 0000  y_testc.........
+000009a0: 0000 0009 0000 0007 0000 0043 0000 0073  ...........C...s
+000009b0: 4a01 0000 7400 7401 a002 a100 9b00 6401  J...t.t.......d.
+000009c0: 9d02 8301 0100 7c00 a003 a100 0100 7c00  ......|.......|.
+000009d0: 6a04 7213 7c00 6a05 7317 7406 6402 8301  j.r.|.j.s.t.d...
+000009e0: 8201 7c00 6a05 6a07 7223 7c00 a008 7c01  ..|.j.j.r#|...|.
+000009f0: 7c02 7c03 7c04 a104 0100 7409 6403 8301  |.|.|.....t.d...
+00000a00: 0100 7409 6404 8301 0100 7c00 6a05 6a0a  ..t.d.....|.j.j.
+00000a10: 7246 7400 7401 a002 a100 9b00 6405 9d02  rFt.t.......d...
+00000a20: 8301 0100 740b a00c 7c01 7c02 6702 a101  ....t...|.|.g...
+00000a30: 7d01 740b a00c 7c03 7c04 6702 a101 7d03  }.t...|.|.g...}.
+00000a40: 7c00 6a04 6a0d 7258 7c00 a00e 7c03 a101  |.j.j.rX|...|...
+00000a50: 7d05 740f 6a10 7c01 7c03 7c05 6406 8d03  }.t.j.|.|.|.d...
+00000a60: 7d06 6e07 740f 6a10 7c01 7c03 6407 8d02  }.n.t.j.|.|.d...
+00000a70: 7d06 740f 6a10 7c02 7c04 6407 8d02 7d07  }.t.j.|.|.d...}.
+00000a80: 7c06 6408 6602 7c07 6409 6602 6702 7d08  |.d.f.|.d.f.g.}.
+00000a90: 7c00 6a05 6a11 640a 6b02 7288 740f 6a12  |.j.j.d.k.r.t.j.
+00000aa0: 7c00 6a04 6a13 7c06 7c00 6a04 6a13 640b  |.j.j.|.|.j.j.d.
+00000ab0: 1900 7c00 6a05 6a14 7c08 640c 8d05 7c00  ..|.j.j.|.d...|.
+00000ac0: 5f15 6e16 740f 6a12 7c00 6a04 6a13 7c06  _.n.t.j.|.j.j.|.
+00000ad0: 7c00 6a04 6a13 640b 1900 7c06 6408 6602  |.j.j.d...|.d.f.
+00000ae0: 7c07 6409 6602 6702 640d 8d04 7c00 5f15  |.d.f.g.d...|._.
+00000af0: 7409 640e 8301 0100 7c00 6a15 5300 290f  t.d.....|.j.S.).
+00000b00: 7a3f 5472 6169 6e20 5867 626f 6f73 7420  z?Train Xgboost 
+00000b10: 6d6f 6465 6c2e 2049 6e63 6c75 6465 7320  model. Includes 
+00000b20: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
+00000b30: 756e 696e 6720 6f6e 2064 6566 6175 6c74  uning on default
+00000b40: 2e7a 1e3a 2053 7461 7274 2066 6974 7469  .z.: Start fitti
+00000b50: 6e67 2058 6762 6f6f 7374 206d 6f64 656c  ng Xgboost model
+00000b60: 2e7a 2c63 6f6e 665f 7061 7261 6d73 5f78  .z,conf_params_x
+00000b70: 6762 6f6f 7374 206f 7220 636f 6e66 5f74  gboost or conf_t
+00000b80: 7261 696e 696e 6720 6973 204e 6f6e 657a  raining is Nonez
+00000b90: 1e46 696e 6973 6865 6420 6879 7065 7270  .Finished hyperp
+00000ba0: 6172 616d 6574 6572 2074 756e 696e 677a  arameter tuningz
+00000bb0: 0e53 7461 7274 2074 7261 696e 696e 677a  .Start trainingz
+00000bc0: 7f3a 2055 6e69 6f6e 2074 7261 696e 2061  .: Union train a
+00000bd0: 6e64 2074 6573 7420 6461 7461 2066 6f72  nd test data for
+00000be0: 2066 696e 616c 206d 6f64 656c 2074 7261   final model tra
+00000bf0: 696e 696e 6720 6261 7365 6420 6f6e 2054  ining based on T
+00000c00: 7261 696e 696e 6743 6f6e 6669 670a 2020  rainingConfig.  
+00000c10: 2020 2020 2020 2020 2020 2070 6172 616d             param
+00000c20: 2027 7573 655f 6675 6c6c 5f64 6174 615f   'use_full_data_
+00000c30: 666f 725f 6669 6e61 6c5f 6d6f 6465 6c27  for_final_model'
+00000c40: a902 da05 6c61 6265 6cda 0677 6569 6768  ....label..weigh
+00000c50: 74a9 0172 2800 0000 da05 7472 6169 6eda  t..r(.....train.
+00000c60: 0474 6573 74e9 0100 0000 da05 7374 6570  .test.......step
+00000c70: 7329 03da 0f6e 756d 5f62 6f6f 7374 5f72  s)...num_boost_r
+00000c80: 6f75 6e64 da15 6561 726c 795f 7374 6f70  ound..early_stop
+00000c90: 7069 6e67 5f72 6f75 6e64 73da 0565 7661  ping_rounds..eva
+00000ca0: 6c73 2902 722f 0000 00da 0865 7661 6c5f  ls).r/.....eval_
+00000cb0: 7365 747a 1146 696e 6973 6865 6420 7472  setz.Finished tr
+00000cc0: 6169 6e69 6e67 2916 720d 0000 0072 0200  aining).r....r..
+00000cd0: 0000 721e 0000 0072 2200 0000 7215 0000  ..r....r"...r...
+00000ce0: 0072 1300 0000 da0a 5661 6c75 6545 7272  .r......ValueErr
+00000cf0: 6f72 da0e 6175 746f 7475 6e65 5f6d 6f64  or..autotune_mod
+00000d00: 656c da08 6175 746f 7475 6e65 da05 7072  el..autotune..pr
+00000d10: 696e 74da 1d75 7365 5f66 756c 6c5f 6461  int..use_full_da
+00000d20: 7461 5f66 6f72 5f66 696e 616c 5f6d 6f64  ta_for_final_mod
+00000d30: 656c da02 7064 da06 636f 6e63 6174 da0d  el..pd..concat..
+00000d40: 7361 6d70 6c65 5f77 6569 6768 7472 2100  sample_weightr!.
+00000d50: 0000 da03 7867 62da 0744 4d61 7472 6978  ....xgb..DMatrix
+00000d60: da14 6879 7065 7274 756e 696e 675f 6376  ..hypertuning_cv
+00000d70: 5f66 6f6c 6473 722b 0000 00da 0670 6172  _foldsr+.....par
+00000d80: 616d 7372 3000 0000 7216 0000 0029 0972  amsr0...r....).r
+00000d90: 1700 0000 7223 0000 0072 2400 0000 7225  ....r#...r$...r%
+00000da0: 0000 0072 2600 0000 7220 0000 00da 0764  ...r&...r .....d
+00000db0: 5f74 7261 696e da06 645f 7465 7374 7232  _train..d_testr2
+00000dc0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00000dd0: 0000 da03 6669 7447 0000 0073 4800 0000  ....fitG...sH...
+00000de0: 1208 0801 0c02 0801 0802 1001 0802 0802  ................
+00000df0: 0801 0201 0c01 04ff 0e04 0e01 0802 0a01  ................
+00000e00: 1201 0e02 0e02 1001 0c02 0401 0601 0201  ................
+00000e10: 0a01 0601 0201 0afb 0408 0601 0201 0a01  ................
+00000e20: 0e01 08fc 0806 0601 7a10 5867 626f 6f73  ........z.Xgboos
+00000e30: 744d 6f64 656c 2e66 6974 6305 0000 0000  tModel.fitc.....
+00000e40: 0000 0000 0000 000b 0000 000a 0000 0003  ................
+00000e50: 0000 0073 c201 0000 7400 7401 a002 a100  ...s....t.t.....
+00000e60: 9b00 6401 9d02 8301 0100 7403 6a04 7c02  ..d.......t.j.|.
+00000e70: 8804 6402 8d02 8900 7405 8300 8902 8801  ..d.....t.......
+00000e80: a006 a100 0100 8801 6a07 7220 8801 6a08  ........j.r ..j.
+00000e90: 7220 8801 6a09 7324 740a 6403 8301 8201  r ..j.s$t.d.....
+00000ea0: 8700 8701 8702 8703 8704 8705 6606 6404  ............f.d.
+00000eb0: 6405 8408 7d05 6406 7d06 740b 6a0c 6a0d  d...}.d.}.t.j.j.
+00000ec0: 6407 8801 6a08 6a0e 6408 8d02 7d07 740b  d...j.j.d...}.t.
+00000ed0: 6a0f 6409 7c07 7c06 9b00 640a 9d02 640b  j.d.|.|...d...d.
+00000ee0: 8d03 7d08 7c08 6a10 7c05 8801 6a08 6a11  ..}.|.j.|...j.j.
+00000ef0: 8801 6a08 6a12 6407 6407 640c 8d05 0100  ..j.j.d.d.d.....
+00000f00: 7a16 740b 6a13 a014 7c08 a101 7d09 7c09  z.t.j...|...}.|.
+00000f10: a015 a100 0100 740b 6a13 a016 7c08 a101  ......t.j...|...
+00000f20: 7d09 7c09 a015 a100 0100 5700 6e0c 0400  }.|.......W.n...
+00000f30: 7417 7418 740a 6603 7976 0100 0100 0100  t.t.t.f.yv......
+00000f40: 5900 6e01 7700 7c08 6a19 6a1a 7d0a 6900  Y.n.w.|.j.j.}.i.
+00000f50: 640d 8801 6a09 6a1b 9301 640e 8801 6a09  d...j.j...d...j.
+00000f60: 6a1c 9301 640f 8801 6a09 6a1d 9301 6410  j...d...j.j...d.
+00000f70: 8802 9301 6411 8805 a01e a100 9301 6412  ....d.........d.
+00000f80: 7c0a 6412 1900 9301 6413 7c0a 6413 1900  |.d.....d.|.d...
+00000f90: 9301 6414 7c0a 6414 1900 9301 6415 7c0a  ..d.|.d.....d.|.
+00000fa0: 6415 1900 9301 6416 7c0a 6416 1900 9301  d.....d.|.d.....
+00000fb0: 6417 7c0a 6417 1900 9301 6418 7c0a 6418  d.|.d.....d.|.d.
+00000fc0: 1900 9301 6419 7c0a 6419 1900 9301 641a  ....d.|.d.....d.
+00000fd0: 7c0a 641a 1900 9301 641b 8801 6a09 6a1f  |.d.....d...j.j.
+00000fe0: 9301 641c 7c0a 641c 1900 9301 641d 7c0a  ..d.|.d.....d.|.
+00000ff0: 641d 1900 9301 8801 6a07 5f1a 7420 641e  d.......j._.t d.
+00001000: 8801 6a07 6a1a 8302 0100 7c0a 641f 1900  ..j.j.....|.d...
+00001010: 8801 6a07 5f21 6420 5300 2921 7a7b 5475  ..j._!d S.)!z{Tu
+00001020: 6e65 2068 7970 6572 7061 7261 6d65 7465  ne hyperparamete
+00001030: 7273 2e0a 0a20 2020 2020 2020 2041 6e20  rs...        An 
+00001040: 616c 7465 726e 6174 6976 6520 636f 6e66  alternative conf
+00001050: 6967 2063 616e 2062 6520 7072 6f76 6964  ig can be provid
+00001060: 6564 2074 6f20 6f76 6572 7772 6974 6520  ed to overwrite 
+00001070: 7468 6520 6879 7065 7270 6172 616d 6574  the hyperparamet
+00001080: 6572 2073 6561 7263 6820 7370 6163 652e  er search space.
+00001090: 0a20 2020 2020 2020 207a 2f3a 2053 7461  .        z/: Sta
+000010a0: 7274 2068 7970 6572 7061 7261 6d65 7465  rt hyperparamete
+000010b0: 7220 7475 6e69 6e67 206f 6620 5867 626f  r tuning of Xgbo
+000010c0: 6f73 7420 6d6f 6465 6c2e 722a 0000 007a  ost model.r*...z
+000010d0: 3941 7420 6c65 6173 7420 6f6e 6520 6f66  9At least one of
+000010e0: 2074 6865 2063 6f6e 6669 6773 2069 7320   the configs is 
+000010f0: 4e6f 6e65 2c20 7768 6963 6820 6973 206e  None, which is n
+00001100: 6f74 2061 6c6c 6f77 6564 6301 0000 0000  ot allowedc.....
+00001110: 0000 0000 0000 000c 0000 000a 0000 0013  ................
+00001120: 0000 0073 3c02 0000 6900 6401 8801 6a00  ...s<...i.d...j.
+00001130: 6a01 9301 6402 8801 6a00 6a02 9301 6403  j...d...j.j...d.
+00001140: 8801 6a00 6a03 9301 6404 8802 9301 6405  ..j.j...d.....d.
+00001150: 8805 a004 a100 9301 6406 7c00 a005 6406  ........d.|...d.
+00001160: 8801 6a00 6a06 8801 6a00 6a07 a103 9301  ..j.j...j.j.....
+00001170: 6407 7c00 a008 6407 8801 6a00 6a09 8801  d.|...d...j.j...
+00001180: 6a00 6a0a a103 9301 6408 7c00 a008 6408  j.j.....d.|...d.
+00001190: 8801 6a00 6a0b 8801 6a00 6a0c a103 9301  ..j.j...j.j.....
+000011a0: 6409 7c00 a005 6409 8801 6a00 6a0d 8801  d.|...d...j.j...
+000011b0: 6a00 6a0e a103 9301 640a 7c00 a008 640a  j.j.....d.|...d.
+000011c0: 8801 6a00 6a0f 8801 6a00 6a10 a103 9301  ..j.j...j.j.....
+000011d0: 640b 7c00 a008 640b 8801 6a00 6a11 8801  d.|...d...j.j...
+000011e0: 6a00 6a12 a103 9301 640c 7c00 a008 640c  j.j.....d.|...d.
+000011f0: 8801 6a00 6a13 8801 6a00 6a14 a103 9301  ..j.j...j.j.....
+00001200: 640d 7c00 a008 640d 8801 6a00 6a15 8801  d.|...d...j.j...
+00001210: 6a00 6a16 a103 9301 640e 7c00 a005 640e  j.j.....d.|...d.
+00001220: 8801 6a00 6a17 8801 6a00 6a18 a103 9301  ..j.j...j.j.....
+00001230: 640f 8801 6a00 6a19 9301 6410 7c00 a005  d...j.j...d.|...
+00001240: 6410 8801 6a00 6a1a 8801 6a00 6a1b a103  d...j.j...j.j...
+00001250: 9301 6411 7c00 a005 6411 8801 6a00 6a1c  ..d.|...d...j.j.
+00001260: 8801 6a00 6a1d a103 9301 7d01 7c00 a01e  ..j.j.....}.|...
+00001270: 6412 6413 6414 6702 a102 7d02 7c02 72ba  d.d.d.g...}.|.r.
+00001280: 8801 a01f 8805 a101 7d03 7420 6a21 8803  ........}.t j!..
+00001290: 8805 7c03 6415 8d03 7d04 6e07 7420 6a21  ..|.d...}.n.t j!
+000012a0: 8803 8805 6416 8d02 7d04 7422 6a23 a024  ....d...}.t"j#.$
+000012b0: 7c00 6417 a102 7d05 8801 6a25 6a26 6418  |.d...}...j%j&d.
+000012c0: 6b02 9001 7202 7c04 6419 6602 8800 641a  k...r.|.d.f...d.
+000012d0: 6602 6702 7d06 7420 6a27 7c01 7c04 7c01  f.g.}.t j'|.|.|.
+000012e0: 6410 1900 8801 6a25 6a28 7c06 7c05 6701  d.....j%j(|.|.g.
+000012f0: 8801 6a00 6a03 641b 8d07 7d07 7c07 a029  ..j.j.d...}.|..)
+00001300: 8800 a101 7d08 742a a02b 641c 641d 8400  ....}.t*.+d.d...
+00001310: 7c08 4400 8301 a101 7d09 742c 8804 7c09  |.D.....}.t,..|.
+00001320: 8302 641e 1400 7d0a 7c0a 5300 7420 6a2d  ..d...}.|.S.t j-
+00001330: 7c01 7c04 7c01 6410 1900 8801 6a25 6a26  |.|.|.d.....j%j&
+00001340: 6413 8801 6a25 6a2e 7c05 6701 8801 6a25  d...j%j.|.g...j%
+00001350: 6a2f 641f 8d08 7d0b 7c0b 6420 1900 a030  j/d...}.|.d ...0
+00001360: a100 5300 2921 4eda 096f 626a 6563 7469  ..S.)!N..objecti
+00001370: 7665 da0b 6576 616c 5f6d 6574 7269 63da  ve..eval_metric.
+00001380: 0776 6572 626f 7365 da0b 7472 6565 5f6d  .verbose..tree_m
+00001390: 6574 686f 64da 096e 756d 5f63 6c61 7373  ethod..num_class
+000013a0: da09 6d61 785f 6465 7074 68da 0561 6c70  ..max_depth..alp
+000013b0: 6861 da06 6c61 6d62 6461 da0a 6e75 6d5f  ha..lambda..num_
+000013c0: 6c65 6176 6573 da09 7375 6273 616d 706c  leaves..subsampl
+000013d0: 65da 1063 6f6c 7361 6d70 6c65 5f62 7974  e..colsample_byt
+000013e0: 7265 65da 1163 6f6c 7361 6d70 6c65 5f62  ree..colsample_b
+000013f0: 796c 6576 656c da10 636f 6c73 616d 706c  ylevel..colsampl
+00001400: 655f 6279 6e6f 6465 da11 6d69 6e5f 6368  e_bynode..min_ch
+00001410: 696c 645f 7361 6d70 6c65 73da 0365 7461  ild_samples..eta
+00001420: 722e 0000 00da 116e 756d 5f70 6172 616c  r......num_paral
+00001430: 6c65 6c5f 7472 6565 723a 0000 0054 4672  lel_treer:...TFr
+00001440: 2700 0000 722a 0000 007a 0d74 6573 742d  '...r*...z.test-
+00001450: 6d6c 6f67 6c6f 7373 722d 0000 0072 2b00  mloglossr-...r+.
+00001460: 0000 722c 0000 0029 0572 2f00 0000 7230  ..r,...).r/...r0
+00001470: 0000 0072 3100 0000 da09 6361 6c6c 6261  ...r1.....callba
+00001480: 636b 73da 0c76 6572 626f 7365 5f65 7661  cks..verbose_eva
+00001490: 6c63 0100 0000 0000 0000 0000 0000 0200  lc..............
+000014a0: 0000 0500 0000 5300 0000 f316 0000 0067  ......S........g
+000014b0: 007c 005d 077d 0174 00a0 017c 01a1 0191  .|.].}.t...|....
+000014c0: 0271 0253 0072 1800 0000 a902 da02 6e70  .q.S.r........np
+000014d0: da06 6172 676d 6178 a902 da02 2e30 da04  ..argmax.....0..
+000014e0: 6c69 6e65 7218 0000 0072 1800 0000 7219  liner....r....r.
+000014f0: 0000 00da 0a3c 6c69 7374 636f 6d70 3ee9  .....<listcomp>.
+00001500: 0000 00f3 0200 0000 1600 7a3c 5867 626f  ..........z<Xgbo
+00001510: 6f73 744d 6f64 656c 2e61 7574 6f74 756e  ostModel.autotun
+00001520: 652e 3c6c 6f63 616c 733e 2e6f 626a 6563  e.<locals>.objec
+00001530: 7469 7665 2e3c 6c6f 6361 6c73 3e2e 3c6c  tive.<locals>.<l
+00001540: 6973 7463 6f6d 703e e9ff ffff ff29 0872  istcomp>.....).r
+00001550: 3e00 0000 da06 6474 7261 696e 722f 0000  >.....dtrainr/..
+00001560: 00da 056e 666f 6c64 da09 6173 5f70 616e  ...nfold..as_pan
+00001570: 6461 73da 0473 6565 6472 5200 0000 da07  das..seedrR.....
+00001580: 7368 7566 666c 657a 1274 6573 742d 6d6c  shufflez.test-ml
+00001590: 6f67 6c6f 7373 2d6d 6561 6e29 3172 1400  ogloss-mean)1r..
+000015a0: 0000 da0f 6d6f 6465 6c5f 6f62 6a65 6374  ....model_object
+000015b0: 6976 65da 116d 6f64 656c 5f65 7661 6c5f  ive..model_eval_
+000015c0: 6d65 7472 6963 da0f 6d6f 6465 6c5f 7665  metric..model_ve
+000015d0: 7262 6f73 6974 79da 076e 756e 6971 7565  rbosity..nunique
+000015e0: 5a0b 7375 6767 6573 745f 696e 74da 0d6d  Z.suggest_int..m
+000015f0: 6178 5f64 6570 7468 5f6d 696e da0d 6d61  ax_depth_min..ma
+00001600: 785f 6465 7074 685f 6d61 785a 0d73 7567  x_depth_maxZ.sug
+00001610: 6765 7374 5f66 6c6f 6174 da09 616c 7068  gest_float..alph
+00001620: 615f 6d69 6eda 0961 6c70 6861 5f6d 6178  a_min..alpha_max
+00001630: da0a 6c61 6d62 6461 5f6d 696e da0a 6c61  ..lambda_min..la
+00001640: 6d62 6461 5f6d 6178 da0e 6e75 6d5f 6c65  mbda_max..num_le
+00001650: 6176 6573 5f6d 696e da0e 6e75 6d5f 6c65  aves_min..num_le
+00001660: 6176 6573 5f6d 6178 da0e 7375 625f 7361  aves_max..sub_sa
+00001670: 6d70 6c65 5f6d 696e da0e 7375 625f 7361  mple_min..sub_sa
+00001680: 6d70 6c65 5f6d 6178 da16 636f 6c5f 7361  mple_max..col_sa
+00001690: 6d70 6c65 5f62 795f 7472 6565 5f6d 696e  mple_by_tree_min
+000016a0: da16 636f 6c5f 7361 6d70 6c65 5f62 795f  ..col_sample_by_
+000016b0: 7472 6565 5f6d 6178 da17 636f 6c5f 7361  tree_max..col_sa
+000016c0: 6d70 6c65 5f62 795f 6c65 7665 6c5f 6d69  mple_by_level_mi
+000016d0: 6eda 1763 6f6c 5f73 616d 706c 655f 6279  n..col_sample_by
+000016e0: 5f6c 6576 656c 5f6d 6178 da16 636f 6c5f  _level_max..col_
+000016f0: 7361 6d70 6c65 5f62 795f 6e6f 6465 5f6d  sample_by_node_m
+00001700: 696e da16 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
+00001710: 795f 6e6f 6465 5f6d 6178 da15 6d69 6e5f  y_node_max..min_
+00001720: 6368 696c 645f 7361 6d70 6c65 735f 6d69  child_samples_mi
+00001730: 6eda 156d 696e 5f63 6869 6c64 5f73 616d  n..min_child_sam
+00001740: 706c 6573 5f6d 6178 7250 0000 00da 0973  ples_maxrP.....s
+00001750: 7465 7073 5f6d 696e da09 7374 6570 735f  teps_min..steps_
+00001760: 6d61 78da 156e 756d 5f70 6172 616c 6c65  max..num_paralle
+00001770: 6c5f 7472 6565 5f6d 696e da15 6e75 6d5f  l_tree_min..num_
+00001780: 7061 7261 6c6c 656c 5f74 7265 655f 6d61  parallel_tree_ma
+00001790: 785a 1373 7567 6765 7374 5f63 6174 6567  xZ.suggest_categ
+000017a0: 6f72 6963 616c 7221 0000 0072 3b00 0000  oricalr!...r;...
+000017b0: 723c 0000 00da 066f 7074 756e 615a 0b69  r<.....optunaZ.i
+000017c0: 6e74 6567 7261 7469 6f6e 5a16 5847 426f  ntegrationZ.XGBo
+000017d0: 6f73 7450 7275 6e69 6e67 4361 6c6c 6261  ostPruningCallba
+000017e0: 636b 7213 0000 0072 3d00 0000 722b 0000  ckr....r=...r+..
+000017f0: 0072 3000 0000 da07 7072 6564 6963 7472  .r0.....predictr
+00001800: 5600 0000 da07 6173 6172 7261 7972 0700  V.....asarrayr..
+00001810: 0000 da02 6376 da13 676c 6f62 616c 5f72  ....cv..global_r
+00001820: 616e 646f 6d5f 7374 6174 65da 1773 6875  andom_state..shu
+00001830: 6666 6c65 5f64 7572 696e 675f 7472 6169  ffle_during_trai
+00001840: 6e69 6e67 da04 6d65 616e 290c da05 7472  ning..mean)...tr
+00001850: 6961 6cda 0570 6172 616d 723a 0000 0072  ial..paramr:...r
+00001860: 2000 0000 723f 0000 005a 1070 7275 6e69   ...r?...Z.pruni
+00001870: 6e67 5f63 616c 6c62 6163 6b72 3200 0000  ng_callbackr2...
+00001880: 7216 0000 00da 0570 7265 6473 da0b 7072  r......preds..pr
+00001890: 6564 5f6c 6162 656c 735a 076d 6174 7468  ed_labelsZ.matth
+000018a0: 6577 da06 7265 7375 6c74 a906 7240 0000  ew..result..r@..
+000018b0: 0072 1700 0000 5a08 7472 6169 6e5f 6f6e  .r....Z.train_on
+000018c0: 7223 0000 0072 2600 0000 7225 0000 0072  r#...r&...r%...r
+000018d0: 1800 0000 7219 0000 0072 4200 0000 9800  ....r....rB.....
+000018e0: 0000 73d6 0000 0002 0108 0102 ff08 0202  ..s.............
+000018f0: fe08 0302 fd04 0402 fc08 0502 fb06 0602  ................
+00001900: 0106 0106 0102 fd02 fa06 0b0e 0102 ff02  ................
+00001910: f506 0e0e 0102 ff02 f206 1102 0106 0106  ................
+00001920: 0102 fd02 ef06 1602 0106 0106 0102 fd02  ................
+00001930: ea06 1b02 0106 0106 0102 fd02 e506 2002  .............. .
+00001940: 0106 0106 0102 fd02 e006 2502 0106 0106  ..........%.....
+00001950: 0102 fd02 db06 2a02 0106 0106 0102 fd02  ......*.........
+00001960: d608 2f02 d106 300e 0102 ff02 d006 3302  ../...0.......3.
+00001970: 0106 0106 0102 fd04 cd10 3904 010a 0112  ..........9.....
+00001980: 010e 0206 0204 0104 ff0e 0410 0104 0102  ................
+00001990: 0102 0106 0106 0102 0104 0106 0106 f90a  ................
+000019a0: 0914 010e 0104 0104 0202 0102 0106 0106  ................
+000019b0: 0202 0106 0104 0106 0106 f70c 0c7a 2858  .............z(X
+000019c0: 6762 6f6f 7374 4d6f 6465 6c2e 6175 746f  gboostModel.auto
+000019d0: 7475 6e65 2e3c 6c6f 6361 6c73 3e2e 6f62  tune.<locals>.ob
+000019e0: 6a65 6374 6976 65da 0778 6762 6f6f 7374  jective..xgboost
+000019f0: 5429 025a 0c6d 756c 7469 7661 7269 6174  T).Z.multivariat
+00001a00: 6572 6100 0000 da08 6d69 6e69 6d69 7a65  era.....minimize
+00001a10: 7a07 2074 756e 696e 6729 03da 0964 6972  z. tuning)...dir
+00001a20: 6563 7469 6f6e da07 7361 6d70 6c65 725a  ection..samplerZ
+00001a30: 0a73 7475 6479 5f6e 616d 6529 04da 086e  .study_name)...n
+00001a40: 5f74 7269 616c 73da 0774 696d 656f 7574  _trials..timeout
+00001a50: 5a0e 6763 5f61 6674 6572 5f74 7269 616c  Z.gc_after_trial
+00001a60: 5a11 7368 6f77 5f70 726f 6772 6573 735f  Z.show_progress_
+00001a70: 6261 7272 4200 0000 7243 0000 0072 4400  barrB...rC...rD.
+00001a80: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
+00001a90: 0072 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
+00001aa0: 724b 0000 0072 4c00 0000 724d 0000 0072  rK...rL...rM...r
+00001ab0: 4e00 0000 724f 0000 0072 5000 0000 722e  N...rO...rP...r.
+00001ac0: 0000 0072 5100 0000 7a0d 4265 7374 2070  ...rQ...z.Best p
+00001ad0: 6172 616d 733a 2072 3a00 0000 4e29 2272  arams: r:...N)"r
+00001ae0: 0d00 0000 7202 0000 0072 1e00 0000 723b  ....r....r....r;
+00001af0: 0000 0072 3c00 0000 720c 0000 0072 2200  ...r<...r....r".
+00001b00: 0000 7215 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00001b10: 0072 3300 0000 727d 0000 005a 0873 616d  .r3...r}...Z.sam
+00001b20: 706c 6572 735a 0a54 5045 5361 6d70 6c65  plersZ.TPESample
+00001b30: 7272 8100 0000 5a0c 6372 6561 7465 5f73  rr....Z.create_s
+00001b40: 7475 6479 da08 6f70 7469 6d69 7a65 da1c  tudy..optimize..
+00001b50: 6879 7065 7270 6172 616d 6574 6572 5f74  hyperparameter_t
+00001b60: 756e 696e 675f 726f 756e 6473 da26 6879  uning_rounds.&hy
+00001b70: 7065 7270 6172 616d 6574 6572 5f74 756e  perparameter_tun
+00001b80: 696e 675f 6d61 785f 7275 6e74 696d 655f  ing_max_runtime_
+00001b90: 7365 6373 5a0d 7669 7375 616c 697a 6174  secsZ.visualizat
+00001ba0: 696f 6e5a 1970 6c6f 745f 6f70 7469 6d69  ionZ.plot_optimi
+00001bb0: 7a61 7469 6f6e 5f68 6973 746f 7279 da04  zation_history..
+00001bc0: 7368 6f77 5a16 706c 6f74 5f70 6172 616d  showZ.plot_param
+00001bd0: 5f69 6d70 6f72 7461 6e63 6573 da11 5a65  _importances..Ze
+00001be0: 726f 4469 7669 7369 6f6e 4572 726f 72da  roDivisionError.
+00001bf0: 0c52 756e 7469 6d65 4572 726f 725a 0a62  .RuntimeErrorZ.b
+00001c00: 6573 745f 7472 6961 6c72 3e00 0000 7263  est_trialr>...rc
+00001c10: 0000 0072 6400 0000 7265 0000 0072 6600  ...rd...re...rf.
+00001c20: 0000 7250 0000 0072 3600 0000 723a 0000  ..rP...r6...r:..
+00001c30: 0029 0b72 1700 0000 7223 0000 0072 2400  .).r....r#...r$.
+00001c40: 0000 7225 0000 0072 2600 0000 7242 0000  ..r%...r&...rB..
+00001c50: 00da 0961 6c67 6f72 6974 686d 728d 0000  ...algorithmr...
+00001c60: 005a 0573 7475 6479 da03 6669 675a 1278  .Z.study..figZ.x
+00001c70: 6762 6f6f 7374 5f62 6573 745f 7061 7261  gboost_best_para
+00001c80: 6d72 1800 0000 7289 0000 0072 1900 0000  mr....r....r....
+00001c90: 7235 0000 007e 0000 0073 9c00 0000 120b  r5...~...s......
+00001ca0: 0e01 0601 0802 0403 02ff 0402 02fe 0403  ................
+00001cb0: 02fd 0205 0201 04ff 1604 0463 0601 0801  ...........c....
+00001cc0: 06ff 0403 0201 0201 0801 06fd 0406 0201  ................
+00001cd0: 0601 0601 0201 0201 06fb 0207 0c01 0801  ................
+00001ce0: 0c01 0c01 1201 0401 02ff 0803 0201 0801  ................
+00001cf0: 02ff 0802 02fe 0803 02fd 0404 02fc 0805  ................
+00001d00: 02fb 0406 0201 02ff 02fa 0809 02f7 080a  ................
+00001d10: 02f6 080b 02f5 080c 02f4 080d 02f3 080e  ................
+00001d20: 02f2 080f 02f1 0810 02f0 0811 02ef 0812  ................
+00001d30: 02ee 0813 08ed 0e15 1001 7a15 5867 626f  ..........z.Xgbo
+00001d40: 6f73 744d 6f64 656c 2e61 7574 6f74 756e  ostModel.autotun
+00001d50: 65da 0264 6663 0200 0000 0000 0000 0000  e..dfc..........
+00001d60: 0000 0600 0000 0400 0000 4300 0000 73a0  ..........C...s.
+00001d70: 0000 0074 0074 01a0 02a1 009b 0064 019d  ...t.t.......d..
+00001d80: 0283 0101 0074 0364 0283 0101 0074 04a0  .....t.d.....t..
+00001d90: 057c 01a1 017d 027c 006a 0673 1974 0764  .|...}.|.j.s.t.d
+00001da0: 0383 0182 017c 006a 0873 2074 0764 0483  .....|.j.s t.d..
+00001db0: 0182 017c 006a 06a0 097c 02a1 017d 037c  ...|.j...|...}.|
+00001dc0: 006a 0a64 056b 0272 3c74 0ba0 0c64 0664  .j.d.k.r<t...d.d
+00001dd0: 0784 007c 0344 0083 01a1 017d 047c 047c  ...|.D.....}.|.|
+00001de0: 006a 086a 0d6b 047d 056e 0c7c 037d 0474  .j.j.k.}.n.|.}.t
+00001df0: 0ba0 0c64 0864 0784 007c 0344 0083 01a1  ...d.d...|.D....
+00001e00: 017d 0574 0364 0983 0101 007c 047c 0566  .}.t.d.....|.|.f
+00001e10: 0253 0029 0a7a 1750 7265 6469 6374 206f  .S.).z.Predict o
+00001e20: 6e20 756e 7365 656e 2064 6174 612e 7a33  n unseen data.z3
+00001e30: 3a20 5374 6172 7420 7072 6564 6963 7469  : Start predicti
+00001e40: 6e67 206f 6e20 6e65 7720 6461 7461 2075  ng on new data u
+00001e50: 7369 6e67 2058 6762 6f6f 7374 206d 6f64  sing Xgboost mod
+00001e60: 656c 2e7a 1c2b 2b2b 2b2b 2b2b 2b2b 2b2b  el.z.+++++++++++
+00001e70: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
+00001e80: 2b7a 204e 6f20 7472 6169 6e65 6420 6d6f  +z No trained mo
+00001e90: 6465 6c20 6861 7320 6265 656e 2066 6f75  del has been fou
+00001ea0: 6e64 2e7a 2b4e 6f20 6d6f 6465 6c20 636f  nd.z+No model co
+00001eb0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+00001ec0: 2068 6173 2062 6565 6e20 666f 756e 642e   has been found.
+00001ed0: 7211 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001ee0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+00001ef0: 0000 0067 007c 005d 067d 017c 0164 0019  ...g.|.].}.|.d..
+00001f00: 0091 0271 0253 0029 0172 2d00 0000 7218  ...q.S.).r-...r.
+00001f10: 0000 0072 5800 0000 7218 0000 0072 1800  ...rX...r....r..
+00001f20: 0000 7219 0000 0072 5b00 0000 3c01 0000  ..r....r[...<...
+00001f30: 7302 0000 0014 007a 2858 6762 6f6f 7374  s......z(Xgboost
+00001f40: 4d6f 6465 6c2e 7072 6564 6963 742e 3c6c  Model.predict.<l
+00001f50: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001f60: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+00001f70: 0000 0500 0000 5300 0000 7254 0000 0072  ......S...rT...r
+00001f80: 1800 0000 7255 0000 0072 5800 0000 7218  ....rU...rX...r.
+00001f90: 0000 0072 1800 0000 7219 0000 0072 5b00  ...r....r....r[.
+00001fa0: 0000 4201 0000 725c 0000 007a 1346 696e  ..B...r\...z.Fin
+00001fb0: 6973 6865 6420 7072 6564 6963 7469 6e67  ished predicting
+00001fc0: 290e 720d 0000 0072 0200 0000 721e 0000  ).r....r....r...
+00001fd0: 0072 3600 0000 723b 0000 0072 3c00 0000  .r6...r;...r<...
+00001fe0: 7216 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
+00001ff0: 7215 0000 0072 7e00 0000 7210 0000 0072  r....r~...r....r
+00002000: 5600 0000 727f 0000 00da 1863 6c61 7373  V...r......class
+00002010: 6966 6963 6174 696f 6e5f 7468 7265 7368  ification_thresh
+00002020: 6f6c 6429 0672 1700 0000 7298 0000 0072  old).r....r....r
+00002030: 4000 0000 5a0d 7061 7274 6961 6c5f 7072  @...Z.partial_pr
+00002040: 6f62 735a 0f70 7265 6469 6374 6564 5f70  obsZ.predicted_p
+00002050: 726f 6273 da11 7072 6564 6963 7465 645f  robs..predicted_
+00002060: 636c 6173 7365 7372 1800 0000 7218 0000  classesr....r...
+00002070: 0072 1900 0000 727e 0000 002d 0100 0073  .r....r~...-...s
+00002080: 2400 0000 0202 0c01 04ff 0803 0a01 0601  $...............
+00002090: 0801 0602 0801 0c02 0a01 1401 0a02 04ff  ................
+000020a0: 0404 1401 0801 0801 7a14 5867 626f 6f73  ........z.Xgboos
+000020b0: 744d 6f64 656c 2e70 7265 6469 6374 2903  tModel.predict).
+000020c0: 4e4e 4e29 1ada 085f 5f6e 616d 655f 5fda  NNN)...__name__.
+000020d0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000020e0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+000020f0: 5f5f 7204 0000 0072 0500 0000 7209 0000  __r....r....r...
+00002100: 0072 0b00 0000 720a 0000 0072 1a00 0000  .r....r....r....
+00002110: 7238 0000 00da 0653 6572 6965 7372 0300  r8.....Seriesr..
+00002120: 0000 da03 7374 72da 0566 6c6f 6174 7221  ....str..floatr!
+00002130: 0000 0072 2200 0000 da09 4461 7461 4672  ...r".....DataFr
+00002140: 616d 6572 3b00 0000 da07 426f 6f73 7465  amer;.....Booste
+00002150: 7272 4100 0000 7235 0000 0072 0600 0000  rrA...r5...r....
+00002160: 7256 0000 00da 076e 6461 7272 6179 727e  rV.....ndarrayr~
+00002170: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
+00002180: 0000 7219 0000 0072 0f00 0000 1a00 0000  ..r....r........
+00002190: 7350 0000 0008 0004 0102 0502 0102 0104  sP..............
+000021a0: fb06 0202 fe06 0302 fd06 0402 fc06 050a  ................
+000021b0: fb1c 0d08 0802 1504 0202 fe04 0302 fd04  ................
+000021c0: 0402 fc04 0502 fb04 060a fa02 3704 0202  ............7...
+000021d0: fe04 0302 fd04 0402 fc04 0502 fb02 060a  ................
+000021e0: fa00 7f24 3072 0f00 0000 291c 729f 0000  ...$0r....).r...
+000021f0: 0072 0200 0000 da06 7479 7069 6e67 7203  .r......typingr.
+00002200: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
+00002210: 0000 da05 6e75 6d70 7972 5600 0000 727d  ....numpyrV...r}
+00002220: 0000 00da 0670 616e 6461 7372 3800 0000  .....pandasr8...
+00002230: 728a 0000 0072 3b00 0000 5a0f 736b 6c65  r....r;...Z.skle
+00002240: 6172 6e2e 6d65 7472 6963 7372 0700 0000  arn.metricsr....
+00002250: da0d 736b 6c65 6172 6e2e 7574 696c 7372  ..sklearn.utilsr
+00002260: 0800 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
+00002270: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
+00002280: 6f6e 6669 6772 0900 0000 720a 0000 0072  onfigr....r....r
+00002290: 0b00 0000 da24 626c 7565 6361 7374 2e67  .....$bluecast.g
+000022a0: 656e 6572 616c 5f75 7469 6c73 2e67 656e  eneral_utils.gen
+000022b0: 6572 616c 5f75 7469 6c73 720c 0000 0072  eral_utilsr....r
+000022c0: 0d00 0000 da22 626c 7565 6361 7374 2e6d  ....."bluecast.m
+000022d0: 6c5f 6d6f 6465 6c6c 696e 672e 6261 7365  l_modelling.base
+000022e0: 5f63 6c61 7373 6573 720e 0000 0072 0f00  _classesr....r..
+000022f0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00002300: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00002310: 0100 0000 731a 0000 0004 000c 0618 0108  ....s...........
+00002320: 0208 0108 0108 010c 010c 0114 0210 050c  ................
+00002330: 0114 03                                  ...
```

### Comparing `bluecast-0.2/bluecast/ml_modelling/base_classes.py` & `bluecast-0.3/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/ml_modelling/xgboost.py` & `bluecast-0.3/bluecast/ml_modelling/xgboost.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,22 +49,28 @@
 
     def check_load_confs(self):
         """Load multiple configs or load default configs instead."""
         logger(f"{datetime.utcnow()}: Start loading existing or default config files..")
         if not self.conf_training:
             self.conf_training = TrainingConfig()
             logger(f"{datetime.utcnow()}: Load default TrainingConfig.")
+        else:
+            logger(f"{datetime.utcnow()}: Found provided TrainingConfig.")
 
         if not self.conf_xgboost:
             self.conf_xgboost = XgboostTuneParamsConfig()
             logger(f"{datetime.utcnow()}: Load default XgboostTuneParamsConfig.")
+        else:
+            logger(f"{datetime.utcnow()}: Found provided XgboostTuneParamsConfig.")
 
         if not self.conf_params_xgboost:
             self.conf_params_xgboost = XgboostFinalParamConfig()
             logger(f"{datetime.utcnow()}: Load default XgboostFinalParamConfig.")
+        else:
+            logger(f"{datetime.utcnow()}: Found provided XgboostFinalParamConfig.")
 
     def fit(
         self,
         x_train: pd.DataFrame,
         x_test: pd.DataFrame,
         y_train: pd.Series,
         y_test: pd.Series,
@@ -77,29 +83,47 @@
             raise ValueError("conf_params_xgboost or conf_training is None")
 
         if self.conf_training.autotune_model:
             self.autotune(x_train, x_test, y_train, y_test)
 
         print("Finished hyperparameter tuning")
 
+        print("Start training")
+        if self.conf_training.use_full_data_for_final_model:
+            logger(
+                f"""{datetime.utcnow()}: Union train and test data for final model training based on TrainingConfig
+             param 'use_full_data_for_final_model'"""
+            )
+            x_train = pd.concat([x_train, x_test])
+            y_train = pd.concat([y_train, y_test])
+
         if self.conf_params_xgboost.sample_weight:
             classes_weights = self.calculate_class_weights(y_train)
             d_train = xgb.DMatrix(x_train, label=y_train, weight=classes_weights)
         else:
             d_train = xgb.DMatrix(x_train, label=y_train)
+
         d_test = xgb.DMatrix(x_test, label=y_test)
         eval_set = [(d_train, "train"), (d_test, "test")]
 
-        self.model = xgb.train(
-            self.conf_params_xgboost.params,
-            d_train,
-            num_boost_round=self.conf_params_xgboost.params["steps"],
-            early_stopping_rounds=self.conf_training.early_stopping_rounds,
-            evals=eval_set,
-        )
+        if self.conf_training.hypertuning_cv_folds == 1:
+            self.model = xgb.train(
+                self.conf_params_xgboost.params,
+                d_train,
+                num_boost_round=self.conf_params_xgboost.params["steps"],
+                early_stopping_rounds=self.conf_training.early_stopping_rounds,
+                evals=eval_set,
+            )
+        else:
+            self.model = xgb.train(
+                self.conf_params_xgboost.params,
+                d_train,
+                num_boost_round=self.conf_params_xgboost.params["steps"],
+                eval_set=[(d_train, "train"), (d_test, "test")],
+            )
         print("Finished training")
         return self.model
 
     def autotune(
         self,
         x_train: pd.DataFrame,
         x_test: pd.DataFrame,
@@ -210,15 +234,15 @@
                 matthew = matthews_corrcoef(y_test, pred_labels) * -1
                 return matthew
             else:
                 result = xgb.cv(
                     params=param,
                     dtrain=d_train,
                     num_boost_round=param["steps"],
-                    early_stopping_rounds=self.conf_training.early_stopping_rounds,
+                    # early_stopping_rounds=self.conf_training.early_stopping_rounds,
                     nfold=self.conf_training.hypertuning_cv_folds,
                     as_pandas=True,
                     seed=self.conf_training.global_random_state,
                     callbacks=[pruning_callback],
                     shuffle=self.conf_training.shuffle_during_training,
                 )
```

### Comparing `bluecast-0.2/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-0.3/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 1424 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 9005 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 f058 8164 9005 0000  o........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 5a07 6401 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 0904 640c 6406 6507 6a0a  m.Z.....d.d.e.j.
 00000070: 6407 6504 6503 6505 650b 650c 650d 6603  d.e.e.e.e.e.e.f.
@@ -68,30 +68,29 @@
 00000430: 0000 5a0a 5f64 6179 6f66 7765 656b 720e  ..Z._dayofweekr.
 00000440: 0000 005a 055f 686f 7572 e901 0000 0029  ...Z._hour.....)
 00000450: 01da 0461 7869 7329 0a72 0600 0000 7202  ...axis).r....r.
 00000460: 0000 00da 0675 7463 6e6f 77da 0264 7472  .....utcnow..dtr
 00000470: 0b00 0000 da03 7374 7272 0c00 0000 720d  ......strr....r.
 00000480: 0000 0072 0e00 0000 da04 6472 6f70 2904  ...r......drop).
 00000490: 7207 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
-000004a0: 0163 a900 7216 0000 00fa 572f 5573 6572  .c..r.....W/User
-000004b0: 732f 7468 6f6d 6173 6d65 6973 736e 6572  s/thomasmeissner
-000004c0: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
-000004d0: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
-000004e0: 7072 6570 726f 6365 7373 696e 672f 6461  preprocessing/da
-000004f0: 7465 7469 6d65 5f66 6561 7475 7265 732e  tetime_features.
-00000500: 7079 da0e 6461 7465 5f63 6f6e 7665 7274  py..date_convert
-00000510: 6572 0e00 0000 7320 0000 0012 0d04 0104  er....s ........
-00000520: 0104 0208 0108 0208 0118 0108 0118 0108  ................
-00000530: 0118 0108 0118 0110 0104 0172 1800 0000  ...........r....
-00000540: 2901 4e29 0fda 075f 5f64 6f63 5f5f 7202  ).N)...__doc__r.
-00000550: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
-00000560: 7204 0000 0072 0500 0000 da06 7061 6e64  r....r......pand
-00000570: 6173 da02 7064 da24 626c 7565 6361 7374  as..pd.$bluecast
-00000580: 2e67 656e 6572 616c 5f75 7469 6c73 2e67  .general_utils.g
-00000590: 656e 6572 616c 5f75 7469 6c73 7206 0000  eneral_utilsr...
-000005a0: 00da 0944 6174 6146 7261 6d65 7213 0000  ...DataFramer...
-000005b0: 00da 0369 6e74 da05 666c 6f61 7472 1800  ...int..floatr..
-000005c0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000005d0: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000005e0: 0100 0000 731e 0000 0004 000c 0514 0108  ....s...........
-000005f0: 020c 0202 0604 fd04 0102 ff14 0202 fe06  ................
-00000600: 0302 fd04 040e fc                        .......
+000004a0: 0163 a900 7216 0000 00fa 4e2f 686f 6d65  .c..r.....N/home
+000004b0: 2f74 686f 6d61 732f 4964 6561 5072 6f6a  /thomas/IdeaProj
+000004c0: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
+000004d0: 7565 6361 7374 2f70 7265 7072 6f63 6573  uecast/preproces
+000004e0: 7369 6e67 2f64 6174 6574 696d 655f 6665  sing/datetime_fe
+000004f0: 6174 7572 6573 2e70 79da 0e64 6174 655f  atures.py..date_
+00000500: 636f 6e76 6572 7465 720e 0000 0073 2000  converter....s .
+00000510: 0000 120d 0401 0401 0402 0801 0802 0801  ................
+00000520: 1801 0801 1801 0801 1801 0801 1801 1001  ................
+00000530: 0401 7218 0000 0029 014e 290f da07 5f5f  ..r....).N)...__
+00000540: 646f 635f 5f72 0200 0000 da06 7479 7069  doc__r......typi
+00000550: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
+00000560: 00da 0670 616e 6461 73da 0270 64da 2462  ...pandas..pd.$b
+00000570: 6c75 6563 6173 742e 6765 6e65 7261 6c5f  luecast.general_
+00000580: 7574 696c 732e 6765 6e65 7261 6c5f 7574  utils.general_ut
+00000590: 696c 7372 0600 0000 da09 4461 7461 4672  ilsr......DataFr
+000005a0: 616d 6572 1300 0000 da03 696e 74da 0566  amer......int..f
+000005b0: 6c6f 6174 7218 0000 0072 1600 0000 7216  loatr....r....r.
+000005c0: 0000 0072 1600 0000 7217 0000 00da 083c  ...r....r......<
+000005d0: 6d6f 6475 6c65 3e01 0000 0073 1e00 0000  module>....s....
+000005e0: 0400 0c05 1401 0802 0c02 0206 04fd 0401  ................
+000005f0: 02ff 1402 02fe 0603 02fd 0404 0efc       ..............
```

### Comparing `bluecast-0.2/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-0.3/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 3122 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 320c 0000  o..........d2...
+00000000: 6f0d 0d0a 0000 0000 f058 8164 320c 0000  o........X.d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6401 6405 6c06 6d07 5a07 0100 4700  Z.d.d.l.m.Z...G.
 00000060: 6406 6407 8400 6407 8302 5a08 6404 5300  d.d...d...Z.d.S.
 00000070: 2908 610b 0100 000a 4120 6d6f 6475 6c65  ).a.....A module
@@ -53,178 +53,178 @@
 00000340: 6c73 6f20 6265 2072 6576 6572 7365 6420  lso be reversed 
 00000350: 746f 2074 7261 6e73 6c61 7465 2062 6163  to translate bac
 00000360: 6b2e 0a20 2020 2063 0100 0000 0000 0000  k..    c........
 00000370: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
 00000380: 730a 0000 0069 007c 005f 0064 0053 0029  s....i.|._.d.S.)
 00000390: 014e 2901 da14 7461 7267 6574 5f6c 6162  .N)...target_lab
 000003a0: 656c 5f6d 6170 7069 6e67 2901 da04 7365  el_mapping)...se
-000003b0: 6c66 a900 7208 0000 00fa 5a2f 5573 6572  lf..r.....Z/User
-000003c0: 732f 7468 6f6d 6173 6d65 6973 736e 6572  s/thomasmeissner
-000003d0: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
-000003e0: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
-000003f0: 7072 6570 726f 6365 7373 696e 672f 656e  preprocessing/en
-00000400: 636f 6465 5f74 6172 6765 745f 6c61 6265  code_target_labe
-00000410: 6c73 2e70 79da 085f 5f69 6e69 745f 5f19  ls.py..__init__.
-00000420: 0000 0073 0200 0000 0a01 7a1b 5461 7267  ...s......z.Targ
-00000430: 6574 4c61 6265 6c45 6e63 6f64 6572 2e5f  etLabelEncoder._
-00000440: 5f69 6e69 745f 5fda 0774 6172 6765 7473  _init__..targets
-00000450: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
-00000460: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
-00000470: 0073 6400 0000 7400 7401 a002 a100 9b00  .sd...t.t.......
-00000480: 6401 9d02 8301 0100 7c01 a003 6402 a101  d.......|...d...
-00000490: 7d01 7c01 6a04 7d02 7405 7c01 7406 6a07  }.|.j.}.t.|.t.j.
-000004a0: 8302 721b 7c01 a008 a100 7d01 7c01 7c02  ..r.|.....}.|.|.
-000004b0: 1900 a009 a100 7d03 6900 7d04 740a 7c03  ......}.i.}.t.|.
-000004c0: 8301 4400 5d08 5c02 7d05 7d06 7c05 7c04  ..D.].\.}.}.|.|.
-000004d0: 7c06 3c00 7127 7c04 5300 2903 7a37 4974  |.<.q'|.S.).z7It
-000004e0: 6572 6174 6520 7468 726f 7567 6820 7461  erate through ta
-000004f0: 7267 6574 2076 616c 7565 7320 616e 6420  rget values and 
-00000500: 6d61 7020 7468 656d 2074 6f20 6e75 6d65  map them to nume
-00000510: 7269 6373 2e7a 253a 2053 7461 7274 2066  rics.z%: Start f
-00000520: 6974 7469 6e67 2074 6172 6765 7420 6c61  itting target la
-00000530: 6265 6c20 656e 636f 6465 722e da08 6361  bel encoder...ca
-00000540: 7465 676f 7279 290b 7204 0000 0072 0200  tegory).r....r..
-00000550: 0000 da06 7574 636e 6f77 da06 6173 7479  ....utcnow..asty
-00000560: 7065 da04 6e61 6d65 da0a 6973 696e 7374  pe..name..isinst
-00000570: 616e 6365 da02 7064 da06 5365 7269 6573  ance..pd..Series
-00000580: da08 746f 5f66 7261 6d65 da06 756e 6971  ..to_frame..uniq
-00000590: 7565 da09 656e 756d 6572 6174 6529 0772  ue..enumerate).r
-000005a0: 0700 0000 720b 0000 00da 0363 6f6c da06  ....r......col..
-000005b0: 7661 6c75 6573 da0b 6361 745f 6d61 7070  values..cat_mapp
-000005c0: 696e 67da 056c 6162 656c da03 6361 7472  ing..label..catr
-000005d0: 0800 0000 7208 0000 0072 0900 0000 da11  ....r....r......
-000005e0: 6669 745f 6c61 6265 6c5f 656e 636f 6465  fit_label_encode
-000005f0: 721c 0000 0073 1400 0000 1202 0a01 0601  r....s..........
-00000600: 0c02 0801 0c02 0401 1001 0a01 0401 7a24  ..............z$
-00000610: 5461 7267 6574 4c61 6265 6c45 6e63 6f64  TargetLabelEncod
-00000620: 6572 2e66 6974 5f6c 6162 656c 5f65 6e63  er.fit_label_enc
-00000630: 6f64 6572 da07 6d61 7070 696e 6763 0300  oder..mappingc..
-00000640: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-00000650: 0000 0300 0000 736c 0000 0074 0074 01a0  ......sl...t.t..
-00000660: 02a1 009b 0064 019d 0283 0101 007c 01a0  .....d.......|..
-00000670: 0364 02a1 017d 017c 016a 047d 0374 057c  .d...}.|.j.}.t.|
-00000680: 0174 066a 0783 0272 1b7c 01a0 08a1 007d  .t.j...r.|.....}
-00000690: 017c 006a 0989 007c 017c 0319 00a0 0a87  .|.j...|.|......
-000006a0: 0066 0164 0364 0484 08a1 017c 017c 033c  .f.d.d.....|.|.<
-000006b0: 007c 017c 0319 00a0 0364 05a1 017c 017c  .|.|.....d...|.|
-000006c0: 033c 007c 0153 0029 067a 4554 7261 6e73  .<.|.S.).zETrans
-000006d0: 666f 726d 2074 6172 6765 7420 636f 6c75  form target colu
-000006e0: 6d6e 2066 726f 6d20 6361 7465 676f 7269  mn from categori
-000006f0: 6361 6c20 746f 206e 756d 6572 6963 616c  cal to numerical
-00000700: 2072 6570 7265 7365 6e74 6174 696f 6e2e   representation.
-00000710: 7a1f 3a20 5374 6172 7420 656e 636f 6469  z.: Start encodi
-00000720: 6e67 2074 6172 6765 7420 6c61 6265 6c73  ng target labels
-00000730: 2e72 0d00 0000 6301 0000 0000 0000 0000  .r....c.........
-00000740: 0000 0001 0000 0004 0000 0013 0000 0073  ...............s
-00000750: 0c00 0000 8800 a000 7c00 6401 a102 5300  ........|.d...S.
-00000760: 2902 4e69 e703 0000 2901 da03 6765 7429  ).Ni....)...get)
-00000770: 01da 0178 a901 721d 0000 0072 0800 0000  ...x..r....r....
-00000780: 7209 0000 00da 083c 6c61 6d62 6461 3e35  r......<lambda>5
-00000790: 0000 0073 0200 0000 0c00 7a3c 5461 7267  ...s......z<Targ
-000007a0: 6574 4c61 6265 6c45 6e63 6f64 6572 2e6c  etLabelEncoder.l
-000007b0: 6162 656c 5f65 6e63 6f64 6572 5f74 7261  abel_encoder_tra
-000007c0: 6e73 666f 726d 2e3c 6c6f 6361 6c73 3e2e  nsform.<locals>.
-000007d0: 3c6c 616d 6264 613e da03 696e 7429 0b72  <lambda>..int).r
-000007e0: 0400 0000 7202 0000 0072 0e00 0000 720f  ....r....r....r.
-000007f0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-00000800: 0000 7213 0000 0072 1400 0000 7206 0000  ..r....r....r...
-00000810: 00da 0561 7070 6c79 2904 7207 0000 0072  ...apply).r....r
-00000820: 0b00 0000 721d 0000 0072 1700 0000 7208  ....r....r....r.
-00000830: 0000 0072 2000 0000 7209 0000 00da 176c  ...r ...r......l
-00000840: 6162 656c 5f65 6e63 6f64 6572 5f74 7261  abel_encoder_tra
-00000850: 6e73 666f 726d 2b00 0000 7312 0000 0012  nsform+...s.....
-00000860: 040a 0106 010c 0108 0106 011a 0112 0104  ................
-00000870: 017a 2a54 6172 6765 744c 6162 656c 456e  .z*TargetLabelEn
-00000880: 636f 6465 722e 6c61 6265 6c5f 656e 636f  coder.label_enco
-00000890: 6465 725f 7472 616e 7366 6f72 6d63 0200  der_transformc..
-000008a0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-000008b0: 0000 4300 0000 7322 0000 007c 00a0 007c  ..C...s"...|...|
-000008c0: 01a1 017d 027c 027c 005f 017c 00a0 027c  ...}.|.|._.|...|
-000008d0: 017c 006a 01a1 027d 017c 0153 0029 017a  .|.j...}.|.S.).z
-000008e0: 4b57 7261 7070 6572 2066 756e 6374 696f  KWrapper functio
-000008f0: 6e20 7468 6174 2063 7265 6174 6573 2074  n that creates t
-00000900: 6865 206d 6170 7069 6e67 2061 6e64 2074  he mapping and t
-00000910: 7261 6e73 666f 726d 7320 7468 6520 7461  ransforms the ta
-00000920: 7267 6574 2063 6f6c 756d 6e2e 2903 721c  rget column.).r.
-00000930: 0000 0072 0600 0000 7224 0000 0029 0372  ...r....r$...).r
-00000940: 0700 0000 720b 0000 0072 1900 0000 7208  ....r....r....r.
-00000950: 0000 0072 0800 0000 7209 0000 00da 1b66  ...r....r......f
-00000960: 6974 5f74 7261 6e73 666f 726d 5f74 6172  it_transform_tar
-00000970: 6765 745f 6c61 6265 6c73 3900 0000 7308  get_labels9...s.
-00000980: 0000 000a 0206 010e 0104 017a 2e54 6172  ...........z.Tar
-00000990: 6765 744c 6162 656c 456e 636f 6465 722e  getLabelEncoder.
-000009a0: 6669 745f 7472 616e 7366 6f72 6d5f 7461  fit_transform_ta
-000009b0: 7267 6574 5f6c 6162 656c 7363 0200 0000  rget_labelsc....
-000009c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000009d0: 4300 0000 7312 0000 007c 00a0 007c 017c  C...s....|...|.|
-000009e0: 006a 01a1 027d 017c 0153 0029 017a 3e54  .j...}.|.S.).z>T
-000009f0: 7261 6e73 666f 726d 2074 6865 2074 6172  ransform the tar
-00000a00: 6765 7420 636f 6c75 6d6e 2062 6173 6564  get column based
-00000a10: 206f 6e20 616c 7265 6164 7920 6372 6561   on already crea
-00000a20: 7465 6420 6d61 7070 696e 6773 2e29 0272  ted mappings.).r
-00000a30: 2400 0000 7206 0000 0029 0272 0700 0000  $...r....).r....
-00000a40: 720b 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00000a50: 0900 0000 da17 7472 616e 7366 6f72 6d5f  ......transform_
-00000a60: 7461 7267 6574 5f6c 6162 656c 7340 0000  target_labels@..
-00000a70: 0073 0400 0000 0e02 0401 7a2a 5461 7267  .s........z*Targ
-00000a80: 6574 4c61 6265 6c45 6e63 6f64 6572 2e74  etLabelEncoder.t
-00000a90: 7261 6e73 666f 726d 5f74 6172 6765 745f  ransform_target_
-00000aa0: 6c61 6265 6c73 6302 0000 0000 0000 0000  labelsc.........
-00000ab0: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
-00000ac0: 5200 0000 7400 7401 a002 a100 9b00 6401  R...t.t.......d.
-00000ad0: 9d02 8301 0100 7c01 6a03 7d02 7404 7c01  ......|.j.}.t.|.
-00000ae0: 7405 6a06 8302 7216 7c01 a007 a100 7d01  t.j...r.|.....}.
-00000af0: 6402 6403 8400 7c00 6a08 a009 a100 4400  d.d...|.j.....D.
-00000b00: 8301 7d03 7c01 a00a 7c02 7c03 6901 a101  ..}.|...|.|.i...
-00000b10: 7d01 7c01 5300 2904 7a38 5265 7665 7273  }.|.S.).z8Revers
-00000b20: 6520 6e75 6d65 7269 6361 6c20 656e 636f  e numerical enco
-00000b30: 6469 6e67 7320 6261 636b 2074 6f20 6f72  dings back to or
-00000b40: 6967 696e 616c 2063 6174 6567 6f72 6965  iginal categorie
-00000b50: 732e 7a27 3a20 5374 6172 7420 7265 7665  s.z': Start reve
-00000b60: 7273 652d 656e 636f 6469 6e67 2074 6172  rse-encoding tar
-00000b70: 6765 7420 6c61 6265 6c73 2e63 0100 0000  get labels.c....
-00000b80: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000b90: 5300 0000 7316 0000 0069 007c 005d 075c  S...s....i.|.].\
-00000ba0: 027d 017d 027c 027c 0193 0271 0253 0072  .}.}.|.|...q.S.r
-00000bb0: 0800 0000 7208 0000 0029 03da 022e 30da  ....r....)....0.
-00000bc0: 036b 6579 da05 7661 6c75 6572 0800 0000  .key..valuer....
-00000bd0: 7208 0000 0072 0900 0000 da0a 3c64 6963  r....r......<dic
-00000be0: 7463 6f6d 703e 4d00 0000 7306 0000 0006  tcomp>M...s.....
-00000bf0: 000a 0106 ff7a 4654 6172 6765 744c 6162  .....zFTargetLab
-00000c00: 656c 456e 636f 6465 722e 6c61 6265 6c5f  elEncoder.label_
-00000c10: 656e 636f 6465 725f 7265 7665 7273 655f  encoder_reverse_
-00000c20: 7472 616e 7366 6f72 6d2e 3c6c 6f63 616c  transform.<local
-00000c30: 733e 2e3c 6469 6374 636f 6d70 3e29 0b72  s>.<dictcomp>).r
-00000c40: 0400 0000 7202 0000 0072 0e00 0000 7210  ....r....r....r.
-00000c50: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00000c60: 0000 7214 0000 0072 0600 0000 da05 6974  ..r....r......it
-00000c70: 656d 73da 0772 6570 6c61 6365 2904 7207  ems..replace).r.
-00000c80: 0000 0072 0b00 0000 7217 0000 005a 0f72  ...r....r....Z.r
-00000c90: 6576 6572 7365 5f6d 6170 7069 6e67 7208  everse_mappingr.
-00000ca0: 0000 0072 0800 0000 7209 0000 00da 1f6c  ...r....r......l
-00000cb0: 6162 656c 5f65 6e63 6f64 6572 5f72 6576  abel_encoder_rev
-00000cc0: 6572 7365 5f74 7261 6e73 666f 726d 4500  erse_transformE.
-00000cd0: 0000 7312 0000 0012 0206 010c 0208 0106  ..s.............
-00000ce0: 0208 0106 ff0e 0304 017a 3254 6172 6765  .........z2Targe
-00000cf0: 744c 6162 656c 456e 636f 6465 722e 6c61  tLabelEncoder.la
-00000d00: 6265 6c5f 656e 636f 6465 725f 7265 7665  bel_encoder_reve
-00000d10: 7273 655f 7472 616e 7366 6f72 6d4e 2910  rse_transformN).
-00000d20: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000d30: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000d40: 6d65 5f5f da07 5f5f 646f 635f 5f72 0a00  me__..__doc__r..
-00000d50: 0000 7212 0000 00da 0944 6174 6146 7261  ..r......DataFra
-00000d60: 6d65 7203 0000 00da 0373 7472 7222 0000  mer......strr"..
-00000d70: 0072 1c00 0000 7224 0000 0072 2500 0000  .r....r$...r%...
-00000d80: 7226 0000 0072 1300 0000 722d 0000 0072  r&...r....r-...r
-00000d90: 0800 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
-00000da0: 0000 0072 0500 0000 1100 0000 731c 0000  ...r........s...
-00000db0: 0008 0004 0108 071c 0302 0f04 0102 ff0a  ................
-00000dc0: 0102 ff04 020a fe16 0e16 071a 0572 0500  .............r..
-00000dd0: 0000 2909 7231 0000 0072 0200 0000 da06  ..).r1...r......
-00000de0: 7479 7069 6e67 7203 0000 00da 0670 616e  typingr......pan
-00000df0: 6461 7372 1200 0000 da24 626c 7565 6361  dasr.....$blueca
-00000e00: 7374 2e67 656e 6572 616c 5f75 7469 6c73  st.general_utils
-00000e10: 2e67 656e 6572 616c 5f75 7469 6c73 7204  .general_utilsr.
-00000e20: 0000 0072 0500 0000 7208 0000 0072 0800  ...r....r....r..
-00000e30: 0000 7208 0000 0072 0900 0000 da08 3c6d  ..r....r......<m
-00000e40: 6f64 756c 653e 0100 0000 730c 0000 0004  odule>....s.....
-00000e50: 000c 080c 0108 020c 0212 03              ...........
+000003b0: 6c66 a900 7208 0000 00fa 512f 686f 6d65  lf..r.....Q/home
+000003c0: 2f74 686f 6d61 732f 4964 6561 5072 6f6a  /thomas/IdeaProj
+000003d0: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
+000003e0: 7565 6361 7374 2f70 7265 7072 6f63 6573  uecast/preproces
+000003f0: 7369 6e67 2f65 6e63 6f64 655f 7461 7267  sing/encode_targ
+00000400: 6574 5f6c 6162 656c 732e 7079 da08 5f5f  et_labels.py..__
+00000410: 696e 6974 5f5f 1900 0000 7302 0000 000a  init__....s.....
+00000420: 017a 1b54 6172 6765 744c 6162 656c 456e  .z.TargetLabelEn
+00000430: 636f 6465 722e 5f5f 696e 6974 5f5f da07  coder.__init__..
+00000440: 7461 7267 6574 73da 0672 6574 7572 6e63  targets..returnc
+00000450: 0200 0000 0000 0000 0000 0000 0700 0000  ................
+00000460: 0400 0000 4300 0000 7364 0000 0074 0074  ....C...sd...t.t
+00000470: 01a0 02a1 009b 0064 019d 0283 0101 007c  .......d.......|
+00000480: 01a0 0364 02a1 017d 017c 016a 047d 0274  ...d...}.|.j.}.t
+00000490: 057c 0174 066a 0783 0272 1b7c 01a0 08a1  .|.t.j...r.|....
+000004a0: 007d 017c 017c 0219 00a0 09a1 007d 0369  .}.|.|.......}.i
+000004b0: 007d 0474 0a7c 0383 0144 005d 085c 027d  .}.t.|...D.].\.}
+000004c0: 057d 067c 057c 047c 063c 0071 277c 0453  .}.|.|.|.<.q'|.S
+000004d0: 0029 037a 3749 7465 7261 7465 2074 6872  .).z7Iterate thr
+000004e0: 6f75 6768 2074 6172 6765 7420 7661 6c75  ough target valu
+000004f0: 6573 2061 6e64 206d 6170 2074 6865 6d20  es and map them 
+00000500: 746f 206e 756d 6572 6963 732e 7a25 3a20  to numerics.z%: 
+00000510: 5374 6172 7420 6669 7474 696e 6720 7461  Start fitting ta
+00000520: 7267 6574 206c 6162 656c 2065 6e63 6f64  rget label encod
+00000530: 6572 2eda 0863 6174 6567 6f72 7929 0b72  er...category).r
+00000540: 0400 0000 7202 0000 00da 0675 7463 6e6f  ....r......utcno
+00000550: 77da 0661 7374 7970 65da 046e 616d 65da  w..astype..name.
+00000560: 0a69 7369 6e73 7461 6e63 65da 0270 64da  .isinstance..pd.
+00000570: 0653 6572 6965 73da 0874 6f5f 6672 616d  .Series..to_fram
+00000580: 65da 0675 6e69 7175 65da 0965 6e75 6d65  e..unique..enume
+00000590: 7261 7465 2907 7207 0000 0072 0b00 0000  rate).r....r....
+000005a0: da03 636f 6cda 0676 616c 7565 73da 0b63  ..col..values..c
+000005b0: 6174 5f6d 6170 7069 6e67 da05 6c61 6265  at_mapping..labe
+000005c0: 6cda 0363 6174 7208 0000 0072 0800 0000  l..catr....r....
+000005d0: 7209 0000 00da 1166 6974 5f6c 6162 656c  r......fit_label
+000005e0: 5f65 6e63 6f64 6572 1c00 0000 7314 0000  _encoder....s...
+000005f0: 0012 020a 0106 010c 0208 010c 0204 0110  ................
+00000600: 010a 0104 017a 2454 6172 6765 744c 6162  .....z$TargetLab
+00000610: 656c 456e 636f 6465 722e 6669 745f 6c61  elEncoder.fit_la
+00000620: 6265 6c5f 656e 636f 6465 72da 076d 6170  bel_encoder..map
+00000630: 7069 6e67 6303 0000 0000 0000 0000 0000  pingc...........
+00000640: 0004 0000 0005 0000 0003 0000 0073 6c00  .............sl.
+00000650: 0000 7400 7401 a002 a100 9b00 6401 9d02  ..t.t.......d...
+00000660: 8301 0100 7c01 a003 6402 a101 7d01 7c01  ....|...d...}.|.
+00000670: 6a04 7d03 7405 7c01 7406 6a07 8302 721b  j.}.t.|.t.j...r.
+00000680: 7c01 a008 a100 7d01 7c00 6a09 8900 7c01  |.....}.|.j...|.
+00000690: 7c03 1900 a00a 8700 6601 6403 6404 8408  |.......f.d.d...
+000006a0: a101 7c01 7c03 3c00 7c01 7c03 1900 a003  ..|.|.<.|.|.....
+000006b0: 6405 a101 7c01 7c03 3c00 7c01 5300 2906  d...|.|.<.|.S.).
+000006c0: 7a45 5472 616e 7366 6f72 6d20 7461 7267  zETransform targ
+000006d0: 6574 2063 6f6c 756d 6e20 6672 6f6d 2063  et column from c
+000006e0: 6174 6567 6f72 6963 616c 2074 6f20 6e75  ategorical to nu
+000006f0: 6d65 7269 6361 6c20 7265 7072 6573 656e  merical represen
+00000700: 7461 7469 6f6e 2e7a 1f3a 2053 7461 7274  tation.z.: Start
+00000710: 2065 6e63 6f64 696e 6720 7461 7267 6574   encoding target
+00000720: 206c 6162 656c 732e 720d 0000 0063 0100   labels.r....c..
+00000730: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000740: 0000 1300 0000 730c 0000 0088 00a0 007c  ......s........|
+00000750: 0064 01a1 0253 0029 024e 69e7 0300 0029  .d...S.).Ni....)
+00000760: 01da 0367 6574 2901 da01 78a9 0172 1d00  ...get)...x..r..
+00000770: 0000 7208 0000 0072 0900 0000 da08 3c6c  ..r....r......<l
+00000780: 616d 6264 613e 3500 0000 7302 0000 000c  ambda>5...s.....
+00000790: 007a 3c54 6172 6765 744c 6162 656c 456e  .z<TargetLabelEn
+000007a0: 636f 6465 722e 6c61 6265 6c5f 656e 636f  coder.label_enco
+000007b0: 6465 725f 7472 616e 7366 6f72 6d2e 3c6c  der_transform.<l
+000007c0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3eda  ocals>.<lambda>.
+000007d0: 0369 6e74 290b 7204 0000 0072 0200 0000  .int).r....r....
+000007e0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+000007f0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00000800: 0000 0072 0600 0000 da05 6170 706c 7929  ...r......apply)
+00000810: 0472 0700 0000 720b 0000 0072 1d00 0000  .r....r....r....
+00000820: 7217 0000 0072 0800 0000 7220 0000 0072  r....r....r ...r
+00000830: 0900 0000 da17 6c61 6265 6c5f 656e 636f  ......label_enco
+00000840: 6465 725f 7472 616e 7366 6f72 6d2b 0000  der_transform+..
+00000850: 0073 1200 0000 1204 0a01 0601 0c01 0801  .s..............
+00000860: 0601 1a01 1201 0401 7a2a 5461 7267 6574  ........z*Target
+00000870: 4c61 6265 6c45 6e63 6f64 6572 2e6c 6162  LabelEncoder.lab
+00000880: 656c 5f65 6e63 6f64 6572 5f74 7261 6e73  el_encoder_trans
+00000890: 666f 726d 6302 0000 0000 0000 0000 0000  formc...........
+000008a0: 0003 0000 0004 0000 0043 0000 0073 2200  .........C...s".
+000008b0: 0000 7c00 a000 7c01 a101 7d02 7c02 7c00  ..|...|...}.|.|.
+000008c0: 5f01 7c00 a002 7c01 7c00 6a01 a102 7d01  _.|...|.|.j...}.
+000008d0: 7c01 5300 2901 7a4b 5772 6170 7065 7220  |.S.).zKWrapper 
+000008e0: 6675 6e63 7469 6f6e 2074 6861 7420 6372  function that cr
+000008f0: 6561 7465 7320 7468 6520 6d61 7070 696e  eates the mappin
+00000900: 6720 616e 6420 7472 616e 7366 6f72 6d73  g and transforms
+00000910: 2074 6865 2074 6172 6765 7420 636f 6c75   the target colu
+00000920: 6d6e 2e29 0372 1c00 0000 7206 0000 0072  mn.).r....r....r
+00000930: 2400 0000 2903 7207 0000 0072 0b00 0000  $...).r....r....
+00000940: 7219 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
+00000950: 0900 0000 da1b 6669 745f 7472 616e 7366  ......fit_transf
+00000960: 6f72 6d5f 7461 7267 6574 5f6c 6162 656c  orm_target_label
+00000970: 7339 0000 0073 0800 0000 0a02 0601 0e01  s9...s..........
+00000980: 0401 7a2e 5461 7267 6574 4c61 6265 6c45  ..z.TargetLabelE
+00000990: 6e63 6f64 6572 2e66 6974 5f74 7261 6e73  ncoder.fit_trans
+000009a0: 666f 726d 5f74 6172 6765 745f 6c61 6265  form_target_labe
+000009b0: 6c73 6302 0000 0000 0000 0000 0000 0002  lsc.............
+000009c0: 0000 0004 0000 0043 0000 0073 1200 0000  .......C...s....
+000009d0: 7c00 a000 7c01 7c00 6a01 a102 7d01 7c01  |...|.|.j...}.|.
+000009e0: 5300 2901 7a3e 5472 616e 7366 6f72 6d20  S.).z>Transform 
+000009f0: 7468 6520 7461 7267 6574 2063 6f6c 756d  the target colum
+00000a00: 6e20 6261 7365 6420 6f6e 2061 6c72 6561  n based on alrea
+00000a10: 6479 2063 7265 6174 6564 206d 6170 7069  dy created mappi
+00000a20: 6e67 732e 2902 7224 0000 0072 0600 0000  ngs.).r$...r....
+00000a30: 2902 7207 0000 0072 0b00 0000 7208 0000  ).r....r....r...
+00000a40: 0072 0800 0000 7209 0000 00da 1774 7261  .r....r......tra
+00000a50: 6e73 666f 726d 5f74 6172 6765 745f 6c61  nsform_target_la
+00000a60: 6265 6c73 4000 0000 7304 0000 000e 0204  bels@...s.......
+00000a70: 017a 2a54 6172 6765 744c 6162 656c 456e  .z*TargetLabelEn
+00000a80: 636f 6465 722e 7472 616e 7366 6f72 6d5f  coder.transform_
+00000a90: 7461 7267 6574 5f6c 6162 656c 7363 0200  target_labelsc..
+00000aa0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00000ab0: 0000 4300 0000 7352 0000 0074 0074 01a0  ..C...sR...t.t..
+00000ac0: 02a1 009b 0064 019d 0283 0101 007c 016a  .....d.......|.j
+00000ad0: 037d 0274 047c 0174 056a 0683 0272 167c  .}.t.|.t.j...r.|
+00000ae0: 01a0 07a1 007d 0164 0264 0384 007c 006a  .....}.d.d...|.j
+00000af0: 08a0 09a1 0044 0083 017d 037c 01a0 0a7c  .....D...}.|...|
+00000b00: 027c 0369 01a1 017d 017c 0153 0029 047a  .|.i...}.|.S.).z
+00000b10: 3852 6576 6572 7365 206e 756d 6572 6963  8Reverse numeric
+00000b20: 616c 2065 6e63 6f64 696e 6773 2062 6163  al encodings bac
+00000b30: 6b20 746f 206f 7269 6769 6e61 6c20 6361  k to original ca
+00000b40: 7465 676f 7269 6573 2e7a 273a 2053 7461  tegories.z': Sta
+00000b50: 7274 2072 6576 6572 7365 2d65 6e63 6f64  rt reverse-encod
+00000b60: 696e 6720 7461 7267 6574 206c 6162 656c  ing target label
+00000b70: 732e 6301 0000 0000 0000 0000 0000 0003  s.c.............
+00000b80: 0000 0004 0000 0053 0000 0073 1600 0000  .......S...s....
+00000b90: 6900 7c00 5d07 5c02 7d01 7d02 7c02 7c01  i.|.].\.}.}.|.|.
+00000ba0: 9302 7102 5300 7208 0000 0072 0800 0000  ..q.S.r....r....
+00000bb0: 2903 da02 2e30 da03 6b65 79da 0576 616c  )....0..key..val
+00000bc0: 7565 7208 0000 0072 0800 0000 7209 0000  uer....r....r...
+00000bd0: 00da 0a3c 6469 6374 636f 6d70 3e4d 0000  ...<dictcomp>M..
+00000be0: 0073 0600 0000 0600 0a01 06ff 7a46 5461  .s..........zFTa
+00000bf0: 7267 6574 4c61 6265 6c45 6e63 6f64 6572  rgetLabelEncoder
+00000c00: 2e6c 6162 656c 5f65 6e63 6f64 6572 5f72  .label_encoder_r
+00000c10: 6576 6572 7365 5f74 7261 6e73 666f 726d  everse_transform
+00000c20: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00000c30: 6f6d 703e 290b 7204 0000 0072 0200 0000  omp>).r....r....
+00000c40: 720e 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000c50: 1200 0000 7213 0000 0072 1400 0000 7206  ....r....r....r.
+00000c60: 0000 00da 0569 7465 6d73 da07 7265 706c  .....items..repl
+00000c70: 6163 6529 0472 0700 0000 720b 0000 0072  ace).r....r....r
+00000c80: 1700 0000 5a0f 7265 7665 7273 655f 6d61  ....Z.reverse_ma
+00000c90: 7070 696e 6772 0800 0000 7208 0000 0072  ppingr....r....r
+00000ca0: 0900 0000 da1f 6c61 6265 6c5f 656e 636f  ......label_enco
+00000cb0: 6465 725f 7265 7665 7273 655f 7472 616e  der_reverse_tran
+00000cc0: 7366 6f72 6d45 0000 0073 1200 0000 1202  sformE...s......
+00000cd0: 0601 0c02 0801 0602 0801 06ff 0e03 0401  ................
+00000ce0: 7a32 5461 7267 6574 4c61 6265 6c45 6e63  z2TargetLabelEnc
+00000cf0: 6f64 6572 2e6c 6162 656c 5f65 6e63 6f64  oder.label_encod
+00000d00: 6572 5f72 6576 6572 7365 5f74 7261 6e73  er_reverse_trans
+00000d10: 666f 726d 4e29 10da 085f 5f6e 616d 655f  formN)...__name_
+00000d20: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000d30: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00000d40: 6f63 5f5f 720a 0000 0072 1200 0000 da09  oc__r....r......
+00000d50: 4461 7461 4672 616d 6572 0300 0000 da03  DataFramer......
+00000d60: 7374 7272 2200 0000 721c 0000 0072 2400  strr"...r....r$.
+00000d70: 0000 7225 0000 0072 2600 0000 7213 0000  ..r%...r&...r...
+00000d80: 0072 2d00 0000 7208 0000 0072 0800 0000  .r-...r....r....
+00000d90: 7208 0000 0072 0900 0000 7205 0000 0011  r....r....r.....
+00000da0: 0000 0073 1c00 0000 0800 0401 0807 1c03  ...s............
+00000db0: 020f 0401 02ff 0a01 02ff 0402 0afe 160e  ................
+00000dc0: 1607 1a05 7205 0000 0029 0972 3100 0000  ....r....).r1...
+00000dd0: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
+00000de0: 0000 da06 7061 6e64 6173 7212 0000 00da  ....pandasr.....
+00000df0: 2462 6c75 6563 6173 742e 6765 6e65 7261  $bluecast.genera
+00000e00: 6c5f 7574 696c 732e 6765 6e65 7261 6c5f  l_utils.general_
+00000e10: 7574 696c 7372 0400 0000 7205 0000 0072  utilsr....r....r
+00000e20: 0800 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
+00000e30: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000e40: 0073 0c00 0000 0400 0c08 0c01 0802 0c02  .s..............
+00000e50: 1203                                     ..
```

### Comparing `bluecast-0.2/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-0.3/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 6054 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 a617 0000  o..........d....
+00000000: 550d 0d0a 0000 0000 f058 8164 a617 0000  U........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c07 5a08 4700 6404 6405 8400 6405  d.l.Z.G.d.d...d.
 00000060: 8302 5a09 6403 5300 2906 7ae3 0a46 6561  ..Z.d.S.).z..Fea
 00000070: 7475 7265 2074 7970 6520 6465 7465 6374  ture type detect
@@ -18,270 +18,269 @@
 00000110: 6e64 2064 6174 6574 696d 6520 636f 6c75  nd datetime colu
 00000120: 6d6e 732e 2049 7420 616c 736f 2063 6173  mns. It also cas
 00000130: 7473 2063 6f6c 756d 6e73 2074 6f20 6120  ts columns to a 
 00000140: 7370 6563 6966 6963 2074 7970 652e 0ae9  specific type...
 00000150: 0000 0000 2905 da04 4469 6374 da04 4c69  ....)...Dict..Li
 00000160: 7374 da08 4f70 7469 6f6e 616c da05 5475  st..Optional..Tu
 00000170: 706c 65da 0555 6e69 6f6e 4e63 0000 0000  ple..UnionNc....
-00000180: 0000 0000 0000 0000 0000 0000 0c00 0000  ................
-00000190: 4000 0000 733a 0100 0065 005a 0164 005a  @...s:...e.Z.d.Z
-000001a0: 0264 015a 0309 0209 0209 0264 1964 0365  .d.Z.......d.d.e
-000001b0: 0465 0565 0665 0765 0865 0966 0319 0019  .e.e.e.e.e.f....
-000001c0: 0019 0064 0465 0465 0565 0665 0765 0865  ...d.e.e.e.e.e.e
-000001d0: 0966 0319 0019 0019 0064 0565 0465 0565  .f.......d.e.e.e
-000001e0: 0665 0765 0865 0966 0319 0019 0019 0066  .e.e.e.f.......f
-000001f0: 0664 0664 0784 055a 0a64 0865 0b6a 0c66  .d.d...Z.d.e.j.f
-00000200: 0264 0964 0a84 045a 0d64 0865 0b6a 0c64  .d.d...Z.d.e.j.d
-00000210: 0b65 0e65 0565 0665 0765 0965 0866 0319  .e.e.e.e.e.e.f..
-00000220: 0019 0065 0565 0665 0765 0965 0866 0319  ...e.e.e.e.e.f..
-00000230: 0019 0066 0219 0066 0464 0c64 0d84 045a  ...f...f.d.d...Z
-00000240: 0f64 0865 0b6a 0c64 0e65 0565 0665 0765  .d.e.j.d.e.e.e.e
-00000250: 0965 0866 0319 0019 0066 0464 0f64 1084  .e.f.....f.d.d..
-00000260: 045a 1064 0865 0b6a 0c64 1165 0565 0665  .Z.d.e.j.d.e.e.e
-00000270: 0765 0965 0866 0319 0019 0064 0b65 0b6a  .e.e.f.....d.e.j
-00000280: 0c66 0664 1264 1384 045a 1164 0865 0b6a  .f.d.d...Z.d.e.j
-00000290: 0c64 0b65 0b6a 0c66 0464 1464 1584 045a  .d.e.j.f.d.d...Z
-000002a0: 1209 0264 1a64 0865 0b6a 0c64 1665 0565  ...d.d.e.j.d.e.e
-000002b0: 0665 0765 0965 0864 0266 0419 0019 0064  .e.e.e.d.f.....d
-000002c0: 0b65 0b6a 0c66 0664 1764 1884 055a 1364  .e.j.f.d.d...Z.d
-000002d0: 0253 0029 1bda 1346 6561 7475 7265 5479  .S.)...FeatureTy
-000002e0: 7065 4465 7465 6374 6f72 7aa9 4465 7465  peDetectorz.Dete
-000002f0: 6374 2061 6e64 2063 6173 7420 6665 6174  ct and cast feat
-00000300: 7572 6520 7479 7065 7320 696e 2044 6174  ure types in Dat
-00000310: 6146 7261 6d65 2e0a 0a20 2020 2043 6f6c  aFrame...    Col
-00000320: 756d 6e20 6e61 6d65 7320 666f 7220 696e  umn names for in
-00000330: 6469 7669 6475 616c 2066 6561 7475 7265  dividual feature
-00000340: 2074 7970 6573 2063 616e 2062 6520 7072   types can be pr
-00000350: 6f76 6964 6564 2e20 4f74 6865 7277 6973  ovided. Otherwis
-00000360: 6520 7479 7065 7320 7769 6c6c 2062 6520  e types will be 
-00000370: 696e 6665 7272 6564 2061 6e64 2063 6173  inferred and cas
-00000380: 7465 6420 6163 636f 7264 696e 676c 792e  ted accordingly.
-00000390: 0a20 2020 204e da0b 6e75 6d5f 636f 6c75  .    N..num_colu
-000003a0: 6d6e 73da 0b63 6174 5f63 6f6c 756d 6e73  mns..cat_columns
-000003b0: da0c 6461 7465 5f63 6f6c 756d 6e73 6304  ..date_columnsc.
-000003c0: 0000 0000 0000 0000 0000 0004 0000 0002  ................
-000003d0: 0000 0043 0000 0073 2600 0000 7c01 7c00  ...C...s&...|.|.
-000003e0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 6900  _.|.|._.|.|._.i.
-000003f0: 7c00 5f03 6700 6401 a201 7c00 5f04 6400  |._.g.d...|._.d.
-00000400: 5300 2902 4e29 07da 0469 6e74 38da 0569  S.).N)...int8..i
-00000410: 6e74 3136 da05 696e 7433 32da 0569 6e74  nt16..int32..int
-00000420: 3634 da07 666c 6f61 7431 36da 0766 6c6f  64..float16..flo
-00000430: 6174 3332 da07 666c 6f61 7436 3429 0572  at32..float64).r
-00000440: 0800 0000 7209 0000 0072 0a00 0000 da12  ....r....r......
-00000450: 6465 7465 6374 6564 5f63 6f6c 5f74 7970  detected_col_typ
-00000460: 6573 da0a 6e75 6d5f 6474 7970 6573 2904  es..num_dtypes).
-00000470: da04 7365 6c66 7208 0000 0072 0900 0000  ..selfr....r....
-00000480: 720a 0000 00a9 0072 1500 0000 fa53 2f55  r......r.....S/U
-00000490: 7365 7273 2f74 686f 6d61 736d 6569 7373  sers/thomasmeiss
-000004a0: 6e65 722f 4964 6561 5072 6f6a 6563 7473  ner/IdeaProjects
-000004b0: 2f42 6c75 6543 6173 742f 626c 7565 6361  /BlueCast/blueca
-000004c0: 7374 2f70 7265 7072 6f63 6573 7369 6e67  st/preprocessing
-000004d0: 2f66 6561 7475 7265 5f74 7970 6573 2e70  /feature_types.p
-000004e0: 79da 085f 5f69 6e69 745f 5f12 0000 0073  y..__init__....s
-000004f0: 0a00 0000 0606 0601 0601 0601 0e01 7a1c  ..............z.
-00000500: 4665 6174 7572 6554 7970 6544 6574 6563  FeatureTypeDetec
-00000510: 746f 722e 5f5f 696e 6974 5f5f da02 6466  tor.__init__..df
-00000520: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-00000530: 0005 0000 0043 0000 0073 4600 0000 7c00  .....C...sF...|.
-00000540: 6a00 7320 6700 7d02 7c00 6a01 4400 5d14  j.s g.}.|.j.D.].
-00000550: 7d03 7c01 6a02 7c03 6701 6401 8d01 6a03  }.|.j.|.g.d...j.
-00000560: 7d04 7c04 4400 5d07 7d05 7c02 a004 7c05  }.|.D.].}.|...|.
-00000570: a101 0100 7114 7108 7c02 7c00 5f00 7c00  ....q.q.|.|._.|.
-00000580: 6a00 5300 2902 7a3f 4964 656e 7469 6679  j.S.).z?Identify
-00000590: 206e 756d 6572 6963 616c 2063 6f6c 756d   numerical colum
-000005a0: 6e73 2062 6173 6564 206f 6e20 616c 7265  ns based on alre
-000005b0: 6164 7920 6578 6973 7469 6e67 2064 6174  ady existing dat
-000005c0: 6120 7479 7065 2e29 01da 0769 6e63 6c75  a type.)...inclu
-000005d0: 6465 2905 7208 0000 0072 1300 0000 da0d  de).r....r......
-000005e0: 7365 6c65 6374 5f64 7479 7065 73da 0763  select_dtypes..c
-000005f0: 6f6c 756d 6e73 da06 6170 7065 6e64 2906  olumns..append).
-00000600: 7214 0000 0072 1800 0000 5a0c 6e75 6d5f  r....r....Z.num_
-00000610: 636f 6c5f 6c69 7374 5a07 7661 7274 7970  col_listZ.vartyp
-00000620: 65da 086e 756d 5f63 6f6c 73da 0363 6f6c  e..num_cols..col
-00000630: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00000640: 1469 6465 6e74 6966 795f 6e75 6d5f 636f  .identify_num_co
-00000650: 6c75 6d6e 7326 0000 0073 1200 0000 0603  lumns&...s......
-00000660: 0401 0a01 1001 0801 0c01 02ff 0602 0601  ................
-00000670: 7a28 4665 6174 7572 6554 7970 6544 6574  z(FeatureTypeDet
-00000680: 6563 746f 722e 6964 656e 7469 6679 5f6e  ector.identify_n
-00000690: 756d 5f63 6f6c 756d 6e73 da06 7265 7475  um_columns..retu
-000006a0: 726e 6302 0000 0000 0000 0000 0000 0006  rnc.............
-000006b0: 0000 0008 0000 0043 0000 0073 8a00 0000  .......C...s....
-000006c0: 7400 7c01 a001 6401 6701 a101 8301 7d02  t.|...d.g.....}.
-000006d0: 7c02 4400 5d10 7d03 7c01 7c03 1900 a002  |.D.].}.|.|.....
-000006e0: 7403 a101 7c01 7c03 3c00 6401 7c00 6a04  t...|.|.<.d.|.j.
-000006f0: 7c03 3c00 710a 7a18 7c01 6a05 6402 6402  |.<.q.z.|.j.d.d.
-00000700: 8502 7c01 6a06 a007 7c02 a101 0f00 6602  ..|.j...|.....f.
-00000710: 1900 7d04 7c04 6a06 a008 a100 7d05 5700  ..}.|.j.....}.W.
-00000720: 7c02 7c05 6602 5300 0400 7409 7944 0100  |.|.f.S...t.yD..
-00000730: 0100 0100 7c01 6a06 a008 a100 7d05 5900  ....|.j.....}.Y.
-00000740: 7c02 7c05 6602 5300 7700 2903 7a2b 4964  |.|.f.S.w.).z+Id
-00000750: 656e 7469 6679 2062 6f6f 6c65 616e 2063  entify boolean c
-00000760: 6f6c 756d 6e73 2062 6173 6564 206f 6e20  olumns based on 
-00000770: 6461 7461 2074 7970 65da 0462 6f6f 6c4e  data type..boolN
-00000780: 290a da04 6c69 7374 721a 0000 00da 0661  )...listr......a
-00000790: 7374 7970 6572 2100 0000 7212 0000 00da  styper!...r.....
-000007a0: 036c 6f63 721b 0000 00da 0469 7369 6eda  .locr......isin.
-000007b0: 0774 6f5f 6c69 7374 da09 4578 6365 7074  .to_list..Except
-000007c0: 696f 6e29 0672 1400 0000 7218 0000 00da  ion).r....r.....
-000007d0: 0962 6f6f 6c5f 636f 6c73 721e 0000 005a  .bool_colsr....Z
-000007e0: 0a6e 6f5f 626f 6f6c 5f64 66da 0c6e 6f5f  .no_bool_df..no_
-000007f0: 626f 6f6c 5f63 6f6c 7372 1500 0000 7215  bool_colsr....r.
-00000800: 0000 0072 1600 0000 da15 6964 656e 7469  ...r......identi
-00000810: 6679 5f62 6f6f 6c5f 636f 6c75 6d6e 7332  fy_bool_columns2
-00000820: 0000 0073 1800 0000 1004 0801 1201 0c01  ...s............
-00000830: 0203 1c01 0c01 0803 0cfe 0c01 0801 02fe  ................
-00000840: 7a29 4665 6174 7572 6554 7970 6544 6574  z)FeatureTypeDet
-00000850: 6563 746f 722e 6964 656e 7469 6679 5f62  ector.identify_b
-00000860: 6f6f 6c5f 636f 6c75 6d6e 7372 2900 0000  ool_columnsr)...
-00000870: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
-00000880: 0009 0000 0043 0000 0073 ee00 0000 7c00  .....C...s....|.
-00000890: 6a00 7239 7c00 6a01 7239 6700 7d03 7c00  j.r9|.j.r9g.}.|.
-000008a0: 6a00 4400 5d2a 7d04 7c04 7c00 6a01 7601  j.D.]*}.|.|.j.v.
-000008b0: 7235 7a19 7402 6a03 7c01 7c04 1900 6401  r5z.t.j.|.|...d.
-000008c0: 6402 8d02 7c01 7c04 3c00 7c03 a004 7c04  d...|.|.<.|...|.
-000008d0: a101 0100 6403 7c00 6a05 7406 7c04 8301  ....d.|.j.t.|...
-000008e0: 3c00 5700 710b 0400 7407 7934 0100 0100  <.W.q...t.y4....
-000008f0: 0100 5900 710b 7700 710b 7c03 7c00 5f00  ..Y.q.w.q.|.|._.
-00000900: 7c00 6a00 7373 7c00 6a01 7275 6700 7d03  |.j.ss|.j.rug.}.
-00000910: 7c02 4400 5d2a 7d04 7c04 7c00 6a01 7601  |.D.]*}.|.|.j.v.
-00000920: 726d 7a19 7402 6a03 7c01 7c04 1900 6401  rmz.t.j.|.|...d.
-00000930: 6402 8d02 7c01 7c04 3c00 7c03 a004 7c04  d...|.|.<.|...|.
-00000940: a101 0100 6403 7c00 6a05 7406 7c04 8301  ....d.|.j.t.|...
-00000950: 3c00 5700 7143 0400 7407 796c 0100 0100  <.W.qC..t.yl....
-00000960: 0100 5900 7143 7700 7143 7c03 7c00 5f00  ..Y.qCw.qC|.|._.
-00000970: 6404 5300 6404 5300 6404 5300 2905 7a44  d.S.d.S.d.S.).zD
-00000980: 5472 7920 6361 7374 696e 6720 746f 2064  Try casting to d
-00000990: 6174 6574 696d 652e 2045 7870 6563 7465  atetime. Expecte
-000009a0: 6420 6973 2061 2064 6174 6574 696d 6520  d is a datetime 
-000009b0: 666f 726d 6174 206f 6620 5959 5959 2d4d  format of YYYY-M
-000009c0: 4d2d 4444 54a9 01da 0979 6561 7266 6972  M-DDT....yearfir
-000009d0: 7374 fa0c 6461 7465 7469 6d65 5b6e 735d  st..datetime[ns]
-000009e0: 4e29 0872 0a00 0000 7208 0000 00da 0270  N).r....r......p
-000009f0: 64da 0b74 6f5f 6461 7465 7469 6d65 721c  d..to_datetimer.
-00000a00: 0000 0072 1200 0000 da03 7374 7272 2700  ...r......strr'.
-00000a10: 0000 2905 7214 0000 0072 1800 0000 7229  ..).r....r....r)
-00000a20: 0000 0072 0a00 0000 721e 0000 0072 1500  ...r....r....r..
-00000a30: 0000 7215 0000 0072 1600 0000 da1a 6964  ..r....r......id
-00000a40: 656e 7469 6679 5f64 6174 655f 7469 6d65  entify_date_time
-00000a50: 5f63 6f6c 756d 6e73 4300 0000 7336 0000  _columnsC...s6..
-00000a60: 000c 0404 010a 020a 0102 0116 010a 0112  ................
-00000a70: 010c 0104 0102 ff02 fb06 070c 0104 0108  ................
-00000a80: 020a 0102 0116 010a 0112 010c 0104 0102  ................
-00000a90: ff02 fb0a 0708 f57a 2e46 6561 7475 7265  .......z.Feature
-00000aa0: 5479 7065 4465 7465 6374 6f72 2e69 6465  TypeDetector.ide
-00000ab0: 6e74 6966 795f 6461 7465 5f74 696d 655f  ntify_date_time_
-00000ac0: 636f 6c75 6d6e 7372 2800 0000 6303 0000  columnsr(...c...
-00000ad0: 0000 0000 0000 0000 0008 0000 0009 0000  ................
-00000ae0: 0043 0000 0073 d200 0000 7c02 720b 7c00  .C...s....|.r.|.
-00000af0: 6a00 720b 7c02 7c00 6a00 1700 7d03 6e13  j.r.|.|.j...}.n.
-00000b00: 7c02 7213 7c00 6a00 7313 7c02 7d03 6e0b  |.r.|.j.s.|.}.n.
-00000b10: 7c02 731c 7c00 6a00 721c 7c00 6a00 7d03  |.s.|.j.r.|.j.}.
-00000b20: 6e02 6700 7d03 7c01 6a01 6401 6401 8502  n.g.}.|.j.d.d...
-00000b30: 7c01 6a02 a003 7c03 a101 0f00 6602 1900  |.j...|.....f...
-00000b40: 7d04 7c04 6a02 a004 a100 7d05 6700 7d06  }.|.j.....}.g.}.
-00000b50: 7c05 4400 5d2e 7d07 7a10 7c01 7c07 1900  |.D.].}.z.|.|...
-00000b60: a005 7406 a101 7c01 7c07 3c00 6402 7c00  ..t...|.|.<.d.|.
-00000b70: 6a07 7c07 3c00 5700 7135 0400 7408 7963  j.|.<.W.q5..t.yc
-00000b80: 0100 0100 0100 7c01 7c07 1900 a005 7409  ......|.|.....t.
-00000b90: a101 7c01 7c07 3c00 6403 7c00 6a07 7c07  ..|.|.<.d.|.j.|.
-00000ba0: 3c00 7c06 a00a 7c07 a101 0100 5900 7135  <.|...|.....Y.q5
-00000bb0: 7700 7c06 7c00 5f0b 7c01 5300 2904 7aae  w.|.|._.|.S.).z.
-00000bc0: 5472 6561 7420 7265 6d61 696e 696e 6720  Treat remaining 
-00000bd0: 636f 6c75 6d6e 732e 0a0a 2020 2020 2020  columns...      
-00000be0: 2020 5461 6b65 7320 7265 6d61 696e 696e    Takes remainin
-00000bf0: 6720 636f 6c75 6d6e 7320 616e 6420 7472  g columns and tr
-00000c00: 6965 7320 746f 2063 6173 7420 7468 656d  ies to cast them
-00000c10: 2061 7320 6e75 6d65 7269 6361 6c2e 2049   as numerical. I
-00000c20: 6620 6e6f 7420 7375 6363 6573 7366 756c  f not successful
-00000c30: 2c20 7468 656e 2063 6f6c 756d 6e73 2061  , then columns a
-00000c40: 7265 2061 7373 756d 6564 2074 6f20 6265  re assumed to be
-00000c50: 0a20 2020 2020 2020 2063 6174 6567 6f72  .        categor
-00000c60: 6963 616c 2e0a 2020 2020 2020 2020 4eda  ical..        N.
-00000c70: 0566 6c6f 6174 da06 6f62 6a65 6374 290c  .float..object).
-00000c80: 720a 0000 0072 2400 0000 721b 0000 0072  r....r$...r....r
-00000c90: 2500 0000 7226 0000 0072 2300 0000 7232  %...r&...r#...r2
-00000ca0: 0000 0072 1200 0000 7227 0000 0072 3000  ...r....r'...r0.
-00000cb0: 0000 721c 0000 0072 0900 0000 2908 7214  ..r....r....).r.
-00000cc0: 0000 0072 1800 0000 7228 0000 005a 0f6e  ...r....r(...Z.n
-00000cd0: 6f5f 626f 6f6c 5f64 745f 636f 6c73 5a13  o_bool_dt_colsZ.
-00000ce0: 6e6f 5f62 6f6f 6c5f 6461 7465 7469 6d65  no_bool_datetime
-00000cf0: 5f64 665a 156e 6f5f 626f 6f6c 5f64 6174  _dfZ.no_bool_dat
-00000d00: 6574 696d 655f 636f 6c73 7209 0000 0072  etime_colsr....r
-00000d10: 1e00 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00000d20: 0000 00da 1b63 6173 745f 7265 7374 5f63  .....cast_rest_c
-00000d30: 6f6c 756d 6e73 5f74 6f5f 6f62 6a65 6374  olumns_to_object
-00000d40: 6000 0000 732a 0000 000a 080c 010a 0106  `...s*..........
-00000d50: 010a 0108 0104 021c 010a 0104 0108 0102  ................
-00000d60: 0112 010e 010c 0112 010a 010e 0102 fd06  ................
-00000d70: 0404 017a 2f46 6561 7475 7265 5479 7065  ...z/FeatureType
-00000d80: 4465 7465 6374 6f72 2e63 6173 745f 7265  Detector.cast_re
-00000d90: 7374 5f63 6f6c 756d 6e73 5f74 6f5f 6f62  st_columns_to_ob
-00000da0: 6a65 6374 6302 0000 0000 0000 0000 0000  jectc...........
-00000db0: 0004 0000 0004 0000 0043 0000 0073 3400  .........C...s4.
-00000dc0: 0000 7c00 a000 7c01 a101 0100 7c00 a001  ..|...|.....|...
-00000dd0: 7c01 a101 5c02 7d02 7d03 7c00 a002 7c01  |...\.}.}.|...|.
-00000de0: 7c03 a102 0100 7c00 a003 7c01 7c02 a102  |.....|...|.|...
-00000df0: 7d01 7c01 5300 2901 7a72 4964 656e 7469  }.|.S.).zrIdenti
-00000e00: 6679 2061 6e64 2074 7261 6e73 666f 726d  fy and transform
-00000e10: 2066 6561 7475 7265 2074 7970 6573 2e0a   feature types..
-00000e20: 0a20 2020 2020 2020 2057 7261 7070 6572  .        Wrapper
-00000e30: 2066 756e 6374 696f 6e20 746f 206f 7263   function to orc
-00000e40: 6865 7374 6572 2064 6966 6665 7265 6e74  hester different
-00000e50: 2064 6574 6563 7469 6f6e 206d 6574 686f   detection metho
-00000e60: 6473 2e0a 2020 2020 2020 2020 2904 721f  ds..        ).r.
-00000e70: 0000 0072 2a00 0000 7231 0000 0072 3400  ...r*...r1...r4.
-00000e80: 0000 2904 7214 0000 0072 1800 0000 7228  ..).r....r....r(
-00000e90: 0000 0072 2900 0000 7215 0000 0072 1500  ...r)...r....r..
-00000ea0: 0000 7216 0000 00da 1b66 6974 5f74 7261  ..r......fit_tra
-00000eb0: 6e73 666f 726d 5f66 6561 7475 7265 5f74  nsform_feature_t
-00000ec0: 7970 6573 7e00 0000 730a 0000 000a 050e  ypes~...s.......
-00000ed0: 010c 010c 0104 017a 2f46 6561 7475 7265  .......z/Feature
-00000ee0: 5479 7065 4465 7465 6374 6f72 2e66 6974  TypeDetector.fit
-00000ef0: 5f74 7261 6e73 666f 726d 5f66 6561 7475  _transform_featu
-00000f00: 7265 5f74 7970 6573 da0b 6967 6e6f 7265  re_types..ignore
-00000f10: 5f63 6f6c 7363 0300 0000 0000 0000 0000  _colsc..........
-00000f20: 0000 0400 0000 0500 0000 4300 0000 7366  ..........C...sf
-00000f30: 0000 0009 007c 006a 0044 005d 2c7d 037c  .....|.j.D.],}.|
-00000f40: 0272 307c 037c 0276 0172 307c 037c 016a  .r0|.|.v.r0|.|.j
-00000f50: 0176 0072 307c 006a 007c 0319 0064 016b  .v.r0|.j.|...d.k
-00000f60: 0272 2474 026a 037c 017c 0319 0064 0264  .r$t.j.|.|...d.d
-00000f70: 038d 027c 017c 033c 0071 047c 017c 0319  ...|.|.<.q.|.|..
-00000f80: 00a0 047c 006a 007c 0319 00a1 017c 017c  ...|.j.|.....|.|
-00000f90: 033c 0071 047c 0153 0029 047a 3654 7261  .<.q.|.S.).z6Tra
-00000fa0: 6e73 666f 726d 2066 6561 7475 7265 2074  nsform feature t
-00000fb0: 7970 6573 2062 6173 6564 206f 6e20 616c  ypes based on al
-00000fc0: 7265 6164 7920 6d61 7070 6564 2074 7970  ready mapped typ
-00000fd0: 6573 2e72 2d00 0000 5472 2b00 0000 2905  es.r-...Tr+...).
-00000fe0: 7212 0000 0072 1b00 0000 722e 0000 0072  r....r....r....r
-00000ff0: 2f00 0000 7223 0000 0029 0472 1400 0000  /...r#...).r....
-00001000: 7218 0000 0072 3600 0000 da03 6b65 7972  r....r6.....keyr
-00001010: 1500 0000 7215 0000 0072 1600 0000 da17  ....r....r......
-00001020: 7472 616e 7366 6f72 6d5f 6665 6174 7572  transform_featur
-00001030: 655f 7479 7065 7389 0000 0073 1000 0000  e_types....s....
-00001040: 0204 0a04 1601 0e01 1801 1802 0280 0401  ................
-00001050: 7a2b 4665 6174 7572 6554 7970 6544 6574  z+FeatureTypeDet
-00001060: 6563 746f 722e 7472 616e 7366 6f72 6d5f  ector.transform_
-00001070: 6665 6174 7572 655f 7479 7065 7329 034e  feature_types).N
-00001080: 4e4e 2901 4e29 14da 085f 5f6e 616d 655f  NN).N)...__name_
-00001090: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000010a0: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-000010b0: 6f63 5f5f 7204 0000 0072 0300 0000 7206  oc__r....r....r.
-000010c0: 0000 0072 3000 0000 da03 696e 7472 3200  ...r0.....intr2.
-000010d0: 0000 7217 0000 0072 2e00 0000 da09 4461  ..r....r......Da
-000010e0: 7461 4672 616d 6572 1f00 0000 7205 0000  taFramer....r...
-000010f0: 0072 2a00 0000 7231 0000 0072 3400 0000  .r*...r1...r4...
-00001100: 7235 0000 0072 3800 0000 7215 0000 0072  r5...r8...r....r
-00001110: 1500 0000 7215 0000 0072 1600 0000 7207  ....r....r....r.
-00001120: 0000 000c 0000 0073 4e00 0000 0800 0401  .......sN.......
-00001130: 0207 0201 0201 04fc 1402 02fe 1403 02fd  ................
-00001140: 1404 0afc 1014 020c 0401 02ff 2602 0afe  ............&...
-00001150: 0211 0401 02ff 1001 0aff 021d 0401 02ff  ................
-00001160: 1001 02ff 0402 0afe 161e 020c 04ff 0401  ................
-00001170: 02ff 1201 02ff 0402 0efe 7207 0000 0029  ..........r....)
-00001180: 0a72 3c00 0000 da06 7479 7069 6e67 7202  .r<.....typingr.
-00001190: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-000011a0: 0000 7206 0000 00da 0670 616e 6461 7372  ..r......pandasr
-000011b0: 2e00 0000 7207 0000 0072 1500 0000 7215  ....r....r....r.
-000011c0: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
-000011d0: 6d6f 6475 6c65 3e01 0000 0073 0800 0000  module>....s....
-000011e0: 0400 1c06 0802 1203                      ........
+00000180: 0000 0000 0000 0000 0000 0000 0900 0000  ................
+00000190: 4000 0000 7320 0100 0065 005a 0164 005a  @...s ...e.Z.d.Z
+000001a0: 0264 015a 0364 1765 0465 0565 0665 0765  .d.Z.d.e.e.e.e.e
+000001b0: 0865 0966 0319 0019 0019 0065 0465 0565  .e.f.......e.e.e
+000001c0: 0665 0765 0865 0966 0319 0019 0019 0065  .e.e.e.f.......e
+000001d0: 0465 0565 0665 0765 0865 0966 0319 0019  .e.e.e.e.e.f....
+000001e0: 0019 0064 039c 0364 0464 0584 055a 0a65  ...d...d.d...Z.e
+000001f0: 0b6a 0c64 069c 0164 0764 0884 045a 0d65  .j.d...d.d...Z.e
+00000200: 0b6a 0c65 0e65 0565 0665 0765 0965 0866  .j.e.e.e.e.e.e.f
+00000210: 0319 0019 0065 0565 0665 0765 0965 0866  .....e.e.e.e.e.f
+00000220: 0319 0019 0066 0219 0064 099c 0264 0a64  .....f...d...d.d
+00000230: 0b84 045a 0f65 0b6a 0c65 0565 0665 0765  ...Z.e.j.e.e.e.e
+00000240: 0965 0866 0319 0019 0064 0c9c 0264 0d64  .e.f.....d...d.d
+00000250: 0e84 045a 1065 0b6a 0c65 0565 0665 0765  ...Z.e.j.e.e.e.e
+00000260: 0965 0866 0319 0019 0065 0b6a 0c64 0f9c  .e.f.....e.j.d..
+00000270: 0364 1064 1184 045a 1165 0b6a 0c65 0b6a  .d.d...Z.e.j.e.j
+00000280: 0c64 099c 0264 1264 1384 045a 1264 1865  .d...d.d...Z.d.e
+00000290: 0b6a 0c65 0565 0665 0765 0965 0864 0266  .j.e.e.e.e.e.d.f
+000002a0: 0419 0019 0065 0b6a 0c64 149c 0364 1564  .....e.j.d...d.d
+000002b0: 1684 055a 1364 0253 0029 19da 1346 6561  ...Z.d.S.)...Fea
+000002c0: 7475 7265 5479 7065 4465 7465 6374 6f72  tureTypeDetector
+000002d0: 7aa9 4465 7465 6374 2061 6e64 2063 6173  z.Detect and cas
+000002e0: 7420 6665 6174 7572 6520 7479 7065 7320  t feature types 
+000002f0: 696e 2044 6174 6146 7261 6d65 2e0a 0a20  in DataFrame... 
+00000300: 2020 2043 6f6c 756d 6e20 6e61 6d65 7320     Column names 
+00000310: 666f 7220 696e 6469 7669 6475 616c 2066  for individual f
+00000320: 6561 7475 7265 2074 7970 6573 2063 616e  eature types can
+00000330: 2062 6520 7072 6f76 6964 6564 2e20 4f74   be provided. Ot
+00000340: 6865 7277 6973 6520 7479 7065 7320 7769  herwise types wi
+00000350: 6c6c 2062 6520 696e 6665 7272 6564 2061  ll be inferred a
+00000360: 6e64 2063 6173 7465 6420 6163 636f 7264  nd casted accord
+00000370: 696e 676c 792e 0a20 2020 204e 2903 da0b  ingly..    N)...
+00000380: 6e75 6d5f 636f 6c75 6d6e 73da 0b63 6174  num_columns..cat
+00000390: 5f63 6f6c 756d 6e73 da0c 6461 7465 5f63  _columns..date_c
+000003a0: 6f6c 756d 6e73 6304 0000 0000 0000 0000  olumnsc.........
+000003b0: 0000 0004 0000 0007 0000 0043 0000 0073  ...........C...s
+000003c0: 3000 0000 7c01 7c00 5f00 7c02 7c00 5f01  0...|.|._.|.|._.
+000003d0: 7c03 7c00 5f02 6900 7c00 5f03 6401 6402  |.|._.i.|._.d.d.
+000003e0: 6403 6404 6405 6406 6407 6707 7c00 5f04  d.d.d.d.d.g.|._.
+000003f0: 6400 5300 2908 4eda 0469 6e74 38da 0569  d.S.).N..int8..i
+00000400: 6e74 3136 da05 696e 7433 32da 0569 6e74  nt16..int32..int
+00000410: 3634 da07 666c 6f61 7431 36da 0766 6c6f  64..float16..flo
+00000420: 6174 3332 da07 666c 6f61 7436 3429 0572  at32..float64).r
+00000430: 0800 0000 7209 0000 0072 0a00 0000 da12  ....r....r......
+00000440: 6465 7465 6374 6564 5f63 6f6c 5f74 7970  detected_col_typ
+00000450: 6573 da0a 6e75 6d5f 6474 7970 6573 2904  es..num_dtypes).
+00000460: da04 7365 6c66 7208 0000 0072 0900 0000  ..selfr....r....
+00000470: 720a 0000 00a9 0072 1500 0000 fa4a 2f68  r......r.....J/h
+00000480: 6f6d 652f 7468 6f6d 6173 2f49 6465 6150  ome/thomas/IdeaP
+00000490: 726f 6a65 6374 732f 426c 7565 4361 7374  rojects/BlueCast
+000004a0: 2f62 6c75 6563 6173 742f 7072 6570 726f  /bluecast/prepro
+000004b0: 6365 7373 696e 672f 6665 6174 7572 655f  cessing/feature_
+000004c0: 7479 7065 732e 7079 da08 5f5f 696e 6974  types.py..__init
+000004d0: 5f5f 1200 0000 7318 0000 0000 0606 0106  __....s.........
+000004e0: 0106 0106 0202 0102 0102 0102 0102 0102  ................
+000004f0: 0102 f97a 1c46 6561 7475 7265 5479 7065  ...z.FeatureType
+00000500: 4465 7465 6374 6f72 2e5f 5f69 6e69 745f  Detector.__init_
+00000510: 5f29 01da 0264 6663 0200 0000 0000 0000  _)...dfc........
+00000520: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
+00000530: 7346 0000 007c 006a 0073 4067 007d 027c  sF...|.j.s@g.}.|
+00000540: 006a 0144 005d 287d 037c 016a 027c 0367  .j.D.](}.|.j.|.g
+00000550: 0164 018d 016a 037d 047c 0444 005d 0e7d  .d...j.}.|.D.].}
+00000560: 057c 02a0 047c 05a1 0101 0071 2871 107c  .|...|.....q(q.|
+00000570: 027c 005f 007c 006a 0053 0029 027a 3f49  .|._.|.j.S.).z?I
+00000580: 6465 6e74 6966 7920 6e75 6d65 7269 6361  dentify numerica
+00000590: 6c20 636f 6c75 6d6e 7320 6261 7365 6420  l columns based 
+000005a0: 6f6e 2061 6c72 6561 6479 2065 7869 7374  on already exist
+000005b0: 696e 6720 6461 7461 2074 7970 652e 2901  ing data type.).
+000005c0: da07 696e 636c 7564 6529 0572 0800 0000  ..include).r....
+000005d0: 7213 0000 00da 0d73 656c 6563 745f 6474  r......select_dt
+000005e0: 7970 6573 da07 636f 6c75 6d6e 73da 0661  ypes..columns..a
+000005f0: 7070 656e 6429 0672 1400 0000 7218 0000  ppend).r....r...
+00000600: 00da 0c6e 756d 5f63 6f6c 5f6c 6973 74da  ...num_col_list.
+00000610: 0776 6172 7479 7065 da08 6e75 6d5f 636f  .vartype..num_co
+00000620: 6c73 da03 636f 6c72 1500 0000 7215 0000  ls..colr....r...
+00000630: 0072 1600 0000 da14 6964 656e 7469 6679  .r......identify
+00000640: 5f6e 756d 5f63 6f6c 756d 6e73 2600 0000  _num_columns&...
+00000650: 7310 0000 0000 0306 0104 010a 0110 0108  s...............
+00000660: 010e 0106 017a 2846 6561 7475 7265 5479  .....z(FeatureTy
+00000670: 7065 4465 7465 6374 6f72 2e69 6465 6e74  peDetector.ident
+00000680: 6966 795f 6e75 6d5f 636f 6c75 6d6e 7329  ify_num_columns)
+00000690: 0272 1800 0000 da06 7265 7475 726e 6302  .r......returnc.
+000006a0: 0000 0000 0000 0000 0000 0006 0000 0008  ................
+000006b0: 0000 0043 0000 0073 8800 0000 7400 7c01  ...C...s....t.|.
+000006c0: a001 6401 6701 a101 8301 7d02 7c02 4400  ..d.g.....}.|.D.
+000006d0: 5d20 7d03 7c01 7c03 1900 a002 7403 a101  ] }.|.|.....t...
+000006e0: 7c01 7c03 3c00 6401 7c00 6a04 7c03 3c00  |.|.<.d.|.j.|.<.
+000006f0: 7114 7a2a 7c01 6a05 6402 6402 8502 7c01  q.z*|.j.d.d...|.
+00000700: 6a06 a007 7c02 a101 0f00 6602 1900 7d04  j...|.....f...}.
+00000710: 7c04 6a06 a008 a100 7d05 5700 6e1e 0400  |.j.....}.W.n...
+00000720: 7409 6b0a 727e 0100 0100 0100 7c01 6a06  t.k.r~......|.j.
+00000730: a008 a100 7d05 5900 6e02 5800 7c02 7c05  ....}.Y.n.X.|.|.
+00000740: 6602 5300 2903 7a2b 4964 656e 7469 6679  f.S.).z+Identify
+00000750: 2062 6f6f 6c65 616e 2063 6f6c 756d 6e73   boolean columns
+00000760: 2062 6173 6564 206f 6e20 6461 7461 2074   based on data t
+00000770: 7970 65da 0462 6f6f 6c4e 290a da04 6c69  ype..boolN)...li
+00000780: 7374 721a 0000 00da 0661 7374 7970 6572  str......astyper
+00000790: 2300 0000 7212 0000 00da 036c 6f63 721b  #...r......locr.
+000007a0: 0000 00da 0469 7369 6eda 0774 6f5f 6c69  .....isin..to_li
+000007b0: 7374 da09 4578 6365 7074 696f 6e29 0672  st..Exception).r
+000007c0: 1400 0000 7218 0000 00da 0962 6f6f 6c5f  ....r......bool_
+000007d0: 636f 6c73 7220 0000 00da 0a6e 6f5f 626f  colsr .....no_bo
+000007e0: 6f6c 5f64 66da 0c6e 6f5f 626f 6f6c 5f63  ol_df..no_bool_c
+000007f0: 6f6c 7372 1500 0000 7215 0000 0072 1600  olsr....r....r..
+00000800: 0000 da15 6964 656e 7469 6679 5f62 6f6f  ....identify_boo
+00000810: 6c5f 636f 6c75 6d6e 7332 0000 0073 1400  l_columns2...s..
+00000820: 0000 0004 1001 0801 1201 0c03 0201 1c01  ................
+00000830: 0e01 0e01 1001 7a29 4665 6174 7572 6554  ......z)FeatureT
+00000840: 7970 6544 6574 6563 746f 722e 6964 656e  ypeDetector.iden
+00000850: 7469 6679 5f62 6f6f 6c5f 636f 6c75 6d6e  tify_bool_column
+00000860: 7329 0272 1800 0000 722c 0000 0063 0300  s).r....r,...c..
+00000870: 0000 0000 0000 0000 0000 0500 0000 0900  ................
+00000880: 0000 4300 0000 73ea 0000 007c 006a 0072  ..C...s....|.j.r
+00000890: 747c 006a 0172 7467 007d 037c 006a 0044  t|.j.rtg.}.|.j.D
+000008a0: 005d 567d 047c 047c 006a 016b 0772 167a  .]V}.|.|.j.k.r.z
+000008b0: 3274 026a 037c 017c 0419 0064 0164 028d  2t.j.|.|...d.d..
+000008c0: 027c 017c 043c 007c 03a0 047c 04a1 0101  .|.|.<.|...|....
+000008d0: 0064 037c 006a 0574 067c 0483 013c 0057  .d.|.j.t.|...<.W
+000008e0: 0071 1604 0074 076b 0a72 6a01 0001 0001  .q...t.k.rj.....
+000008f0: 0059 0071 1658 0071 167c 037c 005f 007c  .Y.q.X.q.|.|._.|
+00000900: 006a 0073 e67c 006a 0172 e667 007d 037c  .j.s.|.j.r.g.}.|
+00000910: 0244 005d 567d 047c 047c 006a 016b 0772  .D.]V}.|.|.j.k.r
+00000920: 887a 3274 026a 037c 017c 0419 0064 0164  .z2t.j.|.|...d.d
+00000930: 028d 027c 017c 043c 007c 03a0 047c 04a1  ...|.|.<.|...|..
+00000940: 0101 0064 037c 006a 0574 067c 0483 013c  ...d.|.j.t.|...<
+00000950: 0057 0071 8804 0074 076b 0a72 dc01 0001  .W.q...t.k.r....
+00000960: 0001 0059 0071 8858 0071 887c 037c 005f  ...Y.q.X.q.|.|._
+00000970: 0064 0453 0029 057a 4454 7279 2063 6173  .d.S.).zDTry cas
+00000980: 7469 6e67 2074 6f20 6461 7465 7469 6d65  ting to datetime
+00000990: 2e20 4578 7065 6374 6564 2069 7320 6120  . Expected is a 
+000009a0: 6461 7465 7469 6d65 2066 6f72 6d61 7420  datetime format 
+000009b0: 6f66 2059 5959 592d 4d4d 2d44 4454 a901  of YYYY-MM-DDT..
+000009c0: da09 7965 6172 6669 7273 74fa 0c64 6174  ..yearfirst..dat
+000009d0: 6574 696d 655b 6e73 5d4e 2908 720a 0000  etime[ns]N).r...
+000009e0: 0072 0800 0000 da02 7064 da0b 746f 5f64  .r......pd..to_d
+000009f0: 6174 6574 696d 6572 1c00 0000 7212 0000  atetimer....r...
+00000a00: 00da 0373 7472 7229 0000 0029 0572 1400  ...strr)...).r..
+00000a10: 0000 7218 0000 0072 2c00 0000 720a 0000  ..r....r,...r...
+00000a20: 0072 2000 0000 7215 0000 0072 1500 0000  .r ...r....r....
+00000a30: 7216 0000 00da 1a69 6465 6e74 6966 795f  r......identify_
+00000a40: 6461 7465 5f74 696d 655f 636f 6c75 6d6e  date_time_column
+00000a50: 7343 0000 0073 2c00 0000 0004 0c01 0402  sC...s,.........
+00000a60: 0a01 0a01 0201 1601 0a01 1201 0e01 0801  ................
+00000a70: 0601 0c01 0402 0801 0a01 0201 1601 0a01  ................
+00000a80: 1201 0e01 0801 7a2e 4665 6174 7572 6554  ......z.FeatureT
+00000a90: 7970 6544 6574 6563 746f 722e 6964 656e  ypeDetector.iden
+00000aa0: 7469 6679 5f64 6174 655f 7469 6d65 5f63  tify_date_time_c
+00000ab0: 6f6c 756d 6e73 2903 7218 0000 0072 2a00  olumns).r....r*.
+00000ac0: 0000 7222 0000 0063 0300 0000 0000 0000  ..r"...c........
+00000ad0: 0000 0000 0800 0000 0900 0000 4300 0000  ............C...
+00000ae0: 73d6 0000 007c 0272 167c 006a 0072 167c  s....|.r.|.j.r.|
+00000af0: 027c 006a 0017 007d 036e 267c 0272 267c  .|.j...}.n&|.r&|
+00000b00: 006a 0073 267c 027d 036e 167c 0273 387c  .j.s&|.}.n.|.s8|
+00000b10: 006a 0072 387c 006a 007d 036e 0467 007d  .j.r8|.j.}.n.g.}
+00000b20: 037c 016a 0164 0164 0185 027c 016a 02a0  .|.j.d.d...|.j..
+00000b30: 037c 03a1 010f 0066 0219 007d 047c 046a  .|.....f...}.|.j
+00000b40: 02a0 04a1 007d 0567 007d 067c 0544 005d  .....}.g.}.|.D.]
+00000b50: 607d 077a 207c 017c 0719 00a0 0574 06a1  `}.z |.|.....t..
+00000b60: 017c 017c 073c 0064 027c 006a 077c 073c  .|.|.<.d.|.j.|.<
+00000b70: 0057 0071 6a04 0074 086b 0a72 c801 0001  .W.qj..t.k.r....
+00000b80: 0001 007c 017c 0719 00a0 0574 09a1 017c  ...|.|.....t...|
+00000b90: 017c 073c 0064 037c 006a 077c 073c 007c  .|.<.d.|.j.|.<.|
+00000ba0: 06a0 0a7c 07a1 0101 0059 0071 6a58 0071  ...|.....Y.qjX.q
+00000bb0: 6a7c 067c 005f 0b7c 0153 0029 047a ae54  j|.|._.|.S.).z.T
+00000bc0: 7265 6174 2072 656d 6169 6e69 6e67 2063  reat remaining c
+00000bd0: 6f6c 756d 6e73 2e0a 0a20 2020 2020 2020  olumns...       
+00000be0: 2054 616b 6573 2072 656d 6169 6e69 6e67   Takes remaining
+00000bf0: 2063 6f6c 756d 6e73 2061 6e64 2074 7269   columns and tri
+00000c00: 6573 2074 6f20 6361 7374 2074 6865 6d20  es to cast them 
+00000c10: 6173 206e 756d 6572 6963 616c 2e20 4966  as numerical. If
+00000c20: 206e 6f74 2073 7563 6365 7373 6675 6c2c   not successful,
+00000c30: 2074 6865 6e20 636f 6c75 6d6e 7320 6172   then columns ar
+00000c40: 6520 6173 7375 6d65 6420 746f 2062 650a  e assumed to be.
+00000c50: 2020 2020 2020 2020 6361 7465 676f 7269          categori
+00000c60: 6361 6c2e 0a20 2020 2020 2020 204e da05  cal..        N..
+00000c70: 666c 6f61 74da 066f 626a 6563 7429 0c72  float..object).r
+00000c80: 0a00 0000 7226 0000 0072 1b00 0000 7227  ....r&...r....r'
+00000c90: 0000 0072 2800 0000 7225 0000 0072 3500  ...r(...r%...r5.
+00000ca0: 0000 7212 0000 0072 2900 0000 7233 0000  ..r....r)...r3..
+00000cb0: 0072 1c00 0000 7209 0000 0029 0872 1400  .r....r....).r..
+00000cc0: 0000 7218 0000 0072 2a00 0000 da0f 6e6f  ..r....r*.....no
+00000cd0: 5f62 6f6f 6c5f 6474 5f63 6f6c 73da 136e  _bool_dt_cols..n
+00000ce0: 6f5f 626f 6f6c 5f64 6174 6574 696d 655f  o_bool_datetime_
+00000cf0: 6466 da15 6e6f 5f62 6f6f 6c5f 6461 7465  df..no_bool_date
+00000d00: 7469 6d65 5f63 6f6c 7372 0900 0000 7220  time_colsr....r 
+00000d10: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000d20: 0000 da1b 6361 7374 5f72 6573 745f 636f  ....cast_rest_co
+00000d30: 6c75 6d6e 735f 746f 5f6f 626a 6563 7460  lumns_to_object`
+00000d40: 0000 0073 2800 0000 0008 0a01 0c01 0a01  ...s(...........
+00000d50: 0601 0a01 0802 0401 1c01 0a01 0401 0801  ................
+00000d60: 0201 1201 0e01 0e01 1201 0a01 1201 0601  ................
+00000d70: 7a2f 4665 6174 7572 6554 7970 6544 6574  z/FeatureTypeDet
+00000d80: 6563 746f 722e 6361 7374 5f72 6573 745f  ector.cast_rest_
+00000d90: 636f 6c75 6d6e 735f 746f 5f6f 626a 6563  columns_to_objec
+00000da0: 7463 0200 0000 0000 0000 0000 0000 0400  tc..............
+00000db0: 0000 0400 0000 4300 0000 7334 0000 007c  ......C...s4...|
+00000dc0: 00a0 007c 01a1 0101 007c 00a0 017c 01a1  ...|.....|...|..
+00000dd0: 015c 027d 027d 037c 00a0 027c 017c 03a1  .\.}.}.|...|.|..
+00000de0: 0201 007c 00a0 037c 017c 02a1 027d 017c  ...|...|.|...}.|
+00000df0: 0153 0029 017a 7249 6465 6e74 6966 7920  .S.).zrIdentify 
+00000e00: 616e 6420 7472 616e 7366 6f72 6d20 6665  and transform fe
+00000e10: 6174 7572 6520 7479 7065 732e 0a0a 2020  ature types...  
+00000e20: 2020 2020 2020 5772 6170 7065 7220 6675        Wrapper fu
+00000e30: 6e63 7469 6f6e 2074 6f20 6f72 6368 6573  nction to orches
+00000e40: 7465 7220 6469 6666 6572 656e 7420 6465  ter different de
+00000e50: 7465 6374 696f 6e20 6d65 7468 6f64 732e  tection methods.
+00000e60: 0a20 2020 2020 2020 2029 0472 2100 0000  .        ).r!...
+00000e70: 722d 0000 0072 3400 0000 723a 0000 0029  r-...r4...r:...)
+00000e80: 0472 1400 0000 7218 0000 0072 2a00 0000  .r....r....r*...
+00000e90: 722c 0000 0072 1500 0000 7215 0000 0072  r,...r....r....r
+00000ea0: 1600 0000 da1b 6669 745f 7472 616e 7366  ......fit_transf
+00000eb0: 6f72 6d5f 6665 6174 7572 655f 7479 7065  orm_feature_type
+00000ec0: 737e 0000 0073 0a00 0000 0005 0a01 0e01  s~...s..........
+00000ed0: 0c01 0c01 7a2f 4665 6174 7572 6554 7970  ....z/FeatureTyp
+00000ee0: 6544 6574 6563 746f 722e 6669 745f 7472  eDetector.fit_tr
+00000ef0: 616e 7366 6f72 6d5f 6665 6174 7572 655f  ansform_feature_
+00000f00: 7479 7065 7329 0372 1800 0000 da0b 6967  types).r......ig
+00000f10: 6e6f 7265 5f63 6f6c 7372 2200 0000 6303  nore_colsr"...c.
+00000f20: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00000f30: 0000 0043 0000 0073 6400 0000 7c00 6a00  ...C...sd...|.j.
+00000f40: 4400 5d58 7d03 7c02 7206 7c03 7c02 6b07  D.]X}.|.r.|.|.k.
+00000f50: 7206 7c03 7c01 6a01 6b06 7206 7c00 6a00  r.|.|.j.k.r.|.j.
+00000f60: 7c03 1900 6401 6b02 7246 7402 6a03 7c01  |...d.k.rFt.j.|.
+00000f70: 7c03 1900 6402 6403 8d02 7c01 7c03 3c00  |...d.d...|.|.<.
+00000f80: 7106 7c01 7c03 1900 a004 7c00 6a00 7c03  q.|.|.....|.j.|.
+00000f90: 1900 a101 7c01 7c03 3c00 7106 7c01 5300  ....|.|.<.q.|.S.
+00000fa0: 2904 7a36 5472 616e 7366 6f72 6d20 6665  ).z6Transform fe
+00000fb0: 6174 7572 6520 7479 7065 7320 6261 7365  ature types base
+00000fc0: 6420 6f6e 2061 6c72 6561 6479 206d 6170  d on already map
+00000fd0: 7065 6420 7479 7065 732e 7230 0000 0054  ped types.r0...T
+00000fe0: 722e 0000 0029 0572 1200 0000 721b 0000  r....).r....r...
+00000ff0: 0072 3100 0000 7232 0000 0072 2500 0000  .r1...r2...r%...
+00001000: 2904 7214 0000 0072 1800 0000 723c 0000  ).r....r....r<..
+00001010: 00da 036b 6579 7215 0000 0072 1500 0000  ...keyr....r....
+00001020: 7216 0000 00da 1774 7261 6e73 666f 726d  r......transform
+00001030: 5f66 6561 7475 7265 5f74 7970 6573 8900  _feature_types..
+00001040: 0000 730c 0000 0000 080a 0116 010e 0118  ..s.............
+00001050: 021a 017a 2b46 6561 7475 7265 5479 7065  ...z+FeatureType
+00001060: 4465 7465 6374 6f72 2e74 7261 6e73 666f  Detector.transfo
+00001070: 726d 5f66 6561 7475 7265 5f74 7970 6573  rm_feature_types
+00001080: 2903 4e4e 4e29 014e 2914 da08 5f5f 6e61  ).NNN).N)...__na
+00001090: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000010a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+000010b0: 5f5f 646f 635f 5f72 0400 0000 7203 0000  __doc__r....r...
+000010c0: 0072 0600 0000 7233 0000 00da 0369 6e74  .r....r3.....int
+000010d0: 7235 0000 0072 1700 0000 7231 0000 00da  r5...r....r1....
+000010e0: 0944 6174 6146 7261 6d65 7221 0000 0072  .DataFramer!...r
+000010f0: 0500 0000 722d 0000 0072 3400 0000 723a  ....r-...r4...r:
+00001100: 0000 0072 3b00 0000 723e 0000 0072 1500  ...r;...r>...r..
+00001110: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00001120: 0072 0700 0000 0c00 0000 7336 0000 0008  .r........s6....
+00001130: 0104 0700 0100 0100 fc02 0214 0114 0114  ................
+00001140: fc0c 1410 0d04 0126 fe0c 1204 0010 ff0c  .......&........
+00001150: 1e04 0010 0104 fe0c 1e14 0c00 ff02 0104  ................
+00001160: 0012 0104 fe72 0700 0000 290a 7242 0000  .....r....).rB..
+00001170: 00da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
+00001180: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
+00001190: 0000 da06 7061 6e64 6173 7231 0000 0072  ....pandasr1...r
+000011a0: 0700 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
+000011b0: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
+000011c0: 653e 0100 0000 7306 0000 0004 061c 0208  e>....s.........
+000011d0: 03                                       .
```

### Comparing `bluecast-0.2/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-0.3/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 862 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 5e03 0000  o..........d^...
+00000000: 550d 0d0a 0000 0000 f058 8164 5e03 0000  U........X.d^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
+00000020: 0005 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6401 6404 6c06 5a07 6401 6405 6c08  Z.d.d.l.Z.d.d.l.
-00000060: 6d09 5a09 0100 640c 6406 6507 6a0a 6407  m.Z...d.d.e.j.d.
-00000070: 6503 650b 650c 6602 1900 6604 6408 6409  e.e.e.f...f.d.d.
-00000080: 8405 5a0d 640c 6406 6507 6a0a 6407 6503  ..Z.d.d.e.j.d.e.
-00000090: 650b 650c 6602 1900 6604 640a 640b 8405  e.e.f...f.d.d...
-000000a0: 5a0e 6404 5300 290d 7ac6 0a54 6869 7320  Z.d.S.).z..This 
-000000b0: 6d6f 6475 6c65 2063 6f6e 7461 696e 7320  module contains 
-000000c0: 6675 6e63 7469 6f6e 7320 746f 2068 616e  functions to han
-000000d0: 646c 6520 6e75 6c6c 7320 616e 6420 696e  dle nulls and in
-000000e0: 6669 6e69 7465 2076 616c 7565 732e 0a0a  finite values...
-000000f0: 4f6e 6c79 2074 6865 2068 616e 646c 696e  Only the handlin
-00000100: 6720 6f66 2069 6e66 696e 6974 6520 7661  g of infinite va
-00000110: 6c75 6573 2069 7320 7061 7274 206f 6620  lues is part of 
-00000120: 7468 6520 7072 6570 726f 6365 7373 696e  the preprocessin
-00000130: 6720 7069 7065 6c69 6e65 2061 7320 5867  g pipeline as Xg
-00000140: 626f 6f73 7420 6361 6e20 6861 6e64 6c65  boost can handle
-00000150: 206d 6973 7369 6e67 2076 616c 7565 7320   missing values 
-00000160: 6f75 7420 6f66 0a74 6865 2062 6f78 2e0a  out of.the box..
-00000170: e900 0000 0029 01da 0864 6174 6574 696d  .....)...datetim
-00000180: 6529 01da 0555 6e69 6f6e 4e29 01da 066c  e)...UnionN)...l
-00000190: 6f67 6765 72da 0264 66da 0966 696c 6c5f  ogger..df..fill_
-000001a0: 7769 7468 6302 0000 0000 0000 0000 0000  withc...........
-000001b0: 0002 0000 0004 0000 0043 0000 0073 2c00  .........C...s,.
-000001c0: 0000 7400 7401 a002 a100 9b00 6401 9d02  ..t.t.......d...
-000001d0: 8301 0100 7c00 a003 7404 6a05 7404 6a05  ....|...t.j.t.j.
-000001e0: 0b00 6702 7c01 a102 7d00 7c00 5300 2902  ..g.|...}.|.S.).
-000001f0: 7a30 5265 706c 6163 6520 696e 6669 6e69  z0Replace infini
-00000200: 7465 2076 616c 7565 7320 7769 7468 204e  te values with N
-00000210: 614e 206f 7220 6769 7665 6e20 7661 6c75  aN or given valu
-00000220: 652e 7a20 3a20 5374 6172 7420 6669 6c6c  e.z : Start fill
-00000230: 696e 6720 696e 6669 6e69 7465 2076 616c  ing infinite val
-00000240: 7565 732e 2906 7204 0000 0072 0200 0000  ues.).r....r....
-00000250: da06 7574 636e 6f77 da07 7265 706c 6163  ..utcnow..replac
-00000260: 65da 026e 70da 0369 6e66 a902 7205 0000  e..np..inf..r...
-00000270: 0072 0600 0000 a900 720c 0000 00fa 542f  .r......r.....T/
-00000280: 5573 6572 732f 7468 6f6d 6173 6d65 6973  Users/thomasmeis
-00000290: 736e 6572 2f49 6465 6150 726f 6a65 6374  sner/IdeaProject
-000002a0: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
-000002b0: 6173 742f 7072 6570 726f 6365 7373 696e  ast/preprocessin
-000002c0: 672f 6e75 6c6c 735f 616e 645f 696e 6673  g/nulls_and_infs
-000002d0: 2e70 79da 1466 696c 6c5f 696e 6669 6e69  .py..fill_infini
-000002e0: 7465 5f76 616c 7565 7310 0000 0073 0600  te_values....s..
-000002f0: 0000 1202 1601 0401 720e 0000 0063 0200  ........r....c..
-00000300: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000310: 0000 4300 0000 7320 0000 0074 0074 01a0  ..C...s ...t.t..
-00000320: 02a1 009b 0064 019d 0283 0101 007c 00a0  .....d.......|..
-00000330: 037c 01a1 017d 007c 0053 0029 027a 2c52  .|...}.|.S.).z,R
-00000340: 6570 6c61 6365 206e 756c 6c20 7661 6c75  eplace null valu
-00000350: 6573 2077 6974 6820 4e61 4e20 6f72 2067  es with NaN or g
-00000360: 6976 656e 2076 616c 7565 2e7a 1f3a 2053  iven value.z.: S
-00000370: 7461 7274 2066 696c 6c69 6e67 2069 6e66  tart filling inf
-00000380: 696e 6974 6520 6e75 6c6c 732e 2904 7204  inite nulls.).r.
-00000390: 0000 0072 0200 0000 7207 0000 00da 0666  ...r....r......f
-000003a0: 696c 6c6e 6172 0b00 0000 720c 0000 0072  illnar....r....r
-000003b0: 0c00 0000 720d 0000 00da 0a66 696c 6c5f  ....r......fill_
-000003c0: 6e75 6c6c 7317 0000 0073 0600 0000 1202  nulls....s......
-000003d0: 0a01 0401 7210 0000 0029 0172 0100 0000  ....r....).r....
-000003e0: 290f da07 5f5f 646f 635f 5f72 0200 0000  )...__doc__r....
-000003f0: da06 7479 7069 6e67 7203 0000 00da 056e  ..typingr......n
-00000400: 756d 7079 7209 0000 00da 0670 616e 6461  umpyr......panda
-00000410: 73da 0270 64da 2462 6c75 6563 6173 742e  s..pd.$bluecast.
-00000420: 6765 6e65 7261 6c5f 7574 696c 732e 6765  general_utils.ge
-00000430: 6e65 7261 6c5f 7574 696c 7372 0400 0000  neral_utilsr....
-00000440: da09 4461 7461 4672 616d 65da 0369 6e74  ..DataFrame..int
-00000450: da05 666c 6f61 7472 0e00 0000 7210 0000  ..floatr....r...
-00000460: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000470: 720d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000480: 0000 0073 1000 0000 0400 0c06 0c01 0802  ...s............
-00000490: 0801 0c02 1e03 2207                      ......".
+00000060: 6d09 5a09 0100 640b 6507 6a0a 6503 650b  m.Z...d.e.j.e.e.
+00000070: 650c 6602 1900 6406 9c02 6407 6408 8405  e.f...d...d.d...
+00000080: 5a0d 640c 6507 6a0a 6503 650b 650c 6602  Z.d.e.j.e.e.e.f.
+00000090: 1900 6406 9c02 6409 640a 8405 5a0e 6404  ..d...d.d...Z.d.
+000000a0: 5300 290d 7ac6 0a54 6869 7320 6d6f 6475  S.).z..This modu
+000000b0: 6c65 2063 6f6e 7461 696e 7320 6675 6e63  le contains func
+000000c0: 7469 6f6e 7320 746f 2068 616e 646c 6520  tions to handle 
+000000d0: 6e75 6c6c 7320 616e 6420 696e 6669 6e69  nulls and infini
+000000e0: 7465 2076 616c 7565 732e 0a0a 4f6e 6c79  te values...Only
+000000f0: 2074 6865 2068 616e 646c 696e 6720 6f66   the handling of
+00000100: 2069 6e66 696e 6974 6520 7661 6c75 6573   infinite values
+00000110: 2069 7320 7061 7274 206f 6620 7468 6520   is part of the 
+00000120: 7072 6570 726f 6365 7373 696e 6720 7069  preprocessing pi
+00000130: 7065 6c69 6e65 2061 7320 5867 626f 6f73  peline as Xgboos
+00000140: 7420 6361 6e20 6861 6e64 6c65 206d 6973  t can handle mis
+00000150: 7369 6e67 2076 616c 7565 7320 6f75 7420  sing values out 
+00000160: 6f66 0a74 6865 2062 6f78 2e0a e900 0000  of.the box......
+00000170: 0029 01da 0864 6174 6574 696d 6529 01da  .)...datetime)..
+00000180: 0555 6e69 6f6e 4e29 01da 066c 6f67 6765  .UnionN)...logge
+00000190: 72a9 02da 0264 66da 0966 696c 6c5f 7769  r....df..fill_wi
+000001a0: 7468 6302 0000 0000 0000 0000 0000 0002  thc.............
+000001b0: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
+000001c0: 7400 7401 a002 a100 9b00 6401 9d02 8301  t.t.......d.....
+000001d0: 0100 7c00 a003 7404 6a05 7404 6a05 0b00  ..|...t.j.t.j...
+000001e0: 6702 7c01 a102 7d00 7c00 5300 2902 7a30  g.|...}.|.S.).z0
+000001f0: 5265 706c 6163 6520 696e 6669 6e69 7465  Replace infinite
+00000200: 2076 616c 7565 7320 7769 7468 204e 614e   values with NaN
+00000210: 206f 7220 6769 7665 6e20 7661 6c75 652e   or given value.
+00000220: 7a20 3a20 5374 6172 7420 6669 6c6c 696e  z : Start fillin
+00000230: 6720 696e 6669 6e69 7465 2076 616c 7565  g infinite value
+00000240: 732e 2906 7204 0000 0072 0200 0000 da06  s.).r....r......
+00000250: 7574 636e 6f77 da07 7265 706c 6163 65da  utcnow..replace.
+00000260: 026e 70da 0369 6e66 7205 0000 00a9 0072  .np..infr......r
+00000270: 0c00 0000 fa4b 2f68 6f6d 652f 7468 6f6d  .....K/home/thom
+00000280: 6173 2f49 6465 6150 726f 6a65 6374 732f  as/IdeaProjects/
+00000290: 426c 7565 4361 7374 2f62 6c75 6563 6173  BlueCast/bluecas
+000002a0: 742f 7072 6570 726f 6365 7373 696e 672f  t/preprocessing/
+000002b0: 6e75 6c6c 735f 616e 645f 696e 6673 2e70  nulls_and_infs.p
+000002c0: 79da 1466 696c 6c5f 696e 6669 6e69 7465  y..fill_infinite
+000002d0: 5f76 616c 7565 7310 0000 0073 0600 0000  _values....s....
+000002e0: 0002 1201 1601 720e 0000 0063 0200 0000  ......r....c....
+000002f0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000300: 4300 0000 7320 0000 0074 0074 01a0 02a1  C...s ...t.t....
+00000310: 009b 0064 019d 0283 0101 007c 00a0 037c  ...d.......|...|
+00000320: 01a1 017d 007c 0053 0029 027a 2c52 6570  ...}.|.S.).z,Rep
+00000330: 6c61 6365 206e 756c 6c20 7661 6c75 6573  lace null values
+00000340: 2077 6974 6820 4e61 4e20 6f72 2067 6976   with NaN or giv
+00000350: 656e 2076 616c 7565 2e7a 1f3a 2053 7461  en value.z.: Sta
+00000360: 7274 2066 696c 6c69 6e67 2069 6e66 696e  rt filling infin
+00000370: 6974 6520 6e75 6c6c 732e 2904 7204 0000  ite nulls.).r...
+00000380: 0072 0200 0000 7208 0000 00da 0666 696c  .r....r......fil
+00000390: 6c6e 6172 0500 0000 720c 0000 0072 0c00  lnar....r....r..
+000003a0: 0000 720d 0000 00da 0a66 696c 6c5f 6e75  ..r......fill_nu
+000003b0: 6c6c 7317 0000 0073 0600 0000 0002 1201  lls....s........
+000003c0: 0a01 7210 0000 0029 0172 0100 0000 2901  ..r....).r....).
+000003d0: 7201 0000 0029 0fda 075f 5f64 6f63 5f5f  r....)...__doc__
+000003e0: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
+000003f0: 0000 da05 6e75 6d70 7972 0a00 0000 da06  ....numpyr......
+00000400: 7061 6e64 6173 da02 7064 da24 626c 7565  pandas..pd.$blue
+00000410: 6361 7374 2e67 656e 6572 616c 5f75 7469  cast.general_uti
+00000420: 6c73 2e67 656e 6572 616c 5f75 7469 6c73  ls.general_utils
+00000430: 7204 0000 00da 0944 6174 6146 7261 6d65  r......DataFrame
+00000440: da03 696e 74da 0566 6c6f 6174 720e 0000  ..int..floatr...
+00000450: 0072 1000 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000460: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+00000470: 756c 653e 0100 0000 730e 0000 0004 060c  ule>....s.......
+00000480: 010c 0208 0108 020c 031c 07              ...........
```

### Comparing `bluecast-0.2/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-0.3/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 18:43:33 2023 UTC, .py size: 1452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5521 8264 ac05 0000  o.......U!.d....
+00000000: 6f0d 0d0a 0000 0000 ca79 8164 ac05 0000  o........y.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a05 4700 6404 6405  ..d.d.l.Z.G.d.d.
 00000050: 8400 6405 8302 5a06 6403 5300 2906 7a23  ..d...Z.d.S.).z#
 00000060: 4d6f 6475 6c65 2066 6f72 2044 6174 6146  Module for DataF
 00000070: 7261 6d65 2073 6368 656d 6120 6368 6563  rame schema chec
@@ -16,108 +16,107 @@
 000000f0: da0e 5363 6865 6d61 4465 7465 6374 6f72  ..SchemaDetector
 00000100: 7a22 4465 7465 6374 2061 6e64 2063 6865  z"Detect and che
 00000110: 636b 2044 6174 6146 7261 6d65 2073 6368  ck DataFrame sch
 00000120: 656d 612e 6301 0000 0000 0000 0000 0000  ema.c...........
 00000130: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
 00000140: 0000 6700 7c00 5f00 6400 5300 2901 4ea9  ..g.|._.d.S.).N.
 00000150: 01da 0c74 7261 696e 5f73 6368 656d 61a9  ...train_schema.
-00000160: 01da 0473 656c 66a9 0072 0900 0000 fa53  ...self..r.....S
-00000170: 2f55 7365 7273 2f74 686f 6d61 736d 6569  /Users/thomasmei
-00000180: 7373 6e65 722f 4964 6561 5072 6f6a 6563  ssner/IdeaProjec
-00000190: 7473 2f42 6c75 6543 6173 742f 626c 7565  ts/BlueCast/blue
-000001a0: 6361 7374 2f70 7265 7072 6f63 6573 7369  cast/preprocessi
-000001b0: 6e67 2f73 6368 656d 615f 6368 6563 6b73  ng/schema_checks
-000001c0: 2e70 79da 085f 5f69 6e69 745f 5f0a 0000  .py..__init__...
-000001d0: 0073 0200 0000 0a01 7a17 5363 6865 6d61  .s......z.Schema
-000001e0: 4465 7465 6374 6f72 2e5f 5f69 6e69 745f  Detector.__init_
-000001f0: 5fda 0264 6663 0200 0000 0000 0000 0000  _..dfc..........
-00000200: 0000 0200 0000 0200 0000 4300 0000 7312  ..........C...s.
-00000210: 0000 007c 016a 00a0 01a1 007c 005f 027c  ...|.j.....|._.|
-00000220: 006a 0253 0029 017a 2653 746f 7265 2074  .j.S.).z&Store t
-00000230: 6865 2073 6368 656d 6120 6f66 2074 6865  he schema of the
-00000240: 2074 7261 696e 2064 6174 6173 6574 2e29   train dataset.)
-00000250: 03da 0763 6f6c 756d 6e73 da07 746f 5f6c  ...columns..to_l
-00000260: 6973 7472 0600 0000 2902 7208 0000 0072  istr....).r....r
-00000270: 0c00 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
-00000280: 0000 00da 0366 6974 0d00 0000 7304 0000  .....fit....s...
-00000290: 000c 0206 017a 1253 6368 656d 6144 6574  .....z.SchemaDet
-000002a0: 6563 746f 722e 6669 7463 0200 0000 0000  ector.fitc......
-000002b0: 0000 0000 0000 0400 0000 0400 0000 0300  ................
-000002c0: 0000 737a 0000 0074 0088 006a 0183 0174  ..sz...t...j...t
-000002d0: 0088 016a 0283 016b 0472 1c87 0166 0164  ...j...k.r...f.d
-000002e0: 0164 0284 0888 006a 0144 0083 017d 0274  .d.....j.D...}.t
-000002f0: 0364 037c 029b 0064 049d 0383 0182 0174  .d.|...d.......t
-00000300: 0088 006a 0183 0174 0088 016a 0283 016b  ...j...t...j...k
-00000310: 0072 3887 0066 0164 0564 0284 0888 016a  .r8..f.d.d.....j
-00000320: 0244 0083 017d 0374 0364 067c 039b 0064  .D...}.t.d.|...d
-00000330: 049d 0383 0182 0188 0088 016a 0219 0053  ...........j...S
-00000340: 0029 077a ca43 6865 636b 2069 6620 7468  .).z.Check if th
-00000350: 6520 7465 7374 2064 6174 6173 6574 2068  e test dataset h
-00000360: 6173 2074 6865 2073 616d 6520 7363 6865  as the same sche
-00000370: 6d61 2061 7320 7468 6520 7472 6169 6e20  ma as the train 
-00000380: 6461 7461 7365 742e 0a0a 2020 2020 2020  dataset...      
-00000390: 2020 5769 6c6c 2072 6169 7365 2061 6e20    Will raise an 
-000003a0: 6572 726f 7220 6966 2073 6368 656d 6120  error if schema 
-000003b0: 6c65 6e67 7468 2064 6f65 7320 6e6f 7420  length does not 
-000003c0: 6d61 7463 6820 616e 6420 7769 6c6c 2072  match and will r
-000003d0: 6169 7365 2061 2077 6172 6e69 6e67 2069  aise a warning i
-000003e0: 6e64 6963 6174 696e 6720 7468 6520 6d69  ndicating the mi
-000003f0: 7373 696e 6720 6f72 2065 7874 7261 0a20  ssing or extra. 
-00000400: 2020 2020 2020 2063 6f6c 756d 6e73 2e63         columns.c
-00000410: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000420: 0400 0000 1300 0000 f31a 0000 0067 007c  .............g.|
-00000430: 005d 097d 017c 0188 006a 0076 0172 027c  .].}.|...j.v.r.|
-00000440: 0191 0271 0253 0072 0900 0000 7205 0000  ...q.S.r....r...
-00000450: 00a9 02da 022e 30da 0363 6f6c 7207 0000  ......0..colr...
-00000460: 0072 0900 0000 720a 0000 00da 0a3c 6c69  .r....r......<li
-00000470: 7374 636f 6d70 3e18 0000 00f3 0200 0000  stcomp>.........
-00000480: 1a00 7a2c 5363 6865 6d61 4465 7465 6374  ..z,SchemaDetect
-00000490: 6f72 2e74 7261 6e73 666f 726d 2e3c 6c6f  or.transform.<lo
-000004a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000004b0: 7a93 5468 6520 6e75 6d62 6572 206f 6620  z.The number of 
-000004c0: 636f 6c75 6d6e 7320 696e 2074 6865 2074  columns in the t
-000004d0: 6573 7420 6461 7461 7365 7420 6973 2067  est dataset is g
-000004e0: 7265 6174 6572 2074 6861 6e20 7468 6520  reater than the 
-000004f0: 6e75 6d62 6572 206f 6620 636f 6c75 6d6e  number of column
-00000500: 730a 2020 2020 2020 2020 2020 2020 696e  s.            in
-00000510: 2074 6865 2074 7261 696e 2064 6174 6173   the train datas
-00000520: 6574 2e20 466f 756e 6420 7468 6520 666f  et. Found the fo
-00000530: 6c6c 6f77 696e 6720 6e65 7720 636f 6c75  llowing new colu
-00000540: 6d6e 733a 20da 012e 6301 0000 0000 0000  mns: ...c.......
-00000550: 0000 0000 0002 0000 0004 0000 0013 0000  ................
-00000560: 0072 1000 0000 7209 0000 0029 0172 0d00  .r....r....).r..
-00000570: 0000 7211 0000 0029 0172 0c00 0000 7209  ..r....).r....r.
-00000580: 0000 0072 0a00 0000 7214 0000 001e 0000  ...r....r.......
-00000590: 0072 1500 0000 7a91 5468 6520 6e75 6d62  .r....z.The numb
-000005a0: 6572 206f 6620 636f 6c75 6d6e 7320 696e  er of columns in
-000005b0: 2074 6865 2074 6573 7420 6461 7461 7365   the test datase
-000005c0: 7420 6973 2073 6d61 6c6c 6572 2074 6861  t is smaller tha
-000005d0: 6e20 7468 6520 6e75 6d62 6572 206f 6620  n the number of 
-000005e0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-000005f0: 2020 2020 696e 2074 6865 2074 7261 696e      in the train
-00000600: 2064 6174 6173 6574 2e20 4d69 7373 696e   dataset. Missin
-00000610: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
-00000620: 636f 6c75 6d6e 733a 2029 04da 036c 656e  columns: )...len
-00000630: 720d 0000 0072 0600 0000 da0a 5661 6c75  r....r......Valu
-00000640: 6545 7272 6f72 2904 7208 0000 0072 0c00  eError).r....r..
-00000650: 0000 da08 6e65 775f 636f 6c73 da0c 6d69  ....new_cols..mi
-00000660: 7373 696e 675f 636f 6c73 7209 0000 0029  ssing_colsr....)
-00000670: 0272 0c00 0000 7208 0000 0072 0a00 0000  .r....r....r....
-00000680: da09 7472 616e 7366 6f72 6d12 0000 0073  ..transform....s
-00000690: 1e00 0000 1405 1401 0201 0201 0201 06ff  ................
-000006a0: 04ff 1404 1401 0201 0201 0201 06ff 04ff  ................
-000006b0: 0a04 7a18 5363 6865 6d61 4465 7465 6374  ..z.SchemaDetect
-000006c0: 6f72 2e74 7261 6e73 666f 726d 4e29 09da  or.transformN)..
-000006d0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000006e0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000006f0: 655f 5fda 075f 5f64 6f63 5f5f 720b 0000  e__..__doc__r...
-00000700: 00da 0270 64da 0944 6174 6146 7261 6d65  ...pd..DataFrame
-00000710: 720f 0000 0072 1b00 0000 7209 0000 0072  r....r....r....r
-00000720: 0900 0000 7209 0000 0072 0a00 0000 7204  ....r....r....r.
-00000730: 0000 0007 0000 0073 0a00 0000 0800 0401  .......s........
-00000740: 0802 1003 1405 7204 0000 0029 0772 1f00  ......r....).r..
-00000750: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
-00000760: 0300 0000 da06 7061 6e64 6173 7220 0000  ......pandasr ..
-00000770: 0072 0400 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000780: 7209 0000 0072 0a00 0000 da08 3c6d 6f64  r....r......<mod
-00000790: 756c 653e 0100 0000 7308 0000 0004 0010  ule>....s.......
-000007a0: 0108 0212 03                             .....
+00000160: 01da 0473 656c 66a9 0072 0900 0000 fa4a  ...self..r.....J
+00000170: 2f68 6f6d 652f 7468 6f6d 6173 2f49 6465  /home/thomas/Ide
+00000180: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
+00000190: 7374 2f62 6c75 6563 6173 742f 7072 6570  st/bluecast/prep
+000001a0: 726f 6365 7373 696e 672f 7363 6865 6d61  rocessing/schema
+000001b0: 5f63 6865 636b 732e 7079 da08 5f5f 696e  _checks.py..__in
+000001c0: 6974 5f5f 0a00 0000 7302 0000 000a 017a  it__....s......z
+000001d0: 1753 6368 656d 6144 6574 6563 746f 722e  .SchemaDetector.
+000001e0: 5f5f 696e 6974 5f5f da02 6466 6302 0000  __init__..dfc...
+000001f0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000200: 0043 0000 0073 1200 0000 7c01 6a00 a001  .C...s....|.j...
+00000210: a100 7c00 5f02 7c00 6a02 5300 2901 7a26  ..|._.|.j.S.).z&
+00000220: 5374 6f72 6520 7468 6520 7363 6865 6d61  Store the schema
+00000230: 206f 6620 7468 6520 7472 6169 6e20 6461   of the train da
+00000240: 7461 7365 742e 2903 da07 636f 6c75 6d6e  taset.)...column
+00000250: 73da 0774 6f5f 6c69 7374 7206 0000 0029  s..to_listr....)
+00000260: 0272 0800 0000 720c 0000 0072 0900 0000  .r....r....r....
+00000270: 7209 0000 0072 0a00 0000 da03 6669 740d  r....r......fit.
+00000280: 0000 0073 0400 0000 0c02 0601 7a12 5363  ...s........z.Sc
+00000290: 6865 6d61 4465 7465 6374 6f72 2e66 6974  hemaDetector.fit
+000002a0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+000002b0: 0004 0000 0003 0000 0073 7a00 0000 7400  .........sz...t.
+000002c0: 8800 6a01 8301 7400 8801 6a02 8301 6b04  ..j...t...j...k.
+000002d0: 721c 8701 6601 6401 6402 8408 8800 6a01  r...f.d.d.....j.
+000002e0: 4400 8301 7d02 7403 6403 7c02 9b00 6404  D...}.t.d.|...d.
+000002f0: 9d03 8301 8201 7400 8800 6a01 8301 7400  ......t...j...t.
+00000300: 8801 6a02 8301 6b00 7238 8700 6601 6405  ..j...k.r8..f.d.
+00000310: 6402 8408 8801 6a02 4400 8301 7d03 7403  d.....j.D...}.t.
+00000320: 6406 7c03 9b00 6404 9d03 8301 8201 8800  d.|...d.........
+00000330: 8801 6a02 1900 5300 2907 7aca 4368 6563  ..j...S.).z.Chec
+00000340: 6b20 6966 2074 6865 2074 6573 7420 6461  k if the test da
+00000350: 7461 7365 7420 6861 7320 7468 6520 7361  taset has the sa
+00000360: 6d65 2073 6368 656d 6120 6173 2074 6865  me schema as the
+00000370: 2074 7261 696e 2064 6174 6173 6574 2e0a   train dataset..
+00000380: 0a20 2020 2020 2020 2057 696c 6c20 7261  .        Will ra
+00000390: 6973 6520 616e 2065 7272 6f72 2069 6620  ise an error if 
+000003a0: 7363 6865 6d61 206c 656e 6774 6820 646f  schema length do
+000003b0: 6573 206e 6f74 206d 6174 6368 2061 6e64  es not match and
+000003c0: 2077 696c 6c20 7261 6973 6520 6120 7761   will raise a wa
+000003d0: 726e 696e 6720 696e 6469 6361 7469 6e67  rning indicating
+000003e0: 2074 6865 206d 6973 7369 6e67 206f 7220   the missing or 
+000003f0: 6578 7472 610a 2020 2020 2020 2020 636f  extra.        co
+00000400: 6c75 6d6e 732e 6301 0000 0000 0000 0000  lumns.c.........
+00000410: 0000 0002 0000 0004 0000 0013 0000 00f3  ................
+00000420: 1a00 0000 6700 7c00 5d09 7d01 7c01 8800  ....g.|.].}.|...
+00000430: 6a00 7601 7202 7c01 9102 7102 5300 7209  j.v.r.|...q.S.r.
+00000440: 0000 0072 0500 0000 a902 da02 2e30 da03  ...r.........0..
+00000450: 636f 6c72 0700 0000 7209 0000 0072 0a00  colr....r....r..
+00000460: 0000 da0a 3c6c 6973 7463 6f6d 703e 1800  ....<listcomp>..
+00000470: 0000 f302 0000 001a 007a 2c53 6368 656d  .........z,Schem
+00000480: 6144 6574 6563 746f 722e 7472 616e 7366  aDetector.transf
+00000490: 6f72 6d2e 3c6c 6f63 616c 733e 2e3c 6c69  orm.<locals>.<li
+000004a0: 7374 636f 6d70 3e7a 9354 6865 206e 756d  stcomp>z.The num
+000004b0: 6265 7220 6f66 2063 6f6c 756d 6e73 2069  ber of columns i
+000004c0: 6e20 7468 6520 7465 7374 2064 6174 6173  n the test datas
+000004d0: 6574 2069 7320 6772 6561 7465 7220 7468  et is greater th
+000004e0: 616e 2074 6865 206e 756d 6265 7220 6f66  an the number of
+000004f0: 2063 6f6c 756d 6e73 0a20 2020 2020 2020   columns.       
+00000500: 2020 2020 2069 6e20 7468 6520 7472 6169       in the trai
+00000510: 6e20 6461 7461 7365 742e 2046 6f75 6e64  n dataset. Found
+00000520: 2074 6865 2066 6f6c 6c6f 7769 6e67 206e   the following n
+00000530: 6577 2063 6f6c 756d 6e73 3a20 da01 2e63  ew columns: ...c
+00000540: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000550: 0400 0000 1300 0000 7210 0000 0072 0900  ........r....r..
+00000560: 0000 2901 720d 0000 0072 1100 0000 2901  ..).r....r....).
+00000570: 720c 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000580: 1400 0000 1e00 0000 7215 0000 007a 9154  ........r....z.T
+00000590: 6865 206e 756d 6265 7220 6f66 2063 6f6c  he number of col
+000005a0: 756d 6e73 2069 6e20 7468 6520 7465 7374  umns in the test
+000005b0: 2064 6174 6173 6574 2069 7320 736d 616c   dataset is smal
+000005c0: 6c65 7220 7468 616e 2074 6865 206e 756d  ler than the num
+000005d0: 6265 7220 6f66 2063 6f6c 756d 6e73 0a20  ber of columns. 
+000005e0: 2020 2020 2020 2020 2020 2069 6e20 7468             in th
+000005f0: 6520 7472 6169 6e20 6461 7461 7365 742e  e train dataset.
+00000600: 204d 6973 7369 6e67 2074 6865 2066 6f6c   Missing the fol
+00000610: 6c6f 7769 6e67 2063 6f6c 756d 6e73 3a20  lowing columns: 
+00000620: 2904 da03 6c65 6e72 0d00 0000 7206 0000  )...lenr....r...
+00000630: 00da 0a56 616c 7565 4572 726f 7229 0472  ...ValueError).r
+00000640: 0800 0000 720c 0000 00da 086e 6577 5f63  ....r......new_c
+00000650: 6f6c 73da 0c6d 6973 7369 6e67 5f63 6f6c  ols..missing_col
+00000660: 7372 0900 0000 2902 720c 0000 0072 0800  sr....).r....r..
+00000670: 0000 720a 0000 00da 0974 7261 6e73 666f  ..r......transfo
+00000680: 726d 1200 0000 731e 0000 0014 0514 0102  rm....s.........
+00000690: 0102 0102 0106 ff04 ff14 0414 0102 0102  ................
+000006a0: 0102 0106 ff04 ff0a 047a 1853 6368 656d  .........z.Schem
+000006b0: 6144 6574 6563 746f 722e 7472 616e 7366  aDetector.transf
+000006c0: 6f72 6d4e 2909 da08 5f5f 6e61 6d65 5f5f  ormN)...__name__
+000006d0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000006e0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+000006f0: 635f 5f72 0b00 0000 da02 7064 da09 4461  c__r......pd..Da
+00000700: 7461 4672 616d 6572 0f00 0000 721b 0000  taFramer....r...
+00000710: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000720: 720a 0000 0072 0400 0000 0700 0000 730a  r....r........s.
+00000730: 0000 0008 0004 0108 0210 0314 0572 0400  .............r..
+00000740: 0000 2907 721f 0000 00da 0674 7970 696e  ..).r......typin
+00000750: 6772 0200 0000 7203 0000 00da 0670 616e  gr....r......pan
+00000760: 6461 7372 2000 0000 7204 0000 0072 0900  dasr ...r....r..
+00000770: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000780: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000790: 0800 0000 0400 1001 0802 1203            ............
```

### Comparing `bluecast-0.2/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-0.3/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 4561 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 d111 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 f058 8164 d111 0000  o........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 0100 6401  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 4700 6407 6408  d.l.m.Z...G.d.d.
@@ -87,223 +87,223 @@
 00000560: 6e73 6302 0000 0000 0000 0000 0000 0002  nsc.............
 00000570: 0000 0002 0000 0043 0000 0073 1600 0000  .......C...s....
 00000580: 6900 7c00 5f00 6401 7c00 5f01 7c01 7c00  i.|._.d.|._.|.|.
 00000590: 5f02 6400 5300 a902 4e46 2903 da08 656e  _.d.S...NF)...en
 000005a0: 636f 6465 7273 da0f 7072 6564 6963 7469  coders..predicti
 000005b0: 6f6e 5f6d 6f64 6572 0c00 0000 a902 da04  on_moder........
 000005c0: 7365 6c66 720c 0000 00a9 0072 1200 0000  selfr......r....
-000005d0: fa55 2f55 7365 7273 2f74 686f 6d61 736d  .U/Users/thomasm
-000005e0: 6569 7373 6e65 722f 4964 6561 5072 6f6a  eissner/IdeaProj
-000005f0: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
-00000600: 7565 6361 7374 2f70 7265 7072 6f63 6573  uecast/preproces
-00000610: 7369 6e67 2f74 6172 6765 745f 656e 636f  sing/target_enco
-00000620: 6469 6e67 2e70 79da 085f 5f69 6e69 745f  ding.py..__init_
-00000630: 5f19 0000 0073 0600 0000 0601 0601 0a01  _....s..........
-00000640: 7a21 4269 6e61 7279 436c 6173 7354 6172  z!BinaryClassTar
-00000650: 6765 7445 6e63 6f64 6572 2e5f 5f69 6e69  getEncoder.__ini
-00000660: 745f 5fda 0178 da01 79da 0672 6574 7572  t__..x..y..retur
-00000670: 6e63 0300 0000 0000 0000 0000 0000 0400  nc..............
-00000680: 0000 0400 0000 4300 0000 7344 0000 0074  ......C...sD...t
-00000690: 0074 01a0 02a1 009b 0064 019d 0283 0101  .t.......d......
-000006a0: 0074 037c 006a 0464 028d 017d 037c 03a0  .t.|.j.d...}.|..
-000006b0: 057c 017c 006a 0419 007c 02a1 027c 017c  .|.|.j...|...|.|
-000006c0: 006a 043c 007c 037c 006a 0664 033c 007c  .j.<.|.|.j.d.<.|
-000006d0: 0153 0029 04fa 2846 6974 2074 6172 6765  .S.)..(Fit targe
-000006e0: 7420 656e 636f 6465 7220 616e 6420 7472  t encoder and tr
-000006f0: 616e 7366 6f72 6d20 636f 6c75 6d6e 2e7a  ansform column.z
-00000700: 263a 2053 7461 7274 2066 6974 7469 6e67  &: Start fitting
-00000710: 2062 696e 6172 7920 7461 7267 6574 2065   binary target e
-00000720: 6e63 6f64 6572 2e29 01da 0463 6f6c 73da  ncoder.)...cols.
-00000730: 1774 6172 6765 745f 656e 636f 6465 725f  .target_encoder_
-00000740: 616c 6c5f 636f 6c73 2907 7209 0000 0072  all_cols).r....r
-00000750: 0200 0000 da06 7574 636e 6f77 7208 0000  ......utcnowr...
-00000760: 0072 0c00 0000 da0d 6669 745f 7472 616e  .r......fit_tran
-00000770: 7366 6f72 6d72 0e00 0000 2904 7211 0000  sformr....).r...
-00000780: 0072 1500 0000 7216 0000 00da 0365 6e63  .r....r......enc
-00000790: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-000007a0: 1e66 6974 5f74 6172 6765 745f 656e 636f  .fit_target_enco
-000007b0: 6465 5f62 696e 6172 795f 636c 6173 731e  de_binary_class.
-000007c0: 0000 0073 0a00 0000 1204 0c01 1801 0a01  ...s............
-000007d0: 0401 7a37 4269 6e61 7279 436c 6173 7354  ..z7BinaryClassT
-000007e0: 6172 6765 7445 6e63 6f64 6572 2e66 6974  argetEncoder.fit
-000007f0: 5f74 6172 6765 745f 656e 636f 6465 5f62  _target_encode_b
-00000800: 696e 6172 795f 636c 6173 7363 0200 0000  inary_classc....
-00000810: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000820: 4300 0000 7336 0000 0074 0074 01a0 02a1  C...s6...t.t....
-00000830: 009b 0064 019d 0283 0101 007c 006a 0364  ...d.......|.j.d
-00000840: 0219 007d 027c 02a0 047c 017c 006a 0519  ...}.|...|.|.j..
-00000850: 00a1 017c 017c 006a 053c 007c 0153 0029  ...|.|.j.<.|.S.)
-00000860: 03fa 3654 7261 6e73 666f 726d 2063 6174  ..6Transform cat
-00000870: 6567 6f72 6965 7320 6261 7365 6420 6f6e  egories based on
-00000880: 2061 6c72 6561 6479 2074 7261 696e 6564   already trained
-00000890: 2065 6e63 6f64 6572 2e7a 3b3a 2053 7461   encoder.z;: Sta
-000008a0: 7274 2074 7261 6e73 666f 726d 696e 6720  rt transforming 
-000008b0: 6361 7465 676f 7269 6573 2077 6974 6820  categories with 
-000008c0: 6269 6e61 7279 2074 6172 6765 7420 656e  binary target en
-000008d0: 636f 6465 722e 721a 0000 0029 0672 0900  coder.r....).r..
-000008e0: 0000 7202 0000 0072 1b00 0000 720e 0000  ..r....r....r...
-000008f0: 00da 0974 7261 6e73 666f 726d 720c 0000  ...transformr...
-00000900: 0029 0372 1100 0000 7215 0000 0072 1d00  .).r....r....r..
-00000910: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000920: 00da 2474 7261 6e73 666f 726d 5f74 6172  ..$transform_tar
-00000930: 6765 745f 656e 636f 6465 5f62 696e 6172  get_encode_binar
-00000940: 795f 636c 6173 7328 0000 0073 0c00 0000  y_class(...s....
-00000950: 0202 0c01 04ff 0a03 1601 0401 7a3d 4269  ............z=Bi
-00000960: 6e61 7279 436c 6173 7354 6172 6765 7445  naryClassTargetE
-00000970: 6e63 6f64 6572 2e74 7261 6e73 666f 726d  ncoder.transform
-00000980: 5f74 6172 6765 745f 656e 636f 6465 5f62  _target_encode_b
-00000990: 696e 6172 795f 636c 6173 734e 290f da08  inary_classN)...
-000009a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000009b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000009c0: 5f5f da07 5f5f 646f 635f 5f72 0400 0000  __..__doc__r....
-000009d0: 7206 0000 00da 0373 7472 da05 666c 6f61  r......str..floa
-000009e0: 74da 0369 6e74 7214 0000 00da 0270 64da  t..intr......pd.
-000009f0: 0944 6174 6146 7261 6d65 da06 5365 7269  .DataFrame..Seri
-00000a00: 6573 721e 0000 0072 2100 0000 7212 0000  esr....r!...r...
-00000a10: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000a20: 720b 0000 0016 0000 0073 1600 0000 0800  r........s......
-00000a30: 0401 1c02 0205 0401 02ff 0401 02ff 0402  ................
-00000a40: 0afe 1a0a 720b 0000 0063 0000 0000 0000  ....r....c......
-00000a50: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
-00000a60: 0000 720a 0000 0029 0dda 174d 756c 7469  ..r....)...Multi
-00000a70: 436c 6173 7354 6172 6765 7445 6e63 6f64  ClassTargetEncod
-00000a80: 6572 7a4f 5461 7267 6574 2065 6e63 6f64  erzOTarget encod
-00000a90: 6520 6361 7465 676f 7269 6361 6c20 6665  e categorical fe
-00000aa0: 6174 7572 6573 2069 6e20 7468 6520 636f  atures in the co
-00000ab0: 6e74 6578 7420 6f66 206d 756c 7469 636c  ntext of multicl
-00000ac0: 6173 7320 636c 6173 7369 6669 6361 7469  ass classificati
-00000ad0: 6f6e 2e72 0c00 0000 6302 0000 0000 0000  on.r....c.......
-00000ae0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00000af0: 0073 1c00 0000 6900 7c00 5f00 6401 7c00  .s....i.|._.d.|.
-00000b00: 5f01 7c01 7c00 5f02 6700 7c00 5f03 6400  _.|.|._.g.|._.d.
-00000b10: 5300 720d 0000 0029 0472 0e00 0000 720f  S.r....).r....r.
-00000b20: 0000 0072 0c00 0000 da0b 636c 6173 735f  ...r......class_
-00000b30: 6e61 6d65 7372 1000 0000 7212 0000 0072  namesr....r....r
-00000b40: 1200 0000 7213 0000 0072 1400 0000 3500  ....r....r....5.
-00000b50: 0000 7308 0000 0006 0106 0106 010a 017a  ..s............z
-00000b60: 204d 756c 7469 436c 6173 7354 6172 6765   MultiClassTarge
-00000b70: 7445 6e63 6f64 6572 2e5f 5f69 6e69 745f  tEncoder.__init_
-00000b80: 5f72 1500 0000 7216 0000 0072 1700 0000  _r....r....r....
-00000b90: 6303 0000 0000 0000 0000 0000 0009 0000  c...............
-00000ba0: 0006 0000 0003 0000 0073 ea00 0000 7400  .........s....t.
-00000bb0: 7401 a002 a100 9b00 6401 9d02 8301 0100  t.......d.......
-00000bc0: 6402 7d03 7403 8300 7d04 7c04 a004 7c02  d.}.t...}.|...|.
-00000bd0: a101 0100 7c04 a005 7c02 a101 7d05 7c05  ....|...|...}.|.
-00000be0: 6a06 a007 a100 7c00 5f08 7c01 6a09 6403  j.....|._.|.j.d.
-00000bf0: 6403 8502 7c00 6a0a 6602 1900 a00b a100  d...|.j.f.......
-00000c00: 7d06 7c01 6a09 6403 6403 8502 7c01 6a06  }.|.j.d.d...|.j.
-00000c10: a00c 7c00 6a0a a101 0f00 6602 1900 7d01  ..|.j.....f...}.
-00000c20: 7c00 6a08 4400 5d2e 8900 740d 8300 7d07  |.j.D.]...t...}.
-00000c30: 7c07 a004 7c06 7c05 8800 1900 a102 0100  |...|.|.........
-00000c40: 7c07 7c00 6a0e 6404 8800 9b00 9d02 3c00  |.|.j.d.......<.
-00000c50: 7c07 a005 7c06 a101 7d08 8700 6601 6405  |...|...}...f.d.
-00000c60: 6406 8408 7c08 6a06 4400 8301 7c08 5f06  d...|.j.D...|._.
-00000c70: 740f 6a10 7c01 7c08 6702 6407 6408 8d02  t.j.|.|.g.d.d...
-00000c80: 7d01 713c 7c04 7c00 6a0e 7c03 9b00 6409  }.q<|.|.j.|...d.
-00000c90: 9d02 3c00 7c01 5300 290a 7218 0000 007a  ..<.|.S.).r....z
-00000ca0: 2a3a 2053 7461 7274 2066 6974 7469 6e67  *: Start fitting
-00000cb0: 206d 756c 7469 636c 6173 7320 7461 7267   multiclass targ
-00000cc0: 6574 2065 6e63 6f64 6572 2eda 246d 756c  et encoder..$mul
-00000cd0: 7469 636c 6173 735f 7461 7267 6574 5f65  ticlass_target_e
-00000ce0: 6e63 6f64 696e 675f 6f6e 6568 6f74 7465  ncoding_onehotte
-00000cf0: 724e da23 6d75 6c74 6963 6c61 7373 5f74  rN.#multiclass_t
-00000d00: 6172 6765 745f 656e 636f 6465 725f 616c  arget_encoder_al
-00000d10: 6c5f 636f 6c73 5f63 0100 0000 0000 0000  l_cols_c........
-00000d20: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-00000d30: f320 0000 0067 007c 005d 0c7d 0174 007c  . ...g.|.].}.t.|
-00000d40: 0183 0164 0017 0074 0088 0083 0117 0091  ...d...t........
-00000d50: 0271 0253 00a9 01da 015f a901 7226 0000  .q.S....._..r&..
-00000d60: 00a9 02da 022e 3072 1500 0000 a901 da06  ......0r........
-00000d70: 636c 6173 735f 7212 0000 0072 1300 0000  class_r....r....
-00000d80: da0a 3c6c 6973 7463 6f6d 703e 4c00 0000  ..<listcomp>L...
-00000d90: f302 0000 0020 007a 484d 756c 7469 436c  ..... .zHMultiCl
-00000da0: 6173 7354 6172 6765 7445 6e63 6f64 6572  assTargetEncoder
-00000db0: 2e66 6974 5f74 6172 6765 745f 656e 636f  .fit_target_enco
-00000dc0: 6465 5f6d 756c 7469 636c 6173 732e 3c6c  de_multiclass.<l
-00000dd0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000de0: 3ee9 0100 0000 a901 da04 6178 6973 da09  >.........axis..
-00000df0: 5f61 6c6c 5f63 6f6c 7329 1172 0900 0000  _all_cols).r....
-00000e00: 7202 0000 0072 1b00 0000 7207 0000 00da  r....r....r.....
-00000e10: 0366 6974 7220 0000 00da 0763 6f6c 756d  .fitr .....colum
-00000e20: 6e73 da07 746f 5f6c 6973 7472 2d00 0000  ns..to_listr-...
-00000e30: da03 6c6f 6372 0c00 0000 da04 636f 7079  ..locr......copy
-00000e40: da04 6973 696e 7208 0000 0072 0e00 0000  ..isinr....r....
-00000e50: 7229 0000 00da 0663 6f6e 6361 7429 0972  r).....concat).r
-00000e60: 1100 0000 7215 0000 0072 1600 0000 da09  ....r....r......
-00000e70: 616c 676f 7269 7468 6d72 1d00 0000 5a08  algorithmr....Z.
-00000e80: 795f 6f6e 6568 6f74 da05 785f 6f62 6ada  y_onehot..x_obj.
-00000e90: 0a74 6172 6765 745f 656e 63da 0474 656d  .target_enc..tem
-00000ea0: 7072 1200 0000 7236 0000 0072 1300 0000  pr....r6...r....
-00000eb0: da1c 6669 745f 7461 7267 6574 5f65 6e63  ..fit_target_enc
-00000ec0: 6f64 655f 6d75 6c74 6963 6c61 7373 3b00  ode_multiclass;.
-00000ed0: 0000 7322 0000 0012 0404 0106 010a 010a  ..s"............
-00000ee0: 010c 0118 011e 010a 0106 0110 0110 010a  ................
-00000ef0: 0116 0114 0110 0104 017a 344d 756c 7469  .........z4Multi
-00000f00: 436c 6173 7354 6172 6765 7445 6e63 6f64  ClassTargetEncod
-00000f10: 6572 2e66 6974 5f74 6172 6765 745f 656e  er.fit_target_en
-00000f20: 636f 6465 5f6d 756c 7469 636c 6173 7363  code_multiclassc
-00000f30: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-00000f40: 0500 0000 0300 0000 73be 0000 0074 0074  ........s....t.t
-00000f50: 01a0 02a1 009b 0064 019d 0283 0101 0064  .......d.......d
-00000f60: 027d 027c 006a 037c 029b 0064 039d 0219  .}.|.j.|...d....
-00000f70: 007d 037c 016a 0464 0464 0485 027c 006a  .}.|.j.d.d...|.j
-00000f80: 0566 0219 00a0 06a1 007d 047c 016a 0464  .f.......}.|.j.d
-00000f90: 0464 0485 027c 016a 07a0 087c 006a 05a1  .d...|.j...|.j..
-00000fa0: 010f 0066 0219 007d 017c 006a 0944 005d  ...f...}.|.j.D.]
-00000fb0: 2389 007c 006a 0364 0588 009b 009d 0219  #..|.j.d........
-00000fc0: 007d 057c 05a0 0a7c 04a1 017d 0687 0066  .}.|...|...}...f
-00000fd0: 0164 0664 0784 087c 066a 0744 0083 017c  .d.d...|.j.D...|
-00000fe0: 065f 0774 0b6a 0c7c 017c 0667 0264 0864  ._.t.j.|.|.g.d.d
-00000ff0: 098d 027d 0171 317c 037c 006a 037c 029b  ...}.q1|.|.j.|..
-00001000: 0064 039d 023c 007c 0153 0029 0a72 1f00  .d...<.|.S.).r..
-00001010: 0000 7a3f 3a20 5374 6172 7420 7472 616e  ..z?: Start tran
-00001020: 7366 6f72 6d69 6e67 2063 6174 6567 6f72  sforming categor
-00001030: 6965 7320 7769 7468 206d 756c 7469 636c  ies with multicl
-00001040: 6173 7320 7461 7267 6574 2065 6e63 6f64  ass target encod
-00001050: 6572 2e72 2e00 0000 723d 0000 004e 722f  er.r....r=...Nr/
-00001060: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001070: 0200 0000 0500 0000 1300 0000 7230 0000  ............r0..
-00001080: 0072 3100 0000 7233 0000 0072 3400 0000  .r1...r3...r4...
-00001090: 7236 0000 0072 1200 0000 7213 0000 0072  r6...r....r....r
-000010a0: 3800 0000 5d00 0000 7239 0000 007a 4e4d  8...]...r9...zNM
-000010b0: 756c 7469 436c 6173 7354 6172 6765 7445  ultiClassTargetE
-000010c0: 6e63 6f64 6572 2e74 7261 6e73 666f 726d  ncoder.transform
-000010d0: 5f74 6172 6765 745f 656e 636f 6465 5f6d  _target_encode_m
-000010e0: 756c 7469 636c 6173 732e 3c6c 6f63 616c  ulticlass.<local
-000010f0: 733e 2e3c 6c69 7374 636f 6d70 3e72 3a00  s>.<listcomp>r:.
-00001100: 0000 723b 0000 0029 0d72 0900 0000 7202  ..r;...).r....r.
-00001110: 0000 0072 1b00 0000 720e 0000 0072 4100  ...r....r....rA.
-00001120: 0000 720c 0000 0072 4200 0000 723f 0000  ..r....rB...r?..
-00001130: 0072 4300 0000 722d 0000 0072 2000 0000  .rC...r-...r ...
-00001140: 7229 0000 0072 4400 0000 2907 7211 0000  r)...rD...).r...
-00001150: 0072 1500 0000 7245 0000 0072 1d00 0000  .r....rE...r....
-00001160: 7246 0000 0072 4700 0000 7248 0000 0072  rF...rG...rH...r
-00001170: 1200 0000 7236 0000 0072 1300 0000 da22  ....r6...r....."
-00001180: 7472 616e 7366 6f72 6d5f 7461 7267 6574  transform_target
-00001190: 5f65 6e63 6f64 655f 6d75 6c74 6963 6c61  _encode_multicla
-000011a0: 7373 5100 0000 731c 0000 0002 020c 0104  ssQ...s.........
-000011b0: ff04 0310 0118 011e 010a 0110 010a 0116  ................
-000011c0: 0114 0110 0104 017a 3a4d 756c 7469 436c  .......z:MultiCl
-000011d0: 6173 7354 6172 6765 7445 6e63 6f64 6572  assTargetEncoder
-000011e0: 2e74 7261 6e73 666f 726d 5f74 6172 6765  .transform_targe
-000011f0: 745f 656e 636f 6465 5f6d 756c 7469 636c  t_encode_multicl
-00001200: 6173 734e 290f 7222 0000 0072 2300 0000  assN).r"...r#...
-00001210: 7224 0000 0072 2500 0000 7204 0000 0072  r$...r%...r....r
-00001220: 0600 0000 7226 0000 0072 2700 0000 7228  ....r&...r'...r(
-00001230: 0000 0072 1400 0000 7229 0000 0072 2a00  ...r....r)...r*.
-00001240: 0000 722b 0000 0072 4900 0000 724a 0000  ..r+...rI...rJ..
-00001250: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00001260: 7213 0000 0072 2c00 0000 3200 0000 7316  r....r,...2...s.
-00001270: 0000 0008 0004 011c 0202 0604 0102 ff04  ................
-00001280: 0102 ff04 020a fe1a 1672 2c00 0000 2910  .........r,...).
-00001290: 7225 0000 0072 0200 0000 da06 7479 7069  r%...r......typi
-000012a0: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
-000012b0: 0072 0600 0000 da06 7061 6e64 6173 7229  .r......pandasr)
-000012c0: 0000 005a 1163 6174 6567 6f72 795f 656e  ...Z.category_en
-000012d0: 636f 6465 7273 7207 0000 0072 0800 0000  codersr....r....
-000012e0: da24 626c 7565 6361 7374 2e67 656e 6572  .$bluecast.gener
-000012f0: 616c 5f75 7469 6c73 2e67 656e 6572 616c  al_utils.general
-00001300: 5f75 7469 6c73 7209 0000 0072 0b00 0000  _utilsr....r....
-00001310: 722c 0000 0072 1200 0000 7212 0000 0072  r,...r....r....r
-00001320: 1200 0000 7213 0000 00da 083c 6d6f 6475  ....r......<modu
-00001330: 6c65 3e01 0000 0073 1000 0000 0400 0c0c  le>....s........
-00001340: 1801 0802 1001 0c02 0e03 121c            ............
+000005d0: fa4c 2f68 6f6d 652f 7468 6f6d 6173 2f49  .L/home/thomas/I
+000005e0: 6465 6150 726f 6a65 6374 732f 426c 7565  deaProjects/Blue
+000005f0: 4361 7374 2f62 6c75 6563 6173 742f 7072  Cast/bluecast/pr
+00000600: 6570 726f 6365 7373 696e 672f 7461 7267  eprocessing/targ
+00000610: 6574 5f65 6e63 6f64 696e 672e 7079 da08  et_encoding.py..
+00000620: 5f5f 696e 6974 5f5f 1900 0000 7306 0000  __init__....s...
+00000630: 0006 0106 010a 017a 2142 696e 6172 7943  .......z!BinaryC
+00000640: 6c61 7373 5461 7267 6574 456e 636f 6465  lassTargetEncode
+00000650: 722e 5f5f 696e 6974 5f5f da01 78da 0179  r.__init__..x..y
+00000660: da06 7265 7475 726e 6303 0000 0000 0000  ..returnc.......
+00000670: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+00000680: 0073 4400 0000 7400 7401 a002 a100 9b00  .sD...t.t.......
+00000690: 6401 9d02 8301 0100 7403 7c00 6a04 6402  d.......t.|.j.d.
+000006a0: 8d01 7d03 7c03 a005 7c01 7c00 6a04 1900  ..}.|...|.|.j...
+000006b0: 7c02 a102 7c01 7c00 6a04 3c00 7c03 7c00  |...|.|.j.<.|.|.
+000006c0: 6a06 6403 3c00 7c01 5300 2904 fa28 4669  j.d.<.|.S.)..(Fi
+000006d0: 7420 7461 7267 6574 2065 6e63 6f64 6572  t target encoder
+000006e0: 2061 6e64 2074 7261 6e73 666f 726d 2063   and transform c
+000006f0: 6f6c 756d 6e2e 7a26 3a20 5374 6172 7420  olumn.z&: Start 
+00000700: 6669 7474 696e 6720 6269 6e61 7279 2074  fitting binary t
+00000710: 6172 6765 7420 656e 636f 6465 722e 2901  arget encoder.).
+00000720: da04 636f 6c73 da17 7461 7267 6574 5f65  ..cols..target_e
+00000730: 6e63 6f64 6572 5f61 6c6c 5f63 6f6c 7329  ncoder_all_cols)
+00000740: 0772 0900 0000 7202 0000 00da 0675 7463  .r....r......utc
+00000750: 6e6f 7772 0800 0000 720c 0000 00da 0d66  nowr....r......f
+00000760: 6974 5f74 7261 6e73 666f 726d 720e 0000  it_transformr...
+00000770: 0029 0472 1100 0000 7215 0000 0072 1600  .).r....r....r..
+00000780: 0000 da03 656e 6372 1200 0000 7212 0000  ....encr....r...
+00000790: 0072 1300 0000 da1e 6669 745f 7461 7267  .r......fit_targ
+000007a0: 6574 5f65 6e63 6f64 655f 6269 6e61 7279  et_encode_binary
+000007b0: 5f63 6c61 7373 1e00 0000 730a 0000 0012  _class....s.....
+000007c0: 040c 0118 010a 0104 017a 3742 696e 6172  .........z7Binar
+000007d0: 7943 6c61 7373 5461 7267 6574 456e 636f  yClassTargetEnco
+000007e0: 6465 722e 6669 745f 7461 7267 6574 5f65  der.fit_target_e
+000007f0: 6e63 6f64 655f 6269 6e61 7279 5f63 6c61  ncode_binary_cla
+00000800: 7373 6302 0000 0000 0000 0000 0000 0003  ssc.............
+00000810: 0000 0004 0000 0043 0000 0073 3600 0000  .......C...s6...
+00000820: 7400 7401 a002 a100 9b00 6401 9d02 8301  t.t.......d.....
+00000830: 0100 7c00 6a03 6402 1900 7d02 7c02 a004  ..|.j.d...}.|...
+00000840: 7c01 7c00 6a05 1900 a101 7c01 7c00 6a05  |.|.j.....|.|.j.
+00000850: 3c00 7c01 5300 2903 fa36 5472 616e 7366  <.|.S.)..6Transf
+00000860: 6f72 6d20 6361 7465 676f 7269 6573 2062  orm categories b
+00000870: 6173 6564 206f 6e20 616c 7265 6164 7920  ased on already 
+00000880: 7472 6169 6e65 6420 656e 636f 6465 722e  trained encoder.
+00000890: 7a3b 3a20 5374 6172 7420 7472 616e 7366  z;: Start transf
+000008a0: 6f72 6d69 6e67 2063 6174 6567 6f72 6965  orming categorie
+000008b0: 7320 7769 7468 2062 696e 6172 7920 7461  s with binary ta
+000008c0: 7267 6574 2065 6e63 6f64 6572 2e72 1a00  rget encoder.r..
+000008d0: 0000 2906 7209 0000 0072 0200 0000 721b  ..).r....r....r.
+000008e0: 0000 0072 0e00 0000 da09 7472 616e 7366  ...r......transf
+000008f0: 6f72 6d72 0c00 0000 2903 7211 0000 0072  ormr....).r....r
+00000900: 1500 0000 721d 0000 0072 1200 0000 7212  ....r....r....r.
+00000910: 0000 0072 1300 0000 da24 7472 616e 7366  ...r.....$transf
+00000920: 6f72 6d5f 7461 7267 6574 5f65 6e63 6f64  orm_target_encod
+00000930: 655f 6269 6e61 7279 5f63 6c61 7373 2800  e_binary_class(.
+00000940: 0000 730c 0000 0002 020c 0104 ff0a 0316  ..s.............
+00000950: 0104 017a 3d42 696e 6172 7943 6c61 7373  ...z=BinaryClass
+00000960: 5461 7267 6574 456e 636f 6465 722e 7472  TargetEncoder.tr
+00000970: 616e 7366 6f72 6d5f 7461 7267 6574 5f65  ansform_target_e
+00000980: 6e63 6f64 655f 6269 6e61 7279 5f63 6c61  ncode_binary_cla
+00000990: 7373 4e29 0fda 085f 5f6e 616d 655f 5fda  ssN)...__name__.
+000009a0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000009b0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+000009c0: 5f5f 7204 0000 0072 0600 0000 da03 7374  __r....r......st
+000009d0: 72da 0566 6c6f 6174 da03 696e 7472 1400  r..float..intr..
+000009e0: 0000 da02 7064 da09 4461 7461 4672 616d  ....pd..DataFram
+000009f0: 65da 0653 6572 6965 7372 1e00 0000 7221  e..Seriesr....r!
+00000a00: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+00000a10: 0000 7213 0000 0072 0b00 0000 1600 0000  ..r....r........
+00000a20: 7316 0000 0008 0004 011c 0202 0504 0102  s...............
+00000a30: ff04 0102 ff04 020a fe1a 0a72 0b00 0000  ...........r....
+00000a40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000a50: 0006 0000 0040 0000 0072 0a00 0000 290d  .....@...r....).
+00000a60: da17 4d75 6c74 6943 6c61 7373 5461 7267  ..MultiClassTarg
+00000a70: 6574 456e 636f 6465 727a 4f54 6172 6765  etEncoderzOTarge
+00000a80: 7420 656e 636f 6465 2063 6174 6567 6f72  t encode categor
+00000a90: 6963 616c 2066 6561 7475 7265 7320 696e  ical features in
+00000aa0: 2074 6865 2063 6f6e 7465 7874 206f 6620   the context of 
+00000ab0: 6d75 6c74 6963 6c61 7373 2063 6c61 7373  multiclass class
+00000ac0: 6966 6963 6174 696f 6e2e 720c 0000 0063  ification.r....c
+00000ad0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000ae0: 0200 0000 4300 0000 731c 0000 0069 007c  ....C...s....i.|
+00000af0: 005f 0064 017c 005f 017c 017c 005f 0267  ._.d.|._.|.|._.g
+00000b00: 007c 005f 0364 0053 0072 0d00 0000 2904  .|._.d.S.r....).
+00000b10: 720e 0000 0072 0f00 0000 720c 0000 00da  r....r....r.....
+00000b20: 0b63 6c61 7373 5f6e 616d 6573 7210 0000  .class_namesr...
+00000b30: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000b40: 7214 0000 0035 0000 0073 0800 0000 0601  r....5...s......
+00000b50: 0601 0601 0a01 7a20 4d75 6c74 6943 6c61  ......z MultiCla
+00000b60: 7373 5461 7267 6574 456e 636f 6465 722e  ssTargetEncoder.
+00000b70: 5f5f 696e 6974 5f5f 7215 0000 0072 1600  __init__r....r..
+00000b80: 0000 7217 0000 0063 0300 0000 0000 0000  ..r....c........
+00000b90: 0000 0000 0900 0000 0600 0000 0300 0000  ................
+00000ba0: 73ea 0000 0074 0074 01a0 02a1 009b 0064  s....t.t.......d
+00000bb0: 019d 0283 0101 0064 027d 0374 0383 007d  .......d.}.t...}
+00000bc0: 047c 04a0 047c 02a1 0101 007c 04a0 057c  .|...|.....|...|
+00000bd0: 02a1 017d 057c 056a 06a0 07a1 007c 005f  ...}.|.j.....|._
+00000be0: 087c 016a 0964 0364 0385 027c 006a 0a66  .|.j.d.d...|.j.f
+00000bf0: 0219 00a0 0ba1 007d 067c 016a 0964 0364  .......}.|.j.d.d
+00000c00: 0385 027c 016a 06a0 0c7c 006a 0aa1 010f  ...|.j...|.j....
+00000c10: 0066 0219 007d 017c 006a 0844 005d 2e89  .f...}.|.j.D.]..
+00000c20: 0074 0d83 007d 077c 07a0 047c 067c 0588  .t...}.|...|.|..
+00000c30: 0019 00a1 0201 007c 077c 006a 0e64 0488  .......|.|.j.d..
+00000c40: 009b 009d 023c 007c 07a0 057c 06a1 017d  .....<.|...|...}
+00000c50: 0887 0066 0164 0564 0684 087c 086a 0644  ...f.d.d...|.j.D
+00000c60: 0083 017c 085f 0674 0f6a 107c 017c 0867  ...|._.t.j.|.|.g
+00000c70: 0264 0764 088d 027d 0171 3c7c 047c 006a  .d.d...}.q<|.|.j
+00000c80: 0e7c 039b 0064 099d 023c 007c 0153 0029  .|...d...<.|.S.)
+00000c90: 0a72 1800 0000 7a2a 3a20 5374 6172 7420  .r....z*: Start 
+00000ca0: 6669 7474 696e 6720 6d75 6c74 6963 6c61  fitting multicla
+00000cb0: 7373 2074 6172 6765 7420 656e 636f 6465  ss target encode
+00000cc0: 722e da24 6d75 6c74 6963 6c61 7373 5f74  r..$multiclass_t
+00000cd0: 6172 6765 745f 656e 636f 6469 6e67 5f6f  arget_encoding_o
+00000ce0: 6e65 686f 7474 6572 4eda 236d 756c 7469  nehotterN.#multi
+00000cf0: 636c 6173 735f 7461 7267 6574 5f65 6e63  class_target_enc
+00000d00: 6f64 6572 5f61 6c6c 5f63 6f6c 735f 6301  oder_all_cols_c.
+00000d10: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00000d20: 0000 0013 0000 00f3 2000 0000 6700 7c00  ........ ...g.|.
+00000d30: 5d0c 7d01 7400 7c01 8301 6400 1700 7400  ].}.t.|...d...t.
+00000d40: 8800 8301 1700 9102 7102 5300 a901 da01  ........q.S.....
+00000d50: 5fa9 0172 2600 0000 a902 da02 2e30 7215  _..r&........0r.
+00000d60: 0000 00a9 01da 0663 6c61 7373 5f72 1200  .......class_r..
+00000d70: 0000 7213 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
+00000d80: 6d70 3e4c 0000 00f3 0200 0000 2000 7a48  mp>L........ .zH
+00000d90: 4d75 6c74 6943 6c61 7373 5461 7267 6574  MultiClassTarget
+00000da0: 456e 636f 6465 722e 6669 745f 7461 7267  Encoder.fit_targ
+00000db0: 6574 5f65 6e63 6f64 655f 6d75 6c74 6963  et_encode_multic
+00000dc0: 6c61 7373 2e3c 6c6f 6361 6c73 3e2e 3c6c  lass.<locals>.<l
+00000dd0: 6973 7463 6f6d 703e e901 0000 00a9 01da  istcomp>........
+00000de0: 0461 7869 73da 095f 616c 6c5f 636f 6c73  .axis.._all_cols
+00000df0: 2911 7209 0000 0072 0200 0000 721b 0000  ).r....r....r...
+00000e00: 0072 0700 0000 da03 6669 7472 2000 0000  .r......fitr ...
+00000e10: da07 636f 6c75 6d6e 73da 0774 6f5f 6c69  ..columns..to_li
+00000e20: 7374 722d 0000 00da 036c 6f63 720c 0000  str-.....locr...
+00000e30: 00da 0463 6f70 79da 0469 7369 6e72 0800  ...copy..isinr..
+00000e40: 0000 720e 0000 0072 2900 0000 da06 636f  ..r....r).....co
+00000e50: 6e63 6174 2909 7211 0000 0072 1500 0000  ncat).r....r....
+00000e60: 7216 0000 00da 0961 6c67 6f72 6974 686d  r......algorithm
+00000e70: 721d 0000 005a 0879 5f6f 6e65 686f 74da  r....Z.y_onehot.
+00000e80: 0578 5f6f 626a da0a 7461 7267 6574 5f65  .x_obj..target_e
+00000e90: 6e63 da04 7465 6d70 7212 0000 0072 3600  nc..tempr....r6.
+00000ea0: 0000 7213 0000 00da 1c66 6974 5f74 6172  ..r......fit_tar
+00000eb0: 6765 745f 656e 636f 6465 5f6d 756c 7469  get_encode_multi
+00000ec0: 636c 6173 733b 0000 0073 2200 0000 1204  class;...s".....
+00000ed0: 0401 0601 0a01 0a01 0c01 1801 1e01 0a01  ................
+00000ee0: 0601 1001 1001 0a01 1601 1401 1001 0401  ................
+00000ef0: 7a34 4d75 6c74 6943 6c61 7373 5461 7267  z4MultiClassTarg
+00000f00: 6574 456e 636f 6465 722e 6669 745f 7461  etEncoder.fit_ta
+00000f10: 7267 6574 5f65 6e63 6f64 655f 6d75 6c74  rget_encode_mult
+00000f20: 6963 6c61 7373 6302 0000 0000 0000 0000  iclassc.........
+00000f30: 0000 0007 0000 0005 0000 0003 0000 0073  ...............s
+00000f40: be00 0000 7400 7401 a002 a100 9b00 6401  ....t.t.......d.
+00000f50: 9d02 8301 0100 6402 7d02 7c00 6a03 7c02  ......d.}.|.j.|.
+00000f60: 9b00 6403 9d02 1900 7d03 7c01 6a04 6404  ..d.....}.|.j.d.
+00000f70: 6404 8502 7c00 6a05 6602 1900 a006 a100  d...|.j.f.......
+00000f80: 7d04 7c01 6a04 6404 6404 8502 7c01 6a07  }.|.j.d.d...|.j.
+00000f90: a008 7c00 6a05 a101 0f00 6602 1900 7d01  ..|.j.....f...}.
+00000fa0: 7c00 6a09 4400 5d23 8900 7c00 6a03 6405  |.j.D.]#..|.j.d.
+00000fb0: 8800 9b00 9d02 1900 7d05 7c05 a00a 7c04  ........}.|...|.
+00000fc0: a101 7d06 8700 6601 6406 6407 8408 7c06  ..}...f.d.d...|.
+00000fd0: 6a07 4400 8301 7c06 5f07 740b 6a0c 7c01  j.D...|._.t.j.|.
+00000fe0: 7c06 6702 6408 6409 8d02 7d01 7131 7c03  |.g.d.d...}.q1|.
+00000ff0: 7c00 6a03 7c02 9b00 6403 9d02 3c00 7c01  |.j.|...d...<.|.
+00001000: 5300 290a 721f 0000 007a 3f3a 2053 7461  S.).r....z?: Sta
+00001010: 7274 2074 7261 6e73 666f 726d 696e 6720  rt transforming 
+00001020: 6361 7465 676f 7269 6573 2077 6974 6820  categories with 
+00001030: 6d75 6c74 6963 6c61 7373 2074 6172 6765  multiclass targe
+00001040: 7420 656e 636f 6465 722e 722e 0000 0072  t encoder.r....r
+00001050: 3d00 0000 4e72 2f00 0000 6301 0000 0000  =...Nr/...c.....
+00001060: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00001070: 0000 0072 3000 0000 7231 0000 0072 3300  ...r0...r1...r3.
+00001080: 0000 7234 0000 0072 3600 0000 7212 0000  ..r4...r6...r...
+00001090: 0072 1300 0000 7238 0000 005d 0000 0072  .r....r8...]...r
+000010a0: 3900 0000 7a4e 4d75 6c74 6943 6c61 7373  9...zNMultiClass
+000010b0: 5461 7267 6574 456e 636f 6465 722e 7472  TargetEncoder.tr
+000010c0: 616e 7366 6f72 6d5f 7461 7267 6574 5f65  ansform_target_e
+000010d0: 6e63 6f64 655f 6d75 6c74 6963 6c61 7373  ncode_multiclass
+000010e0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+000010f0: 6f6d 703e 723a 0000 0072 3b00 0000 290d  omp>r:...r;...).
+00001100: 7209 0000 0072 0200 0000 721b 0000 0072  r....r....r....r
+00001110: 0e00 0000 7241 0000 0072 0c00 0000 7242  ....rA...r....rB
+00001120: 0000 0072 3f00 0000 7243 0000 0072 2d00  ...r?...rC...r-.
+00001130: 0000 7220 0000 0072 2900 0000 7244 0000  ..r ...r)...rD..
+00001140: 0029 0772 1100 0000 7215 0000 0072 4500  .).r....r....rE.
+00001150: 0000 721d 0000 0072 4600 0000 7247 0000  ..r....rF...rG..
+00001160: 0072 4800 0000 7212 0000 0072 3600 0000  .rH...r....r6...
+00001170: 7213 0000 00da 2274 7261 6e73 666f 726d  r....."transform
+00001180: 5f74 6172 6765 745f 656e 636f 6465 5f6d  _target_encode_m
+00001190: 756c 7469 636c 6173 7351 0000 0073 1c00  ulticlassQ...s..
+000011a0: 0000 0202 0c01 04ff 0403 1001 1801 1e01  ................
+000011b0: 0a01 1001 0a01 1601 1401 1001 0401 7a3a  ..............z:
+000011c0: 4d75 6c74 6943 6c61 7373 5461 7267 6574  MultiClassTarget
+000011d0: 456e 636f 6465 722e 7472 616e 7366 6f72  Encoder.transfor
+000011e0: 6d5f 7461 7267 6574 5f65 6e63 6f64 655f  m_target_encode_
+000011f0: 6d75 6c74 6963 6c61 7373 4e29 0f72 2200  multiclassN).r".
+00001200: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
+00001210: 0072 0400 0000 7206 0000 0072 2600 0000  .r....r....r&...
+00001220: 7227 0000 0072 2800 0000 7214 0000 0072  r'...r(...r....r
+00001230: 2900 0000 722a 0000 0072 2b00 0000 7249  )...r*...r+...rI
+00001240: 0000 0072 4a00 0000 7212 0000 0072 1200  ...rJ...r....r..
+00001250: 0000 7212 0000 0072 1300 0000 722c 0000  ..r....r....r,..
+00001260: 0032 0000 0073 1600 0000 0800 0401 1c02  .2...s..........
+00001270: 0206 0401 02ff 0401 02ff 0402 0afe 1a16  ................
+00001280: 722c 0000 0029 1072 2500 0000 7202 0000  r,...).r%...r...
+00001290: 00da 0674 7970 696e 6772 0300 0000 7204  ...typingr....r.
+000012a0: 0000 0072 0500 0000 7206 0000 00da 0670  ...r....r......p
+000012b0: 616e 6461 7372 2900 0000 5a11 6361 7465  andasr)...Z.cate
+000012c0: 676f 7279 5f65 6e63 6f64 6572 7372 0700  gory_encodersr..
+000012d0: 0000 7208 0000 00da 2462 6c75 6563 6173  ..r.....$bluecas
+000012e0: 742e 6765 6e65 7261 6c5f 7574 696c 732e  t.general_utils.
+000012f0: 6765 6e65 7261 6c5f 7574 696c 7372 0900  general_utilsr..
+00001300: 0000 720b 0000 0072 2c00 0000 7212 0000  ..r....r,...r...
+00001310: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001320: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
+00001330: 0000 0004 000c 0c18 0108 0210 010c 020e  ................
+00001340: 0312 1c                                  ...
```

### Comparing `bluecast-0.2/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-0.3/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:39:31 2023 UTC, .py size: 1748 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,112 @@
-00000000: 6f0d 0d0a 0000 0000 03eb 8064 d406 0000  o..........d....
+00000000: 550d 0d0a 0000 0000 f058 8164 d406 0000  U........X.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
+00000020: 0006 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
-00000050: 0100 6401 6405 6c06 6d07 5a07 0100 0906  ..d.d.l.m.Z.....
-00000060: 0907 0903 6412 6408 6503 6a08 6409 6509  ....d.d.e.j.d.e.
-00000070: 640a 650a 640b 6509 6608 640c 640d 8405  d.e.d.e.f.d.d...
-00000080: 5a0b 0906 6413 6408 6503 6a08 6409 6509  Z...d.d.e.j.d.e.
-00000090: 640e 6509 640f 650c 6608 6410 6411 8405  d.e.d.e.f.d.d...
-000000a0: 5a0d 6403 5300 2914 7ab2 0a54 6869 7320  Z.d.S.).z..This 
-000000b0: 6d6f 6475 6c65 2063 6f6e 7461 696e 7320  module contains 
-000000c0: 6675 6e63 7469 6f6e 7320 746f 2073 706c  functions to spl
-000000d0: 6974 2064 6174 6120 696e 746f 2074 7261  it data into tra
-000000e0: 696e 2061 6e64 2074 6573 7420 7365 7473  in and test sets
-000000f0: 2e0a 0a54 6865 2074 7261 696e 2d74 6573  ...The train-tes
-00000100: 7420 7370 6c69 7420 6361 6e20 6265 2064  t split can be d
-00000110: 6f6e 6520 696e 2074 776f 2077 6179 733a  one in two ways:
-00000120: 0a20 2020 202d 2052 616e 646f 6d6c 790a  .    - Randomly.
-00000130: 2020 2020 2d20 4261 7365 6420 6f6e 2061      - Based on a
-00000140: 2070 726f 7669 6465 6420 6f72 6465 7220   provided order 
-00000150: 2869 2e65 2e20 7469 6d65 290a e900 0000  (i.e. time).....
-00000160: 0029 01da 0864 6174 6574 696d 654e 2901  .)...datetimeN).
-00000170: da0f 6d6f 6465 6c5f 7365 6c65 6374 696f  ..model_selectio
-00000180: 6e29 01da 066c 6f67 6765 72e7 9a99 9999  n)...logger.....
-00000190: 9999 e93f e964 0000 00da 0264 66da 0a74  ...?.d.....df..t
-000001a0: 6172 6765 745f 636f 6cda 0c72 616e 646f  arget_col..rando
-000001b0: 6d5f 7374 6174 65da 0c73 7472 6174 6966  m_state..stratif
-000001c0: 795f 636f 6c63 0500 0000 0000 0000 0000  y_colc..........
-000001d0: 0000 0a00 0000 0700 0000 4300 0000 735a  ..........C...sZ
-000001e0: 0000 0074 0074 01a0 02a1 009b 0064 017c  ...t.t.......d.|
-000001f0: 029b 0064 029d 0483 0101 007c 007c 0119  ...d.......|.|..
-00000200: 00a0 03a1 007d 057c 006a 047c 0164 0364  .....}.|.j.|.d.d
-00000210: 048d 027d 0074 056a 067c 007c 057c 027c  ...}.t.j.|.|.|.|
-00000220: 037c 0464 058d 055c 047d 067d 077d 087d  .|.d...\.}.}.}.}
-00000230: 097c 067c 077c 087c 0966 0453 0029 067a  .|.|.|.|.f.S.).z
-00000240: 3b53 706c 6974 2064 6174 6120 696e 746f  ;Split data into
-00000250: 2074 7261 696e 2061 6e64 2074 6573 742e   train and test.
-00000260: 2053 7472 6174 6966 6963 6174 696f 6e20   Stratification 
-00000270: 6973 2070 6f73 7369 626c 652e 7a36 3a20  is possible.z6: 
-00000280: 5374 6172 7420 6578 6563 7574 696e 6720  Start executing 
-00000290: 7472 6169 6e2d 7465 7374 2073 706c 6974  train-test split
-000002a0: 2077 6974 6820 7472 6169 6e20 7369 7a65   with train size
-000002b0: 206f 6620 da01 2ee9 0100 0000 2901 da04   of ........)...
-000002c0: 6178 6973 2903 da0a 7472 6169 6e5f 7369  axis)...train_si
-000002d0: 7a65 7209 0000 00da 0873 7472 6174 6966  zer......stratif
-000002e0: 7929 0772 0400 0000 7202 0000 00da 0675  y).r....r......u
-000002f0: 7463 6e6f 77da 0463 6f70 79da 0464 726f  tcnow..copy..dro
-00000300: 7072 0300 0000 da10 7472 6169 6e5f 7465  pr......train_te
-00000310: 7374 5f73 706c 6974 290a 7207 0000 0072  st_split).r....r
-00000320: 0800 0000 720e 0000 0072 0900 0000 720a  ....r....r....r.
-00000330: 0000 00da 0674 6172 6765 74da 0778 5f74  .....target..x_t
-00000340: 7261 696e da06 785f 7465 7374 da07 795f  rain..x_test..y_
-00000350: 7472 6169 6eda 0679 5f74 6573 74a9 0072  train..y_test..r
-00000360: 1900 0000 fa56 2f55 7365 7273 2f74 686f  .....V/Users/tho
-00000370: 6d61 736d 6569 7373 6e65 722f 4964 6561  masmeissner/Idea
-00000380: 5072 6f6a 6563 7473 2f42 6c75 6543 6173  Projects/BlueCas
-00000390: 742f 626c 7565 6361 7374 2f70 7265 7072  t/bluecast/prepr
-000003a0: 6f63 6573 7369 6e67 2f74 7261 696e 5f74  ocessing/train_t
-000003b0: 6573 745f 7370 6c69 742e 7079 da16 7472  est_split.py..tr
-000003c0: 6169 6e5f 7465 7374 5f73 706c 6974 5f63  ain_test_split_c
-000003d0: 726f 7373 1000 0000 731a 0000 0002 0812  ross....s.......
-000003e0: 0104 ff0c 030e 0104 0102 0102 0102 0102  ................
-000003f0: 0102 010e fb0c 0772 1b00 0000 da0c 7370  .......r......sp
-00000400: 6c69 745f 6279 5f63 6f6c 720e 0000 0063  lit_by_colr....c
-00000410: 0400 0000 0000 0000 0000 0000 0b00 0000  ................
-00000420: 0500 0000 4300 0000 738a 0000 0074 0074  ....C...s....t.t
-00000430: 01a0 02a1 009b 0064 017c 039b 0064 029d  .......d.|...d..
-00000440: 0483 0101 0074 037c 006a 0483 017d 0474  .....t.|.j...}.t
-00000450: 057c 047c 0314 0083 017d 057c 047c 0518  .|.|.....}.|.|..
-00000460: 007d 067c 0273 227c 00a0 06a1 007d 006e  .}.|.s"|.....}.n
-00000470: 0b7c 0272 2c7c 006a 077c 0267 0164 038d  .|.r,|.j.|.g.d..
-00000480: 017d 006e 0109 007c 00a0 087c 05a1 017d  .}.n...|...|...}
-00000490: 077c 00a0 097c 06a1 017d 087c 077c 0119  .|...|...}.|.|..
-000004a0: 007d 097c 087c 0119 007d 0a7c 077c 087c  .}.|.|...}.|.|.|
-000004b0: 097c 0a66 0453 0029 047a 4553 706c 6974  .|.f.S.).zESplit
-000004c0: 2064 6174 6120 696e 746f 2074 7261 696e   data into train
-000004d0: 2061 6e64 2074 6573 7420 6261 7365 6420   and test based 
-000004e0: 6f6e 2061 2070 726f 7669 6465 6420 6f72  on a provided or
-000004f0: 6465 7220 2869 2e65 2e20 7469 6d65 292e  der (i.e. time).
-00000500: 7a3e 3a20 5374 6172 7420 6578 6563 7574  z>: Start execut
-00000510: 696e 6720 6f72 6465 7265 6420 7472 6169  ing ordered trai
-00000520: 6e2d 7465 7374 2073 706c 6974 2077 6974  n-test split wit
-00000530: 6820 7472 6169 6e20 7369 7a65 206f 6620  h train size of 
-00000540: 720b 0000 0029 01da 0262 7929 0a72 0400  r....)...by).r..
-00000550: 0000 7202 0000 0072 1000 0000 da03 6c65  ..r....r......le
-00000560: 6eda 0569 6e64 6578 da03 696e 74da 0a73  n..index..int..s
-00000570: 6f72 745f 696e 6465 78da 0b73 6f72 745f  ort_index..sort_
-00000580: 7661 6c75 6573 da04 6865 6164 da04 7461  values..head..ta
-00000590: 696c 290b 7207 0000 0072 0800 0000 721c  il).r....r....r.
-000005a0: 0000 0072 0e00 0000 da06 6c65 6e67 7468  ...r......length
-000005b0: 5a0c 7472 6169 6e5f 6c65 6e67 7468 5a0b  Z.train_lengthZ.
-000005c0: 7465 7374 5f6c 656e 6774 6872 1500 0000  test_lengthr....
-000005d0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-000005e0: 1900 0000 7219 0000 0072 1a00 0000 da15  ....r....r......
-000005f0: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
-00000600: 5f74 696d 6527 0000 0073 2000 0000 0204  _time'...s .....
-00000610: 1201 04ff 0a03 0c01 0801 0401 0a01 0401  ................
-00000620: 1001 0202 0a01 0a01 0801 0801 0c01 7226  ..............r&
-00000630: 0000 0029 0372 0500 0000 7206 0000 004e  ...).r....r....N
-00000640: 2901 7205 0000 0029 0eda 075f 5f64 6f63  ).r....)...__doc
-00000650: 5f5f 7202 0000 00da 0670 616e 6461 73da  __r......pandas.
-00000660: 0270 64da 0773 6b6c 6561 726e 7203 0000  .pd..sklearnr...
-00000670: 00da 2462 6c75 6563 6173 742e 6765 6e65  ..$bluecast.gene
-00000680: 7261 6c5f 7574 696c 732e 6765 6e65 7261  ral_utils.genera
-00000690: 6c5f 7574 696c 7372 0400 0000 da09 4461  l_utilsr......Da
-000006a0: 7461 4672 616d 65da 0373 7472 7220 0000  taFrame..strr ..
-000006b0: 0072 1b00 0000 da05 666c 6f61 7472 2600  .r......floatr&.
-000006c0: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
-000006d0: 0072 1a00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000006e0: 0100 0000 7336 0000 0004 000c 0708 020c  ....s6..........
-000006f0: 010c 0202 0602 0102 0104 fb04 0102 ff02  ................
-00000700: 0202 fe02 0402 fc02 050a fb02 1804 ff04  ................
-00000710: 0102 ff02 0102 ff02 0102 ff02 010e ff    ...............
+00000050: 0100 6401 6405 6c06 6d07 5a07 0100 640e  ..d.d.l.m.Z...d.
+00000060: 6503 6a08 6509 650a 6509 6408 9c04 6409  e.j.e.e.e.d...d.
+00000070: 640a 8405 5a0b 640f 6503 6a08 6509 6509  d...Z.d.e.j.e.e.
+00000080: 650c 640b 9c04 640c 640d 8405 5a0d 6403  e.d...d.d...Z.d.
+00000090: 5300 2910 7ab2 0a54 6869 7320 6d6f 6475  S.).z..This modu
+000000a0: 6c65 2063 6f6e 7461 696e 7320 6675 6e63  le contains func
+000000b0: 7469 6f6e 7320 746f 2073 706c 6974 2064  tions to split d
+000000c0: 6174 6120 696e 746f 2074 7261 696e 2061  ata into train a
+000000d0: 6e64 2074 6573 7420 7365 7473 2e0a 0a54  nd test sets...T
+000000e0: 6865 2074 7261 696e 2d74 6573 7420 7370  he train-test sp
+000000f0: 6c69 7420 6361 6e20 6265 2064 6f6e 6520  lit can be done 
+00000100: 696e 2074 776f 2077 6179 733a 0a20 2020  in two ways:.   
+00000110: 202d 2052 616e 646f 6d6c 790a 2020 2020   - Randomly.    
+00000120: 2d20 4261 7365 6420 6f6e 2061 2070 726f  - Based on a pro
+00000130: 7669 6465 6420 6f72 6465 7220 2869 2e65  vided order (i.e
+00000140: 2e20 7469 6d65 290a e900 0000 0029 01da  . time)......)..
+00000150: 0864 6174 6574 696d 654e 2901 da0f 6d6f  .datetimeN)...mo
+00000160: 6465 6c5f 7365 6c65 6374 696f 6e29 01da  del_selection)..
+00000170: 066c 6f67 6765 72e7 9a99 9999 9999 e93f  .logger........?
+00000180: e964 0000 0029 04da 0264 66da 0a74 6172  .d...)...df..tar
+00000190: 6765 745f 636f 6cda 0c72 616e 646f 6d5f  get_col..random_
+000001a0: 7374 6174 65da 0c73 7472 6174 6966 795f  state..stratify_
+000001b0: 636f 6c63 0500 0000 0000 0000 0000 0000  colc............
+000001c0: 0a00 0000 0700 0000 4300 0000 735a 0000  ........C...sZ..
+000001d0: 0074 0074 01a0 02a1 009b 0064 017c 029b  .t.t.......d.|..
+000001e0: 0064 029d 0483 0101 007c 007c 0119 00a0  .d.......|.|....
+000001f0: 03a1 007d 057c 006a 047c 0164 0364 048d  ...}.|.j.|.d.d..
+00000200: 027d 0074 056a 067c 007c 057c 027c 037c  .}.t.j.|.|.|.|.|
+00000210: 0464 058d 055c 047d 067d 077d 087d 097c  .d...\.}.}.}.}.|
+00000220: 067c 077c 087c 0966 0453 0029 067a 3b53  .|.|.|.f.S.).z;S
+00000230: 706c 6974 2064 6174 6120 696e 746f 2074  plit data into t
+00000240: 7261 696e 2061 6e64 2074 6573 742e 2053  rain and test. S
+00000250: 7472 6174 6966 6963 6174 696f 6e20 6973  tratification is
+00000260: 2070 6f73 7369 626c 652e 7a36 3a20 5374   possible.z6: St
+00000270: 6172 7420 6578 6563 7574 696e 6720 7472  art executing tr
+00000280: 6169 6e2d 7465 7374 2073 706c 6974 2077  ain-test split w
+00000290: 6974 6820 7472 6169 6e20 7369 7a65 206f  ith train size o
+000002a0: 6620 da01 2ee9 0100 0000 2901 da04 6178  f ........)...ax
+000002b0: 6973 2903 da0a 7472 6169 6e5f 7369 7a65  is)...train_size
+000002c0: 7209 0000 00da 0873 7472 6174 6966 7929  r......stratify)
+000002d0: 0772 0400 0000 7202 0000 00da 0675 7463  .r....r......utc
+000002e0: 6e6f 77da 0463 6f70 79da 0464 726f 7072  now..copy..dropr
+000002f0: 0300 0000 da10 7472 6169 6e5f 7465 7374  ......train_test
+00000300: 5f73 706c 6974 290a 7207 0000 0072 0800  _split).r....r..
+00000310: 0000 720e 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000320: 00da 0674 6172 6765 74da 0778 5f74 7261  ...target..x_tra
+00000330: 696e da06 785f 7465 7374 da07 795f 7472  in..x_test..y_tr
+00000340: 6169 6eda 0679 5f74 6573 74a9 0072 1900  ain..y_test..r..
+00000350: 0000 fa4d 2f68 6f6d 652f 7468 6f6d 6173  ...M/home/thomas
+00000360: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
+00000370: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
+00000380: 7072 6570 726f 6365 7373 696e 672f 7472  preprocessing/tr
+00000390: 6169 6e5f 7465 7374 5f73 706c 6974 2e70  ain_test_split.p
+000003a0: 79da 1674 7261 696e 5f74 6573 745f 7370  y..train_test_sp
+000003b0: 6c69 745f 6372 6f73 7310 0000 0073 1a00  lit_cross....s..
+000003c0: 0000 0008 0201 12ff 0403 0c01 0e01 0401  ................
+000003d0: 0201 0201 0201 0201 02fb 0e07 721b 0000  ............r...
+000003e0: 0029 0472 0700 0000 7208 0000 00da 0c73  .).r....r......s
+000003f0: 706c 6974 5f62 795f 636f 6c72 0e00 0000  plit_by_colr....
+00000400: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
+00000410: 0005 0000 0043 0000 0073 8800 0000 7400  .....C...s....t.
+00000420: 7401 a002 a100 9b00 6401 7c03 9b00 6402  t.......d.|...d.
+00000430: 9d04 8301 0100 7403 7c00 6a04 8301 7d04  ......t.|.j...}.
+00000440: 7405 7c04 7c03 1400 8301 7d05 7c04 7c05  t.|.|.....}.|.|.
+00000450: 1800 7d06 7c02 7344 7c00 a006 a100 7d00  ..}.|.sD|.....}.
+00000460: 6e14 7c02 7258 7c00 6a07 7c02 6701 6403  n.|.rX|.j.|.g.d.
+00000470: 8d01 7d00 6e00 7c00 a008 7c05 a101 7d07  ..}.n.|...|...}.
+00000480: 7c00 a009 7c06 a101 7d08 7c07 7c01 1900  |...|...}.|.|...
+00000490: 7d09 7c08 7c01 1900 7d0a 7c07 7c08 7c09  }.|.|...}.|.|.|.
+000004a0: 7c0a 6604 5300 2904 7a45 5370 6c69 7420  |.f.S.).zESplit 
+000004b0: 6461 7461 2069 6e74 6f20 7472 6169 6e20  data into train 
+000004c0: 616e 6420 7465 7374 2062 6173 6564 206f  and test based o
+000004d0: 6e20 6120 7072 6f76 6964 6564 206f 7264  n a provided ord
+000004e0: 6572 2028 692e 652e 2074 696d 6529 2e7a  er (i.e. time).z
+000004f0: 3e3a 2053 7461 7274 2065 7865 6375 7469  >: Start executi
+00000500: 6e67 206f 7264 6572 6564 2074 7261 696e  ng ordered train
+00000510: 2d74 6573 7420 7370 6c69 7420 7769 7468  -test split with
+00000520: 2074 7261 696e 2073 697a 6520 6f66 2072   train size of r
+00000530: 0b00 0000 2901 da02 6279 290a 7204 0000  ....)...by).r...
+00000540: 0072 0200 0000 7210 0000 00da 036c 656e  .r....r......len
+00000550: da05 696e 6465 78da 0369 6e74 da0a 736f  ..index..int..so
+00000560: 7274 5f69 6e64 6578 da0b 736f 7274 5f76  rt_index..sort_v
+00000570: 616c 7565 73da 0468 6561 64da 0474 6169  alues..head..tai
+00000580: 6c29 0b72 0700 0000 7208 0000 0072 1c00  l).r....r....r..
+00000590: 0000 720e 0000 00da 066c 656e 6774 68da  ..r......length.
+000005a0: 0c74 7261 696e 5f6c 656e 6774 68da 0b74  .train_length..t
+000005b0: 6573 745f 6c65 6e67 7468 7215 0000 0072  est_lengthr....r
+000005c0: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+000005d0: 0000 0072 1900 0000 721a 0000 00da 1574  ...r....r......t
+000005e0: 7261 696e 5f74 6573 745f 7370 6c69 745f  rain_test_split_
+000005f0: 7469 6d65 2700 0000 731e 0000 0000 0402  time'...s.......
+00000600: 0112 ff04 030a 010c 0108 0104 010a 0104  ................
+00000610: 0110 030a 010a 0108 0108 0172 2800 0000  ...........r(...
+00000620: 2903 7205 0000 0072 0600 0000 4e29 0172  ).r....r....N).r
+00000630: 0500 0000 290e da07 5f5f 646f 635f 5f72  ....)...__doc__r
+00000640: 0200 0000 da06 7061 6e64 6173 da02 7064  ......pandas..pd
+00000650: da07 736b 6c65 6172 6e72 0300 0000 da24  ..sklearnr.....$
+00000660: 626c 7565 6361 7374 2e67 656e 6572 616c  bluecast.general
+00000670: 5f75 7469 6c73 2e67 656e 6572 616c 5f75  _utils.general_u
+00000680: 7469 6c73 7204 0000 00da 0944 6174 6146  tilsr......DataF
+00000690: 7261 6d65 da03 7374 7272 2000 0000 721b  rame..strr ...r.
+000006a0: 0000 00da 0566 6c6f 6174 7228 0000 0072  .....floatr(...r
+000006b0: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+000006c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000006d0: 0073 2800 0000 0407 0c02 0801 0c02 0c06  .s(.............
+000006e0: 0001 0001 00fb 0201 0401 0202 0201 02fb  ................
+000006f0: 0c18 00ff 0201 0400 0200 0200 02ff       ..............
```

### Comparing `bluecast-0.2/bluecast/preprocessing/custom.py` & `bluecast-0.3/bluecast/preprocessing/custom.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/preprocessing/datetime_features.py` & `bluecast-0.3/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/preprocessing/encode_target_labels.py` & `bluecast-0.3/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/preprocessing/feature_types.py` & `bluecast-0.3/bluecast/preprocessing/feature_types.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-0.3/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/preprocessing/schema_checks.py` & `bluecast-0.3/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/preprocessing/target_encoding.py` & `bluecast-0.3/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/preprocessing/train_test_split.py` & `bluecast-0.3/bluecast/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 18:43:33 2023 UTC, .py size: 2497 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,250 @@
-00000000: 6f0d 0d0a 0000 0000 5521 8264 c109 0000  o.......U!.d....
+00000000: 6f0d 0d0a 0000 0000 be1c 8364 9c08 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
-00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a0a  Z.m.Z...d.d.l.Z.
-00000060: 6400 6401 6c0b 5a0b 6400 6403 6c0c 6d0d  d.d.l.Z.d.d.l.m.
-00000070: 5a0d 0100 6400 6404 6c0e 6d0f 5a0f 6d10  Z...d.d.l.m.Z.m.
-00000080: 5a10 0100 6400 6405 6c11 6d12 5a12 0100  Z...d.d.l.m.Z...
-00000090: 6400 6406 6c13 6d14 5a14 0100 650b 6a15  d.d.l.m.Z...e.j.
-000000a0: 6407 6508 650a 6a16 650a 6a16 6602 1900  d.e.e.j.e.j.f...
-000000b0: 6602 6408 6409 8404 8301 5a17 640a 640b  f.d.d.....Z.d.d.
-000000c0: 8400 5a18 6401 5300 290c e900 0000 004e  ..Z.d.S.)......N
-000000d0: 2902 da08 4f70 7469 6f6e 616c da05 5475  )...Optional..Tu
-000000e0: 706c 6529 01da 0842 6c75 6543 6173 7429  ple)...BlueCast)
-000000f0: 02da 0e54 7261 696e 696e 6743 6f6e 6669  ...TrainingConfi
-00000100: 67da 1758 6762 6f6f 7374 5475 6e65 5061  g..XgboostTunePa
-00000110: 7261 6d73 436f 6e66 6967 2901 da13 4375  ramsConfig)...Cu
-00000120: 7374 6f6d 5072 6570 726f 6365 7373 696e  stomPreprocessin
-00000130: 67a9 01da 1a63 7265 6174 655f 7379 6e74  g....create_synt
-00000140: 6865 7469 635f 6461 7461 6672 616d 65da  hetic_dataframe.
-00000150: 0672 6574 7572 6e63 0000 0000 0000 0000  .returnc........
-00000160: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000170: 7320 0000 0074 0064 0164 0264 038d 027d  s ...t.d.d.d...}
-00000180: 0074 0064 0164 0464 038d 027d 017c 007c  .t.d.d.d...}.|.|
-00000190: 0166 0253 0029 054e 69d0 0700 00e9 1400  .f.S.).Ni.......
-000001a0: 0000 2901 5a0c 7261 6e64 6f6d 5f73 7461  ..).Z.random_sta
-000001b0: 7465 e9c8 0000 0072 0800 0000 2902 da08  te.....r....)...
-000001c0: 6466 5f74 7261 696e da06 6466 5f76 616c  df_train..df_val
-000001d0: a900 720f 0000 00fa 472f 5573 6572 732f  ..r.....G/Users/
-000001e0: 7468 6f6d 6173 6d65 6973 736e 6572 2f49  thomasmeissner/I
-000001f0: 6465 6150 726f 6a65 6374 732f 426c 7565  deaProjects/Blue
-00000200: 4361 7374 2f62 6c75 6563 6173 742f 7465  Cast/bluecast/te
-00000210: 7374 732f 7465 7374 5f63 6173 742e 7079  sts/test_cast.py
-00000220: da19 7379 6e74 6865 7469 635f 7472 6169  ..synthetic_trai
-00000230: 6e5f 7465 7374 5f64 6174 610c 0000 0073  n_test_data....s
-00000240: 0600 0000 0c02 0c01 0801 7211 0000 0063  ..........r....c
-00000250: 0100 0000 0000 0000 0000 0000 1000 0000  ................
-00000260: 0a00 0000 4300 0000 73ae 0200 007c 0064  ....C...s....|.d
-00000270: 0119 007d 017c 0064 0219 007d 0274 0083  ...}.|.d...}.t..
-00000280: 007d 0364 037c 035f 0164 047c 035f 0274  .}.d.|._.d.|._.t
-00000290: 0383 007d 0464 057c 045f 0447 0064 0664  ...}.d.|._.G.d.d
-000002a0: 0784 0064 0774 0583 037d 057c 0583 007d  ...d.t...}.|...}
-000002b0: 0674 0664 0864 097c 047c 037c 0664 0a8d  .t.d.d.|.|.|.d..
-000002c0: 057d 077c 076a 077c 0164 0964 0b8d 0201  .}.|.j.|.d.d....
-000002d0: 0074 0864 0c83 0101 007c 07a0 097c 026a  .t.d.....|...|.j
-000002e0: 0a64 0964 0264 0d8d 02a1 015c 027d 087d  .d.d.d.....\.}.}
-000002f0: 0974 0864 0e83 0101 0074 0b7c 0883 017d  .t.d.....t.|...}
-00000300: 0a7c 026a 0c7d 0b74 0b7c 0b83 017d 0c7c  .|.j.}.t.|...}.|
-00000310: 0a7c 0c6b 027d 0d7c 0d73 c274 0da0 0e64  .|.k.}.|.s.t...d
-00000320: 0f7c 0d66 0164 107c 0a7c 0c66 02a1 0464  .|.f.d.|.|.f...d
-00000330: 1174 0fa0 10a1 0076 0073 6c74 0da0 1174  .t.....v.slt...t
-00000340: 0ba1 0172 7174 0da0 1274 0ba1 016e 0164  ...rqt...t...n.d
-00000350: 1164 1274 0fa0 10a1 0076 0073 7d74 0da0  .d.t.....v.s}t..
-00000360: 117c 08a1 0172 8274 0da0 127c 08a1 016e  .|...r.t...|...n
-00000370: 0164 1274 0da0 127c 0aa1 0164 1174 0fa0  .d.t...|...d.t..
-00000380: 10a1 0076 0073 9274 0da0 1174 0ba1 0172  ...v.s.t...t...r
-00000390: 9774 0da0 1274 0ba1 016e 0164 1164 1374  .t...t...n.d.d.t
-000003a0: 0fa0 10a1 0076 0073 a374 0da0 117c 02a1  .....v.s.t...|..
-000003b0: 0172 a874 0da0 127c 02a1 016e 0164 1374  .r.t...|...n.d.t
-000003c0: 0da0 127c 0ba1 0174 0da0 127c 0ca1 0164  ...|...t...|...d
-000003d0: 149c 0716 007d 0e64 1564 167c 0e69 0116  .....}.d.d.|.i..
-000003e0: 007d 0f74 1374 0da0 147c 0fa1 0183 0182  .}.t.t...|......
-000003f0: 0164 1704 007d 0a04 007d 0d04 007d 0b7d  .d...}...}...}.}
-00000400: 0c74 0b7c 0983 017d 0a7c 026a 0c7d 0b74  .t.|...}.|.j.}.t
-00000410: 0b7c 0b83 017d 0c7c 0a7c 0c6b 027d 0d7c  .|...}.|.|.k.}.|
-00000420: 0d90 0173 4d74 0da0 0e64 0f7c 0d66 0164  ...sMt...d.|.f.d
-00000430: 107c 0a7c 0c66 02a1 0464 1174 0fa0 10a1  .|.|.f...d.t....
-00000440: 0076 0073 f174 0da0 1174 0ba1 0172 f674  .v.s.t...t...r.t
-00000450: 0da0 1274 0ba1 016e 0164 1164 1874 0fa0  ...t...n.d.d.t..
-00000460: 10a1 0076 0090 0173 0474 0da0 117c 09a1  ...v...s.t...|..
-00000470: 0190 0172 0974 0da0 127c 09a1 016e 0164  ...r.t...|...n.d
-00000480: 1874 0da0 127c 0aa1 0164 1174 0fa0 10a1  .t...|...d.t....
-00000490: 0076 0090 0173 1b74 0da0 1174 0ba1 0190  .v...s.t...t....
-000004a0: 0172 2074 0da0 1274 0ba1 016e 0164 1164  .r t...t...n.d.d
-000004b0: 1374 0fa0 10a1 0076 0090 0173 2e74 0da0  .t.....v...s.t..
-000004c0: 117c 02a1 0190 0172 3374 0da0 127c 02a1  .|.....r3t...|..
-000004d0: 016e 0164 1374 0da0 127c 0ba1 0174 0da0  .n.d.t...|...t..
-000004e0: 127c 0ca1 0164 149c 0716 007d 0e64 1564  .|...d.....}.d.d
-000004f0: 167c 0e69 0116 007d 0f74 1374 0da0 147c  .|.i...}.t.t...|
-00000500: 0fa1 0183 0182 0164 1704 007d 0a04 007d  .......d...}...}
-00000510: 0d04 007d 0b7d 0c64 1753 0029 197a 2254  ...}.}.d.S.).z"T
-00000520: 6573 7420 7468 6174 2074 6573 7473 2074  est that tests t
-00000530: 6865 2042 6c75 6543 6173 7420 636c 6173  he BlueCast clas
-00000540: 7372 0100 0000 e901 0000 00e9 6400 0000  sr..........d...
-00000550: e910 0000 00e9 0a00 0000 6300 0000 0000  ..........c.....
-00000560: 0000 0000 0000 0000 0000 000c 0000 0040  ...............@
-00000570: 0000 0073 8000 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000580: 6401 6503 6a04 6402 6503 6a04 6604 6403  d.e.j.d.e.j.f.d.
-00000590: 6404 8404 5a05 6401 6503 6a04 6405 6503  d...Z.d.e.j.d.e.
-000005a0: 6a06 6402 6507 6503 6a04 6503 6a06 6602  j.d.e.e.j.e.j.f.
-000005b0: 1900 6606 6406 6407 8404 5a08 0908 0909  ..f.d.d...Z.....
-000005c0: 640d 6401 6503 6a04 6405 6509 6503 6a06  d.d.e.j.d.e.e.j.
-000005d0: 1900 640a 650a 6402 6507 6503 6a04 6509  ..d.e.d.e.e.j.e.
-000005e0: 6503 6a06 1900 6602 1900 6608 640b 640c  e.j...f...f.d.d.
-000005f0: 8405 5a0b 6408 5300 290e 7a35 7465 7374  ..Z.d.S.).z5test
-00000600: 5f62 6c75 6570 7269 6e74 5f78 6762 6f6f  _blueprint_xgboo
-00000610: 7374 2e3c 6c6f 6361 6c73 3e2e 4d79 4375  st.<locals>.MyCu
-00000620: 7374 6f6d 5072 6570 726f 6365 7373 696e  stomPreprocessin
-00000630: 67da 0264 6672 0a00 0000 6302 0000 0000  g..dfr....c.....
-00000640: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00000650: 0000 0073 1400 0000 7c01 6401 1b00 7d01  ...s....|.d...}.
-00000660: 6402 7c01 6403 3c00 7c01 5300 2904 4ee9  d.|.d.<.|.S.).N.
-00000670: 0200 0000 e905 0000 005a 0a63 7573 746f  .........Z.custo
-00000680: 6d5f 636f 6c72 0f00 0000 2902 da04 7365  m_colr....)...se
-00000690: 6c66 7216 0000 0072 0f00 0000 720f 0000  lfr....r....r...
-000006a0: 0072 1000 0000 da0f 6375 7374 6f6d 5f66  .r......custom_f
-000006b0: 756e 6374 696f 6e1f 0000 0073 0600 0000  unction....s....
-000006c0: 0801 0801 0401 7a45 7465 7374 5f62 6c75  ......zEtest_blu
-000006d0: 6570 7269 6e74 5f78 6762 6f6f 7374 2e3c  eprint_xgboost.<
-000006e0: 6c6f 6361 6c73 3e2e 4d79 4375 7374 6f6d  locals>.MyCustom
-000006f0: 5072 6570 726f 6365 7373 696e 672e 6375  Preprocessing.cu
-00000700: 7374 6f6d 5f66 756e 6374 696f 6eda 0674  stom_function..t
-00000710: 6172 6765 7463 0300 0000 0000 0000 0000  argetc..........
-00000720: 0000 0300 0000 0300 0000 5300 0000 7326  ..........S...s&
-00000730: 0000 007c 00a0 007c 01a1 017d 017c 01a0  ...|...|...}.|..
-00000740: 0164 01a1 017d 017c 02a0 0164 01a1 017d  .d...}.|...d...}
-00000750: 027c 017c 0266 0253 0029 024e 69e8 0300  .|.|.f.S.).Ni...
-00000760: 0029 0272 1a00 0000 da04 6865 6164 2903  .).r......head).
-00000770: 7219 0000 0072 1600 0000 721b 0000 0072  r....r....r....r
-00000780: 0f00 0000 720f 0000 0072 1000 0000 da0d  ....r....r......
-00000790: 6669 745f 7472 616e 7366 6f72 6d24 0000  fit_transform$..
-000007a0: 0073 0800 0000 0a03 0a01 0a01 0801 7a43  .s............zC
-000007b0: 7465 7374 5f62 6c75 6570 7269 6e74 5f78  test_blueprint_x
-000007c0: 6762 6f6f 7374 2e3c 6c6f 6361 6c73 3e2e  gboost.<locals>.
-000007d0: 4d79 4375 7374 6f6d 5072 6570 726f 6365  MyCustomPreproce
-000007e0: 7373 696e 672e 6669 745f 7472 616e 7366  ssing.fit_transf
-000007f0: 6f72 6d4e 46da 0e70 7265 6469 6374 6f6e  ormNF..predicton
-00000800: 5f6d 6f64 6563 0400 0000 0000 0000 0000  _modec..........
-00000810: 0000 0400 0000 0300 0000 5300 0000 7336  ..........S...s6
-00000820: 0000 007c 00a0 007c 01a1 017d 017c 0373  ...|...|...}.|.s
-00000830: 1774 017c 0274 026a 0383 0272 177c 01a0  .t.|.t.j...r.|..
-00000840: 0464 01a1 017d 017c 02a0 0464 01a1 017d  .d...}.|...d...}
-00000850: 027c 017c 0266 0253 0029 024e 7213 0000  .|.|.f.S.).Nr...
-00000860: 0029 0572 1a00 0000 da0a 6973 696e 7374  .).r......isinst
-00000870: 616e 6365 da02 7064 da06 5365 7269 6573  ance..pd..Series
-00000880: 721c 0000 0029 0472 1900 0000 7216 0000  r....).r....r...
-00000890: 0072 1b00 0000 721e 0000 0072 0f00 0000  .r....r....r....
-000008a0: 720f 0000 0072 1000 0000 da09 7472 616e  r....r......tran
-000008b0: 7366 6f72 6d2c 0000 0073 0a00 0000 0a06  sform,...s......
-000008c0: 1001 0a01 0a01 0801 7a3f 7465 7374 5f62  ........z?test_b
-000008d0: 6c75 6570 7269 6e74 5f78 6762 6f6f 7374  lueprint_xgboost
-000008e0: 2e3c 6c6f 6361 6c73 3e2e 4d79 4375 7374  .<locals>.MyCust
-000008f0: 6f6d 5072 6570 726f 6365 7373 696e 672e  omPreprocessing.
-00000900: 7472 616e 7366 6f72 6d29 024e 4629 0cda  transform).NF)..
-00000910: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000920: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000930: 655f 5f72 2000 0000 da09 4461 7461 4672  e__r .....DataFr
-00000940: 616d 6572 1a00 0000 7221 0000 0072 0300  amer....r!...r..
-00000950: 0000 721d 0000 0072 0200 0000 da04 626f  ..r....r......bo
-00000960: 6f6c 7222 0000 0072 0f00 0000 720f 0000  olr"...r....r...
-00000970: 0072 0f00 0000 7210 0000 00da 154d 7943  .r....r......MyC
-00000980: 7573 746f 6d50 7265 7072 6f63 6573 7369  ustomPreprocessi
-00000990: 6e67 1e00 0000 7328 0000 0008 0016 0102  ng....s(........
-000009a0: 0504 0102 ff04 0102 ff0e 020a fe02 0b02  ................
-000009b0: 0104 fc04 0202 fe08 0302 fd02 0402 fc12  ................
-000009c0: 050e fb72 2800 0000 da06 6269 6e61 7279  ...r(.....binary
-000009d0: 721b 0000 0029 055a 0d63 6c61 7373 5f70  r....).Z.class_p
-000009e0: 726f 626c 656d 5a0d 7461 7267 6574 5f63  roblemZ.target_c
-000009f0: 6f6c 756d 6e5a 0d63 6f6e 665f 7472 6169  olumnZ.conf_trai
-00000a00: 6e69 6e67 5a0c 636f 6e66 5f78 6762 6f6f  ningZ.conf_xgboo
-00000a10: 7374 da13 6375 7374 6f6d 5f70 7265 7072  st..custom_prepr
-00000a20: 6f63 6573 736f 7229 015a 0a74 6172 6765  ocessor).Z.targe
-00000a30: 745f 636f 6c7a 1641 7574 6f74 756e 696e  t_colz.Autotunin
-00000a40: 6720 7375 6363 6573 7366 756c 2e29 015a  g successful.).Z
-00000a50: 0461 7869 737a 1650 7265 6469 6374 696e  .axisz.Predictin
-00000a60: 6720 7375 6363 6573 7366 756c 2e29 01fa  g successful.)..
-00000a70: 023d 3d29 017a 6b25 2870 7933 2973 0a7b  .==).zk%(py3)s.{
-00000a80: 2528 7079 3329 7320 3d20 2528 7079 3029  %(py3)s = %(py0)
-00000a90: 7328 2528 7079 3129 7329 0a7d 203d 3d20  s(%(py1)s).} == 
-00000aa0: 2528 7079 3130 2973 0a7b 2528 7079 3130  %(py10)s.{%(py10
-00000ab0: 2973 203d 2025 2870 7935 2973 2825 2870  )s = %(py5)s(%(p
-00000ac0: 7938 2973 0a7b 2528 7079 3829 7320 3d20  y8)s.{%(py8)s = 
-00000ad0: 2528 7079 3629 732e 696e 6465 780a 7d29  %(py6)s.index.})
-00000ae0: 0a7d da03 6c65 6eda 0779 5f70 726f 6273  .}..len..y_probs
-00000af0: 720e 0000 0029 075a 0370 7930 5a03 7079  r....).Z.py0Z.py
-00000b00: 315a 0370 7933 5a03 7079 355a 0370 7936  1Z.py3Z.py5Z.py6
-00000b10: 5a03 7079 385a 0470 7931 307a 0f61 7373  Z.py8Z.py10z.ass
-00000b20: 6572 7420 2528 7079 3132 2973 5a04 7079  ert %(py12)sZ.py
-00000b30: 3132 4eda 0979 5f63 6c61 7373 6573 2915  12N..y_classes).
-00000b40: 7206 0000 005a 0973 7465 7073 5f6d 6178  r....Z.steps_max
-00000b50: 5a0e 6e75 6d5f 6c65 6176 6573 5f6d 6178  Z.num_leaves_max
-00000b60: 7205 0000 005a 1c68 7970 6572 7061 7261  r....Z.hyperpara
-00000b70: 6d65 7465 725f 7475 6e69 6e67 5f72 6f75  meter_tuning_rou
-00000b80: 6e64 7372 0700 0000 7204 0000 005a 0366  ndsr....r....Z.f
-00000b90: 6974 da05 7072 696e 745a 0770 7265 6469  it..printZ.predi
-00000ba0: 6374 5a04 6472 6f70 722c 0000 00da 0569  ctZ.dropr,.....i
-00000bb0: 6e64 6578 da0a 4070 7974 6573 745f 6172  ndex..@pytest_ar
-00000bc0: da11 5f63 616c 6c5f 7265 7072 636f 6d70  .._call_reprcomp
-00000bd0: 6172 65da 0c40 7079 5f62 7569 6c74 696e  are..@py_builtin
-00000be0: 73da 066c 6f63 616c 73da 185f 7368 6f75  s..locals.._shou
-00000bf0: 6c64 5f72 6570 725f 676c 6f62 616c 5f6e  ld_repr_global_n
-00000c00: 616d 65da 095f 7361 6665 7265 7072 da0e  ame.._saferepr..
-00000c10: 4173 7365 7274 696f 6e45 7272 6f72 da13  AssertionError..
-00000c20: 5f66 6f72 6d61 745f 6578 706c 616e 6174  _format_explanat
-00000c30: 696f 6e29 1072 1100 0000 720d 0000 0072  ion).r....r....r
-00000c40: 0e00 0000 5a14 7867 626f 6f73 745f 7061  ....Z.xgboost_pa
-00000c50: 7261 6d5f 636f 6e66 6967 5a0c 7472 6169  ram_configZ.trai
-00000c60: 6e5f 636f 6e66 6967 7228 0000 0072 2a00  n_configr(...r*.
-00000c70: 0000 5a06 6175 746f 6d6c 722d 0000 0072  ..Z.automlr-...r
-00000c80: 2e00 0000 5a0b 4070 795f 6173 7365 7274  ....Z.@py_assert
-00000c90: 325a 0b40 7079 5f61 7373 6572 7437 5a0b  2Z.@py_assert7Z.
-00000ca0: 4070 795f 6173 7365 7274 395a 0b40 7079  @py_assert9Z.@py
-00000cb0: 5f61 7373 6572 7434 5a0c 4070 795f 666f  _assert4Z.@py_fo
-00000cc0: 726d 6174 3131 5a0c 4070 795f 666f 726d  rmat11Z.@py_form
-00000cd0: 6174 3133 720f 0000 0072 0f00 0000 7210  at13r....r....r.
-00000ce0: 0000 00da 1674 6573 745f 626c 7565 7072  .....test_bluepr
-00000cf0: 696e 745f 7867 626f 6f73 7413 0000 0073  int_xgboost....s
-00000d00: 3000 0000 0802 0801 0601 0601 0601 0601  0...............
-00000d10: 0601 1003 061a 0202 0201 0201 0201 0201  ................
-00000d20: 0201 06fb 0e07 0801 1801 0801 fe01 0a00  ................
-00000d30: fe01 1c00 7239 0000 0029 19da 0862 7569  ....r9...)...bui
-00000d40: 6c74 696e 7372 3300 0000 da19 5f70 7974  ltinsr3....._pyt
-00000d50: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
-00000d60: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
-00000d70: da07 7265 7772 6974 6572 3100 0000 da06  ..rewriter1.....
-00000d80: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000d90: 5a06 7061 6e64 6173 7220 0000 00da 0670  Z.pandasr .....p
-00000da0: 7974 6573 745a 1862 6c75 6563 6173 742e  ytestZ.bluecast.
-00000db0: 626c 7565 7072 696e 7473 2e63 6173 7472  blueprints.castr
-00000dc0: 0400 0000 5a1f 626c 7565 6361 7374 2e63  ....Z.bluecast.c
-00000dd0: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
-00000de0: 6f6e 6669 6772 0500 0000 7206 0000 005a  onfigr....r....Z
-00000df0: 1d62 6c75 6563 6173 742e 7072 6570 726f  .bluecast.prepro
-00000e00: 6365 7373 696e 672e 6375 7374 6f6d 7207  cessing.customr.
-00000e10: 0000 005a 2462 6c75 6563 6173 742e 7465  ...Z$bluecast.te
-00000e20: 7374 732e 6d61 6b65 5f64 6174 612e 6372  sts.make_data.cr
-00000e30: 6561 7465 5f64 6174 6172 0900 0000 da07  eate_datar......
-00000e40: 6669 7874 7572 6572 2600 0000 7211 0000  fixturer&...r...
-00000e50: 0072 3900 0000 720f 0000 0072 0f00 0000  .r9...r....r....
-00000e60: 720f 0000 0072 1000 0000 da08 3c6d 6f64  r....r......<mod
-00000e70: 756c 653e 0100 0000 7314 0000 002a 0008  ule>....s....*..
-00000e80: 0208 010c 0210 010c 010c 0104 031c 010c  ................
-00000e90: 06                                       .
+00000050: 5a07 0100 6400 6401 6c08 5a09 6400 6401  Z...d.d.l.Z.d.d.
+00000060: 6c0a 5a0b 6400 6401 6c0c 5a0c 6400 6403  l.Z.d.d.l.Z.d.d.
+00000070: 6c0d 6d0e 5a0e 0100 6400 6404 6c0f 6d10  l.m.Z...d.d.l.m.
+00000080: 5a10 6d11 5a11 0100 6400 6405 6c12 6d13  Z.m.Z...d.d.l.m.
+00000090: 5a13 0100 6400 6406 6c14 6d15 5a15 0100  Z...d.d.l.m.Z...
+000000a0: 6400 6407 6c16 6d17 5a17 0100 650c 6a18  d.d.l.m.Z...e.j.
+000000b0: 6408 6409 8400 8301 5a19 650c 6a18 640a  d.d.....Z.e.j.d.
+000000c0: 640b 8400 8301 5a1a 640c 640d 8400 5a1b  d.....Z.d.d...Z.
+000000d0: 640e 640f 8400 5a1c 6410 6411 8400 5a1d  d.d...Z.d.d...Z.
+000000e0: 6401 5300 2912 e900 0000 004e 2901 da04  d.S.)......N)...
+000000f0: 6d6f 636b 2901 da08 426c 7565 4361 7374  mock)...BlueCast
+00000100: 2902 da0e 5472 6169 6e69 6e67 436f 6e66  )...TrainingConf
+00000110: 6967 da17 5867 626f 6f73 7454 756e 6550  ig..XgboostTuneP
+00000120: 6172 616d 7343 6f6e 6669 6729 01da 116d  aramsConfig)...m
+00000130: 6174 7468 6577 735f 636f 7272 636f 6566  atthews_corrcoef
+00000140: 2901 da11 7368 6170 5f65 7870 6c61 6e61  )...shap_explana
+00000150: 7469 6f6e 7329 01da 1a63 7265 6174 655f  tions)...create_
+00000160: 7379 6e74 6865 7469 635f 6461 7461 6672  synthetic_datafr
+00000170: 616d 6563 0000 0000 0000 0000 0000 0000  amec............
+00000180: 0000 0000 0200 0000 4300 0000 7308 0000  ........C...s...
+00000190: 0074 00a0 01a1 0053 0029 014e 2902 7202  .t.....S.).N).r.
+000001a0: 0000 005a 044d 6f63 6ba9 0072 0900 0000  ...Z.Mock..r....
+000001b0: 7209 0000 00fa 4b2f 686f 6d65 2f74 686f  r.....K/home/tho
+000001c0: 6d61 732f 4964 6561 5072 6f6a 6563 7473  mas/IdeaProjects
+000001d0: 2f42 6c75 6543 6173 742f 626c 7565 6361  /BlueCast/blueca
+000001e0: 7374 2f74 6573 7473 2f74 6573 745f 7368  st/tests/test_sh
+000001f0: 6170 5f65 7870 6c61 6e61 7469 6f6e 732e  ap_explanations.
+00000200: 7079 da0a 6d6f 636b 5f6d 6f64 656c 0e00  py..mock_model..
+00000210: 0000 7302 0000 0008 0272 0b00 0000 6300  ..s......r....c.
+00000220: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00000230: 0000 0043 0000 0073 1800 0000 7400 a001  ...C...s....t...
+00000240: 6700 6401 a201 6700 6402 a201 6403 9c02  g.d...g.d...d...
+00000250: a101 5300 2904 4e29 03e9 0100 0000 e902  ..S.).N)........
+00000260: 0000 00e9 0300 0000 2903 e904 0000 00e9  ........).......
+00000270: 0500 0000 e906 0000 0029 025a 0866 6561  .........).Z.fea
+00000280: 7475 7265 315a 0866 6561 7475 7265 3229  ture1Z.feature2)
+00000290: 02da 0270 64da 0944 6174 6146 7261 6d65  ...pd..DataFrame
+000002a0: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+000002b0: 0a00 0000 da09 7465 7374 5f64 6174 6113  ......test_data.
+000002c0: 0000 0073 0200 0000 1802 7214 0000 0063  ...s......r....c
+000002d0: 0000 0000 0000 0000 0000 0000 0800 0000  ................
+000002e0: 0700 0000 4300 0000 730a 0100 0074 0064  ....C...s....t.d
+000002f0: 0164 0264 038d 027d 0074 0064 0464 0564  .d.d...}.t.d.d.d
+00000300: 038d 027d 0174 0183 007d 0264 047c 025f  ...}.t...}.d.|._
+00000310: 0264 067c 025f 0374 0483 007d 0364 077c  .d.|._.t...}.d.|
+00000320: 035f 0574 0664 0864 097c 037c 0264 0a8d  ._.t.d.d.|.|.d..
+00000330: 047d 047c 046a 077c 007c 016a 0864 0964  .}.|.j.|.|.j.d.d
+00000340: 0b64 0c8d 027c 0164 0919 0064 0964 0d8d  .d...|.d...d.d..
+00000350: 047d 0574 097c 0583 0101 0074 0a7c 0574  .}.t.|.....t.|.t
+00000360: 0b83 027d 067c 0673 8164 0e64 0f74 0ca0  ...}.|.s.d.d.t..
+00000370: 0da1 0076 0073 4a74 0ea0 0f74 0aa1 0172  ...v.sJt...t...r
+00000380: 4f74 0ea0 1074 0aa1 016e 0164 0f64 1074  Ot...t...n.d.d.t
+00000390: 0ca0 0da1 0076 0073 5b74 0ea0 0f7c 05a1  .....v.s[t...|..
+000003a0: 0172 6074 0ea0 107c 05a1 016e 0164 1064  .r`t...|...n.d.d
+000003b0: 1174 0ca0 0da1 0076 0073 6c74 0ea0 0f74  .t.....v.slt...t
+000003c0: 0ba1 0172 7174 0ea0 1074 0ba1 016e 0164  ...rqt...t...n.d
+000003d0: 1174 0ea0 107c 06a1 0164 129c 0416 007d  .t...|...d.....}
+000003e0: 0774 1174 0ea0 127c 07a1 0183 0182 0164  .t.t...|.......d
+000003f0: 137d 0664 1353 0029 147a 2254 6573 7420  .}.d.S.).z"Test 
+00000400: 7468 6174 2074 6573 7473 2074 6865 2042  that tests the B
+00000410: 6c75 6543 6173 7420 636c 6173 73e9 c800  lueCast class...
+00000420: 0000 e914 0000 0029 01da 0c72 616e 646f  .......)...rando
+00000430: 6d5f 7374 6174 65e9 6400 0000 e915 0000  m_state.d.......
+00000440: 00e9 1000 0000 e90a 0000 00da 0662 696e  .............bin
+00000450: 6172 79da 0674 6172 6765 7429 04da 0d63  ary..target)...c
+00000460: 6c61 7373 5f70 726f 626c 656d da0d 7461  lass_problem..ta
+00000470: 7267 6574 5f63 6f6c 756d 6eda 0d63 6f6e  rget_column..con
+00000480: 665f 7472 6169 6e69 6e67 da0c 636f 6e66  f_training..conf
+00000490: 5f78 6762 6f6f 7374 720c 0000 0029 01da  _xgboostr....)..
+000004a0: 0461 7869 7329 01da 0a74 6172 6765 745f  .axis)...target_
+000004b0: 636f 6c7a 3561 7373 6572 7420 2528 7079  colz5assert %(py
+000004c0: 3429 730a 7b25 2870 7934 2973 203d 2025  4)s.{%(py4)s = %
+000004d0: 2870 7930 2973 2825 2870 7931 2973 2c20  (py0)s(%(py1)s, 
+000004e0: 2528 7079 3229 7329 0a7d da0a 6973 696e  %(py2)s).}..isin
+000004f0: 7374 616e 6365 da09 6576 616c 5f64 6963  stance..eval_dic
+00000500: 74da 0464 6963 7429 04da 0370 7930 da03  t..dict)...py0..
+00000510: 7079 31da 0370 7932 da03 7079 344e 2913  py1..py2..py4N).
+00000520: 7208 0000 0072 0500 0000 da09 7374 6570  r....r......step
+00000530: 735f 6d61 78da 0e6e 756d 5f6c 6561 7665  s_max..num_leave
+00000540: 735f 6d61 7872 0400 0000 da1c 6879 7065  s_maxr......hype
+00000550: 7270 6172 616d 6574 6572 5f74 756e 696e  rparameter_tunin
+00000560: 675f 726f 756e 6473 7203 0000 00da 0866  g_roundsr......f
+00000570: 6974 5f65 7661 6cda 0464 726f 70da 0570  it_eval..drop..p
+00000580: 7269 6e74 7224 0000 0072 2600 0000 da0c  rintr$...r&.....
+00000590: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
+000005a0: 6361 6c73 da0a 4070 7974 6573 745f 6172  cals..@pytest_ar
+000005b0: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
+000005c0: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
+000005d0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
+000005e0: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
+000005f0: 7870 6c61 6e61 7469 6f6e 2908 da08 6466  xplanation)...df
+00000600: 5f74 7261 696e da06 6466 5f76 616c da14  _train..df_val..
+00000610: 7867 626f 6f73 745f 7061 7261 6d5f 636f  xgboost_param_co
+00000620: 6e66 6967 da0c 7472 6169 6e5f 636f 6e66  nfig..train_conf
+00000630: 6967 da06 6175 746f 6d6c 7225 0000 00da  ig..automlr%....
+00000640: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
+00000650: 795f 666f 726d 6174 3572 0900 0000 7209  y_format5r....r.
+00000660: 0000 0072 0a00 0000 da16 7465 7374 5f73  ...r......test_s
+00000670: 6861 705f 6578 706c 616e 6174 696f 6e73  hap_explanations
+00000680: 1800 0000 7324 0000 000c 020c 0106 0106  ....s$..........
+00000690: 0106 0106 0106 0102 0202 0102 0102 0102  ................
+000006a0: 0106 fc04 0616 0106 ff08 039c 0172 3f00  .............r?.
+000006b0: 0000 6302 0000 0000 0000 0000 0000 0013  ..c.............
+000006c0: 0000 0009 0000 0043 0000 0073 ee01 0000  .......C...s....
+000006d0: 6401 7d02 7400 a001 6402 a101 8fe6 7d03  d.}.t...d.....}.
+000006e0: 7400 a001 6403 a101 8fc8 7d04 7402 a003  t...d.....}.t...
+000006f0: 6404 6405 6702 6406 6407 6702 6408 6409  d.d.g.d.d.g.d.d.
+00000700: 6702 6703 a101 7c03 6a04 6a05 5f04 7406  g.g...|.j.j._.t.
+00000710: 7c00 7c01 7c02 8303 7d05 7c03 a007 7c00  |.|.|...}.|...|.
+00000720: 6a08 7c01 a102 0100 7c04 a009 a100 0100  j.|.....|.......
+00000730: 6700 7d06 6400 7d07 7c05 7c07 7501 7d08  g.}.d.}.|.|.u.}.
+00000740: 7c08 7d09 7c08 7247 7c05 6a0a 7d0a 640a  |.}.|.rG|.j.}.d.
+00000750: 7d0b 7c0a 7c0b 6b04 7d0c 7c0c 7d09 7c09  }.|.|.k.}.|.}.|.
+00000760: 73c0 740b a00c 640b 7c08 6601 640c 7c05  s.t...d.|.f.d.|.
+00000770: 7c07 6602 a104 640d 740d a00e a100 7600  |.f...d.t.....v.
+00000780: 735e 740b a00f 7c05 a101 7263 740b a010  s^t...|...rct...
+00000790: 7c05 a101 6e01 640d 740b a010 7c07 a101  |...n.d.t...|...
+000007a0: 640e 9c02 1600 7d0d 640f 6410 7c0d 6901  d.....}.d.d.|.i.
+000007b0: 1600 7d0e 7c06 a011 7c0e a101 0100 7c08  ..}.|...|.....|.
+000007c0: 72ab 740b a00c 6411 7c0c 6601 6412 7c0a  r.t...d.|.f.d.|.
+000007d0: 7c0b 6602 a104 640d 740d a00e a100 7600  |.f...d.t.....v.
+000007e0: 738e 740b a00f 7c05 a101 7293 740b a010  s.t...|...r.t...
+000007f0: 7c05 a101 6e01 640d 740b a010 7c0a a101  |...n.d.t...|...
+00000800: 740b a010 7c0b a101 6413 9c03 1600 7d0f  t...|...d.....}.
+00000810: 6414 6415 7c0f 6901 1600 7d10 7c06 a011  d.d.|.i...}.|...
+00000820: 7c10 a101 0100 740b a012 7c06 640a a102  |.....t...|.d...
+00000830: 6900 1600 7d11 6416 6417 7c11 6901 1600  i...}.d.d.|.i...
+00000840: 7d12 7413 740b a014 7c12 a101 8301 8201  }.t.t...|.......
+00000850: 6400 0400 7d09 0400 7d06 0400 7d08 0400  d...}...}...}...
+00000860: 7d07 0400 7d0a 0400 7d0c 7d0b 5700 6400  }...}...}.}.W.d.
+00000870: 0400 0400 8303 0100 6e10 3100 73d8 7701  ........n.1.s.w.
+00000880: 0100 0100 0100 5900 0100 5700 6400 0400  ......Y...W.d...
+00000890: 0400 8303 0100 6400 5300 5700 6400 0400  ......d.S.W.d...
+000008a0: 0400 8303 0100 6400 5300 3100 73f0 7701  ......d.S.1.s.w.
+000008b0: 0100 0100 0100 5900 0100 6400 5300 2918  ......Y...d.S.).
+000008c0: 4eda 056f 7468 6572 7a34 626c 7565 6361  N..otherz4blueca
+000008d0: 7374 2e65 7661 6c75 6174 696f 6e2e 7368  st.evaluation.sh
+000008e0: 6170 5f76 616c 7565 732e 7368 6170 2e4b  ap_values.shap.K
+000008f0: 6572 6e65 6c45 7870 6c61 696e 6572 7a16  ernelExplainerz.
+00000900: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
+00000910: 742e 7368 6f77 679a 9999 9999 99b9 3f67  t.showg.......?g
+00000920: 9a99 9999 9999 c93f 6733 3333 3333 33d3  .......?g333333.
+00000930: 3f67 9a99 9999 9999 d93f 6700 0000 0000  ?g.......?g.....
+00000940: 00e0 3f67 3333 3333 3333 e33f 7201 0000  ..?g333333.?r...
+00000950: 0029 01fa 0669 7320 6e6f 7429 017a 1625  .)...is not).z.%
+00000960: 2870 7932 2973 2069 7320 6e6f 7420 2528  (py2)s is not %(
+00000970: 7079 3529 73da 0b73 6861 705f 7661 6c75  py5)s..shap_valu
+00000980: 6573 2902 7229 0000 00da 0370 7935 7a07  es).r).....py5z.
+00000990: 2528 7079 3729 73da 0370 7937 2901 fa01  %(py7)s..py7)...
+000009a0: 3e29 017a 2e25 2870 7931 3129 730a 7b25  >).z.%(py11)s.{%
+000009b0: 2870 7931 3129 7320 3d20 2528 7079 3929  (py11)s = %(py9)
+000009c0: 732e 7369 7a65 0a7d 203e 2025 2870 7931  s.size.} > %(py1
+000009d0: 3429 7329 03da 0370 7939 da04 7079 3131  4)s)...py9..py11
+000009e0: da04 7079 3134 7a08 2528 7079 3136 2973  ..py14z.%(py16)s
+000009f0: da04 7079 3136 7a0f 6173 7365 7274 2025  ..py16z.assert %
+00000a00: 2870 7931 3929 735a 0470 7931 3929 1572  (py19)sZ.py19).r
+00000a10: 0200 0000 da05 7061 7463 68da 026e 70da  ......patch..np.
+00000a20: 0561 7272 6179 da0c 7265 7475 726e 5f76  .array..return_v
+00000a30: 616c 7565 7242 0000 0072 0700 0000 5a17  aluerB...r....Z.
+00000a40: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
+00000a50: 6365 5f77 6974 68da 0770 7265 6469 6374  ce_with..predict
+00000a60: 5a12 6173 7365 7274 5f63 616c 6c65 645f  Z.assert_called_
+00000a70: 6f6e 6365 da04 7369 7a65 7233 0000 00da  once..sizer3....
+00000a80: 115f 6361 6c6c 5f72 6570 7263 6f6d 7061  ._call_reprcompa
+00000a90: 7265 7231 0000 0072 3200 0000 7234 0000  rer1...r2...r4..
+00000aa0: 0072 3500 0000 da06 6170 7065 6e64 da0e  .r5.....append..
+00000ab0: 5f66 6f72 6d61 745f 626f 6f6c 6f70 7236  _format_boolopr6
+00000ac0: 0000 0072 3700 0000 2913 720b 0000 0072  ...r7...).r....r
+00000ad0: 1400 0000 da09 6578 706c 6169 6e65 725a  ......explainerZ
+00000ae0: 156d 6f63 6b5f 6b65 726e 656c 5f65 7870  .mock_kernel_exp
+00000af0: 6c61 696e 6572 5a09 6d6f 636b 5f73 686f  lainerZ.mock_sho
+00000b00: 7772 4200 0000 da0b 4070 795f 6173 7365  wrB.....@py_asse
+00000b10: 7274 31da 0b40 7079 5f61 7373 6572 7434  rt1..@py_assert4
+00000b20: 723d 0000 00da 0b40 7079 5f61 7373 6572  r=.....@py_asser
+00000b30: 7430 da0c 4070 795f 6173 7365 7274 3130  t0..@py_assert10
+00000b40: da0c 4070 795f 6173 7365 7274 3133 da0c  ..@py_assert13..
+00000b50: 4070 795f 6173 7365 7274 3132 da0b 4070  @py_assert12..@p
+00000b60: 795f 666f 726d 6174 36da 0b40 7079 5f66  y_format6..@py_f
+00000b70: 6f72 6d61 7438 5a0c 4070 795f 666f 726d  ormat8Z.@py_form
+00000b80: 6174 3135 da0c 4070 795f 666f 726d 6174  at15..@py_format
+00000b90: 3137 5a0c 4070 795f 666f 726d 6174 3138  17Z.@py_format18
+00000ba0: 5a0c 4070 795f 666f 726d 6174 3230 7209  Z.@py_format20r.
+00000bb0: 0000 0072 0900 0000 720a 0000 00da 1b74  ...r....r......t
+00000bc0: 6573 745f 7368 6170 5f65 7870 6c61 6e61  est_shap_explana
+00000bd0: 7469 6f6e 735f 656c 7365 2f00 0000 7320  tions_else/...s 
+00000be0: 0000 0004 0104 0102 0104 ff0a 0202 fe02  ................
+00000bf0: 0204 0114 010a ff0c 040e 0208 01fe 0240  ...............@
+00000c00: 0050 f472 5d00 0000 6300 0000 0000 0000  .P.r]...c.......
+00000c10: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
+00000c20: 0073 a200 0000 7400 a001 6700 6401 a201  .s....t...g.d...
+00000c30: a101 7d00 7400 a001 6700 6402 a201 a101  ..}.t...g.d.....
+00000c40: 7d01 7402 7c00 7c01 8302 7d02 6403 7d03  }.t.|.|...}.d.}.
+00000c50: 7c02 7c03 6b02 7d04 7c04 734b 7403 a004  |.|.k.}.|.sKt...
+00000c60: 6404 7c04 6601 6405 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
+00000c70: 6406 7405 a006 a100 7600 7330 7403 a007  d.t.....v.s0t...
+00000c80: 7c02 a101 7235 7403 a008 7c02 a101 6e01  |...r5t...|...n.
+00000c90: 6406 7403 a008 7c03 a101 6407 9c02 1600  d.t...|...d.....
+00000ca0: 7d05 6408 6409 7c05 6901 1600 7d06 7409  }.d.d.|.i...}.t.
+00000cb0: 7403 a00a 7c06 a101 8301 8201 6400 0400  t...|.......d...
+00000cc0: 7d04 7d03 6400 5300 290a 4e29 0472 0100  }.}.d.S.).N).r..
+00000cd0: 0000 7201 0000 0072 0100 0000 7201 0000  ..r....r....r...
+00000ce0: 0029 0472 0c00 0000 720c 0000 0072 0c00  .).r....r....r..
+00000cf0: 0000 720c 0000 0072 0100 0000 2901 fa02  ..r....r....)...
+00000d00: 3d3d 2901 7a12 2528 7079 3029 7320 3d3d  ==).z.%(py0)s ==
+00000d10: 2025 2870 7933 2973 da06 7265 7375 6c74   %(py3)s..result
+00000d20: 2902 7227 0000 00da 0370 7933 7a0e 6173  ).r'.....py3z.as
+00000d30: 7365 7274 2025 2870 7935 2973 7243 0000  sert %(py5)srC..
+00000d40: 0029 0b72 4b00 0000 724c 0000 0072 0600  .).rK...rL...r..
+00000d50: 0000 7233 0000 0072 5000 0000 7231 0000  ..r3...rP...r1..
+00000d60: 0072 3200 0000 7234 0000 0072 3500 0000  .r2...r4...r5...
+00000d70: 7236 0000 0072 3700 0000 2907 da06 795f  r6...r7...)...y_
+00000d80: 7472 7565 da09 795f 636c 6173 7365 7372  true..y_classesr
+00000d90: 5f00 0000 da0b 4070 795f 6173 7365 7274  _.....@py_assert
+00000da0: 3272 5400 0000 da0b 4070 795f 666f 726d  2rT.....@py_form
+00000db0: 6174 3472 5a00 0000 7209 0000 0072 0900  at4rZ...r....r..
+00000dc0: 0000 720a 0000 00da 1b74 6573 745f 6576  ..r......test_ev
+00000dd0: 616c 5f63 6c61 7373 6966 6965 725f 6578  al_classifier_ex
+00000de0: 6365 7074 4000 0000 7308 0000 000e 010e  cept@...s.......
+00000df0: 010a 017c 0172 6500 0000 291e da08 6275  ...|.re...)...bu
+00000e00: 696c 7469 6e73 7231 0000 00da 195f 7079  iltinsr1....._py
+00000e10: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
+00000e20: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
+00000e30: 6eda 0772 6577 7269 7465 7233 0000 00da  n..rewriter3....
+00000e40: 0875 6e69 7474 6573 7472 0200 0000 da05  .unittestr......
+00000e50: 6e75 6d70 7972 4b00 0000 da06 7061 6e64  numpyrK.....pand
+00000e60: 6173 7212 0000 00da 0670 7974 6573 74da  asr......pytest.
+00000e70: 1862 6c75 6563 6173 742e 626c 7565 7072  .bluecast.bluepr
+00000e80: 696e 7473 2e63 6173 7472 0300 0000 da1f  ints.castr......
+00000e90: 626c 7565 6361 7374 2e63 6f6e 6669 672e  bluecast.config.
+00000ea0: 7472 6169 6e69 6e67 5f63 6f6e 6669 6772  training_configr
+00000eb0: 0400 0000 7205 0000 00da 2062 6c75 6563  ....r..... bluec
+00000ec0: 6173 742e 6576 616c 7561 7469 6f6e 2e65  ast.evaluation.e
+00000ed0: 7661 6c5f 6d65 7472 6963 7372 0600 0000  val_metricsr....
+00000ee0: da1f 626c 7565 6361 7374 2e65 7661 6c75  ..bluecast.evalu
+00000ef0: 6174 696f 6e2e 7368 6170 5f76 616c 7565  ation.shap_value
+00000f00: 7372 0700 0000 da24 626c 7565 6361 7374  sr.....$bluecast
+00000f10: 2e74 6573 7473 2e6d 616b 655f 6461 7461  .tests.make_data
+00000f20: 2e63 7265 6174 655f 6461 7461 7208 0000  .create_datar...
+00000f30: 00da 0766 6978 7475 7265 720b 0000 0072  ...fixturer....r
+00000f40: 1400 0000 723f 0000 0072 5d00 0000 7265  ....r?...r]...re
+00000f50: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
+00000f60: 0000 720a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000f70: 3e01 0000 0073 2000 0000 2600 0802 0801  >....s ...&.....
+00000f80: 0801 0c02 1001 0c01 0c01 0c01 0403 0a01  ................
+00000f90: 0404 0a01 0804 0817 0c11                 ..........
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:14:40 2023 UTC, .py size: 1328 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 30e5 8064 3005 0000  o.......0..d0...
+00000000: 6f0d 0d0a 0000 0000 d188 8064 3005 0000  o..........d0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6401 6c08 5a09 6400 6402 6c0a 6d0b  d.d.l.Z.d.d.l.m.
 00000060: 5a0b 0100 6403 6404 8400 5a0c 6401 5300  Z...d.d...Z.d.S.
 00000070: 2905 e900 0000 004e 2901 da11 6368 6563  )......N)...chec
@@ -127,72 +127,72 @@
 000007e0: 7079 5f66 6f72 6d61 7436 da0b 4070 795f  py_format6..@py_
 000007f0: 6173 7365 7274 345a 0b40 7079 5f61 7373  assert4Z.@py_ass
 00000800: 6572 7436 da0b 4070 795f 6173 7365 7274  ert6..@py_assert
 00000810: 395a 0c40 7079 5f61 7373 6572 7431 315a  9Z.@py_assert11Z
 00000820: 0c40 7079 5f61 7373 6572 7431 335a 0c40  .@py_assert13Z.@
 00000830: 7079 5f61 7373 6572 7431 355a 0c40 7079  py_assert15Z.@py
 00000840: 5f66 6f72 6d61 7431 37a9 0072 2600 0000  _format17..r&...
-00000850: fa54 2f55 7365 7273 2f74 686f 6d61 736d  .T/Users/thomasm
-00000860: 6569 7373 6e65 722f 4964 6561 5072 6f6a  eissner/IdeaProj
-00000870: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
-00000880: 7565 6361 7374 2f74 6573 7473 2f74 6573  uecast/tests/tes
-00000890: 745f 6368 6563 6b5f 6770 755f 7375 7070  t_check_gpu_supp
-000008a0: 6f72 742e 7079 da0a 6d6f 636b 5f74 7261  ort.py..mock_tra
-000008b0: 696e 1300 0000 7308 0000 007e 01fe 010a  in....s....~....
-000008c0: 0004 017a 2a74 6573 745f 6368 6563 6b5f  ...z*test_check_
-000008d0: 6770 755f 7375 7070 6f72 742e 3c6c 6f63  gpu_support.<loc
-000008e0: 616c 733e 2e6d 6f63 6b5f 7472 6169 6eda  als>.mock_train.
-000008f0: 0574 7261 696e da04 7261 6e64 6300 0000  .train..randc...
-00000900: 0000 0000 0000 0000 0001 0000 0008 0000  ................
-00000910: 0057 0000 0073 2800 0000 7400 a001 6401  .W...s(...t...d.
-00000920: 6402 6702 6403 6404 6702 6405 6406 6702  d.g.d.d.g.d.d.g.
-00000930: 6407 6408 6702 6409 6401 6702 6705 a101  d.d.g.d.d.g.g...
-00000940: 5300 290a 4e67 9a99 9999 9999 b93f 679a  S.).Ng.......?g.
-00000950: 9999 9999 99c9 3f67 3333 3333 3333 d33f  ......?g333333.?
-00000960: 679a 9999 9999 99d9 3f67 0000 0000 0000  g.......?g......
-00000970: e03f 6733 3333 3333 33e3 3f67 6666 6666  .?g333333.?gffff
-00000980: 6666 e63f 679a 9999 9999 99e9 3f67 cdcc  ff.?g.......?g..
-00000990: cccc cccc ec3f a902 720f 0000 0072 2000  .....?..r....r .
-000009a0: 0000 2901 da04 6172 6773 7226 0000 0072  ..)...argsr&...r
-000009b0: 2600 0000 7227 0000 00da 083c 6c61 6d62  &...r'.....<lamb
-000009c0: 6461 3e1c 0000 0073 0600 0000 0400 2001  da>....s...... .
-000009d0: 04ff 7a28 7465 7374 5f63 6865 636b 5f67  ..z(test_check_g
-000009e0: 7075 5f73 7570 706f 7274 2e3c 6c6f 6361  pu_support.<loca
-000009f0: 6c73 3e2e 3c6c 616d 6264 613e da07 7261  ls>.<lambda>..ra
-00000a00: 6e64 696e 7463 0200 0000 0000 0000 0000  ndintc..........
-00000a10: 0000 0200 0000 0400 0000 5300 0000 730e  ..........S...s.
-00000a20: 0000 0074 00a0 0167 0064 01a2 01a1 0153  ...t...g.d.....S
-00000a30: 0029 024e 720d 0000 0072 2b00 0000 2902  .).Nr....r+...).
-00000a40: da03 6c6f 77da 0473 697a 6572 2600 0000  ..low..sizer&...
-00000a50: 7226 0000 0072 2700 0000 722d 0000 0021  r&...r'...r-...!
-00000a60: 0000 0073 0200 0000 0e00 7203 0000 0072  ...s......r....r
-00000a70: 0700 0000 2901 7a29 2528 7079 3229 730a  ....).z)%(py2)s.
-00000a80: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
-00000a90: 2973 2829 0a7d 203d 3d20 2528 7079 3529  )s().} == %(py5)
-00000aa0: 7372 0200 0000 2903 720a 0000 0072 1100  sr....).r....r..
-00000ab0: 0000 720c 0000 007a 0e61 7373 6572 7420  ..r....z.assert 
-00000ac0: 2528 7079 3729 7372 1200 0000 4e29 0dda  %(py7)sr....N)..
-00000ad0: 0773 6574 6174 7472 da03 7867 6272 0f00  .setattr..xgbr..
-00000ae0: 0000 da06 7261 6e64 6f6d 7202 0000 0072  ....randomr....r
-00000af0: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
-00000b00: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000b10: 0000 721d 0000 0029 07da 0b6d 6f6e 6b65  ..r....)...monke
-00000b20: 7970 6174 6368 7228 0000 0072 2200 0000  ypatchr(...r"...
-00000b30: 7224 0000 005a 0b40 7079 5f61 7373 6572  r$...Z.@py_asser
-00000b40: 7433 7223 0000 005a 0b40 7079 5f66 6f72  t3r#...Z.@py_for
-00000b50: 6d61 7438 7226 0000 0072 2600 0000 7227  mat8r&...r&...r'
-00000b60: 0000 00da 1674 6573 745f 6368 6563 6b5f  .....test_check_
-00000b70: 6770 755f 7375 7070 6f72 7407 0000 0073  gpu_support....s
-00000b80: 1600 0000 080c 0e05 0401 0401 0201 0601  ................
-00000b90: 04fd 0407 0c01 04ff 8e04 7235 0000 0029  ..........r5...)
-00000ba0: 0dda 0862 7569 6c74 696e 7372 1800 0000  ...builtinsr....
-00000bb0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-00000bc0: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00000bd0: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00000be0: 1600 0000 da05 6e75 6d70 7972 0f00 0000  ......numpyr....
-00000bf0: da07 7867 626f 6f73 7472 3200 0000 da24  ..xgboostr2....$
-00000c00: 626c 7565 6361 7374 2e67 656e 6572 616c  bluecast.general
-00000c10: 5f75 7469 6c73 2e67 656e 6572 616c 5f75  _utils.general_u
-00000c20: 7469 6c73 7202 0000 0072 3500 0000 7226  tilsr....r5...r&
-00000c30: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
-00000c40: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000c50: 7308 0000 0022 0008 010c 020c 03         s....".......
+00000850: fa4b 2f68 6f6d 652f 7468 6f6d 6173 2f49  .K/home/thomas/I
+00000860: 6465 6150 726f 6a65 6374 732f 426c 7565  deaProjects/Blue
+00000870: 4361 7374 2f62 6c75 6563 6173 742f 7465  Cast/bluecast/te
+00000880: 7374 732f 7465 7374 5f63 6865 636b 5f67  sts/test_check_g
+00000890: 7075 5f73 7570 706f 7274 2e70 79da 0a6d  pu_support.py..m
+000008a0: 6f63 6b5f 7472 6169 6e13 0000 0073 0800  ock_train....s..
+000008b0: 0000 7e01 fe01 0a00 0401 7a2a 7465 7374  ..~.......z*test
+000008c0: 5f63 6865 636b 5f67 7075 5f73 7570 706f  _check_gpu_suppo
+000008d0: 7274 2e3c 6c6f 6361 6c73 3e2e 6d6f 636b  rt.<locals>.mock
+000008e0: 5f74 7261 696e da05 7472 6169 6eda 0472  _train..train..r
+000008f0: 616e 6463 0000 0000 0000 0000 0000 0000  andc............
+00000900: 0100 0000 0800 0000 5700 0000 7328 0000  ........W...s(..
+00000910: 0074 00a0 0164 0164 0267 0264 0364 0467  .t...d.d.g.d.d.g
+00000920: 0264 0564 0667 0264 0764 0867 0264 0964  .d.d.g.d.d.g.d.d
+00000930: 0167 0267 05a1 0153 0029 0a4e 679a 9999  .g.g...S.).Ng...
+00000940: 9999 99b9 3f67 9a99 9999 9999 c93f 6733  ....?g.......?g3
+00000950: 3333 3333 33d3 3f67 9a99 9999 9999 d93f  33333.?g.......?
+00000960: 6700 0000 0000 00e0 3f67 3333 3333 3333  g.......?g333333
+00000970: e33f 6766 6666 6666 66e6 3f67 9a99 9999  .?gffffff.?g....
+00000980: 9999 e93f 67cd cccc cccc ccec 3fa9 0272  ...?g.......?..r
+00000990: 0f00 0000 7220 0000 0029 01da 0461 7267  ....r ...)...arg
+000009a0: 7372 2600 0000 7226 0000 0072 2700 0000  sr&...r&...r'...
+000009b0: da08 3c6c 616d 6264 613e 1c00 0000 7306  ..<lambda>....s.
+000009c0: 0000 0004 0020 0104 ff7a 2874 6573 745f  ..... ...z(test_
+000009d0: 6368 6563 6b5f 6770 755f 7375 7070 6f72  check_gpu_suppor
+000009e0: 742e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  t.<locals>.<lamb
+000009f0: 6461 3eda 0772 616e 6469 6e74 6302 0000  da>..randintc...
+00000a00: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000a10: 0053 0000 0073 0e00 0000 7400 a001 6700  .S...s....t...g.
+00000a20: 6401 a201 a101 5300 2902 4e72 0d00 0000  d.....S.).Nr....
+00000a30: 722b 0000 0029 02da 036c 6f77 da04 7369  r+...)...low..si
+00000a40: 7a65 7226 0000 0072 2600 0000 7227 0000  zer&...r&...r'..
+00000a50: 0072 2d00 0000 2100 0000 7302 0000 000e  .r-...!...s.....
+00000a60: 0072 0300 0000 7207 0000 0029 017a 2925  .r....r....).z)%
+00000a70: 2870 7932 2973 0a7b 2528 7079 3229 7320  (py2)s.{%(py2)s 
+00000a80: 3d20 2528 7079 3029 7328 290a 7d20 3d3d  = %(py0)s().} ==
+00000a90: 2025 2870 7935 2973 7202 0000 0029 0372   %(py5)sr....).r
+00000aa0: 0a00 0000 7211 0000 0072 0c00 0000 7a0e  ....r....r....z.
+00000ab0: 6173 7365 7274 2025 2870 7937 2973 7212  assert %(py7)sr.
+00000ac0: 0000 004e 290d da07 7365 7461 7474 72da  ...N)...setattr.
+00000ad0: 0378 6762 720f 0000 00da 0672 616e 646f  .xgbr......rando
+00000ae0: 6d72 0200 0000 7216 0000 0072 1700 0000  mr....r....r....
+00000af0: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000b00: 1b00 0000 721c 0000 0072 1d00 0000 2907  ....r....r....).
+00000b10: da0b 6d6f 6e6b 6579 7061 7463 6872 2800  ..monkeypatchr(.
+00000b20: 0000 7222 0000 0072 2400 0000 5a0b 4070  ..r"...r$...Z.@p
+00000b30: 795f 6173 7365 7274 3372 2300 0000 5a0b  y_assert3r#...Z.
+00000b40: 4070 795f 666f 726d 6174 3872 2600 0000  @py_format8r&...
+00000b50: 7226 0000 0072 2700 0000 da16 7465 7374  r&...r'.....test
+00000b60: 5f63 6865 636b 5f67 7075 5f73 7570 706f  _check_gpu_suppo
+00000b70: 7274 0700 0000 7316 0000 0008 0c0e 0504  rt....s.........
+00000b80: 0104 0102 0106 0104 fd04 070c 0104 ff8e  ................
+00000b90: 0472 3500 0000 290d da08 6275 696c 7469  .r5...)...builti
+00000ba0: 6e73 7218 0000 00da 195f 7079 7465 7374  nsr......_pytest
+00000bb0: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
+00000bc0: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
+00000bd0: 6577 7269 7465 7216 0000 00da 056e 756d  ewriter......num
+00000be0: 7079 720f 0000 00da 0778 6762 6f6f 7374  pyr......xgboost
+00000bf0: 7232 0000 00da 2462 6c75 6563 6173 742e  r2....$bluecast.
+00000c00: 6765 6e65 7261 6c5f 7574 696c 732e 6765  general_utils.ge
+00000c10: 6e65 7261 6c5f 7574 696c 7372 0200 0000  neral_utilsr....
+00000c20: 7235 0000 0072 2600 0000 7226 0000 0072  r5...r&...r&...r
+00000c30: 2600 0000 7227 0000 00da 083c 6d6f 6475  &...r'.....<modu
+00000c40: 6c65 3e01 0000 0073 0800 0000 2200 0801  le>....s...."...
+00000c50: 0c02 0c03                                ....
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 04:56:12 2023 UTC, .py size: 1097 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec0d 8064 4904 0000  o..........dI...
+00000000: 6f0d 0d0a 0000 0000 ab09 8064 4904 0000  o..........dI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6401 6c08 5a08 6400 6402 6c09 6d0a  d.d.l.Z.d.d.l.m.
 00000060: 5a0a 0100 6508 6a0b 6403 6404 8400 8301  Z...e.j.d.d.....
 00000070: 5a0c 6405 6406 8400 5a0d 6401 5300 2907  Z.d.d...Z.d.S.).
@@ -16,57 +16,57 @@
 000000f0: 303a 3030 7a13 3230 3231 2d30 322d 3135  0:00z.2021-02-15
 00000100: 2031 353a 3435 3a30 30e9 0100 0000 e902   15:45:00.......
 00000110: 0000 0029 02da 0c64 6174 6574 696d 655f  ...)...datetime_
 00000120: 636f 6cda 096f 7468 6572 5f63 6f6c 2903  col..other_col).
 00000130: da02 7064 da0b 746f 5f64 6174 6574 696d  ..pd..to_datetim
 00000140: 65da 0944 6174 6146 7261 6d65 2902 da04  e..DataFrame)...
 00000150: 6461 7461 da02 6466 a900 720c 0000 00fa  data..df..r.....
-00000160: 542f 5573 6572 732f 7468 6f6d 6173 6d65  T/Users/thomasme
-00000170: 6973 736e 6572 2f49 6465 6150 726f 6a65  issner/IdeaProje
-00000180: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
-00000190: 6563 6173 742f 7465 7374 732f 7465 7374  ecast/tests/test
-000001a0: 5f64 6174 6574 696d 655f 6665 6174 7572  _datetime_featur
-000001b0: 6573 2e70 79da 1073 616d 706c 655f 6461  es.py..sample_da
-000001c0: 7461 6672 616d 6507 0000 0073 0a00 0000  taframe....s....
-000001d0: 0c04 0601 06fe 0a04 0401 720e 0000 0063  ..........r....c
-000001e0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000001f0: 0800 0000 4300 0000 7350 0000 0074 00a0  ....C...sP...t..
-00000200: 0164 0164 0267 0264 0164 0367 0264 0464  .d.d.g.d.d.g.d.d
-00000210: 0567 0264 0664 0367 0264 0164 0267 0264  .g.d.d.g.d.d.g.d
-00000220: 079c 05a1 017d 0174 027c 0064 0867 0183  .....}.t.|.d.g..
-00000230: 027d 0274 006a 036a 047c 027c 0164 0964  .}.t.j.j.|.|.d.d
-00000240: 0a64 0a64 0b8d 0501 0064 0053 0029 0c4e  .d.d.....d.S.).N
-00000250: 7203 0000 0072 0400 0000 e90f 0000 00e9  r....r..........
-00000260: 0400 0000 7201 0000 00e9 0a00 0000 2905  ....r.........).
-00000270: 5a12 6461 7465 7469 6d65 5f63 6f6c 5f6d  Z.datetime_col_m
-00000280: 6f6e 7468 5a10 6461 7465 7469 6d65 5f63  onthZ.datetime_c
-00000290: 6f6c 5f64 6179 5a16 6461 7465 7469 6d65  ol_dayZ.datetime
-000002a0: 5f63 6f6c 5f64 6179 6f66 7765 656b 5a11  _col_dayofweekZ.
-000002b0: 6461 7465 7469 6d65 5f63 6f6c 5f68 6f75  datetime_col_hou
-000002c0: 7272 0600 0000 7205 0000 0054 4629 03da  rr....r....TF)..
-000002d0: 0a63 6865 636b 5f6c 696b 65da 1163 6865  .check_like..che
-000002e0: 636b 5f63 6f6c 756d 6e5f 7479 7065 da0b  ck_column_type..
-000002f0: 6368 6563 6b5f 6474 7970 6529 0572 0700  check_dtype).r..
-00000300: 0000 7209 0000 0072 0200 0000 da07 7465  ..r....r......te
-00000310: 7374 696e 67da 1261 7373 6572 745f 6672  sting..assert_fr
-00000320: 616d 655f 6571 7561 6c29 0372 0e00 0000  ame_equal).r....
-00000330: 5a0f 6578 7065 6374 6564 5f72 6573 756c  Z.expected_resul
-00000340: 74da 0672 6573 756c 7472 0c00 0000 720c  t..resultr....r.
-00000350: 0000 0072 0d00 0000 da13 7465 7374 5f64  ...r......test_d
-00000360: 6174 655f 636f 6e76 6572 7465 7212 0000  ate_converter...
-00000370: 0073 2000 0000 0402 0602 0601 0601 0601  .s .............
-00000380: 0601 04fb 04ff 0c0b 0603 0201 0201 0201  ................
-00000390: 0201 0201 0afb 7218 0000 0029 0eda 0862  ......r....)...b
-000003a0: 7569 6c74 696e 73da 0c40 7079 5f62 7569  uiltins..@py_bui
-000003b0: 6c74 696e 73da 195f 7079 7465 7374 2e61  ltins.._pytest.a
-000003c0: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
-000003d0: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
-000003e0: 7269 7465 da0a 4070 7974 6573 745f 6172  rite..@pytest_ar
-000003f0: da06 7061 6e64 6173 7207 0000 00da 0670  ..pandasr......p
-00000400: 7974 6573 74da 2862 6c75 6563 6173 742e  ytest.(bluecast.
-00000410: 7072 6570 726f 6365 7373 696e 672e 6461  preprocessing.da
-00000420: 7465 7469 6d65 5f66 6561 7475 7265 7372  tetime_featuresr
-00000430: 0200 0000 da07 6669 7874 7572 6572 0e00  ......fixturer..
-00000440: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000450: 0072 0c00 0000 720d 0000 00da 083c 6d6f  .r....r......<mo
-00000460: 6475 6c65 3e01 0000 0073 0c00 0000 2200  dule>....s....".
-00000470: 0801 0c02 0403 0a01 0c0a                 ..........
+00000160: 4b2f 686f 6d65 2f74 686f 6d61 732f 4964  K/home/thomas/Id
+00000170: 6561 5072 6f6a 6563 7473 2f42 6c75 6543  eaProjects/BlueC
+00000180: 6173 742f 626c 7565 6361 7374 2f74 6573  ast/bluecast/tes
+00000190: 7473 2f74 6573 745f 6461 7465 7469 6d65  ts/test_datetime
+000001a0: 5f66 6561 7475 7265 732e 7079 da10 7361  _features.py..sa
+000001b0: 6d70 6c65 5f64 6174 6166 7261 6d65 0700  mple_dataframe..
+000001c0: 0000 730a 0000 000c 0406 0106 fe0a 0404  ..s.............
+000001d0: 0172 0e00 0000 6301 0000 0000 0000 0000  .r....c.........
+000001e0: 0000 0003 0000 0008 0000 0043 0000 0073  ...........C...s
+000001f0: 5000 0000 7400 a001 6401 6402 6702 6401  P...t...d.d.g.d.
+00000200: 6403 6702 6404 6405 6702 6406 6403 6702  d.g.d.d.g.d.d.g.
+00000210: 6401 6402 6702 6407 9c05 a101 7d01 7402  d.d.g.d.....}.t.
+00000220: 7c00 6408 6701 8302 7d02 7400 6a03 6a04  |.d.g...}.t.j.j.
+00000230: 7c02 7c01 6409 640a 640a 640b 8d05 0100  |.|.d.d.d.d.....
+00000240: 6400 5300 290c 4e72 0300 0000 7204 0000  d.S.).Nr....r...
+00000250: 00e9 0f00 0000 e904 0000 0072 0100 0000  ...........r....
+00000260: e90a 0000 0029 055a 1264 6174 6574 696d  .....).Z.datetim
+00000270: 655f 636f 6c5f 6d6f 6e74 685a 1064 6174  e_col_monthZ.dat
+00000280: 6574 696d 655f 636f 6c5f 6461 795a 1664  etime_col_dayZ.d
+00000290: 6174 6574 696d 655f 636f 6c5f 6461 796f  atetime_col_dayo
+000002a0: 6677 6565 6b5a 1164 6174 6574 696d 655f  fweekZ.datetime_
+000002b0: 636f 6c5f 686f 7572 7206 0000 0072 0500  col_hourr....r..
+000002c0: 0000 5446 2903 da0a 6368 6563 6b5f 6c69  ..TF)...check_li
+000002d0: 6b65 da11 6368 6563 6b5f 636f 6c75 6d6e  ke..check_column
+000002e0: 5f74 7970 65da 0b63 6865 636b 5f64 7479  _type..check_dty
+000002f0: 7065 2905 7207 0000 0072 0900 0000 7202  pe).r....r....r.
+00000300: 0000 00da 0774 6573 7469 6e67 da12 6173  .....testing..as
+00000310: 7365 7274 5f66 7261 6d65 5f65 7175 616c  sert_frame_equal
+00000320: 2903 720e 0000 005a 0f65 7870 6563 7465  ).r....Z.expecte
+00000330: 645f 7265 7375 6c74 da06 7265 7375 6c74  d_result..result
+00000340: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000350: 1374 6573 745f 6461 7465 5f63 6f6e 7665  .test_date_conve
+00000360: 7274 6572 1200 0000 7320 0000 0004 0206  rter....s ......
+00000370: 0206 0106 0106 0106 0104 fb04 ff0c 0b06  ................
+00000380: 0302 0102 0102 0102 0102 010a fb72 1800  .............r..
+00000390: 0000 290e da08 6275 696c 7469 6e73 da0c  ..)...builtins..
+000003a0: 4070 795f 6275 696c 7469 6e73 da19 5f70  @py_builtins.._p
+000003b0: 7974 6573 742e 6173 7365 7274 696f 6e2e  ytest.assertion.
+000003c0: 7265 7772 6974 65da 0961 7373 6572 7469  rewrite..asserti
+000003d0: 6f6e da07 7265 7772 6974 65da 0a40 7079  on..rewrite..@py
+000003e0: 7465 7374 5f61 72da 0670 616e 6461 7372  test_ar..pandasr
+000003f0: 0700 0000 da06 7079 7465 7374 da28 626c  ......pytest.(bl
+00000400: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
+00000410: 7369 6e67 2e64 6174 6574 696d 655f 6665  sing.datetime_fe
+00000420: 6174 7572 6573 7202 0000 00da 0766 6978  aturesr......fix
+00000430: 7475 7265 720e 0000 0072 1800 0000 720c  turer....r....r.
+00000440: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000450: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000460: 730c 0000 0022 0008 010c 0204 030a 010c  s...."..........
+00000470: 0a                                       .
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 04:56:12 2023 UTC, .py size: 1996 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec0d 8064 cc07 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ab09 8064 cc07 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6401 6c08 5a08 6400 6402 6c09 6d0a  d.d.l.Z.d.d.l.m.
 00000060: 5a0a 0100 6508 6a0b 6403 6404 8400 8301  Z...e.j.d.d.....
 00000070: 5a0c 6508 6a0b 6405 6406 8400 8301 5a0d  Z.e.j.d.d.....Z.
@@ -11,141 +11,140 @@
 000000a0: 640e 8400 5a11 640f 6410 8400 5a12 6411  d...Z.d.d...Z.d.
 000000b0: 6412 8400 5a13 6401 5300 2913 e900 0000  d...Z.d.S.).....
 000000c0: 004e a901 da12 5461 7267 6574 4c61 6265  .N....TargetLabe
 000000d0: 6c45 6e63 6f64 6572 6300 0000 0000 0000  lEncoderc.......
 000000e0: 0000 0000 0000 0000 0001 0000 0043 0000  .............C..
 000000f0: 0073 0600 0000 7400 8300 5300 2901 4e72  .s....t...S.).Nr
 00000100: 0200 0000 a900 7204 0000 0072 0400 0000  ......r....r....
-00000110: fa57 2f55 7365 7273 2f74 686f 6d61 736d  .W/Users/thomasm
-00000120: 6569 7373 6e65 722f 4964 6561 5072 6f6a  eissner/IdeaProj
-00000130: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
-00000140: 7565 6361 7374 2f74 6573 7473 2f74 6573  uecast/tests/tes
-00000150: 745f 656e 636f 6465 5f74 6172 6765 745f  t_encode_target_
-00000160: 6c61 6265 6c73 2e70 79da 0d6c 6162 656c  labels.py..label
-00000170: 5f65 6e63 6f64 6572 0700 0000 7302 0000  _encoder....s...
-00000180: 0006 0272 0600 0000 6300 0000 0000 0000  ...r....c.......
-00000190: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-000001a0: 0073 1600 0000 7400 a001 6401 6700 6402  .s....t...d.g.d.
-000001b0: a201 6901 a101 7d00 7c00 5300 2903 4eda  ..i...}.|.S.).N.
-000001c0: 0674 6172 6765 74a9 06da 0141 da01 42da  .target....A..B.
-000001d0: 0143 7209 0000 0072 0a00 0000 720b 0000  .Cr....r....r...
-000001e0: 0029 02da 0270 64da 0944 6174 6146 7261  .)...pd..DataFra
-000001f0: 6d65 2901 da04 6461 7461 7204 0000 0072  me)...datar....r
-00000200: 0400 0000 7205 0000 00da 0b73 616d 706c  ....r......sampl
-00000210: 655f 6461 7461 0c00 0000 7304 0000 0012  e_data....s.....
-00000220: 0204 0172 0f00 0000 6302 0000 0000 0000  ...r....c.......
-00000230: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000240: 0073 1200 0000 7c00 a000 7c01 6401 1900  .s....|...|.d...
-00000250: a101 0100 7c00 5300 2902 4e72 0700 0000  ....|.S.).Nr....
-00000260: 2901 da1b 6669 745f 7472 616e 7366 6f72  )...fit_transfor
-00000270: 6d5f 7461 7267 6574 5f6c 6162 656c 7329  m_target_labels)
-00000280: 0272 0600 0000 720f 0000 0072 0400 0000  .r....r....r....
-00000290: 7204 0000 0072 0500 0000 da15 7472 6169  r....r......trai
-000002a0: 6e65 645f 6c61 6265 6c5f 656e 636f 6465  ned_label_encode
-000002b0: 7212 0000 0073 0400 0000 0e02 0401 7211  r....s........r.
-000002c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000002d0: 0700 0000 0700 0000 4300 0000 73a8 0000  ........C...s...
-000002e0: 007c 00a0 007c 0164 0119 00a1 017d 0264  .|...|.d.....}.d
-000002f0: 0264 0364 0464 059c 037d 037c 027c 036b  .d.d.d...}.|.|.k
-00000300: 027d 047c 0473 5074 01a0 0264 067c 0466  .}.|.sPt...d.|.f
-00000310: 0164 077c 027c 0366 02a1 0464 0874 03a0  .d.|.|.f...d.t..
-00000320: 04a1 0076 0073 2874 01a0 057c 02a1 0172  ...v.s(t...|...r
-00000330: 2d74 01a0 067c 02a1 016e 0164 0864 0974  -t...|...n.d.d.t
-00000340: 03a0 04a1 0076 0073 3974 01a0 057c 03a1  .....v.s9t...|..
-00000350: 0172 3e74 01a0 067c 03a1 016e 0164 0964  .r>t...|...n.d.d
-00000360: 0a9c 0216 007d 0564 0b64 0c7c 0569 0116  .....}.d.d.|.i..
-00000370: 007d 0674 0774 01a0 087c 06a1 0183 0182  .}.t.t...|......
-00000380: 0164 007d 0464 0053 0029 0d4e 7207 0000  .d.}.d.S.).Nr...
-00000390: 0072 0100 0000 e901 0000 00e9 0200 0000  .r..............
-000003a0: 2903 7209 0000 0072 0a00 0000 720b 0000  ).r....r....r...
-000003b0: 0029 01fa 023d 3d29 017a 1225 2870 7930  .)...==).z.%(py0
-000003c0: 2973 203d 3d20 2528 7079 3229 73da 076d  )s == %(py2)s..m
-000003d0: 6170 7069 6e67 da10 6578 7065 6374 6564  apping..expected
-000003e0: 5f6d 6170 7069 6e67 2902 da03 7079 30da  _mapping)...py0.
-000003f0: 0370 7932 7a0e 6173 7365 7274 2025 2870  .py2z.assert %(p
-00000400: 7934 2973 5a03 7079 3429 09da 1166 6974  y4)sZ.py4)...fit
-00000410: 5f6c 6162 656c 5f65 6e63 6f64 6572 da0a  _label_encoder..
-00000420: 4070 7974 6573 745f 6172 da11 5f63 616c  @pytest_ar.._cal
-00000430: 6c5f 7265 7072 636f 6d70 6172 65da 0c40  l_reprcompare..@
-00000440: 7079 5f62 7569 6c74 696e 73da 066c 6f63  py_builtins..loc
-00000450: 616c 73da 185f 7368 6f75 6c64 5f72 6570  als.._should_rep
-00000460: 725f 676c 6f62 616c 5f6e 616d 65da 095f  r_global_name.._
-00000470: 7361 6665 7265 7072 da0e 4173 7365 7274  saferepr..Assert
-00000480: 696f 6e45 7272 6f72 da13 5f66 6f72 6d61  ionError.._forma
-00000490: 745f 6578 706c 616e 6174 696f 6e29 0772  t_explanation).r
-000004a0: 0600 0000 720f 0000 0072 1500 0000 7216  ....r....r....r.
-000004b0: 0000 00da 0b40 7079 5f61 7373 6572 7431  .....@py_assert1
-000004c0: 5a0b 4070 795f 666f 726d 6174 335a 0b40  Z.@py_format3Z.@
-000004d0: 7079 5f66 6f72 6d61 7435 7204 0000 0072  py_format5r....r
-000004e0: 0400 0000 7205 0000 00da 1674 6573 745f  ....r......test_
-000004f0: 6669 745f 6c61 6265 6c5f 656e 636f 6465  fit_label_encode
-00000500: 7218 0000 0073 0600 0000 0e01 0c01 8e01  r....s..........
-00000510: 7223 0000 0063 0200 0000 0000 0000 0000  r#...c..........
-00000520: 0000 0400 0000 0500 0000 4300 0000 f332  ..........C....2
-00000530: 0000 007c 00a0 007c 0164 0119 00a1 017d  ...|...|.d.....}
-00000540: 0274 01a0 0264 0167 0064 02a2 0169 01a1  .t...d.g.d...i..
-00000550: 017d 0374 016a 03a0 047c 027c 03a1 0201  .}.t.j...|.|....
-00000560: 0064 0053 00a9 034e 7207 0000 00a9 0672  .d.S...Nr......r
-00000570: 0100 0000 7212 0000 0072 1300 0000 7201  ....r....r....r.
-00000580: 0000 0072 1200 0000 7213 0000 00a9 05da  ...r....r.......
-00000590: 1774 7261 6e73 666f 726d 5f74 6172 6765  .transform_targe
-000005a0: 745f 6c61 6265 6c73 720c 0000 0072 0d00  t_labelsr....r..
-000005b0: 0000 da07 7465 7374 696e 67da 1261 7373  ....testing..ass
-000005c0: 6572 745f 6672 616d 655f 6571 7561 6ca9  ert_frame_equal.
-000005d0: 0472 1100 0000 720f 0000 00da 1074 7261  .r....r......tra
-000005e0: 6e73 666f 726d 6564 5f64 6174 61da 0d65  nsformed_data..e
-000005f0: 7870 6563 7465 645f 6461 7461 7204 0000  xpected_datar...
-00000600: 0072 0400 0000 7205 0000 00da 1c74 6573  .r....r......tes
-00000610: 745f 6c61 6265 6c5f 656e 636f 6465 725f  t_label_encoder_
-00000620: 7472 616e 7366 6f72 6d1e 0000 00f3 0a00  transform.......
-00000630: 0000 0401 0601 04ff 1203 1201 722e 0000  ............r...
-00000640: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-00000650: 0000 0500 0000 4300 0000 7224 0000 0072  ......C...r$...r
-00000660: 2500 0000 2905 7210 0000 0072 0c00 0000  %...).r....r....
-00000670: 720d 0000 0072 2900 0000 722a 0000 0029  r....r)...r*...)
-00000680: 0472 0600 0000 720f 0000 0072 2c00 0000  .r....r....r,...
-00000690: 722d 0000 0072 0400 0000 7204 0000 0072  r-...r....r....r
-000006a0: 0500 0000 da20 7465 7374 5f66 6974 5f74  ..... test_fit_t
-000006b0: 7261 6e73 666f 726d 5f74 6172 6765 745f  ransform_target_
-000006c0: 6c61 6265 6c73 2600 0000 7306 0000 000e  labels&...s.....
-000006d0: 0112 0112 0172 3000 0000 6302 0000 0000  .....r0...c.....
-000006e0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
-000006f0: 0000 0072 2400 0000 7225 0000 0072 2700  ...r$...r%...r'.
-00000700: 0000 722b 0000 0072 0400 0000 7204 0000  ..r+...r....r...
-00000710: 0072 0500 0000 da1c 7465 7374 5f74 7261  .r......test_tra
-00000720: 6e73 666f 726d 5f74 6172 6765 745f 6c61  nsform_target_la
-00000730: 6265 6c73 2c00 0000 722f 0000 0072 3100  bels,...r/...r1.
-00000740: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
-00000750: 0000 0005 0000 0043 0000 0073 4400 0000  .......C...sD...
-00000760: 7400 a001 6401 6700 6402 a201 6901 a101  t...d.g.d...i...
-00000770: 7d02 7c00 a002 7c02 6401 1900 a101 7d03  }.|...|.d.....}.
-00000780: 7400 a001 6401 6700 6403 a201 6901 a101  t...d.g.d...i...
-00000790: 7d04 7400 6a03 a004 7c03 7c04 a102 0100  }.t.j...|.|.....
-000007a0: 6400 5300 2904 4e72 0700 0000 7226 0000  d.S.).Nr....r&..
-000007b0: 0072 0800 0000 2905 720c 0000 0072 0d00  .r....).r....r..
-000007c0: 0000 da1f 6c61 6265 6c5f 656e 636f 6465  ....label_encode
-000007d0: 725f 7265 7665 7273 655f 7472 616e 7366  r_reverse_transf
-000007e0: 6f72 6d72 2900 0000 722a 0000 0029 0572  ormr)...r*...).r
-000007f0: 1100 0000 720f 0000 0072 2c00 0000 5a0d  ....r....r,...Z.
-00000800: 7265 7665 7273 6564 5f64 6174 6172 2d00  reversed_datar-.
-00000810: 0000 7204 0000 0072 0400 0000 7205 0000  ..r....r....r...
-00000820: 00da 2474 6573 745f 6c61 6265 6c5f 656e  ..$test_label_en
-00000830: 636f 6465 725f 7265 7665 7273 655f 7472  coder_reverse_tr
-00000840: 616e 7366 6f72 6d34 0000 0073 0c00 0000  ansform4...s....
-00000850: 1201 0401 0601 04ff 1203 1201 7233 0000  ............r3..
-00000860: 0029 14da 0862 7569 6c74 696e 7372 1c00  .)...builtinsr..
-00000870: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
-00000880: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
-00000890: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
-000008a0: 6572 1a00 0000 da06 7061 6e64 6173 720c  er......pandasr.
-000008b0: 0000 00da 0670 7974 6573 74da 2b62 6c75  .....pytest.+blu
-000008c0: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-000008d0: 696e 672e 656e 636f 6465 5f74 6172 6765  ing.encode_targe
-000008e0: 745f 6c61 6265 6c73 7203 0000 00da 0766  t_labelsr......f
-000008f0: 6978 7475 7265 7206 0000 0072 0f00 0000  ixturer....r....
-00000900: 7211 0000 0072 2300 0000 722e 0000 0072  r....r#...r....r
-00000910: 3000 0000 7231 0000 0072 3300 0000 7204  0...r1...r3...r.
-00000920: 0000 0072 0400 0000 7204 0000 0072 0500  ...r....r....r..
-00000930: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000940: 731c 0000 0022 0008 010c 0204 030a 0104  s...."..........
-00000950: 040a 0104 050a 0108 0508 0608 0808 060c  ................
-00000960: 08                                       .
+00000110: fa4e 2f68 6f6d 652f 7468 6f6d 6173 2f49  .N/home/thomas/I
+00000120: 6465 6150 726f 6a65 6374 732f 426c 7565  deaProjects/Blue
+00000130: 4361 7374 2f62 6c75 6563 6173 742f 7465  Cast/bluecast/te
+00000140: 7374 732f 7465 7374 5f65 6e63 6f64 655f  sts/test_encode_
+00000150: 7461 7267 6574 5f6c 6162 656c 732e 7079  target_labels.py
+00000160: da0d 6c61 6265 6c5f 656e 636f 6465 7207  ..label_encoder.
+00000170: 0000 0073 0200 0000 0602 7206 0000 0063  ...s......r....c
+00000180: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000190: 0500 0000 4300 0000 7316 0000 0074 00a0  ....C...s....t..
+000001a0: 0164 0167 0064 02a2 0169 01a1 017d 007c  .d.g.d...i...}.|
+000001b0: 0053 0029 034e da06 7461 7267 6574 a906  .S.).N..target..
+000001c0: da01 41da 0142 da01 4372 0900 0000 720a  ..A..B..Cr....r.
+000001d0: 0000 0072 0b00 0000 2902 da02 7064 da09  ...r....)...pd..
+000001e0: 4461 7461 4672 616d 6529 01da 0464 6174  DataFrame)...dat
+000001f0: 6172 0400 0000 7204 0000 0072 0500 0000  ar....r....r....
+00000200: da0b 7361 6d70 6c65 5f64 6174 610c 0000  ..sample_data...
+00000210: 0073 0400 0000 1202 0401 720f 0000 0063  .s........r....c
+00000220: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000230: 0400 0000 4300 0000 7312 0000 007c 00a0  ....C...s....|..
+00000240: 007c 0164 0119 00a1 0101 007c 0053 0029  .|.d.......|.S.)
+00000250: 024e 7207 0000 0029 01da 1b66 6974 5f74  .Nr....)...fit_t
+00000260: 7261 6e73 666f 726d 5f74 6172 6765 745f  ransform_target_
+00000270: 6c61 6265 6c73 2902 7206 0000 0072 0f00  labels).r....r..
+00000280: 0000 7204 0000 0072 0400 0000 7205 0000  ..r....r....r...
+00000290: 00da 1574 7261 696e 6564 5f6c 6162 656c  ...trained_label
+000002a0: 5f65 6e63 6f64 6572 1200 0000 7304 0000  _encoder....s...
+000002b0: 000e 0204 0172 1100 0000 6302 0000 0000  .....r....c.....
+000002c0: 0000 0000 0000 0007 0000 0007 0000 0043  ...............C
+000002d0: 0000 0073 a800 0000 7c00 a000 7c01 6401  ...s....|...|.d.
+000002e0: 1900 a101 7d02 6402 6403 6404 6405 9c03  ....}.d.d.d.d...
+000002f0: 7d03 7c02 7c03 6b02 7d04 7c04 7350 7401  }.|.|.k.}.|.sPt.
+00000300: a002 6406 7c04 6601 6407 7c02 7c03 6602  ..d.|.f.d.|.|.f.
+00000310: a104 6408 7403 a004 a100 7600 7328 7401  ..d.t.....v.s(t.
+00000320: a005 7c02 a101 722d 7401 a006 7c02 a101  ..|...r-t...|...
+00000330: 6e01 6408 6409 7403 a004 a100 7600 7339  n.d.d.t.....v.s9
+00000340: 7401 a005 7c03 a101 723e 7401 a006 7c03  t...|...r>t...|.
+00000350: a101 6e01 6409 640a 9c02 1600 7d05 640b  ..n.d.d.....}.d.
+00000360: 640c 7c05 6901 1600 7d06 7407 7401 a008  d.|.i...}.t.t...
+00000370: 7c06 a101 8301 8201 6400 7d04 6400 5300  |.......d.}.d.S.
+00000380: 290d 4e72 0700 0000 7201 0000 00e9 0100  ).Nr....r.......
+00000390: 0000 e902 0000 0029 0372 0900 0000 720a  .......).r....r.
+000003a0: 0000 0072 0b00 0000 2901 fa02 3d3d 2901  ...r....)...==).
+000003b0: 7a12 2528 7079 3029 7320 3d3d 2025 2870  z.%(py0)s == %(p
+000003c0: 7932 2973 da07 6d61 7070 696e 67da 1065  y2)s..mapping..e
+000003d0: 7870 6563 7465 645f 6d61 7070 696e 6729  xpected_mapping)
+000003e0: 02da 0370 7930 da03 7079 327a 0e61 7373  ...py0..py2z.ass
+000003f0: 6572 7420 2528 7079 3429 735a 0370 7934  ert %(py4)sZ.py4
+00000400: 2909 da11 6669 745f 6c61 6265 6c5f 656e  )...fit_label_en
+00000410: 636f 6465 72da 0a40 7079 7465 7374 5f61  coder..@pytest_a
+00000420: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
+00000430: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
+00000440: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
+00000450: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
+00000460: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
+00000470: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
+00000480: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
+00000490: 7469 6f6e 2907 7206 0000 0072 0f00 0000  tion).r....r....
+000004a0: 7215 0000 0072 1600 0000 da0b 4070 795f  r....r......@py_
+000004b0: 6173 7365 7274 315a 0b40 7079 5f66 6f72  assert1Z.@py_for
+000004c0: 6d61 7433 5a0b 4070 795f 666f 726d 6174  mat3Z.@py_format
+000004d0: 3572 0400 0000 7204 0000 0072 0500 0000  5r....r....r....
+000004e0: da16 7465 7374 5f66 6974 5f6c 6162 656c  ..test_fit_label
+000004f0: 5f65 6e63 6f64 6572 1800 0000 7306 0000  _encoder....s...
+00000500: 000e 010c 018e 0172 2300 0000 6302 0000  .......r#...c...
+00000510: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00000520: 0043 0000 00f3 3200 0000 7c00 a000 7c01  .C....2...|...|.
+00000530: 6401 1900 a101 7d02 7401 a002 6401 6700  d.....}.t...d.g.
+00000540: 6402 a201 6901 a101 7d03 7401 6a03 a004  d...i...}.t.j...
+00000550: 7c02 7c03 a102 0100 6400 5300 a903 4e72  |.|.....d.S...Nr
+00000560: 0700 0000 a906 7201 0000 0072 1200 0000  ......r....r....
+00000570: 7213 0000 0072 0100 0000 7212 0000 0072  r....r....r....r
+00000580: 1300 0000 a905 da17 7472 616e 7366 6f72  ........transfor
+00000590: 6d5f 7461 7267 6574 5f6c 6162 656c 7372  m_target_labelsr
+000005a0: 0c00 0000 720d 0000 00da 0774 6573 7469  ....r......testi
+000005b0: 6e67 da12 6173 7365 7274 5f66 7261 6d65  ng..assert_frame
+000005c0: 5f65 7175 616c a904 7211 0000 0072 0f00  _equal..r....r..
+000005d0: 0000 da10 7472 616e 7366 6f72 6d65 645f  ....transformed_
+000005e0: 6461 7461 da0d 6578 7065 6374 6564 5f64  data..expected_d
+000005f0: 6174 6172 0400 0000 7204 0000 0072 0500  atar....r....r..
+00000600: 0000 da1c 7465 7374 5f6c 6162 656c 5f65  ....test_label_e
+00000610: 6e63 6f64 6572 5f74 7261 6e73 666f 726d  ncoder_transform
+00000620: 1e00 0000 f30a 0000 0004 0106 0104 ff12  ................
+00000630: 0312 0172 2e00 0000 6302 0000 0000 0000  ...r....c.......
+00000640: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+00000650: 0072 2400 0000 7225 0000 0029 0572 1000  .r$...r%...).r..
+00000660: 0000 720c 0000 0072 0d00 0000 7229 0000  ..r....r....r)..
+00000670: 0072 2a00 0000 2904 7206 0000 0072 0f00  .r*...).r....r..
+00000680: 0000 722c 0000 0072 2d00 0000 7204 0000  ..r,...r-...r...
+00000690: 0072 0400 0000 7205 0000 00da 2074 6573  .r....r..... tes
+000006a0: 745f 6669 745f 7472 616e 7366 6f72 6d5f  t_fit_transform_
+000006b0: 7461 7267 6574 5f6c 6162 656c 7326 0000  target_labels&..
+000006c0: 0073 0600 0000 0e01 1201 1201 7230 0000  .s..........r0..
+000006d0: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
+000006e0: 0000 0500 0000 4300 0000 7224 0000 0072  ......C...r$...r
+000006f0: 2500 0000 7227 0000 0072 2b00 0000 7204  %...r'...r+...r.
+00000700: 0000 0072 0400 0000 7205 0000 00da 1c74  ...r....r......t
+00000710: 6573 745f 7472 616e 7366 6f72 6d5f 7461  est_transform_ta
+00000720: 7267 6574 5f6c 6162 656c 732c 0000 0072  rget_labels,...r
+00000730: 2f00 0000 7231 0000 0063 0200 0000 0000  /...r1...c......
+00000740: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+00000750: 0000 7344 0000 0074 00a0 0164 0167 0064  ..sD...t...d.g.d
+00000760: 02a2 0169 01a1 017d 027c 00a0 027c 0264  ...i...}.|...|.d
+00000770: 0119 00a1 017d 0374 00a0 0164 0167 0064  .....}.t...d.g.d
+00000780: 03a2 0169 01a1 017d 0474 006a 03a0 047c  ...i...}.t.j...|
+00000790: 037c 04a1 0201 0064 0053 0029 044e 7207  .|.....d.S.).Nr.
+000007a0: 0000 0072 2600 0000 7208 0000 0029 0572  ...r&...r....).r
+000007b0: 0c00 0000 720d 0000 00da 1f6c 6162 656c  ....r......label
+000007c0: 5f65 6e63 6f64 6572 5f72 6576 6572 7365  _encoder_reverse
+000007d0: 5f74 7261 6e73 666f 726d 7229 0000 0072  _transformr)...r
+000007e0: 2a00 0000 2905 7211 0000 0072 0f00 0000  *...).r....r....
+000007f0: 722c 0000 005a 0d72 6576 6572 7365 645f  r,...Z.reversed_
+00000800: 6461 7461 722d 0000 0072 0400 0000 7204  datar-...r....r.
+00000810: 0000 0072 0500 0000 da24 7465 7374 5f6c  ...r.....$test_l
+00000820: 6162 656c 5f65 6e63 6f64 6572 5f72 6576  abel_encoder_rev
+00000830: 6572 7365 5f74 7261 6e73 666f 726d 3400  erse_transform4.
+00000840: 0000 730c 0000 0012 0104 0106 0104 ff12  ..s.............
+00000850: 0312 0172 3300 0000 2914 da08 6275 696c  ...r3...)...buil
+00000860: 7469 6e73 721c 0000 00da 195f 7079 7465  tinsr......_pyte
+00000870: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
+00000880: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
+00000890: 0772 6577 7269 7465 721a 0000 00da 0670  .rewriter......p
+000008a0: 616e 6461 7372 0c00 0000 da06 7079 7465  andasr......pyte
+000008b0: 7374 da2b 626c 7565 6361 7374 2e70 7265  st.+bluecast.pre
+000008c0: 7072 6f63 6573 7369 6e67 2e65 6e63 6f64  processing.encod
+000008d0: 655f 7461 7267 6574 5f6c 6162 656c 7372  e_target_labelsr
+000008e0: 0300 0000 da07 6669 7874 7572 6572 0600  ......fixturer..
+000008f0: 0000 720f 0000 0072 1100 0000 7223 0000  ..r....r....r#..
+00000900: 0072 2e00 0000 7230 0000 0072 3100 0000  .r....r0...r1...
+00000910: 7233 0000 0072 0400 0000 7204 0000 0072  r3...r....r....r
+00000920: 0400 0000 7205 0000 00da 083c 6d6f 6475  ....r......<modu
+00000930: 6c65 3e01 0000 0073 1c00 0000 2200 0801  le>....s...."...
+00000940: 0c02 0403 0a01 0404 0a01 0405 0a01 0805  ................
+00000950: 0806 0808 0806 0c08                      ........
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 20:14:40 2023 UTC, .py size: 2608 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 30e5 8064 300a 0000  o.......0..d0...
+00000000: 6f0d 0d0a 0000 0000 4f89 8064 300a 0000  o.......O..d0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6401 6c08 5a09 6400 6402 6c0a 6d0b  d.d.l.Z.d.d.l.m.
 00000060: 5a0b 0100 6403 6404 8400 5a0c 6401 5300  Z...d.d...Z.d.S.
 00000070: 2905 e900 0000 004e 2901 da13 4665 6174  )......N)...Feat
@@ -270,32 +270,32 @@
 000010d0: 7274 385a 0c40 7079 5f61 7373 6572 7431  rt8Z.@py_assert1
 000010e0: 305a 0c40 7079 5f66 6f72 6d61 7431 325a  0Z.@py_format12Z
 000010f0: 0c40 7079 5f66 6f72 6d61 7431 345a 0b40  .@py_format14Z.@
 00001100: 7079 5f61 7373 6572 7435 5a0b 4070 795f  py_assert5Z.@py_
 00001110: 666f 726d 6174 375a 0b40 7079 5f66 6f72  format7Z.@py_for
 00001120: 6d61 7439 da0b 4070 795f 6173 7365 7274  mat9..@py_assert
 00001130: 31da 0b40 7079 5f66 6f72 6d61 7436 a900  1..@py_format6..
-00001140: 723d 0000 00fa 582f 5573 6572 732f 7468  r=....X/Users/th
-00001150: 6f6d 6173 6d65 6973 736e 6572 2f49 6465  omasmeissner/Ide
-00001160: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
-00001170: 7374 2f62 6c75 6563 6173 742f 7465 7374  st/bluecast/test
-00001180: 732f 7465 7374 5f66 6561 7475 7265 5f74  s/test_feature_t
-00001190: 7970 655f 6465 7465 6374 6f72 2e70 79da  ype_detector.py.
-000011a0: 1a74 6573 745f 6665 6174 7572 655f 7479  .test_feature_ty
-000011b0: 7065 5f64 6574 6563 746f 7207 0000 0073  pe_detector....s
-000011c0: 4600 0000 0402 0602 0601 0601 0601 0601  F...............
-000011d0: 0601 0601 0601 04f8 04ff 020e 0601 0601  ................
-000011e0: 0601 06fd 0a07 6a03 6a01 a003 a601 ca03  ......j.j.......
-000011f0: ca01 6c03 6c01 0a03 8203 8201 a601 a601  ..l.l...........
-00001200: ca01 ca01 a601 a601 9403 723f 0000 0029  ..........r?...)
-00001210: 0dda 0862 7569 6c74 696e 7372 3100 0000  ...builtinsr1...
-00001220: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-00001230: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00001240: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00001250: 2a00 0000 da05 6e75 6d70 7972 1b00 0000  *.....numpyr....
-00001260: da06 7061 6e64 6173 7226 0000 00da 2462  ..pandasr&....$b
-00001270: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
-00001280: 7373 696e 672e 6665 6174 7572 655f 7479  ssing.feature_ty
-00001290: 7065 7372 0200 0000 723f 0000 0072 3d00  pesr....r?...r=.
-000012a0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-000012b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000012c0: 0800 0000 2200 0801 0c02 0c03            ....".......
+00001140: 723d 0000 00fa 4f2f 686f 6d65 2f74 686f  r=....O/home/tho
+00001150: 6d61 732f 4964 6561 5072 6f6a 6563 7473  mas/IdeaProjects
+00001160: 2f42 6c75 6543 6173 742f 626c 7565 6361  /BlueCast/blueca
+00001170: 7374 2f74 6573 7473 2f74 6573 745f 6665  st/tests/test_fe
+00001180: 6174 7572 655f 7479 7065 5f64 6574 6563  ature_type_detec
+00001190: 746f 722e 7079 da1a 7465 7374 5f66 6561  tor.py..test_fea
+000011a0: 7475 7265 5f74 7970 655f 6465 7465 6374  ture_type_detect
+000011b0: 6f72 0700 0000 7346 0000 0004 0206 0206  or....sF........
+000011c0: 0106 0106 0106 0106 0106 0106 0104 f804  ................
+000011d0: ff02 0e06 0106 0106 0106 fd0a 076a 036a  .............j.j
+000011e0: 01a0 03a6 01ca 03ca 016c 036c 010a 0382  .........l.l....
+000011f0: 0382 01a6 01a6 01ca 01ca 01a6 01a6 0194  ................
+00001200: 0372 3f00 0000 290d da08 6275 696c 7469  .r?...)...builti
+00001210: 6e73 7231 0000 00da 195f 7079 7465 7374  nsr1....._pytest
+00001220: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
+00001230: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
+00001240: 6577 7269 7465 722a 0000 00da 056e 756d  ewriter*.....num
+00001250: 7079 721b 0000 00da 0670 616e 6461 7372  pyr......pandasr
+00001260: 2600 0000 da24 626c 7565 6361 7374 2e70  &....$bluecast.p
+00001270: 7265 7072 6f63 6573 7369 6e67 2e66 6561  reprocessing.fea
+00001280: 7475 7265 5f74 7970 6573 7202 0000 0072  ture_typesr....r
+00001290: 3f00 0000 723d 0000 0072 3d00 0000 723d  ?...r=...r=...r=
+000012a0: 0000 0072 3e00 0000 da08 3c6d 6f64 756c  ...r>.....<modul
+000012b0: 653e 0100 0000 7308 0000 0022 0008 010c  e>....s...."....
+000012c0: 020c 03                                  ...
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 18:49:23 2023 UTC, .py size: 1649 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,100 @@
-00000000: 6f0d 0d0a 0000 0000 b322 8264 7106 0000  o........".dq...
+00000000: 6f0d 0d0a 0000 0000 11be 8264 ca05 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
+00000020: 0002 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
-00000050: 6400 6401 6c07 5a07 6400 6401 6c08 5a08  d.d.l.Z.d.d.l.Z.
-00000060: 6400 6402 6c09 6d0a 5a0a 0100 6403 6404  d.d.l.m.Z...d.d.
-00000070: 8400 5a0b 6405 6406 8400 5a0c 6401 5300  ..Z.d.d...Z.d.S.
-00000080: 2907 e900 0000 004e 2901 da13 6c6f 6164  )......N)...load
-00000090: 5f66 6f72 5f70 726f 6475 6374 696f 6e63  _for_productionc
-000000a0: 0000 0000 0000 0000 0000 0000 0900 0000  ................
-000000b0: 0800 0000 4300 0000 73fc 0000 0064 017d  ....C...s....d.}
-000000c0: 0064 027d 0164 037d 0264 047d 0374 007c  .d.}.d.}.d.}.t.|
-000000d0: 007c 0117 007c 0217 0064 0583 028f 0e7d  .|...|...d.....}
-000000e0: 0474 01a0 027c 037c 04a1 0201 0057 0064  .t...|.|.....W.d
-000000f0: 0004 0004 0083 0301 006e 0831 0073 2277  .........n.1.s"w
-00000100: 0101 0001 0001 0059 0001 0074 037c 007c  .......Y...t.|.|
-00000110: 017c 0264 068d 037d 057c 057c 036b 027d  .|.d...}.|.|.k.}
-00000120: 067c 0673 7174 04a0 0564 077c 0666 0164  .|.sqt...d.|.f.d
-00000130: 087c 057c 0366 02a1 0464 0974 06a0 07a1  .|.|.f...d.t....
-00000140: 0076 0073 4974 04a0 087c 05a1 0172 4e74  .v.sIt...|...rNt
-00000150: 04a0 097c 05a1 016e 0164 0964 0a74 06a0  ...|...n.d.d.t..
-00000160: 07a1 0076 0073 5a74 04a0 087c 03a1 0172  ...v.sZt...|...r
-00000170: 5f74 04a0 097c 03a1 016e 0164 0a64 0b9c  _t...|...n.d.d..
-00000180: 0216 007d 0764 0c64 0d7c 0769 0116 007d  ...}.d.d.|.i...}
-00000190: 0874 0a74 04a0 0b7c 08a1 0183 0182 0164  .t.t...|.......d
-000001a0: 007d 0674 0ca0 0d7c 007c 0117 007c 0217  .}.t...|.|...|..
-000001b0: 00a1 0101 0064 0053 0029 0e4e fa0d 7061  .....d.S.).N..pa
-000001c0: 7468 2f74 6f2f 6669 6c65 2fda 0d74 6573  th/to/file/..tes
-000001d0: 745f 696e 7374 616e 6365 fa04 2e64 6174  t_instance...dat
-000001e0: da09 7465 7374 5f64 6174 61da 0277 6229  ..test_data..wb)
-000001f0: 03da 0966 696c 655f 7061 7468 da09 6669  ...file_path..fi
-00000200: 6c65 5f6e 616d 65da 0966 696c 655f 7479  le_name..file_ty
-00000210: 7065 a901 fa02 3d3d a901 7a12 2528 7079  pe....==..z.%(py
-00000220: 3029 7320 3d3d 2025 2870 7932 2973 da0f  0)s == %(py2)s..
-00000230: 6c6f 6164 6564 5f69 6e73 7461 6e63 65da  loaded_instance.
-00000240: 0e64 756d 6d79 5f69 6e73 7461 6e63 65a9  .dummy_instance.
-00000250: 02da 0370 7930 da03 7079 32fa 0e61 7373  ...py0..py2..ass
-00000260: 6572 7420 2528 7079 3429 73da 0370 7934  ert %(py4)s..py4
-00000270: a90e da04 6f70 656e da06 7069 636b 6c65  ....open..pickle
-00000280: da04 6475 6d70 7202 0000 00da 0a40 7079  ..dumpr......@py
-00000290: 7465 7374 5f61 72da 115f 6361 6c6c 5f72  test_ar.._call_r
-000002a0: 6570 7263 6f6d 7061 7265 da0c 4070 795f  eprcompare..@py_
-000002b0: 6275 696c 7469 6e73 da06 6c6f 6361 6c73  builtins..locals
-000002c0: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
-000002d0: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
-000002e0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
-000002f0: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
-00000300: 7870 6c61 6e61 7469 6f6e da02 6f73 da06  xplanation..os..
-00000310: 7265 6d6f 7665 2909 7208 0000 0072 0900  remove).r....r..
-00000320: 0000 720a 0000 0072 0f00 0000 da04 6669  ..r....r......fi
-00000330: 6c65 720e 0000 00da 0b40 7079 5f61 7373  ler......@py_ass
-00000340: 6572 7431 da0b 4070 795f 666f 726d 6174  ert1..@py_format
-00000350: 33da 0b40 7079 5f66 6f72 6d61 7435 a900  3..@py_format5..
-00000360: 7227 0000 00fa 562f 5573 6572 732f 7468  r'....V/Users/th
-00000370: 6f6d 6173 6d65 6973 736e 6572 2f49 6465  omasmeissner/Ide
-00000380: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
-00000390: 7374 2f62 6c75 6563 6173 742f 7465 7374  st/bluecast/test
-000003a0: 732f 7465 7374 5f6c 6f61 645f 666f 725f  s/test_load_for_
-000003b0: 7072 6f64 7563 7469 6f6e 2e70 79da 1874  production.py..t
-000003c0: 6573 745f 6c6f 6164 5f66 6f72 5f70 726f  est_load_for_pro
-000003d0: 6475 6374 696f 6e07 0000 0073 1400 0000  duction....s....
-000003e0: 0402 0401 0401 0403 1403 0e01 1cff 0e04  ................
-000003f0: 8a03 1603 7229 0000 0063 0000 0000 0000  ....r)...c......
-00000400: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
-00000410: 0000 73f6 0000 0064 017d 0064 027d 0164  ..s....d.}.d.}.d
-00000420: 037d 0274 007c 007c 0117 0064 0417 0064  .}.t.|.|...d...d
-00000430: 0583 028f 0e7d 0374 01a0 027c 027c 03a1  .....}.t...|.|..
-00000440: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000450: 0831 0073 2077 0101 0001 0001 0059 0001  .1.s w.......Y..
-00000460: 0074 037c 007c 0164 068d 027d 047c 047c  .t.|.|.d...}.|.|
-00000470: 026b 027d 057c 0573 6e74 04a0 0564 077c  .k.}.|.snt...d.|
-00000480: 0566 0164 087c 047c 0266 02a1 0464 0974  .f.d.|.|.f...d.t
-00000490: 06a0 07a1 0076 0073 4674 04a0 087c 04a1  .....v.sFt...|..
-000004a0: 0172 4b74 04a0 097c 04a1 016e 0164 0964  .rKt...|...n.d.d
-000004b0: 0a74 06a0 07a1 0076 0073 5774 04a0 087c  .t.....v.sWt...|
-000004c0: 02a1 0172 5c74 04a0 097c 02a1 016e 0164  ...r\t...|...n.d
-000004d0: 0a64 0b9c 0216 007d 0664 0c64 0d7c 0669  .d.....}.d.d.|.i
-000004e0: 0116 007d 0774 0a74 04a0 0b7c 07a1 0183  ...}.t.t...|....
-000004f0: 0182 0164 007d 0574 0ca0 0d7c 007c 0117  ...d.}.t...|.|..
-00000500: 0064 0417 00a1 0101 0064 0053 0029 0e4e  .d.......d.S.).N
-00000510: 7203 0000 0072 0400 0000 7206 0000 0072  r....r....r....r
-00000520: 0500 0000 7207 0000 0029 0272 0800 0000  ....r....).r....
-00000530: 7209 0000 0072 0b00 0000 720d 0000 0072  r....r....r....r
-00000540: 0e00 0000 720f 0000 0072 1000 0000 7213  ....r....r....r.
-00000550: 0000 0072 1400 0000 7215 0000 0029 0872  ...r....r....).r
-00000560: 0800 0000 7209 0000 0072 0f00 0000 7223  ....r....r....r#
-00000570: 0000 0072 0e00 0000 7224 0000 0072 2500  ...r....r$...r%.
-00000580: 0000 7226 0000 0072 2700 0000 7227 0000  ..r&...r'...r'..
-00000590: 0072 2800 0000 da2f 7465 7374 5f6c 6f61  .r(..../test_loa
-000005a0: 645f 666f 725f 7072 6f64 7563 7469 6f6e  d_for_production
-000005b0: 5f77 6974 685f 6465 6661 756c 745f 6669  _with_default_fi
-000005c0: 6c65 5f74 7970 651e 0000 0073 1200 0000  le_type....s....
-000005d0: 0402 0401 0403 1403 0e01 1cff 0c04 8a03  ................
-000005e0: 1603 722a 0000 0029 0dda 0862 7569 6c74  ..r*...)...built
-000005f0: 696e 7372 1b00 0000 da19 5f70 7974 6573  insr......_pytes
-00000600: 742e 6173 7365 7274 696f 6e2e 7265 7772  t.assertion.rewr
-00000610: 6974 65da 0961 7373 6572 7469 6f6e da07  ite..assertion..
-00000620: 7265 7772 6974 6572 1900 0000 7221 0000  rewriter....r!..
-00000630: 00da 0670 7974 6573 7472 1700 0000 da24  ...pytestr.....$
-00000640: 626c 7565 6361 7374 2e67 656e 6572 616c  bluecast.general
-00000650: 5f75 7469 6c73 2e67 656e 6572 616c 5f75  _utils.general_u
-00000660: 7469 6c73 7202 0000 0072 2900 0000 722a  tilsr....r)...r*
-00000670: 0000 0072 2700 0000 7227 0000 0072 2700  ...r'...r'...r'.
-00000680: 0000 7228 0000 00da 083c 6d6f 6475 6c65  ..r(.....<module
-00000690: 3e01 0000 0073 0c00 0000 2200 0801 0801  >....s....".....
-000006a0: 0c01 0803 0c17                           ......
+00000050: 6400 6401 6c07 5a07 6400 6402 6c08 6d09  d.d.l.Z.d.d.l.m.
+00000060: 5a09 0100 6403 6404 8400 5a0a 6405 6406  Z...d.d...Z.d.d.
+00000070: 8400 5a0b 6401 5300 2907 e900 0000 004e  ..Z.d.S.)......N
+00000080: 2901 da13 6c6f 6164 5f66 6f72 5f70 726f  )...load_for_pro
+00000090: 6475 6374 696f 6e63 0000 0000 0000 0000  ductionc........
+000000a0: 0000 0000 0800 0000 0800 0000 4300 0000  ............C...
+000000b0: 73ee 0000 0064 017d 0064 027d 0164 037d  s....d.}.d.}.d.}
+000000c0: 0274 007c 007c 0117 0064 0483 028f 0e7d  .t.|.|...d.....}
+000000d0: 0374 01a0 027c 027c 03a1 0201 0057 0064  .t...|.|.....W.d
+000000e0: 0004 0004 0083 0301 006e 0831 0073 1e77  .........n.1.s.w
+000000f0: 0101 0001 0001 0059 0001 0074 037c 007c  .......Y...t.|.|
+00000100: 0164 058d 027d 047c 047c 026b 027d 057c  .d...}.|.|.k.}.|
+00000110: 0573 6c74 04a0 0564 067c 0566 0164 077c  .slt...d.|.f.d.|
+00000120: 047c 0266 02a1 0464 0874 06a0 07a1 0076  .|.f...d.t.....v
+00000130: 0073 4474 04a0 087c 04a1 0172 4974 04a0  .sDt...|...rIt..
+00000140: 097c 04a1 016e 0164 0864 0974 06a0 07a1  .|...n.d.d.t....
+00000150: 0076 0073 5574 04a0 087c 02a1 0172 5a74  .v.sUt...|...rZt
+00000160: 04a0 097c 02a1 016e 0164 0964 0a9c 0216  ...|...n.d.d....
+00000170: 007d 0664 0b64 0c7c 0669 0116 007d 0774  .}.d.d.|.i...}.t
+00000180: 0a74 04a0 0b7c 07a1 0183 0182 0164 007d  .t...|.......d.}
+00000190: 0574 0ca0 0d7c 007c 0117 00a1 0101 0064  .t...|.|.......d
+000001a0: 0053 0029 0d4e da0d 7465 7374 5f69 6e73  .S.).N..test_ins
+000001b0: 7461 6e63 65fa 042e 6461 74da 0974 6573  tance...dat..tes
+000001c0: 745f 6461 7461 da02 7762 2902 da09 6669  t_data..wb)...fi
+000001d0: 6c65 5f6e 616d 65da 0966 696c 655f 7479  le_name..file_ty
+000001e0: 7065 a901 fa02 3d3d a901 7a12 2528 7079  pe....==..z.%(py
+000001f0: 3029 7320 3d3d 2025 2870 7932 2973 da0f  0)s == %(py2)s..
+00000200: 6c6f 6164 6564 5f69 6e73 7461 6e63 65da  loaded_instance.
+00000210: 0e64 756d 6d79 5f69 6e73 7461 6e63 65a9  .dummy_instance.
+00000220: 02da 0370 7930 da03 7079 32fa 0e61 7373  ...py0..py2..ass
+00000230: 6572 7420 2528 7079 3429 73da 0370 7934  ert %(py4)s..py4
+00000240: a90e da04 6f70 656e da06 7069 636b 6c65  ....open..pickle
+00000250: da04 6475 6d70 7202 0000 00da 0a40 7079  ..dumpr......@py
+00000260: 7465 7374 5f61 72da 115f 6361 6c6c 5f72  test_ar.._call_r
+00000270: 6570 7263 6f6d 7061 7265 da0c 4070 795f  eprcompare..@py_
+00000280: 6275 696c 7469 6e73 da06 6c6f 6361 6c73  builtins..locals
+00000290: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
+000002a0: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
+000002b0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
+000002c0: 4572 726f 72da 135f 666f 726d 6174 5f65  Error.._format_e
+000002d0: 7870 6c61 6e61 7469 6f6e da02 6f73 da06  xplanation..os..
+000002e0: 7265 6d6f 7665 2908 7207 0000 0072 0800  remove).r....r..
+000002f0: 0000 720d 0000 00da 0466 696c 6572 0c00  ..r......filer..
+00000300: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
+00000310: 0b40 7079 5f66 6f72 6d61 7433 da0b 4070  .@py_format3..@p
+00000320: 795f 666f 726d 6174 35a9 0072 2500 0000  y_format5..r%...
+00000330: fa4d 2f68 6f6d 652f 7468 6f6d 6173 2f49  .M/home/thomas/I
+00000340: 6465 6150 726f 6a65 6374 732f 426c 7565  deaProjects/Blue
+00000350: 4361 7374 2f62 6c75 6563 6173 742f 7465  Cast/bluecast/te
+00000360: 7374 732f 7465 7374 5f6c 6f61 645f 666f  sts/test_load_fo
+00000370: 725f 7072 6f64 7563 7469 6f6e 2e70 79da  r_production.py.
+00000380: 1874 6573 745f 6c6f 6164 5f66 6f72 5f70  .test_load_for_p
+00000390: 726f 6475 6374 696f 6e07 0000 0073 1200  roduction....s..
+000003a0: 0000 0402 0401 0403 1003 0e01 1cff 0c04  ................
+000003b0: 8a03 1203 7227 0000 0063 0000 0000 0000  ....r'...c......
+000003c0: 0000 0000 0000 0700 0000 0800 0000 4300  ..............C.
+000003d0: 0000 73e8 0000 0064 017d 0064 027d 0174  ..s....d.}.d.}.t
+000003e0: 007c 0064 0317 0064 0483 028f 0e7d 0274  .|.d...d.....}.t
+000003f0: 01a0 027c 017c 02a1 0201 0057 0064 0004  ...|.|.....W.d..
+00000400: 0004 0083 0301 006e 0831 0073 1c77 0101  .......n.1.s.w..
+00000410: 0001 0001 0059 0001 0074 037c 0064 058d  .....Y...t.|.d..
+00000420: 017d 037c 037c 016b 027d 047c 0473 6974  .}.|.|.k.}.|.sit
+00000430: 04a0 0564 067c 0466 0164 077c 037c 0166  ...d.|.f.d.|.|.f
+00000440: 02a1 0464 0874 06a0 07a1 0076 0073 4174  ...d.t.....v.sAt
+00000450: 04a0 087c 03a1 0172 4674 04a0 097c 03a1  ...|...rFt...|..
+00000460: 016e 0164 0864 0974 06a0 07a1 0076 0073  .n.d.d.t.....v.s
+00000470: 5274 04a0 087c 01a1 0172 5774 04a0 097c  Rt...|...rWt...|
+00000480: 01a1 016e 0164 0964 0a9c 0216 007d 0564  ...n.d.d.....}.d
+00000490: 0b64 0c7c 0569 0116 007d 0674 0a74 04a0  .d.|.i...}.t.t..
+000004a0: 0b7c 06a1 0183 0182 0164 007d 0474 0ca0  .|.......d.}.t..
+000004b0: 0d7c 0064 0317 00a1 0101 0064 0053 0029  .|.d.......d.S.)
+000004c0: 0d4e 7203 0000 0072 0500 0000 7204 0000  .Nr....r....r...
+000004d0: 0072 0600 0000 2901 7207 0000 0072 0900  .r....).r....r..
+000004e0: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000004f0: 0072 0e00 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000500: 7213 0000 0029 0772 0700 0000 720d 0000  r....).r....r...
+00000510: 0072 2100 0000 720c 0000 0072 2200 0000  .r!...r....r"...
+00000520: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
+00000530: 2500 0000 7226 0000 00da 2f74 6573 745f  %...r&..../test_
+00000540: 6c6f 6164 5f66 6f72 5f70 726f 6475 6374  load_for_product
+00000550: 696f 6e5f 7769 7468 5f64 6566 6175 6c74  ion_with_default
+00000560: 5f66 696c 655f 7479 7065 1d00 0000 7310  _file_type....s.
+00000570: 0000 0004 0204 0310 030e 011c ff0a 048a  ................
+00000580: 0312 0372 2800 0000 290c da08 6275 696c  ...r(...)...buil
+00000590: 7469 6e73 7219 0000 00da 195f 7079 7465  tinsr......_pyte
+000005a0: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
+000005b0: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
+000005c0: 0772 6577 7269 7465 7217 0000 0072 1f00  .rewriter....r..
+000005d0: 0000 7215 0000 00da 2462 6c75 6563 6173  ..r.....$bluecas
+000005e0: 742e 6765 6e65 7261 6c5f 7574 696c 732e  t.general_utils.
+000005f0: 6765 6e65 7261 6c5f 7574 696c 7372 0200  general_utilsr..
+00000600: 0000 7227 0000 0072 2800 0000 7225 0000  ..r'...r(...r%..
+00000610: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00000620: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000630: 0000 0022 0008 010c 0208 030c 16         ...".........
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 04:56:12 2023 UTC, .py size: 1575 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec0d 8064 2706 0000  o..........d'...
+00000000: 6f0d 0d0a 0000 0000 ab09 8064 2706 0000  o..........d'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6401 6c08 5a09 6400 6402 6c0a 6d0b  d.d.l.Z.d.d.l.m.
 00000060: 5a0b 6d0c 5a0c 0100 6403 6404 8400 5a0d  Z.m.Z...d.d...Z.
 00000070: 6405 6406 8400 5a0e 6401 5300 2907 e900  d.d...Z.d.S.)...
@@ -128,161 +128,160 @@
 000007f0: 7365 7274 3134 da0c 4070 795f 6173 7365  sert14..@py_asse
 00000800: 7274 3137 5a0c 4070 795f 6173 7365 7274  rt17Z.@py_assert
 00000810: 3139 5a0c 4070 795f 666f 726d 6174 3231  19Z.@py_format21
 00000820: 721e 0000 00da 0b40 7079 5f61 7373 6572  r......@py_asser
 00000830: 7437 da0c 4070 795f 6173 7365 7274 3132  t7..@py_assert12
 00000840: da0c 4070 795f 6173 7365 7274 3135 da0c  ..@py_assert15..
 00000850: 4070 795f 666f 726d 6174 3139 a900 7238  @py_format19..r8
-00000860: 0000 00fa 512f 5573 6572 732f 7468 6f6d  ....Q/Users/thom
-00000870: 6173 6d65 6973 736e 6572 2f49 6465 6150  asmeissner/IdeaP
-00000880: 726f 6a65 6374 732f 426c 7565 4361 7374  rojects/BlueCast
-00000890: 2f62 6c75 6563 6173 742f 7465 7374 732f  /bluecast/tests/
-000008a0: 7465 7374 5f6e 756c 6c73 5f61 6e64 5f69  test_nulls_and_i
-000008b0: 6e66 732e 7079 da0f 7465 7374 5f66 696c  nfs.py..test_fil
-000008c0: 6c5f 6e75 6c6c 7307 0000 0073 1200 0000  l_nulls....s....
-000008d0: 1802 1803 fe01 6200 0405 2401 04ff fe03  ......b...$.....
-000008e0: 6800 723a 0000 0063 0000 0000 0000 0000  h.r:...c........
-000008f0: 0000 0000 0f00 0000 0f00 0000 4300 0000  ............C...
-00000900: 73c8 0300 0074 00a0 0164 0164 0274 026a  s....t...d.d.t.j
-00000910: 0364 0367 0474 026a 0364 0474 026a 030b  .d.g.t.j.d.t.j..
-00000920: 0064 0567 0464 069c 02a1 017d 0074 00a0  .d.g.d.....}.t..
-00000930: 0167 0064 07a2 0167 0064 08a2 0164 069c  .g.d...g.d...d..
-00000940: 02a1 017d 017c 006a 047d 027c 0274 0583  ...}.|.j.}.|.t..
-00000950: 017d 0374 067c 0383 017d 047c 046a 077d  .}.t.|...}.|.j.}
-00000960: 057c 016a 047d 067c 0674 0583 017d 077c  .|.j.}.|.t...}.|
-00000970: 057c 0783 017d 087c 0873 b864 0964 0a74  .|...}.|.s.d.d.t
-00000980: 08a0 09a1 0076 0073 4774 0aa0 0b74 06a1  .....v.sGt...t..
-00000990: 0172 4c74 0aa0 0c74 06a1 016e 0164 0a64  .rLt...t...n.d.d
-000009a0: 0b74 08a0 09a1 0076 0073 5874 0aa0 0b7c  .t.....v.sXt...|
-000009b0: 00a1 0172 5d74 0aa0 0c7c 00a1 016e 0164  ...r]t...|...n.d
-000009c0: 0b74 0aa0 0c7c 02a1 0164 0c74 08a0 09a1  .t...|...d.t....
-000009d0: 0076 0073 6d74 0aa0 0b74 05a1 0172 7274  .v.smt...t...rrt
-000009e0: 0aa0 0c74 05a1 016e 0164 0c74 0aa0 0c7c  ...t...n.d.t...|
-000009f0: 03a1 0174 0aa0 0c7c 04a1 0174 0aa0 0c7c  ...t...|...t...|
-00000a00: 05a1 0164 0d74 08a0 09a1 0076 0073 8a74  ...d.t.....v.s.t
-00000a10: 0aa0 0b7c 01a1 0172 8f74 0aa0 0c7c 01a1  ...|...r.t...|..
-00000a20: 016e 0164 0d74 0aa0 0c7c 06a1 0164 0c74  .n.d.t...|...d.t
-00000a30: 08a0 09a1 0076 0073 9f74 0aa0 0b74 05a1  .....v.s.t...t..
-00000a40: 0172 a474 0aa0 0c74 05a1 016e 0164 0c74  .r.t...t...n.d.t
-00000a50: 0aa0 0c7c 07a1 0174 0aa0 0c7c 08a1 0164  ...|...t...|...d
-00000a60: 0e9c 0c16 007d 0974 0d74 0aa0 0e7c 09a1  .....}.t.t...|..
-00000a70: 0183 0182 0164 0004 007d 0204 007d 0304  .....d...}...}..
-00000a80: 007d 0404 007d 0504 007d 0604 007d 077d  .}...}...}...}.}
-00000a90: 0874 00a0 0167 0064 0fa2 0167 0064 10a2  .t...g.d...g.d..
-00000aa0: 0164 069c 02a1 017d 0164 117d 0274 067c  .d.....}.d.}.t.|
-00000ab0: 007c 0264 128d 027d 0a7c 0a6a 077d 0b7c  .|.d...}.|.j.}.|
-00000ac0: 016a 047d 057c 0574 0583 017d 067c 0b7c  .j.}.|.t...}.|.|
-00000ad0: 0683 017d 0c7c 0c90 0173 5964 1364 0a74  ...}.|...sYd.d.t
-00000ae0: 08a0 09a1 0076 0073 f774 0aa0 0b74 06a1  .....v.s.t...t..
-00000af0: 0172 fc74 0aa0 0c74 06a1 016e 0164 0a64  .r.t...t...n.d.d
-00000b00: 0b74 08a0 09a1 0076 0090 0173 0a74 0aa0  .t.....v...s.t..
-00000b10: 0b7c 00a1 0190 0172 0f74 0aa0 0c7c 00a1  .|.....r.t...|..
-00000b20: 016e 0164 0b74 0aa0 0c7c 02a1 0174 0aa0  .n.d.t...|...t..
-00000b30: 0c7c 0aa1 0174 0aa0 0c7c 0ba1 0164 0d74  .|...t...|...d.t
-00000b40: 08a0 09a1 0076 0090 0173 2974 0aa0 0b7c  .....v...s)t...|
-00000b50: 01a1 0190 0172 2e74 0aa0 0c7c 01a1 016e  .....r.t...|...n
-00000b60: 0164 0d74 0aa0 0c7c 05a1 0164 0c74 08a0  .d.t...|...d.t..
-00000b70: 09a1 0076 0090 0173 4074 0aa0 0b74 05a1  ...v...s@t...t..
-00000b80: 0190 0172 4574 0aa0 0c74 05a1 016e 0164  ...rEt...t...n.d
-00000b90: 0c74 0aa0 0c7c 06a1 0174 0aa0 0c7c 0ca1  .t...|...t...|..
-00000ba0: 0164 149c 0a16 007d 0d74 0d74 0aa0 0e7c  .d.....}.t.t...|
-00000bb0: 0da1 0183 0182 0164 0004 007d 0204 007d  .......d...}...}
-00000bc0: 0a04 007d 0b04 007d 0504 007d 067d 0c74  ...}...}...}.}.t
-00000bd0: 00a0 0167 0064 15a2 0167 0064 16a2 0164  ...g.d...g.d...d
-00000be0: 069c 02a1 017d 0074 00a0 0167 0064 15a2  .....}.t...g.d..
-00000bf0: 0167 0064 16a2 0164 069c 02a1 017d 0174  .g.d...d.....}.t
-00000c00: 067c 0083 017d 027c 026a 077d 0a7c 0a7c  .|...}.|.j.}.|.|
-00000c10: 0183 017d 047c 0490 0173 dc64 1764 0a74  ...}.|...s.d.d.t
-00000c20: 08a0 09a1 0076 0090 0173 9974 0aa0 0b74  .....v...s.t...t
-00000c30: 06a1 0190 0172 9e74 0aa0 0c74 06a1 016e  .....r.t...t...n
-00000c40: 0164 0a64 0b74 08a0 09a1 0076 0090 0173  .d.d.t.....v...s
-00000c50: ac74 0aa0 0b7c 00a1 0190 0172 b174 0aa0  .t...|.....r.t..
-00000c60: 0c7c 00a1 016e 0164 0b74 0aa0 0c7c 02a1  .|...n.d.t...|..
-00000c70: 0174 0aa0 0c7c 0aa1 0164 0d74 08a0 09a1  .t...|...d.t....
-00000c80: 0076 0090 0173 c774 0aa0 0b7c 01a1 0190  .v...s.t...|....
-00000c90: 0172 cc74 0aa0 0c7c 01a1 016e 0164 0d74  .r.t...|...n.d.t
-00000ca0: 0aa0 0c7c 04a1 0164 189c 0616 007d 0e74  ...|...d.....}.t
-00000cb0: 0d74 0aa0 0e7c 0ea1 0183 0182 0164 0004  .t...|.......d..
-00000cc0: 007d 0204 007d 0a7d 0464 0053 0029 194e  .}...}.}.d.S.).N
-00000cd0: 7204 0000 00e9 0200 0000 7206 0000 0072  r.........r....r
-00000ce0: 0700 0000 e908 0000 0072 0900 0000 2904  .........r....).
-00000cf0: 7204 0000 0072 3b00 0000 7201 0000 0072  r....r;...r....r
-00000d00: 0600 0000 2904 7201 0000 0072 0700 0000  ....).r....r....
-00000d10: 7201 0000 0072 3c00 0000 7ae4 6173 7365  r....r<...z.asse
-00000d20: 7274 2025 2870 7931 3829 730a 7b25 2870  rt %(py18)s.{%(p
-00000d30: 7931 3829 7320 3d20 2528 7079 3130 2973  y18)s = %(py10)s
-00000d40: 0a7b 2528 7079 3130 2973 203d 2025 2870  .{%(py10)s = %(p
-00000d50: 7938 2973 0a7b 2528 7079 3829 7320 3d20  y8)s.{%(py8)s = 
-00000d60: 2528 7079 3029 7328 2528 7079 3629 730a  %(py0)s(%(py6)s.
-00000d70: 7b25 2870 7936 2973 203d 2025 2870 7933  {%(py6)s = %(py3
-00000d80: 2973 0a7b 2528 7079 3329 7320 3d20 2528  )s.{%(py3)s = %(
-00000d90: 7079 3129 732e 6173 7479 7065 0a7d 2825  py1)s.astype.}(%
-00000da0: 2870 7934 2973 290a 7d29 0a7d 2e65 7175  (py4)s).}).}.equ
-00000db0: 616c 730a 7d28 2528 7079 3136 2973 0a7b  als.}(%(py16)s.{
-00000dc0: 2528 7079 3136 2973 203d 2025 2870 7931  %(py16)s = %(py1
-00000dd0: 3329 730a 7b25 2870 7931 3329 7320 3d20  3)s.{%(py13)s = 
-00000de0: 2528 7079 3131 2973 2e61 7374 7970 650a  %(py11)s.astype.
-00000df0: 7d28 2528 7079 3134 2973 290a 7d29 0a7d  }(%(py14)s).}).}
-00000e00: 7202 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00000e10: 0f65 7870 6563 7465 645f 7265 7375 6c74  .expected_result
-00000e20: 290c 7211 0000 0072 1200 0000 7213 0000  ).r....r....r...
-00000e30: 00da 0370 7934 721f 0000 0072 1600 0000  ...py4r....r....
-00000e40: 7217 0000 0072 2000 0000 7219 0000 0072  r....r ...r....r
-00000e50: 2100 0000 721b 0000 0072 1c00 0000 2904  !...r....r....).
-00000e60: 7204 0000 0072 3b00 0000 e90a 0000 0072  r....r;........r
-00000e70: 0600 0000 2904 723f 0000 0072 0700 0000  ....).r?...r....
-00000e80: 723f 0000 0072 3c00 0000 723f 0000 0072  r?...r<...r?...r
-00000e90: 0c00 0000 7aba 6173 7365 7274 2025 2870  ....z.assert %(p
-00000ea0: 7931 3529 730a 7b25 2870 7931 3529 7320  y15)s.{%(py15)s 
-00000eb0: 3d20 2528 7079 3729 730a 7b25 2870 7937  = %(py7)s.{%(py7
-00000ec0: 2973 203d 2025 2870 7935 2973 0a7b 2528  )s = %(py5)s.{%(
-00000ed0: 7079 3529 7320 3d20 2528 7079 3029 7328  py5)s = %(py0)s(
-00000ee0: 2528 7079 3129 732c 2066 696c 6c5f 7769  %(py1)s, fill_wi
-00000ef0: 7468 3d25 2870 7933 2973 290a 7d2e 6571  th=%(py3)s).}.eq
-00000f00: 7561 6c73 0a7d 2825 2870 7931 3329 730a  uals.}(%(py13)s.
-00000f10: 7b25 2870 7931 3329 7320 3d20 2528 7079  {%(py13)s = %(py
-00000f20: 3130 2973 0a7b 2528 7079 3130 2973 203d  10)s.{%(py10)s =
-00000f30: 2025 2870 7938 2973 2e61 7374 7970 650a   %(py8)s.astype.
-00000f40: 7d28 2528 7079 3131 2973 290a 7d29 0a7d  }(%(py11)s).}).}
-00000f50: 290a 7211 0000 0072 1200 0000 7213 0000  ).r....r....r...
-00000f60: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000f70: 7217 0000 0072 2000 0000 7219 0000 0072  r....r ...r....r
-00000f80: 1a00 0000 2903 7204 0000 0072 3b00 0000  ....).r....r;...
-00000f90: 7205 0000 0029 0372 0600 0000 e905 0000  r....).r........
-00000fa0: 0072 0700 0000 7a66 6173 7365 7274 2025  .r....zfassert %
-00000fb0: 2870 7938 2973 0a7b 2528 7079 3829 7320  (py8)s.{%(py8)s 
-00000fc0: 3d20 2528 7079 3529 730a 7b25 2870 7935  = %(py5)s.{%(py5
-00000fd0: 2973 203d 2025 2870 7933 2973 0a7b 2528  )s = %(py3)s.{%(
-00000fe0: 7079 3329 7320 3d20 2528 7079 3029 7328  py3)s = %(py0)s(
-00000ff0: 2528 7079 3129 7329 0a7d 2e65 7175 616c  %(py1)s).}.equal
-00001000: 730a 7d28 2528 7079 3629 7329 0a7d 2906  s.}(%(py6)s).}).
-00001010: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00001020: 1400 0000 721f 0000 0072 1600 0000 290f  ....r....r....).
-00001030: 7222 0000 0072 2300 0000 da02 6e70 da03  r"...r#.....np..
-00001040: 696e 6672 2400 0000 720f 0000 0072 0200  infr$...r....r..
-00001050: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
-00001060: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
-00001070: 722b 0000 0072 2c00 0000 290f 720e 0000  r+...r,...).r...
-00001080: 0072 3d00 0000 722d 0000 00da 0b40 7079  .r=...r-.....@py
-00001090: 5f61 7373 6572 7435 7234 0000 0072 3000  _assert5r4...r0.
-000010a0: 0000 7235 0000 0072 3600 0000 7233 0000  ..r5...r6...r3..
-000010b0: 0072 3700 0000 722e 0000 0072 2f00 0000  .r7...r....r/...
-000010c0: 7232 0000 005a 0c40 7079 5f66 6f72 6d61  r2...Z.@py_forma
-000010d0: 7431 36da 0b40 7079 5f66 6f72 6d61 7439  t16..@py_format9
-000010e0: 7238 0000 0072 3800 0000 7239 0000 00da  r8...r8...r9....
-000010f0: 1974 6573 745f 6669 6c6c 5f69 6e66 696e  .test_fill_infin
-00001100: 6974 655f 7661 6c75 6573 1800 0000 7314  ite_values....s.
-00001110: 0000 0028 0218 03fe 014e 0018 03fe 0128  ...(.....N.....(
-00001120: 0018 0318 01ce 0172 4500 0000 290f da08  .......rE...)...
-00001130: 6275 696c 7469 6e73 7226 0000 00da 195f  builtinsr&....._
-00001140: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
-00001150: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
-00001160: 696f 6eda 0772 6577 7269 7465 7228 0000  ion..rewriter(..
-00001170: 00da 056e 756d 7079 7241 0000 00da 0670  ...numpyrA.....p
-00001180: 616e 6461 7372 2200 0000 da25 626c 7565  andasr"....%blue
-00001190: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
-000011a0: 6e67 2e6e 756c 6c73 5f61 6e64 5f69 6e66  ng.nulls_and_inf
-000011b0: 7372 0200 0000 7203 0000 0072 3a00 0000  sr....r....r:...
-000011c0: 7245 0000 0072 3800 0000 7238 0000 0072  rE...r8...r8...r
-000011d0: 3800 0000 7239 0000 00da 083c 6d6f 6475  8...r9.....<modu
-000011e0: 6c65 3e01 0000 0073 0a00 0000 2200 0801  le>....s...."...
-000011f0: 1002 0803 0c11                           ......
+00000860: 0000 00fa 482f 686f 6d65 2f74 686f 6d61  ....H/home/thoma
+00000870: 732f 4964 6561 5072 6f6a 6563 7473 2f42  s/IdeaProjects/B
+00000880: 6c75 6543 6173 742f 626c 7565 6361 7374  lueCast/bluecast
+00000890: 2f74 6573 7473 2f74 6573 745f 6e75 6c6c  /tests/test_null
+000008a0: 735f 616e 645f 696e 6673 2e70 79da 0f74  s_and_infs.py..t
+000008b0: 6573 745f 6669 6c6c 5f6e 756c 6c73 0700  est_fill_nulls..
+000008c0: 0000 7312 0000 0018 0218 03fe 0162 0004  ..s..........b..
+000008d0: 0524 0104 fffe 0368 0072 3a00 0000 6300  .$.....h.r:...c.
+000008e0: 0000 0000 0000 0000 0000 000f 0000 000f  ................
+000008f0: 0000 0043 0000 0073 c803 0000 7400 a001  ...C...s....t...
+00000900: 6401 6402 7402 6a03 6403 6704 7402 6a03  d.d.t.j.d.g.t.j.
+00000910: 6404 7402 6a03 0b00 6405 6704 6406 9c02  d.t.j...d.g.d...
+00000920: a101 7d00 7400 a001 6700 6407 a201 6700  ..}.t...g.d...g.
+00000930: 6408 a201 6406 9c02 a101 7d01 7c00 6a04  d...d.....}.|.j.
+00000940: 7d02 7c02 7405 8301 7d03 7406 7c03 8301  }.|.t...}.t.|...
+00000950: 7d04 7c04 6a07 7d05 7c01 6a04 7d06 7c06  }.|.j.}.|.j.}.|.
+00000960: 7405 8301 7d07 7c05 7c07 8301 7d08 7c08  t...}.|.|...}.|.
+00000970: 73b8 6409 640a 7408 a009 a100 7600 7347  s.d.d.t.....v.sG
+00000980: 740a a00b 7406 a101 724c 740a a00c 7406  t...t...rLt...t.
+00000990: a101 6e01 640a 640b 7408 a009 a100 7600  ..n.d.d.t.....v.
+000009a0: 7358 740a a00b 7c00 a101 725d 740a a00c  sXt...|...r]t...
+000009b0: 7c00 a101 6e01 640b 740a a00c 7c02 a101  |...n.d.t...|...
+000009c0: 640c 7408 a009 a100 7600 736d 740a a00b  d.t.....v.smt...
+000009d0: 7405 a101 7272 740a a00c 7405 a101 6e01  t...rrt...t...n.
+000009e0: 640c 740a a00c 7c03 a101 740a a00c 7c04  d.t...|...t...|.
+000009f0: a101 740a a00c 7c05 a101 640d 7408 a009  ..t...|...d.t...
+00000a00: a100 7600 738a 740a a00b 7c01 a101 728f  ..v.s.t...|...r.
+00000a10: 740a a00c 7c01 a101 6e01 640d 740a a00c  t...|...n.d.t...
+00000a20: 7c06 a101 640c 7408 a009 a100 7600 739f  |...d.t.....v.s.
+00000a30: 740a a00b 7405 a101 72a4 740a a00c 7405  t...t...r.t...t.
+00000a40: a101 6e01 640c 740a a00c 7c07 a101 740a  ..n.d.t...|...t.
+00000a50: a00c 7c08 a101 640e 9c0c 1600 7d09 740d  ..|...d.....}.t.
+00000a60: 740a a00e 7c09 a101 8301 8201 6400 0400  t...|.......d...
+00000a70: 7d02 0400 7d03 0400 7d04 0400 7d05 0400  }...}...}...}...
+00000a80: 7d06 0400 7d07 7d08 7400 a001 6700 640f  }...}.}.t...g.d.
+00000a90: a201 6700 6410 a201 6406 9c02 a101 7d01  ..g.d...d.....}.
+00000aa0: 6411 7d02 7406 7c00 7c02 6412 8d02 7d0a  d.}.t.|.|.d...}.
+00000ab0: 7c0a 6a07 7d0b 7c01 6a04 7d05 7c05 7405  |.j.}.|.j.}.|.t.
+00000ac0: 8301 7d06 7c0b 7c06 8301 7d0c 7c0c 9001  ..}.|.|...}.|...
+00000ad0: 7359 6413 640a 7408 a009 a100 7600 73f7  sYd.d.t.....v.s.
+00000ae0: 740a a00b 7406 a101 72fc 740a a00c 7406  t...t...r.t...t.
+00000af0: a101 6e01 640a 640b 7408 a009 a100 7600  ..n.d.d.t.....v.
+00000b00: 9001 730a 740a a00b 7c00 a101 9001 720f  ..s.t...|.....r.
+00000b10: 740a a00c 7c00 a101 6e01 640b 740a a00c  t...|...n.d.t...
+00000b20: 7c02 a101 740a a00c 7c0a a101 740a a00c  |...t...|...t...
+00000b30: 7c0b a101 640d 7408 a009 a100 7600 9001  |...d.t.....v...
+00000b40: 7329 740a a00b 7c01 a101 9001 722e 740a  s)t...|.....r.t.
+00000b50: a00c 7c01 a101 6e01 640d 740a a00c 7c05  ..|...n.d.t...|.
+00000b60: a101 640c 7408 a009 a100 7600 9001 7340  ..d.t.....v...s@
+00000b70: 740a a00b 7405 a101 9001 7245 740a a00c  t...t.....rEt...
+00000b80: 7405 a101 6e01 640c 740a a00c 7c06 a101  t...n.d.t...|...
+00000b90: 740a a00c 7c0c a101 6414 9c0a 1600 7d0d  t...|...d.....}.
+00000ba0: 740d 740a a00e 7c0d a101 8301 8201 6400  t.t...|.......d.
+00000bb0: 0400 7d02 0400 7d0a 0400 7d0b 0400 7d05  ..}...}...}...}.
+00000bc0: 0400 7d06 7d0c 7400 a001 6700 6415 a201  ..}.}.t...g.d...
+00000bd0: 6700 6416 a201 6406 9c02 a101 7d00 7400  g.d...d.....}.t.
+00000be0: a001 6700 6415 a201 6700 6416 a201 6406  ..g.d...g.d...d.
+00000bf0: 9c02 a101 7d01 7406 7c00 8301 7d02 7c02  ....}.t.|...}.|.
+00000c00: 6a07 7d0a 7c0a 7c01 8301 7d04 7c04 9001  j.}.|.|...}.|...
+00000c10: 73dc 6417 640a 7408 a009 a100 7600 9001  s.d.d.t.....v...
+00000c20: 7399 740a a00b 7406 a101 9001 729e 740a  s.t...t.....r.t.
+00000c30: a00c 7406 a101 6e01 640a 640b 7408 a009  ..t...n.d.d.t...
+00000c40: a100 7600 9001 73ac 740a a00b 7c00 a101  ..v...s.t...|...
+00000c50: 9001 72b1 740a a00c 7c00 a101 6e01 640b  ..r.t...|...n.d.
+00000c60: 740a a00c 7c02 a101 740a a00c 7c0a a101  t...|...t...|...
+00000c70: 640d 7408 a009 a100 7600 9001 73c7 740a  d.t.....v...s.t.
+00000c80: a00b 7c01 a101 9001 72cc 740a a00c 7c01  ..|.....r.t...|.
+00000c90: a101 6e01 640d 740a a00c 7c04 a101 6418  ..n.d.t...|...d.
+00000ca0: 9c06 1600 7d0e 740d 740a a00e 7c0e a101  ....}.t.t...|...
+00000cb0: 8301 8201 6400 0400 7d02 0400 7d0a 7d04  ....d...}...}.}.
+00000cc0: 6400 5300 2919 4e72 0400 0000 e902 0000  d.S.).Nr........
+00000cd0: 0072 0600 0000 7207 0000 00e9 0800 0000  .r....r.........
+00000ce0: 7209 0000 0029 0472 0400 0000 723b 0000  r....).r....r;..
+00000cf0: 0072 0100 0000 7206 0000 0029 0472 0100  .r....r....).r..
+00000d00: 0000 7207 0000 0072 0100 0000 723c 0000  ..r....r....r<..
+00000d10: 007a e461 7373 6572 7420 2528 7079 3138  .z.assert %(py18
+00000d20: 2973 0a7b 2528 7079 3138 2973 203d 2025  )s.{%(py18)s = %
+00000d30: 2870 7931 3029 730a 7b25 2870 7931 3029  (py10)s.{%(py10)
+00000d40: 7320 3d20 2528 7079 3829 730a 7b25 2870  s = %(py8)s.{%(p
+00000d50: 7938 2973 203d 2025 2870 7930 2973 2825  y8)s = %(py0)s(%
+00000d60: 2870 7936 2973 0a7b 2528 7079 3629 7320  (py6)s.{%(py6)s 
+00000d70: 3d20 2528 7079 3329 730a 7b25 2870 7933  = %(py3)s.{%(py3
+00000d80: 2973 203d 2025 2870 7931 2973 2e61 7374  )s = %(py1)s.ast
+00000d90: 7970 650a 7d28 2528 7079 3429 7329 0a7d  ype.}(%(py4)s).}
+00000da0: 290a 7d2e 6571 7561 6c73 0a7d 2825 2870  ).}.equals.}(%(p
+00000db0: 7931 3629 730a 7b25 2870 7931 3629 7320  y16)s.{%(py16)s 
+00000dc0: 3d20 2528 7079 3133 2973 0a7b 2528 7079  = %(py13)s.{%(py
+00000dd0: 3133 2973 203d 2025 2870 7931 3129 732e  13)s = %(py11)s.
+00000de0: 6173 7479 7065 0a7d 2825 2870 7931 3429  astype.}(%(py14)
+00000df0: 7329 0a7d 290a 7d72 0200 0000 720e 0000  s).}).}r....r...
+00000e00: 0072 0f00 0000 da0f 6578 7065 6374 6564  .r......expected
+00000e10: 5f72 6573 756c 7429 0c72 1100 0000 7212  _result).r....r.
+00000e20: 0000 0072 1300 0000 da03 7079 3472 1f00  ...r......py4r..
+00000e30: 0000 7216 0000 0072 1700 0000 7220 0000  ..r....r....r ..
+00000e40: 0072 1900 0000 7221 0000 0072 1b00 0000  .r....r!...r....
+00000e50: 721c 0000 0029 0472 0400 0000 723b 0000  r....).r....r;..
+00000e60: 00e9 0a00 0000 7206 0000 0029 0472 3f00  ......r....).r?.
+00000e70: 0000 7207 0000 0072 3f00 0000 723c 0000  ..r....r?...r<..
+00000e80: 0072 3f00 0000 720c 0000 007a ba61 7373  .r?...r....z.ass
+00000e90: 6572 7420 2528 7079 3135 2973 0a7b 2528  ert %(py15)s.{%(
+00000ea0: 7079 3135 2973 203d 2025 2870 7937 2973  py15)s = %(py7)s
+00000eb0: 0a7b 2528 7079 3729 7320 3d20 2528 7079  .{%(py7)s = %(py
+00000ec0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
+00000ed0: 2870 7930 2973 2825 2870 7931 2973 2c20  (py0)s(%(py1)s, 
+00000ee0: 6669 6c6c 5f77 6974 683d 2528 7079 3329  fill_with=%(py3)
+00000ef0: 7329 0a7d 2e65 7175 616c 730a 7d28 2528  s).}.equals.}(%(
+00000f00: 7079 3133 2973 0a7b 2528 7079 3133 2973  py13)s.{%(py13)s
+00000f10: 203d 2025 2870 7931 3029 730a 7b25 2870   = %(py10)s.{%(p
+00000f20: 7931 3029 7320 3d20 2528 7079 3829 732e  y10)s = %(py8)s.
+00000f30: 6173 7479 7065 0a7d 2825 2870 7931 3129  astype.}(%(py11)
+00000f40: 7329 0a7d 290a 7d29 0a72 1100 0000 7212  s).}).}).r....r.
+00000f50: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+00000f60: 0000 7216 0000 0072 1700 0000 7220 0000  ..r....r....r ..
+00000f70: 0072 1900 0000 721a 0000 0029 0372 0400  .r....r....).r..
+00000f80: 0000 723b 0000 0072 0500 0000 2903 7206  ..r;...r....).r.
+00000f90: 0000 00e9 0500 0000 7207 0000 007a 6661  ........r....zfa
+00000fa0: 7373 6572 7420 2528 7079 3829 730a 7b25  ssert %(py8)s.{%
+00000fb0: 2870 7938 2973 203d 2025 2870 7935 2973  (py8)s = %(py5)s
+00000fc0: 0a7b 2528 7079 3529 7320 3d20 2528 7079  .{%(py5)s = %(py
+00000fd0: 3329 730a 7b25 2870 7933 2973 203d 2025  3)s.{%(py3)s = %
+00000fe0: 2870 7930 2973 2825 2870 7931 2973 290a  (py0)s(%(py1)s).
+00000ff0: 7d2e 6571 7561 6c73 0a7d 2825 2870 7936  }.equals.}(%(py6
+00001000: 2973 290a 7d29 0672 1100 0000 7212 0000  )s).}).r....r...
+00001010: 0072 1300 0000 7214 0000 0072 1f00 0000  .r....r....r....
+00001020: 7216 0000 0029 0f72 2200 0000 7223 0000  r....).r"...r#..
+00001030: 00da 026e 70da 0369 6e66 7224 0000 0072  ...np..infr$...r
+00001040: 0f00 0000 7202 0000 0072 2500 0000 7226  ....r....r%...r&
+00001050: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
+00001060: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
+00001070: 0029 0f72 0e00 0000 723d 0000 0072 2d00  .).r....r=...r-.
+00001080: 0000 da0b 4070 795f 6173 7365 7274 3572  ....@py_assert5r
+00001090: 3400 0000 7230 0000 0072 3500 0000 7236  4...r0...r5...r6
+000010a0: 0000 0072 3300 0000 7237 0000 0072 2e00  ...r3...r7...r..
+000010b0: 0000 722f 0000 0072 3200 0000 5a0c 4070  ..r/...r2...Z.@p
+000010c0: 795f 666f 726d 6174 3136 da0b 4070 795f  y_format16..@py_
+000010d0: 666f 726d 6174 3972 3800 0000 7238 0000  format9r8...r8..
+000010e0: 0072 3900 0000 da19 7465 7374 5f66 696c  .r9.....test_fil
+000010f0: 6c5f 696e 6669 6e69 7465 5f76 616c 7565  l_infinite_value
+00001100: 7318 0000 0073 1400 0000 2802 1803 fe01  s....s....(.....
+00001110: 4e00 1803 fe01 2800 1803 1801 ce01 7245  N.....(.......rE
+00001120: 0000 0029 0fda 0862 7569 6c74 696e 7372  ...)...builtinsr
+00001130: 2600 0000 da19 5f70 7974 6573 742e 6173  &....._pytest.as
+00001140: 7365 7274 696f 6e2e 7265 7772 6974 65da  sertion.rewrite.
+00001150: 0961 7373 6572 7469 6f6e da07 7265 7772  .assertion..rewr
+00001160: 6974 6572 2800 0000 da05 6e75 6d70 7972  iter(.....numpyr
+00001170: 4100 0000 da06 7061 6e64 6173 7222 0000  A.....pandasr"..
+00001180: 00da 2562 6c75 6563 6173 742e 7072 6570  ..%bluecast.prep
+00001190: 726f 6365 7373 696e 672e 6e75 6c6c 735f  rocessing.nulls_
+000011a0: 616e 645f 696e 6673 7202 0000 0072 0300  and_infsr....r..
+000011b0: 0000 723a 0000 0072 4500 0000 7238 0000  ..r:...rE...r8..
+000011c0: 0072 3800 0000 7238 0000 0072 3900 0000  .r8...r8...r9...
+000011d0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+000011e0: 0000 0022 0008 0110 0208 030c 11         ...".........
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 18:47:12 2023 UTC, .py size: 1216 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,119 @@
-00000000: 6f0d 0d0a 0000 0000 3022 8264 c004 0000  o.......0".d....
+00000000: 6f0d 0d0a 0000 0000 11be 8264 fc03 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
-00000050: 6400 6401 6c07 5a07 6400 6401 6c08 5a08  d.d.l.Z.d.d.l.Z.
-00000060: 6400 6402 6c09 6d0a 5a0a 0100 6400 6403  d.d.l.m.Z...d.d.
-00000070: 6c0b 6d0c 5a0c 0100 4700 6404 6405 8400  l.m.Z...G.d.d...
-00000080: 6405 8302 5a0d 6406 6407 8400 5a0e 6401  d...Z.d.d...Z.d.
-00000090: 5300 2908 e900 0000 004e 2901 da12 5465  S.)......N)...Te
-000000a0: 6d70 6f72 6172 7944 6972 6563 746f 7279  mporaryDirectory
-000000b0: 2901 da12 7361 7665 5f74 6f5f 7072 6f64  )...save_to_prod
-000000c0: 7563 7469 6f6e 6300 0000 0000 0000 0000  uctionc.........
-000000d0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-000000e0: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
-000000f0: 8400 5a03 6403 5300 2904 da0a 4475 6d6d  ..Z.d.S.)...Dumm
-00000100: 7943 6c61 7373 6302 0000 0000 0000 0000  yClassc.........
-00000110: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00000120: 0a00 0000 7c01 7c00 5f00 6400 5300 2901  ....|.|._.d.S.).
-00000130: 4e29 01da 0464 6174 6129 02da 0473 656c  N)...data)...sel
-00000140: 6672 0500 0000 a900 7207 0000 00fa 552f  fr......r.....U/
-00000150: 5573 6572 732f 7468 6f6d 6173 6d65 6973  Users/thomasmeis
-00000160: 736e 6572 2f49 6465 6150 726f 6a65 6374  sner/IdeaProject
-00000170: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
-00000180: 6173 742f 7465 7374 732f 7465 7374 5f73  ast/tests/test_s
-00000190: 6176 655f 746f 5f70 726f 6475 6374 696f  ave_to_productio
-000001a0: 6e2e 7079 da08 5f5f 696e 6974 5f5f 0900  n.py..__init__..
-000001b0: 0000 7302 0000 000a 017a 1344 756d 6d79  ..s......z.Dummy
-000001c0: 436c 6173 732e 5f5f 696e 6974 5f5f 4e29  Class.__init__N)
-000001d0: 04da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000001e0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000001f0: 616d 655f 5f72 0900 0000 7207 0000 0072  ame__r....r....r
-00000200: 0700 0000 7207 0000 0072 0800 0000 7204  ....r....r....r.
-00000210: 0000 0008 0000 0073 0400 0000 0800 0c01  .......s........
-00000220: 7204 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000230: 0000 0f00 0000 0900 0000 4300 0000 73dc  ..........C...s.
-00000240: 0100 0074 0083 008f e17d 0074 0164 0183  ...t.....}.t.d..
-00000250: 017d 017c 007d 0264 027d 0364 037d 0474  .}.|.}.d.}.d.}.t
-00000260: 027c 017c 027c 037c 0464 048d 0401 0074  .|.|.|.|.d.....t
-00000270: 036a 04a0 057c 027c 037c 0417 00a1 027d  .j...|.|.|.....}
-00000280: 0574 036a 047d 067c 066a 067d 077c 077c  .t.j.}.|.j.}.|.|
-00000290: 0583 017d 087c 0873 6564 0564 0674 07a0  ...}.|.sed.d.t..
-000002a0: 08a1 0076 0073 3774 09a0 0a74 03a1 0172  ...v.s7t...t...r
-000002b0: 3c74 09a0 0b74 03a1 016e 0164 0674 09a0  <t...t...n.d.t..
-000002c0: 0b7c 06a1 0174 09a0 0b7c 07a1 0164 0774  .|...t...|...d.t
-000002d0: 07a0 08a1 0076 0073 5074 09a0 0a7c 05a1  .....v.sPt...|..
-000002e0: 0172 5574 09a0 0b7c 05a1 016e 0164 0774  .rUt...|...n.d.t
-000002f0: 09a0 0b7c 08a1 0164 089c 0516 007d 0974  ...|...d.....}.t
-00000300: 0c74 09a0 0d7c 09a1 0183 0182 0164 0004  .t...|.......d..
-00000310: 007d 0604 007d 077d 0874 0e7c 0564 0983  .}...}.}.t.|.d..
-00000320: 028f 0d7d 0a74 0fa0 107c 0aa1 017d 0b57  ...}.t...|...}.W
-00000330: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
-00000340: 8077 0101 0001 0001 0059 0001 007c 0b6a  .w.......Y...|.j
-00000350: 117d 067c 016a 117d 0c7c 067c 0c6b 027d  .}.|.j.}.|.|.k.}
-00000360: 077c 0773 d674 09a0 1264 0a7c 0766 0164  .|.s.t...d.|.f.d
-00000370: 0b7c 067c 0c66 02a1 0464 0c74 07a0 08a1  .|.|.f...d.t....
-00000380: 0076 0073 a674 09a0 0a7c 0ba1 0172 ab74  .v.s.t...|...r.t
-00000390: 09a0 0b7c 0ba1 016e 0164 0c74 09a0 0b7c  ...|...n.d.t...|
-000003a0: 06a1 0164 0d74 07a0 08a1 0076 0073 bb74  ...d.t.....v.s.t
-000003b0: 09a0 0a7c 01a1 0172 c074 09a0 0b7c 01a1  ...|...r.t...|..
-000003c0: 016e 0164 0d74 09a0 0b7c 0ca1 0164 0e9c  .n.d.t...|...d..
-000003d0: 0416 007d 0d64 0f64 107c 0d69 0116 007d  ...}.d.d.|.i...}
-000003e0: 0e74 0c74 09a0 0d7c 0ea1 0183 0182 0164  .t.t...|.......d
-000003f0: 0004 007d 0604 007d 077d 0c57 0064 0004  ...}...}.}.W.d..
-00000400: 0004 0083 0301 0064 0053 0031 0073 e777  .......d.S.1.s.w
-00000410: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00000420: 114e da09 7465 7374 5f64 6174 61da 0d74  .N..test_data..t
-00000430: 6573 745f 696e 7374 616e 6365 7a04 2e64  est_instancez..d
-00000440: 6174 2903 da09 6669 6c65 5f70 6174 68da  at)...file_path.
-00000450: 0966 696c 655f 6e61 6d65 da09 6669 6c65  .file_name..file
-00000460: 5f74 7970 657a 6261 7373 6572 7420 2528  _typezbassert %(
-00000470: 7079 3729 730a 7b25 2870 7937 2973 203d  py7)s.{%(py7)s =
-00000480: 2025 2870 7934 2973 0a7b 2528 7079 3429   %(py4)s.{%(py4)
-00000490: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
-000004a0: 7932 2973 203d 2025 2870 7930 2973 2e70  y2)s = %(py0)s.p
-000004b0: 6174 680a 7d2e 6578 6973 7473 0a7d 2825  ath.}.exists.}(%
-000004c0: 2870 7935 2973 290a 7dda 026f 73da 1265  (py5)s).}..os..e
-000004d0: 7870 6563 7465 645f 6669 6c65 5f70 6174  xpected_file_pat
-000004e0: 6829 05da 0370 7930 da03 7079 32da 0370  h)...py0..py2..p
-000004f0: 7934 da03 7079 35da 0370 7937 da02 7262  y4..py5..py7..rb
-00000500: 2901 fa02 3d3d 2901 7a46 2528 7079 3229  )...==).zF%(py2)
-00000510: 730a 7b25 2870 7932 2973 203d 2025 2870  s.{%(py2)s = %(p
-00000520: 7930 2973 2e64 6174 610a 7d20 3d3d 2025  y0)s.data.} == %
-00000530: 2870 7936 2973 0a7b 2528 7079 3629 7320  (py6)s.{%(py6)s 
-00000540: 3d20 2528 7079 3429 732e 6461 7461 0a7d  = %(py4)s.data.}
-00000550: da0f 6c6f 6164 6564 5f69 6e73 7461 6e63  ..loaded_instanc
-00000560: 65da 0e64 756d 6d79 5f69 6e73 7461 6e63  e..dummy_instanc
-00000570: 6529 0472 1400 0000 7215 0000 0072 1600  e).r....r....r..
-00000580: 0000 da03 7079 367a 0e61 7373 6572 7420  ....py6z.assert 
-00000590: 2528 7079 3829 73da 0370 7938 2913 7202  %(py8)s..py8).r.
-000005a0: 0000 0072 0400 0000 7203 0000 0072 1200  ...r....r....r..
-000005b0: 0000 da04 7061 7468 da04 6a6f 696e da06  ....path..join..
-000005c0: 6578 6973 7473 da0c 4070 795f 6275 696c  exists..@py_buil
-000005d0: 7469 6e73 da06 6c6f 6361 6c73 da0a 4070  tins..locals..@p
-000005e0: 7974 6573 745f 6172 da18 5f73 686f 756c  ytest_ar.._shoul
-000005f0: 645f 7265 7072 5f67 6c6f 6261 6c5f 6e61  d_repr_global_na
-00000600: 6d65 da09 5f73 6166 6572 6570 72da 0e41  me.._saferepr..A
-00000610: 7373 6572 7469 6f6e 4572 726f 72da 135f  ssertionError.._
-00000620: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
-00000630: 6f6e da04 6f70 656e da06 7069 636b 6c65  on..open..pickle
-00000640: da04 6c6f 6164 7205 0000 00da 115f 6361  ..loadr......_ca
-00000650: 6c6c 5f72 6570 7263 6f6d 7061 7265 290f  ll_reprcompare).
-00000660: da08 7465 6d70 5f64 6972 721c 0000 0072  ..temp_dirr....r
-00000670: 0f00 0000 7210 0000 0072 1100 0000 7213  ....r....r....r.
-00000680: 0000 00da 0b40 7079 5f61 7373 6572 7431  .....@py_assert1
-00000690: da0b 4070 795f 6173 7365 7274 33da 0b40  ..@py_assert3..@
-000006a0: 7079 5f61 7373 6572 7436 da0b 4070 795f  py_assert6..@py_
-000006b0: 666f 726d 6174 38da 0466 696c 6572 1b00  format8..filer..
-000006c0: 0000 da0b 4070 795f 6173 7365 7274 35da  ....@py_assert5.
-000006d0: 0b40 7079 5f66 6f72 6d61 7437 da0b 4070  .@py_format7..@p
-000006e0: 795f 666f 726d 6174 3972 0700 0000 7207  y_format9r....r.
-000006f0: 0000 0072 0800 0000 da17 7465 7374 5f73  ...r......test_s
-00000700: 6176 655f 746f 5f70 726f 6475 6374 696f  ave_to_productio
-00000710: 6e0d 0000 0073 1a00 0000 0802 0802 0403  n....s..........
-00000720: 0401 0401 1003 1203 9803 0c03 0c01 1cff  ................
-00000730: b004 22e9 7236 0000 0029 0fda 0862 7569  ..".r6...)...bui
-00000740: 6c74 696e 7372 2200 0000 da19 5f70 7974  ltinsr"....._pyt
-00000750: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
-00000760: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
-00000770: da07 7265 7772 6974 6572 2400 0000 7212  ..rewriter$...r.
-00000780: 0000 00da 0670 7974 6573 7472 2a00 0000  .....pytestr*...
-00000790: da08 7465 6d70 6669 6c65 7202 0000 00da  ..tempfiler.....
-000007a0: 2462 6c75 6563 6173 742e 6765 6e65 7261  $bluecast.genera
-000007b0: 6c5f 7574 696c 732e 6765 6e65 7261 6c5f  l_utils.general_
-000007c0: 7574 696c 7372 0300 0000 7204 0000 0072  utilsr....r....r
-000007d0: 3600 0000 7207 0000 0072 0700 0000 7207  6...r....r....r.
-000007e0: 0000 0072 0800 0000 da08 3c6d 6f64 756c  ...r......<modul
-000007f0: 653e 0100 0000 730e 0000 0022 0008 0108  e>....s...."....
-00000800: 010c 010c 010e 030c 05                   .........
+00000050: 6400 6401 6c07 5a07 6400 6402 6c08 6d09  d.d.l.Z.d.d.l.m.
+00000060: 5a09 0100 4700 6403 6404 8400 6404 8302  Z...G.d.d...d...
+00000070: 5a0a 6405 6406 8400 5a0b 6401 5300 2907  Z.d.d...Z.d.S.).
+00000080: e900 0000 004e 2901 da12 7361 7665 5f74  .....N)...save_t
+00000090: 6f5f 7072 6f64 7563 7469 6f6e 6300 0000  o_productionc...
+000000a0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+000000b0: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
+000000c0: 5a02 6401 6402 8400 5a03 6403 5300 2904  Z.d.d...Z.d.S.).
+000000d0: da0a 4475 6d6d 7943 6c61 7373 6302 0000  ..DummyClassc...
+000000e0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+000000f0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000100: 6400 5300 2901 4e29 01da 0464 6174 6129  d.S.).N)...data)
+00000110: 02da 0473 656c 6672 0400 0000 a900 7206  ...selfr......r.
+00000120: 0000 00fa 4c2f 686f 6d65 2f74 686f 6d61  ....L/home/thoma
+00000130: 732f 4964 6561 5072 6f6a 6563 7473 2f42  s/IdeaProjects/B
+00000140: 6c75 6543 6173 742f 626c 7565 6361 7374  lueCast/bluecast
+00000150: 2f74 6573 7473 2f74 6573 745f 7361 7665  /tests/test_save
+00000160: 5f74 6f5f 7072 6f64 7563 7469 6f6e 2e70  _to_production.p
+00000170: 79da 085f 5f69 6e69 745f 5f08 0000 0073  y..__init__....s
+00000180: 0200 0000 0a01 7a13 4475 6d6d 7943 6c61  ......z.DummyCla
+00000190: 7373 2e5f 5f69 6e69 745f 5f4e 2904 da08  ss.__init__N)...
+000001a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000001b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000001c0: 5f5f 7208 0000 0072 0600 0000 7206 0000  __r....r....r...
+000001d0: 0072 0600 0000 7207 0000 0072 0300 0000  .r....r....r....
+000001e0: 0700 0000 7304 0000 0008 000c 0172 0300  ....s........r..
+000001f0: 0000 6300 0000 0000 0000 0000 0000 000d  ..c.............
+00000200: 0000 0008 0000 0043 0000 0073 ac01 0000  .......C...s....
+00000210: 7400 6401 8301 7d00 6402 7d01 6403 7d02  t.d...}.d.}.d.}.
+00000220: 7401 7c00 7c01 7c02 6404 8d03 0100 7402  t.|.|.|.d.....t.
+00000230: 6a03 a004 7c01 7c02 1700 a101 7d03 7402  j...|.|.....}.t.
+00000240: 6a03 7d04 7c04 6a05 7d05 7c05 7c03 8301  j.}.|.j.}.|.|...
+00000250: 7d06 7c06 735d 6405 6406 7406 a007 a100  }.|.s]d.d.t.....
+00000260: 7600 732f 7408 a009 7402 a101 7234 7408  v.s/t...t...r4t.
+00000270: a00a 7402 a101 6e01 6406 7408 a00a 7c04  ..t...n.d.t...|.
+00000280: a101 7408 a00a 7c05 a101 6407 7406 a007  ..t...|...d.t...
+00000290: a100 7600 7348 7408 a009 7c03 a101 724d  ..v.sHt...|...rM
+000002a0: 7408 a00a 7c03 a101 6e01 6407 7408 a00a  t...|...n.d.t...
+000002b0: 7c06 a101 6408 9c05 1600 7d07 740b 7408  |...d.....}.t.t.
+000002c0: a00c 7c07 a101 8301 8201 6400 0400 7d04  ..|.......d...}.
+000002d0: 0400 7d05 7d06 740d 7c03 6409 8302 8f0d  ..}.}.t.|.d.....
+000002e0: 7d08 740e a00f 7c08 a101 7d09 5700 6400  }.t...|...}.W.d.
+000002f0: 0400 0400 8303 0100 6e08 3100 7378 7701  ........n.1.sxw.
+00000300: 0100 0100 0100 5900 0100 7c09 6a10 7d04  ......Y...|.j.}.
+00000310: 7c00 6a10 7d0a 7c04 7c0a 6b02 7d05 7c05  |.j.}.|.|.k.}.|.
+00000320: 73ce 7408 a011 640a 7c05 6601 640b 7c04  s.t...d.|.f.d.|.
+00000330: 7c0a 6602 a104 640c 7406 a007 a100 7600  |.f...d.t.....v.
+00000340: 739e 7408 a009 7c09 a101 72a3 7408 a00a  s.t...|...r.t...
+00000350: 7c09 a101 6e01 640c 7408 a00a 7c04 a101  |...n.d.t...|...
+00000360: 640d 7406 a007 a100 7600 73b3 7408 a009  d.t.....v.s.t...
+00000370: 7c00 a101 72b8 7408 a00a 7c00 a101 6e01  |...r.t...|...n.
+00000380: 640d 7408 a00a 7c0a a101 640e 9c04 1600  d.t...|...d.....
+00000390: 7d0b 640f 6410 7c0b 6901 1600 7d0c 740b  }.d.d.|.i...}.t.
+000003a0: 7408 a00c 7c0c a101 8301 8201 6400 0400  t...|.......d...
+000003b0: 7d04 0400 7d05 7d0a 6400 5300 2911 4eda  }...}.}.d.S.).N.
+000003c0: 0974 6573 745f 6461 7461 da0d 7465 7374  .test_data..test
+000003d0: 5f69 6e73 7461 6e63 657a 042e 6461 7429  _instancez..dat)
+000003e0: 02da 0966 696c 655f 6e61 6d65 da09 6669  ...file_name..fi
+000003f0: 6c65 5f74 7970 657a 6261 7373 6572 7420  le_typezbassert 
+00000400: 2528 7079 3729 730a 7b25 2870 7937 2973  %(py7)s.{%(py7)s
+00000410: 203d 2025 2870 7934 2973 0a7b 2528 7079   = %(py4)s.{%(py
+00000420: 3429 7320 3d20 2528 7079 3229 730a 7b25  4)s = %(py2)s.{%
+00000430: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
+00000440: 2e70 6174 680a 7d2e 6578 6973 7473 0a7d  .path.}.exists.}
+00000450: 2825 2870 7935 2973 290a 7dda 026f 73da  (%(py5)s).}..os.
+00000460: 1265 7870 6563 7465 645f 6669 6c65 5f70  .expected_file_p
+00000470: 6174 6829 05da 0370 7930 da03 7079 32da  ath)...py0..py2.
+00000480: 0370 7934 da03 7079 35da 0370 7937 da02  .py4..py5..py7..
+00000490: 7262 2901 fa02 3d3d 2901 7a46 2528 7079  rb)...==).zF%(py
+000004a0: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
+000004b0: 2870 7930 2973 2e64 6174 610a 7d20 3d3d  (py0)s.data.} ==
+000004c0: 2025 2870 7936 2973 0a7b 2528 7079 3629   %(py6)s.{%(py6)
+000004d0: 7320 3d20 2528 7079 3429 732e 6461 7461  s = %(py4)s.data
+000004e0: 0a7d da0f 6c6f 6164 6564 5f69 6e73 7461  .}..loaded_insta
+000004f0: 6e63 65da 0e64 756d 6d79 5f69 6e73 7461  nce..dummy_insta
+00000500: 6e63 6529 0472 1200 0000 7213 0000 0072  nce).r....r....r
+00000510: 1400 0000 da03 7079 367a 0e61 7373 6572  ......py6z.asser
+00000520: 7420 2528 7079 3829 73da 0370 7938 2912  t %(py8)s..py8).
+00000530: 7203 0000 0072 0200 0000 7210 0000 00da  r....r....r.....
+00000540: 0470 6174 68da 046a 6f69 6eda 0665 7869  .path..join..exi
+00000550: 7374 73da 0c40 7079 5f62 7569 6c74 696e  sts..@py_builtin
+00000560: 73da 066c 6f63 616c 73da 0a40 7079 7465  s..locals..@pyte
+00000570: 7374 5f61 72da 185f 7368 6f75 6c64 5f72  st_ar.._should_r
+00000580: 6570 725f 676c 6f62 616c 5f6e 616d 65da  epr_global_name.
+00000590: 095f 7361 6665 7265 7072 da0e 4173 7365  ._saferepr..Asse
+000005a0: 7274 696f 6e45 7272 6f72 da13 5f66 6f72  rtionError.._for
+000005b0: 6d61 745f 6578 706c 616e 6174 696f 6eda  mat_explanation.
+000005c0: 046f 7065 6eda 0670 6963 6b6c 65da 046c  .open..pickle..l
+000005d0: 6f61 6472 0400 0000 da11 5f63 616c 6c5f  oadr......_call_
+000005e0: 7265 7072 636f 6d70 6172 6529 0d72 1a00  reprcompare).r..
+000005f0: 0000 720e 0000 0072 0f00 0000 7211 0000  ..r....r....r...
+00000600: 00da 0b40 7079 5f61 7373 6572 7431 da0b  ...@py_assert1..
+00000610: 4070 795f 6173 7365 7274 33da 0b40 7079  @py_assert3..@py
+00000620: 5f61 7373 6572 7436 da0b 4070 795f 666f  _assert6..@py_fo
+00000630: 726d 6174 38da 0466 696c 6572 1900 0000  rmat8..filer....
+00000640: da0b 4070 795f 6173 7365 7274 35da 0b40  ..@py_assert5..@
+00000650: 7079 5f66 6f72 6d61 7437 da0b 4070 795f  py_format7..@py_
+00000660: 666f 726d 6174 3972 0600 0000 7206 0000  format9r....r...
+00000670: 0072 0700 0000 da17 7465 7374 5f73 6176  .r......test_sav
+00000680: 655f 746f 5f70 726f 6475 6374 696f 6e0c  e_to_production.
+00000690: 0000 0073 1c00 0000 0803 0402 0401 0202  ...s............
+000006a0: 0201 0201 0201 06fd 1006 9802 0c02 0c01  ................
+000006b0: 1cff b203 7233 0000 0029 0cda 0862 7569  ....r3...)...bui
+000006c0: 6c74 696e 7372 2000 0000 da19 5f70 7974  ltinsr ....._pyt
+000006d0: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
+000006e0: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
+000006f0: da07 7265 7772 6974 6572 2200 0000 7210  ..rewriter"...r.
+00000700: 0000 0072 2800 0000 da24 626c 7565 6361  ...r(....$blueca
+00000710: 7374 2e67 656e 6572 616c 5f75 7469 6c73  st.general_utils
+00000720: 2e67 656e 6572 616c 5f75 7469 6c73 7202  .general_utilsr.
+00000730: 0000 0072 0300 0000 7233 0000 0072 0600  ...r....r3...r..
+00000740: 0000 7206 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00000750: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000760: 0a00 0000 2200 0801 0c02 0e03 0c05       ....".........
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 18:43:33 2023 UTC, .py size: 2080 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5521 8264 2008 0000  o.......U!.d ...
+00000000: 6f0d 0d0a 0000 0000 ca79 8164 2008 0000  o........y.d ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6401 6c08 5a08 6400 6402 6c09 6d0a  d.d.l.Z.d.d.l.m.
 00000060: 5a0a 0100 6403 6404 8400 5a0b 6405 6406  Z...d.d...Z.d.d.
 00000070: 8400 5a0c 6407 6408 8400 5a0d 6401 5300  ..Z.d.d...Z.d.S.
@@ -63,70 +63,70 @@
 000003e0: 0874 7261 696e 5f64 66da 0974 6573 745f  .train_df..test_
 000003f0: 6461 7461 da07 7465 7374 5f64 6672 1800  data..test_dfr..
 00000400: 0000 da0b 4070 795f 6173 7365 7274 32da  ....@py_assert2.
 00000410: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
 00000420: 795f 6173 7365 7274 38da 0b40 7079 5f61  y_assert8..@py_a
 00000430: 7373 6572 7436 da0c 4070 795f 666f 726d  ssert6..@py_form
 00000440: 6174 3130 da0c 4070 795f 666f 726d 6174  at10..@py_format
-00000450: 3132 a900 7239 0000 00fa 502f 5573 6572  12..r9....P/User
-00000460: 732f 7468 6f6d 6173 6d65 6973 736e 6572  s/thomasmeissner
-00000470: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
-00000480: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
-00000490: 7465 7374 732f 7465 7374 5f73 6368 656d  tests/test_schem
-000004a0: 615f 6368 6563 6b73 2e70 79da 1a74 6573  a_checks.py..tes
-000004b0: 745f 7472 616e 7366 6f72 6d5f 7361 6d65  t_transform_same
-000004c0: 5f73 6368 656d 6107 0000 0073 1000 0000  _schema....s....
-000004d0: 0602 1202 0a01 1202 0a01 0a02 0a02 e802  ................
-000004e0: 723b 0000 0063 0000 0000 0000 0000 0000  r;...c..........
-000004f0: 0000 0500 0000 0800 0000 4300 0000 737c  ..........C...s|
-00000500: 0000 0074 0083 007d 0067 0064 01a2 0167  ...t...}.g.d...g
-00000510: 0064 02a2 0164 039c 027d 0174 01a0 027c  .d...d...}.t...|
-00000520: 01a1 017d 0264 0467 0064 05a2 0169 017d  ...}.d.g.d...i.}
-00000530: 0374 01a0 027c 03a1 017d 047c 00a0 037c  .t...|...}.|...|
-00000540: 02a1 0101 0074 04a0 0574 06a1 018f 0e01  .....t...t......
-00000550: 007c 00a0 077c 04a1 0101 0057 0064 0004  .|...|.....W.d..
-00000560: 0004 0083 0301 0064 0053 0031 0073 3777  .......d.S.1.s7w
-00000570: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00000580: 064e 7203 0000 0072 0700 0000 720b 0000  .Nr....r....r...
-00000590: 0072 0c00 0000 720e 0000 00a9 0872 0200  .r....r......r..
-000005a0: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
-000005b0: 00da 0670 7974 6573 74da 0672 6169 7365  ...pytest..raise
-000005c0: 73da 0a56 616c 7565 4572 726f 7272 2400  s..ValueErrorr$.
-000005d0: 0000 a905 7219 0000 0072 2f00 0000 7230  ....r....r/...r0
-000005e0: 0000 0072 3100 0000 7232 0000 0072 3900  ...r1...r2...r9.
-000005f0: 0000 7239 0000 0072 3a00 0000 da1e 7465  ..r9...r:.....te
-00000600: 7374 5f74 7261 6e73 666f 726d 5f6d 6973  st_transform_mis
-00000610: 7369 6e67 5f63 6f6c 756d 6e73 1800 0000  sing_columns....
-00000620: 7312 0000 0006 0212 020a 010c 020a 010a  s...............
-00000630: 020c 020c 0122 ff72 4100 0000 6300 0000  .....".rA...c...
-00000640: 0000 0000 0000 0000 0005 0000 0008 0000  ................
-00000650: 0043 0000 0073 8800 0000 7400 8300 7d00  .C...s....t...}.
-00000660: 6700 6401 a201 6700 6402 a201 6403 9c02  g.d...g.d...d...
-00000670: 7d01 7401 a002 7c01 a101 7d02 6700 6404  }.t...|...}.g.d.
-00000680: a201 6700 6405 a201 6700 6406 a201 6407  ..g.d...g.d...d.
-00000690: 9c03 7d03 7401 a002 7c03 a101 7d04 7c00  ..}.t...|...}.|.
-000006a0: a003 7c02 a101 0100 7404 a005 7406 a101  ..|.....t...t...
-000006b0: 8f0e 0100 7c00 a007 7c04 a101 0100 5700  ....|...|.....W.
-000006c0: 6400 0400 0400 8303 0100 6400 5300 3100  d.........d.S.1.
-000006d0: 733d 7701 0100 0100 0100 5900 0100 6400  s=w.......Y...d.
-000006e0: 5300 2908 4e72 0300 0000 7207 0000 0072  S.).Nr....r....r
-000006f0: 0b00 0000 720e 0000 0072 1200 0000 2903  ....r....r....).
-00000700: e907 0000 00e9 0800 0000 e909 0000 0029  ...............)
-00000710: 0372 0c00 0000 720d 0000 005a 0463 6f6c  .r....r....Z.col
-00000720: 3372 3c00 0000 7240 0000 0072 3900 0000  3r<...r@...r9...
-00000730: 7239 0000 0072 3a00 0000 da1c 7465 7374  r9...r:.....test
-00000740: 5f74 7261 6e73 666f 726d 5f65 7874 7261  _transform_extra
-00000750: 5f63 6f6c 756d 6e73 2800 0000 7312 0000  _columns(...s...
-00000760: 0006 0212 020a 0118 020a 010a 020c 020c  ................
-00000770: 0122 ff72 4500 0000 290e da08 6275 696c  .".rE...)...buil
-00000780: 7469 6e73 7229 0000 00da 195f 7079 7465  tinsr)....._pyte
-00000790: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
-000007a0: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
-000007b0: 0772 6577 7269 7465 7227 0000 00da 0670  .rewriter'.....p
-000007c0: 616e 6461 7372 2100 0000 723d 0000 00da  andasr!...r=....
-000007d0: 2462 6c75 6563 6173 742e 7072 6570 726f  $bluecast.prepro
-000007e0: 6365 7373 696e 672e 7363 6865 6d61 5f63  cessing.schema_c
-000007f0: 6865 636b 7372 0200 0000 723b 0000 0072  hecksr....r;...r
-00000800: 4100 0000 7245 0000 0072 3900 0000 7239  A...rE...r9...r9
-00000810: 0000 0072 3900 0000 723a 0000 00da 083c  ...r9...r:.....<
-00000820: 6d6f 6475 6c65 3e01 0000 0073 0c00 0000  module>....s....
-00000830: 2200 0801 0c02 0803 0811 0c10            "...........
+00000450: 3132 a900 7239 0000 00fa 472f 686f 6d65  12..r9....G/home
+00000460: 2f74 686f 6d61 732f 4964 6561 5072 6f6a  /thomas/IdeaProj
+00000470: 6563 7473 2f42 6c75 6543 6173 742f 626c  ects/BlueCast/bl
+00000480: 7565 6361 7374 2f74 6573 7473 2f74 6573  uecast/tests/tes
+00000490: 745f 7363 6865 6d61 5f63 6865 636b 732e  t_schema_checks.
+000004a0: 7079 da1a 7465 7374 5f74 7261 6e73 666f  py..test_transfo
+000004b0: 726d 5f73 616d 655f 7363 6865 6d61 0700  rm_same_schema..
+000004c0: 0000 7310 0000 0006 0212 020a 0112 020a  ..s.............
+000004d0: 010a 020a 02e8 0272 3b00 0000 6300 0000  .......r;...c...
+000004e0: 0000 0000 0000 0000 0005 0000 0008 0000  ................
+000004f0: 0043 0000 0073 7c00 0000 7400 8300 7d00  .C...s|...t...}.
+00000500: 6700 6401 a201 6700 6402 a201 6403 9c02  g.d...g.d...d...
+00000510: 7d01 7401 a002 7c01 a101 7d02 6404 6700  }.t...|...}.d.g.
+00000520: 6405 a201 6901 7d03 7401 a002 7c03 a101  d...i.}.t...|...
+00000530: 7d04 7c00 a003 7c02 a101 0100 7404 a005  }.|...|.....t...
+00000540: 7406 a101 8f0e 0100 7c00 a007 7c04 a101  t.......|...|...
+00000550: 0100 5700 6400 0400 0400 8303 0100 6400  ..W.d.........d.
+00000560: 5300 3100 7337 7701 0100 0100 0100 5900  S.1.s7w.......Y.
+00000570: 0100 6400 5300 2906 4e72 0300 0000 7207  ..d.S.).Nr....r.
+00000580: 0000 0072 0b00 0000 720c 0000 0072 0e00  ...r....r....r..
+00000590: 0000 a908 7202 0000 0072 2100 0000 7222  ....r....r!...r"
+000005a0: 0000 0072 2300 0000 da06 7079 7465 7374  ...r#.....pytest
+000005b0: da06 7261 6973 6573 da0a 5661 6c75 6545  ..raises..ValueE
+000005c0: 7272 6f72 7224 0000 00a9 0572 1900 0000  rrorr$.....r....
+000005d0: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
+000005e0: 3200 0000 7239 0000 0072 3900 0000 723a  2...r9...r9...r:
+000005f0: 0000 00da 1e74 6573 745f 7472 616e 7366  .....test_transf
+00000600: 6f72 6d5f 6d69 7373 696e 675f 636f 6c75  orm_missing_colu
+00000610: 6d6e 7318 0000 0073 1200 0000 0602 1202  mns....s........
+00000620: 0a01 0c02 0a01 0a02 0c02 0c01 22ff 7241  ............".rA
+00000630: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000640: 0500 0000 0800 0000 4300 0000 7388 0000  ........C...s...
+00000650: 0074 0083 007d 0067 0064 01a2 0167 0064  .t...}.g.d...g.d
+00000660: 02a2 0164 039c 027d 0174 01a0 027c 01a1  ...d...}.t...|..
+00000670: 017d 0267 0064 04a2 0167 0064 05a2 0167  .}.g.d...g.d...g
+00000680: 0064 06a2 0164 079c 037d 0374 01a0 027c  .d...d...}.t...|
+00000690: 03a1 017d 047c 00a0 037c 02a1 0101 0074  ...}.|...|.....t
+000006a0: 04a0 0574 06a1 018f 0e01 007c 00a0 077c  ...t.......|...|
+000006b0: 04a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+000006c0: 0064 0053 0031 0073 3d77 0101 0001 0001  .d.S.1.s=w......
+000006d0: 0059 0001 0064 0053 0029 084e 7203 0000  .Y...d.S.).Nr...
+000006e0: 0072 0700 0000 720b 0000 0072 0e00 0000  .r....r....r....
+000006f0: 7212 0000 0029 03e9 0700 0000 e908 0000  r....)..........
+00000700: 00e9 0900 0000 2903 720c 0000 0072 0d00  ......).r....r..
+00000710: 0000 5a04 636f 6c33 723c 0000 0072 4000  ..Z.col3r<...r@.
+00000720: 0000 7239 0000 0072 3900 0000 723a 0000  ..r9...r9...r:..
+00000730: 00da 1c74 6573 745f 7472 616e 7366 6f72  ...test_transfor
+00000740: 6d5f 6578 7472 615f 636f 6c75 6d6e 7328  m_extra_columns(
+00000750: 0000 0073 1200 0000 0602 1202 0a01 1802  ...s............
+00000760: 0a01 0a02 0c02 0c01 22ff 7245 0000 0029  ........".rE...)
+00000770: 0eda 0862 7569 6c74 696e 7372 2900 0000  ...builtinsr)...
+00000780: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
+00000790: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
+000007a0: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
+000007b0: 2700 0000 da06 7061 6e64 6173 7221 0000  '.....pandasr!..
+000007c0: 0072 3d00 0000 da24 626c 7565 6361 7374  .r=....$bluecast
+000007d0: 2e70 7265 7072 6f63 6573 7369 6e67 2e73  .preprocessing.s
+000007e0: 6368 656d 615f 6368 6563 6b73 7202 0000  chema_checksr...
+000007f0: 0072 3b00 0000 7241 0000 0072 4500 0000  .r;...rA...rE...
+00000800: 7239 0000 0072 3900 0000 7239 0000 0072  r9...r9...r9...r
+00000810: 3a00 0000 da08 3c6d 6f64 756c 653e 0100  :.....<module>..
+00000820: 0000 730c 0000 0022 0008 010c 0208 0308  ..s...."........
+00000830: 110c 10                                  ...
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 04:56:12 2023 UTC, .py size: 1337 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec0d 8064 3905 0000  o..........d9...
+00000000: 6f0d 0d0a 0000 0000 ab09 8064 3905 0000  o..........d9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6401 6c08 5a08 6400 6402 6c09 6d0a  d.d.l.Z.d.d.l.m.
 00000060: 5a0a 0100 6508 6a0b 6403 6404 8400 8301  Z...e.j.d.d.....
 00000070: 5a0c 6405 6406 8400 5a0d 6401 5300 2907  Z.d.d...Z.d.S.).
@@ -17,102 +17,102 @@
 00000100: 06da 0158 da01 59da 015a 7206 0000 0072  ...X..Y..Zr....r
 00000110: 0700 0000 7208 0000 0029 0672 0100 0000  ....r....).r....
 00000120: e901 0000 0072 0100 0000 7209 0000 0072  .....r....r....r
 00000130: 0100 0000 7209 0000 0029 03da 0463 6f6c  ....r....)...col
 00000140: 31da 0463 6f6c 32da 0674 6172 6765 7429  1..col2..target)
 00000150: 02da 0270 64da 0944 6174 6146 7261 6d65  ...pd..DataFrame
 00000160: 2901 da04 6461 7461 a900 7210 0000 00fa  )...data..r.....
-00000170: 592f 5573 6572 732f 7468 6f6d 6173 6d65  Y/Users/thomasme
-00000180: 6973 736e 6572 2f49 6465 6150 726f 6a65  issner/IdeaProje
-00000190: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
-000001a0: 6563 6173 742f 7465 7374 732f 7465 7374  ecast/tests/test
-000001b0: 5f74 6172 6765 745f 656e 636f 6469 6e67  _target_encoding
-000001c0: 5f62 696e 6172 792e 7079 da0b 7361 6d70  _binary.py..samp
-000001d0: 6c65 5f64 6174 6107 0000 0073 0e00 0000  le_data....s....
-000001e0: 0403 0602 0601 0601 04fd 04ff 0407 7212  ..............r.
-000001f0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000200: 0b00 0000 0a00 0000 4300 0000 7372 0100  ........C...sr..
-00000210: 0074 0064 0164 0267 0264 038d 017d 017c  .t.d.d.g.d...}.|
-00000220: 01a0 017c 0064 0164 0267 0219 007c 0064  ...|.d.d.g...|.d
-00000230: 0419 00a1 0201 007c 01a0 027c 0064 0164  .......|...|.d.d
-00000240: 0267 0219 00a1 017d 0264 0164 0267 027d  .g.....}.d.d.g.}
-00000250: 037c 026a 037d 0474 047c 0483 017d 0574  .|.j.}.t.|...}.t
-00000260: 047c 0383 017d 067c 057c 066b 027d 077c  .|...}.|.|.k.}.|
-00000270: 0773 9c74 05a0 0664 057c 0766 0164 067c  .s.t...d.|.f.d.|
-00000280: 057c 0666 02a1 0464 0774 07a0 08a1 0076  .|.f...d.t.....v
-00000290: 0073 4674 05a0 0974 04a1 0172 4b74 05a0  .sFt...t...rKt..
-000002a0: 0a74 04a1 016e 0164 0764 0874 07a0 08a1  .t...n.d.d.t....
-000002b0: 0076 0073 5774 05a0 097c 02a1 0172 5c74  .v.sWt...|...r\t
-000002c0: 05a0 0a7c 02a1 016e 0164 0874 05a0 0a7c  ...|...n.d.t...|
-000002d0: 04a1 0174 05a0 0a7c 05a1 0164 0774 07a0  ...t...|...d.t..
-000002e0: 08a1 0076 0073 7074 05a0 0974 04a1 0172  ...v.spt...t...r
-000002f0: 7574 05a0 0a74 04a1 016e 0164 0764 0974  ut...t...n.d.d.t
-00000300: 07a0 08a1 0076 0073 8174 05a0 097c 03a1  .....v.s.t...|..
-00000310: 0172 8674 05a0 0a7c 03a1 016e 0164 0974  .r.t...|...n.d.t
-00000320: 05a0 0a7c 06a1 0164 0a9c 0716 007d 0864  ...|...d.....}.d
-00000330: 0b64 0c7c 0869 0116 007d 0974 0b74 05a0  .d.|.i...}.t.t..
-00000340: 0c7c 09a1 0183 0182 0164 0004 007d 0404  .|.......d...}..
-00000350: 007d 0504 007d 077d 0674 0da0 0e67 0064  .}...}.}.t...g.d
-00000360: 0da2 0167 0064 0da2 0164 0e9c 02a1 017d  ...g.d...d.....}
-00000370: 0a74 0d6a 0fa0 107c 027c 0aa1 0201 0064  .t.j...|.|.....d
-00000380: 0053 0029 0f4e 720a 0000 0072 0b00 0000  .S.).Nr....r....
-00000390: 2901 da0b 6361 745f 636f 6c75 6d6e 7372  )...cat_columnsr
-000003a0: 0c00 0000 2901 fa02 3d3d 2901 7a6d 2528  ....)...==).zm%(
-000003b0: 7079 3529 730a 7b25 2870 7935 2973 203d  py5)s.{%(py5)s =
-000003c0: 2025 2870 7930 2973 2825 2870 7933 2973   %(py0)s(%(py3)s
-000003d0: 0a7b 2528 7079 3329 7320 3d20 2528 7079  .{%(py3)s = %(py
-000003e0: 3129 732e 636f 6c75 6d6e 730a 7d29 0a7d  1)s.columns.}).}
-000003f0: 203d 3d20 2528 7079 3130 2973 0a7b 2528   == %(py10)s.{%(
-00000400: 7079 3130 2973 203d 2025 2870 7937 2973  py10)s = %(py7)s
-00000410: 2825 2870 7938 2973 290a 7dda 0373 6574  (%(py8)s).}..set
-00000420: da10 7472 616e 7366 6f72 6d65 645f 6461  ..transformed_da
-00000430: 7461 da10 6578 7065 6374 6564 5f63 6f6c  ta..expected_col
-00000440: 756d 6e73 2907 da03 7079 30da 0370 7931  umns)...py0..py1
-00000450: da03 7079 33da 0370 7935 da03 7079 37da  ..py3..py5..py7.
-00000460: 0370 7938 da04 7079 3130 7a0f 6173 7365  .py8..py10z.asse
-00000470: 7274 2025 2870 7931 3229 73da 0470 7931  rt %(py12)s..py1
-00000480: 3229 06e7 0000 0000 0000 e03f 7220 0000  2).........?r ..
-00000490: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
-000004a0: 7220 0000 0029 0272 0a00 0000 720b 0000  r ...).r....r...
-000004b0: 0029 1172 0200 0000 da1e 6669 745f 7461  .).r......fit_ta
-000004c0: 7267 6574 5f65 6e63 6f64 655f 6269 6e61  rget_encode_bina
-000004d0: 7279 5f63 6c61 7373 da24 7472 616e 7366  ry_class.$transf
-000004e0: 6f72 6d5f 7461 7267 6574 5f65 6e63 6f64  orm_target_encod
-000004f0: 655f 6269 6e61 7279 5f63 6c61 7373 da07  e_binary_class..
-00000500: 636f 6c75 6d6e 7372 1500 0000 da0a 4070  columnsr......@p
-00000510: 7974 6573 745f 6172 da11 5f63 616c 6c5f  ytest_ar.._call_
-00000520: 7265 7072 636f 6d70 6172 65da 0c40 7079  reprcompare..@py
-00000530: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
-00000540: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
-00000550: 676c 6f62 616c 5f6e 616d 65da 095f 7361  global_name.._sa
-00000560: 6665 7265 7072 da0e 4173 7365 7274 696f  ferepr..Assertio
-00000570: 6e45 7272 6f72 da13 5f66 6f72 6d61 745f  nError.._format_
-00000580: 6578 706c 616e 6174 696f 6e72 0d00 0000  explanationr....
-00000590: 720e 0000 00da 0774 6573 7469 6e67 da12  r......testing..
-000005a0: 6173 7365 7274 5f66 7261 6d65 5f65 7175  assert_frame_equ
-000005b0: 616c 290b 7212 0000 00da 0765 6e63 6f64  al).r......encod
-000005c0: 6572 7216 0000 0072 1700 0000 da0b 4070  err....r......@p
-000005d0: 795f 6173 7365 7274 32da 0b40 7079 5f61  y_assert2..@py_a
-000005e0: 7373 6572 7434 da0b 4070 795f 6173 7365  ssert4..@py_asse
-000005f0: 7274 39da 0b40 7079 5f61 7373 6572 7436  rt9..@py_assert6
-00000600: da0c 4070 795f 666f 726d 6174 3131 da0c  ..@py_format11..
-00000610: 4070 795f 666f 726d 6174 3133 da0f 6578  @py_format13..ex
-00000620: 7065 6374 6564 5f76 616c 7565 7372 1000  pected_valuesr..
-00000630: 0000 7210 0000 0072 1100 0000 da29 7465  ..r....r.....)te
-00000640: 7374 5f74 7261 6e73 666f 726d 5f74 6172  st_transform_tar
-00000650: 6765 745f 656e 636f 6465 5f62 696e 6172  get_encode_binar
-00000660: 795f 636c 6173 7314 0000 0073 1c00 0000  y_class....s....
-00000670: 0e02 0403 1001 04ff 0405 0a01 04ff 0805  ................
-00000680: fe01 0a00 0403 1001 04ff 1203 7236 0000  ............r6..
-00000690: 0029 0eda 0862 7569 6c74 696e 7372 2600  .)...builtinsr&.
-000006a0: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
-000006b0: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
-000006c0: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
-000006d0: 6572 2400 0000 da06 7061 6e64 6173 720d  er$.....pandasr.
-000006e0: 0000 00da 0670 7974 6573 74da 2662 6c75  .....pytest.&blu
-000006f0: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-00000700: 696e 672e 7461 7267 6574 5f65 6e63 6f64  ing.target_encod
-00000710: 696e 6772 0200 0000 da07 6669 7874 7572  ingr......fixtur
-00000720: 6572 1200 0000 7236 0000 0072 1000 0000  er....r6...r....
-00000730: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000740: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00000750: 0000 2200 0801 0c02 0403 0a01 0c0c       .."...........
+00000170: 502f 686f 6d65 2f74 686f 6d61 732f 4964  P/home/thomas/Id
+00000180: 6561 5072 6f6a 6563 7473 2f42 6c75 6543  eaProjects/BlueC
+00000190: 6173 742f 626c 7565 6361 7374 2f74 6573  ast/bluecast/tes
+000001a0: 7473 2f74 6573 745f 7461 7267 6574 5f65  ts/test_target_e
+000001b0: 6e63 6f64 696e 675f 6269 6e61 7279 2e70  ncoding_binary.p
+000001c0: 79da 0b73 616d 706c 655f 6461 7461 0700  y..sample_data..
+000001d0: 0000 730e 0000 0004 0306 0206 0106 0104  ..s.............
+000001e0: fd04 ff04 0772 1200 0000 6301 0000 0000  .....r....c.....
+000001f0: 0000 0000 0000 000b 0000 000a 0000 0043  ...............C
+00000200: 0000 0073 7201 0000 7400 6401 6402 6702  ...sr...t.d.d.g.
+00000210: 6403 8d01 7d01 7c01 a001 7c00 6401 6402  d...}.|...|.d.d.
+00000220: 6702 1900 7c00 6404 1900 a102 0100 7c01  g...|.d.......|.
+00000230: a002 7c00 6401 6402 6702 1900 a101 7d02  ..|.d.d.g.....}.
+00000240: 6401 6402 6702 7d03 7c02 6a03 7d04 7404  d.d.g.}.|.j.}.t.
+00000250: 7c04 8301 7d05 7404 7c03 8301 7d06 7c05  |...}.t.|...}.|.
+00000260: 7c06 6b02 7d07 7c07 739c 7405 a006 6405  |.k.}.|.s.t...d.
+00000270: 7c07 6601 6406 7c05 7c06 6602 a104 6407  |.f.d.|.|.f...d.
+00000280: 7407 a008 a100 7600 7346 7405 a009 7404  t.....v.sFt...t.
+00000290: a101 724b 7405 a00a 7404 a101 6e01 6407  ..rKt...t...n.d.
+000002a0: 6408 7407 a008 a100 7600 7357 7405 a009  d.t.....v.sWt...
+000002b0: 7c02 a101 725c 7405 a00a 7c02 a101 6e01  |...r\t...|...n.
+000002c0: 6408 7405 a00a 7c04 a101 7405 a00a 7c05  d.t...|...t...|.
+000002d0: a101 6407 7407 a008 a100 7600 7370 7405  ..d.t.....v.spt.
+000002e0: a009 7404 a101 7275 7405 a00a 7404 a101  ..t...rut...t...
+000002f0: 6e01 6407 6409 7407 a008 a100 7600 7381  n.d.d.t.....v.s.
+00000300: 7405 a009 7c03 a101 7286 7405 a00a 7c03  t...|...r.t...|.
+00000310: a101 6e01 6409 7405 a00a 7c06 a101 640a  ..n.d.t...|...d.
+00000320: 9c07 1600 7d08 640b 640c 7c08 6901 1600  ....}.d.d.|.i...
+00000330: 7d09 740b 7405 a00c 7c09 a101 8301 8201  }.t.t...|.......
+00000340: 6400 0400 7d04 0400 7d05 0400 7d07 7d06  d...}...}...}.}.
+00000350: 740d a00e 6700 640d a201 6700 640d a201  t...g.d...g.d...
+00000360: 640e 9c02 a101 7d0a 740d 6a0f a010 7c02  d.....}.t.j...|.
+00000370: 7c0a a102 0100 6400 5300 290f 4e72 0a00  |.....d.S.).Nr..
+00000380: 0000 720b 0000 0029 01da 0b63 6174 5f63  ..r....)...cat_c
+00000390: 6f6c 756d 6e73 720c 0000 0029 01fa 023d  olumnsr....)...=
+000003a0: 3d29 017a 6d25 2870 7935 2973 0a7b 2528  =).zm%(py5)s.{%(
+000003b0: 7079 3529 7320 3d20 2528 7079 3029 7328  py5)s = %(py0)s(
+000003c0: 2528 7079 3329 730a 7b25 2870 7933 2973  %(py3)s.{%(py3)s
+000003d0: 203d 2025 2870 7931 2973 2e63 6f6c 756d   = %(py1)s.colum
+000003e0: 6e73 0a7d 290a 7d20 3d3d 2025 2870 7931  ns.}).} == %(py1
+000003f0: 3029 730a 7b25 2870 7931 3029 7320 3d20  0)s.{%(py10)s = 
+00000400: 2528 7079 3729 7328 2528 7079 3829 7329  %(py7)s(%(py8)s)
+00000410: 0a7d da03 7365 74da 1074 7261 6e73 666f  .}..set..transfo
+00000420: 726d 6564 5f64 6174 61da 1065 7870 6563  rmed_data..expec
+00000430: 7465 645f 636f 6c75 6d6e 7329 07da 0370  ted_columns)...p
+00000440: 7930 da03 7079 31da 0370 7933 da03 7079  y0..py1..py3..py
+00000450: 35da 0370 7937 da03 7079 38da 0470 7931  5..py7..py8..py1
+00000460: 307a 0f61 7373 6572 7420 2528 7079 3132  0z.assert %(py12
+00000470: 2973 da04 7079 3132 2906 e700 0000 0000  )s..py12).......
+00000480: 00e0 3f72 2000 0000 7220 0000 0072 2000  ..?r ...r ...r .
+00000490: 0000 7220 0000 0072 2000 0000 2902 720a  ..r ...r ...).r.
+000004a0: 0000 0072 0b00 0000 2911 7202 0000 00da  ...r....).r.....
+000004b0: 1e66 6974 5f74 6172 6765 745f 656e 636f  .fit_target_enco
+000004c0: 6465 5f62 696e 6172 795f 636c 6173 73da  de_binary_class.
+000004d0: 2474 7261 6e73 666f 726d 5f74 6172 6765  $transform_targe
+000004e0: 745f 656e 636f 6465 5f62 696e 6172 795f  t_encode_binary_
+000004f0: 636c 6173 73da 0763 6f6c 756d 6e73 7215  class..columnsr.
+00000500: 0000 00da 0a40 7079 7465 7374 5f61 72da  .....@pytest_ar.
+00000510: 115f 6361 6c6c 5f72 6570 7263 6f6d 7061  ._call_reprcompa
+00000520: 7265 da0c 4070 795f 6275 696c 7469 6e73  re..@py_builtins
+00000530: da06 6c6f 6361 6c73 da18 5f73 686f 756c  ..locals.._shoul
+00000540: 645f 7265 7072 5f67 6c6f 6261 6c5f 6e61  d_repr_global_na
+00000550: 6d65 da09 5f73 6166 6572 6570 72da 0e41  me.._saferepr..A
+00000560: 7373 6572 7469 6f6e 4572 726f 72da 135f  ssertionError.._
+00000570: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
+00000580: 6f6e 720d 0000 0072 0e00 0000 da07 7465  onr....r......te
+00000590: 7374 696e 67da 1261 7373 6572 745f 6672  sting..assert_fr
+000005a0: 616d 655f 6571 7561 6c29 0b72 1200 0000  ame_equal).r....
+000005b0: da07 656e 636f 6465 7272 1600 0000 7217  ..encoderr....r.
+000005c0: 0000 00da 0b40 7079 5f61 7373 6572 7432  .....@py_assert2
+000005d0: da0b 4070 795f 6173 7365 7274 34da 0b40  ..@py_assert4..@
+000005e0: 7079 5f61 7373 6572 7439 da0b 4070 795f  py_assert9..@py_
+000005f0: 6173 7365 7274 36da 0c40 7079 5f66 6f72  assert6..@py_for
+00000600: 6d61 7431 31da 0c40 7079 5f66 6f72 6d61  mat11..@py_forma
+00000610: 7431 33da 0f65 7870 6563 7465 645f 7661  t13..expected_va
+00000620: 6c75 6573 7210 0000 0072 1000 0000 7211  luesr....r....r.
+00000630: 0000 00da 2974 6573 745f 7472 616e 7366  ....)test_transf
+00000640: 6f72 6d5f 7461 7267 6574 5f65 6e63 6f64  orm_target_encod
+00000650: 655f 6269 6e61 7279 5f63 6c61 7373 1400  e_binary_class..
+00000660: 0000 731c 0000 000e 0204 0310 0104 ff04  ..s.............
+00000670: 050a 0104 ff08 05fe 010a 0004 0310 0104  ................
+00000680: ff12 0372 3600 0000 290e da08 6275 696c  ...r6...)...buil
+00000690: 7469 6e73 7226 0000 00da 195f 7079 7465  tinsr&....._pyte
+000006a0: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
+000006b0: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
+000006c0: 0772 6577 7269 7465 7224 0000 00da 0670  .rewriter$.....p
+000006d0: 616e 6461 7372 0d00 0000 da06 7079 7465  andasr......pyte
+000006e0: 7374 da26 626c 7565 6361 7374 2e70 7265  st.&bluecast.pre
+000006f0: 7072 6f63 6573 7369 6e67 2e74 6172 6765  processing.targe
+00000700: 745f 656e 636f 6469 6e67 7202 0000 00da  t_encodingr.....
+00000710: 0766 6978 7475 7265 7212 0000 0072 3600  .fixturer....r6.
+00000720: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000730: 0072 1100 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000740: 0100 0000 730c 0000 0022 0008 010c 0204  ....s...."......
+00000750: 030a 010c 0c                             .....
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 04:56:12 2023 UTC, .py size: 735 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec0d 8064 df02 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ab09 8064 df02 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c08 6d09 5a09 0100 6403 6404  d.d.l.m.Z...d.d.
 00000060: 8400 5a0a 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da17 4d75 6c74 6943 6c61 7373 5461  )...MultiClassTa
@@ -64,29 +64,28 @@
 000003f0: 6e61 7469 6f6e da22 7472 616e 7366 6f72  nation."transfor
 00000400: 6d5f 7461 7267 6574 5f65 6e63 6f64 655f  m_target_encode_
 00000410: 6d75 6c74 6963 6c61 7373 2908 7205 0000  multiclass).r...
 00000420: 00da 0179 da07 656e 636f 6465 7272 0c00  ...y..encoderr..
 00000430: 0000 da0b 4070 795f 6173 7365 7274 33da  ....@py_assert3.
 00000440: 0b40 7079 5f61 7373 6572 7435 da0b 4070  .@py_assert5..@p
 00000450: 795f 666f 726d 6174 3772 1300 0000 a900  y_format7r......
-00000460: 7224 0000 00fa 5d2f 5573 6572 732f 7468  r$....]/Users/th
-00000470: 6f6d 6173 6d65 6973 736e 6572 2f49 6465  omasmeissner/Ide
-00000480: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
-00000490: 7374 2f62 6c75 6563 6173 742f 7465 7374  st/bluecast/test
-000004a0: 732f 7465 7374 5f74 6172 6765 745f 656e  s/test_target_en
-000004b0: 636f 6469 6e67 5f6d 756c 7469 636c 6173  coding_multiclas
-000004c0: 732e 7079 da1f 7465 7374 5f6d 756c 7469  s.py..test_multi
-000004d0: 5f63 6c61 7373 5f74 6172 6765 745f 656e  _class_target_en
-000004e0: 636f 6465 7206 0000 0073 0e00 0000 1802  coder....s......
-000004f0: 0e01 0e03 0c03 aa01 0a03 ae01 7226 0000  ............r&..
-00000500: 0029 0bda 0862 7569 6c74 696e 7372 1700  .)...builtinsr..
-00000510: 0000 da19 5f70 7974 6573 742e 6173 7365  ...._pytest.asse
-00000520: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
-00000530: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
-00000540: 6572 1900 0000 da06 7061 6e64 6173 720d  er......pandasr.
-00000550: 0000 00da 2662 6c75 6563 6173 742e 7072  ....&bluecast.pr
-00000560: 6570 726f 6365 7373 696e 672e 7461 7267  eprocessing.targ
-00000570: 6574 5f65 6e63 6f64 696e 6772 0200 0000  et_encodingr....
-00000580: 7226 0000 0072 2400 0000 7224 0000 0072  r&...r$...r$...r
-00000590: 2400 0000 7225 0000 00da 083c 6d6f 6475  $...r%.....<modu
-000005a0: 6c65 3e01 0000 0073 0600 0000 2200 0c02  le>....s...."...
-000005b0: 0c03                                     ..
+00000460: 7224 0000 00fa 542f 686f 6d65 2f74 686f  r$....T/home/tho
+00000470: 6d61 732f 4964 6561 5072 6f6a 6563 7473  mas/IdeaProjects
+00000480: 2f42 6c75 6543 6173 742f 626c 7565 6361  /BlueCast/blueca
+00000490: 7374 2f74 6573 7473 2f74 6573 745f 7461  st/tests/test_ta
+000004a0: 7267 6574 5f65 6e63 6f64 696e 675f 6d75  rget_encoding_mu
+000004b0: 6c74 6963 6c61 7373 2e70 79da 1f74 6573  lticlass.py..tes
+000004c0: 745f 6d75 6c74 695f 636c 6173 735f 7461  t_multi_class_ta
+000004d0: 7267 6574 5f65 6e63 6f64 6572 0600 0000  rget_encoder....
+000004e0: 730e 0000 0018 020e 010e 030c 03aa 010a  s...............
+000004f0: 03ae 0172 2600 0000 290b da08 6275 696c  ...r&...)...buil
+00000500: 7469 6e73 7217 0000 00da 195f 7079 7465  tinsr......_pyte
+00000510: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
+00000520: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
+00000530: 0772 6577 7269 7465 7219 0000 00da 0670  .rewriter......p
+00000540: 616e 6461 7372 0d00 0000 da26 626c 7565  andasr.....&blue
+00000550: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
+00000560: 6e67 2e74 6172 6765 745f 656e 636f 6469  ng.target_encodi
+00000570: 6e67 7202 0000 0072 2600 0000 7224 0000  ngr....r&...r$..
+00000580: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+00000590: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
+000005a0: 0000 0022 000c 020c 03                   ...".....
```

### Comparing `bluecast-0.2/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.3/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 04:56:12 2023 UTC, .py size: 1051 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec0d 8064 1b04 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 460d 8064 1b04 0000  o.......F..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a07  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c08 6d09 5a09 6d0a 5a0a 0100  d.d.l.m.Z.m.Z...
 00000060: 6403 6404 8400 5a0b 6405 6406 8400 5a0c  d.d...Z.d.d...Z.
 00000070: 6401 5300 2907 e900 0000 004e 2902 da16  d.S.)......N)...
@@ -87,49 +87,49 @@
 00000560: 745f 636f 6cda 0a74 7261 696e 5f73 697a  t_col..train_siz
 00000570: 65da 0c72 616e 646f 6d5f 7374 6174 6572  e..random_stater
 00000580: 1a00 0000 7222 0000 0072 2300 0000 7224  ....r"...r#...r$
 00000590: 0000 00da 0b40 7079 5f61 7373 6572 7432  .....@py_assert2
 000005a0: da0b 4070 795f 6173 7365 7274 35da 0b40  ..@py_assert5..@
 000005b0: 7079 5f61 7373 6572 7434 da0b 4070 795f  py_assert4..@py_
 000005c0: 666f 726d 6174 37da 0b40 7079 5f66 6f72  format7..@py_for
-000005d0: 6d61 7439 a900 7238 0000 00fa 532f 5573  mat9..r8....S/Us
-000005e0: 6572 732f 7468 6f6d 6173 6d65 6973 736e  ers/thomasmeissn
-000005f0: 6572 2f49 6465 6150 726f 6a65 6374 732f  er/IdeaProjects/
-00000600: 426c 7565 4361 7374 2f62 6c75 6563 6173  BlueCast/bluecas
-00000610: 742f 7465 7374 732f 7465 7374 5f74 7261  t/tests/test_tra
-00000620: 696e 5f74 6573 745f 7370 6c69 742e 7079  in_test_split.py
-00000630: da1b 7465 7374 5f74 7261 696e 5f74 6573  ..test_train_tes
-00000640: 745f 7370 6c69 745f 6372 6f73 730a 0000  t_split_cross...
-00000650: 00f3 1600 0000 1801 0401 0401 0401 0202  ................
-00000660: 0801 0cff ae05 ae01 b201 bc01 723a 0000  ............r:..
-00000670: 0063 0000 0000 0000 0000 0000 0000 0d00  .c..............
-00000680: 0000 0700 0000 4300 0000 7204 0000 0029  ......C...r....)
-00000690: 134e 7205 0000 0072 0b00 0000 7211 0000  .Nr....r....r...
-000006a0: 0072 1300 0000 7212 0000 0072 1400 0000  .r....r....r....
-000006b0: 7209 0000 0072 1600 0000 7218 0000 0072  r....r....r....r
-000006c0: 1900 0000 721a 0000 0072 1b00 0000 7220  ....r....r....r 
-000006d0: 0000 0072 2100 0000 7206 0000 0072 2200  ...r!...r....r".
-000006e0: 0000 7223 0000 0072 2400 0000 290c 7225  ..r#...r$...).r%
-000006f0: 0000 0072 2600 0000 7203 0000 0072 1900  ...r&...r....r..
-00000700: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-00000710: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000720: 722d 0000 0072 2e00 0000 290d 722f 0000  r-...r....).r/..
-00000730: 0072 3000 0000 da0c 7370 6c69 745f 6279  .r0.....split_by
-00000740: 5f63 6f6c 7231 0000 0072 1a00 0000 7222  _colr1...r....r"
-00000750: 0000 0072 2300 0000 7224 0000 0072 3300  ...r#...r$...r3.
-00000760: 0000 7234 0000 0072 3500 0000 7236 0000  ..r4...r5...r6..
-00000770: 0072 3700 0000 7238 0000 0072 3800 0000  .r7...r8...r8...
-00000780: 7239 0000 00da 1a74 6573 745f 7472 6169  r9.....test_trai
-00000790: 6e5f 7465 7374 5f73 706c 6974 5f74 696d  n_test_split_tim
-000007a0: 651c 0000 0072 3b00 0000 723d 0000 0029  e....r;...r=...)
-000007b0: 0dda 0862 7569 6c74 696e 7372 2900 0000  ...builtinsr)...
-000007c0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-000007d0: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-000007e0: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-000007f0: 2700 0000 da06 7061 6e64 6173 7225 0000  '.....pandasr%..
-00000800: 00da 2762 6c75 6563 6173 742e 7072 6570  ..'bluecast.prep
-00000810: 726f 6365 7373 696e 672e 7472 6169 6e5f  rocessing.train_
-00000820: 7465 7374 5f73 706c 6974 7202 0000 0072  test_splitr....r
-00000830: 0300 0000 723a 0000 0072 3d00 0000 7238  ....r:...r=...r8
-00000840: 0000 0072 3800 0000 7238 0000 0072 3900  ...r8...r8...r9.
-00000850: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000860: 7308 0000 0022 0010 0208 070c 12         s....".......
+000005d0: 6d61 7439 a900 7238 0000 00fa 4a2f 686f  mat9..r8....J/ho
+000005e0: 6d65 2f74 686f 6d61 732f 4964 6561 5072  me/thomas/IdeaPr
+000005f0: 6f6a 6563 7473 2f42 6c75 6543 6173 742f  ojects/BlueCast/
+00000600: 626c 7565 6361 7374 2f74 6573 7473 2f74  bluecast/tests/t
+00000610: 6573 745f 7472 6169 6e5f 7465 7374 5f73  est_train_test_s
+00000620: 706c 6974 2e70 79da 1b74 6573 745f 7472  plit.py..test_tr
+00000630: 6169 6e5f 7465 7374 5f73 706c 6974 5f63  ain_test_split_c
+00000640: 726f 7373 0a00 0000 f316 0000 0018 0104  ross............
+00000650: 0104 0104 0102 0208 010c ffae 05ae 01b2  ................
+00000660: 01bc 0172 3a00 0000 6300 0000 0000 0000  ...r:...c.......
+00000670: 0000 0000 000d 0000 0007 0000 0043 0000  .............C..
+00000680: 0072 0400 0000 2913 4e72 0500 0000 720b  .r....).Nr....r.
+00000690: 0000 0072 1100 0000 7213 0000 0072 1200  ...r....r....r..
+000006a0: 0000 7214 0000 0072 0900 0000 7216 0000  ..r....r....r...
+000006b0: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+000006c0: 721b 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+000006d0: 0600 0000 7222 0000 0072 2300 0000 7224  ....r"...r#...r$
+000006e0: 0000 0029 0c72 2500 0000 7226 0000 0072  ...).r%...r&...r
+000006f0: 0300 0000 7219 0000 0072 2700 0000 7228  ....r....r'...r(
+00000700: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00000710: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+00000720: 0029 0d72 2f00 0000 7230 0000 00da 0c73  .).r/...r0.....s
+00000730: 706c 6974 5f62 795f 636f 6c72 3100 0000  plit_by_colr1...
+00000740: 721a 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
+00000750: 2400 0000 7233 0000 0072 3400 0000 7235  $...r3...r4...r5
+00000760: 0000 0072 3600 0000 7237 0000 0072 3800  ...r6...r7...r8.
+00000770: 0000 7238 0000 0072 3900 0000 da1a 7465  ..r8...r9.....te
+00000780: 7374 5f74 7261 696e 5f74 6573 745f 7370  st_train_test_sp
+00000790: 6c69 745f 7469 6d65 1c00 0000 723b 0000  lit_time....r;..
+000007a0: 0072 3d00 0000 290d da08 6275 696c 7469  .r=...)...builti
+000007b0: 6e73 7229 0000 00da 195f 7079 7465 7374  nsr)....._pytest
+000007c0: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
+000007d0: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
+000007e0: 6577 7269 7465 7227 0000 00da 0670 616e  ewriter'.....pan
+000007f0: 6461 7372 2500 0000 da27 626c 7565 6361  dasr%....'blueca
+00000800: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+00000810: 2e74 7261 696e 5f74 6573 745f 7370 6c69  .train_test_spli
+00000820: 7472 0200 0000 7203 0000 0072 3a00 0000  tr....r....r:...
+00000830: 723d 0000 0072 3800 0000 7238 0000 0072  r=...r8...r8...r
+00000840: 3800 0000 7239 0000 00da 083c 6d6f 6475  8...r9.....<modu
+00000850: 6c65 3e01 0000 0073 0800 0000 2200 1002  le>....s...."...
+00000860: 0807 0c12                                ....
```

### Comparing `bluecast-0.2/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-0.3/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 04:56:12 2023 UTC, .py size: 1289 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ec0d 8064 0905 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 2305 8064 0905 0000  o.......#..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c04 6d05 5a05 0100 0904 6409 6405  d.l.m.Z.....d.d.
 00000050: 6506 6406 6503 6a07 6604 6407 6408 8405  e.d.e.j.f.d.d...
 00000060: 5a08 6401 5300 290a e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da13 6d61 6b65 5f63 6c61 7373 6966 6963  ..make_classific
@@ -45,27 +45,27 @@
 000002c0: 6461 7465 5f72 616e 6765 da02 6e70 da06  date_range..np..
 000002d0: 7261 6e64 6f6d da06 6368 6f69 6365 da09  random..choice..
 000002e0: 4461 7461 4672 616d 6529 0ada 0b6e 756d  DataFrame)...num
 000002f0: 5f73 616d 706c 6573 7205 0000 00da 0178  _samplesr......x
 00000300: da01 79da 0a73 7461 7274 5f64 6174 65da  ..y..start_date.
 00000310: 0865 6e64 5f64 6174 6572 1a00 0000 7218  .end_dater....r.
 00000320: 0000 0072 1900 0000 da02 6466 a900 7229  ...r......df..r)
-00000330: 0000 00fa 532f 5573 6572 732f 7468 6f6d  ....S/Users/thom
-00000340: 6173 6d65 6973 736e 6572 2f49 6465 6150  asmeissner/IdeaP
-00000350: 726f 6a65 6374 732f 426c 7565 4361 7374  rojects/BlueCast
-00000360: 2f62 6c75 6563 6173 742f 7465 7374 732f  /bluecast/tests/
-00000370: 6d61 6b65 5f64 6174 612f 6372 6561 7465  make_data/create
-00000380: 5f64 6174 612e 7079 da1a 6372 6561 7465  _data.py..create
-00000390: 5f73 796e 7468 6574 6963 5f64 6174 6166  _synthetic_dataf
-000003a0: 7261 6d65 0600 0000 7334 0000 0002 0402  rame....s4......
-000003b0: 0102 0102 0102 0102 0102 010a fa0a 0a0a  ................
-000003c0: 0104 0106 0106 ff14 0514 0104 0302 0202  ................
-000003d0: 010e 010e 010e 0102 0102 0104 f904 ff04  ................
-000003e0: 0c72 2b00 0000 2902 7203 0000 0072 0400  .r+...).r....r..
-000003f0: 0000 2909 da05 6e75 6d70 7972 1f00 0000  ..)...numpyr....
-00000400: da06 7061 6e64 6173 721c 0000 00da 1073  ..pandasr......s
-00000410: 6b6c 6561 726e 2e64 6174 6173 6574 7372  klearn.datasetsr
-00000420: 0200 0000 da03 696e 7472 2200 0000 722b  ......intr"...r+
-00000430: 0000 0072 2900 0000 7229 0000 0072 2900  ...r)...r)...r).
-00000440: 0000 722a 0000 00da 083c 6d6f 6475 6c65  ..r*.....<module
-00000450: 3e01 0000 0073 1200 0000 0800 0801 0c01  >....s..........
-00000460: 0204 04ff 0201 02ff 0402 0efe            ............
+00000330: 0000 00fa 4a2f 686f 6d65 2f74 686f 6d61  ....J/home/thoma
+00000340: 732f 4964 6561 5072 6f6a 6563 7473 2f42  s/IdeaProjects/B
+00000350: 6c75 6543 6173 742f 626c 7565 6361 7374  lueCast/bluecast
+00000360: 2f74 6573 7473 2f6d 616b 655f 6461 7461  /tests/make_data
+00000370: 2f63 7265 6174 655f 6461 7461 2e70 79da  /create_data.py.
+00000380: 1a63 7265 6174 655f 7379 6e74 6865 7469  .create_syntheti
+00000390: 635f 6461 7461 6672 616d 6506 0000 0073  c_dataframe....s
+000003a0: 3400 0000 0204 0201 0201 0201 0201 0201  4...............
+000003b0: 0201 0afa 0a0a 0a01 0401 0601 06ff 1405  ................
+000003c0: 1401 0403 0202 0201 0e01 0e01 0e01 0201  ................
+000003d0: 0201 04f9 04ff 040c 722b 0000 0029 0272  ........r+...).r
+000003e0: 0300 0000 7204 0000 0029 09da 056e 756d  ....r....)...num
+000003f0: 7079 721f 0000 00da 0670 616e 6461 7372  pyr......pandasr
+00000400: 1c00 0000 da10 736b 6c65 6172 6e2e 6461  ......sklearn.da
+00000410: 7461 7365 7473 7202 0000 00da 0369 6e74  tasetsr......int
+00000420: 7222 0000 0072 2b00 0000 7229 0000 0072  r"...r+...r)...r
+00000430: 2900 0000 7229 0000 0072 2a00 0000 da08  )...r)...r*.....
+00000440: 3c6d 6f64 756c 653e 0100 0000 7312 0000  <module>....s...
+00000450: 0008 0008 010c 0102 0404 ff02 0102 ff04  ................
+00000460: 020e fe                                  ...
```

### Comparing `bluecast-0.2/bluecast/tests/make_data/create_data.py` & `bluecast-0.3/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_check_gpu_support.py` & `bluecast-0.3/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-0.3/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_datetime_features.py` & `bluecast-0.3/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_encode_target_labels.py` & `bluecast-0.3/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_feature_type_detector.py` & `bluecast-0.3/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_load_for_production.py` & `bluecast-0.3/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_nulls_and_infs.py` & `bluecast-0.3/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_save_to_production.py` & `bluecast-0.3/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_schema_checks.py` & `bluecast-0.3/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_shap_explanations.py` & `bluecast-0.3/bluecast/tests/test_shap_explanations.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_target_encoding_binary.py` & `bluecast-0.3/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-0.3/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/bluecast/tests/test_train_test_split.py` & `bluecast-0.3/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.2/pyproject.toml` & `bluecast-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "0.2"
+version = "0.3"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `bluecast-0.2/PKG-INFO` & `bluecast-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 0.2
+Version: 0.3
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -47,26 +47,28 @@
 A lightweight and fast auto-ml library. This is the successor of the
 e2eml automl library. While e2eml tried to cover many model
 architectures and a lot of different preprocessing options,
 BlueCast focuses on a few model architectures (on default Xgboost
 only) and a few preprocessing options (only what is
 needed for Xgboost). This allows for a much faster development
 cycle and a much more stable codebase while also having as few dependencies
-as possible for the library.
+as possible for the library. Despite being lightweight in its core BlueCast
+offers high customization options for advanced users.
 
 <!-- toc -->
 
 * [Installation](#installation)
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
     * [Custom training configuration](#custom--training-configuration)
     * [Custom preprocessing](#custom-preprocessing)
+    * [Custom feature selection](#custom-feature-selection)
     * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
 * [Meta](#meta)
 
@@ -263,14 +265,61 @@
         custom_last_mile_computation=custom_last_mile_computation, # last step before model training/prediction
     )
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
+#### Custom feature selection
+
+As of version 0.3 BlueCast added automated feature selection. Also this
+step can be customized. An instance of `RFECV` is expected for `selection_strategy`.
+Otherwise the pipeline will fail. To disable feature selection set `execute_selection`
+to `False`. To surpass the `RFECV` limitation a custom feature selection algorithm
+can also be passed as part of a custom last mile computation.
+
+```sh
+from bluecast.config.training_config import FeatureSelectionConfig
+from sklearn.feature_selection import RFECV
+from sklearn.metrics import make_scorer, matthews_corrcoef
+from sklearn.model_selection import StratifiedKFold
+
+# add custom feature selection
+custom_feat_sel = FeatureSelectionConfig()
+# custom_feat_sel.execute_selection = False
+custom_feat_sel.selection_strategy = RFECV(
+    estimator=xgb.XGBClassifier(),
+    step=1,
+    cv=StratifiedKFold(10, random_state=0, shuffle=True),
+    min_features_to_select=1,
+    scoring=make_scorer(matthews_corrcoef),
+    n_jobs=1,
+)
+
+# Create an instance of the BlueCast class with the custom model
+bluecast = BlueCast(
+    class_problem="binary",
+    target_column="target",
+    conf_feature_selection=custom_feat_sel,
+
+# Create some sample data for testing
+x_train = pd.DataFrame(
+    {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
+)
+y_train = pd.Series([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
+x_test = pd.DataFrame(
+    {"feature1": [i for i in range(10)], "feature2": [i for i in range(10)]}
+
+x_train["target"] = y_trai
+# Fit the BlueCast model using the custom model
+bluecast.fit(x_train, "target"
+# Predict on the test data using the custom model
+predicted_probas, predicted_classes = bluecast.predict(x_test)
+```
+
 #### Custom ML model
 
 For some users it might just be convenient to use the BlueCast class to
 enjoy convenience features (details see below), but use a custom ML model.
 This is possible by passing a custom model to the BlueCast class. The needed properties
 are defined via the BaseClassMlModel class. Here is an example:
 
@@ -389,15 +438,15 @@
 * Push your changes and create a pull request
 
 If library or dev dependencies have to be changed, adjust the pyproject.toml.
 For readthedocs it is also requited to update the
 `docs/srtd_requirements.txt` file. Simply run:
 
 ```sh
-poetry export --with doc -f requirements.txt --output docs/rtd_requirements.txt
+poetry export --with dev -f requirements.txt --output docs/rtd_requirements.txt
 ```
 
 If readthedocs will be able to create the documentation can be tested via:
 
 ```sh
 poetry run sphinx-autobuild docs/source docs/build/html
 ```
```

