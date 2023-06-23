# Comparing `tmp/autogluon.tabular-0.8.1b20230622.tar.gz` & `tmp/autogluon.tabular-0.8.1b20230623.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.8.1b20230622.tar", last modified: Thu Jun 22 09:04:00 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.8.1b20230623.tar", last modified: Fri Jun 23 09:04:27 2023, max compression
```

## Comparing `autogluon.tabular-0.8.1b20230622.tar` & `autogluon.tabular-0.8.1b20230623.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.931861 autogluon.tabular-0.8.1b20230622/
--rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-22 09:04:00.931861 autogluon.tabular-0.8.1b20230622/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:04:00.931861 autogluon.tabular-0.8.1b20230622/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.915860 autogluon.tabular-0.8.1b20230622/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.915860 autogluon.tabular-0.8.1b20230622/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.923860 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35982 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.927861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)   267286 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.931861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.931861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.931861 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-22 09:03:32.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:00.919860 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:04:00.000000 autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.709527 autogluon.tabular-0.8.1b20230623/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.709527 autogluon.tabular-0.8.1b20230623/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.713527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.713527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.713527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50070 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.713527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.713527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.713527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15630 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25573 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.717527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.721527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.721527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.721527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.721527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.721527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.721527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36172 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22903 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22575 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16873 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34250 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.725527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   263985 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.729527 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-23 09:04:00.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:04:27.713527 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12918 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:04:27.000000 autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.8.1b20230622/PKG-INFO` & `autogluon.tabular-0.8.1b20230623/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.8.1b20230622
+Version: 0.8.1b20230623
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.8.1b20230622/setup.py` & `autogluon.tabular-0.8.1b20230623/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,103 @@
 #!/usr/bin/env python
 ###########################
 # This code block is a HACK (!), but is necessary to avoid code duplication. Do NOT alter these lines.
+import importlib.util
 import os
+
 from setuptools import setup
-import importlib.util
+
 filepath = os.path.abspath(os.path.dirname(__file__))
-filepath_import = os.path.join(filepath, '..', 'core', 'src', 'autogluon', 'core', '_setup_utils.py')
+filepath_import = os.path.join(filepath, "..", "core", "src", "autogluon", "core", "_setup_utils.py")
 spec = importlib.util.spec_from_file_location("ag_min_dependencies", filepath_import)
 ag = importlib.util.module_from_spec(spec)
 # Identical to `from autogluon.core import _setup_utils as ag`, but works without `autogluon.core` being installed.
 spec.loader.exec_module(ag)
 ###########################
 
 import sys
 
 version = ag.load_version_file()
 version = ag.update_version(version)
 
-submodule = 'tabular'
+submodule = "tabular"
 install_requires = [
     # version ranges added in ag.get_dependency_version_ranges()
-    'numpy',  # version range defined in `core/_setup_utils.py`
-    'scipy',  # version range defined in `core/_setup_utils.py`
-    'pandas',  # version range defined in `core/_setup_utils.py`
-    'scikit-learn',  # version range defined in `core/_setup_utils.py`
-    'networkx',  # version range defined in `core/_setup_utils.py`
-    f'{ag.PACKAGE_NAME}.core=={version}',
-    f'{ag.PACKAGE_NAME}.features=={version}',
+    "numpy",  # version range defined in `core/_setup_utils.py`
+    "scipy",  # version range defined in `core/_setup_utils.py`
+    "pandas",  # version range defined in `core/_setup_utils.py`
+    "scikit-learn",  # version range defined in `core/_setup_utils.py`
+    "networkx",  # version range defined in `core/_setup_utils.py`
+    f"{ag.PACKAGE_NAME}.core=={version}",
+    f"{ag.PACKAGE_NAME}.features=={version}",
 ]
 
 extras_require = {
-    'lightgbm': [
-        'lightgbm>=3.3,<3.4',
+    "lightgbm": [
+        "lightgbm>=3.3,<3.4",
     ],
-    'catboost': [
+    "catboost": [
         # CatBoost wheel build is not working correctly on darwin for CatBoost 1.2, so use old version in this case.
         # https://github.com/autogluon/autogluon/pull/3190#issuecomment-1540599280
         'catboost>=1.1,<1.2 ; sys_platform == "darwin"',
-        'catboost>=1.1,<1.3',
+        "catboost>=1.1,<1.3",
     ],
     # FIXME: Debug why xgboost 1.6 has 4x+ slower inference on multiclass datasets compared to 1.4
     #  It is possibly only present on MacOS, haven't tested linux.
     # XGBoost made API breaking changes in 1.6 with custom metric and callback support, so we don't support older versions.
-    'xgboost': [
-        'xgboost>=1.6,<1.8',
+    "xgboost": [
+        "xgboost>=1.6,<1.8",
     ],
-    'fastai': [
-        'torch>=1.9,<1.14',
-        'fastai>=2.3.1,<2.8',
+    "fastai": [
+        "torch>=1.9,<1.14",
+        "fastai>=2.3.1,<2.8",
     ],
-    'tabpfn': [
-        'tabpfn>=0.1,<0.2',
+    "tabpfn": [
+        "tabpfn>=0.1,<0.2",
     ],
-    'ray': [
-        f'{ag.PACKAGE_NAME}.core[all]=={version}',
+    "ray": [
+        f"{ag.PACKAGE_NAME}.core[all]=={version}",
     ],
-    'skex': [
+    "skex": [
         # Note: 2021.7 released on Sep 2022, version 2022.x doesn't exist (went directly from 2021.7 to 2023.0)
-        'scikit-learn-intelex>=2021.7,<2023.2',
+        "scikit-learn-intelex>=2021.7,<2023.2",
     ],
-    'imodels': [
-        'imodels>=1.3.10,<1.4.0',  # 1.3.8/1.3.9 either remove/renamed attribute `complexity_` causing failures. https://github.com/csinva/imodels/issues/147
+    "imodels": [
+        "imodels>=1.3.10,<1.4.0",  # 1.3.8/1.3.9 either remove/renamed attribute `complexity_` causing failures. https://github.com/csinva/imodels/issues/147
     ],
-    'vowpalwabbit': [
+    "vowpalwabbit": [
         # FIXME: 9.5+ causes VW to save an empty model which always predicts 0. Confirmed on MacOS (Intel CPU). Unknown how to fix.
-        'vowpalwabbit>=9,<9.5',
+        "vowpalwabbit>=9,<9.5",
     ],
-    'skl2onnx': [
-        'skl2onnx>=1.13.0,<1.14.0',
+    "skl2onnx": [
+        "skl2onnx>=1.13.0,<1.14.0",
         # For macOS, there isn't a onnxruntime-gpu package installed with skl2onnx.
         # Therefore, we install onnxruntime explicitly here just for macOS.
-        'onnxruntime>=1.13.0,<1.14.0'
-    ] if sys.platform == 'darwin' else [
-        'skl2onnx>=1.13.0,<1.14.0',
-        'onnxruntime-gpu>=1.13.0,<1.14.0'
+        "onnxruntime>=1.13.0,<1.14.0",
     ]
+    if sys.platform == "darwin"
+    else ["skl2onnx>=1.13.0,<1.14.0", "onnxruntime-gpu>=1.13.0,<1.14.0"],
 }
 
 # TODO: v1.0: Rename `all` to `core`, make `all` contain everything.
 all_requires = []
 # TODO: Consider adding 'skex' to 'all'
-for extra_package in ['lightgbm', 'catboost', 'xgboost', 'fastai', 'ray']:
+for extra_package in ["lightgbm", "catboost", "xgboost", "fastai", "ray"]:
     all_requires += extras_require[extra_package]
 all_requires = list(set(all_requires))
-extras_require['all'] = all_requires
+extras_require["all"] = all_requires
 
 
 test_requires = []
-for test_package in ['tabpfn', 'imodels', 'vowpalwabbit', 'skl2onnx']:
+for test_package in ["tabpfn", "imodels", "vowpalwabbit", "skl2onnx"]:
     test_requires += extras_require[test_package]
-extras_require['tests'] = test_requires
+extras_require["tests"] = test_requires
 install_requires = ag.get_dependency_version_ranges(install_requires)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     ag.create_version_file(version=version, submodule=submodule)
     setup_args = ag.default_setup_args(version=version, submodule=submodule)
     setup(
         install_requires=install_requires,
         extras_require=extras_require,
         **setup_args,
     )
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/config_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,96 +19,95 @@
 
     def enable_numeric_features(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         Whether to keep features of 'int' and 'float' raw types.
         These features are passed without alteration to the models.
         Appends IdentityFeatureGenerator(infer_features_in_args=dict(valid_raw_types=['int', 'float']))) to the generator group.
         """
-        self.config['enable_numeric_features'] = value
+        self.config["enable_numeric_features"] = value
         return self
 
     def enable_categorical_features(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         Whether to keep features of 'object' and 'category' raw types.
         These features are processed into memory optimized 'category' features.
         Appends CategoryFeatureGenerator() to the generator group.
         """
-        self.config['enable_categorical_features'] = value
+        self.config["enable_categorical_features"] = value
         return self
 
     def enable_datetime_features(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         Whether to keep features of 'datetime' raw type and 'object' features identified as 'datetime_as_object' features.
         These features will be converted to 'int' features representing milliseconds since epoch.
         Appends DatetimeFeatureGenerator() to the generator group.
         """
-        self.config['enable_datetime_features'] = value
+        self.config["enable_datetime_features"] = value
         return self
 
     def enable_text_special_features(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         Whether to use 'object' features identified as 'text' features to generate 'text_special' features such as word count, capital letter ratio, and symbol counts.
         Appends TextSpecialFeatureGenerator() to the generator group.
         """
-        self.config['enable_text_special_features'] = value
+        self.config["enable_text_special_features"] = value
         return self
 
     def enable_text_ngram_features(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         Whether to use 'object' features identified as 'text' features to generate 'text_ngram' features.
         Appends TextNgramFeatureGenerator(vectorizer=vectorizer) to the generator group.
         """
-        self.config['enable_text_ngram_features'] = value
+        self.config["enable_text_ngram_features"] = value
         return self
 
     def enable_raw_text_features(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         Whether to keep the raw text features.
         Appends IdentityFeatureGenerator(infer_features_in_args=dict(required_special_types=['text'])) to the generator group.
         """
-        self.config['enable_raw_text_features'] = value
+        self.config["enable_raw_text_features"] = value
         return self
 
     def enable_vision_features(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         [Experimental]
         Whether to keep 'object' features identified as 'image_path' special type. Features of this form should have a string path to an image file as their value.
         Only vision models can leverage these features, and these features will not be treated as categorical.
         Note: 'image_path' features will not be automatically inferred. These features must be explicitly specified as such in a custom FeatureMetadata object.
         Note: It is recommended that the string paths use absolute paths rather than relative, as it will likely be more stable.
         """
-        self.config['enable_vision_features'] = value
+        self.config["enable_vision_features"] = value
         return self
 
     def vectorizer(self, value: BaseEstimator) -> FeatureGeneratorBuilder:
         """
         sklearn CountVectorizer object to use in TextNgramFeatureGenerator.
         Only used if `enable_text_ngram_features=True`.
         """
-        self.config['vectorizer'] = value
+        self.config["vectorizer"] = value
         return self
 
     def text_ngram_params(self, value: bool = True) -> FeatureGeneratorBuilder:
         """
         Appends TextNgramFeatureGenerator(vectorizer=vectorizer, text_ngram_params) to the generator group. See text_ngram.py for valid parameters.
         """
-        self.config['text_ngram_params'] = value
+        self.config["text_ngram_params"] = value
         return self
 
     def build(self) -> Union[ConfigBuilder, AutoMLPipelineFeatureGenerator]:
         generator = AutoMLPipelineFeatureGenerator(**self.config)
         if self.parent:
-            self.parent.config['feature_generator'] = generator
+            self.parent.config["feature_generator"] = generator
             return self.parent
         else:
             return generator
 
 
 class ConfigBuilder:
-
     def __init__(self):
         self.config = {}
 
     def presets(self, presets: Union[str, list, dict]) -> ConfigBuilder:
         """
         List of preset configurations for various arguments in `fit()`. Can significantly impact predictive accuracy, memory-footprint, and inference latency of trained models, and various other properties of the returned `predictor`.
         It is recommended to specify presets and avoid specifying most other `fit()` arguments or model hyperparameters prior to becoming familiar with AutoGluon.
@@ -118,231 +117,231 @@
         """
         valid_keys = list(tabular_presets_dict.keys())
         if isinstance(presets, str):
             presets = [presets]
 
         if isinstance(presets, list):
             unknown_keys = [k for k in presets if k not in valid_keys]
-            assert len(unknown_keys) == 0, f'The following presets are not recognized: {unknown_keys} - use one of the valid presets: {valid_keys}'
+            assert len(unknown_keys) == 0, f"The following presets are not recognized: {unknown_keys} - use one of the valid presets: {valid_keys}"
 
-        self.config['presets'] = presets
+        self.config["presets"] = presets
         return self
 
     def time_limit(self, time_limit: int) -> ConfigBuilder:
         """
         Approximately how long `fit()` should run for (wallclock time in seconds).
         If not specified, `fit()` will run until all models have completed training, but will not repeatedly bag models unless `num_bag_sets` is specified.
         """
         if time_limit is not None:
-            assert time_limit > 0, 'time_limit must be greater than zero'
-        self.config['time_limit'] = time_limit
+            assert time_limit > 0, "time_limit must be greater than zero"
+        self.config["time_limit"] = time_limit
         return self
 
     def hyperparameters(self, hyperparameters: Union[str, dict]) -> ConfigBuilder:
-        valid_keys = [m for m in MODEL_TYPES.keys() if m not in ['ENS_WEIGHTED', 'SIMPLE_ENS_WEIGHTED']]
+        valid_keys = [m for m in MODEL_TYPES.keys() if m not in ["ENS_WEIGHTED", "SIMPLE_ENS_WEIGHTED"]]
         valid_str_values = list(hyperparameter_config_dict.keys())
         if isinstance(hyperparameters, str):
-            assert hyperparameters in hyperparameter_config_dict, f'{hyperparameters} is not one of the valid presets {valid_str_values}'
+            assert hyperparameters in hyperparameter_config_dict, f"{hyperparameters} is not one of the valid presets {valid_str_values}"
         elif isinstance(hyperparameters, dict):
             unknown_keys = [k for k in hyperparameters.keys() if isinstance(k, str) and (k not in valid_keys)]
-            assert len(unknown_keys) == 0, f'The following model types are not recognized: {unknown_keys} - use one of the valid models: {valid_keys}'
+            assert len(unknown_keys) == 0, f"The following model types are not recognized: {unknown_keys} - use one of the valid models: {valid_keys}"
         else:
-            raise ValueError(f'hyperparameters must be either str: {valid_str_values} or dict with keys of {valid_keys}')
-        self.config['hyperparameters'] = hyperparameters
+            raise ValueError(f"hyperparameters must be either str: {valid_str_values} or dict with keys of {valid_keys}")
+        self.config["hyperparameters"] = hyperparameters
         return self
 
     def auto_stack(self, auto_stack: bool = True) -> ConfigBuilder:
         """
         Whether AutoGluon should automatically utilize bagging and multi-layer stack ensembling to boost predictive accuracy.
         Set this = True if you are willing to tolerate longer training times in order to maximize predictive accuracy!
         Automatically sets `num_bag_folds` and `num_stack_levels` arguments based on dataset properties.
         Note: Setting `num_bag_folds` and `num_stack_levels` arguments will override `auto_stack`.
         Note: This can increase training time (and inference time) by up to 20x, but can greatly improve predictive performance.
         """
-        self.config['auto_stack'] = auto_stack
+        self.config["auto_stack"] = auto_stack
         return self
 
     def num_bag_folds(self, num_bag_folds: int) -> ConfigBuilder:
         """
         Number of folds used for bagging of models. When `num_bag_folds = k`, training time is roughly increased by a factor of `k` (set = 0 to disable bagging).
         Disabled by default (0), but we recommend values between 5-10 to maximize predictive performance.
         Increasing num_bag_folds will result in models with lower bias but that are more prone to overfitting.
         `num_bag_folds = 1` is an invalid value, and will raise a ValueError.
         Values > 10 may produce diminishing returns, and can even harm overall results due to overfitting.
         To further improve predictions, avoid increasing `num_bag_folds` much beyond 10 and instead increase `num_bag_sets`.
         """
-        assert num_bag_folds >= 0, 'num_bag_folds must be greater or equal than zero'
-        self.config['num_bag_folds'] = num_bag_folds
+        assert num_bag_folds >= 0, "num_bag_folds must be greater or equal than zero"
+        self.config["num_bag_folds"] = num_bag_folds
         return self
 
     def num_bag_sets(self, num_bag_sets: int) -> ConfigBuilder:
         """
         Number of repeats of kfold bagging to perform (values must be >= 1). Total number of models trained during bagging = `num_bag_folds * num_bag_sets`.
         Defaults to 1 if `time_limit` is not specified, otherwise 20 (always disabled if `num_bag_folds` is not specified).
         Values greater than 1 will result in superior predictive performance, especially on smaller problems and with stacking enabled (reduces overall variance).
         """
-        assert num_bag_sets > 0, 'num_bag_sets must be greater than zero'
-        self.config['num_bag_sets'] = num_bag_sets
+        assert num_bag_sets > 0, "num_bag_sets must be greater than zero"
+        self.config["num_bag_sets"] = num_bag_sets
         return self
 
     def num_stack_levels(self, num_stack_levels: int) -> ConfigBuilder:
         """
         Number of stacking levels to use in stack ensemble. Roughly increases model training time by factor of `num_stack_levels+1` (set = 0 to disable stack ensembling).
         Disabled by default (0), but we recommend values between 1-3 to maximize predictive performance.
         To prevent overfitting, `num_bag_folds >= 2` must also be set or else a ValueError will be raised.
         """
-        assert num_stack_levels >= 0, 'num_stack_levels must be greater or equal than zero'
-        self.config['num_stack_levels'] = num_stack_levels
+        assert num_stack_levels >= 0, "num_stack_levels must be greater or equal than zero"
+        self.config["num_stack_levels"] = num_stack_levels
         return self
 
     def holdout_frac(self, holdout_frac: float) -> ConfigBuilder:
         """
         Fraction of train_data to holdout as tuning data for optimizing hyperparameters (ignored unless `tuning_data = None`, ignored if `num_bag_folds != 0` unless `use_bag_holdout == True`).
         Default value (if None) is selected based on the number of rows in the training data. Default values range from 0.2 at 2,500 rows to 0.01 at 250,000 rows.
         Default value is doubled if `hyperparameter_tune_kwargs` is set, up to a maximum of 0.2.
         Disabled if `num_bag_folds >= 2` unless `use_bag_holdout == True`.
         """
-        assert (holdout_frac >= 0) & (holdout_frac <= 1), 'holdout_frac must be between 0 and 1'
-        self.config['holdout_frac'] = holdout_frac
+        assert (holdout_frac >= 0) & (holdout_frac <= 1), "holdout_frac must be between 0 and 1"
+        self.config["holdout_frac"] = holdout_frac
         return self
 
     def use_bag_holdout(self, use_bag_holdout: bool = True) -> ConfigBuilder:
         """
         If True, a `holdout_frac` portion of the data is held-out from model bagging.
         This held-out data is only used to score models and determine weighted ensemble weights.
         Enable this if there is a large gap between score_val and score_test in stack models.
         Note: If `tuning_data` was specified, `tuning_data` is used as the holdout data.
         Disabled if not bagging.
         """
-        self.config['use_bag_holdout'] = use_bag_holdout
+        self.config["use_bag_holdout"] = use_bag_holdout
         return self
 
     def hyperparameter_tune_kwargs(self, hyperparameter_tune_kwargs: Union[str, dict]) -> ConfigBuilder:
         """
         Hyperparameter tuning strategy and kwargs (for example, how many HPO trials to run).
         If None, then hyperparameter tuning will not be performed.
         Valid preset values:
             'auto': Uses the 'random' preset.
             'random': Performs HPO via random search using local scheduler.
         The 'searcher' key is required when providing a dict.
         """
         valid_str_values = scheduler_factory._scheduler_presets.keys()
         if isinstance(hyperparameter_tune_kwargs, str):
-            assert hyperparameter_tune_kwargs in valid_str_values, f'{hyperparameter_tune_kwargs} string must be one of {valid_str_values}'
+            assert hyperparameter_tune_kwargs in valid_str_values, f"{hyperparameter_tune_kwargs} string must be one of {valid_str_values}"
         elif not isinstance(hyperparameter_tune_kwargs, dict):
-            raise ValueError(f'hyperparameter_tune_kwargs must be either str: {valid_str_values} or dict')
-        self.config['hyperparameter_tune_kwargs'] = hyperparameter_tune_kwargs
+            raise ValueError(f"hyperparameter_tune_kwargs must be either str: {valid_str_values} or dict")
+        self.config["hyperparameter_tune_kwargs"] = hyperparameter_tune_kwargs
 
         return self
 
     def ag_args(self, ag_args: dict) -> ConfigBuilder:
         """
         Keyword arguments to pass to all models (i.e. common hyperparameters shared by all AutoGluon models).
         See the `ag_args` argument from "Advanced functionality: Custom AutoGluon model arguments" in the `hyperparameters` argument documentation for valid values.
         Identical to specifying `ag_args` parameter for all models in `hyperparameters`.
         If a key in `ag_args` is already specified for a model in `hyperparameters`, it will not be altered through this argument.
         """
-        self.config['ag_args'] = ag_args
+        self.config["ag_args"] = ag_args
         return self
 
     def ag_args_fit(self, ag_args_fit: dict) -> ConfigBuilder:
         """
         Keyword arguments to pass to all models.
         See the `ag_args_fit` argument from "Advanced functionality: Custom AutoGluon model arguments" in the `hyperparameters` argument documentation for valid values.
         Identical to specifying `ag_args_fit` parameter for all models in `hyperparameters`.
         If a key in `ag_args_fit` is already specified for a model in `hyperparameters`, it will not be altered through this argument.
         """
-        self.config['ag_args_fit'] = ag_args_fit
+        self.config["ag_args_fit"] = ag_args_fit
         return self
 
     def ag_args_ensemble(self, ag_args_ensemble: dict) -> ConfigBuilder:
         """
         Keyword arguments to pass to all models.
         See the `ag_args_ensemble` argument from "Advanced functionality: Custom AutoGluon model arguments" in the `hyperparameters` argument documentation for valid values.
         Identical to specifying `ag_args_ensemble` parameter for all models in `hyperparameters`.
         If a key in `ag_args_ensemble` is already specified for a model in `hyperparameters`, it will not be altered through this argument.
         """
-        self.config['ag_args_ensemble'] = ag_args_ensemble
+        self.config["ag_args_ensemble"] = ag_args_ensemble
         return self
 
     def excluded_model_types(self, models: Union[str, list]) -> ConfigBuilder:
         """
         Banned subset of model types to avoid training during `fit()`, even if present in `hyperparameters`.
         Reference `hyperparameters` documentation for what models correspond to each value.
         Useful when a particular model type such as 'KNN' or 'custom' is not desired but altering the `hyperparameters` dictionary is difficult or time-consuming.
             Example: To exclude both 'KNN' and 'custom' models, specify `excluded_model_types=['KNN', 'custom']`.
         """
-        valid_keys = [m for m in MODEL_TYPES.keys() if m not in ['ENS_WEIGHTED', 'SIMPLE_ENS_WEIGHTED']]
+        valid_keys = [m for m in MODEL_TYPES.keys() if m not in ["ENS_WEIGHTED", "SIMPLE_ENS_WEIGHTED"]]
         if not isinstance(models, list):
             models = [models]
         for model in models:
-            assert model in valid_keys, f'{model} is not one of the valid models {valid_keys}'
-        self.config['excluded_model_types'] = sorted(list(set(models)))
+            assert model in valid_keys, f"{model} is not one of the valid models {valid_keys}"
+        self.config["excluded_model_types"] = sorted(list(set(models)))
         return self
 
     def included_model_types(self, models: Union[str, list]) -> ConfigBuilder:
         """
         Subset of model types to train during `fit()`.
         Reference `hyperparameters` documentation for what models correspond to each value.
         Useful when only the particular models should be trained such as 'KNN' or 'custom', but altering the `hyperparameters` dictionary is difficult or time-consuming.
             Example: To keep only 'KNN' and 'custom' models, specify `included_model_types=['KNN', 'custom']`.
         """
-        valid_keys = [m for m in MODEL_TYPES.keys() if m not in ['ENS_WEIGHTED', 'SIMPLE_ENS_WEIGHTED']]
+        valid_keys = [m for m in MODEL_TYPES.keys() if m not in ["ENS_WEIGHTED", "SIMPLE_ENS_WEIGHTED"]]
         if not isinstance(models, list):
             models = [models]
 
         unknown_keys = [k for k in models if isinstance(k, str) and (k not in valid_keys)]
-        assert len(unknown_keys) == 0, f'The following model types are not recognized: {unknown_keys} - use one of the valid models: {valid_keys}'
+        assert len(unknown_keys) == 0, f"The following model types are not recognized: {unknown_keys} - use one of the valid models: {valid_keys}"
 
         models = [m for m in valid_keys if m not in models]
-        self.config['excluded_model_types'] = models
+        self.config["excluded_model_types"] = models
         return self
 
     def refit_full(self, refit_full: Union[bool, str] = True) -> ConfigBuilder:
         """
         Whether to retrain all models on all of the data (training + validation) after the normal training procedure.
         This is equivalent to calling `predictor.refit_full(model=refit_full)` after fit.
         If `refit_full=True`, it will be treated as `refit_full='all'`.
         If `refit_full=False`, refitting will not occur.
         Valid str values:
             `all`: refits all models.
             `best`: refits only the best model (and its ancestors if it is a stacker model).
             `{model_name}`: refits only the specified model (and its ancestors if it is a stacker model).
         """
-        self.config['refit_full'] = refit_full
+        self.config["refit_full"] = refit_full
         return self
 
     def set_best_to_refit_full(self, set_best_to_refit_full=True) -> ConfigBuilder:
         """
         If True, will change the default model that Predictor uses for prediction when model is not specified to the refit_full version of the model that exhibited the highest validation score.
         Only valid if `refit_full` is set.
         """
-        self.config['set_best_to_refit_full'] = set_best_to_refit_full
+        self.config["set_best_to_refit_full"] = set_best_to_refit_full
         return self
 
     def keep_only_best(self, keep_only_best=True) -> ConfigBuilder:
         """
         If True, only the best model and its ancestor models are saved in the outputted `predictor`. All other models are deleted.
             If you only care about deploying the most accurate predictor with the smallest file-size and no longer need any of the other trained models or functionality beyond prediction on new data, then set: `keep_only_best=True`, `save_space=True`.
             This is equivalent to calling `predictor.delete_models(models_to_keep='best', dry_run=False)` directly after `fit()`.
         If used with `refit_full` and `set_best_to_refit_full`, the best model will be the refit_full model, and the original bagged best model will be deleted.
             `refit_full` will be automatically set to 'best' in this case to avoid training models which will be later deleted.
         """
-        self.config['keep_only_best'] = keep_only_best
+        self.config["keep_only_best"] = keep_only_best
         return self
 
     def save_space(self, save_space=True) -> ConfigBuilder:
         """
         If True, reduces the memory and disk size of predictor by deleting auxiliary model files that aren't needed for prediction on new data.
             This is equivalent to calling `predictor.save_space()` directly after `fit()`.
         This has NO impact on inference accuracy.
         It is recommended if the only goal is to use the trained model for prediction.
         Certain advanced functionality may no longer be available if `save_space=True`. Refer to `predictor.save_space()` documentation for more details.
         """
-        self.config['save_space'] = save_space
+        self.config["save_space"] = save_space
         return self
 
     def feature_generator(self) -> FeatureGeneratorBuilder:
         """
         The feature generator used by AutoGluon to process the input data to the form sent to the models. This often includes automated feature generation and data cleaning.
         It is generally recommended to keep the default feature generator unless handling an advanced use-case.
         """
@@ -351,15 +350,15 @@
     def calibrate(self, calibrate=True) -> ConfigBuilder:
         """
         If True and the problem_type is classification, temperature scaling will be used to calibrate the Predictor's estimated class probabilities
         (which may improve metrics like log_loss) and will train a scalar parameter on the validation set.
         If True and the problem_type is quantile regression, conformalization will be used to calibrate the Predictor's estimated quantiles
         (which may improve the prediction interval coverage, and bagging could further improve it) and will compute a set of scalar parameters on the validation set.
         """
-        self.config['calibrate'] = calibrate
+        self.config["calibrate"] = calibrate
         return self
 
     def build(self) -> dict:
         """
         Build the config.
         """
         return copy.deepcopy(self.config)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-
 import copy
 
-from autogluon.features.generators import AutoMLPipelineFeatureGenerator, AutoMLInterpretablePipelineFeatureGenerator, IdentityFeatureGenerator
+from autogluon.features.generators import (
+    AutoMLInterpretablePipelineFeatureGenerator,
+    AutoMLPipelineFeatureGenerator,
+    IdentityFeatureGenerator,
+)
 
 
 def get_default_feature_generator(feature_generator, feature_metadata=None, init_kwargs=None):
     if init_kwargs is None:
         init_kwargs = dict()
     if feature_generator is None:
         feature_generator = IdentityFeatureGenerator()
     elif isinstance(feature_generator, str):
-        if feature_generator == 'auto':
+        if feature_generator == "auto":
             feature_generator = AutoMLPipelineFeatureGenerator(**init_kwargs)
-        elif feature_generator == 'interpretable':
+        elif feature_generator == "interpretable":
             feature_generator = AutoMLInterpretablePipelineFeatureGenerator(**init_kwargs)
         else:
             raise ValueError(f"Unknown feature_generator preset: '{feature_generator}', valid presets: {['auto', 'interpretable']}")
     if feature_metadata is not None:
         if feature_generator.feature_metadata_in is None and not feature_generator.is_fit():
             feature_generator.feature_metadata_in = copy.deepcopy(feature_metadata)
         else:
-            raise AssertionError('`feature_metadata_in` already exists in `feature_generator`.')
+            raise AssertionError("`feature_metadata_in` already exists in `feature_generator`.")
     return feature_generator
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/configs/presets_configs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,68 @@
-
 # Dictionary of preset fit() parameter configurations.
 tabular_presets_dict = dict(
     # Best predictive accuracy with little consideration to inference time or disk usage. Achieve even better results by specifying a large time_limit value.
     # Recommended for applications that benefit from the best possible model accuracy.
     # Aliases: best
-    best_quality={'auto_stack': True},
-
+    best_quality={"auto_stack": True},
     # High predictive accuracy with fast inference. ~10x-200x faster inference and ~10x-200x lower disk usage than `best_quality`.
     # Recommended for applications that require reasonable inference speed and/or model size.
     # Aliases: high, high_quality_fast_inference_only_refit
-    high_quality={'auto_stack': True, 'refit_full': True, 'set_best_to_refit_full': True, '_save_bag_folds': False},
-
+    high_quality={"auto_stack": True, "refit_full": True, "set_best_to_refit_full": True, "_save_bag_folds": False},
     # Good predictive accuracy with very fast inference. ~4x faster inference and ~4x lower disk usage than `high_quality`.
     # Recommended for applications that require fast inference speed.
     # Aliases: good, good_quality_faster_inference_only_refit
-    good_quality={'auto_stack': True, 'refit_full': True, 'set_best_to_refit_full': True, '_save_bag_folds': False, 'hyperparameters': 'light'},
-
+    good_quality={"auto_stack": True, "refit_full": True, "set_best_to_refit_full": True, "_save_bag_folds": False, "hyperparameters": "light"},
     # Medium predictive accuracy with very fast inference and very fast training time. ~20x faster training than `good_quality`.
     # This is the default preset in AutoGluon, but should generally only be used for quick prototyping, as `good_quality` results in significantly better predictive accuracy and faster inference time.
     # Aliases: medium, medium_quality_faster_train
-    medium_quality={'auto_stack': False},
-
+    medium_quality={"auto_stack": False},
     # Optimizes result immediately for deployment by deleting unused models and removing training artifacts.
     # Often can reduce disk usage by ~2-4x with no negatives to model accuracy or inference speed.
     # This will disable numerous advanced functionality, but has no impact on inference.
     # Recommended for applications where the inner details of AutoGluon's training is not important and there is no intention of manually choosing between the final models.
     # This preset pairs well with the other presets such as `good_quality` to make a very compact final model.
     # Identical to calling `predictor.delete_models(models_to_keep='best', dry_run=False)` and `predictor.save_space()` directly after `fit()`.
-    optimize_for_deployment={'keep_only_best': True, 'save_space': True},
-
+    optimize_for_deployment={"keep_only_best": True, "save_space": True},
     # Disables automated feature generation when text features are detected.
     # This is useful to determine how beneficial text features are to the end result, as well as to ensure features are not mistaken for text when they are not.
-    ignore_text={'_feature_generator_kwargs': {'enable_text_ngram_features': False, 'enable_text_special_features': False, 'enable_raw_text_features': False}},
-
+    ignore_text={"_feature_generator_kwargs": {"enable_text_ngram_features": False, "enable_text_special_features": False, "enable_raw_text_features": False}},
     # Fit only interpretable models.
     interpretable={
-        'auto_stack': False,
-        'hyperparameters': 'interpretable',
-        'feature_generator': 'interpretable',
-        'fit_weighted_ensemble': False,
-        'calibrate': False,
+        "auto_stack": False,
+        "hyperparameters": "interpretable",
+        "feature_generator": "interpretable",
+        "fit_weighted_ensemble": False,
+        "calibrate": False,
     },
-
     # ------------------------------------------
     # ------------------------------------------
     # ------------------------------------------
     # Experimental presets. Only use these presets if you are ok with unstable and potentially poor performing presets.
     #  Experimental presets can be removed or changed without warning.
-
     # Best quality with an additional FTTransformer model, GPU is recommended.
-    experimental_best_quality={'auto_stack': True, 'hyperparameters': 'default_FTT'},
-
+    experimental_best_quality={"auto_stack": True, "hyperparameters": "default_FTT"},
     # Best quality with an additional FTTransformer and TabPFN model, GPU is recommended.
     #  May have **extremely** slow inference speed, to a potentially unusable degree.
-    experimental_extreme_quality={'auto_stack': True, 'hyperparameters': 'extreme'},
-
+    experimental_extreme_quality={"auto_stack": True, "hyperparameters": "extreme"},
     # Experimental simulated model portfolio.
     # Shown to achieve superior results compared to best_quality on OpenML datasets <5000 rows.
     # Note that runtimes might be much longer than usual with this config.
-    experimental_zeroshot_hpo={'auto_stack': True, 'hyperparameters': 'zeroshot_hpo'},
-    experimental_zeroshot_hpo_hybrid={'auto_stack': True, 'hyperparameters': 'zeroshot_hpo_hybrid'},
-
+    experimental_zeroshot_hpo={"auto_stack": True, "hyperparameters": "zeroshot_hpo"},
+    experimental_zeroshot_hpo_hybrid={"auto_stack": True, "hyperparameters": "zeroshot_hpo_hybrid"},
     # ------------------------------------------
     # ------------------------------------------
     # ------------------------------------------
-
     # TODO: Consider HPO-enabled configs if training time doesn't matter but inference latency does.
 )
 
 
 # Alias preset name alternatives
 tabular_presets_alias = dict(
-    best='best_quality',
-    high='high_quality',
-    high_quality_fast_inference_only_refit='high_quality',
-    good='good_quality',
-    good_quality_faster_inference_only_refit='good_quality',
-    medium='medium_quality',
-    medium_quality_faster_train='medium_quality',
+    best="best_quality",
+    high="high_quality",
+    high_quality_fast_inference_only_refit="high_quality",
+    good="good_quality",
+    good_quality_faster_inference_only_refit="good_quality",
+    medium="medium_quality",
+    medium_quality_faster_train="medium_quality",
 )
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,112 @@
 from __future__ import annotations
 
 import copy
 import json
 import logging
 import time
 from collections.abc import Iterable
+from typing import List, Union
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
-from typing import List, Union
 from sklearn.metrics import classification_report
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, AUTO_WEIGHT, BALANCE_WEIGHT
+from autogluon.core.constants import AUTO_WEIGHT, BALANCE_WEIGHT, BINARY, MULTICLASS, QUANTILE, REGRESSION
 from autogluon.core.data.label_cleaner import LabelCleaner, LabelCleanerMulticlassToBinary
 from autogluon.core.learner import AbstractLearner
-from autogluon.core.metrics import confusion_matrix, get_metric, Scorer
+from autogluon.core.metrics import Scorer, confusion_matrix, get_metric
 from autogluon.core.models.greedy_ensemble.ensemble_selection import EnsembleSelection
-from autogluon.core.utils import get_leaderboard_pareto_frontier, augment_rare_classes, extract_column, compute_weighted_metric
-from autogluon.core.utils import get_pred_from_proba, get_pred_from_proba_df, infer_problem_type
+from autogluon.core.utils import (
+    augment_rare_classes,
+    compute_weighted_metric,
+    extract_column,
+    get_leaderboard_pareto_frontier,
+    get_pred_from_proba,
+    get_pred_from_proba_df,
+    infer_problem_type,
+)
 from autogluon.features.generators import PipelineFeatureGenerator
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: - Semi-supervised learning
 # TODO: - Minimize memory usage of DataFrames (convert int64 -> uint8 when possible etc.)
 # Learner encompasses full problem, loading initial data, feature generation, model training, model prediction
 # TODO: Loading learner from S3 on Windows may cause issues due to os.path.sep
 class AbstractTabularLearner(AbstractLearner):
-
-    def __init__(self, path_context: str, label: str, feature_generator: PipelineFeatureGenerator,
-                 ignored_columns: list = None, label_count_threshold=10, problem_type=None, quantile_levels=None,
-                 eval_metric=None, positive_class=None, cache_data=True, is_trainer_present=False, random_state=0,
-                 sample_weight=None, weight_evaluation=False, groups=None):
+    def __init__(
+        self,
+        path_context: str,
+        label: str,
+        feature_generator: PipelineFeatureGenerator,
+        ignored_columns: list = None,
+        label_count_threshold=10,
+        problem_type=None,
+        quantile_levels=None,
+        eval_metric=None,
+        positive_class=None,
+        cache_data=True,
+        is_trainer_present=False,
+        random_state=0,
+        sample_weight=None,
+        weight_evaluation=False,
+        groups=None,
+    ):
         super().__init__(path_context=path_context, random_state=random_state)
         self.label = label
         self.ignored_columns = ignored_columns
         if self.ignored_columns is None:
             self.ignored_columns = []
         self.threshold = label_count_threshold
         self.problem_type = problem_type
-        self.eval_metric = get_metric(eval_metric, self.problem_type, 'eval_metric')
+        self.eval_metric = get_metric(eval_metric, self.problem_type, "eval_metric")
 
         if self.problem_type == QUANTILE and quantile_levels is None:
             raise ValueError("if `problem_type='quantile'`, `quantile_levels` has to be specified")
         if isinstance(quantile_levels, float):
             quantile_levels = [quantile_levels]
         if isinstance(quantile_levels, Iterable):
             for quantile in quantile_levels:
                 if quantile <= 0.0 or quantile >= 1.0:
-                    raise ValueError("quantile values have to be non-negative and less than 1.0 (0.0 < q < 1.0). "
-                                     "For example, 0.95 quantile = 95 percentile")
+                    raise ValueError("quantile values have to be non-negative and less than 1.0 (0.0 < q < 1.0). " "For example, 0.95 quantile = 95 percentile")
             quantile_levels = np.sort(np.array(quantile_levels))
         self.quantile_levels = quantile_levels
 
         self.cache_data = cache_data
         if not self.cache_data:
-            logger.log(30, 'Warning: `cache_data=False` will disable or limit advanced functionality after training such as feature importance calculations. It is recommended to set `cache_data=True` unless you explicitly wish to not have the data saved to disk.')
+            logger.log(
+                30,
+                "Warning: `cache_data=False` will disable or limit advanced functionality after training such as feature importance calculations. It is recommended to set `cache_data=True` unless you explicitly wish to not have the data saved to disk.",
+            )
         self.is_trainer_present = is_trainer_present
 
         self.cleaner = None
         self.label_cleaner: LabelCleaner = None
         self.feature_generator: PipelineFeatureGenerator = feature_generator
 
         self._original_features = None
         self._pre_X_rows = None
         self._post_X_rows = None
         self._positive_class = positive_class
         self.sample_weight = sample_weight
         self.weight_evaluation = weight_evaluation
         self.groups = groups
         if sample_weight is not None and not isinstance(sample_weight, str):
-            raise ValueError("sample_weight must be a string indicating the name of the column that contains sample weights. If you have a vector of sample weights, first add these as an extra column to your data.")
+            raise ValueError(
+                "sample_weight must be a string indicating the name of the column that contains sample weights. If you have a vector of sample weights, first add these as an extra column to your data."
+            )
         if weight_evaluation and sample_weight is None:
             raise ValueError("Must specify sample_weight column if you specify weight_evaluation=True")
         if groups is not None and not isinstance(groups, str):
-            raise ValueError('groups must be a string indicating the name of the column that contains the split groups. If you have a vector of split groups, first add these as an extra column to your data.')
+            raise ValueError(
+                "groups must be a string indicating the name of the column that contains the split groups. If you have a vector of split groups, first add these as an extra column to your data."
+            )
 
     @property
     def original_features(self) -> List[str]:
         """Original features user passed in before autogluon doing any processing"""
         return self._original_features
 
     # TODO: Possibly rename to features_in or consider refactoring all feature_generators features_in -> features
@@ -114,72 +140,81 @@
         Returns
         -------
         The positive class name in binary classification or None if the problem is not binary classification.
         """
         if not self.is_fit:
             if self._positive_class is not None:
                 return self._positive_class
-            raise AssertionError('Predictor must be fit to return positive_class.')
+            raise AssertionError("Predictor must be fit to return positive_class.")
         if self.problem_type != BINARY:
-            logger.warning(f"Warning: Attempted to retrieve positive class label in a non-binary problem. Positive class labels only exist in binary classification. Returning None instead. self.problem_type is '{self.problem_type}' but positive_class only exists for '{BINARY}'.")
+            logger.warning(
+                f"Warning: Attempted to retrieve positive class label in a non-binary problem. Positive class labels only exist in binary classification. Returning None instead. self.problem_type is '{self.problem_type}' but positive_class only exists for '{BINARY}'."
+            )
             return None
         return self.label_cleaner.cat_mappings_dependent_var[1]
 
     def fit(self, X: DataFrame, X_val: DataFrame = None, **kwargs):
         if self.is_fit:
-            raise AssertionError('Learner is already fit.')
+            raise AssertionError("Learner is already fit.")
         self._validate_fit_input(X=X, X_val=X_val, **kwargs)
         return self._fit(X=X, X_val=X_val, **kwargs)
 
-    def _fit(self, X: DataFrame, X_val: DataFrame = None, scheduler_options=None, hyperparameter_tune=False,
-             feature_prune=False, holdout_frac=0.1, hyperparameters=None, verbosity=2):
+    def _fit(
+        self,
+        X: DataFrame,
+        X_val: DataFrame = None,
+        scheduler_options=None,
+        hyperparameter_tune=False,
+        feature_prune=False,
+        holdout_frac=0.1,
+        hyperparameters=None,
+        verbosity=2,
+    ):
         raise NotImplementedError
 
-    def predict_proba(self,
-                      X: DataFrame,
-                      model: str | None = None,
-                      as_pandas: bool = True,
-                      as_multiclass: bool = True,
-                      inverse_transform: bool = True,
-                      transform_features: bool = True):
+    def predict_proba(
+        self,
+        X: DataFrame,
+        model: str | None = None,
+        as_pandas: bool = True,
+        as_multiclass: bool = True,
+        inverse_transform: bool = True,
+        transform_features: bool = True,
+    ):
         X_index = copy.deepcopy(X.index) if as_pandas else None
         if X.empty:
             y_pred_proba = np.array([])
         else:
             if transform_features:
                 X = self.transform_features(X)
             y_pred_proba = self.load_trainer().predict_proba(X, model=model)
-        y_pred_proba = self._post_process_predict_proba(y_pred_proba=y_pred_proba,
-                                                        as_pandas=as_pandas,
-                                                        index=X_index,
-                                                        as_multiclass=as_multiclass,
-                                                        inverse_transform=inverse_transform)
+        y_pred_proba = self._post_process_predict_proba(
+            y_pred_proba=y_pred_proba, as_pandas=as_pandas, index=X_index, as_multiclass=as_multiclass, inverse_transform=inverse_transform
+        )
         return y_pred_proba
 
-    def predict(self,
-                X: DataFrame,
-                model: str | None = None,
-                as_pandas: bool = True,
-                inverse_transform: bool = True,
-                transform_features: bool = True,
-                *,
-                decision_threshold: float | None = None,
-                ):
+    def predict(
+        self,
+        X: DataFrame,
+        model: str | None = None,
+        as_pandas: bool = True,
+        inverse_transform: bool = True,
+        transform_features: bool = True,
+        *,
+        decision_threshold: float | None = None,
+    ):
         if decision_threshold is None:
             decision_threshold = 0.5
         X_index = copy.deepcopy(X.index) if as_pandas else None
-        y_pred_proba = self.predict_proba(X=X, model=model, as_pandas=False, as_multiclass=False, inverse_transform=False, transform_features=transform_features)
+        y_pred_proba = self.predict_proba(
+            X=X, model=model, as_pandas=False, as_multiclass=False, inverse_transform=False, transform_features=transform_features
+        )
         problem_type = self.label_cleaner.problem_type_transform or self.problem_type
-        y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba,
-                                     problem_type=problem_type,
-                                     decision_threshold=decision_threshold)
-        y_pred = self._post_process_predict(y_pred=y_pred,
-                                            as_pandas=as_pandas,
-                                            index=X_index,
-                                            inverse_transform=inverse_transform)
+        y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=problem_type, decision_threshold=decision_threshold)
+        y_pred = self._post_process_predict(y_pred=y_pred, as_pandas=as_pandas, index=X_index, inverse_transform=inverse_transform)
         return y_pred
 
     def _post_process_predict(
         self,
         y_pred: np.ndarray,
         as_pandas: bool = True,
         index=None,
@@ -200,20 +235,15 @@
                 y_pred = y_pred.values
         else:
             if as_pandas:
                 y_pred = pd.DataFrame(data=y_pred, columns=self.quantile_levels, index=index)
         return y_pred
 
     def _post_process_predict_proba(
-        self,
-        y_pred_proba: np.ndarray,
-        as_pandas: bool = True,
-        index=None,
-        as_multiclass: bool = True,
-        inverse_transform: bool = True
+        self, y_pred_proba: np.ndarray, as_pandas: bool = True, index=None, as_multiclass: bool = True, inverse_transform: bool = True
     ):
         """
         Given internal prediction probabilities, post-process them to vend to user.
         """
         if inverse_transform:
             y_pred_proba = self.label_cleaner.inverse_transform_proba(y_pred_proba)
         if as_multiclass and (self.problem_type == BINARY):
@@ -224,22 +254,23 @@
                 y_pred_proba = pd.DataFrame(data=y_pred_proba, columns=classes, index=index)
             elif self.problem_type == QUANTILE:
                 y_pred_proba = pd.DataFrame(data=y_pred_proba, columns=self.quantile_levels, index=index)
             else:
                 y_pred_proba = pd.Series(data=y_pred_proba, name=self.label, index=index)
         return y_pred_proba
 
-    def predict_proba_multi(self,
-                            X: DataFrame = None,
-                            models: List[str] = None,
-                            as_pandas: bool = True,
-                            as_multiclass: bool = True,
-                            transform_features: bool = True,
-                            inverse_transform: bool = True,
-                            ) -> dict:
+    def predict_proba_multi(
+        self,
+        X: DataFrame = None,
+        models: List[str] = None,
+        as_pandas: bool = True,
+        as_multiclass: bool = True,
+        transform_features: bool = True,
+        inverse_transform: bool = True,
+    ) -> dict:
         """
         Returns a dictionary of prediction probabilities where the key is
         the model name and the value is the model's prediction probabilities on the data.
 
         Note that this will generally be much faster than calling `self.predict_proba` separately for each model
         because this method leverages the model dependency graph to avoid redundant computation.
 
@@ -296,66 +327,56 @@
                 X_index = copy.deepcopy(X.index) if as_pandas else None
                 predict_proba_dict = dict()
                 for m in models:
                     predict_proba_dict[m] = trainer.get_model_oof(m)
 
         # Inverse Transform labels
         for m, pred_proba in predict_proba_dict.items():
-            predict_proba_dict[m] = self._post_process_predict_proba(y_pred_proba=pred_proba,
-                                                                     as_pandas=as_pandas,
-                                                                     as_multiclass=as_multiclass,
-                                                                     index=X_index,
-                                                                     inverse_transform=inverse_transform)
+            predict_proba_dict[m] = self._post_process_predict_proba(
+                y_pred_proba=pred_proba, as_pandas=as_pandas, as_multiclass=as_multiclass, index=X_index, inverse_transform=inverse_transform
+            )
         return predict_proba_dict
 
-    def predict_multi(self,
-                      X: DataFrame = None,
-                      models: List[str] = None,
-                      as_pandas: bool = True,
-                      transform_features: bool = True,
-                      inverse_transform: bool = True,
-                      *,
-                      decision_threshold: float = None) -> dict:
+    def predict_multi(
+        self,
+        X: DataFrame = None,
+        models: List[str] = None,
+        as_pandas: bool = True,
+        transform_features: bool = True,
+        inverse_transform: bool = True,
+        *,
+        decision_threshold: float = None,
+    ) -> dict:
         """
         Identical to predict_proba_multi, except returns predictions instead of probabilities.
         """
-        predict_proba_dict = self.predict_proba_multi(X=X,
-                                                      models=models,
-                                                      as_pandas=as_pandas,
-                                                      transform_features=transform_features,
-                                                      inverse_transform=inverse_transform)
+        predict_proba_dict = self.predict_proba_multi(
+            X=X, models=models, as_pandas=as_pandas, transform_features=transform_features, inverse_transform=inverse_transform
+        )
         predict_dict = {}
         for m in predict_proba_dict:
-            predict_dict[m] = self.get_pred_from_proba(y_pred_proba=predict_proba_dict[m],
-                                                       decision_threshold=decision_threshold,
-                                                       inverse_transform=inverse_transform)
+            predict_dict[m] = self.get_pred_from_proba(
+                y_pred_proba=predict_proba_dict[m], decision_threshold=decision_threshold, inverse_transform=inverse_transform
+            )
         return predict_dict
 
-    def get_pred_from_proba(self,
-                            y_pred_proba: np.ndarray | pd.DataFrame,
-                            decision_threshold: float | None = None,
-                            inverse_transform: bool = True) -> np.array | pd.Series:
+    def get_pred_from_proba(
+        self, y_pred_proba: np.ndarray | pd.DataFrame, decision_threshold: float | None = None, inverse_transform: bool = True
+    ) -> np.array | pd.Series:
         if isinstance(y_pred_proba, pd.DataFrame):
-            y_pred = get_pred_from_proba_df(y_pred_proba,
-                                            problem_type=self.problem_type,
-                                            decision_threshold=decision_threshold)
-        else:
-            y_pred = get_pred_from_proba(y_pred_proba,
-                                         problem_type=self.problem_type,
-                                         decision_threshold=decision_threshold)
-            y_pred = self._post_process_predict(y_pred=y_pred,
-                                                as_pandas=False,
-                                                index=None,
-                                                inverse_transform=inverse_transform)
+            y_pred = get_pred_from_proba_df(y_pred_proba, problem_type=self.problem_type, decision_threshold=decision_threshold)
+        else:
+            y_pred = get_pred_from_proba(y_pred_proba, problem_type=self.problem_type, decision_threshold=decision_threshold)
+            y_pred = self._post_process_predict(y_pred=y_pred, as_pandas=False, index=None, inverse_transform=inverse_transform)
         return y_pred
 
     def _validate_fit_input(self, X: DataFrame, **kwargs):
         if self.label not in X.columns:
             raise KeyError(f"Label column '{self.label}' is missing from training data. Training data columns: {list(X.columns)}")
-        X_val = kwargs.get('X_val', None)
+        X_val = kwargs.get("X_val", None)
         self._validate_sample_weight(X, X_val)
         self._validate_groups(X, X_val)
 
     def _validate_sample_weight(self, X, X_val):
         if self.sample_weight is not None:
             if self.sample_weight in [AUTO_WEIGHT, BALANCE_WEIGHT]:
                 prefix = f"Using predefined sample weighting strategy: {self.sample_weight}."
@@ -363,42 +384,45 @@
                     prefix += " Warning: We do not recommend weight_evaluation=True with predefined sample weighting."
             else:
                 if self.sample_weight not in X.columns:
                     raise KeyError(f"sample_weight column '{self.sample_weight}' is missing from training data. Training data columns: {list(X.columns)}")
                 weight_vals = X[self.sample_weight]
                 if weight_vals.isna().sum() > 0:
                     raise ValueError(f"Sample weights in column '{self.sample_weight}' cannot be nan")
-                if weight_vals.dtype.kind not in 'biuf':
+                if weight_vals.dtype.kind not in "biuf":
                     raise ValueError(f"Sample weights in column '{self.sample_weight}' must be numeric values")
                 if weight_vals.min() < 0:
                     raise ValueError(f"Sample weights in column '{self.sample_weight}' must be nonnegative")
                 if self.weight_evaluation and X_val is not None and self.sample_weight not in X_val.columns:
                     raise KeyError(f"sample_weight column '{self.sample_weight}' cannot be missing from validation data if weight_evaluation=True")
                 prefix = f"Values in column '{self.sample_weight}' used as sample weights instead of predictive features."
             if self.weight_evaluation:
                 suffix = " Evaluation will report weighted metrics, so ensure same column exists in test data."
             else:
                 suffix = " Evaluation metrics will ignore sample weights, specify weight_evaluation=True to instead report weighted metrics."
-            logger.log(20, prefix+suffix)
+            logger.log(20, prefix + suffix)
 
     def _validate_groups(self, X, X_val):
         if self.groups is not None:
             if self.groups not in X.columns:
                 raise KeyError(f"groups column '{self.groups}' is missing from training data. Training data columns: {list(X.columns)}")
             groups_vals = X[self.groups]
             if len(groups_vals.unique()) < 2:
                 raise ValueError(f"Groups in column '{self.groups}' cannot have fewer than 2 unique values. Values: {list(groups_vals.unique())}")
             if X_val is not None and self.groups in X_val.columns:
                 raise KeyError(f"groups column '{self.groups}' cannot be in validation data. Validation data columns: {list(X_val.columns)}")
-            logger.log(20, f"Values in column '{self.groups}' used as split folds instead of being automatically set. Bagged models will have {len(groups_vals.unique())} splits.")
+            logger.log(
+                20,
+                f"Values in column '{self.groups}' used as split folds instead of being automatically set. Bagged models will have {len(groups_vals.unique())} splits.",
+            )
 
     def get_inputs_to_stacker(self, dataset=None, model=None, base_models: list = None, use_orig_features=True):
         if model is not None or base_models is not None:
             if model is not None and base_models is not None:
-                raise AssertionError('Only one of `model`, `base_models` is allowed to be set.')
+                raise AssertionError("Only one of `model`, `base_models` is allowed to be set.")
 
         trainer = self.load_trainer()
         if dataset is None:
             if trainer.bagged_mode:
                 dataset_preprocessed = trainer.load_X()
                 fit = True
             else:
@@ -416,23 +440,23 @@
             # dataset_preprocessed = trainer.get_inputs_to_model(model=model_to_get_inputs_for, X=dataset_preprocessed, fit=fit)
 
         return dataset_preprocessed
 
     # Fits _FULL models and links them in the stack so _FULL models only use other _FULL models as input during stacking
     # If model is specified, will fit all _FULL models that are ancestors of the provided model, automatically linking them.
     # If no model is specified, all models are refit and linked appropriately.
-    def refit_ensemble_full(self, model='all'):
+    def refit_ensemble_full(self, model="all"):
         return self.load_trainer().refit_ensemble_full(model=model)
 
     def fit_transform_features(self, X, y=None, **kwargs):
         if self.label in X:
             X = X.drop(columns=[self.label])
         if self.ignored_columns:
-            logger.log(20, f'Dropping user-specified ignored columns: {self.ignored_columns}')
-            X = X.drop(columns=self.ignored_columns, errors='ignore')
+            logger.log(20, f"Dropping user-specified ignored columns: {self.ignored_columns}")
+            X = X.drop(columns=self.ignored_columns, errors="ignore")
         for feature_generator in self.feature_generators:
             X = feature_generator.fit_transform(X, y, **kwargs)
         return X
 
     def transform_features(self, X):
         for feature_generator in self.feature_generators:
             X = feature_generator.transform(X)
@@ -455,16 +479,17 @@
             y_pred = self.predict(X=X, model=model, as_pandas=False)
         else:
             y_pred = self.predict_proba(X=X, model=model, as_pandas=False, as_multiclass=False)
             y = self.label_cleaner.transform(y)
         return compute_weighted_metric(y, y_pred, self.eval_metric, w, weight_evaluation=self.weight_evaluation, quantile_levels=self.quantile_levels)
 
     # Scores both learner and all individual models, along with computing the optimal ensemble score + weights (oracle)
-    def score_debug(self, X: DataFrame, y=None, extra_info=False, compute_oracle=False, extra_metrics=None,
-                    decision_threshold=None, skip_score=False, silent=False):
+    def score_debug(
+        self, X: DataFrame, y=None, extra_info=False, compute_oracle=False, extra_metrics=None, decision_threshold=None, skip_score=False, silent=False
+    ):
         leaderboard_df = self.leaderboard(extra_info=extra_info, silent=silent)
         if extra_metrics is None:
             extra_metrics = []
         if y is None:
             error_if_missing = extra_metrics or not skip_score
             X, y = self.extract_label(X, error_if_missing=error_if_missing)
         w = None
@@ -484,61 +509,53 @@
         all_trained_models = trainer.get_model_names()
         all_trained_models_can_infer = trainer.get_model_names(can_infer=True)
         all_trained_models_original = all_trained_models.copy()
         model_pred_proba_dict, pred_time_test_marginal = trainer.get_model_pred_proba_dict(X=X, models=all_trained_models_can_infer, record_pred_time=True)
 
         if compute_oracle:
             pred_probas = list(model_pred_proba_dict.values())
-            ensemble_selection = EnsembleSelection(ensemble_size=100, problem_type=trainer.problem_type, metric=self.eval_metric, quantile_levels=self.quantile_levels)
+            ensemble_selection = EnsembleSelection(
+                ensemble_size=100, problem_type=trainer.problem_type, metric=self.eval_metric, quantile_levels=self.quantile_levels
+            )
             ensemble_selection.fit(predictions=pred_probas, labels=y_internal, identifiers=None, sample_weight=w)  # TODO: Only fit non-nan
 
             oracle_weights = ensemble_selection.weights_
             oracle_pred_time_start = time.time()
             oracle_pred_proba_norm = [pred * weight for pred, weight in zip(pred_probas, oracle_weights)]
             oracle_pred_proba_ensemble = np.sum(oracle_pred_proba_norm, axis=0)
             oracle_pred_time = time.time() - oracle_pred_time_start
-            model_pred_proba_dict['OracleEnsemble'] = oracle_pred_proba_ensemble
-            pred_time_test_marginal['OracleEnsemble'] = oracle_pred_time
-            all_trained_models.append('OracleEnsemble')
+            model_pred_proba_dict["OracleEnsemble"] = oracle_pred_proba_ensemble
+            pred_time_test_marginal["OracleEnsemble"] = oracle_pred_time
+            all_trained_models.append("OracleEnsemble")
 
-        scoring_args = dict(
-            y=y,
-            y_internal=y_internal,
-            sample_weight=w
-        )
+        scoring_args = dict(y=y, y_internal=y_internal, sample_weight=w)
 
         extra_scores = {}
         for model_name, y_pred_proba_internal in model_pred_proba_dict.items():
             if skip_score:
                 scores[model_name] = np.nan
             else:
                 scores[model_name] = self._score_with_pred_proba(
-                    y_pred_proba_internal=y_pred_proba_internal,
-                    metric=self.eval_metric,
-                    decision_threshold=decision_threshold,
-                    **scoring_args
+                    y_pred_proba_internal=y_pred_proba_internal, metric=self.eval_metric, decision_threshold=decision_threshold, **scoring_args
                 )
             for metric in extra_metrics:
-                metric = get_metric(metric, self.problem_type, 'leaderboard_metric')
+                metric = get_metric(metric, self.problem_type, "leaderboard_metric")
                 if metric.name not in extra_scores:
                     extra_scores[metric.name] = {}
                 extra_scores[metric.name][model_name] = self._score_with_pred_proba(
-                    y_pred_proba_internal=y_pred_proba_internal,
-                    metric=metric,
-                    decision_threshold=decision_threshold,
-                    **scoring_args
+                    y_pred_proba_internal=y_pred_proba_internal, metric=metric, decision_threshold=decision_threshold, **scoring_args
                 )
 
         if extra_scores:
             series = []
             for metric in extra_scores:
                 series.append(pd.Series(extra_scores[metric], name=metric))
             df_extra_scores = pd.concat(series, axis=1)
             extra_metrics_names = list(df_extra_scores.columns)
-            df_extra_scores['model'] = df_extra_scores.index
+            df_extra_scores["model"] = df_extra_scores.index
             df_extra_scores = df_extra_scores.reset_index(drop=True)
         else:
             df_extra_scores = None
             extra_metrics_names = None
 
         pred_time_test = {}
         # TODO: Add support for calculating pred_time_test_full for oracle_ensemble, need to copy graph from trainer and add oracle_ensemble to it with proper edges.
@@ -558,127 +575,116 @@
         scored_models = list(scores.keys())
         for model in all_trained_models:
             if model not in scored_models:
                 scores[model] = None
                 pred_time_test[model] = None
                 pred_time_test_marginal[model] = None
 
-        logger.debug('Model scores:')
+        logger.debug("Model scores:")
         logger.debug(str(scores))
         model_names_final = list(scores.keys())
         df = pd.DataFrame(
             data={
-                'model': model_names_final,
-                'score_test': list(scores.values()),
-                'pred_time_test': [pred_time_test[model] for model in model_names_final],
-                'pred_time_test_marginal': [pred_time_test_marginal[model] for model in model_names_final],
+                "model": model_names_final,
+                "score_test": list(scores.values()),
+                "pred_time_test": [pred_time_test[model] for model in model_names_final],
+                "pred_time_test_marginal": [pred_time_test_marginal[model] for model in model_names_final],
             }
         )
         if df_extra_scores is not None:
-            df = pd.merge(df, df_extra_scores, on='model', how='left')
+            df = pd.merge(df, df_extra_scores, on="model", how="left")
 
-        df_merged = pd.merge(df, leaderboard_df, on='model', how='left')
-        df_merged = df_merged.sort_values(by=['score_test', 'pred_time_test', 'score_val', 'pred_time_val', 'model'], ascending=[False, True, False, True, False]).reset_index(drop=True)
+        df_merged = pd.merge(df, leaderboard_df, on="model", how="left")
+        df_merged = df_merged.sort_values(
+            by=["score_test", "pred_time_test", "score_val", "pred_time_val", "model"], ascending=[False, True, False, True, False]
+        ).reset_index(drop=True)
         df_columns_lst = df_merged.columns.tolist()
         explicit_order = [
-            'model',
-            'score_test',
+            "model",
+            "score_test",
         ]
         if extra_metrics_names is not None:
             explicit_order += extra_metrics_names
         explicit_order += [
-            'score_val',
-            'pred_time_test',
-            'pred_time_val',
-            'fit_time',
-            'pred_time_test_marginal',
-            'pred_time_val_marginal',
-            'fit_time_marginal',
-            'stack_level',
-            'can_infer',
-            'fit_order',
+            "score_val",
+            "pred_time_test",
+            "pred_time_val",
+            "fit_time",
+            "pred_time_test_marginal",
+            "pred_time_val_marginal",
+            "fit_time_marginal",
+            "stack_level",
+            "can_infer",
+            "fit_order",
         ]
         df_columns_other = [column for column in df_columns_lst if column not in explicit_order]
         df_columns_new = explicit_order + df_columns_other
         df_merged = df_merged[df_columns_new]
 
         return df_merged
 
-    def _score_with_pred_proba(self,
-                               y,
-                               y_internal,
-                               y_pred_proba_internal,
-                               metric,
-                               sample_weight=None,
-                               decision_threshold=None,
-                               weight_evaluation=None):
-        metric = get_metric(metric, self.problem_type, 'leaderboard_metric')
+    def _score_with_pred_proba(self, y, y_internal, y_pred_proba_internal, metric, sample_weight=None, decision_threshold=None, weight_evaluation=None):
+        metric = get_metric(metric, self.problem_type, "leaderboard_metric")
         if weight_evaluation is None:
             weight_evaluation = self.weight_evaluation
         if metric.needs_pred:
             if self.problem_type == BINARY:
                 # Use 1 and 0, otherwise f1 can crash due to unknown pos_label.
-                y_pred = self.get_pred_from_proba(y_pred_proba_internal,
-                                                  decision_threshold=decision_threshold,
-                                                  inverse_transform=False)
+                y_pred = self.get_pred_from_proba(y_pred_proba_internal, decision_threshold=decision_threshold, inverse_transform=False)
                 y_tmp = y_internal
             else:
                 y_pred = self.label_cleaner.inverse_transform_proba(y_pred_proba_internal, as_pred=True)
                 y_tmp = y
         elif metric.needs_quantile:
             y_pred = self.label_cleaner.inverse_transform_proba(y_pred_proba_internal, as_pred=True)
             y_tmp = y
         else:
             y_pred = self.label_cleaner.inverse_transform_proba(y_pred_proba_internal, as_pred=False)
             y_tmp = y_internal
         return compute_weighted_metric(y_tmp, y_pred, metric, weights=sample_weight, weight_evaluation=weight_evaluation, quantile_levels=self.quantile_levels)
 
-    def _score_with_pred(self,
-                         y,
-                         y_internal,
-                         y_pred_internal,
-                         metric,
-                         sample_weight=None,
-                         weight_evaluation=None):
-        metric = get_metric(metric, self.problem_type, 'leaderboard_metric')
+    def _score_with_pred(self, y, y_internal, y_pred_internal, metric, sample_weight=None, weight_evaluation=None):
+        metric = get_metric(metric, self.problem_type, "leaderboard_metric")
         if weight_evaluation is None:
             weight_evaluation = self.weight_evaluation
         if self.problem_type == BINARY:
             # Use 1 and 0, otherwise f1 can crash due to unknown pos_label.
             y_pred = y_pred_internal
             y_tmp = y_internal
         else:
             y_pred = self.label_cleaner.inverse_transform(y_pred_internal)
             y_tmp = y
         return compute_weighted_metric(y_tmp, y_pred, metric, weights=sample_weight, weight_evaluation=weight_evaluation, quantile_levels=self.quantile_levels)
 
     def _validate_class_labels(self, y: Series):
         null_count = y.isnull().sum()
         if null_count:
-            raise ValueError(f'Labels cannot contain missing (nan) values. Found {null_count} missing label values.')
+            raise ValueError(f"Labels cannot contain missing (nan) values. Found {null_count} missing label values.")
         if self.problem_type == MULTICLASS and not self.eval_metric.needs_pred:
             y_unique = np.unique(y)
             valid_class_set = set(self.class_labels)
             unknown_classes = []
             for cls in y_unique:
                 if cls not in valid_class_set:
                     unknown_classes.append(cls)
             if unknown_classes:
                 # log_loss / pac_score
-                raise ValueError(f'Multiclass scoring with eval_metric=\'{self.eval_metric.name}\' does not support unknown classes. Unknown classes: {unknown_classes}')
+                raise ValueError(
+                    f"Multiclass scoring with eval_metric='{self.eval_metric.name}' does not support unknown classes. Unknown classes: {unknown_classes}"
+                )
 
     def evaluate_predictions(self, y_true, y_pred, sample_weight=None, decision_threshold=None, silent=False, auxiliary_metrics=True, detailed_report=False):
-        """ Evaluate predictions. Does not support sample weights since this method reports a variety of metrics.
-            Args:
-                silent (bool): Should we print which metric is being used as well as performance.
-                auxiliary_metrics (bool): Should we compute other (problem_type specific) metrics in addition to the default metric?
-                detailed_report (bool): Should we computed more-detailed versions of the auxiliary_metrics? (requires auxiliary_metrics=True).
+        """Evaluate predictions. Does not support sample weights since this method reports a variety of metrics.
+        Args:
+            silent (bool): Should we print which metric is being used as well as performance.
+            auxiliary_metrics (bool): Should we compute other (problem_type specific) metrics in addition to the default metric?
+            detailed_report (bool): Should we computed more-detailed versions of the auxiliary_metrics? (requires auxiliary_metrics=True).
 
-            Returns single performance-value if auxiliary_metrics=False.
-            Otherwise returns dict where keys = metrics, values = performance along each metric.
+        Returns single performance-value if auxiliary_metrics=False.
+        Otherwise returns dict where keys = metrics, values = performance along each metric.
         """
 
         is_proba = False
         assert isinstance(y_true, (np.ndarray, pd.Series))
         assert isinstance(y_pred, (np.ndarray, pd.Series, pd.DataFrame))
         self._validate_class_labels(y_true)
         if isinstance(y_pred, np.ndarray):
@@ -686,19 +692,21 @@
                 y_pred = pd.DataFrame(data=y_pred, columns=self.quantile_levels)
             elif len(y_pred.shape) > 1:
                 y_pred = pd.DataFrame(data=y_pred, columns=self.class_labels)
 
         if isinstance(y_pred, pd.DataFrame):
             is_proba = True
         elif not self.eval_metric.needs_pred:
-            raise AssertionError(f'`evaluate_predictions` requires y_pred_proba input '
-                                 f'when evaluating "{self.eval_metric.name}"... Please generate valid input via `predictor.predict_proba(data)`.\n'
-                                 f'This may have occurred if you passed in predict input instead of predict_proba input, '
-                                 f'or if you specified `as_multiclass=False` to `predictor.predict_proba(data, as_multiclass=False)`, '
-                                 f'which is not supported by `evaluate_predictions`.')
+            raise AssertionError(
+                f"`evaluate_predictions` requires y_pred_proba input "
+                f'when evaluating "{self.eval_metric.name}"... Please generate valid input via `predictor.predict_proba(data)`.\n'
+                f"This may have occurred if you passed in predict input instead of predict_proba input, "
+                f"or if you specified `as_multiclass=False` to `predictor.predict_proba(data, as_multiclass=False)`, "
+                f"which is not supported by `evaluate_predictions`."
+            )
         if is_proba:
             y_pred_proba = y_pred
             y_pred = self.get_pred_from_proba(y_pred_proba=y_pred_proba, decision_threshold=decision_threshold)
             if self.problem_type == BINARY:
                 # roc_auc crashes if this isn't done
                 y_pred_proba = y_pred_proba[self.positive_class]
         else:
@@ -715,87 +723,82 @@
         # Compute auxiliary metrics:
         auxiliary_metrics_lst = [self.eval_metric]
         performance_dict = {}
 
         if auxiliary_metrics:
             if self.problem_type == REGRESSION:  # Adding regression metrics
                 auxiliary_metrics_lst += [
-                    'root_mean_squared_error',
-                    'mean_squared_error',
-                    'mean_absolute_error',
-                    'r2',
-                    'pearsonr',
-                    'median_absolute_error',
+                    "root_mean_squared_error",
+                    "mean_squared_error",
+                    "mean_absolute_error",
+                    "r2",
+                    "pearsonr",
+                    "median_absolute_error",
                 ]
             if self.problem_type in [BINARY, MULTICLASS]:  # Adding classification metrics
                 auxiliary_metrics_lst += [
-                    'accuracy',
-                    'balanced_accuracy',
+                    "accuracy",
+                    "balanced_accuracy",
                     # 'log_loss',  # Don't include as it probably adds more confusion to novice users (can be infinite)
-                    'mcc',
+                    "mcc",
                 ]
             if self.problem_type == BINARY:  # binary-specific metrics
                 auxiliary_metrics_lst += [
-                    'roc_auc',
-                    'f1',
-                    'precision',
-                    'recall',
+                    "roc_auc",
+                    "f1",
+                    "precision",
+                    "recall",
                 ]
 
         scoring_args = dict(
             y=y_true,
             y_internal=y_true_internal,
             weight_evaluation=False,
         )
 
         if sample_weight is not None:
-            scoring_args['sample_weight'] = sample_weight
-            scoring_args['weight_evaluation'] = True
+            scoring_args["sample_weight"] = sample_weight
+            scoring_args["weight_evaluation"] = True
 
         for aux_metric in auxiliary_metrics_lst:
             if isinstance(aux_metric, str):
-                aux_metric = get_metric(metric=aux_metric, problem_type=self.problem_type, metric_type='aux_metric')
+                aux_metric = get_metric(metric=aux_metric, problem_type=self.problem_type, metric_type="aux_metric")
             if not aux_metric.needs_pred and y_pred_proba_internal is None:
-                logger.log(15, f'Skipping {aux_metric.name} because no prediction probabilities are available to score.')
+                logger.log(15, f"Skipping {aux_metric.name} because no prediction probabilities are available to score.")
                 continue
 
             if aux_metric.name not in performance_dict:
                 if y_pred_proba_internal is not None:
                     score = self._score_with_pred_proba(
-                        y_pred_proba_internal=y_pred_proba_internal,
-                        metric=aux_metric,
-                        decision_threshold=decision_threshold,
-                        **scoring_args
+                        y_pred_proba_internal=y_pred_proba_internal, metric=aux_metric, decision_threshold=decision_threshold, **scoring_args
                     )
                 else:
-                    score = self._score_with_pred(
-                        y_pred_internal=y_pred_internal,
-                        metric=aux_metric,
-                        **scoring_args
-                    )
+                    score = self._score_with_pred(y_pred_internal=y_pred_internal, metric=aux_metric, **scoring_args)
                 performance_dict[aux_metric.name] = score
 
         if not silent:
             if self.eval_metric.name in performance_dict:
                 score_eval = performance_dict[self.eval_metric.name]
                 logger.log(20, f"Evaluation: {self.eval_metric.name} on test data: {score_eval}")
                 if not self.eval_metric.greater_is_better_internal:
                     logger.log(20, f"\tNote: Scores are always higher_is_better. This metric score can be multiplied by -1 to get the metric value.")
             logger.log(20, "Evaluations on test data:")
             logger.log(20, json.dumps(performance_dict, indent=4))
 
         if detailed_report and (self.problem_type != REGRESSION):
             # Construct confusion matrix
             try:
-                performance_dict['confusion_matrix'] = confusion_matrix(y_true, y_pred, labels=self.label_cleaner.ordered_class_labels, output_format='pandas_dataframe')
+                performance_dict["confusion_matrix"] = confusion_matrix(
+                    y_true, y_pred, labels=self.label_cleaner.ordered_class_labels, output_format="pandas_dataframe"
+                )
             except ValueError:
                 pass
             # One final set of metrics to report
             cl_metric = lambda y_true, y_pred: classification_report(y_true, y_pred, output_dict=True)
-            metric_name = 'classification_report'
+            metric_name = "classification_report"
             if metric_name not in performance_dict:
                 try:  # only compute auxiliary metrics which do not error (y_pred = class-probabilities may cause some metrics to error)
                     performance_dict[metric_name] = cl_metric(y_true, y_pred)
                 except ValueError:
                     pass
                 if not silent and metric_name in performance_dict:
                     logger.log(20, "Detailed (per-class) classification report:")
@@ -808,112 +811,133 @@
                 raise ValueError(f"Provided DataFrame does not contain label column: {self.label}")
             else:
                 return X, None
         y = X[self.label].copy()
         X = X.drop(self.label, axis=1)
         return X, y
 
-    def leaderboard(self, X=None, y=None, extra_info=False, extra_metrics=None, decision_threshold=None,
-                    only_pareto_frontier=False, skip_score=False, silent=False) -> pd.DataFrame:
+    def leaderboard(
+        self, X=None, y=None, extra_info=False, extra_metrics=None, decision_threshold=None, only_pareto_frontier=False, skip_score=False, silent=False
+    ) -> pd.DataFrame:
         if X is not None:
-            leaderboard = self.score_debug(X=X, y=y, extra_info=extra_info, extra_metrics=extra_metrics,
-                                           decision_threshold=decision_threshold, skip_score=skip_score, silent=True)
+            leaderboard = self.score_debug(
+                X=X, y=y, extra_info=extra_info, extra_metrics=extra_metrics, decision_threshold=decision_threshold, skip_score=skip_score, silent=True
+            )
         else:
             if extra_metrics:
-                raise AssertionError('`extra_metrics` is only valid when data is specified.')
+                raise AssertionError("`extra_metrics` is only valid when data is specified.")
             trainer = self.load_trainer()
             leaderboard = trainer.leaderboard(extra_info=extra_info)
         if only_pareto_frontier:
-            if 'score_test' in leaderboard.columns and 'pred_time_test' in leaderboard.columns:
-                score_col = 'score_test'
-                inference_time_col = 'pred_time_test'
+            if "score_test" in leaderboard.columns and "pred_time_test" in leaderboard.columns:
+                score_col = "score_test"
+                inference_time_col = "pred_time_test"
             else:
-                score_col = 'score_val'
-                inference_time_col = 'pred_time_val'
+                score_col = "score_val"
+                inference_time_col = "pred_time_val"
             leaderboard = get_leaderboard_pareto_frontier(leaderboard=leaderboard, score_col=score_col, inference_time_col=inference_time_col)
         if not silent:
-            with pd.option_context('display.max_rows', None, 'display.max_columns', None, 'display.width', 1000):
+            with pd.option_context("display.max_rows", None, "display.max_columns", None, "display.width", 1000):
                 print(leaderboard)
         return leaderboard
 
     # TODO: cache_data must be set to True to be able to pass X and y as None in this function, otherwise it will error.
     # Warning: This can take a very, very long time to compute if the data is large and the model is complex.
     # A value of 0.01 means that the objective metric error would be expected to increase by 0.01 if the feature were removed.
     # Negative values mean the feature is likely harmful.
     # model: model (str) to get feature importances for, if None will choose best model.
     # features: list of feature names that feature importances are calculated for and returned, specify None to get all feature importances.
     # feature_stage: Whether to compute feature importance on raw original features ('original'), transformed features ('transformed') or on the features used by the particular model ('transformed_model').
-    def get_feature_importance(self, model=None, X=None, y=None, features: list = None, feature_stage='original', subsample_size=5000, silent=False, **kwargs) -> DataFrame:
-        valid_feature_stages = ['original', 'transformed', 'transformed_model']
+    def get_feature_importance(
+        self, model=None, X=None, y=None, features: list = None, feature_stage="original", subsample_size=5000, silent=False, **kwargs
+    ) -> DataFrame:
+        valid_feature_stages = ["original", "transformed", "transformed_model"]
         if feature_stage not in valid_feature_stages:
-            raise ValueError(f'feature_stage must be one of: {valid_feature_stages}, but was {feature_stage}.')
+            raise ValueError(f"feature_stage must be one of: {valid_feature_stages}, but was {feature_stage}.")
         trainer = self.load_trainer()
         if X is not None:
             if y is None:
                 X, y = self.extract_label(X)
             y = self.label_cleaner.transform(y)
             X, y = self._remove_nan_label_rows(X, y)
             if self.ignored_columns:
-                X = X.drop(columns=self.ignored_columns, errors='ignore')
+                X = X.drop(columns=self.ignored_columns, errors="ignore")
             unused_features = [f for f in list(X.columns) if f not in self.features]
             if len(unused_features) > 0:
-                logger.log(30, f'These features in provided data are not utilized by the predictor and will be ignored: {unused_features}')
+                logger.log(30, f"These features in provided data are not utilized by the predictor and will be ignored: {unused_features}")
                 X = X.drop(columns=unused_features)
-            
-            if feature_stage == 'original':
-                return trainer._get_feature_importance_raw(model=model, X=X, y=y, features=features, subsample_size=subsample_size, transform_func=self.transform_features, silent=silent, **kwargs)
+
+            if feature_stage == "original":
+                return trainer._get_feature_importance_raw(
+                    model=model, X=X, y=y, features=features, subsample_size=subsample_size, transform_func=self.transform_features, silent=silent, **kwargs
+                )
             X = self.transform_features(X)
         else:
-            if feature_stage == 'original':
-                raise AssertionError('Feature importance `dataset` cannot be None if `feature_stage==\'original\'`. A test dataset must be specified.')
+            if feature_stage == "original":
+                raise AssertionError("Feature importance `dataset` cannot be None if `feature_stage=='original'`. A test dataset must be specified.")
             y = None
-        raw = feature_stage == 'transformed'
+        raw = feature_stage == "transformed"
         return trainer.get_feature_importance(X=X, y=y, model=model, features=features, raw=raw, subsample_size=subsample_size, silent=silent, **kwargs)
 
     @staticmethod
     def _remove_nan_label_rows(X, y):
         if y.isnull().any():
             y = y.dropna()
             X = X.loc[y.index]
         return X, y
 
     def infer_problem_type(self, y: Series, silent=False):
         problem_type = self._infer_problem_type(y, silent=silent)
         if problem_type == QUANTILE:
             if self.quantile_levels is None:
-                raise AssertionError(f'problem_type is inferred to be {QUANTILE}, yet quantile_levels is not specified.')
+                raise AssertionError(f"problem_type is inferred to be {QUANTILE}, yet quantile_levels is not specified.")
         elif self.quantile_levels is not None:
             if problem_type == REGRESSION:
                 problem_type = QUANTILE
             else:
-                raise AssertionError(f"autogluon infers this to be classification problem ('{problem_type}'), yet quantile_levels is not None."
-                                     "If it is truly a quantile regression problem, "
-                                     f"please specify problem_type='{QUANTILE}'.")
+                raise AssertionError(
+                    f"autogluon infers this to be classification problem ('{problem_type}'), yet quantile_levels is not None."
+                    "If it is truly a quantile regression problem, "
+                    f"please specify problem_type='{QUANTILE}'."
+                )
         return problem_type
 
     @staticmethod
     def _infer_problem_type(y: Series, silent=False):
         return infer_problem_type(y=y, silent=silent)
 
     # Loads models in memory so that they don't have to be loaded during predictions
-    def persist_trainer(self, low_memory=False, models='all', with_ancestors=False, max_memory=None) -> list:
+    def persist_trainer(self, low_memory=False, models="all", with_ancestors=False, max_memory=None) -> list:
         self.trainer = self.load_trainer()
         if not low_memory:
             return self.trainer.persist_models(models, with_ancestors=with_ancestors, max_memory=max_memory)
             # Warning: After calling this, it is not necessarily safe to save learner or trainer anymore
             #  If neural network is persisted and then trainer or learner is saved, there will be an exception thrown
         else:
             return []
 
-    def distill(self, X=None, y=None, X_val=None, y_val=None, time_limit=None, hyperparameters=None, holdout_frac=None,
-                verbosity=None, models_name_suffix=None, teacher_preds='soft',
-                augmentation_data=None, augment_method='spunge', augment_args={'size_factor': 5, 'max_size': int(1e5)}):
-        """ See abstract_trainer.distill() for details. """
+    def distill(
+        self,
+        X=None,
+        y=None,
+        X_val=None,
+        y_val=None,
+        time_limit=None,
+        hyperparameters=None,
+        holdout_frac=None,
+        verbosity=None,
+        models_name_suffix=None,
+        teacher_preds="soft",
+        augmentation_data=None,
+        augment_method="spunge",
+        augment_args={"size_factor": 5, "max_size": int(1e5)},
+    ):
+        """See abstract_trainer.distill() for details."""
         if X is not None:
-            if (self.eval_metric is not None) and (self.eval_metric.name == 'log_loss') and (self.problem_type == MULTICLASS):
+            if (self.eval_metric is not None) and (self.eval_metric.name == "log_loss") and (self.problem_type == MULTICLASS):
                 X = augment_rare_classes(X, self.label, self.threshold)
             if y is None:
                 X, y = self.extract_label(X)
             X = self.transform_features(X)
             y = self.label_cleaner.transform(y)
             if self.problem_type == MULTICLASS:
                 y = y.fillna(-1)
@@ -928,17 +952,29 @@
             X_val = self.transform_features(X_val)
             y_val = self.label_cleaner.transform(y_val)
 
         if augmentation_data is not None:
             augmentation_data = self.transform_features(augmentation_data)
 
         trainer = self.load_trainer()
-        distilled_model_names = trainer.distill(X=X, y=y, X_val=X_val, y_val=y_val, time_limit=time_limit, hyperparameters=hyperparameters,
-                                                holdout_frac=holdout_frac, verbosity=verbosity, teacher_preds=teacher_preds, models_name_suffix=models_name_suffix,
-                                                augmentation_data=augmentation_data, augment_method=augment_method, augment_args=augment_args)
+        distilled_model_names = trainer.distill(
+            X=X,
+            y=y,
+            X_val=X_val,
+            y_val=y_val,
+            time_limit=time_limit,
+            hyperparameters=hyperparameters,
+            holdout_frac=holdout_frac,
+            verbosity=verbosity,
+            teacher_preds=teacher_preds,
+            models_name_suffix=models_name_suffix,
+            augmentation_data=augmentation_data,
+            augment_method=augment_method,
+            augment_args=augment_args,
+        )
         self.save_trainer(trainer=trainer)
         return distilled_model_names
 
     def transform_labels(self, y, inverse=False, proba=False):
         if inverse:
             if proba:
                 y_transformed = self.label_cleaner.inverse_transform_proba(y=y, as_pandas=True)
@@ -947,48 +983,46 @@
         else:
             if proba:
                 y_transformed = self.label_cleaner.transform_proba(y=y, as_pandas=True)
             else:
                 y_transformed = self.label_cleaner.transform(y=y)
         return y_transformed
 
-    def calibrate_decision_threshold(self,
-                                     data: pd.DataFrame | None = None,
-                                     metric: str | Scorer | None = None,
-                                     model: str = 'best',
-                                     decision_thresholds: int | List[float] = 50,
-                                     verbose: bool = True) -> float:
+    def calibrate_decision_threshold(
+        self,
+        data: pd.DataFrame | None = None,
+        metric: str | Scorer | None = None,
+        model: str = "best",
+        decision_thresholds: int | List[float] = 50,
+        verbose: bool = True,
+    ) -> float:
         # TODO: docstring
         if metric is None:
             metric = self.eval_metric
 
         weights = None
         if data is None:
             X = None
             y = None
         else:
             if self.weight_evaluation:
                 data, weights = extract_column(data, self.sample_weight)
             X = self.transform_features(X=data)
             y = self.transform_labels(y=data[self.label])
 
-        return self.load_trainer().calibrate_decision_threshold(X=X,
-                                                                y=y,
-                                                                metric=metric,
-                                                                model=model,
-                                                                weights=weights,
-                                                                decision_thresholds=decision_thresholds,
-                                                                verbose=verbose)
+        return self.load_trainer().calibrate_decision_threshold(
+            X=X, y=y, metric=metric, model=model, weights=weights, decision_thresholds=decision_thresholds, verbose=verbose
+        )
 
     # TODO: Add data info gathering at beginning of .fit() that is used by all learners to add to get_info output
     # TODO: Add feature inference / feature engineering info to get_info output
     def get_info(self, **kwargs):
         learner_info = {
-            'path': self.path,
-            'label': self.label,
-            'random_state': self.random_state,
-            'version': self.version,
-            'features': self.features,
-            'feature_metadata_in': self.feature_metadata_in,
+            "path": self.path,
+            "label": self.label,
+            "random_state": self.random_state,
+            "version": self.version,
+            "features": self.features,
+            "feature_metadata_in": self.feature_metadata_in,
         }
 
         return learner_info
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/learner/default_learner.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 
 from autogluon.common.utils.log_utils import convert_time_in_s_to_log_friendly
 from autogluon.common.utils.resource_utils import ResourceManager
-
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, AUTO_WEIGHT, BALANCE_WEIGHT
+from autogluon.core.constants import AUTO_WEIGHT, BALANCE_WEIGHT, BINARY, MULTICLASS, QUANTILE, REGRESSION
 from autogluon.core.data import LabelCleaner
 from autogluon.core.data.cleaner import Cleaner
 from autogluon.core.utils.time import sample_df_for_time_func, time_func
 from autogluon.core.utils.utils import augment_rare_classes, extract_column
 
-from .abstract_learner import AbstractTabularLearner
 from ..trainer import AutoTrainer
+from .abstract_learner import AbstractTabularLearner
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Add functionality for advanced feature generators such as gl_code_matrix_generator (inter-row dependencies, apply to train differently than test, etc., can only run after train/test split, rerun for each cv fold)
 # TODO: - Differentiate between advanced generators that require fit (stateful, gl_code_matrix) and those that do not (bucket label averaging in SCOT GC 2019)
 # TODO: - Those that do not could be added to preprocessing function of model, but would then have to be recomputed on each model.
@@ -37,87 +36,101 @@
         self._time_fit_preprocessing = None
         self._time_fit_training = None
         self._time_limit = None
         self.preprocess_1_time = None  # Time required to preprocess 1 row of data
         self.preprocess_1_batch_size = None  # Batch size used to calculate self.preprocess_1_time
 
     # TODO: v0.1 Document trainer_fit_kwargs
-    def _fit(self, X: DataFrame, X_val: DataFrame = None, X_unlabeled: DataFrame = None, holdout_frac=0.1,
-             num_bag_folds=0, num_bag_sets=1, time_limit=None,
-             infer_limit=None, infer_limit_batch_size=None,
-             verbosity=2, **trainer_fit_kwargs):
-        """ Arguments:
-                X (DataFrame): training data
-                X_val (DataFrame): data used for hyperparameter tuning. Note: final model may be trained using this data as well as training data
-                X_unlabeled (DataFrame): data used for pretraining a model. This is same data format as X, without label-column. This data is used for semi-supervised learning.
-                holdout_frac (float): Fraction of data to hold out for evaluating validation performance (ignored if X_val != None, ignored if kfolds != 0)
-                num_bag_folds (int): kfolds used for bagging of models, roughly increases model training time by a factor of k (0: disabled)
-                num_bag_sets (int): number of repeats of kfold bagging to perform (values must be >= 1),
-                    total number of models trained during bagging = num_bag_folds * num_bag_sets
+    def _fit(
+        self,
+        X: DataFrame,
+        X_val: DataFrame = None,
+        X_unlabeled: DataFrame = None,
+        holdout_frac=0.1,
+        num_bag_folds=0,
+        num_bag_sets=1,
+        time_limit=None,
+        infer_limit=None,
+        infer_limit_batch_size=None,
+        verbosity=2,
+        **trainer_fit_kwargs,
+    ):
+        """Arguments:
+        X (DataFrame): training data
+        X_val (DataFrame): data used for hyperparameter tuning. Note: final model may be trained using this data as well as training data
+        X_unlabeled (DataFrame): data used for pretraining a model. This is same data format as X, without label-column. This data is used for semi-supervised learning.
+        holdout_frac (float): Fraction of data to hold out for evaluating validation performance (ignored if X_val != None, ignored if kfolds != 0)
+        num_bag_folds (int): kfolds used for bagging of models, roughly increases model training time by a factor of k (0: disabled)
+        num_bag_sets (int): number of repeats of kfold bagging to perform (values must be >= 1),
+            total number of models trained during bagging = num_bag_folds * num_bag_sets
         """
         # TODO: if provided, feature_types in X, X_val are ignored right now, need to pass to Learner/trainer and update this documentation.
         self._time_limit = time_limit
         if time_limit:
-            logger.log(20, f'Beginning AutoGluon training ... Time limit = {time_limit}s')
+            logger.log(20, f"Beginning AutoGluon training ... Time limit = {time_limit}s")
         else:
-            logger.log(20, 'Beginning AutoGluon training ...')
+            logger.log(20, "Beginning AutoGluon training ...")
         logger.log(20, f'AutoGluon will save models to "{self.path}"')
-        logger.log(20, f'AutoGluon Version:  {self.version}')
-        logger.log(20, f'Python Version:     {self._python_version}')
-        logger.log(20, f'Operating System:   {platform.system()}')
-        logger.log(20, f'Platform Machine:   {platform.machine()}')
-        logger.log(20, f'Platform Version:   {platform.version()}')
+        logger.log(20, f"AutoGluon Version:  {self.version}")
+        logger.log(20, f"Python Version:     {self._python_version}")
+        logger.log(20, f"Operating System:   {platform.system()}")
+        logger.log(20, f"Platform Machine:   {platform.machine()}")
+        logger.log(20, f"Platform Version:   {platform.version()}")
         try:
             # TODO: Make this logic smarter, incorporate training data size and potentially models to train into the logic to define the recommended disk space.
             #  For example, `best_quality` will require more disk space than `medium_quality`, and HPO would require additional disk space.
             disk_stats = ResourceManager.get_disk_usage(path=self.path)
             disk_free_gb = disk_stats.free / 1e9
             disk_total_gb = disk_stats.total / 1e9
             disk_proportion_avail = disk_stats.free / disk_stats.total
-            disk_log_extra = ''
+            disk_log_extra = ""
             disk_free_gb_warning_threshold = 10
             disk_verbosity = 20
             if disk_free_gb <= disk_free_gb_warning_threshold:
-                disk_log_extra += f'\n\tWARNING: Available disk space is low and there is a risk that ' \
-                                  f'AutoGluon will run out of disk during fit, causing an exception. ' \
-                                  f'\n\tWe recommend a minimum available disk space of {disk_free_gb_warning_threshold} GB, ' \
-                                  f'and large datasets may require more.'
+                disk_log_extra += (
+                    f"\n\tWARNING: Available disk space is low and there is a risk that "
+                    f"AutoGluon will run out of disk during fit, causing an exception. "
+                    f"\n\tWe recommend a minimum available disk space of {disk_free_gb_warning_threshold} GB, "
+                    f"and large datasets may require more."
+                )
                 disk_verbosity = 30
-            logger.log(disk_verbosity,
-                       f'Disk Space Avail:   {disk_free_gb:.2f} GB / {disk_total_gb:.2f} GB '
-                       f'({disk_proportion_avail * 100:.1f}%){disk_log_extra}')
+            logger.log(
+                disk_verbosity, f"Disk Space Avail:   {disk_free_gb:.2f} GB / {disk_total_gb:.2f} GB " f"({disk_proportion_avail * 100:.1f}%){disk_log_extra}"
+            )
         except Exception as e:
             # Note: using a broad exception catch as it is unknown what scenarios an exception would be raised, and what exception type would be used.
             #  The broad exception ensures that we don't completely break AutoGluon for users who may be running on strange hardware or environments.
-            logger.log(30,
-                       f'Disk Space Avail:   WARNING, an exception ({e.__class__.__name__}) occurred while attempting to get available disk space. '
-                       f'Consider opening a GitHub Issue.')
-        logger.log(20, f'Train Data Rows:    {len(X)}')
-        logger.log(20, f'Train Data Columns: {len([column for column in X.columns if column != self.label])}')
+            logger.log(
+                30,
+                f"Disk Space Avail:   WARNING, an exception ({e.__class__.__name__}) occurred while attempting to get available disk space. "
+                f"Consider opening a GitHub Issue.",
+            )
+        logger.log(20, f"Train Data Rows:    {len(X)}")
+        logger.log(20, f"Train Data Columns: {len([column for column in X.columns if column != self.label])}")
         if X_val is not None:
-            logger.log(20, f'Tuning Data Rows:    {len(X_val)}')
-            logger.log(20, f'Tuning Data Columns: {len([column for column in X_val.columns if column != self.label])}')
-        logger.log(20, f'Label Column: {self.label}')
+            logger.log(20, f"Tuning Data Rows:    {len(X_val)}")
+            logger.log(20, f"Tuning Data Columns: {len([column for column in X_val.columns if column != self.label])}")
+        logger.log(20, f"Label Column: {self.label}")
         time_preprocessing_start = time.time()
-        logger.log(20, 'Preprocessing data ...')
+        logger.log(20, "Preprocessing data ...")
         self._pre_X_rows = len(X)
         if self.problem_type is None:
             self.problem_type = self.infer_problem_type(y=X[self.label])
         if self.groups is not None:
             num_bag_sets = 1
             num_bag_folds = len(X[self.groups].unique())
         X_og = None if infer_limit_batch_size is None else X
         X, y, X_val, y_val, X_unlabeled, holdout_frac, num_bag_folds, groups = self.general_data_processing(X, X_val, X_unlabeled, holdout_frac, num_bag_folds)
         if X_og is not None:
             infer_limit = self._update_infer_limit(X=X_og, infer_limit_batch_size=infer_limit_batch_size, infer_limit=infer_limit)
 
         self._post_X_rows = len(X)
         time_preprocessing_end = time.time()
         self._time_fit_preprocessing = time_preprocessing_end - time_preprocessing_start
-        logger.log(20, f'Data preprocessing and feature engineering runtime = {round(self._time_fit_preprocessing, 2)}s ...')
+        logger.log(20, f"Data preprocessing and feature engineering runtime = {round(self._time_fit_preprocessing, 2)}s ...")
         if time_limit:
             time_limit_trainer = time_limit - self._time_fit_preprocessing
         else:
             time_limit_trainer = None
 
         trainer = self.trainer_type(
             path=self.model_context,
@@ -129,15 +142,15 @@
             low_memory=True,
             k_fold=num_bag_folds,  # TODO: Consider moving to fit call
             n_repeats=num_bag_sets,  # TODO: Consider moving to fit call
             sample_weight=self.sample_weight,
             weight_evaluation=self.weight_evaluation,
             save_data=self.cache_data,
             random_state=self.random_state,
-            verbosity=verbosity
+            verbosity=verbosity,
         )
 
         self.trainer_path = trainer.path
         if self.eval_metric is None:
             self.eval_metric = trainer.eval_metric
 
         self.save()
@@ -148,15 +161,15 @@
             y_val=y_val,
             X_unlabeled=X_unlabeled,
             holdout_frac=holdout_frac,
             time_limit=time_limit_trainer,
             infer_limit=infer_limit,
             infer_limit_batch_size=infer_limit_batch_size,
             groups=groups,
-            **trainer_fit_kwargs
+            **trainer_fit_kwargs,
         )
         self.save_trainer(trainer=trainer)
         time_end = time.time()
         self._time_fit_training = time_end - time_preprocessing_end
         self._time_fit_total = time_end - time_preprocessing_start
         logger.log(20, f'AutoGluon training complete, total runtime = {round(self._time_fit_total, 2)}s ... Best model: "{trainer.model_best}"')
 
@@ -167,92 +180,103 @@
         Raises an exception if preprocessing time is greater than or equal to the infer_limit
         """
         X_batch = sample_df_for_time_func(df=X, sample_size=infer_limit_batch_size)
         infer_limit_batch_size_actual = len(X_batch)
         self.preprocess_1_time = time_func(f=self.transform_features, args=[X_batch]) / infer_limit_batch_size_actual
         self.preprocess_1_batch_size = infer_limit_batch_size
         preprocess_1_time_log, time_unit_preprocess_1_time = convert_time_in_s_to_log_friendly(self.preprocess_1_time)
-        logger.log(20, f'\t{round(preprocess_1_time_log, 3)}{time_unit_preprocess_1_time}\t= Feature Preprocessing Time (1 row | {infer_limit_batch_size} batch size)')
+        logger.log(
+            20, f"\t{round(preprocess_1_time_log, 3)}{time_unit_preprocess_1_time}\t= Feature Preprocessing Time (1 row | {infer_limit_batch_size} batch size)"
+        )
 
         if infer_limit is not None:
             infer_limit_new = infer_limit - self.preprocess_1_time
             infer_limit_log, time_unit_infer_limit = convert_time_in_s_to_log_friendly(infer_limit)
             infer_limit_new_log, time_unit_infer_limit_new = convert_time_in_s_to_log_friendly(infer_limit_new)
 
-            logger.log(20, f'\t\tFeature Preprocessing requires {round(self.preprocess_1_time/infer_limit*100, 2)}% '
-                           f'of the overall inference constraint ({infer_limit_log}{time_unit_infer_limit})\n'
-                           f'\t\t{round(infer_limit_new_log, 3)}{time_unit_infer_limit_new} inference time budget remaining for models...')
+            logger.log(
+                20,
+                f"\t\tFeature Preprocessing requires {round(self.preprocess_1_time/infer_limit*100, 2)}% "
+                f"of the overall inference constraint ({infer_limit_log}{time_unit_infer_limit})\n"
+                f"\t\t{round(infer_limit_new_log, 3)}{time_unit_infer_limit_new} inference time budget remaining for models...",
+            )
             if infer_limit_new <= 0:
-                raise AssertionError('Impossible to satisfy inference constraint, budget is exceeded during data preprocessing!\n'
-                                     'Consider using fewer features, relaxing the inference constraint, or simplifying the feature generator.')
+                raise AssertionError(
+                    "Impossible to satisfy inference constraint, budget is exceeded during data preprocessing!\n"
+                    "Consider using fewer features, relaxing the inference constraint, or simplifying the feature generator."
+                )
             infer_limit = infer_limit_new
         return infer_limit
 
     # TODO: Add default values to X_val, X_unlabeled, holdout_frac, and num_bag_folds
     def general_data_processing(self, X: DataFrame, X_val: DataFrame, X_unlabeled: DataFrame, holdout_frac: float, num_bag_folds: int):
-        """ General data processing steps used for all models. """
+        """General data processing steps used for all models."""
         X = copy.deepcopy(X)
 
-        with pd.option_context('mode.use_inf_as_na', True): # treat None, NaN, INF, NINF as NA
+        with pd.option_context("mode.use_inf_as_na", True):  # treat None, NaN, INF, NINF as NA
             invalid_labels = X[self.label].isna()
         if invalid_labels.any():
             first_invalid_label_idx = invalid_labels.idxmax()
             raise ValueError(f"Label column cannot contain non-finite values (NaN, Inf, Ninf). First invalid label at idx: {first_invalid_label_idx}")
 
         holdout_frac_og = holdout_frac
         if X_val is not None and self.label in X_val.columns:
-            with pd.option_context('mode.use_inf_as_na', True): # treat None, NaN, INF, NINF as NA
+            with pd.option_context("mode.use_inf_as_na", True):  # treat None, NaN, INF, NINF as NA
                 invalid_tuning_labels = X_val[self.label].isna()
             if invalid_tuning_labels.any():
                 first_invalid_label_idx = invalid_tuning_labels.idxmax()
                 raise ValueError(f"Label column cannot contain non-finite values (NaN, Inf, Ninf). First invalid label at idx: {first_invalid_label_idx}")
 
             holdout_frac = 1
 
-        if (self.eval_metric is not None) and (self.eval_metric.name in ['log_loss', 'pac_score']) and (self.problem_type == MULTICLASS):
+        if (self.eval_metric is not None) and (self.eval_metric.name in ["log_loss", "pac_score"]) and (self.problem_type == MULTICLASS):
             if num_bag_folds > 0:
                 self.threshold = 2
                 if self.groups is None:
                     X = augment_rare_classes(X, self.label, threshold=2)
             else:
                 self.threshold = 1
 
-        self.threshold, holdout_frac, num_bag_folds = self.adjust_threshold_if_necessary(X[self.label], threshold=self.threshold, holdout_frac=holdout_frac, num_bag_folds=num_bag_folds)
+        self.threshold, holdout_frac, num_bag_folds = self.adjust_threshold_if_necessary(
+            X[self.label], threshold=self.threshold, holdout_frac=holdout_frac, num_bag_folds=num_bag_folds
+        )
 
         # Gets labels prior to removal of infrequent classes
         y_uncleaned = X[self.label].copy()
 
         self.cleaner = Cleaner.construct(problem_type=self.problem_type, label=self.label, threshold=self.threshold)
         X = self.cleaner.fit_transform(X)  # TODO: Consider merging cleaner into label_cleaner
         X, y = self.extract_label(X)
         self.label_cleaner = LabelCleaner.construct(problem_type=self.problem_type, y=y, y_uncleaned=y_uncleaned, positive_class=self._positive_class)
         y = self.label_cleaner.transform(y)
         X = self.set_predefined_weights(X, y)
         X, w = extract_column(X, self.sample_weight)
         X, groups = extract_column(X, self.groups)
         if self.label_cleaner.num_classes is not None and self.problem_type != BINARY:
-            logger.log(20, f'Train Data Class Count: {self.label_cleaner.num_classes}')
+            logger.log(20, f"Train Data Class Count: {self.label_cleaner.num_classes}")
 
         if X_val is not None and self.label in X_val.columns:
             y_val_og = X_val[self.label]
             X_val = self.cleaner.transform(X_val)
             if len(X_val) == 0:
-                logger.warning('############################################################################################################\n'
-                               'WARNING: All X_val data contained low frequency classes, ignoring X_val and generating from subset of X\n'
-                               '\tYour input validation data or training data labels might be corrupted, please manually inspect them for correctness!')
+                logger.warning(
+                    "############################################################################################################\n"
+                    "WARNING: All X_val data contained low frequency classes, ignoring X_val and generating from subset of X\n"
+                    "\tYour input validation data or training data labels might be corrupted, please manually inspect them for correctness!"
+                )
                 if self.problem_type in [BINARY, MULTICLASS]:
                     train_classes = sorted(list(y_uncleaned.unique()))
                     val_classes = sorted(list(y_val_og.unique()))
-                    logger.warning(f'\tTraining Classes: {train_classes}')
-                    logger.warning(f'\tTuning   Classes: {val_classes}')
-                    logger.warning(f'\tTraining Class Dtype: {y_uncleaned.dtype}')
-                    logger.warning(f'\tTuning   Class Dtype: {y_val_og.dtype}')
+                    logger.warning(f"\tTraining Classes: {train_classes}")
+                    logger.warning(f"\tTuning   Classes: {val_classes}")
+                    logger.warning(f"\tTraining Class Dtype: {y_uncleaned.dtype}")
+                    logger.warning(f"\tTuning   Class Dtype: {y_val_og.dtype}")
                     missing_classes = [c for c in val_classes if c not in train_classes]
-                    logger.warning(f'\tClasses missing from Training Data: {missing_classes}')
-                logger.warning('############################################################################################################')
+                    logger.warning(f"\tClasses missing from Training Data: {missing_classes}")
+                logger.warning("############################################################################################################")
 
                 X_val = None
                 y_val = None
                 w_val = None
                 holdout_frac = holdout_frac_og
             else:
                 X_val, y_val = self.extract_label(X_val)
@@ -261,41 +285,50 @@
                 X_val, w_val = extract_column(X_val, self.sample_weight)
         else:
             y_val = None
             w_val = None
 
         self._original_features = list(X.columns)
         # TODO: Move this up to top of data before removing data, this way our feature generator is better
-        logger.log(20, f'Using Feature Generators to preprocess the data ...')
+        logger.log(20, f"Using Feature Generators to preprocess the data ...")
         if X_val is not None:
             # Do this if working with SKLearn models, otherwise categorical features may perform very badly on the test set
-            logger.log(15, 'Performing general data preprocessing with merged train & validation data, so validation performance may not accurately reflect performance on new test data')
+            logger.log(
+                15,
+                "Performing general data preprocessing with merged train & validation data, so validation performance may not accurately reflect performance on new test data",
+            )
             X_super = pd.concat([X, X_val, X_unlabeled], ignore_index=True)
             if self.feature_generator.is_fit():
-                logger.log(20, f'{self.feature_generator.__class__.__name__} is already fit, so the training data will be processed via .transform() instead of .fit_transform().')
+                logger.log(
+                    20,
+                    f"{self.feature_generator.__class__.__name__} is already fit, so the training data will be processed via .transform() instead of .fit_transform().",
+                )
                 X_super = self.feature_generator.transform(X_super)
                 self.feature_generator.print_feature_metadata_info()
             else:
                 if X_unlabeled is None:
                     y_super = pd.concat([y, y_val], ignore_index=True)
                 else:
                     y_unlabeled = pd.Series(np.nan, index=X_unlabeled.index)
                     y_super = pd.concat([y, y_val, y_unlabeled], ignore_index=True)
                 X_super = self.fit_transform_features(X_super, y_super, problem_type=self.label_cleaner.problem_type_transform, eval_metric=self.eval_metric)
             X = X_super.head(len(X)).set_index(X.index)
 
-            X_val = X_super.head(len(X)+len(X_val)).tail(len(X_val)).set_index(X_val.index)
+            X_val = X_super.head(len(X) + len(X_val)).tail(len(X_val)).set_index(X_val.index)
 
             if X_unlabeled is not None:
                 X_unlabeled = X_super.tail(len(X_unlabeled)).set_index(X_unlabeled.index)
             del X_super
         else:
             X_super = pd.concat([X, X_unlabeled], ignore_index=True)
             if self.feature_generator.is_fit():
-                logger.log(20, f'{self.feature_generator.__class__.__name__} is already fit, so the training data will be processed via .transform() instead of .fit_transform().')
+                logger.log(
+                    20,
+                    f"{self.feature_generator.__class__.__name__} is already fit, so the training data will be processed via .transform() instead of .fit_transform().",
+                )
                 X_super = self.feature_generator.transform(X_super)
                 self.feature_generator.print_feature_metadata_info()
             else:
                 if X_unlabeled is None:
                     y_super = y.reset_index(drop=True)
                 else:
                     y_unlabeled = pd.Series(np.nan, index=X_unlabeled.index)
@@ -320,42 +353,44 @@
                     nan_vals[:] = np.nan
                     X_val[self.sample_weight] = nan_vals
                 else:
                     raise ValueError(f"sample_weight column '{self.sample_weight}' cannot be missing from X_val if weight_evaluation=True")
         return X, X_val
 
     def set_predefined_weights(self, X, y):
-        if self.sample_weight not in [AUTO_WEIGHT,BALANCE_WEIGHT] or self.problem_type not in [BINARY,MULTICLASS]:
+        if self.sample_weight not in [AUTO_WEIGHT, BALANCE_WEIGHT] or self.problem_type not in [BINARY, MULTICLASS]:
             return X
         if self.sample_weight in X.columns:
-            raise ValueError(f"Column name '{self.sample_weight}' cannot appear in your dataset with predefined weighting strategy. Please change it and try again.")
+            raise ValueError(
+                f"Column name '{self.sample_weight}' cannot appear in your dataset with predefined weighting strategy. Please change it and try again."
+            )
         if self.sample_weight == BALANCE_WEIGHT:
             if self.class_weights is None:
                 class_counts = y.value_counts()
                 n = len(y)
                 k = len(class_counts)
-                self.class_weights = {c : n/(class_counts[c]*k) for c in class_counts.index}
+                self.class_weights = {c: n / (class_counts[c] * k) for c in class_counts.index}
                 logger.log(20, "Assigning sample weights to balance differences in frequency of classes.")
                 logger.log(15, f"Balancing classes via the following weights: {self.class_weights}")
             w = y.map(self.class_weights)
         elif self.sample_weight == AUTO_WEIGHT:  # TODO: support more sophisticated auto_weight strategy
             raise NotImplementedError(f"{AUTO_WEIGHT} strategy not yet supported.")
         X[self.sample_weight] = w  # TODO: consider not bundling sample weights inside X
         return X
 
     def adjust_threshold_if_necessary(self, y, threshold, holdout_frac, num_bag_folds):
         new_threshold, new_holdout_frac, new_num_bag_folds = self._adjust_threshold_if_necessary(y, threshold, holdout_frac, num_bag_folds)
         if new_threshold != threshold:
             if new_threshold < threshold:
-                logger.warning(f'Warning: Updated label_count_threshold from {threshold} to {new_threshold} to avoid cutting too many classes.')
+                logger.warning(f"Warning: Updated label_count_threshold from {threshold} to {new_threshold} to avoid cutting too many classes.")
         if new_holdout_frac != holdout_frac:
             if new_holdout_frac > holdout_frac:
-                logger.warning(f'Warning: Updated holdout_frac from {holdout_frac} to {new_holdout_frac} to avoid cutting too many classes.')
+                logger.warning(f"Warning: Updated holdout_frac from {holdout_frac} to {new_holdout_frac} to avoid cutting too many classes.")
         if new_num_bag_folds != num_bag_folds:
-            logger.warning(f'Warning: Updated num_bag_folds from {num_bag_folds} to {new_num_bag_folds} to avoid cutting too many classes.')
+            logger.warning(f"Warning: Updated num_bag_folds from {num_bag_folds} to {new_num_bag_folds} to avoid cutting too many classes.")
         return new_threshold, new_holdout_frac, new_num_bag_folds
 
     def _adjust_threshold_if_necessary(self, y, threshold, holdout_frac, num_bag_folds):
         new_threshold = threshold
         num_rows = len(y)
         holdout_frac = max(holdout_frac, 1 / num_rows + 0.001)
         num_bag_folds = min(num_bag_folds, num_rows)
@@ -397,16 +432,18 @@
 
         return new_threshold, holdout_frac, num_bag_folds
 
     def get_info(self, include_model_info=False, **kwargs):
         learner_info = super().get_info(**kwargs)
         trainer = self.load_trainer()
         trainer_info = trainer.get_info(include_model_info=include_model_info)
-        learner_info.update({
-            'time_fit_preprocessing': self._time_fit_preprocessing,
-            'time_fit_training': self._time_fit_training,
-            'time_fit_total': self._time_fit_total,
-            'time_limit': self._time_limit,
-        })
+        learner_info.update(
+            {
+                "time_fit_preprocessing": self._time_fit_preprocessing,
+                "time_fit_training": self._time_fit_training,
+                "time_fit_total": self._time_fit_total,
+                "time_limit": self._time_limit,
+            }
+        )
 
         learner_info.update(trainer_info)
         return learner_info
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from autogluon.core.models.abstract.abstract_model import AbstractModel
 
-from .lgb.lgb_model import LGBModel
+from .automm.automm_model import MultiModalPredictorModel
+from .automm.ft_transformer import FTTransformerModel
 from .catboost.catboost_model import CatBoostModel
-from .xgboost.xgboost_model import XGBoostModel
-from .rf.rf_model import RFModel
-from .xt.xt_model import XTModel
+from .fastainn.tabular_nn_fastai import NNFastAiTabularModel
+from .fasttext.fasttext_model import FastTextModel
+from .image_prediction.image_predictor import ImagePredictorModel
+from .imodels.imodels_models import (
+    BoostedRulesModel,
+    FigsModel,
+    GreedyTreeModel,
+    HSTreeModel,
+    RuleFitModel,
+    _IModelsModel,
+)
 from .knn.knn_model import KNNModel
+from .lgb.lgb_model import LGBModel
 from .lr.lr_model import LinearModel
+from .rf.rf_model import RFModel
+from .tabpfn.tabpfn_model import TabPFNModel
 from .tabular_nn.torch.tabular_nn_torch import TabularNeuralNetTorchModel
-from .fastainn.tabular_nn_fastai import NNFastAiTabularModel
-from .fasttext.fasttext_model import FastTextModel
 from .text_prediction.text_prediction_v1_model import TextPredictorModel
-from .image_prediction.image_predictor import ImagePredictorModel
-from .imodels.imodels_models import RuleFitModel, BoostedRulesModel, GreedyTreeModel, HSTreeModel, \
-    FigsModel, _IModelsModel
 from .vowpalwabbit.vowpalwabbit_model import VowpalWabbitModel
-from .automm.automm_model import MultiModalPredictorModel
-from .automm.ft_transformer import FTTransformerModel
-from .tabpfn.tabpfn_model import TabPFNModel
-
+from .xgboost.xgboost_model import XGBoostModel
+from .xt.xt_model import XTModel
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from typing import Dict
 
 from autogluon.common.utils.resource_utils import ResourceManager
 
 
 class RapidsModelMixin:
     """Mixin class for methods re-used across RAPIDS models"""
+
     # FIXME: Efficient OOF doesn't work in RAPIDS
     @classmethod
     def _get_default_ag_args_ensemble(cls, **kwargs) -> dict:
         default_ag_args_ensemble = super()._get_default_ag_args_ensemble(**kwargs)
-        extra_ag_args_ensemble = {'use_child_oof': False}
+        extra_ag_args_ensemble = {"use_child_oof": False}
         default_ag_args_ensemble.update(extra_ag_args_ensemble)
         return default_ag_args_ensemble
 
     def _get_default_resources(self):
         num_cpus, _ = super()._get_default_resources()
         num_gpus = min(ResourceManager.get_gpu_count_torch(), 1)  # Use single gpu training by default. Consider revising it later.
         return num_cpus, num_gpus
 
     def get_minimum_resources(self, is_gpu_available=False) -> Dict[str, int]:
         return {
-            'num_cpus': 1,
-            'num_gpus': 1,
+            "num_cpus": 1,
+            "num_gpus": 1,
         }
 
     def _more_tags(self):
-        return {'valid_oof': False}
+        return {"valid_oof": False}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import torch
 
 
 class TorchThreadManager:
     """
     Temporary updates torch num_threads to the specified value within the context, then reverts to the original num_threads upon exit.
     """
+
     def __init__(self, num_threads):
         self.num_threads = num_threads
         self.num_threads_og = None
 
     def __enter__(self):
         self.num_threads_og = torch.get_num_threads()
         torch.set_num_threads(self.num_threads)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,35 @@
 
 import logging
 import os
 from typing import Dict, Optional
 
 import pandas as pd
 
-from autogluon.common.features.types import R_OBJECT, R_INT, R_FLOAT, R_CATEGORY, \
-    S_TEXT, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY, S_TEXT_SPECIAL, S_IMAGE_PATH
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION
+from autogluon.common.features.types import (
+    R_CATEGORY,
+    R_FLOAT,
+    R_INT,
+    R_OBJECT,
+    S_IMAGE_PATH,
+    S_TEXT,
+    S_TEXT_AS_CATEGORY,
+    S_TEXT_NGRAM,
+    S_TEXT_SPECIAL,
+)
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_autogluon_multimodal
+from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION
 from autogluon.core.models import AbstractModel
 
 logger = logging.getLogger(__name__)
 
 
 class MultiModalPredictorModel(AbstractModel):
-    _NN_MODEL_NAME = 'automm_model'
+    _NN_MODEL_NAME = "automm_model"
 
     def __init__(self, **kwargs):
         """Wrapper of autogluon.multimodal.MultiModalPredictor.
 
         The features can be a mix of
         - image column
         - text column
@@ -67,25 +76,25 @@
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     @classmethod
     def _get_default_ag_args(cls) -> dict:
         default_ag_args = super()._get_default_ag_args()
         extra_ag_args = {
-            'valid_stacker': False,
-            'problem_types': [BINARY, MULTICLASS, REGRESSION],
+            "valid_stacker": False,
+            "problem_types": [BINARY, MULTICLASS, REGRESSION],
         }
         default_ag_args.update(extra_ag_args)
         return default_ag_args
 
     # FIXME: Enable parallel bagging once AutoMM supports being run within Ray without hanging
     @classmethod
     def _get_default_ag_args_ensemble(cls, **kwargs) -> dict:
         default_ag_args_ensemble = super()._get_default_ag_args_ensemble(**kwargs)
-        extra_ag_args_ensemble = {'fold_fitting_strategy': 'sequential_local'}
+        extra_ag_args_ensemble = {"fold_fitting_strategy": "sequential_local"}
         default_ag_args_ensemble.update(extra_ag_args_ensemble)
         return default_ag_args_ensemble
 
     def _set_default_params(self):
         super()._set_default_params()
         try_import_autogluon_multimodal()
 
@@ -95,22 +104,24 @@
         This method is a placeholder for inheriting models to override with more complex functionality if needed.
         """
         X = self.preprocess(X=X, **kwargs)
         if X_val is not None:
             X_val = self.preprocess(X=X_val, **kwargs)
         return X, y, X_val, y_val
 
-    def _fit(self,
-             X: pd.DataFrame,
-             y: pd.Series,
-             X_val: Optional[pd.DataFrame] = None,
-             y_val: Optional[pd.Series] = None,
-             time_limit: Optional[int] = None,
-             sample_weight=None,
-             **kwargs):
+    def _fit(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        X_val: Optional[pd.DataFrame] = None,
+        y_val: Optional[pd.Series] = None,
+        time_limit: Optional[int] = None,
+        sample_weight=None,
+        **kwargs,
+    ):
         """The internal fit function
 
         Parameters
         ----------
         X
             Features of the training dataset
         y
@@ -127,72 +138,73 @@
             Other keyword arguments
 
         """
         try_import_autogluon_multimodal()
         from autogluon.multimodal import MultiModalPredictor
 
         # Decide name of the label column
-        if 'label' in X.columns:
+        if "label" in X.columns:
             label_col_id = 0
             while True:
-                self._label_column_name = 'label{}'.format(label_col_id)
+                self._label_column_name = "label{}".format(label_col_id)
                 if self._label_column_name not in X.columns:
                     break
                 label_col_id += 1
         else:
-            self._label_column_name = 'label'
+            self._label_column_name = "label"
 
         X, y, X_val, y_val = self.preprocess_fit(X=X, y=y, X_val=X_val, y_val=y_val)
         params = self._get_model_params()
-        max_features = params.pop('_max_features', None)  # FIXME: `_max_features` is a hack. Instead use ag_args_fit and make generic
+        max_features = params.pop("_max_features", None)  # FIXME: `_max_features` is a hack. Instead use ag_args_fit and make generic
         num_features = len(X.columns)
         if max_features is not None and num_features > max_features:
-            raise AssertionError(f'Feature count ({num_features}) is greater than max allowed features ({max_features}) for {self.name}. Skipping model... '
-                                 f'To increase the max allowed features, specify the value via the `_max_features` parameter '
-                                 f'(Fully ignore by specifying `None`. '
-                                 f'`_max_features` is experimental and will likely change API without warning in future releases.')
+            raise AssertionError(
+                f"Feature count ({num_features}) is greater than max allowed features ({max_features}) for {self.name}. Skipping model... "
+                f"To increase the max allowed features, specify the value via the `_max_features` parameter "
+                f"(Fully ignore by specifying `None`. "
+                f"`_max_features` is experimental and will likely change API without warning in future releases."
+            )
 
         # Get arguments from kwargs
-        verbosity = kwargs.get('verbosity', 2)
+        verbosity = kwargs.get("verbosity", 2)
         if verbosity <= 2:
             enable_progress_bar = False
         else:
             enable_progress_bar = True
-        num_gpus = kwargs.get('num_gpus', None)
+        num_gpus = kwargs.get("num_gpus", None)
         if sample_weight is not None:  # TODO: support
-            logger.log(15, "sample_weight not yet supported for MultiModalPredictorModel, "
-                           "this model will ignore them in training.")
+            logger.log(15, "sample_weight not yet supported for MultiModalPredictorModel, " "this model will ignore them in training.")
 
         # Need to deep copy to avoid altering outer context
         X = X.copy()
         X.insert(len(X.columns), self._label_column_name, y)
         if X_val is not None:
             X_val = X_val.copy()
             X_val.insert(len(X_val.columns), self._label_column_name, y_val)
 
         column_types = self._construct_column_types()
 
         verbosity_text = max(0, verbosity - 1)
-        root_logger = logging.getLogger('autogluon')
+        root_logger = logging.getLogger("autogluon")
         root_log_level = root_logger.level
         # in self.save(), the model is saved to automm_nn_path
         automm_nn_path = os.path.join(self.path, self._NN_MODEL_NAME)
         self.model = MultiModalPredictor(
             label=self._label_column_name,
             problem_type=self.problem_type,
             path=automm_nn_path,
             eval_metric=self.eval_metric,
             verbosity=verbosity_text,
             enable_progress_bar=enable_progress_bar,
         )
 
         if num_gpus is not None:
-            params['env.num_gpus'] = num_gpus
-        presets = params.pop('presets', None)
-        seed = params.pop('seed', 0)
+            params["env.num_gpus"] = num_gpus
+        presets = params.pop("presets", None)
+        seed = params.pop("seed", 0)
 
         self.model.fit(
             train_data=X,
             tuning_data=X_val,
             time_limit=time_limit,
             presets=presets,
             hyperparameters=params,
@@ -230,14 +242,15 @@
 
     @classmethod
     def load(cls, path: str, reset_paths=True, verbose=True):
         model = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
         if model._load_model:
             try_import_autogluon_multimodal()
             from autogluon.multimodal import MultiModalPredictor
+
             model.model = MultiModalPredictor.load(os.path.join(path, cls._NN_MODEL_NAME))
         model._load_model = None
         return model
 
     def get_memory_size(self) -> int:
         """Return the memory size by calculating the total number of parameters.
 
@@ -253,42 +266,42 @@
     def _get_default_resources(self):
         num_cpus = ResourceManager.get_cpu_count()
         num_gpus = min(ResourceManager.get_gpu_count_torch(), 1)  # Use single gpu training by default. Consider to revise it later.
         return num_cpus, num_gpus
 
     def get_minimum_resources(self, is_gpu_available=False) -> Dict[str, int]:
         return {
-            'num_cpus': 1,
-            'num_gpus': 1,
+            "num_cpus": 1,
+            "num_gpus": 1,
         }
 
     def _construct_column_types(self) -> dict:
         # Construct feature types input to MultimodalPredictor
         features_image_path = set(self._feature_metadata.get_features(required_special_types=[S_IMAGE_PATH]))
         features_text = set(self._feature_metadata.get_features(required_special_types=[S_TEXT]))
         features_categorical = set(self._feature_metadata.get_features(valid_raw_types=[R_CATEGORY]))
         features_numerical = set(self._feature_metadata.get_features(valid_raw_types=[R_INT, R_FLOAT]))
 
         key_map = {
-            'image_path': features_image_path,
-            'text': features_text,
-            'categorical': features_categorical,
-            'numerical': features_numerical,
+            "image_path": features_image_path,
+            "text": features_text,
+            "categorical": features_categorical,
+            "numerical": features_numerical,
         }
 
         features = self._feature_metadata.get_features()
 
         column_types = {}
         for feature in features:
-            for key in ['image_path', 'text', 'categorical', 'numerical']:
+            for key in ["image_path", "text", "categorical", "numerical"]:
                 if feature in key_map[key]:
                     column_types[feature] = key
                     break
         return column_types
 
     def _more_tags(self):
         # `can_refit_full=False` because MultiModalPredictor does not communicate how to train until the best epoch in refit_full.
-        return {'can_refit_full': False}
+        return {"can_refit_full": False}
 
     @classmethod
     def _class_tags(cls):
-        return {'handles_text': True}
+        return {"handles_text": True}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Wrapper of the MultiModalPredictor."""
 import logging
 from typing import Dict
 
-from autogluon.common.features.types import R_INT, R_FLOAT, R_CATEGORY, \
-    S_TEXT_NGRAM, S_TEXT_SPECIAL
+from autogluon.common.features.types import R_CATEGORY, R_FLOAT, R_INT, S_TEXT_NGRAM, S_TEXT_SPECIAL
 
 from .automm_model import MultiModalPredictorModel
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Add unit tests
@@ -43,18 +42,18 @@
         features
             Names of the features.
         feature_metadata
             The feature metadata.
         """
         super().__init__(**kwargs)
 
-    def _fit(self, X, num_gpus='auto', **kwargs):
+    def _fit(self, X, num_gpus="auto", **kwargs):
         if not isinstance(num_gpus, str):
             if num_gpus == 0:
-                logger.log(30, f'WARNING: Training {self.name} on CPU (no GPU specified). This could take a long time. Use GPU to speed up training.')
+                logger.log(30, f"WARNING: Training {self.name} on CPU (no GPU specified). This could take a long time. Use GPU to speed up training.")
         super()._fit(X, num_gpus=num_gpus, **kwargs)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             valid_raw_types=[R_INT, R_FLOAT, R_CATEGORY],
             ignored_type_group_special=[S_TEXT_NGRAM, S_TEXT_SPECIAL],
@@ -74,31 +73,31 @@
             "optimization.max_epochs": 2000,  # Specify a large value to train until convergence
             "optimization.weight_decay": 1.0e-5,
             "optimization.lr_choice": None,
             "optimization.lr_schedule": "polynomial_decay",
             "optimization.warmup_steps": 0.0,
             "optimization.patience": 20,
             "optimization.top_k": 3,
-            '_max_features': 300,  # FIXME: This is a hack, move to AG_ARGS_FIT for v0.7
+            "_max_features": 300,  # FIXME: This is a hack, move to AG_ARGS_FIT for v0.7
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def get_minimum_resources(self, is_gpu_available=False) -> Dict[str, int]:
         return {
             "num_cpus": 1,
             "num_gpus": 0,  # allow FT_Transformer to be trained on CPU only
         }
 
     @classmethod
     def _get_default_ag_args_ensemble(cls, **kwargs) -> dict:
         default_ag_args_ensemble = super()._get_default_ag_args_ensemble(**kwargs)
         extra_ag_args_ensemble = {
-            'fold_fitting_strategy': 'auto',
-            'fold_fitting_strategy_gpu': 'sequential_local',  # Crashes when using GPU in parallel bagging
+            "fold_fitting_strategy": "auto",
+            "fold_fitting_strategy_gpu": "sequential_local",  # Crashes when using GPU in parallel bagging
         }
         default_ag_args_ensemble.update(extra_ag_args_ensemble)
         return default_ag_args_ensemble
 
     @classmethod
     def _class_tags(cls):
-        return {'handles_text': False}
+        return {"handles_text": False}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-
 import logging
 import time
 
 from autogluon.common.utils.resource_utils import ResourceManager
 
 from .catboost_utils import CATBOOST_QUANTILE_PREFIX
 
-
 logger = logging.getLogger(__name__)
 
 
 class MemoryCheckCallback:
     """
     Callback to ensure memory usage is safe, otherwise early stops the model to avoid OOM errors.
 
@@ -19,28 +17,29 @@
     Parameters
     ----------
     period : int, default = 10
         Number of iterations between checking memory status. Higher values are less precise but use less compute.
     verbose : bool, default = False
         Whether to log information on memory status even if memory usage is low.
     """
+
     def __init__(self, period: int = 10, verbose=False):
         self.period = period
         self.init_mem_rss = ResourceManager.get_memory_rss()
         self.init_mem_avail = ResourceManager.get_available_virtual_mem()
         self.verbose = verbose
 
         self._cur_period = 1
 
     def after_iteration(self, info):
         iteration = info.iteration
         if iteration % self._cur_period == 0:
             not_enough_memory = self.memory_check(iteration)
             if not_enough_memory:
-                logger.log(20, f'\tRan low on memory, early stopping on iteration {info.iteration}.')
+                logger.log(20, f"\tRan low on memory, early stopping on iteration {info.iteration}.")
                 return False
         return True
 
     def memory_check(self, iter) -> bool:
         """Checks if memory usage is unsafe. If so, then returns True to signal the model to stop training early."""
         available_bytes = ResourceManager.get_available_virtual_mem()
         cur_rss = ResourceManager.get_memory_rss()
@@ -49,28 +48,29 @@
             self.init_mem_rss = cur_rss
         estimated_model_size_mb = (cur_rss - self.init_mem_rss) >> 20
         available_mb = available_bytes >> 20
         model_size_memory_ratio = estimated_model_size_mb / available_mb
 
         early_stop = False
         if model_size_memory_ratio > 1.0:
-            logger.warning(f'Warning: Large model size may cause OOM error if training continues')
+            logger.warning(f"Warning: Large model size may cause OOM error if training continues")
             early_stop = True
 
         if available_mb < 512:  # Less than 500 MB
-            logger.warning(f'Warning: Low available memory may cause OOM error if training continues')
+            logger.warning(f"Warning: Low available memory may cause OOM error if training continues")
             early_stop = True
 
         if early_stop:
-            logger.warning('Warning: Early stopped model prior to optimal result to avoid OOM error. '
-                           'Please increase available memory to avoid subpar model quality.')
-            logger.warning(f'Available Memory: {available_mb} MB, Estimated Model size: {estimated_model_size_mb} MB')
+            logger.warning(
+                "Warning: Early stopped model prior to optimal result to avoid OOM error. " "Please increase available memory to avoid subpar model quality."
+            )
+            logger.warning(f"Available Memory: {available_mb} MB, Estimated Model size: {estimated_model_size_mb} MB")
             return True
         elif self.verbose or (model_size_memory_ratio > 0.25):
-            logging.debug(f'Available Memory: {available_mb} MB, Estimated Model size: {estimated_model_size_mb} MB')
+            logging.debug(f"Available Memory: {available_mb} MB, Estimated Model size: {estimated_model_size_mb} MB")
 
         if model_size_memory_ratio > 0.5:
             self._cur_period = 1  # Increase rate of memory check if model gets large enough to cause OOM potentially
         elif iter > self.period:
             self._cur_period = self.period
 
         return False
@@ -85,23 +85,24 @@
     Parameters
     ----------
     time_start : float
         The starting time (usually obtained via `time.time()`) of the training.
     time_limit : float
         The time in seconds before stopping training.
     """
+
     def __init__(self, time_start, time_limit):
         self.time_end = time_start + time_limit
         self.time_start = time_start
 
     def after_iteration(self, info):
         time_cur = time.time()
         time_per_iter = (time_cur - self.time_start) / info.iteration
-        if self.time_end < (time_cur + 2*time_per_iter):
-            logger.log(20, f'\tRan out of time, early stopping on iteration {info.iteration}.')
+        if self.time_end < (time_cur + 2 * time_per_iter):
+            logger.log(20, f"\tRan out of time, early stopping on iteration {info.iteration}.")
             return False
         return True
 
 
 class EarlyStoppingCallback:
     """
     Early stopping callback.
@@ -114,26 +115,29 @@
        If int, The possible number of rounds without the trend occurrence.
        If tuple, contains early stopping class as first element and class init kwargs as second element.
     eval_metric : str
        The eval_metric to use for early stopping. Must also be specified in the CatBoost model params.
     compare_key : str, default = 'validation'
         The data to use for scoring. It is recommended to keep as default.
     """
-    def __init__(self, stopping_rounds, eval_metric, compare_key='validation'):
+
+    def __init__(self, stopping_rounds, eval_metric, compare_key="validation"):
         if isinstance(stopping_rounds, int):
             from autogluon.core.utils.early_stopping import SimpleES
+
             self.es = SimpleES(patience=stopping_rounds)
         else:
             self.es = stopping_rounds[0](**stopping_rounds[1])
         self.best_score = None
         self.compare_key = compare_key
 
         if isinstance(eval_metric, str):
             # FIXME: Avoid using private API! (https://github.com/autogluon/autogluon/issues/1381)
             from catboost._catboost import is_maximizable_metric
+
             is_max_optimal = is_maximizable_metric(eval_metric)
             eval_metric_name = eval_metric
         else:
             is_max_optimal = eval_metric.is_max_optimal()
             # FIXME: Unsure if this works for custom metrics!
             eval_metric_name = eval_metric.__class__.__name__
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 import os
 import time
+
 import numpy as np
 
-from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY
+from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
-from autogluon.core.constants import PROBLEM_TYPES_CLASSIFICATION, MULTICLASS, QUANTILE, SOFTCLASS
+from autogluon.common.utils.try_import import try_import_catboost
+from autogluon.core.constants import MULTICLASS, PROBLEM_TYPES_CLASSIFICATION, QUANTILE, SOFTCLASS
 from autogluon.core.models import AbstractModel
 from autogluon.core.models._utils import get_early_stopping_rounds
 from autogluon.core.utils.exceptions import TimeLimitExceeded
-from autogluon.common.utils.try_import import try_import_catboost
 
 from .callbacks import EarlyStoppingCallback, MemoryCheckCallback, TimeCheckCallback
 from .catboost_utils import get_catboost_metric_from_ag_metric
 from .hyperparameters.parameters import get_param_baseline
 from .hyperparameters.searchspaces import get_default_searchspace
 
 logger = logging.getLogger(__name__)
@@ -23,201 +24,197 @@
 # TODO: Consider having CatBoost variant that converts all categoricals to numerical as done in RFModel, was showing improved results in some problems.
 class CatBoostModel(AbstractModel):
     """
     CatBoost model: https://catboost.ai/
 
     Hyperparameter options: https://catboost.ai/docs/concepts/python-reference_parameters-list.html
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._category_features = None
 
     def _set_default_params(self):
         default_params = get_param_baseline(problem_type=self.problem_type)
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
-        self._set_default_param_value('random_seed', 0)  # Remove randomness for reproducibility
+        self._set_default_param_value("random_seed", 0)  # Remove randomness for reproducibility
         # Set 'allow_writing_files' to True in order to keep log files created by catboost during training (these will be saved in the directory where AutoGluon stores this model)
-        self._set_default_param_value('allow_writing_files', False)  # Disables creation of catboost logging files during training by default
+        self._set_default_param_value("allow_writing_files", False)  # Disables creation of catboost logging files during training by default
         if self.problem_type != SOFTCLASS:  # TODO: remove this after catboost 0.24
             default_eval_metric = get_catboost_metric_from_ag_metric(self.stopping_metric, self.problem_type, self.quantile_levels)
-            self._set_default_param_value('eval_metric', default_eval_metric)
+            self._set_default_param_value("eval_metric", default_eval_metric)
 
     def _get_default_searchspace(self):
         return get_default_searchspace(self.problem_type, num_classes=self.num_classes)
 
     def _preprocess_nonadaptive(self, X, **kwargs):
         X = super()._preprocess_nonadaptive(X, **kwargs)
         if self._category_features is None:
-            self._category_features = list(X.select_dtypes(include='category').columns)
+            self._category_features = list(X.select_dtypes(include="category").columns)
         if self._category_features:
             X = X.copy()
             for category in self._category_features:
                 current_categories = X[category].cat.categories
-                if '__NaN__' in current_categories:
-                    X[category] = X[category].fillna('__NaN__')
+                if "__NaN__" in current_categories:
+                    X[category] = X[category].fillna("__NaN__")
                 else:
-                    X[category] = X[category].cat.add_categories('__NaN__').fillna('__NaN__')
+                    X[category] = X[category].cat.add_categories("__NaN__").fillna("__NaN__")
         return X
 
     def _estimate_memory_usage(self, X, **kwargs):
         num_classes = self.num_classes if self.num_classes else 1  # self.num_classes could be None after initialization if it's a regression problem
         data_mem_usage = get_approximate_df_mem_usage(X).sum()
         approx_mem_size_req = data_mem_usage * 7 + data_mem_usage / 4 * num_classes  # TODO: Extremely crude approximation, can be vastly improved
         return approx_mem_size_req
 
     # TODO: Use Pool in preprocess, optimize bagging to do Pool.split() to avoid re-computing pool for each fold! Requires stateful + y
     #  Pool is much more memory efficient, avoids copying data twice in memory
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             time_limit=None,
-             num_gpus=0,
-             num_cpus=-1,
-             sample_weight=None,
-             sample_weight_val=None,
-             **kwargs):
+    def _fit(self, X, y, X_val=None, y_val=None, time_limit=None, num_gpus=0, num_cpus=-1, sample_weight=None, sample_weight_val=None, **kwargs):
         time_start = time.time()
         try_import_catboost()
         from catboost import CatBoostClassifier, CatBoostRegressor, Pool
+
         ag_params = self._get_ag_params()
         params = self._get_model_params()
-        params['thread_count'] = num_cpus
+        params["thread_count"] = num_cpus
         if self.problem_type == SOFTCLASS:
             # FIXME: This is extremely slow due to unoptimized metric / objective sent to CatBoost
             from .catboost_softclass_utils import SoftclassCustomMetric, SoftclassObjective
-            params['loss_function'] = SoftclassObjective.SoftLogLossObjective()
-            params['eval_metric'] = SoftclassCustomMetric.SoftLogLossMetric()
+
+            params["loss_function"] = SoftclassObjective.SoftLogLossObjective()
+            params["eval_metric"] = SoftclassCustomMetric.SoftLogLossMetric()
         elif self.problem_type == QUANTILE:
             # FIXME: Unless specified, CatBoost defaults to loss_function='MultiQuantile' and raises an exception
-            params['loss_function'] = params['eval_metric']
+            params["loss_function"] = params["eval_metric"]
 
         model_type = CatBoostClassifier if self.problem_type in PROBLEM_TYPES_CLASSIFICATION else CatBoostRegressor
         num_rows_train = len(X)
         num_cols_train = len(X.columns)
         num_classes = self.num_classes if self.num_classes else 1  # self.num_classes could be None after initialization if it's a regression problem
 
         X = self.preprocess(X)
-        cat_features = list(X.select_dtypes(include='category').columns)
+        cat_features = list(X.select_dtypes(include="category").columns)
         X = Pool(data=X, label=y, cat_features=cat_features, weight=sample_weight)
 
         if X_val is None:
             eval_set = None
             early_stopping_rounds = None
         else:
             X_val = self.preprocess(X_val)
             X_val = Pool(data=X_val, label=y_val, cat_features=cat_features, weight=sample_weight_val)
             eval_set = X_val
-            early_stopping_rounds = ag_params.get('early_stop', 'adaptive')
+            early_stopping_rounds = ag_params.get("early_stop", "adaptive")
             if isinstance(early_stopping_rounds, (str, tuple, list)):
                 early_stopping_rounds = self._get_early_stopping_rounds(num_rows_train=num_rows_train, strategy=early_stopping_rounds)
 
-        if params.get('allow_writing_files', False):
-            if 'train_dir' not in params:
+        if params.get("allow_writing_files", False):
+            if "train_dir" not in params:
                 try:
                     # TODO: What if path is in S3?
                     os.makedirs(os.path.dirname(self.path), exist_ok=True)
                 except:
                     pass
                 else:
-                    params['train_dir'] = self.path + 'catboost_info'
+                    params["train_dir"] = self.path + "catboost_info"
 
         # TODO: Add more control over these params (specifically early_stopping_rounds)
-        verbosity = kwargs.get('verbosity', 2)
+        verbosity = kwargs.get("verbosity", 2)
         if verbosity <= 1:
             verbose = False
         elif verbosity == 2:
             verbose = False
         elif verbosity == 3:
             verbose = 20
         else:
             verbose = True
 
         num_features = len(self._features)
 
         if num_gpus != 0:
-            if 'task_type' not in params:
-                params['task_type'] = 'GPU'
-                logger.log(20, f'\tTraining {self.name} with GPU, note that this may negatively impact model quality compared to CPU training.')
+            if "task_type" not in params:
+                params["task_type"] = "GPU"
+                logger.log(20, f"\tTraining {self.name} with GPU, note that this may negatively impact model quality compared to CPU training.")
                 # TODO: Confirm if GPU is used in HPO (Probably not)
                 # TODO: Adjust max_bins to 254?
 
-        if params.get('task_type', None) == 'GPU':
-            if 'colsample_bylevel' in params:
-                params.pop('colsample_bylevel')
-                logger.log(30, f'\t\'colsample_bylevel\' is not supported on GPU, using default value (Default = 1).')
-            if 'rsm' in params:
-                params.pop('rsm')
-                logger.log(30, f'\t\'rsm\' is not supported on GPU, using default value (Default = 1).')
+        if params.get("task_type", None) == "GPU":
+            if "colsample_bylevel" in params:
+                params.pop("colsample_bylevel")
+                logger.log(30, f"\t'colsample_bylevel' is not supported on GPU, using default value (Default = 1).")
+            if "rsm" in params:
+                params.pop("rsm")
+                logger.log(30, f"\t'rsm' is not supported on GPU, using default value (Default = 1).")
 
-        if self.problem_type == MULTICLASS and 'rsm' not in params and 'colsample_bylevel' not in params and num_features > 1000:
+        if self.problem_type == MULTICLASS and "rsm" not in params and "colsample_bylevel" not in params and num_features > 1000:
             # Subsample columns to speed up training
-            if params.get('task_type', None) != 'GPU':  # RSM does not work on GPU
-                params['colsample_bylevel'] = max(min(1.0, 1000 / num_features), 0.05)
-                logger.log(30, f'\tMany features detected ({num_features}), dynamically setting \'colsample_bylevel\' to {params["colsample_bylevel"]} to speed up training (Default = 1).')
-                logger.log(30, f'\tTo disable this functionality, explicitly specify \'colsample_bylevel\' in the model hyperparameters.')
+            if params.get("task_type", None) != "GPU":  # RSM does not work on GPU
+                params["colsample_bylevel"] = max(min(1.0, 1000 / num_features), 0.05)
+                logger.log(
+                    30,
+                    f'\tMany features detected ({num_features}), dynamically setting \'colsample_bylevel\' to {params["colsample_bylevel"]} to speed up training (Default = 1).',
+                )
+                logger.log(30, f"\tTo disable this functionality, explicitly specify 'colsample_bylevel' in the model hyperparameters.")
             else:
-                params['colsample_bylevel'] = 1.0
-                logger.log(30, f'\t\'colsample_bylevel\' is not supported on GPU, using default value (Default = 1).')
+                params["colsample_bylevel"] = 1.0
+                logger.log(30, f"\t'colsample_bylevel' is not supported on GPU, using default value (Default = 1).")
 
-        logger.log(15, f'\tCatboost model hyperparameters: {params}')
+        logger.log(15, f"\tCatboost model hyperparameters: {params}")
 
         extra_fit_kwargs = dict()
-        if params.get('task_type', None) != 'GPU':
+        if params.get("task_type", None) != "GPU":
             callbacks = []
             if early_stopping_rounds is not None:
-                callbacks.append(EarlyStoppingCallback(stopping_rounds=early_stopping_rounds, eval_metric=params['eval_metric']))
+                callbacks.append(EarlyStoppingCallback(stopping_rounds=early_stopping_rounds, eval_metric=params["eval_metric"]))
 
             if num_rows_train * num_cols_train * num_classes > 5_000_000:
                 # The data is large enough to potentially cause memory issues during training, so monitor memory usage via callback.
                 callbacks.append(MemoryCheckCallback())
             if time_limit is not None:
                 time_cur = time.time()
                 time_left = time_limit - (time_cur - time_start)
                 if time_left <= time_limit * 0.4:  # if 60% of time was spent preprocessing, likely not enough time to train model
                     raise TimeLimitExceeded
                 callbacks.append(TimeCheckCallback(time_start=time_cur, time_limit=time_left))
-            extra_fit_kwargs['callbacks'] = callbacks
+            extra_fit_kwargs["callbacks"] = callbacks
         else:
-            logger.log(30, f'\tWarning: CatBoost on GPU is experimental. If you encounter issues, use CPU for training CatBoost instead.')
+            logger.log(30, f"\tWarning: CatBoost on GPU is experimental. If you encounter issues, use CPU for training CatBoost instead.")
             if time_limit is not None:
-                params['iterations'] = self._estimate_iter_in_time_gpu(
+                params["iterations"] = self._estimate_iter_in_time_gpu(
                     X=X,
                     eval_set=eval_set,
                     time_limit=time_limit,
                     verbose=verbose,
                     params=params,
                     num_rows_train=num_rows_train,
                     time_start=time_start,
                     model_type=model_type,
                 )
             if early_stopping_rounds is not None:
                 if isinstance(early_stopping_rounds, int):
-                    extra_fit_kwargs['early_stopping_rounds'] = early_stopping_rounds
+                    extra_fit_kwargs["early_stopping_rounds"] = early_stopping_rounds
                 elif isinstance(early_stopping_rounds, tuple):
-                    extra_fit_kwargs['early_stopping_rounds'] = 50
+                    extra_fit_kwargs["early_stopping_rounds"] = 50
         self.model = model_type(**params)
 
         # TODO: Custom metrics don't seem to work anymore
         # TODO: Custom metrics not supported in GPU mode
         # TODO: Callbacks not supported in GPU mode
         fit_final_kwargs = dict(
             eval_set=eval_set,
             verbose=verbose,
             **extra_fit_kwargs,
         )
 
         if eval_set is not None:
-            fit_final_kwargs['use_best_model'] = True
+            fit_final_kwargs["use_best_model"] = True
 
         self.model.fit(X, **fit_final_kwargs)
 
-        self.params_trained['iterations'] = self.model.tree_count_
+        self.params_trained["iterations"] = self.model.tree_count_
 
     # FIXME: This logic is a hack made to maintain compatibility with GPU CatBoost.
     #  GPU CatBoost does not support callbacks or custom metrics.
     #  Since we use callbacks to check memory and training time in CPU mode, we need a way to estimate these things prior to training for GPU mode.
     #  This method will train a model on a toy number of iterations to estimate memory and training time.
     #  It will return an updated iterations to train on that will avoid running OOM and running over time limit.
     #  Remove this logic once CatBoost fixes GPU support for callbacks and custom metrics.
@@ -227,18 +224,18 @@
         import sys
 
         modifier = min(1.0, 10000 / num_rows_train)
         num_sample_iter_max = max(round(modifier * 50), 2)
         time_left_start = time_limit - (time.time() - time_start)
         if time_left_start <= time_limit * 0.4:  # if 60% of time was spent preprocessing, likely not enough time to train model
             raise TimeLimitExceeded
-        default_iters = params['iterations']
+        default_iters = params["iterations"]
         params_init = params.copy()
-        num_sample_iter = min(num_sample_iter_max, params_init['iterations'])
-        params_init['iterations'] = num_sample_iter
+        num_sample_iter = min(num_sample_iter_max, params_init["iterations"])
+        params_init["iterations"] = num_sample_iter
         sample_model = model_type(
             **params_init,
         )
         sample_model.fit(
             X,
             eval_set=eval_set,
             use_best_model=True,
@@ -263,52 +260,51 @@
         return final_iters
 
     def _predict_proba(self, X, **kwargs):
         if self.problem_type != SOFTCLASS:
             return super()._predict_proba(X, **kwargs)
         # For SOFTCLASS problems, manually transform predictions into probabilities via softmax
         X = self.preprocess(X, **kwargs)
-        y_pred_proba = self.model.predict(X, prediction_type='RawFormulaVal')
+        y_pred_proba = self.model.predict(X, prediction_type="RawFormulaVal")
         y_pred_proba = np.exp(y_pred_proba)
-        y_pred_proba = np.multiply(y_pred_proba, 1/np.sum(y_pred_proba, axis=1)[:, np.newaxis])
+        y_pred_proba = np.multiply(y_pred_proba, 1 / np.sum(y_pred_proba, axis=1)[:, np.newaxis])
         if y_pred_proba.shape[1] == 2:
-            y_pred_proba = y_pred_proba[:,1]
+            y_pred_proba = y_pred_proba[:, 1]
         return y_pred_proba
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             valid_raw_types=[R_BOOL, R_INT, R_FLOAT, R_CATEGORY],
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
-    def _get_early_stopping_rounds(self, num_rows_train, strategy='auto'):
+    def _get_early_stopping_rounds(self, num_rows_train, strategy="auto"):
         return get_early_stopping_rounds(num_rows_train=num_rows_train, strategy=strategy)
 
     def _ag_params(self) -> set:
-        return {'early_stop'}
+        return {"early_stop"}
 
     def _validate_fit_memory_usage(self, mem_error_threshold: float = 1, mem_warning_threshold: float = 0.75, mem_size_threshold: int = 1e9, **kwargs):
-        return super()._validate_fit_memory_usage(mem_error_threshold=mem_error_threshold,
-                                                  mem_warning_threshold=mem_warning_threshold,
-                                                  mem_size_threshold=mem_size_threshold,
-                                                  **kwargs)
+        return super()._validate_fit_memory_usage(
+            mem_error_threshold=mem_error_threshold, mem_warning_threshold=mem_warning_threshold, mem_size_threshold=mem_size_threshold, **kwargs
+        )
 
     def get_minimum_resources(self, is_gpu_available=False):
         minimum_resources = {
-            'num_cpus': 1,
+            "num_cpus": 1,
         }
         if is_gpu_available:
             # Our custom implementation does not support partial GPU. No gpu usage according to nvidia-smi when the `num_gpus` passed to fit is fractional`
-            minimum_resources['num_gpus'] = 0.5
+            minimum_resources["num_gpus"] = 0.5
         return minimum_resources
 
     def _get_default_resources(self):
         # logical=False is faster in training
         num_cpus = ResourceManager.get_cpu_count_psutil(logical=False)
         num_gpus = 0
         return num_cpus, num_gpus
 
     def _more_tags(self):
         # `can_refit_full=True` because iterations is communicated at end of `_fit`
-        return {'can_refit_full': True}
+        return {"can_refit_full": True}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import math
-import numpy as np
 
+import numpy as np
 from catboost import MultiRegressionCustomMetric, MultiRegressionCustomObjective
+
 from autogluon.core.metrics.softclass_metrics import EPS
+
 from .catboost_utils import CustomMetric
 
 
 # Ojectives for SOFTCLASS problem_type
 class SoftclassCustomMetric(CustomMetric):
     def __init__(self, metric, is_higher_better, needs_pred_proba):  # metric is ignored
         super().__init__(metric, is_higher_better, needs_pred_proba)
@@ -23,26 +25,26 @@
             return True
 
         def evaluate(self, approxes, target, weight):
             assert len(target) == len(approxes)
             assert len(target[0]) == len(approxes[0])
             weight_sum = len(target)
             # TODO: inefficient copy of approxes, targets to np.array from provided UniTuple (required for JIT to work)
-            approxes2 = np.zeros((len(approxes[0]),len(approxes)))
-            target2 = np.zeros((len(approxes[0]),len(approxes)))
+            approxes2 = np.zeros((len(approxes[0]), len(approxes)))
+            target2 = np.zeros((len(approxes[0]), len(approxes)))
             for i in range(len(approxes)):
-                approxes2[:,i] = approxes[i]
-                target2[:,i] = target[i]
+                approxes2[:, i] = approxes[i]
+                target2[:, i] = target[i]
             approxes = approxes2
             target = target2
             approxes = np.exp(approxes)
-            approxes = (approxes.T/approxes.sum(axis=1)).T  # softmax
+            approxes = (approxes.T / approxes.sum(axis=1)).T  # softmax
             # Numpy implementation of soft logloss:
             approxes = np.clip(approxes, a_min=EPS, a_max=None)  # clip 0s to avoid NaN
-            approxes = (approxes.T/approxes.sum(axis=1)).T  # renormalize
+            approxes = (approxes.T / approxes.sum(axis=1)).T  # renormalize
             losses = np.multiply(np.log(approxes), target).sum(axis=1)
             error_sum = np.mean(losses)
             return error_sum, weight_sum
             """ The above numpy evaluate() function is necessary for JIT to work and not print warnings, here is the original function (that works without JIT):
             def evaluate(self, approxes, target, weight):
                 assert len(target) == len(approxes)
                 assert len(target[0]) == len(approxes[0])
@@ -65,11 +67,10 @@
         def calc_ders_multi(self, approxes, targets, weight):
             exp_approx = [math.exp(val) for val in approxes]
             # exp_sum = sum(exp_approx)  # not yet supported in numba jit: https://stackoverflow.com/questions/64936311/numba-cannot-determine-numba-type-of-class-builtin-function-or-method, using for loop below instead:
             exp_sum = 0.0
             for x in exp_approx:
                 exp_sum += x
             exp_approx = [val / exp_sum for val in exp_approx]
-            grad = [(targets[j] - exp_approx[j])*weight for j in range(len(targets))]
-            hess = [[(exp_approx[j] * exp_approx[j2] - (j==j2)*exp_approx[j]) * weight
-                    for j in range(len(targets))] for j2 in range(len(targets))]
+            grad = [(targets[j] - exp_approx[j]) * weight for j in range(len(targets))]
+            hess = [[(exp_approx[j] * exp_approx[j2] - (j == j2) * exp_approx[j]) * weight for j in range(len(targets))] for j2 in range(len(targets))]
             return (grad, hess)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
 logger = logging.getLogger(__name__)
 
 
-CATBOOST_QUANTILE_PREFIX = 'MultiQuantile:'
+CATBOOST_QUANTILE_PREFIX = "MultiQuantile:"
 
 
 # TODO: Add weight support?
 # TODO: Can these be optimized? What computational cost do they have compared to the default catboost versions?
 class CustomMetric:
     def __init__(self, metric, is_higher_better, needs_pred_proba):
         self.metric = metric
@@ -26,56 +26,57 @@
     def evaluate(self, approxes, target, weight):
         raise NotImplementedError
 
 
 def get_catboost_metric_from_ag_metric(metric, problem_type, quantile_levels=None):
     if problem_type == SOFTCLASS:
         from .catboost_softclass_utils import SoftclassCustomMetric
-        if metric.name != 'soft_log_loss':
+
+        if metric.name != "soft_log_loss":
             logger.warning("Setting metric=soft_log_loss, the only metric supported for softclass problem_type")
         return SoftclassCustomMetric(metric=None, is_higher_better=True, needs_pred_proba=True)
     elif problem_type == BINARY:
         metric_map = dict(
-            log_loss='Logloss',
-            accuracy='Accuracy',
-            roc_auc='AUC',
-            f1='Logloss',  # f1 uses Logloss because f1 in CatBoost is not reliable (causes errors between versions)
-            f1_macro='Logloss',
-            f1_micro='Logloss',
-            f1_weighted='Logloss',
-            balanced_accuracy='BalancedAccuracy',
-            recall='Recall',
-            recall_macro='Recall',
-            recall_micro='Recall',
-            recall_weighted='Recall',
-            precision='Precision',
-            precision_macro='Precision',
-            precision_micro='Precision',
-            precision_weighted='Precision',
+            log_loss="Logloss",
+            accuracy="Accuracy",
+            roc_auc="AUC",
+            f1="Logloss",  # f1 uses Logloss because f1 in CatBoost is not reliable (causes errors between versions)
+            f1_macro="Logloss",
+            f1_micro="Logloss",
+            f1_weighted="Logloss",
+            balanced_accuracy="BalancedAccuracy",
+            recall="Recall",
+            recall_macro="Recall",
+            recall_micro="Recall",
+            recall_weighted="Recall",
+            precision="Precision",
+            precision_macro="Precision",
+            precision_micro="Precision",
+            precision_weighted="Precision",
         )
-        metric_class = metric_map.get(metric.name, 'Logloss')
+        metric_class = metric_map.get(metric.name, "Logloss")
     elif problem_type == MULTICLASS:
         metric_map = dict(
-            log_loss='MultiClass',
-            accuracy='Accuracy',
+            log_loss="MultiClass",
+            accuracy="Accuracy",
         )
-        metric_class = metric_map.get(metric.name, 'MultiClass')
+        metric_class = metric_map.get(metric.name, "MultiClass")
     elif problem_type == REGRESSION:
         metric_map = dict(
-            mean_squared_error='RMSE',
-            root_mean_squared_error='RMSE',
-            mean_absolute_error='MAE',
-            median_absolute_error='MedianAbsoluteError',
-            r2='R2',
+            mean_squared_error="RMSE",
+            root_mean_squared_error="RMSE",
+            mean_absolute_error="MAE",
+            median_absolute_error="MedianAbsoluteError",
+            r2="R2",
         )
-        metric_class = metric_map.get(metric.name, 'RMSE')
+        metric_class = metric_map.get(metric.name, "RMSE")
     elif problem_type == QUANTILE:
         if quantile_levels is None:
-            raise AssertionError(f'quantile_levels must be provided for problem_type = {problem_type}')
+            raise AssertionError(f"quantile_levels must be provided for problem_type = {problem_type}")
         if not all(0 < q < 1 for q in quantile_levels):
-            raise AssertionError(f'quantile_levels must fulfill 0 < q < 1, provided quantile_levels: {quantile_levels}')
-        quantile_string = ','.join(str(q) for q in quantile_levels)
-        metric_class = f'{CATBOOST_QUANTILE_PREFIX}alpha={quantile_string}'
+            raise AssertionError(f"quantile_levels must fulfill 0 < q < 1, provided quantile_levels: {quantile_levels}")
+        quantile_string = ",".join(str(q) for q in quantile_levels)
+        metric_class = f"{CATBOOST_QUANTILE_PREFIX}alpha={quantile_string}"
     else:
-        raise AssertionError(f'CatBoost does not support {problem_type} problem type.')
+        raise AssertionError(f"CatBoost does not support {problem_type} problem type.")
 
     return metric_class
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,27 @@
         return get_param_regression_baseline()
     else:
         return get_param_binary_baseline()
 
 
 def get_param_binary_baseline():
     params = {
-        'iterations': DEFAULT_ITERATIONS,
-        'learning_rate': 0.05,
+        "iterations": DEFAULT_ITERATIONS,
+        "learning_rate": 0.05,
     }
     return params
 
 
 def get_param_multiclass_baseline(num_classes):
     params = {
-        'iterations': DEFAULT_ITERATIONS,
-        'learning_rate': 0.05,
+        "iterations": DEFAULT_ITERATIONS,
+        "learning_rate": 0.05,
     }
     return params
 
 
 def get_param_regression_baseline():
     params = {
-        'iterations': DEFAULT_ITERATIONS,
-        'learning_rate': 0.05,
+        "iterations": DEFAULT_ITERATIONS,
+        "learning_rate": 0.05,
     }
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Default hyperparameter search spaces used in CatBoost Boosting model """
 from autogluon.common import space
-
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION
 
 
 def get_default_searchspace(problem_type, num_classes=None):
     if problem_type == BINARY:
         return get_searchspace_binary_baseline()
     elif problem_type == MULTICLASS:
@@ -13,30 +12,30 @@
         return get_searchspace_regression_baseline()
     else:
         return get_searchspace_binary_baseline()
 
 
 def get_searchspace_multiclass_baseline(num_classes):
     params = {
-        'learning_rate': space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
-        'depth': space.Int(lower=5, upper=8, default=6),
-        'l2_leaf_reg': space.Real(lower=1, upper=5, default=3),
+        "learning_rate": space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
+        "depth": space.Int(lower=5, upper=8, default=6),
+        "l2_leaf_reg": space.Real(lower=1, upper=5, default=3),
     }
     return params
 
 
 def get_searchspace_binary_baseline():
     params = {
-        'learning_rate': space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
-        'depth': space.Int(lower=5, upper=8, default=6),
-        'l2_leaf_reg': space.Real(lower=1, upper=5, default=3),
+        "learning_rate": space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
+        "depth": space.Int(lower=5, upper=8, default=6),
+        "l2_leaf_reg": space.Real(lower=1, upper=5, default=3),
     }
     return params
 
 
 def get_searchspace_regression_baseline():
     params = {
-        'learning_rate': space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
-        'depth': space.Int(lower=5, upper=8, default=6),
-        'l2_leaf_reg': space.Real(lower=1, upper=5, default=3),
+        "learning_rate": space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
+        "depth": space.Int(lower=5, upper=8, default=6),
+        "l2_leaf_reg": space.Real(lower=1, upper=5, default=3),
     }
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import time
 
-from fastai.callback.core import CancelFitException, Callback
+from fastai.callback.core import Callback, CancelFitException
 from fastai.callback.tracker import TrackerCallback
 from fastcore.basics import store_attr
 
 logger = logging.getLogger(__name__)
 
 
 class BatchTimeTracker(Callback):
@@ -29,79 +29,79 @@
             raise CancelFitException()
 
     def _time_now(self):
         return time.time()
 
 
 class EarlyStoppingCallbackWithTimeLimit(TrackerCallback):
-
-    def __init__(self, monitor='valid_loss', comp=None, min_delta=0., patience=1, reset_on_fit=True, time_limit=None, best_epoch_stop=None):
+    def __init__(self, monitor="valid_loss", comp=None, min_delta=0.0, patience=1, reset_on_fit=True, time_limit=None, best_epoch_stop=None):
         super().__init__(monitor=monitor, comp=comp, min_delta=min_delta, reset_on_fit=reset_on_fit)
         self.patience = patience
         self.time_limit = time_limit
         self.start_time = time.time()
         self.best_epoch_stop = best_epoch_stop
         self.wait = None
 
     def before_fit(self):
         self.wait = 0
         super().before_fit()
 
     def after_epoch(self):
         if self.best_epoch_stop is not None:
             if self.epoch >= self.best_epoch_stop:
-                logger.log(20, f'\tStopping at the best epoch learned earlier - {self.epoch}.')
+                logger.log(20, f"\tStopping at the best epoch learned earlier - {self.epoch}.")
                 raise CancelFitException()
 
         super().after_epoch()
 
         if self.new_best:
             self.wait = 0
         else:
             self.wait += 1
             if self.wait >= self.patience:
-                logger.log(20, f'No improvement since epoch {self.epoch - self.wait}: early stopping')
+                logger.log(20, f"No improvement since epoch {self.epoch - self.wait}: early stopping")
                 raise CancelFitException()
 
         if self.time_limit:
             time_elapsed = time.time() - self.start_time
             time_left = self.time_limit - time_elapsed
             time_per_epoch = time_elapsed / (self.epoch + 1)
             if time_left < time_per_epoch:
-                logger.log(20, f'\tRan out of time, stopping training early. (Stopping on epoch {self.epoch})')
+                logger.log(20, f"\tRan out of time, stopping training early. (Stopping on epoch {self.epoch})")
                 raise CancelFitException()
 
 
 class AgSaveModelCallback(TrackerCallback):
     "A `TrackerCallback` that saves the model's best during training and loads it at the end."
     _only_train_loop = True
 
-    def __init__(self, monitor='valid_loss', comp=None, min_delta=0., fname='model', every_epoch=False,
-                 with_opt=False, reset_on_fit=True, best_epoch_stop=None):
+    def __init__(
+        self, monitor="valid_loss", comp=None, min_delta=0.0, fname="model", every_epoch=False, with_opt=False, reset_on_fit=True, best_epoch_stop=None
+    ):
         super().__init__(monitor=monitor, comp=comp, min_delta=min_delta, reset_on_fit=reset_on_fit)
         # keep track of file path for loggers
         self.last_saved_path = None
         self.best_epoch_stop = best_epoch_stop
-        store_attr('fname,every_epoch,with_opt')
+        store_attr("fname,every_epoch,with_opt")
 
     def _save(self, name):
         self.last_saved_path = self.learn.save(name, with_opt=self.with_opt)
 
     def after_epoch(self):
         "Compare the value monitored to its best score and save if best."
         if self.best_epoch_stop is not None:  # use epoch learned earlier
             if self.epoch >= self.best_epoch_stop:
-                logger.log(15, f'Saving model model at the best epoch learned earlier - {self.epoch}.')
+                logger.log(15, f"Saving model model at the best epoch learned earlier - {self.epoch}.")
                 self.best_epoch = self.epoch
-                self.learn.save(f'{self.fname}')
+                self.learn.save(f"{self.fname}")
         if self.every_epoch:
-            self._save(f'{self.fname}_{self.epoch}')
+            self._save(f"{self.fname}_{self.epoch}")
         else:  # every improvement
             super().after_epoch()
             if self.new_best:
-                logger.log(15, f'Better model found at epoch {self.epoch} with {self.monitor} value: {self.best}.')
+                logger.log(15, f"Better model found at epoch {self.epoch} with {self.monitor} value: {self.best}.")
                 self.best_epoch = self.epoch
-                self._save(f'{self.fname}')
+                self._save(f"{self.fname}")
 
     def after_fit(self, **kwargs):
         if not self.every_epoch:
-            self.learn.load(f'{self.fname}', with_opt=self.with_opt)
+            self.learn.load(f"{self.fname}", with_opt=self.with_opt)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from pathlib import Path
 from typing import Any
 
 import torch
 from fastai.torch_core import flatten_check
 
 
-def export(model, filename_or_stream='export.pkl', pickle_module=pickle, pickle_protocol=2):
-    from fastai.torch_core import rank_distrib
+def export(model, filename_or_stream="export.pkl", pickle_module=pickle, pickle_protocol=2):
     import torch
+    from fastai.torch_core import rank_distrib
+
     "Export the content of `self` without the items and the optimizer state for inference"
-    if rank_distrib(): return  # don't export if child proc
+    if rank_distrib():
+        return  # don't export if child proc
     model._end_cleanup()
     old_dbunch = model.dls
     model.dls = model.dls.new_empty()
     state = model.opt.state_dict() if model.opt is not None else None
     model.opt = None
-    target = open(model.path / filename_or_stream, 'wb') if is_pathlike(filename_or_stream) else filename_or_stream
+    target = open(model.path / filename_or_stream, "wb") if is_pathlike(filename_or_stream) else filename_or_stream
     with warnings.catch_warnings():
         # To avoid the warning that come from PyTorch about model not being checked
         warnings.simplefilter("ignore")
         torch.save(model, target, pickle_module=pickle_module, pickle_protocol=pickle_protocol)
     model.create_opt()
     if state is not None:
         model.opt.load_state_dict(state)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION
 
 
 # TODO this method is generalizable and potentially should be moved out into framework
 def get_param_baseline(problem_type, num_classes=None):
     if problem_type == BINARY:
         return get_param_binary_baseline()
     elif problem_type == MULTICLASS:
@@ -15,31 +15,28 @@
         return get_param_binary_baseline()
 
 
 def get_param_multiclass_baseline():
     # TODO: explore/add other hyperparameters like weight decay, use of batch-norm, activation-function choice, etc.
     params = {
         # See docs: https://docs.fast.ai/tabular.models.html
-        'layers': None,  # layers configuration; None - use model's heuristics
-        'emb_drop': 0.1,  # embedding layers dropout
-        'ps': 0.1,  # linear layers dropout
-        'bs': 'auto',  # batch size
-
+        "layers": None,  # layers configuration; None - use model's heuristics
+        "emb_drop": 0.1,  # embedding layers dropout
+        "ps": 0.1,  # linear layers dropout
+        "bs": "auto",  # batch size
         # maximum learning rate for one cycle policy https://docs.fast.ai/train.html#fit_one_cycle
         # One-cycle policy paper: https://arxiv.org/abs/1803.09820
-        'lr': 1e-2,
-        'epochs': 'auto',  # maximum number of epochs
-
+        "lr": 1e-2,
+        "epochs": "auto",  # maximum number of epochs
         # Early stopping settings. See more details here: https://docs.fast.ai/callbacks.tracker.html#EarlyStoppingCallback
-        'early.stopping.min_delta': 0.0001,
-        'early.stopping.patience': 20,
-
+        "early.stopping.min_delta": 0.0001,
+        "early.stopping.patience": 20,
         # If > 0, then use LabelSmoothingCrossEntropy loss function for binary/multi-class classification;
         # otherwise use default loss function for this type of problem
-        'smoothing': 0.0,
+        "smoothing": 0.0,
     }
     return params
 
 
 def get_param_binary_baseline():
     return get_param_multiclass_baseline()
 
@@ -48,9 +45,9 @@
     return get_param_multiclass_baseline()
 
 
 def get_param_quantile_baseline():
     params = get_param_regression_baseline()
 
     # residual threshold parameter in HuberPinballLoss
-    params.update({'alpha': 0.01})
+    params.update({"alpha": 0.01})
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from autogluon.common import space
-
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION
 
 
 def get_default_searchspace(problem_type, num_classes=None):
     if problem_type == BINARY:
         return get_searchspace_binary().copy()
     elif problem_type == MULTICLASS:
         return get_searchspace_multiclass(num_classes=num_classes)
@@ -15,22 +14,24 @@
     else:
         return get_searchspace_binary().copy()
 
 
 def get_searchspace_binary():
     spaces = {
         # See docs: https://docs.fast.ai/tabular.models.html
-        'layers': space.Categorical(None, [200, 100], [200], [500], [1000], [500, 200], [50, 25], [1000, 500], [200, 100, 50], [500, 200, 100], [1000, 500, 200]),
-        'emb_drop': space.Real(0.0, 0.5, default=0.1),
-        'ps': space.Real(0.0, 0.5, default=0.1),
-        'bs': space.Categorical(256, 64, 128, 512, 1024, 2048, 4096),
-        'lr': space.Real(5e-5, 1e-1, default=1e-2, log=True),
-        'epochs': space.Int(lower=5, upper=30, default=30),
-        'early.stopping.min_delta': 0.0001,
-        'early.stopping.patience': 20,
+        "layers": space.Categorical(
+            None, [200, 100], [200], [500], [1000], [500, 200], [50, 25], [1000, 500], [200, 100, 50], [500, 200, 100], [1000, 500, 200]
+        ),
+        "emb_drop": space.Real(0.0, 0.5, default=0.1),
+        "ps": space.Real(0.0, 0.5, default=0.1),
+        "bs": space.Categorical(256, 64, 128, 512, 1024, 2048, 4096),
+        "lr": space.Real(5e-5, 1e-1, default=1e-2, log=True),
+        "epochs": space.Int(lower=5, upper=30, default=30),
+        "early.stopping.min_delta": 0.0001,
+        "early.stopping.patience": 20,
     }
     return spaces
 
 
 def get_searchspace_multiclass(num_classes):
     return get_searchspace_binary()
 
@@ -39,9 +40,9 @@
     return get_searchspace_binary()
 
 
 def get_searchspace_quantile():
     spaces = get_searchspace_regression()
 
     # residual threshold parameter in HuberPinballLoss
-    spaces.update({'alpha': Categorical(0.001, 0.01, 0.1, 1.0)})
+    spaces.update({"alpha": Categorical(0.001, 0.01, 0.1, 1.0)})
     return spaces
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 "Implements various metrics to measure training accuracy"
+import numpy as np
 import torch
 import torch.nn as nn
-import numpy as np
 from sklearn.isotonic import IsotonicRegression
 
 
 def isotonic(input_data, quantile_list):
     quantile_list = np.array(quantile_list).reshape(-1)
     batch_size = input_data.shape[0]
     new_output_data = []
     for i in range(batch_size):
         new_output_data.append(IsotonicRegression().fit_transform(quantile_list, input_data[i]))
     return np.stack(new_output_data, 0)
 
 
 class HuberPinballLoss(nn.Module):
-    __name__ = 'huber_pinball_loss'
+    __name__ = "huber_pinball_loss"
 
     def __init__(self, quantile_levels, alpha=0.01):
         super(HuberPinballLoss, self).__init__()
         if quantile_levels is not None:
             self.quantile_levels = torch.Tensor(quantile_levels).contiguous().reshape(1, -1)
         else:
             self.quantile_levels = None
@@ -32,17 +32,13 @@
         batch_size = target_data.size()[0]
         predict_data = predict_data.contiguous().reshape(batch_size, -1)
 
         error_data = target_data - predict_data
         if self.alpha == 0.0:
             loss_data = torch.max(self.quantile_levels * error_data, (self.quantile_levels - 1) * error_data)
         else:
-            loss_data = torch.where(torch.abs(error_data) < self.alpha,
-                                    0.5 * error_data * error_data,
-                                    self.alpha * (torch.abs(error_data) - 0.5 * self.alpha))
+            loss_data = torch.where(torch.abs(error_data) < self.alpha, 0.5 * error_data * error_data, self.alpha * (torch.abs(error_data) - 0.5 * self.alpha))
             loss_data = loss_data / self.alpha
 
-            scale = torch.where(error_data >= 0,
-                                torch.ones_like(error_data) * self.quantile_levels,
-                                torch.ones_like(error_data) * (1 - self.quantile_levels))
+            scale = torch.where(error_data >= 0, torch.ones_like(error_data) * self.quantile_levels, torch.ones_like(error_data) * (1 - self.quantile_levels))
             loss_data *= scale
         return loss_data.mean()
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,37 @@
 from builtins import classmethod
 from pathlib import Path
 from typing import Dict, Union
 
 import numpy as np
 import pandas as pd
 import sklearn
-from autogluon.common.features.types import R_OBJECT, R_INT, R_FLOAT, R_DATETIME, R_CATEGORY, R_BOOL, S_TEXT_SPECIAL, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY
+
+from autogluon.common.features.types import (
+    R_BOOL,
+    R_CATEGORY,
+    R_DATETIME,
+    R_FLOAT,
+    R_INT,
+    R_OBJECT,
+    S_TEXT_AS_CATEGORY,
+    S_TEXT_NGRAM,
+    S_TEXT_SPECIAL,
+)
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_fastai
-from autogluon.core.constants import REGRESSION, BINARY, QUANTILE
+from autogluon.core.constants import BINARY, QUANTILE, REGRESSION
 from autogluon.core.hpo.constants import RAY_BACKEND
 from autogluon.core.models import AbstractModel
 from autogluon.core.utils.exceptions import TimeLimitExceeded
 from autogluon.core.utils.files import make_temp_directory
 from autogluon.core.utils.loaders import load_pkl
 from autogluon.core.utils.savers import save_pkl
+
 from .hyperparameters.parameters import get_param_baseline
 from .hyperparameters.searchspaces import get_default_searchspace
 
 # FIXME: Has a leak somewhere, training additional models in a single python script will slow down training for each additional model. Gets very slow after 20+ models (10x+ slowdown)
 #  Slowdown does not appear to impact Mac OS
 # Reproduced with raw torch: https://github.com/pytorch/pytorch/issues/31867
 # https://forums.fast.ai/t/runtimeerror-received-0-items-of-ancdata/48935
@@ -30,86 +42,87 @@
 # https://pytorch.org/docs/master/multiprocessing.html#file-system-file-system
 # Slowdown bug not experienced on Linux if 'torch.multiprocessing.set_sharing_strategy('file_system')' commented out
 # NOTE: If below line is commented out, Torch uses many file descriptors. If issues arise, increase ulimit through 'ulimit -n 2048' or larger. Default on Linux is 1024.
 # torch.multiprocessing.set_sharing_strategy('file_system')
 
 # MacOS issue: torchvision==0.7.0 + torch==1.6.0 can cause segfaults; use torch==1.2.0 torchvision==0.4.0
 
-LABEL = '__label__'
+LABEL = "__label__"
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Takes extremely long time prior to training start if many (10000) continuous features from ngrams, debug - explore TruncateSVD option to reduce input dimensionality
 # TODO: currently fastai automatically detect and use CUDA if available - add code to honor autogluon settings
 class NNFastAiTabularModel(AbstractModel):
-    """ Class for fastai v1 neural network models that operate on tabular data.
+    """Class for fastai v1 neural network models that operate on tabular data.
 
-        Hyperparameters:
-            y_scaler: on a regression problems, the model can give unreasonable predictions on unseen data.
-            This attribute allows to pass a scaler for y values to address this problem. Please note that intermediate
-            iteration metrics will be affected by this transform and as a result intermediate iteration scores will be
-            different from the final ones (these will be correct).
-            https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing
+    Hyperparameters:
+        y_scaler: on a regression problems, the model can give unreasonable predictions on unseen data.
+        This attribute allows to pass a scaler for y values to address this problem. Please note that intermediate
+        iteration metrics will be affected by this transform and as a result intermediate iteration scores will be
+        different from the final ones (these will be correct).
+        https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing
 
-            'layers': list of hidden layers sizes; None - use model's heuristics; default is None
+        'layers': list of hidden layers sizes; None - use model's heuristics; default is None
 
-            'emb_drop': embedding layers dropout; default is 0.1
+        'emb_drop': embedding layers dropout; default is 0.1
 
-            'ps': linear layers dropout - list of values applied to every layer in `layers`; default is [0.1]
+        'ps': linear layers dropout - list of values applied to every layer in `layers`; default is [0.1]
 
-            'bs': batch size; default is 256
+        'bs': batch size; default is 256
 
-            'lr': maximum learning rate for one cycle policy; default is 1e-2;
-            see also https://docs.fast.ai/callback.schedule.html#Learner.fit_one_cycle,
-            One-cycle policy paper: https://arxiv.org/abs/1803.09820
+        'lr': maximum learning rate for one cycle policy; default is 1e-2;
+        see also https://docs.fast.ai/callback.schedule.html#Learner.fit_one_cycle,
+        One-cycle policy paper: https://arxiv.org/abs/1803.09820
 
-            'epochs': number of epochs; default is 30
+        'epochs': number of epochs; default is 30
 
-            # Early stopping settings. See more details here: https://docs.fast.ai/callback.tracker.html#EarlyStoppingCallback
-            'early.stopping.min_delta': 0.0001,
-            'early.stopping.patience': 10,
+        # Early stopping settings. See more details here: https://docs.fast.ai/callback.tracker.html#EarlyStoppingCallback
+        'early.stopping.min_delta': 0.0001,
+        'early.stopping.patience': 10,
     """
 
-    model_internals_file_name = 'model-internals.pkl'
+    model_internals_file_name = "model-internals.pkl"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.cat_columns = None
         self.cont_columns = None
         self.columns_fills = None
         self._columns_fills_names = None
         self.procs = None
         self.y_scaler = None
         self._cont_normalization = None
         self._load_model = None  # Whether to load inner model when loading.
         self._num_cpus_infer = None
 
     def _preprocess_train(self, X, y, X_val, y_val):
-        from fastai.tabular.core import TabularPandas
-        from fastai.data.block import RegressionBlock, CategoryBlock
+        from fastai.data.block import CategoryBlock, RegressionBlock
         from fastai.data.transforms import IndexSplitter
+        from fastai.tabular.core import TabularPandas
         from fastcore.basics import range_of
 
         X = self.preprocess(X, fit=True)
         if X_val is not None:
             X_val = self.preprocess(X_val)
 
         from fastai.tabular.core import Categorify
+
         self.procs = [Categorify]
 
         if self.problem_type in [REGRESSION, QUANTILE] and self.y_scaler is not None:
             y_norm = pd.Series(self.y_scaler.fit_transform(y.values.reshape(-1, 1)).reshape(-1))
             y_val_norm = pd.Series(self.y_scaler.transform(y_val.values.reshape(-1, 1)).reshape(-1)) if y_val is not None else None
-            logger.log(0, f'Training with scaled targets: {self.y_scaler} - !!! NN training metric will be different from the final results !!!')
+            logger.log(0, f"Training with scaled targets: {self.y_scaler} - !!! NN training metric will be different from the final results !!!")
         else:
             y_norm = y
             y_val_norm = y_val
 
-        logger.log(15, f'Using {len(self.cont_columns)} cont features')
+        logger.log(15, f"Using {len(self.cont_columns)} cont features")
         df_train, train_idx, val_idx = self._generate_datasets(X, y_norm, X_val, y_val_norm)
         y_block = RegressionBlock() if self.problem_type in [REGRESSION, QUANTILE] else CategoryBlock()
 
         # Copy cat_columns and cont_columns because TabularList is mutating the list
         data = TabularPandas(
             df_train,
             cat_names=self.cat_columns.copy(),
@@ -128,23 +141,25 @@
             self.cat_columns = self._feature_metadata.get_features(valid_raw_types=[R_OBJECT, R_CATEGORY, R_BOOL])
             if self.cont_columns:
                 self._cont_normalization = (np.array(X[self.cont_columns].mean()), np.array(X[self.cont_columns].std()))
 
             num_cat_cols_og = len(self.cat_columns)
             if self.cat_columns:
                 try:
-                    X_stats = X[self.cat_columns].describe(include='all').T.reset_index()
-                    cat_cols_to_drop = list(X_stats[(X_stats['unique'] > self.params.get('max_unique_categorical_values', 10000)) | (X_stats['unique'].isna())]['index'].values)
+                    X_stats = X[self.cat_columns].describe(include="all").T.reset_index()
+                    cat_cols_to_drop = list(
+                        X_stats[(X_stats["unique"] > self.params.get("max_unique_categorical_values", 10000)) | (X_stats["unique"].isna())]["index"].values
+                    )
                 except:
                     cat_cols_to_drop = []
                 if len(cat_cols_to_drop) != 0:
                     cat_cols_to_drop = set(cat_cols_to_drop)
                     self.cat_columns = [col for col in self.cat_columns if (col not in cat_cols_to_drop)]
             num_cat_cols_use = len(self.cat_columns)
-            logger.log(15, f'Using {num_cat_cols_use}/{num_cat_cols_og} categorical features')
+            logger.log(15, f"Using {num_cat_cols_use}/{num_cat_cols_og} categorical features")
 
             nullable_numeric_features = self._feature_metadata.get_features(valid_raw_types=[R_FLOAT, R_DATETIME], invalid_special_types=[S_TEXT_SPECIAL])
             self.columns_fills = dict()
             self._columns_fills_names = nullable_numeric_features
             for c in self._columns_fills_names:  # No need to do this for int features, int can't have null
                 self.columns_fills[c] = X[c].mean()
         X = self._fill_missing(X)
@@ -175,41 +190,33 @@
                 df = df.fillna(column_fills, inplace=False, downcast=False)
             else:
                 df = df.copy()
         else:
             df = df.copy()
         return df
 
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             time_limit=None,
-             num_cpus=None,
-             num_gpus=0,
-             sample_weight=None,
-             **kwargs):
+    def _fit(self, X, y, X_val=None, y_val=None, time_limit=None, num_cpus=None, num_gpus=0, sample_weight=None, **kwargs):
         try_import_fastai()
-        from fastai.tabular.model import tabular_config
-        from fastai.tabular.learner import tabular_learner
+        import torch
         from fastai import torch_core
+        from fastai.tabular.learner import tabular_learner
+        from fastai.tabular.model import tabular_config
+
         from .callbacks import AgSaveModelCallback, EarlyStoppingCallbackWithTimeLimit
         from .quantile_helpers import HuberPinballLoss
 
-        import torch
         torch.set_num_threads(num_cpus)
         start_time = time.time()
         if sample_weight is not None:  # TODO: support
             logger.log(15, "sample_weight not yet supported for NNFastAiTabularModel, this model will ignore them in training.")
 
         params = self._get_model_params()
-        self._num_cpus_infer = params.pop('_num_cpus_infer', 1)
+        self._num_cpus_infer = params.pop("_num_cpus_infer", 1)
 
-        self.y_scaler = params.get('y_scaler', None)
+        self.y_scaler = params.get("y_scaler", None)
         if self.y_scaler is None:
             if self.problem_type == REGRESSION:
                 self.y_scaler = sklearn.preprocessing.StandardScaler()
             elif self.problem_type == QUANTILE:
                 self.y_scaler = sklearn.preprocessing.MinMaxScaler()
         else:
             self.y_scaler = copy.deepcopy(self.y_scaler)
@@ -218,144 +225,160 @@
             # TODO: Control CPU vs GPU usage during inference
             if num_gpus == 0:
                 torch_core.default_device(False)
             else:
                 # TODO: respect CUDA_VISIBLE_DEVICES to select proper GPU
                 torch_core.default_device(True)
 
-        logger.log(15, f'Fitting Neural Network with parameters {params}...')
+        logger.log(15, f"Fitting Neural Network with parameters {params}...")
         data = self._preprocess_train(X, y, X_val, y_val)
 
         nn_metric, objective_func_name = self.__get_objective_func_name(self.stopping_metric)
         objective_func_name_to_monitor = self.__get_objective_func_to_monitor(objective_func_name)
-        objective_optim_mode = np.less if objective_func_name in [
-            'log_loss',
-            'root_mean_squared_error', 'mean_squared_error', 'mean_absolute_error', 'median_absolute_error',  # Regression objectives
-            'pinball_loss',  # Quantile objective
-        ] else np.greater
+        objective_optim_mode = (
+            np.less
+            if objective_func_name
+            in [
+                "log_loss",
+                "root_mean_squared_error",
+                "mean_squared_error",
+                "mean_absolute_error",
+                "median_absolute_error",  # Regression objectives
+                "pinball_loss",  # Quantile objective
+            ]
+            else np.greater
+        )
 
         # TODO: calculate max emb concat layer size and use 1st layer as that value and 2nd in between number of classes and the value
-        if params.get('layers', None) is not None:
-            layers = params['layers']
+        if params.get("layers", None) is not None:
+            layers = params["layers"]
             if isinstance(layers, tuple):
                 layers = list(layers)
         elif self.problem_type in [REGRESSION, BINARY]:
             layers = [200, 100]
         elif self.problem_type == QUANTILE:
             base_size = max(len(self.quantile_levels) * 4, 128)
             layers = [base_size, base_size, base_size]
         else:
             base_size = max(data.c * 2, 100)
             layers = [base_size * 2, base_size]
 
         loss_func = None
         if self.problem_type == QUANTILE:
-            loss_func = HuberPinballLoss(self.quantile_levels, alpha=self.params['alpha'])
+            loss_func = HuberPinballLoss(self.quantile_levels, alpha=self.params["alpha"])
 
         best_epoch_stop = params.get("best_epoch", None)  # Use best epoch for refit_full.
         batch_size = self._get_batch_size(X)
         dls = data.dataloaders(bs=batch_size)
 
         # Make deterministic
         from fastai.torch_core import set_seed
+
         set_seed(0, True)
         dls.rng.seed(0)
 
         if self.problem_type == QUANTILE:
             dls.c = len(self.quantile_levels)
 
         self.model = tabular_learner(
-            dls, layers=layers, metrics=nn_metric,
-            config=tabular_config(ps=params['ps'], embed_p=params['emb_drop']),
+            dls,
+            layers=layers,
+            metrics=nn_metric,
+            config=tabular_config(ps=params["ps"], embed_p=params["emb_drop"]),
             loss_func=loss_func,
         )
         logger.log(15, self.model.model)
 
-        fname = 'model'
+        fname = "model"
         save_callback = AgSaveModelCallback(
-            monitor=objective_func_name_to_monitor, comp=objective_optim_mode, fname=fname,
-            best_epoch_stop=best_epoch_stop, with_opt=True
+            monitor=objective_func_name_to_monitor, comp=objective_optim_mode, fname=fname, best_epoch_stop=best_epoch_stop, with_opt=True
         )
 
         if time_limit is not None:
             time_elapsed = time.time() - start_time
             time_left = time_limit - time_elapsed
             if time_left <= time_limit * 0.7:  # if 30% of time was spent preprocessing, likely not enough time to train model
                 raise TimeLimitExceeded
         else:
             time_left = None
 
         early_stopping = EarlyStoppingCallbackWithTimeLimit(
             monitor=objective_func_name_to_monitor,
             comp=objective_optim_mode,
-            min_delta=params['early.stopping.min_delta'],
-            patience=params['early.stopping.patience'],
-            time_limit=time_left, best_epoch_stop=best_epoch_stop
+            min_delta=params["early.stopping.min_delta"],
+            patience=params["early.stopping.patience"],
+            time_limit=time_left,
+            best_epoch_stop=best_epoch_stop,
         )
 
         callbacks = [save_callback, early_stopping]
 
         with make_temp_directory() as temp_dir:
             with self.model.no_bar():
                 with self.model.no_logging():
                     original_path = self.model.path
                     self.model.path = Path(temp_dir)
 
                     len_val = len(X_val) if X_val is not None else 0
-                    epochs = self._get_epochs_number(samples_num=len(X) + len_val, epochs=params['epochs'], batch_size=batch_size, time_left=time_left)
+                    epochs = self._get_epochs_number(samples_num=len(X) + len_val, epochs=params["epochs"], batch_size=batch_size, time_left=time_left)
                     if epochs == 0:
                         # Stop early if there is not enough time to train a full epoch
                         raise TimeLimitExceeded
 
-                    self.model.fit_one_cycle(epochs, params['lr'], cbs=callbacks)
+                    self.model.fit_one_cycle(epochs, params["lr"], cbs=callbacks)
 
                     # Load the best one and export it
                     self.model = self.model.load(fname)
 
-                    if objective_func_name == 'log_loss':
+                    if objective_func_name == "log_loss":
                         eval_result = self.model.validate(dl=dls.valid)[0]
                     else:
                         eval_result = self.model.validate(dl=dls.valid)[1]
 
-                    logger.log(15, f'Model validation metrics: {eval_result}')
+                    logger.log(15, f"Model validation metrics: {eval_result}")
                     self.model.path = original_path
 
-            self.params_trained['epochs'] = epochs
-            self.params_trained['best_epoch'] = save_callback.best_epoch
+            self.params_trained["epochs"] = epochs
+            self.params_trained["best_epoch"] = save_callback.best_epoch
 
     def _get_batch_size(self, X, default_batch_size_for_small_inputs=32):
-        bs = self.params['bs']
-        if bs == 'auto':
+        bs = self.params["bs"]
+        if bs == "auto":
             bs = 512 if len(X) >= 200000 else 256
         bs = bs if len(X) > bs else default_batch_size_for_small_inputs
 
-        if self.params['bs'] == 'auto':
-            logger.log(15, f'Automated batch size selection: {bs}')
+        if self.params["bs"] == "auto":
+            logger.log(15, f"Automated batch size selection: {bs}")
 
         return bs
 
     def _get_epochs_number(self, samples_num, epochs, batch_size, time_left=None, min_batches_count=30, default_epochs=30):
-        if epochs == 'auto':
+        if epochs == "auto":
             batches_count = int(samples_num / batch_size) + 1
             if not time_left:
                 return default_epochs
             elif batches_count < min_batches_count:
                 return default_epochs
             else:
                 est_batch_time = self._measure_batch_times(min_batches_count)
                 est_epoch_time = batches_count * est_batch_time * 1.1
                 est_max_epochs = int(time_left / est_epoch_time)
                 epochs = min(default_epochs, est_max_epochs)
                 epochs = max(epochs, 0)
-                logger.log(15, f'Automated epochs selection: training for {epochs} epoch(s). Estimated time budget use {epochs * est_epoch_time:.2f} / {time_left:.2f} sec')
+                logger.log(
+                    15,
+                    f"Automated epochs selection: training for {epochs} epoch(s). Estimated time budget use {epochs * est_epoch_time:.2f} / {time_left:.2f} sec",
+                )
         return epochs
 
     def _measure_batch_times(self, min_batches_count):
         from fastai.callback.core import CancelFitException
+
         from .callbacks import BatchTimeTracker
+
         batch_time_tracker_callback = BatchTimeTracker(batches_to_measure=min_batches_count)
         try:
             with self.model.no_bar():
                 with self.model.no_logging():
                     self.model.fit(1, lr=0, cbs=[batch_time_tracker_callback])
         except CancelFitException:
             pass  # expected early exit
@@ -377,29 +400,29 @@
     def __get_objective_func_name(self, stopping_metric):
         metrics_map = self.__get_metrics_map()
 
         # Unsupported metrics will be replaced by defaults for a given problem type
         objective_func_name = stopping_metric.name
         if objective_func_name not in metrics_map.keys():
             if self.problem_type == REGRESSION:
-                objective_func_name = 'mean_squared_error'
+                objective_func_name = "mean_squared_error"
             elif self.problem_type == QUANTILE:
-                objective_func_name = 'pinball_loss'
+                objective_func_name = "pinball_loss"
             else:
-                objective_func_name = 'log_loss'
-            logger.warning(f'Metric {stopping_metric.name} is not supported by this model - using {objective_func_name} instead')
+                objective_func_name = "log_loss"
+            logger.warning(f"Metric {stopping_metric.name} is not supported by this model - using {objective_func_name} instead")
 
         nn_metric = metrics_map.get(objective_func_name, None)
 
         return nn_metric, objective_func_name
 
     def __get_objective_func_to_monitor(self, objective_func_name):
         monitor_obj_func = {
-            **{k: m.name if hasattr(m, 'name') else m.__name__ for k, m in self.__get_metrics_map().items() if m is not None},
-            'log_loss': 'valid_loss'
+            **{k: m.name if hasattr(m, "name") else m.__name__ for k, m in self.__get_metrics_map().items() if m is not None},
+            "log_loss": "valid_loss",
         }
         objective_func_name_to_monitor = objective_func_name
         if objective_func_name in monitor_obj_func:
             objective_func_name_to_monitor = monitor_obj_func[objective_func_name]
         return objective_func_name_to_monitor
 
     def _predict_proba(self, X, **kwargs):
@@ -421,64 +444,63 @@
         if self.problem_type == REGRESSION:
             if self.y_scaler is not None:
                 return self.y_scaler.inverse_transform(preds.numpy()).reshape(-1)
             else:
                 return preds.numpy().reshape(-1)
         elif self.problem_type == QUANTILE:
             from .quantile_helpers import isotonic
+
             if self.y_scaler is not None:
                 preds = self.y_scaler.inverse_transform(preds.numpy()).reshape(-1, len(self.quantile_levels))
             else:
                 preds = preds.numpy().reshape(-1, len(self.quantile_levels))
             return isotonic(preds, self.quantile_levels)
         elif self.problem_type == BINARY:
             return preds[:, 1].numpy()
         else:
             return preds.numpy()
 
     def save(self, path: str = None, verbose=True) -> str:
         from .fastai_helpers import export
+
         self._load_model = self.model is not None
         __model = self.model
         self.model = None
         path = super().save(path=path, verbose=verbose)
         self.model = __model
         # Export model
         if self._load_model:
-            save_pkl.save_with_fn(
-                f'{path}{self.model_internals_file_name}',
-                self.model,
-                pickle_fn=lambda m, buffer: export(m, buffer),
-                verbose=verbose
-            )
+            save_pkl.save_with_fn(f"{path}{self.model_internals_file_name}", self.model, pickle_fn=lambda m, buffer: export(m, buffer), verbose=verbose)
         self._load_model = None
         return path
 
     @classmethod
     def load(cls, path: str, reset_paths=True, verbose=True):
         from fastai.learner import load_learner
+
         model = super().load(path, reset_paths=reset_paths, verbose=verbose)
         if model._load_model:
             # Need the following logic to allow cross os loading of fastai model
             # https://github.com/fastai/fastai/issues/1482
             import pathlib
             import platform
+
             plt = platform.system()
             og_windows_path = None
-            if plt != 'Windows':
+            if plt != "Windows":
                 og_windows_path = pathlib.WindowsPath
                 pathlib.WindowsPath = pathlib.PosixPath
-            model.model = load_pkl.load_with_fn(f'{model.path}{model.model_internals_file_name}', lambda p: load_learner(p), verbose=verbose)
+            model.model = load_pkl.load_with_fn(f"{model.path}{model.model_internals_file_name}", lambda p: load_learner(p), verbose=verbose)
             if og_windows_path is not None:
                 pathlib.WindowsPath = og_windows_path
         model._load_model = None
         return model
 
     def _set_default_params(self):
-        """ Specifies hyperparameter values to use by default """
+        """Specifies hyperparameter values to use by default"""
         default_params = get_param_baseline(self.problem_type)
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_searchspace(self):
         return get_default_searchspace(self.problem_type, num_classes=None)
 
@@ -494,67 +516,61 @@
     def _get_default_resources(self):
         # logical=False is faster in training
         num_cpus = ResourceManager.get_cpu_count_psutil(logical=False)
         num_gpus = 0
         return num_cpus, num_gpus
 
     def __get_metrics_map(self):
-        from fastai.metrics import rmse, mse, mae, accuracy, FBeta, RocAucBinary, Precision, Recall, R2Score
+        from fastai.metrics import FBeta, Precision, R2Score, Recall, RocAucBinary, accuracy, mae, mse, rmse
+
         from .fastai_helpers import medae
         from .quantile_helpers import HuberPinballLoss
+
         metrics_map = {
             # Regression
-            'root_mean_squared_error': rmse,
-            'mean_squared_error': mse,
-            'mean_absolute_error': mae,
-            'r2': R2Score(),
-            'median_absolute_error': medae,
-
+            "root_mean_squared_error": rmse,
+            "mean_squared_error": mse,
+            "mean_absolute_error": mae,
+            "r2": R2Score(),
+            "median_absolute_error": medae,
             # Classification
-            'accuracy': accuracy,
-
-            'f1': FBeta(beta=1),
-            'f1_macro': FBeta(beta=1, average='macro'),
-            'f1_micro': FBeta(beta=1, average='micro'),
-            'f1_weighted': FBeta(beta=1, average='weighted'),  # this one has some issues
-
-            'roc_auc': RocAucBinary(),
-
-            'precision': Precision(),
-            'precision_macro': Precision(average='macro'),
-            'precision_micro': Precision(average='micro'),
-            'precision_weighted': Precision(average='weighted'),
-
-            'recall': Recall(),
-            'recall_macro': Recall(average='macro'),
-            'recall_micro': Recall(average='micro'),
-            'recall_weighted': Recall(average='weighted'),
-            'log_loss': None,
-
-            'pinball_loss': HuberPinballLoss(quantile_levels=self.quantile_levels)
+            "accuracy": accuracy,
+            "f1": FBeta(beta=1),
+            "f1_macro": FBeta(beta=1, average="macro"),
+            "f1_micro": FBeta(beta=1, average="micro"),
+            "f1_weighted": FBeta(beta=1, average="weighted"),  # this one has some issues
+            "roc_auc": RocAucBinary(),
+            "precision": Precision(),
+            "precision_macro": Precision(average="macro"),
+            "precision_micro": Precision(average="micro"),
+            "precision_weighted": Precision(average="weighted"),
+            "recall": Recall(),
+            "recall_macro": Recall(average="macro"),
+            "recall_micro": Recall(average="micro"),
+            "recall_weighted": Recall(average="weighted"),
+            "log_loss": None,
+            "pinball_loss": HuberPinballLoss(quantile_levels=self.quantile_levels)
             # Not supported: pac_score
         }
         return metrics_map
 
     def _estimate_memory_usage(self, X, **kwargs):
         return 10 * get_approximate_df_mem_usage(X).sum()
-    
+
     def _get_hpo_backend(self):
         """Choose which backend(Ray or Custom) to use for hpo"""
         return RAY_BACKEND
-    
+
     def _get_maximum_resources(self) -> Dict[str, Union[int, float]]:
         # fastai model trains slower when utilizing virtual cores and this issue scale up when the number of cpu cores increases
-        return {
-            "num_cpus": ResourceManager.get_cpu_count_psutil(logical=False)
-        }
+        return {"num_cpus": ResourceManager.get_cpu_count_psutil(logical=False)}
 
     def get_minimum_resources(self, is_gpu_available=False):
         minimum_resources = {
-            'num_cpus': 1,
+            "num_cpus": 1,
         }
         if is_gpu_available:
-            minimum_resources['num_gpus'] = 0.5
+            minimum_resources["num_gpus"] = 0.5
         return minimum_resources
 
     def _more_tags(self):
-        return {'can_refit_full': True}
+        return {"can_refit_full": True}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import logging
 import os
 import tempfile
 
 import numpy as np
 import pandas as pd
 
+from autogluon.common.features.types import S_TEXT
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_fasttext
-from autogluon.common.features.types import S_TEXT
 from autogluon.core.constants import BINARY, MULTICLASS
 from autogluon.core.models import AbstractModel
 
 from .hyperparameters.parameters import get_param_baseline
 
 logger = logging.getLogger(__name__)
 
@@ -42,42 +42,36 @@
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     @classmethod
     def _get_default_ag_args(cls) -> dict:
         default_ag_args = super()._get_default_ag_args()
-        extra_ag_args = {'valid_stacker': False, 'problem_types': [BINARY, MULTICLASS]}
+        extra_ag_args = {"valid_stacker": False, "problem_types": [BINARY, MULTICLASS]}
         default_ag_args.update(extra_ag_args)
         return default_ag_args
 
-    def _fit(self,
-             X,
-             y,
-             sample_weight=None,
-             **kwargs):
+    def _fit(self, X, y, sample_weight=None, **kwargs):
         if self.problem_type not in (BINARY, MULTICLASS):
-            raise ValueError(
-                "FastText model only supports binary or multiclass classification"
-            )
+            raise ValueError("FastText model only supports binary or multiclass classification")
 
         try_import_fasttext()
         import fasttext
 
         params = self._get_model_params()
-        quantize_model = params.pop('quantize_model', True)
+        quantize_model = params.pop("quantize_model", True)
 
-        verbosity = kwargs.get('verbosity', 2)
-        if 'verbose' not in params:
+        verbosity = kwargs.get("verbosity", 2)
+        if "verbose" not in params:
             if verbosity <= 2:
-                params['verbose'] = 0
+                params["verbose"] = 0
             elif verbosity == 3:
-                params['verbose'] = 1
+                params["verbose"] = 1
             else:
-                params['verbose'] = 2
+                params["verbose"] = 2
 
         if sample_weight is not None:
             logger.log(15, "sample_weight not yet supported for FastTextModel, this model will ignore them in training.")
 
         X = self.preprocess(X)
 
         self._label_dtype = y.dtype
@@ -102,16 +96,15 @@
 
     # TODO: move logic to self._preprocess_nonadaptive()
     # TODO: text features: alternate text preprocessing steps
     # TODO: categorical features: special encoding:  <feature name>_<feature value>
     def _preprocess(self, X: pd.DataFrame, **kwargs) -> list:
         X = super()._preprocess(X, **kwargs)
         text_col = (
-            X
-            .astype(str)
+            X.astype(str)
             .fillna(" ")
             .apply(lambda r: " ".join(v for v in r.values), axis=1)
             .str.lower()
             .str.replace("<.*?>", " ")  # remove html tags
             # .str.replace('''(\\d[\\d,]*)(\\.\\d+)?''', ' __NUMBER__ ') # process numbers preserve dot
             .str.replace("""([\\W])""", " \\1 ")  # separate special characters
             .str.replace("\\s", " ")
@@ -131,17 +124,15 @@
     def _predict_proba(self, X: pd.DataFrame, **kwargs) -> np.ndarray:
         X = self.preprocess(X, **kwargs)
 
         pred_labels, pred_probs = self.model.predict(X, k=len(self.model.labels))
 
         recs = []
         for labels, probs in zip(pred_labels, pred_probs):
-            recs.append(
-                dict(zip((self._label_inv_map[label] for label in labels), probs))
-            )
+            recs.append(dict(zip((self._label_inv_map[label] for label in labels), probs)))
 
         y_pred_proba: np.ndarray = pd.DataFrame(recs).sort_index(axis=1).values
         return self._convert_proba_to_unified_form(y_pred_proba)
 
     def save(self, path: str = None, verbose=True) -> str:
         self._load_model = self.model is not None
         # pickle model parts
@@ -161,26 +152,27 @@
     def load(cls, path: str, reset_paths=True, verbose=True):
         model: FastTextModel = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
 
         # load binary fasttext model
         if model._load_model:
             try_import_fasttext()
             import fasttext
+
             fasttext_model_file_name = model.path + cls.model_bin_file_name
             # TODO: hack to subpress a deprecation warning from fasttext
             # remove it once official fasttext is updated beyond 0.9.2
             # https://github.com/facebookresearch/fastText/issues/1067
-            with open(os.devnull, 'w') as f, contextlib.redirect_stderr(f):
+            with open(os.devnull, "w") as f, contextlib.redirect_stderr(f):
                 model.model = fasttext.load_model(fasttext_model_file_name)
         model._load_model = None
         return model
 
     def get_memory_size(self) -> int:
         return self._model_size_estimate
 
     def _more_tags(self):
         # `can_refit_full=True` because validation data is not used and there is no form of early stopping implemented.
-        return {'can_refit_full': True}
+        return {"can_refit_full": True}
 
     @classmethod
     def _class_tags(cls):
-        return {'handles_text': True}
+        return {"handles_text": True}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import numpy as np
 import pandas as pd
 
 from autogluon.common.features.types import R_OBJECT, S_IMAGE_PATH
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, SOFTCLASS
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
 from ..automm.automm_model import MultiModalPredictorModel
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Handle multiple image columns?
@@ -18,14 +18,15 @@
 class ImagePredictorModel(MultiModalPredictorModel):
     """
     MultimodalPredictor that only uses image features.
     Currently only supports 1 image column, with 1 image per sample.
     Additionally has special null image handling to improve performance in the presence of null images (aka image path of '')
         Note: null handling has not been compared to the built-in null handling of MultimodalPredictor yet.
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._dummy_pred_proba = None  # Dummy value to predict if image is NaN
         self._image_col_name = None
 
     @property
     def _has_predict_proba(self):
@@ -42,60 +43,60 @@
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     @classmethod
     def _get_default_ag_args(cls) -> dict:
         default_ag_args = super()._get_default_ag_args()
         extra_ag_args = {
-            'valid_stacker': False,
-            'problem_types': [BINARY, MULTICLASS, REGRESSION],
+            "valid_stacker": False,
+            "problem_types": [BINARY, MULTICLASS, REGRESSION],
         }
         default_ag_args.update(extra_ag_args)
         return default_ag_args
 
     def preprocess_fit(self, X, y, X_val=None, y_val=None, **kwargs):
         X, y, X_val, y_val = super().preprocess_fit(X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
         X_features = list(X.columns)
         if len(X_features) != 1:
-            raise AssertionError(f'ImagePredictorModel only supports one image feature, but {len(X_features)} were given: {X_features}')
+            raise AssertionError(f"ImagePredictorModel only supports one image feature, but {len(X_features)} were given: {X_features}")
         self._image_col_name = X_features[0]
-        null_indices = X[self._image_col_name] == ''
+        null_indices = X[self._image_col_name] == ""
 
         # TODO: Consider some kind of weighting of the two options so there isn't a harsh cutoff at 50
         # FIXME: What if all rows in a class are null? Will probably crash.
         if null_indices.sum() > 50:
             self._dummy_pred_proba = self._compute_dummy_pred_proba(y[null_indices])  # FIXME: Do this one for better results
         else:
             # Not enough null to get a confident estimate of null label average, instead use all data average
             self._dummy_pred_proba = self._compute_dummy_pred_proba(y)
 
         if null_indices.sum() > 0:
             X = X[~null_indices]
             y = y[~null_indices]
 
         if X_val is not None:
-            null_indices_val = X_val[self._image_col_name] == ''
+            null_indices_val = X_val[self._image_col_name] == ""
             if null_indices_val.sum() > 0:
                 X_val = X_val[~null_indices_val]
                 y_val = y_val[~null_indices_val]
 
         return X, y, X_val, y_val
 
     def _predict_proba(self, X, **kwargs):
         X = self.preprocess(X, **kwargs)
         pred_method = self.model.predict_proba if self._has_predict_proba else self.model.predict
         # TODO: Add option to crash if null is present for faster predict_proba
-        null_indices = X[self._image_col_name] == ''
+        null_indices = X[self._image_col_name] == ""
         if null_indices.sum() > 0:
             if self.num_classes is None:
                 y_pred_proba = np.zeros(len(X))
             else:
                 y_pred_proba = np.zeros((len(X), self.num_classes))
             X = X.reset_index(drop=True)
-            null_indices = X[self._image_col_name] == ''
+            null_indices = X[self._image_col_name] == ""
             X = X[~null_indices]
             null_indices_rows = list(null_indices[null_indices].index)
             non_null_indices_rows = list(null_indices[~null_indices].index)
             y_pred_proba[null_indices_rows] = self._dummy_pred_proba
             y_pred_proba[non_null_indices_rows] = pred_method(X, as_pandas=False)
         else:
             y_pred_proba = pred_method(X, as_pandas=False)
@@ -114,9 +115,9 @@
                         dummies[c] = 0
             dummies = dummies[list(range(num_classes))]
             pred_proba_mean = dummies.mean().values
 
         elif self.problem_type in [REGRESSION, QUANTILE, SOFTCLASS]:
             pred_proba_mean = y.mean()
         else:
-            raise NotImplementedError(f'Computing dummy pred_proba is not implemented for {self.problem_type}.')
+            raise NotImplementedError(f"Computing dummy pred_proba is not implemented for {self.problem_type}.")
         return pred_proba_mean
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
     @abstractmethod
     def get_model(self):
         return NotImplemented
 
     def get_info(self):
         info = super().get_info()
-        info['complexity'] = self.model.complexity_
+        info["complexity"] = self.model.complexity_
         return info
 
     def _preprocess(self, X: pd.DataFrame, is_train=False, **kwargs) -> pd.DataFrame:
         X = super()._preprocess(X, **kwargs)
         if is_train:
-            self._categorical_featnames = self._feature_metadata.get_features(valid_raw_types=['category'])
-            self._other_featnames = self._feature_metadata.get_features(invalid_raw_types=['category'])
+            self._categorical_featnames = self._feature_metadata.get_features(valid_raw_types=["category"])
+            self._other_featnames = self._feature_metadata.get_features(invalid_raw_types=["category"])
             if self._categorical_featnames:
-                self._ohe = OneHotEncoder(dtype=np.uint8, handle_unknown='ignore')
+                self._ohe = OneHotEncoder(dtype=np.uint8, handle_unknown="ignore")
                 self._ohe.fit(X=X[self._categorical_featnames])
                 self._ohe_columns = self._ohe.get_feature_names_out()
             else:
                 self._ohe = None  # otherwise no model is fitted when there are not self._categorical_featnames
 
         if self._ohe is not None:
             X_index = X.index
@@ -45,95 +45,87 @@
             if self._other_featnames:
                 X = pd.concat([X[self._other_featnames], X_ohe], axis=1)
             else:
                 X = X_ohe
 
         return X.fillna(0)
 
-    def _fit(self,
-             X: pd.DataFrame,  # training data
-             y: pd.Series,  # training labels
-             **kwargs):
+    def _fit(self, X: pd.DataFrame, y: pd.Series, **kwargs):  # training data  # training labels
 
         model_cls = self.get_model()
         X = self.preprocess(X, is_train=True)
         params = self._get_model_params()
         self.model = model_cls(**params)
         self.model.fit(X, y, feature_names=X.columns.values.tolist())
 
     def _set_default_params(self):
         default_params = {
-            'random_state': 0,
+            "random_state": 0,
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             get_features_kwargs=dict(
-                valid_raw_types=['int', 'float', 'category'],
+                valid_raw_types=["int", "float", "category"],
             ),
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
 
 class RuleFitModel(_IModelsModel):
-
     def get_model(self):
         try_import_imodels()
-        from imodels import RuleFitRegressor, RuleFitClassifier
+        from imodels import RuleFitClassifier, RuleFitRegressor
 
-        if self.problem_type in ['regression', 'softclass']:
+        if self.problem_type in ["regression", "softclass"]:
             return RuleFitRegressor
         else:
             return RuleFitClassifier
 
 
 class GreedyTreeModel(_IModelsModel):
-
     def get_model(self):
         try_import_imodels()
         from imodels import GreedyTreeClassifier
         from sklearn.tree import DecisionTreeRegressor
 
-        if self.problem_type in ['regression', 'softclass']:
+        if self.problem_type in ["regression", "softclass"]:
             return DecisionTreeRegressor
         else:
             return GreedyTreeClassifier
 
 
 class BoostedRulesModel(_IModelsModel):
-
     def get_model(self):
         try_import_imodels()
         from imodels import BoostedRulesClassifier
 
-        if self.problem_type in ['binary']:
+        if self.problem_type in ["binary"]:
             return BoostedRulesClassifier
         else:
-            raise Exception('Boosted Rule Set only supports binary classification!')
+            raise Exception("Boosted Rule Set only supports binary classification!")
 
 
 class HSTreeModel(_IModelsModel):
-
     def get_model(self):
         try_import_imodels()
-        from imodels import HSTreeRegressorCV, HSTreeClassifierCV
+        from imodels import HSTreeClassifierCV, HSTreeRegressorCV
 
-        if self.problem_type in ['regression', 'softclass']:
+        if self.problem_type in ["regression", "softclass"]:
             return HSTreeRegressorCV
         else:
             return HSTreeClassifierCV
 
 
 class FigsModel(_IModelsModel):
-
     def get_model(self):
         try_import_imodels()
-        from imodels import FIGSClassifier, 	FIGSRegressor
+        from imodels import FIGSClassifier, FIGSRegressor
 
-        if self.problem_type in ['regression', 'softclass']:
+        if self.problem_type in ["regression", "softclass"]:
             return FIGSRegressor
         else:
             return FIGSClassifier
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # These are variants of sklearn KNN models which have the ability to calculate unbiased predictions on the training data via leave-one-out (LOO) calculation.
 # TODO: Consider contributing to sklearn officially
 # TODO: This uses private methods in sklearn, could potentially break without warning in future sklearn releases
 # TODO: Code is largely identical to `predict` and `predict_proba` methods, but due to how those methods are coded, we can't call them directly.
 #  This means if code within those methods changes, the LOO equivalents may start to become outdated.
 
-__all__ = ['KNeighborsClassifierLOOMixin', 'KNeighborsRegressorLOOMixin']
+__all__ = ["KNeighborsClassifierLOOMixin", "KNeighborsRegressorLOOMixin"]
 
 
 class KNeighborsClassifierLOOMixin:
     @staticmethod
     def predict_loo(self):
         """Predict the class labels for the training data via leave-one-out.
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import logging
-
-import numpy as np
 import math
 import time
-
 from typing import Dict, Union
 
-from autogluon.common.features.types import R_INT, R_FLOAT, S_BOOL
+import numpy as np
+
+from autogluon.common.features.types import R_FLOAT, R_INT, S_BOOL
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION
-from autogluon.core.utils.exceptions import NotEnoughMemoryError
 from autogluon.core.models import AbstractModel
+from autogluon.core.utils.exceptions import NotEnoughMemoryError
 from autogluon.core.utils.utils import normalize_pred_probas
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Normalize data!
 class KNNModel(AbstractModel):
     """
     KNearestNeighbors model (scikit-learn): https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._X_unused_index = None  # Keeps track of unused training data indices, necessary for LOO OOF generation
 
     def _get_model_type(self):
-        if self.params_aux.get('use_daal', True):
+        if self.params_aux.get("use_daal", True):
             try:
                 # TODO: Add more granular switch, currently this affects all future KNN models even if they had `use_daal=False`
                 from sklearnex.neighbors import KNeighborsClassifier, KNeighborsRegressor
+
                 # sklearnex backend for KNN seems to be 20-40x+ faster than native sklearn with no downsides.
-                logger.log(15, '\tUsing sklearnex KNN backend...')
+                logger.log(15, "\tUsing sklearnex KNN backend...")
             except:
                 from sklearn.neighbors import KNeighborsClassifier, KNeighborsRegressor
         else:
             from sklearn.neighbors import KNeighborsClassifier, KNeighborsRegressor
         if self.problem_type == REGRESSION:
             return KNeighborsRegressor
         else:
@@ -44,15 +45,15 @@
     def _preprocess(self, X, **kwargs):
         X = super()._preprocess(X, **kwargs)
         X = X.fillna(0).to_numpy(dtype=np.float32)
         return X
 
     def _set_default_params(self):
         default_params = {
-            'weights': 'uniform',
+            "weights": "uniform",
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
@@ -61,62 +62,55 @@
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     @classmethod
     def _get_default_ag_args(cls) -> dict:
         default_ag_args = super()._get_default_ag_args()
-        extra_ag_args = {'valid_stacker': False}
+        extra_ag_args = {"valid_stacker": False}
         default_ag_args.update(extra_ag_args)
         return default_ag_args
 
     @classmethod
     def _get_default_ag_args_ensemble(cls, **kwargs) -> dict:
         default_ag_args_ensemble = super()._get_default_ag_args_ensemble(**kwargs)
-        extra_ag_args_ensemble = {'use_child_oof': True}
+        extra_ag_args_ensemble = {"use_child_oof": True}
         default_ag_args_ensemble.update(extra_ag_args_ensemble)
         return default_ag_args_ensemble
 
     # TODO: Enable HPO for KNN
     def _get_default_searchspace(self):
         spaces = {}
         return spaces
 
-    def _fit(self,
-             X,
-             y,
-             num_cpus=-1,
-             time_limit=None,
-             sample_weight=None,
-             **kwargs):
+    def _fit(self, X, y, num_cpus=-1, time_limit=None, sample_weight=None, **kwargs):
         time_start = time.time()
         X = self.preprocess(X)
         params = self._get_model_params()
-        if 'n_jobs' not in params:
-            params['n_jobs'] = num_cpus
+        if "n_jobs" not in params:
+            params["n_jobs"] = num_cpus
         if sample_weight is not None:  # TODO: support
             logger.log(15, "sample_weight not yet supported for KNNModel, this model will ignore them in training.")
 
         num_rows_max = len(X)
         # FIXME: v0.1 Must store final num rows for refit_full or else will use everything! Worst case refit_full could train far longer than the original model.
         if time_limit is None or num_rows_max <= 10000:
             self.model = self._get_model_type()(**params).fit(X, y)
         else:
             self.model = self._fit_with_samples(X=X, y=y, model_params=params, time_limit=time_limit - (time.time() - time_start))
 
     def _estimate_memory_usage(self, X, **kwargs):
         model_size_bytes = 4 * X.shape[0] * X.shape[1]  # Assuming float32 types
-        expected_final_model_size_bytes = model_size_bytes * 3.6 # Roughly what can be expected of the final KNN model in memory size
+        expected_final_model_size_bytes = model_size_bytes * 3.6  # Roughly what can be expected of the final KNN model in memory size
         return expected_final_model_size_bytes
 
     def _validate_fit_memory_usage(self, mem_error_threshold: float = 0.2, mem_warning_threshold: float = 0.15, mem_size_threshold: int = 1e7, **kwargs):
-        return super()._validate_fit_memory_usage(mem_error_threshold=mem_error_threshold,
-                                                  mem_warning_threshold=mem_warning_threshold,
-                                                  mem_size_threshold=mem_size_threshold,
-                                                  **kwargs)
+        return super()._validate_fit_memory_usage(
+            mem_error_threshold=mem_error_threshold, mem_warning_threshold=mem_warning_threshold, mem_size_threshold=mem_size_threshold, **kwargs
+        )
 
     # TODO: Won't work for RAPIDS without modification
     # TODO: Technically isn't OOF, but can be used inplace of OOF. Perhaps rename to something more accurate?
     def get_oof_pred_proba(self, X, normalize=None, **kwargs):
         """X should be the same X passed to `.fit`"""
         y_oof_pred_proba = self._get_oof_pred_proba(X=X, **kwargs)
         if normalize is None:
@@ -124,14 +118,15 @@
         if normalize:
             y_oof_pred_proba = normalize_pred_probas(y_oof_pred_proba, self.problem_type)
         y_oof_pred_proba = y_oof_pred_proba.astype(np.float32)
         return y_oof_pred_proba
 
     def _get_oof_pred_proba(self, X, **kwargs):
         from ._knn_loo_variants import KNeighborsClassifierLOOMixin, KNeighborsRegressorLOOMixin
+
         if self.problem_type in [BINARY, MULTICLASS]:
             y_oof_pred_proba = KNeighborsClassifierLOOMixin.predict_proba_loo(self.model)
         else:
             y_oof_pred_proba = KNeighborsRegressorLOOMixin.predict_loo(self.model)
         y_oof_pred_proba = self._convert_proba_to_unified_form(y_oof_pred_proba)
         if X is not None and self._X_unused_index:
             X_unused = X.iloc[self._X_unused_index]
@@ -148,23 +143,15 @@
                 y_oof_tmp = np.zeros((num_rows, oof_pred_shape[1]), dtype=np.float32)
                 y_oof_tmp[X_used_index, :] = y_oof_pred_proba
                 y_oof_tmp[self._X_unused_index, :] = y_pred_proba_new
             y_oof_pred_proba = y_oof_tmp
         return y_oof_pred_proba
 
     # TODO: Consider making this fully generic and available to all models
-    def _fit_with_samples(self,
-                          X,
-                          y,
-                          model_params,
-                          time_limit,
-                          start_samples=10000,
-                          max_samples=None,
-                          sample_growth_factor=2,
-                          sample_time_growth_factor=8):
+    def _fit_with_samples(self, X, y, model_params, time_limit, start_samples=10000, max_samples=None, sample_growth_factor=2, sample_time_growth_factor=8):
         """
         Fit model with samples of the data repeatedly, gradually increasing the amount of data until time_limit is reached or all data is used.
 
         X and y must already be preprocessed.
 
         Parameters
         ----------
@@ -206,86 +193,88 @@
 
         def sample_func(chunk, frac):
             # Guarantee at least 1 sample (otherwise log_loss would crash or model would return different column counts in pred_proba)
             n = max(math.ceil(len(chunk) * frac), 1)
             return chunk.sample(n=n, replace=False, random_state=0)
 
         if self.problem_type != REGRESSION:
-            y_df = y.to_frame(name='label').reset_index(drop=True)
+            y_df = y.to_frame(name="label").reset_index(drop=True)
         else:
             y_df = None
 
         time_start_sample_loop = time.time()
         time_limit_left = time_limit - (time_start_sample_loop - time_start)
         model_type = self._get_model_type()
         idx = None
         for i, samples in enumerate(num_rows_samples):
             if samples != num_rows_max:
                 if self.problem_type == REGRESSION:
                     idx = np.random.choice(num_rows_max, size=samples, replace=False)
                 else:
-                    idx = y_df.groupby('label', group_keys=False).apply(sample_func, frac=samples/num_rows_max).index
+                    idx = y_df.groupby("label", group_keys=False).apply(sample_func, frac=samples / num_rows_max).index
                 X_samp = X[idx, :]
                 y_samp = y.iloc[idx]
             else:
                 X_samp = X
                 y_samp = y
                 idx = None
             self.model = model_type(**model_params).fit(X_samp, y_samp)
             time_limit_left_prior = time_limit_left
             time_fit_end_sample = time.time()
             time_limit_left = time_limit - (time_fit_end_sample - time_start)
             time_fit_sample = time_limit_left_prior - time_limit_left
             time_required_for_next = time_fit_sample * sample_time_growth_factor
-            logger.log(15, f'\t{round(time_fit_sample, 2)}s \t= Train Time (Using {samples}/{num_rows_max} rows) ({round(time_limit_left, 2)}s remaining time)')
+            logger.log(15, f"\t{round(time_fit_sample, 2)}s \t= Train Time (Using {samples}/{num_rows_max} rows) ({round(time_limit_left, 2)}s remaining time)")
             if time_required_for_next > time_limit_left and i != len(num_rows_samples) - 1:
-                logger.log(20, f'\tNot enough time to train KNN model on all training rows. Fit {samples}/{num_rows_max} rows. (Training KNN model on {num_rows_samples[i+1]} rows is expected to take {round(time_required_for_next, 2)}s)')
+                logger.log(
+                    20,
+                    f"\tNot enough time to train KNN model on all training rows. Fit {samples}/{num_rows_max} rows. (Training KNN model on {num_rows_samples[i+1]} rows is expected to take {round(time_required_for_next, 2)}s)",
+                )
                 break
         if idx is not None:
             idx = set(idx)
             self._X_unused_index = [i for i in range(num_rows_max) if i not in idx]
         return self.model
-    
+
     def _get_maximum_resources(self) -> Dict[str, Union[int, float]]:
         # use at most 32 cpus to avoid OpenBLAS error: https://github.com/autogluon/autogluon/issues/1020
-        return {
-            "num_cpus": 32
-        }
+        return {"num_cpus": 32}
 
     def _get_default_resources(self):
         # use at most 32 cpus to avoid OpenBLAS error: https://github.com/autogluon/autogluon/issues/1020
         num_cpus = ResourceManager.get_cpu_count()
         num_gpus = 0
         return num_cpus, num_gpus
 
     def _more_tags(self):
         return {
-            'valid_oof': True,
-            'can_refit_full': True,
+            "valid_oof": True,
+            "can_refit_full": True,
         }
 
 
 class FAISSModel(KNNModel):
     def _get_model_type(self):
         from .knn_utils import FAISSNeighborsClassifier, FAISSNeighborsRegressor
+
         if self.problem_type == REGRESSION:
             return FAISSNeighborsRegressor
         else:
             return FAISSNeighborsClassifier
 
     def _set_default_params(self):
         default_params = {
-            'index_factory_string': 'Flat',
+            "index_factory_string": "Flat",
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
         super()._set_default_params()
 
     @classmethod
     def _get_default_ag_args_ensemble(cls, **kwargs) -> dict:
         default_ag_args_ensemble = super()._get_default_ag_args_ensemble(**kwargs)
-        extra_ag_args_ensemble = {'use_child_oof': False}
+        extra_ag_args_ensemble = {"use_child_oof": False}
         default_ag_args_ensemble.update(extra_ag_args_ensemble)
         return default_ag_args_ensemble
 
     def _more_tags(self):
-        return {'valid_oof': False}
+        return {"valid_oof": False}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
-from autogluon.core.constants import REGRESSION
 from autogluon.common.utils.try_import import try_import_rapids_cuml
+from autogluon.core.constants import REGRESSION
 
-from .knn_model import KNNModel
 from .._utils.rapids_utils import RapidsModelMixin
+from .knn_model import KNNModel
 
 logger = logging.getLogger(__name__)
 
 
 # FIXME: Benchmarks show that CPU KNN can be trained in ~3 seconds with 0.2 second validation time for CoverType on automlbenchmark (m5.2xlarge)
 #  This is over 100 seconds validation time on CPU with rapids installed, investigate how it was so fast on CPU.
 #  "2021_02_26/autogluon_hpo_auto.openml_s_271.1h8c.aws.20210228T000327/aws.openml_s_271.1h8c.covertype.0.autogluon_hpo_auto/"
@@ -21,14 +21,16 @@
     NOTE: This code is experimental, it is recommend to not use this unless you are a developer.
     This was tested on rapids-21.06 via:
 
     conda create -n rapids-21.06 -c rapidsai -c nvidia -c conda-forge rapids=21.06 python=3.8 cudatoolkit=11.2
     conda activate rapids-21.06
     pip install --pre autogluon.tabular[all]
     """
+
     def _get_model_type(self):
         try_import_rapids_cuml()
         from cuml.neighbors import KNeighborsClassifier, KNeighborsRegressor
+
         if self.problem_type == REGRESSION:
             return KNeighborsRegressor
         else:
             return KNeighborsClassifier
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,80 @@
+import logging
+
 import numpy as np
 from pandas import DataFrame
 from scipy.stats import mode
 from sklearn.utils.extmath import weighted_mode
-from autogluon.common.utils.try_import import try_import_faiss
-
-import logging
 
+from autogluon.common.utils.try_import import try_import_faiss
 
 logger = logging.getLogger(__name__)
 
 
 # Rather than try to import non-public sklearn internals, we implement our own weighting functions here
 # These support the same operations as the sklearn functions - at least as far as possible with FAISS
 def _check_weights(weights):
     """Check to make sure weights are valid"""
-    if weights in (None, 'uniform', 'distance'):
+    if weights in (None, "uniform", "distance"):
         return weights
     elif callable(weights):
         return weights
     else:
         raise ValueError("weights not recognized: should be 'uniform', 'distance', or a callable function")
 
 
 def _get_weights(dist, weights):
     """Get the weights from an array of distances and a parameter weights"""
-    if weights in (None, 'uniform'):
+    if weights in (None, "uniform"):
         return None
-    elif weights == 'distance':
+    elif weights == "distance":
         # if user attempts to classify a point that was zero distance from one
         # or more training points, those training points are weighted as 1.0
         # and the other points as 0.0
-        with np.errstate(divide='ignore'):
-            dist = 1. / dist
+        with np.errstate(divide="ignore"):
+            dist = 1.0 / dist
         inf_mask = np.isinf(dist)
         inf_row = np.any(inf_mask, axis=1)
         dist[inf_row] = inf_mask[inf_row]
         return dist
     elif callable(weights):
         return weights(dist)
     else:
         raise ValueError("weights not recognized: should be 'uniform', 'distance', or a callable function")
 
 
 class FAISSNeighborsRegressor:
-    def __init__(self, n_neighbors=5, weights='uniform', n_jobs=-1, index_factory_string="Flat"):
+    def __init__(self, n_neighbors=5, weights="uniform", n_jobs=-1, index_factory_string="Flat"):
         """
         Creates a KNN regressor model based on FAISS. FAISS allows you to compose different
         near-neighbor search algorithms from several different preprocessing / search algorithms
-        This composition is specified by the string that is passed to the FAISS index_factory. 
-        Here are good guidelines for choosing the index string: 
+        This composition is specified by the string that is passed to the FAISS index_factory.
+        Here are good guidelines for choosing the index string:
         https://github.com/facebookresearch/faiss/wiki/Guidelines-to-choose-an-index
 
         The model itself is a clone of the sklearn one
         """
         try_import_faiss()
         import faiss
+
         self.faiss = faiss
         self.index_factory_string = index_factory_string
         self.n_neighbors = n_neighbors
         self.weights = weights
         self.n_jobs = n_jobs
         if n_jobs > 0:
             # global config, affects all faiss indexes
             faiss.omp_set_num_threads(n_jobs)
 
     def fit(self, X, y):
         if isinstance(X, DataFrame):
             X = X.to_numpy(dtype=np.float32)
         else:
             X = X.astype(np.float32)
-        if not X.flags['C_CONTIGUOUS']:
+        if not X.flags["C_CONTIGUOUS"]:
             X = np.ascontiguousarray(X)
         d = X.shape[1]
         self.index = self.faiss.index_factory(d, self.index_factory_string)
         self.y = np.array(y)
         self.index.train(X)
         self.index.add(X)
         return self
@@ -109,32 +110,34 @@
             else:
                 state[k] = self.faiss.serialize_index(self.index)
         return state
 
     def __setstate__(self, state):
         try_import_faiss()
         import faiss
+
         self.__dict__.update(state)
         self.faiss = faiss
         self.index = self.faiss.deserialize_index(self.index)
 
 
 class FAISSNeighborsClassifier:
-    def __init__(self, n_neighbors=5, weights='uniform', n_jobs=-1, index_factory_string="Flat"):
+    def __init__(self, n_neighbors=5, weights="uniform", n_jobs=-1, index_factory_string="Flat"):
         """
         Creates a KNN classifier model based on FAISS. FAISS allows you to compose different
         near-neighbor search algorithms from several different preprocessing / search algorithms
-        This composition is specified by the string that is passed to the FAISS index_factory. 
-        Here are good guidelines for choosing the index string: 
+        This composition is specified by the string that is passed to the FAISS index_factory.
+        Here are good guidelines for choosing the index string:
         https://github.com/facebookresearch/faiss/wiki/Guidelines-to-choose-an-index
 
         The model itself is a clone of the sklearn one
         """
         try_import_faiss()
         import faiss
+
         self.faiss = faiss
         self.index_factory_string = index_factory_string
         self.n_neighbors = n_neighbors
         self.weights = weights
         self.classes = []
         self.n_jobs = n_jobs
         if n_jobs > 0:
@@ -142,15 +145,15 @@
             faiss.omp_set_num_threads(n_jobs)
 
     def fit(self, X, y):
         if isinstance(X, DataFrame):
             X = X.to_numpy(dtype=np.float32)
         else:
             X = X.astype(np.float32)
-        if not X.flags['C_CONTIGUOUS']:
+        if not X.flags["C_CONTIGUOUS"]:
             X = np.ascontiguousarray(X)
         d = X.shape[1]
         self.index = self.faiss.index_factory(d, self.index_factory_string)
         self.labels = np.array(y)
         self.index.train(X)
         self.index.add(X)
         self.classes = np.unique(y)
@@ -199,10 +202,11 @@
             else:
                 state[k] = self.faiss.serialize_index(self.index)
         return state
 
     def __setstate__(self, state):
         try_import_faiss()
         import faiss
+
         self.__dict__.update(state)
         self.faiss = faiss
         self.index = self.faiss.deserialize_index(self.index)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 import copy
 import logging
 import os
 import time
 import warnings
 from operator import gt, lt
 
-from lightgbm.callback import _format_eval_result, EarlyStopException
+from lightgbm.callback import EarlyStopException, _format_eval_result
 
-from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.lite import disable_if_lite_mode
+from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.core.utils.early_stopping import SimpleES
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Add option to stop if current run's metric value is X% lower, such as min 30%, current 40% -> Stop
-def early_stopping_custom(stopping_rounds, first_metric_only=False, metrics_to_use=None, start_time=None, time_limit=None, verbose=True, max_diff=None, ignore_dart_warning=False, manual_stop_file=None, train_loss_name=None, reporter=None):
+def early_stopping_custom(
+    stopping_rounds,
+    first_metric_only=False,
+    metrics_to_use=None,
+    start_time=None,
+    time_limit=None,
+    verbose=True,
+    max_diff=None,
+    ignore_dart_warning=False,
+    manual_stop_file=None,
+    train_loss_name=None,
+    reporter=None,
+):
     """Create a callback that activates early stopping.
 
     Note
     ----
     Activates early stopping.
     The model will train until the validation score stops improving.
     Validation score needs to improve at least every ``early_stopping_rounds`` round(s)
@@ -58,46 +70,42 @@
     init_mem_avail = []
     es = []
 
     mem_status = ResourceManager.get_process()
 
     def _init(env):
         if not ignore_dart_warning:
-            enabled[0] = not any((boost_alias in env.params
-                                  and env.params[boost_alias] == 'dart') for boost_alias in ('boosting',
-                                                                                             'boosting_type',
-                                                                                             'boost'))
+            enabled[0] = not any((boost_alias in env.params and env.params[boost_alias] == "dart") for boost_alias in ("boosting", "boosting_type", "boost"))
         if not enabled[0]:
-            warnings.warn('Early stopping is not available in dart mode')
+            warnings.warn("Early stopping is not available in dart mode")
             return
         if not env.evaluation_result_list:
-            raise ValueError('For early stopping, '
-                             'at least one dataset and eval metric is required for evaluation')
+            raise ValueError("For early stopping, " "at least one dataset and eval metric is required for evaluation")
 
         if verbose:
             msg = "Training until validation scores don't improve for {} rounds."
             logger.debug(msg.format(stopping_rounds))
             if manual_stop_file:
-                logger.debug('Manually stop training by creating file at location: ', manual_stop_file)
+                logger.debug("Manually stop training by creating file at location: ", manual_stop_file)
 
         if isinstance(stopping_rounds, int):
             es_template = SimpleES(patience=stopping_rounds)
         else:
             es_template = stopping_rounds[0](**stopping_rounds[1])
 
         for eval_ret in env.evaluation_result_list:
             best_iter.append(0)
             best_score_list.append(None)
             best_trainloss.append(None)
             es.append(copy.deepcopy(es_template))
             if eval_ret[3]:
-                best_score.append(float('-inf'))
+                best_score.append(float("-inf"))
                 cmp_op.append(gt)
             else:
-                best_score.append(float('inf'))
+                best_score.append(float("inf"))
                 cmp_op.append(lt)
 
         if metrics_to_use is None:
             for i in range(len(env.evaluation_result_list)):
                 indices_to_check.append(i)
                 if first_metric_only:
                     break
@@ -123,45 +131,45 @@
         if cur_rss < init_mem_rss[0]:
             init_mem_rss[0] = cur_rss
         estimated_model_size_mb = (cur_rss - init_mem_rss[0]) >> 20
         available_mb = available >> 20
 
         model_size_memory_ratio = estimated_model_size_mb / available_mb
         if verbose or (model_size_memory_ratio > 0.25):
-            logging.debug('Available Memory: ' + str(available_mb) + ' MB')
-            logging.debug('Estimated Model Size: ' + str(estimated_model_size_mb) + ' MB')
+            logging.debug("Available Memory: " + str(available_mb) + " MB")
+            logging.debug("Estimated Model Size: " + str(estimated_model_size_mb) + " MB")
 
         early_stop = False
         if model_size_memory_ratio > 1.0:
-            logger.warning('Warning: Large GBM model size may cause OOM error if training continues')
-            logger.warning('Available Memory: ' + str(available_mb) + ' MB')
-            logger.warning('Estimated GBM model size: ' + str(estimated_model_size_mb) + ' MB')
+            logger.warning("Warning: Large GBM model size may cause OOM error if training continues")
+            logger.warning("Available Memory: " + str(available_mb) + " MB")
+            logger.warning("Estimated GBM model size: " + str(estimated_model_size_mb) + " MB")
             early_stop = True
 
         # TODO: We will want to track size of model as well, even if we early stop before OOM, we will still crash when saving if the model is large enough
         if available_mb < 512:  # Less than 500 MB
-            logger.warning('Warning: Low available memory may cause OOM error if training continues')
-            logger.warning('Available Memory: ' + str(available_mb) + ' MB')
-            logger.warning('Estimated GBM model size: ' + str(estimated_model_size_mb) + ' MB')
+            logger.warning("Warning: Low available memory may cause OOM error if training continues")
+            logger.warning("Available Memory: " + str(available_mb) + " MB")
+            logger.warning("Estimated GBM model size: " + str(estimated_model_size_mb) + " MB")
             early_stop = True
 
         if early_stop:
             logger.warning(
-                'Warning: Early stopped GBM model prior to optimal result to avoid OOM error. Please increase available memory to avoid subpar model quality.')
-            logger.log(15, 'Early stopping, best iteration is:\n[%d]\t%s' % (
-                best_iter[0] + 1, '\t'.join([_format_eval_result(x) for x in best_score_list[0]])))
+                "Warning: Early stopped GBM model prior to optimal result to avoid OOM error. Please increase available memory to avoid subpar model quality."
+            )
+            logger.log(15, "Early stopping, best iteration is:\n[%d]\t%s" % (best_iter[0] + 1, "\t".join([_format_eval_result(x) for x in best_score_list[0]])))
             raise EarlyStopException(best_iter[0], best_score_list[0])
 
     def _callback(env):
         if not cmp_op:
             _init(env)
         if not enabled[0]:
             return
         if train_loss_name is not None:
-            train_loss_evals = [eval for eval in env.evaluation_result_list if eval[0] == 'train_set' and eval[1] == train_loss_name]
+            train_loss_evals = [eval for eval in env.evaluation_result_list if eval[0] == "train_set" and eval[1] == train_loss_name]
             train_loss_val = train_loss_evals[0][2]
         else:
             train_loss_val = 0.0
         for i in indices_to_check:
             is_best_iter = False
             eval_result = env.evaluation_result_list[i]
             _, eval_metric, score, greater_is_better = eval_result
@@ -173,55 +181,68 @@
                 best_trainloss[i] = train_loss_val
             if reporter is not None:  # Report current best scores for iteration, used in HPO
                 if i == indices_to_check[0]:  # TODO: documentation needs to note that we assume 0th index is the 'official' validation performance metric.
                     if cmp_op[i] == gt:
                         validation_perf = score
                     else:
                         validation_perf = -score
-                    reporter(epoch=env.iteration + 1,
-                             validation_performance=validation_perf,
-                             train_loss=best_trainloss[i],
-                             best_iter_sofar=best_iter[i] + 1,
-                             best_valperf_sofar=best_score[i],
-                             eval_metric=eval_metric,  # eval_metric here is the stopping_metric from LGBModel
-                             greater_is_better=greater_is_better,
-                             )
+                    reporter(
+                        epoch=env.iteration + 1,
+                        validation_performance=validation_perf,
+                        train_loss=best_trainloss[i],
+                        best_iter_sofar=best_iter[i] + 1,
+                        best_valperf_sofar=best_score[i],
+                        eval_metric=eval_metric,  # eval_metric here is the stopping_metric from LGBModel
+                        greater_is_better=greater_is_better,
+                    )
             early_stop = es[i].update(cur_round=env.iteration, is_best=is_best_iter)
             if early_stop:
                 if verbose:
-                    logger.log(15, 'Early stopping, best iteration is:\n[%d]\t%s' % (
-                        best_iter[i] + 1, '\t'.join([_format_eval_result(x) for x in best_score_list[i]])))
+                    logger.log(
+                        15, "Early stopping, best iteration is:\n[%d]\t%s" % (best_iter[i] + 1, "\t".join([_format_eval_result(x) for x in best_score_list[i]]))
+                    )
                 raise EarlyStopException(best_iter[i], best_score_list[i])
             elif (max_diff is not None) and (abs(score - best_score[i]) > max_diff):
                 if verbose:
-                    logger.debug('max_diff breached!')
+                    logger.debug("max_diff breached!")
                     logger.debug(abs(score - best_score[i]))
-                    logger.log(15, 'Early stopping, best iteration is:\n[%d]\t%s' % (
-                        best_iter[i] + 1, '\t'.join([_format_eval_result(x) for x in best_score_list[i]])))
+                    logger.log(
+                        15, "Early stopping, best iteration is:\n[%d]\t%s" % (best_iter[i] + 1, "\t".join([_format_eval_result(x) for x in best_score_list[i]]))
+                    )
                 raise EarlyStopException(best_iter[i], best_score_list[i])
             if env.iteration == env.end_iteration - 1:
                 if verbose:
-                    logger.log(15, 'Did not meet early stopping criterion. Best iteration is:\n[%d]\t%s' % (
-                        best_iter[i] + 1, '\t'.join([_format_eval_result(x) for x in best_score_list[i]])))
+                    logger.log(
+                        15,
+                        "Did not meet early stopping criterion. Best iteration is:\n[%d]\t%s"
+                        % (best_iter[i] + 1, "\t".join([_format_eval_result(x) for x in best_score_list[i]])),
+                    )
                 raise EarlyStopException(best_iter[i], best_score_list[i])
             if verbose:
                 logger.debug((env.iteration - best_iter[i], eval_result))
         if manual_stop_file:
             if os.path.exists(manual_stop_file):
                 i = indices_to_check[0]
-                logger.log(20, 'Found manual stop file, early stopping. Best iteration is:\n[%d]\t%s' % (
-                    best_iter[i] + 1, '\t'.join([_format_eval_result(x) for x in best_score_list[i]])))
+                logger.log(
+                    20,
+                    "Found manual stop file, early stopping. Best iteration is:\n[%d]\t%s"
+                    % (best_iter[i] + 1, "\t".join([_format_eval_result(x) for x in best_score_list[i]])),
+                )
                 raise EarlyStopException(best_iter[i], best_score_list[i])
         if time_limit:
             time_elapsed = time.time() - start_time
             time_left = time_limit - time_elapsed
             if time_left <= 0:
                 i = indices_to_check[0]
-                logger.log(20, '\tRan out of time, early stopping on iteration ' + str(env.iteration+1) + '. Best iteration is:\n\t[%d]\t%s' % (
-                    best_iter[i] + 1, '\t'.join([_format_eval_result(x) for x in best_score_list[i]])))
+                logger.log(
+                    20,
+                    "\tRan out of time, early stopping on iteration "
+                    + str(env.iteration + 1)
+                    + ". Best iteration is:\n\t[%d]\t%s" % (best_iter[i] + 1, "\t".join([_format_eval_result(x) for x in best_score_list[i]])),
+                )
                 raise EarlyStopException(best_iter[i], best_score_list[i])
 
         # TODO: Add toggle parameter to early_stopping to disable this
         # TODO: Identify optimal threshold values for early_stopping based on lack of memory
         if env.iteration % 10 == 0:
             _mem_early_stop()
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
 DEFAULT_NUM_BOOST_ROUND = 10000  # default for single training run
 
 
 def get_lgb_objective(problem_type):
     return {
-        BINARY: 'binary',
-        MULTICLASS: 'multiclass',
-        QUANTILE: 'quantile',
-        REGRESSION: 'regression',
-        SOFTCLASS: 'multiclass',
+        BINARY: "binary",
+        MULTICLASS: "multiclass",
+        QUANTILE: "quantile",
+        REGRESSION: "regression",
+        SOFTCLASS: "multiclass",
     }[problem_type]
 
 
 def get_param_baseline_custom(problem_type):
     if problem_type == BINARY:
         return get_param_binary_baseline_custom()
     elif problem_type == MULTICLASS:
@@ -39,67 +39,67 @@
         return get_param_softclass_baseline()
     else:
         return get_param_binary_baseline()
 
 
 def get_param_multiclass_baseline_custom():
     params = {
-        'learning_rate': 0.03,
-        'num_leaves': 128,
-        'feature_fraction': 0.9,
-        'min_data_in_leaf': 3,
+        "learning_rate": 0.03,
+        "num_leaves": 128,
+        "feature_fraction": 0.9,
+        "min_data_in_leaf": 3,
         # TODO: Bin size max increase
     }
     return params
 
 
 def get_param_binary_baseline():
     params = {
-        'learning_rate': 0.05,
+        "learning_rate": 0.05,
     }
     return params
 
 
 def get_param_multiclass_baseline():
     params = {
-        'learning_rate': 0.05,
+        "learning_rate": 0.05,
     }
     return params
 
 
 def get_param_regression_baseline():
     params = {
-        'learning_rate': 0.05,
+        "learning_rate": 0.05,
     }
     return params
 
 
 def get_param_binary_baseline_custom():
     params = {
-        'learning_rate': 0.03,
-        'num_leaves': 128,
-        'feature_fraction': 0.9,
-        'min_data_in_leaf': 5,
+        "learning_rate": 0.03,
+        "num_leaves": 128,
+        "feature_fraction": 0.9,
+        "min_data_in_leaf": 5,
     }
     return params
 
 
 def get_param_regression_baseline_custom():
     params = {
-        'learning_rate': 0.03,
-        'num_leaves': 128,
-        'feature_fraction': 0.9,
-        'min_data_in_leaf': 5,
+        "learning_rate": 0.03,
+        "num_leaves": 128,
+        "feature_fraction": 0.9,
+        "min_data_in_leaf": 5,
     }
     return params
 
 
 def get_param_softclass_baseline():
     params = get_param_multiclass_baseline()
-    params.pop('metric', None)
+    params.pop("metric", None)
     return params
 
 
 def get_param_softclass_baseline_custom():
     params = get_param_multiclass_baseline_custom()
-    params.pop('metric', None)
+    params.pop("metric", None)
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Default hyperparameter search spaces used in Gradient Boosting model """
 from autogluon.common import space
-
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION
 
 
 def get_default_searchspace(problem_type):
     if problem_type == BINARY:
         return get_searchspace_binary_baseline()
     elif problem_type == MULTICLASS:
@@ -13,34 +12,36 @@
         return get_searchspace_regression_baseline()
     else:
         return get_searchspace_binary_baseline()
 
 
 def get_searchspace_multiclass_baseline():
     params = {
-        'learning_rate': space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
-        'feature_fraction': space.Real(lower=0.75, upper=1.0, default=1.0),
-        'min_data_in_leaf': space.Int(lower=2, upper=60, default=20),  # TODO: Use size of dataset to set upper, if row count is small upper should be small
-        'num_leaves': space.Int(lower=16, upper=96, default=31),  # TODO: Use row count and feature count to set this, the higher feature count the higher num_leaves upper
+        "learning_rate": space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
+        "feature_fraction": space.Real(lower=0.75, upper=1.0, default=1.0),
+        "min_data_in_leaf": space.Int(lower=2, upper=60, default=20),  # TODO: Use size of dataset to set upper, if row count is small upper should be small
+        "num_leaves": space.Int(
+            lower=16, upper=96, default=31
+        ),  # TODO: Use row count and feature count to set this, the higher feature count the higher num_leaves upper
         # TODO: Bin size max increase
     }
     return params
 
 
 def get_searchspace_binary_baseline():
     params = {
-        'learning_rate': space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
-        'feature_fraction': space.Real(lower=0.75, upper=1.0, default=1.0),
-        'min_data_in_leaf': space.Int(lower=2, upper=60, default=20),
-        'num_leaves': space.Int(lower=16, upper=96, default=31),
+        "learning_rate": space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
+        "feature_fraction": space.Real(lower=0.75, upper=1.0, default=1.0),
+        "min_data_in_leaf": space.Int(lower=2, upper=60, default=20),
+        "num_leaves": space.Int(lower=16, upper=96, default=31),
     }
     return params
 
 
 def get_searchspace_regression_baseline():
     params = {
-        'learning_rate': space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
-        'feature_fraction': space.Real(lower=0.75, upper=1.0, default=1.0),
-        'min_data_in_leaf': space.Int(lower=2, upper=60, default=20),
-        'num_leaves': space.Int(lower=16, upper=96, default=31),
+        "learning_rate": space.Real(lower=5e-3, upper=0.2, default=0.05, log=True),
+        "feature_fraction": space.Real(lower=0.75, upper=1.0, default=1.0),
+        "min_data_in_leaf": space.Int(lower=2, upper=60, default=20),
+        "num_leaves": space.Int(lower=16, upper=96, default=31),
     }
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import re
 import time
 import warnings
 
 import numpy as np
 from pandas import DataFrame, Series
 
-from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY
+from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
+from autogluon.common.utils.try_import import try_import_lightgbm
 from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 from autogluon.core.models import AbstractModel
 from autogluon.core.models._utils import get_early_stopping_rounds
-from autogluon.common.utils.try_import import try_import_lightgbm
 
 from . import lgb_utils
-from .hyperparameters.parameters import get_param_baseline, get_lgb_objective, DEFAULT_NUM_BOOST_ROUND
+from .hyperparameters.parameters import DEFAULT_NUM_BOOST_ROUND, get_lgb_objective, get_param_baseline
 from .hyperparameters.searchspaces import get_default_searchspace
 from .lgb_utils import construct_dataset, train_lgb_model
 
 warnings.filterwarnings("ignore", category=UserWarning, message="Starting from version")  # lightGBM brew libomp warning
 logger = logging.getLogger(__name__)
 
 
@@ -32,14 +32,15 @@
     LightGBM model: https://lightgbm.readthedocs.io/en/latest/
 
     Hyperparameter options: https://lightgbm.readthedocs.io/en/latest/Parameters.html
 
     Extra hyperparameter options:
         ag.early_stop : int, specifies the early stopping rounds. Defaults to an adaptive strategy. Recommended to keep default.
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self._features_internal_map = None
         self._features_internal_list = None
         self._requires_remap = None
 
@@ -51,38 +52,29 @@
     def _get_default_searchspace(self):
         return get_default_searchspace(problem_type=self.problem_type)
 
     # Use specialized LightGBM metric if available (fast), otherwise use custom func generator
     def _get_stopping_metric_internal(self):
         stopping_metric = lgb_utils.convert_ag_metric_to_lgbm(ag_metric_name=self.stopping_metric.name, problem_type=self.problem_type)
         if stopping_metric is None:
-            stopping_metric = lgb_utils.func_generator(metric=self.stopping_metric, is_higher_better=True, needs_pred_proba=not self.stopping_metric.needs_pred, problem_type=self.problem_type)
+            stopping_metric = lgb_utils.func_generator(
+                metric=self.stopping_metric, is_higher_better=True, needs_pred_proba=not self.stopping_metric.needs_pred, problem_type=self.problem_type
+            )
             stopping_metric_name = self.stopping_metric.name
         else:
             stopping_metric_name = stopping_metric
         return stopping_metric, stopping_metric_name
 
     def _estimate_memory_usage(self, X, **kwargs):
         num_classes = self.num_classes if self.num_classes else 1  # self.num_classes could be None after initialization if it's a regression problem
         data_mem_usage = get_approximate_df_mem_usage(X).sum()
         approx_mem_size_req = data_mem_usage * 7 + data_mem_usage / 4 * num_classes  # TODO: Extremely crude approximation, can be vastly improved
         return approx_mem_size_req
 
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             time_limit=None,
-             num_gpus=0,
-             num_cpus=0,
-             sample_weight=None,
-             sample_weight_val=None,
-             verbosity=2,
-             **kwargs):
+    def _fit(self, X, y, X_val=None, y_val=None, time_limit=None, num_gpus=0, num_cpus=0, sample_weight=None, sample_weight_val=None, verbosity=2, **kwargs):
         try_import_lightgbm()  # raise helpful error message if LightGBM isn't installed
         start_time = time.time()
         ag_params = self._get_ag_params()
         params = self._get_model_params()
 
         if verbosity <= 1:
             log_period = False
@@ -91,151 +83,154 @@
         elif verbosity == 3:
             log_period = 50
         else:
             log_period = 1
 
         stopping_metric, stopping_metric_name = self._get_stopping_metric_internal()
 
-        num_boost_round = params.pop('num_boost_round', DEFAULT_NUM_BOOST_ROUND)
-        dart_retrain = params.pop('dart_retrain', False)  # Whether to retrain the model to get optimal iteration if model is trained in 'dart' mode.
+        num_boost_round = params.pop("num_boost_round", DEFAULT_NUM_BOOST_ROUND)
+        dart_retrain = params.pop("dart_retrain", False)  # Whether to retrain the model to get optimal iteration if model is trained in 'dart' mode.
         if num_gpus != 0:
-            if 'device' not in params:
+            if "device" not in params:
                 # TODO: lightgbm must have a special install to support GPU: https://github.com/Microsoft/LightGBM/tree/master/python-package#build-gpu-version
                 #  Before enabling GPU, we should add code to detect that GPU-enabled version is installed and that a valid GPU exists.
                 #  GPU training heavily alters accuracy, often in a negative manner. We will have to be careful about when to use GPU.
-                params['device'] = 'gpu'
-                logger.log(20, f'\tTraining {self.name} with GPU, note that this may negatively impact model quality compared to CPU training.')
+                params["device"] = "gpu"
+                logger.log(20, f"\tTraining {self.name} with GPU, note that this may negatively impact model quality compared to CPU training.")
         logger.log(15, f"\tFitting {num_boost_round} rounds... Hyperparameters: {params}")
 
-        if 'num_threads' not in params:
-            params['num_threads'] = num_cpus
-        if 'objective' not in params:
-            params['objective'] = get_lgb_objective(problem_type=self.problem_type)
-        if self.problem_type in [MULTICLASS, SOFTCLASS] and 'num_classes' not in params:
-            params['num_classes'] = self.num_classes
-        if 'verbose' not in params:
-            params['verbose'] = -1
+        if "num_threads" not in params:
+            params["num_threads"] = num_cpus
+        if "objective" not in params:
+            params["objective"] = get_lgb_objective(problem_type=self.problem_type)
+        if self.problem_type in [MULTICLASS, SOFTCLASS] and "num_classes" not in params:
+            params["num_classes"] = self.num_classes
+        if "verbose" not in params:
+            params["verbose"] = -1
 
         num_rows_train = len(X)
         dataset_train, dataset_val = self.generate_datasets(
-            X=X, y=y, params=params, X_val=X_val, y_val=y_val,
-            sample_weight=sample_weight, sample_weight_val=sample_weight_val
+            X=X, y=y, params=params, X_val=X_val, y_val=y_val, sample_weight=sample_weight, sample_weight_val=sample_weight_val
         )
         gc.collect()
 
         callbacks = []
         valid_names = []
         valid_sets = []
         if dataset_val is not None:
             from .callbacks import early_stopping_custom
+
             # TODO: Better solution: Track trend to early stop when score is far worse than best score, or score is trending worse over time
-            early_stopping_rounds = ag_params.get('early_stop', 'adaptive')
+            early_stopping_rounds = ag_params.get("early_stop", "adaptive")
             if isinstance(early_stopping_rounds, (str, tuple, list)):
                 early_stopping_rounds = self._get_early_stopping_rounds(num_rows_train=num_rows_train, strategy=early_stopping_rounds)
             if early_stopping_rounds is None:
                 early_stopping_rounds = 999999
-            reporter = kwargs.get('reporter', None)
+            reporter = kwargs.get("reporter", None)
             train_loss_name = self._get_train_loss_name() if reporter is not None else None
             if train_loss_name is not None:
-                if 'metric' not in params or params['metric'] == '':
-                    params['metric'] = train_loss_name
-                elif train_loss_name not in params['metric']:
-                    params['metric'] = f'{params["metric"]},{train_loss_name}'
+                if "metric" not in params or params["metric"] == "":
+                    params["metric"] = train_loss_name
+                elif train_loss_name not in params["metric"]:
+                    params["metric"] = f'{params["metric"]},{train_loss_name}'
             # early stopping callback will be added later by QuantileBooster if problem_type==QUANTILE
             early_stopping_callback_kwargs = dict(
                 stopping_rounds=early_stopping_rounds,
-                metrics_to_use=[('valid_set', stopping_metric_name)],
+                metrics_to_use=[("valid_set", stopping_metric_name)],
                 max_diff=None,
                 start_time=start_time,
                 time_limit=time_limit,
                 ignore_dart_warning=True,
                 verbose=False,
                 manual_stop_file=False,
                 reporter=reporter,
                 train_loss_name=train_loss_name,
             )
             callbacks += [
                 # Note: Don't use self.params_aux['max_memory_usage_ratio'] here as LightGBM handles memory per iteration optimally.  # TODO: Consider using when ratio < 1.
                 early_stopping_custom(**early_stopping_callback_kwargs)
             ]
-            valid_names = ['valid_set'] + valid_names
+            valid_names = ["valid_set"] + valid_names
             valid_sets = [dataset_val] + valid_sets
         else:
             early_stopping_callback_kwargs = None
         from lightgbm.callback import log_evaluation
+
         if log_period is not None:
             callbacks.append(log_evaluation(period=log_period))
 
-        seed_val = params.pop('seed_value', 0)
+        seed_val = params.pop("seed_value", 0)
         train_params = {
-            'params': params,
-            'train_set': dataset_train,
-            'num_boost_round': num_boost_round,
-            'valid_sets': valid_sets,
-            'valid_names': valid_names,
-            'callbacks': callbacks,
+            "params": params,
+            "train_set": dataset_train,
+            "num_boost_round": num_boost_round,
+            "valid_sets": valid_sets,
+            "valid_names": valid_names,
+            "callbacks": callbacks,
         }
         if not isinstance(stopping_metric, str):
-            train_params['feval'] = stopping_metric
+            train_params["feval"] = stopping_metric
         else:
-            if 'metric' not in train_params['params'] or train_params['params']['metric'] == '':
-                train_params['params']['metric'] = stopping_metric
-            elif stopping_metric not in train_params['params']['metric']:
-                train_params['params']['metric'] = f'{train_params["params"]["metric"]},{stopping_metric}'
+            if "metric" not in train_params["params"] or train_params["params"]["metric"] == "":
+                train_params["params"]["metric"] = stopping_metric
+            elif stopping_metric not in train_params["params"]["metric"]:
+                train_params["params"]["metric"] = f'{train_params["params"]["metric"]},{stopping_metric}'
         if self.problem_type == SOFTCLASS:
-            train_params['fobj'] = lgb_utils.softclass_lgbobj
+            train_params["fobj"] = lgb_utils.softclass_lgbobj
         elif self.problem_type == QUANTILE:
-            train_params['params']['quantile_levels'] = self.quantile_levels
+            train_params["params"]["quantile_levels"] = self.quantile_levels
         if seed_val is not None:
-            train_params['params']['seed'] = seed_val
+            train_params["params"]["seed"] = seed_val
             random.seed(seed_val)
             np.random.seed(seed_val)
 
         # Train LightGBM model:
         from lightgbm.basic import LightGBMError
+
         with warnings.catch_warnings():
             # Filter harmless warnings introduced in lightgbm 3.0, future versions plan to remove: https://github.com/microsoft/LightGBM/issues/3379
-            warnings.filterwarnings('ignore', message='Overriding the parameters from Reference Dataset.')
-            warnings.filterwarnings('ignore', message='categorical_column in param dict is overridden.')
+            warnings.filterwarnings("ignore", message="Overriding the parameters from Reference Dataset.")
+            warnings.filterwarnings("ignore", message="categorical_column in param dict is overridden.")
             try:
                 self.model = train_lgb_model(early_stopping_callback_kwargs=early_stopping_callback_kwargs, **train_params)
             except LightGBMError:
-                if train_params['params'].get('device', 'cpu') != 'gpu':
+                if train_params["params"].get("device", "cpu") != "gpu":
                     raise
                 else:
-                    logger.warning('Warning: GPU mode might not be installed for LightGBM, GPU training raised an exception. Falling back to CPU training...'
-                                   'Refer to LightGBM GPU documentation: https://github.com/Microsoft/LightGBM/tree/master/python-package#build-gpu-version'
-                                   'One possible method is:'
-                                   '\tpip uninstall lightgbm -y'
-                                   '\tpip install lightgbm --install-option=--gpu'
-                                   )
-                    train_params['params']['device'] = 'cpu'
+                    logger.warning(
+                        "Warning: GPU mode might not be installed for LightGBM, GPU training raised an exception. Falling back to CPU training..."
+                        "Refer to LightGBM GPU documentation: https://github.com/Microsoft/LightGBM/tree/master/python-package#build-gpu-version"
+                        "One possible method is:"
+                        "\tpip uninstall lightgbm -y"
+                        "\tpip install lightgbm --install-option=--gpu"
+                    )
+                    train_params["params"]["device"] = "cpu"
                     self.model = train_lgb_model(early_stopping_callback_kwargs=early_stopping_callback_kwargs, **train_params)
             retrain = False
-            if train_params['params'].get('boosting_type', '') == 'dart':
+            if train_params["params"].get("boosting_type", "") == "dart":
                 if dataset_val is not None and dart_retrain and (self.model.best_iteration != num_boost_round):
                     retrain = True
                     if time_limit is not None:
                         time_left = time_limit + start_time - time.time()
                         if time_left < 0.5 * time_limit:
                             retrain = False
                     if retrain:
                         logger.log(15, f"Retraining LGB model to optimal iterations ('dart' mode).")
-                        train_params.pop('callbacks', None)
-                        train_params.pop('valid_sets', None)
-                        train_params.pop('valid_names', None)
-                        train_params['num_boost_round'] = self.model.best_iteration
+                        train_params.pop("callbacks", None)
+                        train_params.pop("valid_sets", None)
+                        train_params.pop("valid_names", None)
+                        train_params["num_boost_round"] = self.model.best_iteration
                         self.model = train_lgb_model(**train_params)
                     else:
                         logger.log(15, f"Not enough time to retrain LGB model ('dart' mode)...")
 
         if dataset_val is not None and not retrain:
-            self.params_trained['num_boost_round'] = self.model.best_iteration
+            self.params_trained["num_boost_round"] = self.model.best_iteration
         else:
-            self.params_trained['num_boost_round'] = self.model.current_iteration()
+            self.params_trained["num_boost_round"] = self.model.current_iteration()
 
     def _predict_proba(self, X, num_cpus=0, **kwargs):
         X = self.preprocess(X, **kwargs)
 
         y_pred_proba = self.model.predict(X, num_threads=num_cpus)
         if self.problem_type == REGRESSION:
             return y_pred_proba
@@ -246,15 +241,15 @@
                 return y_pred_proba[:, 1]
             else:
                 return y_pred_proba
         elif self.problem_type == MULTICLASS:
             return y_pred_proba
         elif self.problem_type == SOFTCLASS:  # apply softmax
             y_pred_proba = np.exp(y_pred_proba)
-            y_pred_proba = np.multiply(y_pred_proba, 1/np.sum(y_pred_proba, axis=1)[:, np.newaxis])
+            y_pred_proba = np.multiply(y_pred_proba, 1 / np.sum(y_pred_proba, axis=1)[:, np.newaxis])
             return y_pred_proba
         else:
             if len(y_pred_proba.shape) == 1:
                 return y_pred_proba
             elif y_pred_proba.shape[1] > 2:  # Should this ever happen?
                 return y_pred_proba
             else:  # Should this ever happen?
@@ -263,15 +258,15 @@
     def _preprocess_nonadaptive(self, X, is_train=False, **kwargs):
         X = super()._preprocess_nonadaptive(X=X, **kwargs)
 
         if is_train:
             self._requires_remap = False
             for column in X.columns:
                 if isinstance(column, str):
-                    new_column = re.sub(r'[",:{}[\]]', '', column)
+                    new_column = re.sub(r'[",:{}[\]]', "", column)
                     if new_column != column:
                         self._features_internal_map = {feature: i for i, feature in enumerate(list(X.columns))}
                         self._requires_remap = True
                         break
             if self._requires_remap:
                 self._features_internal_list = np.array([self._features_internal_map[feature] for feature in list(X.columns)])
             else:
@@ -281,15 +276,15 @@
             X_new = X.copy(deep=False)
             X_new.columns = self._features_internal_list
             return X_new
         else:
             return X
 
     def generate_datasets(self, X: DataFrame, y: Series, params, X_val=None, y_val=None, sample_weight=None, sample_weight_val=None, save=False):
-        lgb_dataset_params_keys = ['two_round']  # Keys that are specific to lightGBM Dataset object construction.
+        lgb_dataset_params_keys = ["two_round"]  # Keys that are specific to lightGBM Dataset object construction.
         data_params = {key: params[key] for key in lgb_dataset_params_keys if key in params}.copy()
 
         X = self.preprocess(X, is_train=True)
         if X_val is not None:
             X_val = self.preprocess(X_val)
         # TODO: Try creating multiple Datasets for subsets of features, then combining with Dataset.add_features_from(), this might avoid memory spike
 
@@ -299,82 +294,91 @@
             y_og = np.array(y)
             y = None
             if X_val is not None:
                 y_val_og = np.array(y_val)
                 y_val = None
 
         # X, W_train = self.convert_to_weight(X=X)
-        dataset_train = construct_dataset(x=X, y=y, location=f'{self.path}datasets{os.path.sep}train', params=data_params, save=save, weight=sample_weight)
+        dataset_train = construct_dataset(x=X, y=y, location=f"{self.path}datasets{os.path.sep}train", params=data_params, save=save, weight=sample_weight)
         # dataset_train = construct_dataset_lowest_memory(X=X, y=y, location=self.path + 'datasets/train', params=data_params)
         if X_val is not None:
             # X_val, W_val = self.convert_to_weight(X=X_val)
-            dataset_val = construct_dataset(x=X_val, y=y_val, location=f'{self.path}datasets{os.path.sep}val', reference=dataset_train, params=data_params, save=save, weight=sample_weight_val)
+            dataset_val = construct_dataset(
+                x=X_val,
+                y=y_val,
+                location=f"{self.path}datasets{os.path.sep}val",
+                reference=dataset_train,
+                params=data_params,
+                save=save,
+                weight=sample_weight_val,
+            )
             # dataset_val = construct_dataset_lowest_memory(X=X_val, y=y_val, location=self.path + 'datasets/val', reference=dataset_train, params=data_params)
         else:
             dataset_val = None
         if self.problem_type == SOFTCLASS:
             if y_og is not None:
                 dataset_train.softlabels = y_og
             if y_val_og is not None:
                 dataset_val.softlabels = y_val_og
         return dataset_train, dataset_val
 
     def _get_train_loss_name(self):
         if self.problem_type == BINARY:
-            train_loss_name = 'binary_logloss'
+            train_loss_name = "binary_logloss"
         elif self.problem_type == MULTICLASS:
-            train_loss_name = 'multi_logloss'
+            train_loss_name = "multi_logloss"
         elif self.problem_type == REGRESSION:
-            train_loss_name = 'l2'
+            train_loss_name = "l2"
         else:
             raise ValueError(f"unknown problem_type for LGBModel: {self.problem_type}")
         return train_loss_name
 
-    def _get_early_stopping_rounds(self, num_rows_train, strategy='auto'):
+    def _get_early_stopping_rounds(self, num_rows_train, strategy="auto"):
         return get_early_stopping_rounds(num_rows_train=num_rows_train, strategy=strategy)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             valid_raw_types=[R_BOOL, R_INT, R_FLOAT, R_CATEGORY],
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     def _is_gpu_lgbm_installed(self):
         # Taken from https://github.com/microsoft/LightGBM/issues/3939
         try_import_lightgbm()
         import lightgbm
+
         try:
             data = np.random.rand(50, 2)
             label = np.random.randint(2, size=50)
             train_data = lightgbm.Dataset(data, label=label)
-            params = {'device': 'gpu'}
+            params = {"device": "gpu"}
             gbm = lightgbm.train(params, train_set=train_data, verbose=-1)
             return True
         except Exception as e:
             return False
 
     def get_minimum_resources(self, is_gpu_available=False):
         minimum_resources = {
-            'num_cpus': 1,
+            "num_cpus": 1,
         }
         if is_gpu_available and self._is_gpu_lgbm_installed():
-            minimum_resources['num_gpus'] = 0.5
+            minimum_resources["num_gpus"] = 0.5
         return minimum_resources
 
     def _get_default_resources(self):
         # logical=False is faster in training
         num_cpus = ResourceManager.get_cpu_count_psutil(logical=False)
         num_gpus = 0
         return num_cpus, num_gpus
 
     @property
     def _features(self):
         return self._features_internal_list
 
     def _ag_params(self) -> set:
-        return {'early_stop'}
+        return {"early_stop"}
 
     def _more_tags(self):
         # `can_refit_full=True` because num_boost_round is communicated at end of `_fit`
-        return {'can_refit_full': True}
+        return {"can_refit_full": True}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,154 +3,165 @@
 import time
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 
+from autogluon.common.utils.try_import import try_import_lightgbm
 from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 from autogluon.core.utils.exceptions import TimeLimitExceeded
-from autogluon.common.utils.try_import import try_import_lightgbm
-
 
 # Mapping to specialized LightGBM metrics that are much faster than the standard metric computation
 _ag_to_lgbm_metric_dict = {
     BINARY: dict(
-        accuracy='binary_error',
-        log_loss='binary_logloss',
-        roc_auc='auc',
+        accuracy="binary_error",
+        log_loss="binary_logloss",
+        roc_auc="auc",
     ),
     MULTICLASS: dict(
-        accuracy='multi_error',
-        log_loss='multi_logloss',
+        accuracy="multi_error",
+        log_loss="multi_logloss",
     ),
     QUANTILE: dict(
-        pinball_loss='quantile',
+        pinball_loss="quantile",
     ),
     REGRESSION: dict(
-        mean_absolute_error='l1',
-        mean_squared_error='l2',
-        root_mean_squared_error='rmse',
+        mean_absolute_error="l1",
+        mean_squared_error="l2",
+        root_mean_squared_error="rmse",
     ),
 }
 
 
 def convert_ag_metric_to_lgbm(ag_metric_name, problem_type):
     return _ag_to_lgbm_metric_dict.get(problem_type, dict()).get(ag_metric_name, None)
 
 
 def func_generator(metric, is_higher_better, needs_pred_proba, problem_type):
     if needs_pred_proba:
         if problem_type == MULTICLASS:
+
             def function_template(y_hat, data):
                 y_true = data.get_label()
                 y_hat = y_hat.reshape(len(np.unique(y_true)), -1).T
                 return metric.name, metric(y_true, y_hat), is_higher_better
+
         elif problem_type == SOFTCLASS:  # metric must take in soft labels array, like soft_log_loss
+
             def function_template(y_hat, data):
                 y_true = data.softlabels
                 y_hat = y_hat.reshape(y_true.shape[1], -1).T
                 y_hat = np.exp(y_hat)
-                y_hat = np.multiply(y_hat, 1/np.sum(y_hat, axis=1)[:, np.newaxis])
+                y_hat = np.multiply(y_hat, 1 / np.sum(y_hat, axis=1)[:, np.newaxis])
                 return metric.name, metric(y_true, y_hat), is_higher_better
+
         else:
+
             def function_template(y_hat, data):
                 y_true = data.get_label()
                 return metric.name, metric(y_true, y_hat), is_higher_better
+
     else:
         if problem_type == MULTICLASS:
+
             def function_template(y_hat, data):
                 y_true = data.get_label()
                 y_hat = y_hat.reshape(len(np.unique(y_true)), -1)
                 y_hat = y_hat.argmax(axis=0)
                 return metric.name, metric(y_true, y_hat), is_higher_better
+
         else:
+
             def function_template(y_hat, data):
                 y_true = data.get_label()
                 y_hat = np.round(y_hat)
                 return metric.name, metric(y_true, y_hat), is_higher_better
+
     return function_template
 
 
 def softclass_lgbobj(preds, train_data):
-    """ Custom LightGBM loss function for soft (probabilistic, vector-valued) class-labels only,
-        which have been appended to lgb.Dataset (train_data) as additional ".softlabels" attribute (2D numpy array).
+    """Custom LightGBM loss function for soft (probabilistic, vector-valued) class-labels only,
+    which have been appended to lgb.Dataset (train_data) as additional ".softlabels" attribute (2D numpy array).
     """
     softlabels = train_data.softlabels
     num_classes = softlabels.shape[1]
-    preds=np.reshape(preds, (len(softlabels), num_classes), order='F')
+    preds = np.reshape(preds, (len(softlabels), num_classes), order="F")
     preds = np.exp(preds)
-    preds = np.multiply(preds, 1/np.sum(preds, axis=1)[:, np.newaxis])
-    grad = (preds - softlabels)
-    hess = 2.0 * preds * (1.0-preds)
-    return grad.flatten('F'), hess.flatten('F')
+    preds = np.multiply(preds, 1 / np.sum(preds, axis=1)[:, np.newaxis])
+    grad = preds - softlabels
+    hess = 2.0 * preds * (1.0 - preds)
+    return grad.flatten("F"), hess.flatten("F")
 
 
 def construct_dataset(x: DataFrame, y: Series, location=None, reference=None, params=None, save=False, weight=None):
     try_import_lightgbm()
     import lightgbm as lgb
 
     dataset = lgb.Dataset(data=x, label=y, reference=reference, free_raw_data=True, params=params, weight=weight)
 
     if save:
         assert location is not None
-        saving_path = f'{location}.bin'
+        saving_path = f"{location}.bin"
         if os.path.exists(saving_path):
             os.remove(saving_path)
 
         os.makedirs(os.path.dirname(saving_path), exist_ok=True)
         dataset.save_binary(saving_path)
         # dataset_binary = lgb.Dataset(location + '.bin', reference=reference, free_raw_data=False)# .construct()
 
     return dataset
 
 
 def train_lgb_model(early_stopping_callback_kwargs=None, **train_params):
     import lightgbm as lgb
 
-    if train_params['params']['objective'] == 'quantile':
-        quantile_levels = train_params['params'].pop('quantile_levels')
+    if train_params["params"]["objective"] == "quantile":
+        quantile_levels = train_params["params"].pop("quantile_levels")
         booster = QuantileBooster(quantile_levels=quantile_levels, early_stopping_callback_kwargs=early_stopping_callback_kwargs)
         return booster.fit(**train_params)
     else:
         return lgb.train(**train_params)
 
 
 class QuantileBooster:
     """Wrapper that trains a separate LGBM Booster for each quantile level."""
+
     def __init__(self, quantile_levels: List[float], early_stopping_callback_kwargs: Optional[dict] = None):
         if quantile_levels is None:
             raise AssertionError
         if not all(0 < q < 1 for q in quantile_levels):
-            raise AssertionError(f'quantile_levels must fulfill 0 < q < 1, provided quantile_levels: {quantile_levels}')
+            raise AssertionError(f"quantile_levels must fulfill 0 < q < 1, provided quantile_levels: {quantile_levels}")
 
         self.quantile_levels = quantile_levels
 
         self.early_stopping_callback_kwargs = None
         self.time_limit_global = None
 
         if early_stopping_callback_kwargs is not None:
             self.early_stopping_callback_kwargs = early_stopping_callback_kwargs
-            self.time_limit_global = early_stopping_callback_kwargs.pop('time_limit')
+            self.time_limit_global = early_stopping_callback_kwargs.pop("time_limit")
         self.model_dict = {}
 
     def fit(self, **train_params_base):
         import lightgbm as lgb
+
         from .callbacks import early_stopping_custom
 
         start_time_global = time.time()
 
         for q in self.quantile_levels:
             train_params = copy.deepcopy(train_params_base)
-            train_params['params']['alpha'] = q
+            train_params["params"]["alpha"] = q
             if self.early_stopping_callback_kwargs is not None:
                 es_kwargs = copy.deepcopy(self.early_stopping_callback_kwargs)
                 if self.time_limit_global is not None:
-                    es_kwargs['start_time'] = time.time()
-                    es_kwargs['time_limit'] = self.time_limit_global / len(self.quantile_levels)
+                    es_kwargs["start_time"] = time.time()
+                    es_kwargs["time_limit"] = self.time_limit_global / len(self.quantile_levels)
                 # Don't add a logging callback to avoid printing logs for each base booster
                 train_params["callbacks"] = [early_stopping_custom(**es_kwargs)]
             else:
                 train_params["callbacks"] = []
 
             self.model_dict[q] = lgb.train(**train_params)
             if self.time_limit_global is not None:
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import logging
 
 from autogluon.core.constants import BINARY
 
-IGNORE = 'ignore'
-ONLY = 'only'
-INCLUDE = 'include'
+IGNORE = "ignore"
+ONLY = "only"
+INCLUDE = "include"
 
 logger = logging.getLogger(__name__)
 
 preprocess_params_set = {
-    'vectorizer_dict_size',
-    'proc.ngram_range',
-    'proc.skew_threshold',
-    'proc.impute_strategy',
-    'penalty',
-    'handle_text',
+    "vectorizer_dict_size",
+    "proc.ngram_range",
+    "proc.skew_threshold",
+    "proc.impute_strategy",
+    "penalty",
+    "handle_text",
 }
 
 
 def get_param_baseline():
     default_params = {
-        'C': 1,
-        'vectorizer_dict_size': 75000,  # size of TFIDF vectorizer dictionary; used only in text model
-        'proc.ngram_range': (1, 5),  # range of n-grams for TFIDF vectorizer dictionary; used only in text model
-        'proc.skew_threshold': 0.99,  # numerical features whose absolute skewness is greater than this receive special power-transform preprocessing. Choose big value to avoid using power-transforms
-        'proc.impute_strategy': 'median',  # strategy argument of sklearn.SimpleImputer() used to impute missing numeric values
-        'penalty': 'L2',  # regularization to use with regression models
-        'handle_text': IGNORE, # how text should be handled: `ignore` - don't use NLP features; `only` - only use NLP features; `include` - use both regular and NLP features
+        "C": 1,
+        "vectorizer_dict_size": 75000,  # size of TFIDF vectorizer dictionary; used only in text model
+        "proc.ngram_range": (1, 5),  # range of n-grams for TFIDF vectorizer dictionary; used only in text model
+        "proc.skew_threshold": 0.99,  # numerical features whose absolute skewness is greater than this receive special power-transform preprocessing. Choose big value to avoid using power-transforms
+        "proc.impute_strategy": "median",  # strategy argument of sklearn.SimpleImputer() used to impute missing numeric values
+        "penalty": "L2",  # regularization to use with regression models
+        "handle_text": IGNORE,  # how text should be handled: `ignore` - don't use NLP features; `only` - only use NLP features; `include` - use both regular and NLP features
     }
     return default_params
 
 
 def _get_solver(problem_type):
     if problem_type == BINARY:
         # TODO explore using liblinear for smaller datasets
-        solver = 'lbfgs'
+        solver = "lbfgs"
     else:
-        solver = 'lbfgs'
+        solver = "lbfgs"
     return solver
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 import re
 import time
 import warnings
 from collections import defaultdict
 
 import numpy as np
+from sklearn.compose import ColumnTransformer
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
-from sklearn.compose import ColumnTransformer
-from sklearn.preprocessing import StandardScaler, QuantileTransformer
+from sklearn.preprocessing import QuantileTransformer, StandardScaler
 
-from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY, R_OBJECT, S_TEXT_AS_CATEGORY, S_BOOL
+from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT, R_OBJECT, S_BOOL, S_TEXT_AS_CATEGORY
 from autogluon.core.constants import BINARY, REGRESSION
+from autogluon.core.models import AbstractModel
+from autogluon.core.utils.exceptions import TimeLimitExceeded
 
-from .hyperparameters.parameters import get_param_baseline, INCLUDE, IGNORE, ONLY, _get_solver, preprocess_params_set
+from .hyperparameters.parameters import IGNORE, INCLUDE, ONLY, _get_solver, get_param_baseline, preprocess_params_set
 from .hyperparameters.searchspaces import get_default_searchspace
 from .lr_preprocessing_utils import NlpDataPreprocessor, OheFeaturesGenerator
-from autogluon.core.models import AbstractModel
-from autogluon.core.utils.exceptions import TimeLimitExceeded
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Can Bagged LinearModels be combined during inference to 1 model by averaging their weights?
 #  What about just always using refit_full model? Should we even bag at all? Do we care that its slightly overfit?
 class LinearModel(AbstractModel):
@@ -31,171 +31,175 @@
 
     Model backend differs depending on problem_type:
 
         'binary' & 'multiclass': https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
 
         'regression': https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html#sklearn.linear_model.Ridge
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._pipeline = None
 
     def _get_model_type(self):
-        penalty = self.params.get('penalty', 'L2')
-        if self.params_aux.get('use_daal', True):
+        penalty = self.params.get("penalty", "L2")
+        if self.params_aux.get("use_daal", True):
             # Appears to give 20x training speedup when enabled
             try:
                 # TODO: Add more granular switch, currently this affects all future LR models even if they had `use_daal=False`
-                from sklearnex.linear_model import LogisticRegression, Ridge, Lasso
-                logger.log(15, '\tUsing sklearnex LR backend...')
+                from sklearnex.linear_model import Lasso, LogisticRegression, Ridge
+
+                logger.log(15, "\tUsing sklearnex LR backend...")
             except:
-                from sklearn.linear_model import LogisticRegression, Ridge, Lasso
+                from sklearn.linear_model import Lasso, LogisticRegression, Ridge
         else:
-            from sklearn.linear_model import LogisticRegression, Ridge, Lasso
+            from sklearn.linear_model import Lasso, LogisticRegression, Ridge
         if self.problem_type == REGRESSION:
-            if penalty == 'L2':
+            if penalty == "L2":
                 model_type = Ridge
-            elif penalty == 'L1':
+            elif penalty == "L1":
                 model_type = Lasso
             else:
                 raise AssertionError(f'Unknown value for penalty "{penalty}" - supported types are ["L1", "L2"]')
         else:
             model_type = LogisticRegression
         return model_type
 
     def _tokenize(self, s):
-        return re.split('[ ]+', s)
+        return re.split("[ ]+", s)
 
     def _get_types_of_features(self, df):
-        """ Returns dict with keys: : 'continuous', 'skewed', 'onehot', 'embed', 'language', values = ordered list of feature-names falling into each category.
-            Each value is a list of feature-names corresponding to columns in original dataframe.
+        """Returns dict with keys: : 'continuous', 'skewed', 'onehot', 'embed', 'language', values = ordered list of feature-names falling into each category.
+        Each value is a list of feature-names corresponding to columns in original dataframe.
         """
         continuous_featnames = self._feature_metadata.get_features(valid_raw_types=[R_INT, R_FLOAT], invalid_special_types=[S_BOOL])
         categorical_featnames = self._feature_metadata.get_features(valid_raw_types=[R_CATEGORY, R_OBJECT])
         bool_featnames = self._feature_metadata.get_features(required_special_types=[S_BOOL])
         language_featnames = []  # TODO: Disabled currently, have to pass raw text data features here to function properly
-        return self._select_features(df=df,
-                                     categorical_featnames=categorical_featnames,
-                                     language_featnames=language_featnames,
-                                     continuous_featnames=continuous_featnames,
-                                     bool_featnames=bool_featnames)
+        return self._select_features(
+            df=df,
+            categorical_featnames=categorical_featnames,
+            language_featnames=language_featnames,
+            continuous_featnames=continuous_featnames,
+            bool_featnames=bool_featnames,
+        )
 
     def _select_features(self, df, **kwargs):
         features_selector = {
             INCLUDE: self._select_features_handle_text_include,
             ONLY: self._select_features_handle_text_only,
             IGNORE: self._select_features_handle_text_ignore,
-        }.get(self.params.get('handle_text', IGNORE), self._select_features_handle_text_ignore)
+        }.get(self.params.get("handle_text", IGNORE), self._select_features_handle_text_ignore)
         return features_selector(df=df, **kwargs)
 
     # TODO: handle collinear features - they will impact results quality
     def _preprocess(self, X, is_train=False, **kwargs):
         if is_train:
             feature_types = self._get_types_of_features(X)
-            X = self._preprocess_train(X, feature_types, self.params['vectorizer_dict_size'])
+            X = self._preprocess_train(X, feature_types, self.params["vectorizer_dict_size"])
         else:
             X = self._pipeline.transform(X)
         return X
 
     def _preprocess_train(self, X, feature_types, vect_max_features):
         transformer_list = []
-        if feature_types.get('language', None):
-            pipeline = Pipeline(steps=[
-                ("preparator", NlpDataPreprocessor(nlp_cols=feature_types['language'])),
-                ("vectorizer", TfidfVectorizer(ngram_range=self.params['proc.ngram_range'], sublinear_tf=True, max_features=vect_max_features, tokenizer=self._tokenize)),
-            ])
-            transformer_list.append(('vect', pipeline, feature_types['language']))
-        if feature_types.get('onehot', None):
-            pipeline = Pipeline(steps=[
-                ('generator', OheFeaturesGenerator()),
-            ])
-            transformer_list.append(('cats', pipeline, feature_types['onehot']))
-        if feature_types.get('continuous', None):
-            pipeline = Pipeline(steps=[
-                ('imputer', SimpleImputer(strategy=self.params['proc.impute_strategy'])),
-                ('scaler', StandardScaler())
-            ])
-            transformer_list.append(('cont', pipeline, feature_types['continuous']))
-        if feature_types.get('bool', None):
-            pipeline = Pipeline(steps=[
-                ('scaler', StandardScaler())
-            ])
-            transformer_list.append(('bool', pipeline, feature_types['bool']))
-        if feature_types.get('skewed', None):
-            pipeline = Pipeline(steps=[
-                ('imputer', SimpleImputer(strategy=self.params['proc.impute_strategy'])),
-                ('quantile', QuantileTransformer(output_distribution='normal')),  # Or output_distribution = 'uniform'
-            ])
-            transformer_list.append(('skew', pipeline, feature_types['skewed']))
+        if feature_types.get("language", None):
+            pipeline = Pipeline(
+                steps=[
+                    ("preparator", NlpDataPreprocessor(nlp_cols=feature_types["language"])),
+                    (
+                        "vectorizer",
+                        TfidfVectorizer(
+                            ngram_range=self.params["proc.ngram_range"], sublinear_tf=True, max_features=vect_max_features, tokenizer=self._tokenize
+                        ),
+                    ),
+                ]
+            )
+            transformer_list.append(("vect", pipeline, feature_types["language"]))
+        if feature_types.get("onehot", None):
+            pipeline = Pipeline(
+                steps=[
+                    ("generator", OheFeaturesGenerator()),
+                ]
+            )
+            transformer_list.append(("cats", pipeline, feature_types["onehot"]))
+        if feature_types.get("continuous", None):
+            pipeline = Pipeline(steps=[("imputer", SimpleImputer(strategy=self.params["proc.impute_strategy"])), ("scaler", StandardScaler())])
+            transformer_list.append(("cont", pipeline, feature_types["continuous"]))
+        if feature_types.get("bool", None):
+            pipeline = Pipeline(steps=[("scaler", StandardScaler())])
+            transformer_list.append(("bool", pipeline, feature_types["bool"]))
+        if feature_types.get("skewed", None):
+            pipeline = Pipeline(
+                steps=[
+                    ("imputer", SimpleImputer(strategy=self.params["proc.impute_strategy"])),
+                    ("quantile", QuantileTransformer(output_distribution="normal")),  # Or output_distribution = 'uniform'
+                ]
+            )
+            transformer_list.append(("skew", pipeline, feature_types["skewed"]))
         self._pipeline = ColumnTransformer(transformers=transformer_list)
         return self._pipeline.fit_transform(X)
 
     def _set_default_params(self):
-        default_params = {'random_state': 0, 'fit_intercept': True}
+        default_params = {"random_state": 0, "fit_intercept": True}
         if self.problem_type != REGRESSION:
-            default_params.update({'solver': _get_solver(self.problem_type)})
+            default_params.update({"solver": _get_solver(self.problem_type)})
         default_params.update(get_param_baseline())
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_searchspace(self):
         return get_default_searchspace(self.problem_type)
 
-    def _fit(self,
-             X,
-             y,
-             time_limit=None,
-             num_cpus=-1,
-             sample_weight=None,
-             **kwargs):
+    def _fit(self, X, y, time_limit=None, num_cpus=-1, sample_weight=None, **kwargs):
         time_fit_start = time.time()
         X = self.preprocess(X, is_train=True)
         if self.problem_type == BINARY:
             y = y.astype(int).values
 
         params = {k: v for k, v in self.params.items() if k not in preprocess_params_set}
-        if 'n_jobs' not in params:
+        if "n_jobs" not in params:
             if self.problem_type != REGRESSION:
-                params['n_jobs'] = num_cpus
+                params["n_jobs"] = num_cpus
 
         # Ridge/Lasso are using alpha instead of C, which is C^-1
         # https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html#sklearn.linear_model.Ridge
-        if self.problem_type == REGRESSION and 'alpha' not in params:
+        if self.problem_type == REGRESSION and "alpha" not in params:
             # For numerical reasons, using alpha = 0 with the Lasso object is not advised, so we add epsilon
-            params['alpha'] = 1 / (params['C'] if params['C'] != 0 else 1e-8)
-            params.pop('C', None)
+            params["alpha"] = 1 / (params["C"] if params["C"] != 0 else 1e-8)
+            params.pop("C", None)
 
-        logger.log(15, f'Training Model with the following hyperparameter settings:')
+        logger.log(15, f"Training Model with the following hyperparameter settings:")
         logger.log(15, params)
 
-        max_iter = params.pop('max_iter', 10000)
+        max_iter = params.pop("max_iter", 10000)
 
         # TODO: copy_X=True currently set during regression problem type, could potentially set to False to avoid unnecessary data copy.
         model_cls = self._get_model_type()
 
         time_fit_model_start = time.time()
         if time_limit is not None:
             time_left = time_limit - (time_fit_model_start - time_fit_start)
             time_left = time_left - 0.2  # Account for 0.2s of overhead
             if time_left <= 0:
                 raise TimeLimitExceeded
         else:
             time_left = None
 
         if time_left is not None and max_iter >= 200 and self.problem_type != REGRESSION:
-            max_iter_list = [100, max_iter-100]
+            max_iter_list = [100, max_iter - 100]
         else:
             max_iter_list = [max_iter]
 
         fit_args = dict(X=X, y=y)
         if sample_weight is not None:
-            fit_args['sample_weight'] = sample_weight
+            fit_args["sample_weight"] = sample_weight
 
         if len(max_iter_list) > 1:
-            params['warm_start'] = True  # Force True
+            params["warm_start"] = True  # Force True
 
         total_iter = 0
         total_iter_used = 0
         total_max_iter = sum(max_iter_list)
         model = model_cls(max_iter=max_iter_list[0], **params)
         early_stop = False
         for i, cur_max_iter in enumerate(max_iter_list):
@@ -203,36 +207,36 @@
                 time_spent = time.time() - time_fit_model_start
                 time_left_train = time_left - time_spent
                 time_per_iter = time_spent / total_iter
                 time_to_train_cur_max_iter = time_per_iter * cur_max_iter
                 if time_to_train_cur_max_iter > time_left_train:
                     cur_max_iter = min(int(time_left_train / time_per_iter) - 1, cur_max_iter)
                     if cur_max_iter <= 0:
-                        logger.warning(f'\tEarly stopping due to lack of time remaining. Fit {total_iter}/{total_max_iter} iters...')
+                        logger.warning(f"\tEarly stopping due to lack of time remaining. Fit {total_iter}/{total_max_iter} iters...")
                         break
                     early_stop = True
 
             model.max_iter = cur_max_iter
             with warnings.catch_warnings():
                 # Filter the not-converged warning since we are purposefully training in increments.
                 # FIXME: Annoyingly, this doesn't filter the warning on Mac due to how multiprocessing works when n_cpus>1. Unsure how to fix.
-                warnings.simplefilter(action='ignore', category=UserWarning)
+                warnings.simplefilter(action="ignore", category=UserWarning)
                 model = model.fit(**fit_args)
             total_iter += model.max_iter
             if model.n_iter_ is not None:
                 total_iter_used += model.n_iter_[0]
             else:
                 total_iter_used += model.max_iter
             if early_stop:
                 if total_iter_used == total_iter:  # Not yet converged
-                    logger.warning(f'\tEarly stopping due to lack of time remaining. Fit {total_iter}/{total_max_iter} iters...')
+                    logger.warning(f"\tEarly stopping due to lack of time remaining. Fit {total_iter}/{total_max_iter} iters...")
                 break
 
         self.model = model
-        self.params_trained['max_iter'] = total_iter
+        self.params_trained["max_iter"] = total_iter
 
     def _select_features_handle_text_include(self, df, categorical_featnames, language_featnames, continuous_featnames, bool_featnames):
         types_of_features = dict()
         types_of_features.update(self._select_continuous(df, continuous_featnames))
         types_of_features.update(self._select_bool(df, bool_featnames))
         types_of_features.update(self._select_categorical(df, categorical_featnames))
         types_of_features.update(self._select_text(df, language_featnames))
@@ -254,18 +258,18 @@
         return dict(onehot=features)
 
     def _select_continuous(self, df, features):
         # continuous = numeric features to rescale
         # skewed = features to which we will apply power (ie. log / box-cox) transform before normalization
         types_of_features = defaultdict(list)
         for feature in features:
-            if np.abs(df[feature].skew()) > self.params['proc.skew_threshold']:
-                types_of_features['skewed'].append(feature)
+            if np.abs(df[feature].skew()) > self.params["proc.skew_threshold"]:
+                types_of_features["skewed"].append(feature)
             else:
-                types_of_features['continuous'].append(feature)
+                types_of_features["continuous"].append(feature)
         return types_of_features
 
     def _select_text(self, df, features):
         return dict(language=features)
 
     def _select_bool(self, df, features):
         return dict(bool=features)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,20 +18,19 @@
         return self._encoder.transform_ohe(X)
 
     def get_feature_names(self):
         return self._feature_names
 
 
 class NlpDataPreprocessor(BaseEstimator, TransformerMixin):
-
     def __init__(self, nlp_cols):
         self.nlp_cols = nlp_cols
 
     def fit(self, X, y=None):
         return self
 
     def transform(self, X, y=None):
         X = X[self.nlp_cols].copy()
         for c in self.nlp_cols:
-            X[c] = X[c].astype(str).fillna(' ')
-        X = X.apply(' '.join, axis=1).str.replace('[ ]+', ' ', regex=True)
+            X[c] = X[c].astype(str).fillna(" ")
+        X = X.apply(" ".join, axis=1).str.replace("[ ]+", " ", regex=True)
         return X.values.tolist()
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
 import numpy as np
 
-from autogluon.core.constants import REGRESSION
 from autogluon.common.utils.try_import import try_import_rapids_cuml
+from autogluon.core.constants import REGRESSION
 
+from .._utils.rapids_utils import RapidsModelMixin
 from .hyperparameters.parameters import get_param_baseline
 from .lr_model import LinearModel
-from .._utils.rapids_utils import RapidsModelMixin
 
 logger = logging.getLogger(__name__)
 
 
 # FIXME: If rapids is installed, normal CPU LinearModel crashes.
 class LinearRapidsModel(RapidsModelMixin, LinearModel):
     """
@@ -20,39 +20,41 @@
     NOTE: This code is experimental, it is recommend to not use this unless you are a developer.
     This was tested on rapids-21.06 via:
 
     conda create -n rapids-21.06 -c rapidsai -c nvidia -c conda-forge rapids=21.06 python=3.8 cudatoolkit=11.2
     conda activate rapids-21.06
     pip install --pre autogluon.tabular[all]
     """
+
     def _get_model_type(self):
-        penalty = self.params.get('penalty', 'L2')
+        penalty = self.params.get("penalty", "L2")
         try_import_rapids_cuml()
-        from cuml.linear_model import LogisticRegression, Ridge, Lasso
+        from cuml.linear_model import Lasso, LogisticRegression, Ridge
+
         if self.problem_type == REGRESSION:
-            if penalty == 'L2':
+            if penalty == "L2":
                 model_type = Ridge
-            elif penalty == 'L1':
+            elif penalty == "L1":
                 model_type = Lasso
             else:
                 raise AssertionError(f'Unknown value for penalty "{penalty}" - supported types are ["L1", "L2"]')
         else:
             model_type = LogisticRegression
         return model_type
 
     def _set_default_params(self):
-        default_params = {'fit_intercept': True, 'max_iter': 10000}
+        default_params = {"fit_intercept": True, "max_iter": 10000}
         if self.problem_type != REGRESSION:
-            default_params.update({'solver': 'qn'})
+            default_params.update({"solver": "qn"})
         default_params.update(get_param_baseline())
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _preprocess(self, X, **kwargs):
         X = super()._preprocess(X=X, **kwargs)
         if not isinstance(X, np.ndarray):
             X = X.toarray()
         return X
 
     def _fit(self, X, y, **kwargs):
-        kwargs.pop('sample_weight', None)  # sample_weight is not supported
+        kwargs.pop("sample_weight", None)  # sample_weight is not supported
         super()._fit(X=X, y=y, **kwargs)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pickle
 
 
 class AbstractNativeCompiler:
-    name = 'native'
+    name = "native"
     save_in_pkl = True
 
     @staticmethod
     def can_compile():
         return True
 
     @staticmethod
@@ -28,18 +28,18 @@
         """
         AbstractNativeCompiler.save(model, path)
         return model
 
     @staticmethod
     def save(model, path: str):
         os.makedirs(os.path.dirname(path), exist_ok=True)
-        with open(path + 'model_native.pkl', 'wb') as fp:
+        with open(path + "model_native.pkl", "wb") as fp:
             fp.write(pickle.dumps(model))
 
     @staticmethod
     def load(path: str):
-        with open(path + 'model_native.pkl', 'rb') as fp:
+        with open(path + "model_native.pkl", "rb") as fp:
             pkl = fp.read()
         return pickle.loads(pkl)
 
 
 RFNativeCompiler = AbstractNativeCompiler
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
+
 import numpy as np
 
 
 class InferenceSessionWrapper:
     """
     Wrap around InferenceSession in onnxruntime, since it cannot be pickled.
     See https://github.com/microsoft/onnxruntime/issues/10097
     """
+
     def __init__(self, onnx_bytes):
         import onnxruntime as rt
-        self.sess = rt.InferenceSession(onnx_bytes.SerializeToString(),
-                                        providers=['CPUExecutionProvider'])
+
+        self.sess = rt.InferenceSession(onnx_bytes.SerializeToString(), providers=["CPUExecutionProvider"])
 
     def run(self, *args):
         return self.sess.run(*args)
 
     def get_inputs(self, *args):
         return self.sess.get_inputs(*args)
 
@@ -46,23 +48,23 @@
         label_name = self.sess.get_outputs()[1].name
         pred_proba = self.sess.run([label_name], {input_name: X})[0]
         pred_proba = np.array([[r[i] for i in range(self.num_classes)] for r in pred_proba])
         return pred_proba
 
 
 class RFOnnxCompiler:
-    name = 'onnx'
+    name = "onnx"
     save_in_pkl = False
 
     @staticmethod
     def can_compile():
         """Verify whether the required package has been installed."""
         try:
-            import skl2onnx
             import onnxruntime
+            import skl2onnx
 
             return True
         except ImportError:
             return False
 
     @staticmethod
     def compile(model, path: str, input_types=None):
@@ -77,30 +79,30 @@
             The path for saving the compiled model.
         input_types : list, default=None
             A list of tuples containing shape and element type info, e.g. [((1, 14), np.float32),].
             The list would be used as the input data for the model.
             The compiler would optimize the model to perform best with the given input type.
         """
         if input_types is None or not isinstance(input_types[0], tuple):
-            raise RuntimeError("input_types argument should contain at least one tuple"
-                               ", e.g. [((1, 14), np.float32)]")
+            raise RuntimeError("input_types argument should contain at least one tuple" ", e.g. [((1, 14), np.float32)]")
         if isinstance(model, RFOnnxPredictor):
             return model
 
         from skl2onnx import convert_sklearn
         from skl2onnx.common.data_types import FloatTensorType
-        from sklearn.ensemble import RandomForestClassifier, ExtraTreesClassifier
+        from sklearn.ensemble import ExtraTreesClassifier, RandomForestClassifier
+
         input_shape = list(input_types[0][0])
-        initial_type = [('float_input', FloatTensorType(input_shape))]
+        initial_type = [("float_input", FloatTensorType(input_shape))]
 
         # Without ZipMap
         # See http://onnx.ai/sklearn-onnx/auto_examples/plot_convert_zipmap.html#without-zipmap
         options = {}
         if isinstance(model, (RandomForestClassifier, ExtraTreesClassifier)):
-            options = {id(model): {'zipmap': False}}
+            options = {id(model): {"zipmap": False}}
 
         # Convert the model to onnx
         onnx_model = convert_sklearn(model, initial_types=initial_type, options=options)
         predictor = RFOnnxPredictor(model=onnx_model)
         RFOnnxCompiler.save(onnx_model, path)
         return predictor
 
@@ -112,9 +114,10 @@
             f.write(model.SerializeToString())
         return path + "model.onnx"
 
     @staticmethod
     def load(path: str) -> RFOnnxPredictor:
         """Load from the path that contains an onnx file."""
         import onnx
+
         onnx_bytes = onnx.load(path + "model.onnx")
         return RFOnnxPredictor(model=onnx_bytes)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 import logging
 import math
-import pickle
 import os
+import pickle
 import sys
 import time
 
 import numpy as np
 
-from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY
+from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT
 from autogluon.common.utils.resource_utils import ResourceManager
-from autogluon.core.constants import MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
+from autogluon.core.constants import MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
+from autogluon.core.models import AbstractModel
 from autogluon.core.utils.exceptions import NotEnoughMemoryError, TimeLimitExceeded
 from autogluon.core.utils.utils import normalize_pred_probas
-
-from autogluon.core.models import AbstractModel
 from autogluon.features.generators import LabelEncoderFeatureGenerator
 
 from .compilers.native import RFNativeCompiler
 from .compilers.onnx import RFOnnxCompiler
 
 logger = logging.getLogger(__name__)
 
 
 class RFModel(AbstractModel):
     """
     Random Forest model (scikit-learn): https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._feature_generator = None
         self._daal = False  # Whether daal4py backend is being used
         self._num_features_post_process = None
 
     def _get_model_type(self):
         if self.problem_type == QUANTILE:
             from .rf_quantile import RandomForestQuantileRegressor
+
             return RandomForestQuantileRegressor
-        if self.params_aux.get('use_daal', False):
+        if self.params_aux.get("use_daal", False):
             # Disabled by default because OOB score does not yet work properly
             try:
                 # FIXME: sklearnex OOB score is broken, returns biased predictions. Without this optimization, can't compute Efficient OOF.
                 #  Refer to https://github.com/intel/scikit-learn-intelex/issues/933
                 #  Current workaround: Forcibly set oob_score=True during fit to compute OOB during train time.
                 #  Downsides:
                 #    1. Slows down training slightly by forcing computation of OOB even if OOB is not needed (such as in medium_quality)
                 #    2. Makes computing the correct pred_time_val difficult, as the time is instead added to the fit_time,
                 #       and we would need to waste extra time to compute the proper pred_time_val post-fit.
                 #       Therefore with sklearnex enabled, pred_time_val is incorrect.
                 from sklearnex.ensemble import RandomForestClassifier, RandomForestRegressor
-                logger.log(15, '\tUsing sklearnex RF backend...')
+
+                logger.log(15, "\tUsing sklearnex RF backend...")
                 self._daal = True
             except:
                 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+
                 self._daal = False
         else:
             from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
+
             self._daal = False
         if self.problem_type in [REGRESSION, SOFTCLASS]:
             return RandomForestRegressor
         else:
             return RandomForestClassifier
 
     # TODO: X.fillna -inf? Add extra is_missing column?
@@ -73,26 +77,26 @@
         X = X.fillna(0).to_numpy(dtype=np.float32)
         return X
 
     def _set_default_params(self):
         default_params = {
             # TODO: 600 is much better, but increases info leakage in stacking -> therefore 300 is ~equal in stack ensemble final quality.
             #  Consider adding targeted noise to OOF to avoid info leakage, or increase `min_samples_leaf`.
-            'n_estimators': 300,
+            "n_estimators": 300,
             # Cap leaf nodes to 15000 to avoid large datasets using unreasonable amounts of memory/disk for RF/XT.
             #  Ensures that memory and disk usage of RF model with 300 n_estimators is at most ~500 MB for binary/regression, ~200 MB per class for multiclass.
             #  This has no effect on datasets with <=15000 rows, and minimal to no impact on datasets with <50000 rows.
             #  For large datasets, will often make the model worse, but will significantly speed up inference speed and massively reduce memory and disk usage.
             #  For example, when left uncapped, RF can use 5 GB of disk for a regression dataset with 2M rows.
             #  Multiply by the 8 RF/XT models in config for best quality / high quality and this is 40 GB of tree models, which is unreasonable.
             #  This size scales linearly with number of rows.
-            'max_leaf_nodes': 15000,
-            'n_jobs': -1,
-            'random_state': 0,
-            'bootstrap': True,  # Required for OOB estimates, setting to False will raise exception if bagging.
+            "max_leaf_nodes": 15000,
+            "n_jobs": -1,
+            "random_state": 0,
+            "bootstrap": True,  # Required for OOB estimates, setting to False will raise exception if bagging.
             # TODO: min_samples_leaf=5 is too large on most problems, however on some datasets it helps a lot (airlines likes >40 min_samples_leaf, adult likes 2 much better than 1)
             #  This value would need to be tuned per dataset, likely very worthwhile.
             #  Higher values = less OOF info leak, default = 1, which maximizes info leak.
             # 'min_samples_leaf': 5,  # Significantly reduces info leakage to stacker models. Never use the default/1 when using as base model.
             # 'oob_score': True,  # Disabled by default as it is better to do it post-fit via custom logic.
         }
         for param, val in default_params.items():
@@ -117,87 +121,80 @@
                 num_trees_per_estimator = self.num_classes
         else:
             num_trees_per_estimator = 1
         return num_trees_per_estimator
 
     def _estimate_memory_usage(self, X, **kwargs):
         params = self._get_model_params()
-        n_estimators_final = params['n_estimators']
+        n_estimators_final = params["n_estimators"]
         if isinstance(n_estimators_final, int):
             n_estimators_minimum = min(40, n_estimators_final)
         else:  # if search space
             n_estimators_minimum = 40
         num_trees_per_estimator = self._get_num_trees_per_estimator()
         bytes_per_estimator = num_trees_per_estimator * len(X) / 60000 * 1e6  # Underestimates by 3x on ExtraTrees
         expected_min_memory_usage = bytes_per_estimator * n_estimators_minimum
         return expected_min_memory_usage
 
     def _validate_fit_memory_usage(self, mem_error_threshold: float = 0.5, mem_warning_threshold: float = 0.4, mem_size_threshold: int = 1e7, **kwargs):
-        return super()._validate_fit_memory_usage(mem_error_threshold=mem_error_threshold,
-                                                  mem_warning_threshold=mem_warning_threshold,
-                                                  mem_size_threshold=mem_size_threshold,
-                                                  **kwargs)
+        return super()._validate_fit_memory_usage(
+            mem_error_threshold=mem_error_threshold, mem_warning_threshold=mem_warning_threshold, mem_size_threshold=mem_size_threshold, **kwargs
+        )
 
     def _expected_mem_usage(self, n_estimators_final, bytes_per_estimator):
         available_mem = ResourceManager.get_available_virtual_mem()
         return n_estimators_final * bytes_per_estimator / available_mem
 
-    def _fit(self,
-             X,
-             y,
-             num_cpus=-1,
-             time_limit=None,
-             sample_weight=None,
-             **kwargs):
+    def _fit(self, X, y, num_cpus=-1, time_limit=None, sample_weight=None, **kwargs):
         time_start = time.time()
 
         model_cls = self._get_model_type()
 
-        max_memory_usage_ratio = self.params_aux['max_memory_usage_ratio']
+        max_memory_usage_ratio = self.params_aux["max_memory_usage_ratio"]
         params = self._get_model_params()
-        if 'n_jobs' not in params:
-            params['n_jobs'] = num_cpus
-        n_estimators_final = params['n_estimators']
+        if "n_jobs" not in params:
+            params["n_jobs"] = num_cpus
+        n_estimators_final = params["n_estimators"]
 
         n_estimators_minimum = min(40, n_estimators_final)
-        n_estimators_test = min(4, max(1, math.floor(n_estimators_minimum/5)))
+        n_estimators_test = min(4, max(1, math.floor(n_estimators_minimum / 5)))
 
         X = self.preprocess(X)
         n_estimator_increments = [n_estimators_final]
 
         num_trees_per_estimator = self._get_num_trees_per_estimator()
         bytes_per_estimator = num_trees_per_estimator * len(X) / 60000 * 1e6  # Underestimates by 3x on ExtraTrees
         expected_memory_usage = self._expected_mem_usage(n_estimators_final, bytes_per_estimator)
 
         if n_estimators_final > n_estimators_test * 2:
             if self.problem_type == MULTICLASS:
                 n_estimator_increments = [n_estimators_test, n_estimators_final]
-                params['warm_start'] = True
+                params["warm_start"] = True
             else:
                 if expected_memory_usage > (0.05 * max_memory_usage_ratio):  # Somewhat arbitrary, consider finding a better value, should it scale by cores?
                     # Causes ~10% training slowdown, so try to avoid if memory is not an issue
                     n_estimator_increments = [n_estimators_test, n_estimators_final]
-                    params['warm_start'] = True
+                    params["warm_start"] = True
 
-        params['n_estimators'] = n_estimator_increments[0]
+        params["n_estimators"] = n_estimator_increments[0]
         if self._daal:
-            if params.get('warm_start', False):
-                params['warm_start'] = False
+            if params.get("warm_start", False):
+                params["warm_start"] = False
             # FIXME: This is inefficient but sklearnex doesn't support computing oob_score after training
-            params['oob_score'] = True
+            params["oob_score"] = True
 
         model = model_cls(**params)
 
         time_train_start = time.time()
         for i, n_estimators in enumerate(n_estimator_increments):
             if i != 0:
-                if params.get('warm_start', False):
+                if params.get("warm_start", False):
                     model.n_estimators = n_estimators
                 else:
-                    params['n_estimators'] = n_estimators
+                    params["n_estimators"] = n_estimators
                     model = model_cls(**params)
             model = model.fit(X, y, sample_weight=sample_weight)
             if (i == 0) and (len(n_estimator_increments) > 1):
                 time_elapsed = max(time.time() - time_train_start, 0.001)  # avoid it being too small and being truncated to 0
                 model_size_bytes = 0
                 for estimator in model.estimators_:  # Uses far less memory than pickling the entire forest at once
                     model_size_bytes += sys.getsizeof(pickle.dumps(estimator))
@@ -206,37 +203,43 @@
                 model_memory_ratio = expected_final_model_size_bytes / available_mem
 
                 ideal_memory_ratio = 0.15 * max_memory_usage_ratio
                 n_estimators_ideal = min(n_estimators_final, math.floor(ideal_memory_ratio / model_memory_ratio * n_estimators_final))
 
                 if n_estimators_final > n_estimators_ideal:
                     if n_estimators_ideal < n_estimators_minimum:
-                        logger.warning(f'\tWarning: Model is expected to require {round(model_memory_ratio*100, 2)}% of available memory...')
+                        logger.warning(f"\tWarning: Model is expected to require {round(model_memory_ratio*100, 2)}% of available memory...")
                         raise NotEnoughMemoryError  # don't train full model to avoid OOM error
-                    logger.warning(f'\tWarning: Reducing model \'n_estimators\' from {n_estimators_final} -> {n_estimators_ideal} due to low memory. Expected memory usage reduced from {round(model_memory_ratio*100, 2)}% -> {round(ideal_memory_ratio*100, 2)}% of available memory...')
+                    logger.warning(
+                        f"\tWarning: Reducing model 'n_estimators' from {n_estimators_final} -> {n_estimators_ideal} due to low memory. Expected memory usage reduced from {round(model_memory_ratio*100, 2)}% -> {round(ideal_memory_ratio*100, 2)}% of available memory..."
+                    )
 
                 if time_limit is not None:
                     time_expected = time_train_start - time_start + (time_elapsed * n_estimators_ideal / n_estimators)
                     n_estimators_time = math.floor((time_limit - time_train_start + time_start) * n_estimators / time_elapsed)
                     if n_estimators_time < n_estimators_ideal:
                         if n_estimators_time < n_estimators_minimum:
-                            logger.warning(f'\tWarning: Model is expected to require {round(time_expected, 1)}s to train, which exceeds the maximum time limit of {round(time_limit, 1)}s, skipping model...')
+                            logger.warning(
+                                f"\tWarning: Model is expected to require {round(time_expected, 1)}s to train, which exceeds the maximum time limit of {round(time_limit, 1)}s, skipping model..."
+                            )
                             raise TimeLimitExceeded
-                        logger.warning(f'\tWarning: Reducing model \'n_estimators\' from {n_estimators_ideal} -> {n_estimators_time} due to low time. Expected time usage reduced from {round(time_expected, 1)}s -> {round(time_limit, 1)}s...')
+                        logger.warning(
+                            f"\tWarning: Reducing model 'n_estimators' from {n_estimators_ideal} -> {n_estimators_time} due to low time. Expected time usage reduced from {round(time_expected, 1)}s -> {round(time_limit, 1)}s..."
+                        )
                         n_estimators_ideal = n_estimators_time
 
                 for j in range(len(n_estimator_increments)):
                     if n_estimator_increments[j] > n_estimators_ideal:
                         n_estimator_increments[j] = n_estimators_ideal
-        if self._daal and model.criterion != 'entropy':
+        if self._daal and model.criterion != "entropy":
             # TODO: entropy is not accelerated by sklearnex, need to not set estimators_ to None to avoid crash
             # This reduces memory usage / disk usage.
             model.estimators_ = None
         self.model = model
-        self.params_trained['n_estimators'] = self.model.n_estimators
+        self.params_trained["n_estimators"] = self.model.n_estimators
 
     # TODO: Remove this after simplifying _predict_proba to reduce code duplication. This is only present for SOFTCLASS support.
     def _predict_proba(self, X, **kwargs):
         X = self.preprocess(X, **kwargs)
 
         if self.problem_type == REGRESSION:
             return self.model.predict(X)
@@ -266,30 +269,31 @@
         """Returns True if model supports computing out-of-bag prediction probabilities"""
         # TODO: Remove `_set_oob_score` after sklearn version requirement is >=1.0
         return callable(getattr(self.model, "_set_oob_score", None)) or self._is_sklearn_1()
 
     # FIXME: Unknown if this works with quantile regression
     def _get_oof_pred_proba(self, X, y, **kwargs):
         if not self.model.bootstrap:
-            raise ValueError('Forest models must set `bootstrap=True` to compute out-of-fold predictions via out-of-bag predictions.')
+            raise ValueError("Forest models must set `bootstrap=True` to compute out-of-fold predictions via out-of-bag predictions.")
 
         oob_is_not_set = getattr(self.model, "oob_decision_function_", None) is None and getattr(self.model, "oob_prediction_", None) is None
 
         if oob_is_not_set and self._daal:
-            raise AssertionError('DAAL forest backend does not support out-of-bag predictions.')
+            raise AssertionError("DAAL forest backend does not support out-of-bag predictions.")
 
         # TODO: This can also be done via setting `oob_score=True` in model params,
         #  but getting the correct `pred_time_val` that way is not easy, since we can't time the internal call.
         if oob_is_not_set and self._model_supports_oob_pred_proba():
             X = self.preprocess(X)
 
             if getattr(self.model, "n_classes_", None) is not None:
                 if self.model.n_outputs_ == 1:
                     self.model.n_classes_ = [self.model.n_classes_]
-            from sklearn.tree._tree import DTYPE, DOUBLE
+            from sklearn.tree._tree import DOUBLE, DTYPE
+
             X, y = self.model._validate_data(X, y, multi_output=True, accept_sparse="csc", dtype=DTYPE)
             if y.ndim == 1:
                 # reshape is necessary to preserve the data contiguity against vs
                 # [:, np.newaxis] that does not.
                 y = np.reshape(y, (-1, 1))
             if getattr(y, "dtype", None) != DOUBLE or not y.flags.contiguous:
                 y = np.ascontiguousarray(y, dtype=DOUBLE)
@@ -308,22 +312,23 @@
         if getattr(self.model, "oob_decision_function_", None) is not None:
             y_oof_pred_proba = self.model.oob_decision_function_
             self.model.oob_decision_function_ = None  # save memory
         elif getattr(self.model, "oob_prediction_", None) is not None:
             y_oof_pred_proba = self.model.oob_prediction_
             self.model.oob_prediction_ = None  # save memory
         else:
-            raise AssertionError(f'Model class {type(self.model)} does not support out-of-fold prediction generation.')
+            raise AssertionError(f"Model class {type(self.model)} does not support out-of-fold prediction generation.")
 
         # TODO: Regression does not return NaN for missing rows, instead it sets them to 0. This makes life hard.
         #  The below code corrects the missing rows to NaN instead of 0.
         # Don't bother if >60 trees, near impossible to have missing
         # If using 68% of data for training, chance of missing for each row is 1 in 11 billion.
         if self.problem_type == REGRESSION and self.model.n_estimators <= 60:
-            from sklearn.ensemble._forest import _get_n_samples_bootstrap, _generate_unsampled_indices
+            from sklearn.ensemble._forest import _generate_unsampled_indices, _get_n_samples_bootstrap
+
             n_samples = len(y)
 
             n_predictions = np.zeros(n_samples)
             n_samples_bootstrap = _get_n_samples_bootstrap(n_samples, self.model.max_samples)
             for estimator in self.model.estimators_:
                 unsampled_indices = _generate_unsampled_indices(estimator.random_state, n_samples, n_samples_bootstrap)
                 n_predictions[unsampled_indices] += 1
@@ -350,26 +355,26 @@
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     @classmethod
     def _get_default_ag_args_ensemble(cls, problem_type=None, **kwargs) -> dict:
         default_ag_args_ensemble = super()._get_default_ag_args_ensemble(problem_type=problem_type, **kwargs)
         if problem_type != QUANTILE:  # use_child_oof not supported in quantile regression
-            extra_ag_args_ensemble = {'use_child_oof': True}
+            extra_ag_args_ensemble = {"use_child_oof": True}
             default_ag_args_ensemble.update(extra_ag_args_ensemble)
         return default_ag_args_ensemble
 
     def _more_tags(self):
         # `can_refit_full=True` because final n_estimators is communicated at end of `_fit`:
         #  `self.params_trained['n_estimators'] = self.model.n_estimators`
-        tags = {'can_refit_full': True}
+        tags = {"can_refit_full": True}
         if self.problem_type == QUANTILE:
-            tags['valid_oof'] = False  # not supported in quantile regression
+            tags["valid_oof"] = False  # not supported in quantile regression
         else:
-            tags['valid_oof'] = True
+            tags["valid_oof"] = True
         return tags
 
     def _valid_compilers(self):
         return [RFNativeCompiler, RFOnnxCompiler]
 
     def _default_compiler(self):
         return RFNativeCompiler
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,24 +31,21 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
 # OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
 # DAMAGE.
 
 import logging
-import pandas as pd
-import numpy as np
 from functools import partial
-from sklearn.tree import BaseDecisionTree
-from sklearn.tree import DecisionTreeRegressor
-from sklearn.tree import ExtraTreeRegressor
+
+import numpy as np
+import pandas as pd
 from sklearn.ensemble._forest import ForestRegressor
-from sklearn.utils import check_array
-from sklearn.utils import check_X_y
-from sklearn.utils import check_random_state
+from sklearn.tree import BaseDecisionTree, DecisionTreeRegressor, ExtraTreeRegressor
+from sklearn.utils import check_array, check_random_state, check_X_y
 
 logger = logging.getLogger(__name__)
 
 
 def weighted_percentile(a, q, weights=None, sorter=None, is_filtered=False):
     """
     Returns the weighted percentile of a at q given weights.
@@ -550,17 +547,15 @@
             quantile_levels = [quantile_levels]
 
         X_leaves = self.apply(X)
 
         samples_with_weighted_neighbors = get_weighted_neighbors_dataframe(
             X_leaves=X_leaves, y_train_leaves=self.y_train_leaves_, y_train=self.y_train_, y_weights=self.y_weights_
         )
-        quantile_preds = samples_with_weighted_neighbors.groupby("item_id").apply(
-            partial(get_quantiles, quantile_levels=quantile_levels)
-        )
+        quantile_preds = samples_with_weighted_neighbors.groupby("item_id").apply(partial(get_quantiles, quantile_levels=quantile_levels))
         return np.stack(quantile_preds.values.tolist())
 
 
 class RandomForestQuantileRegressor(BaseForestQuantileRegressor):
     """
     A random forest regressor that provides quantile estimates.
     A random forest is a meta estimator that fits a number of classifying
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import logging
 
-from autogluon.core.constants import REGRESSION, SOFTCLASS
 from autogluon.common.utils.try_import import try_import_rapids_cuml
+from autogluon.core.constants import REGRESSION, SOFTCLASS
 
-from .rf_model import RFModel
 from .._utils.rapids_utils import RapidsModelMixin
+from .rf_model import RFModel
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Improve memory safety
 # TODO: Respect time limit
-# TODO: Depending on max_depth parameter, RFRapidsModel is slower than RFModel. 
-#  A lower max_depth (e.g., 16) results in a RFRapidsModel that is faster than RFModel, 
+# TODO: Depending on max_depth parameter, RFRapidsModel is slower than RFModel.
+#  A lower max_depth (e.g., 16) results in a RFRapidsModel that is faster than RFModel,
 #  but a higher max_depth (e.g., approximating unlimited depth)
-#  results in a RFRapidsModel that is significantly slower than RFModel. 
+#  results in a RFRapidsModel that is significantly slower than RFModel.
 #  Refer to https://github.com/rapidsai/cuml/issues/1977
 class RFRapidsModel(RapidsModelMixin, RFModel):
     """
     RAPIDS Random Forest model : https://rapids.ai/start.html
 
     NOTE: This code is experimental, it is recommend to not use this unless you are a developer.
     This was tested on rapids-21.06 via:
 
     conda create -n rapids-21.06 -c rapidsai -c nvidia -c conda-forge rapids=21.06 python=3.8 cudatoolkit=11.2
     conda activate rapids-21.06
     pip install --pre autogluon.tabular[all]
     """
+
     def _get_model_type(self):
         try_import_rapids_cuml()
         from cuml.ensemble import RandomForestClassifier, RandomForestRegressor
+
         if self.problem_type in [REGRESSION, SOFTCLASS]:
             return RandomForestRegressor
         else:
             return RandomForestClassifier
 
     def _set_default_params(self):
         default_params = {
-            'n_estimators': 300,
-            'max_depth': 99,  # RAPIDS does not allow unlimited depth, so this approximates it.
-            'random_state': 0,
+            "n_estimators": 300,
+            "max_depth": 99,  # RAPIDS does not allow unlimited depth, so this approximates it.
+            "random_state": 0,
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _fit(self, X, y, **kwargs):
         X = self.preprocess(X)
         self.model = self._get_model_type()(**self._get_model_params())
         self.model = self.model.fit(X, y)
-        self.params_trained['n_estimators'] = self.model.n_estimators
+        self.params_trained["n_estimators"] = self.model.n_estimators
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,67 @@
-
 def get_fixed_params():
-    """ Parameters that currently cannot be searched during HPO """
-    fixed_params = {'batch_size': 512, # The size of example chunks to predict on.
-                    'n_cont_embeddings': 0, # How many continuous feature embeddings to use.
-                    'norm_class_name': 'LayerNorm', # What kind of normalization to use on continuous features.
-                    'column_embedding': True, # If True, 1/(n_shared_embs)th of every embedding will be reserved for a learned parameter that's common to all embeddings.
-                    #'shared_embedding': False,
-                    #'n_shared_embs': 8,
-                    'orig_emb_resid': False, # If True, concatenate the original embeddings on top of the feature embeddings in the Transformer layers.
-                    'one_hot_embeddings': False, # If True, one-hot encode variables whose cardinality is < max_emb_dim.
-                    'drop_whole_embeddings': False, # If True, dropout pretends the embedding was a missing value. If false, dropout sets embed features to 0
-                    'max_emb_dim': 8, # Maximum allowable amount of embeddings.
-                    'base_exp_decay': 0.95, # Rate of exponential decay for learning rate, used during finetuning.
-                    'encoders':  {'CATEGORICAL': 'CategoricalOrdinalEnc', # How to "encode"(vectorize) each column type.
-                                  'DATETIME'   : 'DatetimeOrdinalEnc',
-                                  'LATLONG'    : 'LatLongQuantileOrdinalEnc',
-                                  'SCALAR'     : 'ScalarQuantileOrdinalEnc',
-                                  'TEXT'       : 'TextSummaryScalarEnc'},
-                    'aug_mask_prob' : 0.4, # What percentage of values to apply augmentation to.
-                    'num_augs' : 0, # Number of augmentations to add.
-                    'pretext': 'BERTPretext', # What pretext to use when performing pretraining/semi-supervised learning.
-                    'n_cont_features': 8, # How many continuous features to concatenate onto the categorical features
-                    'fix_attention': False, # If True, use the categorical embeddings in the transformer architecture.
-                    'epochs': 200, # How many epochs to train on with labeled data.
-                    'pretrain_epochs': 200, # How many epochs to pretrain on with unlabeled data.
-                    'epochs_wo_improve': 30, # How many epochs to continue running without improving on metric. aka "Early Stopping Patience"
-                    'num_workers': 16, # How many workers to use for torch DataLoader.
-                    'max_columns': 500, # Maximum number of columns TabTransformer will accept as input. This is to combat huge memory requirements/errors.
-                    'tab_readout': 'none', # What sort of readout from the transformer. Options: ['readout_emb', 'mean', 'concat_pool', 'concat_pool_all', 'concat_pool_add', 'all_feat_embs', 'mean_feat_embs', 'none']
-                    }
+    """Parameters that currently cannot be searched during HPO"""
+    fixed_params = {
+        "batch_size": 512,  # The size of example chunks to predict on.
+        "n_cont_embeddings": 0,  # How many continuous feature embeddings to use.
+        "norm_class_name": "LayerNorm",  # What kind of normalization to use on continuous features.
+        "column_embedding": True,  # If True, 1/(n_shared_embs)th of every embedding will be reserved for a learned parameter that's common to all embeddings.
+        #'shared_embedding': False,
+        #'n_shared_embs': 8,
+        "orig_emb_resid": False,  # If True, concatenate the original embeddings on top of the feature embeddings in the Transformer layers.
+        "one_hot_embeddings": False,  # If True, one-hot encode variables whose cardinality is < max_emb_dim.
+        "drop_whole_embeddings": False,  # If True, dropout pretends the embedding was a missing value. If false, dropout sets embed features to 0
+        "max_emb_dim": 8,  # Maximum allowable amount of embeddings.
+        "base_exp_decay": 0.95,  # Rate of exponential decay for learning rate, used during finetuning.
+        "encoders": {
+            "CATEGORICAL": "CategoricalOrdinalEnc",  # How to "encode"(vectorize) each column type.
+            "DATETIME": "DatetimeOrdinalEnc",
+            "LATLONG": "LatLongQuantileOrdinalEnc",
+            "SCALAR": "ScalarQuantileOrdinalEnc",
+            "TEXT": "TextSummaryScalarEnc",
+        },
+        "aug_mask_prob": 0.4,  # What percentage of values to apply augmentation to.
+        "num_augs": 0,  # Number of augmentations to add.
+        "pretext": "BERTPretext",  # What pretext to use when performing pretraining/semi-supervised learning.
+        "n_cont_features": 8,  # How many continuous features to concatenate onto the categorical features
+        "fix_attention": False,  # If True, use the categorical embeddings in the transformer architecture.
+        "epochs": 200,  # How many epochs to train on with labeled data.
+        "pretrain_epochs": 200,  # How many epochs to pretrain on with unlabeled data.
+        "epochs_wo_improve": 30,  # How many epochs to continue running without improving on metric. aka "Early Stopping Patience"
+        "num_workers": 16,  # How many workers to use for torch DataLoader.
+        "max_columns": 500,  # Maximum number of columns TabTransformer will accept as input. This is to combat huge memory requirements/errors.
+        "tab_readout": "none",  # What sort of readout from the transformer. Options: ['readout_emb', 'mean', 'concat_pool', 'concat_pool_all', 'concat_pool_add', 'all_feat_embs', 'mean_feat_embs', 'none']
+    }
 
     return fixed_params
 
+
 def get_hyper_params():
-    """ Parameters that currently can be tuned during HPO """
+    """Parameters that currently can be tuned during HPO"""
     hyper_params = {
-        'lr': 3.6e-3, # Learning rate
+        "lr": 3.6e-3,  # Learning rate
         # Options: Real(5e-5, 5e-3)
-        'weight_decay': 1e-6, # Rate of linear weight decay for learning rate
+        "weight_decay": 1e-6,  # Rate of linear weight decay for learning rate
         # Options: Real(1e-6, 5e-2)
-        'p_dropout': 0, # dropout probability, 0 turns off Dropout.
+        "p_dropout": 0,  # dropout probability, 0 turns off Dropout.
         # Options: Categorical(0, 0.1, 0.2, 0.3, 0.4, 0.5)
-        'n_heads': 4, # Number of attention heads
+        "n_heads": 4,  # Number of attention heads
         # Options: Categorical(2, 4, 8)
-        'hidden_dim': 128, # hidden dimension size
+        "hidden_dim": 128,  # hidden dimension size
         # Options: Categorical(32, 64, 128, 256)
-        'n_layers': 2, # Number of Tab Transformer encoder layers,
+        "n_layers": 2,  # Number of Tab Transformer encoder layers,
         # Options: Categorical(1, 2, 3, 4, 5)
-        'feature_dim': 64, # Size of fully connected layer in TabNet.
+        "feature_dim": 64,  # Size of fully connected layer in TabNet.
         # Options: Int(8, 128)
-        'num_output_layers': 1 # How many fully-connected layers on top of transformer to produce predictions. Minimum 1 layer.
+        "num_output_layers": 1  # How many fully-connected layers on top of transformer to produce predictions. Minimum 1 layer.
         # Options: Categorical(1, 2, 3)
     }
 
     return hyper_params
 
+
 def get_default_param():
 
     params = get_fixed_params()
     params.update(get_hyper_params())
 
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,60 +2,62 @@
 This code is a modification of the official PyTorch Transformer code found at: 
 https://github.com/pytorch/pytorch/blob/master/torch/nn/modules/transformer.py
 
 The modification allows the option of fixing the attention map 
 """
 
 import math
-from typing import Tuple, Optional
+from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
+
 # Needed for pytorch 1.7 and 1.2
 try:
-    from torch.overrides import has_torch_function, handle_torch_function
+    from torch.overrides import handle_torch_function, has_torch_function
 # Needed for pytorch 1.6
 except ImportError:
     from torch._overrides import has_torch_function, handle_torch_function
-from torch.nn import Module
-from torch.nn import init
-from torch.nn.functional import linear, softmax, dropout
-from torch.nn.init import xavier_uniform_, constant_, xavier_normal_
+
+from torch.nn import Module, init
+from torch.nn.functional import dropout, linear, softmax
+from torch.nn.init import constant_, xavier_normal_, xavier_uniform_
 from torch.nn.modules.dropout import Dropout
 from torch.nn.modules.normalization import LayerNorm
 from torch.nn.parameter import Parameter
 
 
-def multi_head_attention_forward(self,
-                                 query,  # type: Tensor
-                                 key,  # type: Tensor
-                                 value,  # type: Tensor
-                                 embed_dim_to_check,  # type: int
-                                 num_heads,  # type: int
-                                 in_proj_weight,  # type: Tensor
-                                 in_proj_bias,  # type: Tensor
-                                 bias_k,  # type: Optional[Tensor]
-                                 bias_v,  # type: Optional[Tensor]
-                                 add_zero_attn,  # type: bool
-                                 dropout_p,  # type: float
-                                 out_proj_weight,  # type: Tensor
-                                 out_proj_bias,
-                                 fixed_k=None,  # type: Tensor
-                                 fixed_q=None,  # type: Tensor
-                                 training=True,  # type: bool
-                                 key_padding_mask=None,  # type: Optional[Tensor]
-                                 need_weights=True,  # type: bool
-                                 attn_mask=None,  # type: Optional[Tensor]
-                                 use_separate_proj_weight=False,  # type: bool
-                                 q_proj_weight=None,  # type: Optional[Tensor]
-                                 k_proj_weight=None,  # type: Optional[Tensor]
-                                 v_proj_weight=None,  # type: Optional[Tensor]
-                                 static_k=None,  # type: Optional[Tensor]
-                                 static_v=None  # type: Optional[Tensor]
-                                 ):
+def multi_head_attention_forward(
+    self,
+    query,  # type: Tensor
+    key,  # type: Tensor
+    value,  # type: Tensor
+    embed_dim_to_check,  # type: int
+    num_heads,  # type: int
+    in_proj_weight,  # type: Tensor
+    in_proj_bias,  # type: Tensor
+    bias_k,  # type: Optional[Tensor]
+    bias_v,  # type: Optional[Tensor]
+    add_zero_attn,  # type: bool
+    dropout_p,  # type: float
+    out_proj_weight,  # type: Tensor
+    out_proj_bias,
+    fixed_k=None,  # type: Tensor
+    fixed_q=None,  # type: Tensor
+    training=True,  # type: bool
+    key_padding_mask=None,  # type: Optional[Tensor]
+    need_weights=True,  # type: bool
+    attn_mask=None,  # type: Optional[Tensor]
+    use_separate_proj_weight=False,  # type: bool
+    q_proj_weight=None,  # type: Optional[Tensor]
+    k_proj_weight=None,  # type: Optional[Tensor]
+    v_proj_weight=None,  # type: Optional[Tensor]
+    static_k=None,  # type: Optional[Tensor]
+    static_v=None,  # type: Optional[Tensor]
+):
     # type: (...) -> Tuple[Tensor, Optional[Tensor]]
     """
     Args:
         query, key, value: map a query and a set of key-value pairs to an output.
             See "Attention Is All You Need" for more details.
         embed_dim_to_check: total dimension of the model.
         num_heads: parallel attention heads.
@@ -104,26 +106,43 @@
         - attn_output: :math:`(L, N, E)` where L is the target sequence length, N is the batch size,
           E is the embedding dimension.
         - attn_output_weights: :math:`(N, L, S)` where N is the batch size,
           L is the target sequence length, S is the source sequence length.
     """
 
     if not torch.jit.is_scripting():
-        tens_ops = (query, key, value, in_proj_weight, in_proj_bias, bias_k, bias_v,
-                    out_proj_weight, out_proj_bias)
+        tens_ops = (query, key, value, in_proj_weight, in_proj_bias, bias_k, bias_v, out_proj_weight, out_proj_bias)
         if any([type(t) is not torch.Tensor for t in tens_ops]) and has_torch_function(tens_ops):
             return handle_torch_function(
-                self.multi_head_attention_forward, tens_ops, query, key, value,
-                embed_dim_to_check, num_heads, in_proj_weight, in_proj_bias,
-                bias_k, bias_v, add_zero_attn, dropout_p, out_proj_weight,
-                out_proj_bias, training=training, key_padding_mask=key_padding_mask,
-                need_weights=need_weights, attn_mask=attn_mask,
+                self.multi_head_attention_forward,
+                tens_ops,
+                query,
+                key,
+                value,
+                embed_dim_to_check,
+                num_heads,
+                in_proj_weight,
+                in_proj_bias,
+                bias_k,
+                bias_v,
+                add_zero_attn,
+                dropout_p,
+                out_proj_weight,
+                out_proj_bias,
+                training=training,
+                key_padding_mask=key_padding_mask,
+                need_weights=need_weights,
+                attn_mask=attn_mask,
                 use_separate_proj_weight=use_separate_proj_weight,
-                q_proj_weight=q_proj_weight, k_proj_weight=k_proj_weight,
-                v_proj_weight=v_proj_weight, static_k=static_k, static_v=static_v)
+                q_proj_weight=q_proj_weight,
+                k_proj_weight=k_proj_weight,
+                v_proj_weight=v_proj_weight,
+                static_k=static_k,
+                static_v=static_v,
+            )
     tgt_len, bsz, embed_dim = query.size()
 
     assert embed_dim == embed_dim_to_check
     # allow MHA to have different sizes for the feature dimension
     assert key.size(0) == value.size(0) and key.size(1) == value.size(1)
 
     head_dim = embed_dim // num_heads
@@ -189,21 +208,21 @@
         query, key, and value have the same number of features.
 
     Examples::
 
         >>> multihead_attn = nn.MultiheadAttention(embed_dim, num_heads)
         >>> attn_output, attn_output_weights = multihead_attn(query, key, value)
     """
+
     __annotations__ = {
-        'bias_k': torch._jit_internal.Optional[torch.Tensor],
-        'bias_v': torch._jit_internal.Optional[torch.Tensor],
+        "bias_k": torch._jit_internal.Optional[torch.Tensor],
+        "bias_v": torch._jit_internal.Optional[torch.Tensor],
     }
 
-    def __init__(self, embed_dim, n_cat_embeddings, num_heads, dropout=0., bias=True, add_bias_kv=False,
-                 add_zero_attn=False, kdim=None, vdim=None):
+    def __init__(self, embed_dim, n_cat_embeddings, num_heads, dropout=0.0, bias=True, add_bias_kv=False, add_zero_attn=False, kdim=None, vdim=None):
         super().__init__()
 
         self.embed_dim = embed_dim
         self.kdim = kdim if kdim is not None else embed_dim
         self.vdim = vdim if vdim is not None else embed_dim
         self._qkv_same_embed_dim = self.kdim == embed_dim and self.vdim == embed_dim
 
@@ -212,29 +231,29 @@
         self.head_dim = embed_dim // num_heads
         assert self.head_dim * num_heads == self.embed_dim, "embed_dim must be divisible by num_heads"
 
         if self._qkv_same_embed_dim is False:
             self.q_proj_weight = Parameter(torch.Tensor(embed_dim, embed_dim))
             self.k_proj_weight = Parameter(torch.Tensor(embed_dim, self.kdim))
             self.v_proj_weight = Parameter(torch.Tensor(embed_dim, self.vdim))
-            self.register_parameter('in_proj_weight', None)
-            self.register_parameter('fixed_k', None)
+            self.register_parameter("in_proj_weight", None)
+            self.register_parameter("fixed_k", None)
         else:
             self.in_proj_weight = Parameter(torch.empty(embed_dim, embed_dim))
             # self.in_proj_weight = Parameter(torch.empty(2 * embed_dim, embed_dim))
             self.fixed_k = Parameter(torch.empty(n_cat_embeddings, embed_dim))
             self.fixed_q = Parameter(torch.empty(n_cat_embeddings, embed_dim))
-            self.register_parameter('q_proj_weight', None)
-            self.register_parameter('k_proj_weight', None)
-            self.register_parameter('v_proj_weight', None)
+            self.register_parameter("q_proj_weight", None)
+            self.register_parameter("k_proj_weight", None)
+            self.register_parameter("v_proj_weight", None)
 
         if bias:
             self.in_proj_bias = Parameter(torch.empty(embed_dim))
         else:
-            self.register_parameter('in_proj_bias', None)
+            self.register_parameter("in_proj_bias", None)
         self.out_proj = _LinearWithBias(embed_dim, embed_dim)
 
         if add_bias_kv:
             self.bias_k = Parameter(torch.empty(1, 1, embed_dim))
             self.bias_v = Parameter(torch.empty(1, 1, embed_dim))
         else:
             self.bias_k = self.bias_v = None
@@ -250,77 +269,92 @@
             xavier_uniform_(self.fixed_q)
         else:
             xavier_uniform_(self.q_proj_weight)
             xavier_uniform_(self.k_proj_weight)
             xavier_uniform_(self.v_proj_weight)
 
         if self.in_proj_bias is not None:
-            constant_(self.in_proj_bias, 0.)
-            constant_(self.out_proj.bias, 0.)
+            constant_(self.in_proj_bias, 0.0)
+            constant_(self.out_proj.bias, 0.0)
         if self.bias_k is not None:
             xavier_normal_(self.bias_k)
         if self.bias_v is not None:
             xavier_normal_(self.bias_v)
 
     def __setstate__(self, state):
         # Support loading old MultiheadAttention checkpoints generated by v1.1.0
-        if '_qkv_same_embed_dim' not in state:
-            state['_qkv_same_embed_dim'] = True
+        if "_qkv_same_embed_dim" not in state:
+            state["_qkv_same_embed_dim"] = True
 
         super().__setstate__(state)
 
-    def forward(self, query, key, value, key_padding_mask=None,
-                need_weights=True, attn_mask=None):
+    def forward(self, query, key, value, key_padding_mask=None, need_weights=True, attn_mask=None):
         # type: (Tensor, Tensor, Tensor, Optional[Tensor], bool, Optional[Tensor]) -> Tuple[Tensor, Optional[Tensor]]
         """
-    Args:
-        query, key, value: map a query and a set of key-value pairs to an output.
-            See "Attention Is All You Need" for more details.
-        key_padding_mask: if provided, specified padding elements in the key will
-            be ignored by the attention. When given a binary mask and a value is True,
-            the corresponding value on the attention layer will be ignored. When given
-            a byte mask and a value is non-zero, the corresponding value on the attention
-            layer will be ignored
-        need_weights: output attn_output_weights.
-        attn_mask: 2D or 3D mask that prevents attention to certain positions. A 2D mask will be broadcasted for all
-            the batches while a 3D mask allows to specify a different mask for the entries of each batch.
-
-    Shape:
-        - Inputs:
-        - query: :math:`(L, N, E)` where L is the target sequence length, N is the batch size, E is
-          the embedding dimension.
-        - key: :math:`(S, N, E)`, where S is the source sequence length, N is the batch size, E is
-          the embedding dimension.
-        - value: :math:`(S, N, E)` where S is the source sequence length, N is the batch size, E is
-          the embedding dimension.
-        - key_padding_mask: :math:`(N, S)` where N is the batch size, S is the source sequence length.
-          If a ByteTensor is provided, the non-zero positions will be ignored while the position
-          with the zero positions will be unchanged. If a BoolTensor is provided, the positions with the
-          value of ``True`` will be ignored while the position with the value of ``False`` will be unchanged.
-        - attn_mask: 2D mask :math:`(L, S)` where L is the target sequence length, S is the source sequence length.
-          3D mask :math:`(N*num_heads, L, S)` where N is the batch size, L is the target sequence length,
-          S is the source sequence length. attn_mask ensure that position i is allowed to attend the unmasked
-          positions. If a ByteTensor is provided, the non-zero positions are not allowed to attend
-          while the zero positions will be unchanged. If a BoolTensor is provided, positions with ``True``
-          is not allowed to attend while ``False`` values will be unchanged. If a FloatTensor
-          is provided, it will be added to the attention weight.
+        Args:
+            query, key, value: map a query and a set of key-value pairs to an output.
+                See "Attention Is All You Need" for more details.
+            key_padding_mask: if provided, specified padding elements in the key will
+                be ignored by the attention. When given a binary mask and a value is True,
+                the corresponding value on the attention layer will be ignored. When given
+                a byte mask and a value is non-zero, the corresponding value on the attention
+                layer will be ignored
+            need_weights: output attn_output_weights.
+            attn_mask: 2D or 3D mask that prevents attention to certain positions. A 2D mask will be broadcasted for all
+                the batches while a 3D mask allows to specify a different mask for the entries of each batch.
 
-        - Outputs:
-        - attn_output: :math:`(L, N, E)` where L is the target sequence length, N is the batch size,
-          E is the embedding dimension.
-        - attn_output_weights: :math:`(N, L, S)` where N is the batch size,
-          L is the target sequence length, S is the source sequence length.
+        Shape:
+            - Inputs:
+            - query: :math:`(L, N, E)` where L is the target sequence length, N is the batch size, E is
+              the embedding dimension.
+            - key: :math:`(S, N, E)`, where S is the source sequence length, N is the batch size, E is
+              the embedding dimension.
+            - value: :math:`(S, N, E)` where S is the source sequence length, N is the batch size, E is
+              the embedding dimension.
+            - key_padding_mask: :math:`(N, S)` where N is the batch size, S is the source sequence length.
+              If a ByteTensor is provided, the non-zero positions will be ignored while the position
+              with the zero positions will be unchanged. If a BoolTensor is provided, the positions with the
+              value of ``True`` will be ignored while the position with the value of ``False`` will be unchanged.
+            - attn_mask: 2D mask :math:`(L, S)` where L is the target sequence length, S is the source sequence length.
+              3D mask :math:`(N*num_heads, L, S)` where N is the batch size, L is the target sequence length,
+              S is the source sequence length. attn_mask ensure that position i is allowed to attend the unmasked
+              positions. If a ByteTensor is provided, the non-zero positions are not allowed to attend
+              while the zero positions will be unchanged. If a BoolTensor is provided, positions with ``True``
+              is not allowed to attend while ``False`` values will be unchanged. If a FloatTensor
+              is provided, it will be added to the attention weight.
+
+            - Outputs:
+            - attn_output: :math:`(L, N, E)` where L is the target sequence length, N is the batch size,
+              E is the embedding dimension.
+            - attn_output_weights: :math:`(N, L, S)` where N is the batch size,
+              L is the target sequence length, S is the source sequence length.
         """
 
-        return multi_head_attention_forward(self,
-            query=query, key=key, value=value, embed_dim_to_check=self.embed_dim, num_heads=self.num_heads,
-            in_proj_weight=self.in_proj_weight, in_proj_bias=self.in_proj_bias, bias_k=self.bias_k, bias_v=self.bias_v,
-            add_zero_attn=self.add_zero_attn, dropout_p=self.dropout, out_proj_weight=self.out_proj.weight,
-            out_proj_bias=self.out_proj.bias, fixed_k=self.fixed_k, fixed_q=self.fixed_q, training=self.training,
-            key_padding_mask=key_padding_mask, need_weights=need_weights, attn_mask=attn_mask)
+        return multi_head_attention_forward(
+            self,
+            query=query,
+            key=key,
+            value=value,
+            embed_dim_to_check=self.embed_dim,
+            num_heads=self.num_heads,
+            in_proj_weight=self.in_proj_weight,
+            in_proj_bias=self.in_proj_bias,
+            bias_k=self.bias_k,
+            bias_v=self.bias_v,
+            add_zero_attn=self.add_zero_attn,
+            dropout_p=self.dropout,
+            out_proj_weight=self.out_proj.weight,
+            out_proj_bias=self.out_proj.bias,
+            fixed_k=self.fixed_k,
+            fixed_q=self.fixed_q,
+            training=self.training,
+            key_padding_mask=key_padding_mask,
+            need_weights=need_weights,
+            attn_mask=attn_mask,
+        )
 
 
 class Linear(Module):
     r"""Applies a linear transformation to the incoming data: :math:`y = xA^T + b`
     Args:
         in_features: size of each input sample
         out_features: size of each output sample
@@ -344,45 +378,43 @@
         >>> m = nn.Linear(20, 30)
         >>> input = torch.randn(128, 20)
         >>> output = m(input)
         >>> print(output.size())
         torch.Size([128, 30])
     """
 
-    __constants__ = ['in_features', 'out_features']
+    __constants__ = ["in_features", "out_features"]
     in_features: int
     out_features: int
     weight: torch.Tensor
 
     def __init__(self, in_features: int, out_features: int, bias: bool = True) -> None:
         super().__init__()
 
         self.in_features = in_features
         self.out_features = out_features
         self.weight = Parameter(torch.Tensor(out_features, in_features))
         if bias:
             self.bias = Parameter(torch.Tensor(out_features))
         else:
-            self.register_parameter('bias', None)
+            self.register_parameter("bias", None)
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         init.kaiming_uniform_(self.weight, a=math.sqrt(5))
         if self.bias is not None:
             fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
             bound = 1 / math.sqrt(fan_in)
             init.uniform_(self.bias, -bound, bound)
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:
         return F.linear(input, self.weight, self.bias)
 
     def extra_repr(self) -> str:
-        return 'in_features={}, out_features={}, bias={}'.format(
-            self.in_features, self.out_features, self.bias is not None
-        )
+        return "in_features={}, out_features={}, bias={}".format(self.in_features, self.out_features, self.bias is not None)
 
 
 # This class exists solely for Transformer; it has an annotation stating
 # that bias is never None, which appeases TorchScript
 class _LinearWithBias(Linear):
     bias: torch.Tensor
 
@@ -425,32 +457,30 @@
         self.norm2 = LayerNorm(d_model)
         self.dropout1 = Dropout(dropout)
         self.dropout2 = Dropout(dropout)
 
         self.activation = _get_activation_fn(activation)
 
     def __setstate__(self, state):
-        if 'activation' not in state:
-            state['activation'] = F.relu
+        if "activation" not in state:
+            state["activation"] = F.relu
         super().__setstate__(state)
 
-    def forward(self, src: torch.Tensor, src_mask: Optional[torch.Tensor] = None,
-                src_key_padding_mask: Optional[torch.Tensor] = None) -> torch.Tensor:
+    def forward(self, src: torch.Tensor, src_mask: Optional[torch.Tensor] = None, src_key_padding_mask: Optional[torch.Tensor] = None) -> torch.Tensor:
         """Pass the input through the encoder layer.
 
         Args:
             src: the sequence to the encoder layer (required).
             src_mask: the mask for the src sequence (optional).
             src_key_padding_mask: the mask for the src keys per batch (optional).
 
         Shape:
             see the docs in Transformer class.
         """
-        src2 = self.self_attn(src, src, src, attn_mask=src_mask,
-                              key_padding_mask=src_key_padding_mask)[0]
+        src2 = self.self_attn(src, src, src, attn_mask=src_mask, key_padding_mask=src_key_padding_mask)[0]
         src = src + self.dropout1(src2)
         src = self.norm1(src)
         src2 = self.linear2(self.dropout(self.activation(self.linear1(src))))
         src = src + self.dropout2(src2)
         src = self.norm2(src)
         return src
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             inputs: out (embedding for TabTransformer), target (pretext task label)
             outputs: loss, % accuracy on pretext task
 
             given the embedding it passes it through a classifier which learns to
             predict the pretext label.
     """
 
-    def __init__(self, cat_feat_origin_cards, device, hidden_dim, replacement_noise='random', p_replace=0.3):
+    def __init__(self, cat_feat_origin_cards, device, hidden_dim, replacement_noise="random", p_replace=0.3):
         super().__init__()
         self.cat_feat_origin_cards = cat_feat_origin_cards
         self.device = device
         self.hidden_dim = hidden_dim
         self.loss_funct = nn.CrossEntropyLoss()
         self.p_replace = p_replace
         self.predicters = nn.ModuleList()
@@ -87,21 +87,21 @@
         return loss, correct
 
     def get(self, data, target):
         cat_feats = data
 
         orig_cat_feats = deepcopy(cat_feats.detach())
 
-        if self.replacement_noise == 'swap':
+        if self.replacement_noise == "swap":
             n_cat = cat_feats.shape[1]
             cols_to_shuffle = np.random.choice(n_cat, int(self.p_replace * n_cat), replace=False)
             for col in cols_to_shuffle:
                 cat_feats[:, col] = cat_feats[:, col][torch.randperm(cat_feats.shape[0])]
 
-        elif self.replacement_noise == 'random':
+        elif self.replacement_noise == "random":
             locs_to_replace = torch.empty_like(cat_feats, dtype=float).uniform_() < self.p_replace
             col_cardinalities = torch.LongTensor([i[1] for i in self.cat_feat_origin_cards]).to(cat_feats)
             col_cardinalities = col_cardinalities.unsqueeze(0).expand_as(cat_feats)
 
             unif = torch.rand(cat_feats.shape, device=col_cardinalities.device)
             random_feats = (unif * col_cardinalities).floor().to(torch.int64) + 1  # + 1 since 0 is the padding value
 
@@ -113,21 +113,19 @@
             extra_minus1 = cat_feats[extra_replace] - 1
             extra_zero_padd_idx = extra_minus1 == 0
             extra_minus1[extra_zero_padd_idx] = extra_plus1[extra_zero_padd_idx]
 
             cat_feats[extra_replace] = extra_minus1
             assert torch.all(~(cat_feats[extra_replace] == orig_cat_feats[extra_replace])).item() is True
 
-        elif self.replacement_noise == 'low_rank':
+        elif self.replacement_noise == "low_rank":
             assert self.p_replace + 0.2 <= 1, "p_replace too big, lower it!"
-            weights = torch.tensor([self.p_replace, 0.1, 0.9 - self.p_replace],
-                                   dtype=torch.float)  # 0=pad, 1=replace with random value, 2=dont change
+            weights = torch.tensor([self.p_replace, 0.1, 0.9 - self.p_replace], dtype=torch.float)  # 0=pad, 1=replace with random value, 2=dont change
 
-            locs_to_change = torch.multinomial(weights, np.prod(cat_feats.shape), replacement=True).view(
-                cat_feats.shape)
+            locs_to_change = torch.multinomial(weights, np.prod(cat_feats.shape), replacement=True).view(cat_feats.shape)
             col_cardinalities = torch.LongTensor([i[1] for i in self.cat_feat_origin_cards]).to(cat_feats)
             col_cardinalities = col_cardinalities.unsqueeze(0).expand_as(cat_feats)
 
             unif = torch.rand(cat_feats.shape, device=col_cardinalities.device)
             random_feats = (unif * col_cardinalities).floor().to(torch.int64) + 1  # + 1 since 0 is the padding value
 
             extra_replace = torch.mul((cat_feats == random_feats).to(int), (locs_to_change == 1).to(int)).to(torch.bool)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
         Parameters
         ----------
         num_class (int): Number of classes identified.
         cat_feat_origin_cards (list): List of categorical features
         """
         super().__init__()
         import torch.nn as nn
+
         from .tab_transformer import TabTransformer
+
         self.embed = TabTransformer(**params)
 
         relu = nn.ReLU()
         in_dim = 2 * feature_dim
         lin = nn.Linear(in_dim, in_dim, bias=True)
         lin_out = nn.Linear(in_dim, num_class, bias=True)
         self.fc = [nn.Sequential(*[relu, lin])] * (num_output_layers - 1) + [nn.Sequential(*[relu, lin_out])]
@@ -34,16 +36,15 @@
         out = features.mean(dim=1)
         for layer in range(len(self.fc)):
             out = self.fc[layer](out)
         return out, features
 
 
 class TabModelBase(nn.Module):
-    def __init__(self, n_cont_features, norm_class_name, cat_feat_origin_cards, max_emb_dim,
-                 p_dropout, one_hot_embeddings, drop_whole_embeddings):
+    def __init__(self, n_cont_features, norm_class_name, cat_feat_origin_cards, max_emb_dim, p_dropout, one_hot_embeddings, drop_whole_embeddings):
         super().__init__()
         """
         Base class for all TabTransformer models
         
         Parameters
         ----------
         max_emb_dim (int): Maximum allowable amount of embeddings.
@@ -63,19 +64,20 @@
         self.p_dropout = p_dropout
         self.drop_whole_embeddings = drop_whole_embeddings
         self.one_hot_embeddings = one_hot_embeddings
 
         self.cat_initializers = nn.ModuleDict()
 
         from .tab_transformer_encoder import EmbeddingInitializer
+
         if isinstance(self.cat_feat_origin_cards, list):
             for col_name, card in self.cat_feat_origin_cards:
-                self.cat_initializers[col_name] = EmbeddingInitializer(card, max_emb_dim, p_dropout,
-                                                                       drop_whole_embeddings=drop_whole_embeddings,
-                                                                       one_hot=one_hot_embeddings)
+                self.cat_initializers[col_name] = EmbeddingInitializer(
+                    card, max_emb_dim, p_dropout, drop_whole_embeddings=drop_whole_embeddings, one_hot=one_hot_embeddings
+                )
             self.init_feat_dim = sum(i.emb_dim for i in self.cat_initializers.values()) + self.n_cont_features
 
     def forward(self, input):
         raise NotImplementedError
 
     def get_norm(self, num_feats):
         return self.norm_class(num_feats)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,37 @@
 class TabTransformer(TabModelBase):
     """
     Transformer model for tabular data, can also be used for semi-supervised learning.
     This is the internal transformer model embedding that will have further fully connected layers (TabNet) to
     actually produce predictions.
     """
 
-    def __init__(self, n_cont_embeddings, n_layers, n_heads, hidden_dim, tab_readout, column_embedding, orig_emb_resid,
-                 fix_attention, n_shared_embs=8, shared_embedding_added=False, **kwargs):
-        super().__init__(n_cont_features=kwargs['n_cont_features'], norm_class_name=kwargs['norm_class_name'],
-                         cat_feat_origin_cards=kwargs['cat_feat_origin_cards'], max_emb_dim=kwargs['max_emb_dim'],
-                         p_dropout=kwargs['p_dropout'], one_hot_embeddings=kwargs['one_hot_embeddings'],
-                         drop_whole_embeddings=kwargs['drop_whole_embeddings'])
+    def __init__(
+        self,
+        n_cont_embeddings,
+        n_layers,
+        n_heads,
+        hidden_dim,
+        tab_readout,
+        column_embedding,
+        orig_emb_resid,
+        fix_attention,
+        n_shared_embs=8,
+        shared_embedding_added=False,
+        **kwargs,
+    ):
+        super().__init__(
+            n_cont_features=kwargs["n_cont_features"],
+            norm_class_name=kwargs["norm_class_name"],
+            cat_feat_origin_cards=kwargs["cat_feat_origin_cards"],
+            max_emb_dim=kwargs["max_emb_dim"],
+            p_dropout=kwargs["p_dropout"],
+            one_hot_embeddings=kwargs["one_hot_embeddings"],
+            drop_whole_embeddings=kwargs["drop_whole_embeddings"],
+        )
 
         from .modified_transformer import TransformerEncoderLayerModified
 
         self.n_cont_embeddings = n_cont_embeddings
         self.hidden_dim = hidden_dim
         self.readout = tab_readout
         self.orig_emb_resid = orig_emb_resid
@@ -37,14 +54,15 @@
             self.n_embeddings = len(self.cat_feat_origin_cards) + (n_cont_embeddings if self.n_cont_features else 0)
         else:
             self.n_embeddings = None
 
         self.cat_initializers = nn.ModuleDict()
 
         from .tab_transformer_encoder import EmbeddingInitializer
+
         for col_name, card in self.cat_feat_origin_cards:
             self.cat_initializers[col_name] = EmbeddingInitializer(
                 num_embeddings=card,
                 max_emb_dim=self.max_emb_dim,
                 p_dropout=self.p_dropout,
                 minimize_emb_dim=False,
                 drop_whole_embeddings=self.drop_whole_embeddings,
@@ -55,103 +73,107 @@
                 shared_embedding_added=shared_embedding_added,
             )
         if self.n_cont_features:
             self.cont_norm = self.get_norm(self.n_cont_features)
             self.cont_initializer = nn.Linear(self.n_cont_features, hidden_dim * n_cont_embeddings)
             self.cont_init_norm = self.get_norm(hidden_dim * n_cont_embeddings)
 
-        if self.readout == 'readout_emb':
-            self.readout_emb = nn.Parameter(
-                torch.zeros(1, hidden_dim).uniform_(-1, 1))  # We do the readout from a learned embedding
+        if self.readout == "readout_emb":
+            self.readout_emb = nn.Parameter(torch.zeros(1, hidden_dim).uniform_(-1, 1))  # We do the readout from a learned embedding
             self.n_embeddings += 1
 
         if fix_attention is True:
             self.n_cat_embeddings = len(self.cat_feat_origin_cards)
-            self.tfmr_layers = nn.ModuleList([TransformerEncoderLayerModified(d_model=hidden_dim,
-                                                                               n_cat_embeddings=self.n_cat_embeddings,
-                                                                               nhead=n_heads,
-                                                                               dim_feedforward=4 * hidden_dim,
-                                                                               dropout=self.p_dropout,
-                                                                               activation='gelu') for _ in
-                                              range(n_layers)])
+            self.tfmr_layers = nn.ModuleList(
+                [
+                    TransformerEncoderLayerModified(
+                        d_model=hidden_dim,
+                        n_cat_embeddings=self.n_cat_embeddings,
+                        nhead=n_heads,
+                        dim_feedforward=4 * hidden_dim,
+                        dropout=self.p_dropout,
+                        activation="gelu",
+                    )
+                    for _ in range(n_layers)
+                ]
+            )
         else:
-            self.tfmr_layers = nn.ModuleList([nn.TransformerEncoderLayer(d_model=hidden_dim,
-                                                                         nhead=n_heads,
-                                                                         dim_feedforward=4 * hidden_dim,
-                                                                         dropout=self.p_dropout,
-                                                                         activation='gelu') for _ in
-                                              range(n_layers)])
+            self.tfmr_layers = nn.ModuleList(
+                [
+                    nn.TransformerEncoderLayer(d_model=hidden_dim, nhead=n_heads, dim_feedforward=4 * hidden_dim, dropout=self.p_dropout, activation="gelu")
+                    for _ in range(n_layers)
+                ]
+            )
 
     def init_input(self, input):
         feats = [init(input[:, i]) for i, init in enumerate(self.cat_initializers.values())]
 
-        if self.readout == 'readout_emb':
+        if self.readout == "readout_emb":
             readout_emb = self.readout_emb.expand_as(feats[0])
-            feat_embs = torch.stack([readout_emb] + feats,
-                                    dim=0)  # (n_feat_embeddings + 1) x batch x hidden_dim
+            feat_embs = torch.stack([readout_emb] + feats, dim=0)  # (n_feat_embeddings + 1) x batch x hidden_dim
         else:
             feat_embs = torch.stack(feats, dim=0)  # n_feat_embeddings x batch x hidden_dim
         return feat_embs
 
     def run_tfmr(self, feat_embs):
         orig_feat_embs = feat_embs
         all_feat_embs = [feat_embs]
         for layer in self.tfmr_layers:
             feat_embs = layer(feat_embs)
             all_feat_embs.append(feat_embs)
             if self.orig_emb_resid:
                 feat_embs = feat_embs + orig_feat_embs
 
-        if self.readout == 'readout_emb':
+        if self.readout == "readout_emb":
             out = self.fc_out(feat_embs[0])
-        elif self.readout == 'mean':
+        elif self.readout == "mean":
             out = torch.mean(feat_embs, dim=0)
             out = self.fc_out(out)
-        elif self.readout == 'concat_pool':
+        elif self.readout == "concat_pool":
             all_feat_embs = torch.cat(all_feat_embs, dim=0)
 
             max = all_feat_embs.max(dim=0).values
             mean = all_feat_embs.mean(dim=0)
             last_layer = feat_embs.transpose(0, 1).reshape(feat_embs.shape[1], -1)
             out = torch.cat((last_layer, max, mean), dim=1)
             out = self.fc_out(out)
-        elif self.readout == 'concat_pool_all':
+        elif self.readout == "concat_pool_all":
             feat_embs_all_layers = []
             for each_feat_embs in [all_feat_embs[0], all_feat_embs[-1]]:
                 feat_embs_all_layers.append(each_feat_embs.transpose(0, 1).reshape(each_feat_embs.shape[1], -1))
 
             all_feat_embs = torch.cat(all_feat_embs, dim=0)
             max = all_feat_embs.max(dim=0).values
             mean = all_feat_embs.mean(dim=0)
 
             feat_embs_all_layers.append(max)
             feat_embs_all_layers.append(mean)
             out = torch.cat(feat_embs_all_layers, dim=1)
             out = self.fc_out(out)
-        elif self.readout == 'concat_pool_add':
+        elif self.readout == "concat_pool_add":
             orig_feat_embs_cp = copy.deepcopy(orig_feat_embs.detach())
             # ce_dim = orig_feat_embs_cp.shape[-1]//8
             # orig_feat_embs_cp[:, :, ce_dim:] = 0
 
             last_layer = feat_embs.transpose(0, 1).reshape(feat_embs.shape[1], -1)
             last_layer += orig_feat_embs_cp.transpose(0, 1).reshape(orig_feat_embs_cp.shape[1], -1)
 
             all_feat_embs = torch.cat(all_feat_embs, dim=0)
             max = all_feat_embs.max(dim=0).values
             mean = all_feat_embs.mean(dim=0)
 
             out = torch.cat([last_layer, max, mean], dim=1)
 
-        elif self.readout == 'all_feat_embs':
+        elif self.readout == "all_feat_embs":
             out = feat_embs
 
-        elif self.readout == 'mean_feat_embs':
+        elif self.readout == "mean_feat_embs":
             out = feat_embs.mean(dim=0)
 
-        elif self.readout == 'none':
+        elif self.readout == "none":
             out = feat_embs.transpose(1, 0)
 
         return out
 
     def forward(self, input):
         """
         Returns logits for output classes
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Credits for code in this script to Milan Cvitkovic,
 # Xin Huang, Ashish Khetan and Zohar Karnin
 
 import calendar
 import datetime
 import re
 from collections import Counter
-from datetime import datetime, date
+from datetime import date, datetime
 from functools import partial
-from typing import List, Union, Iterable
+from typing import Iterable, List, Union
 
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn as nn
 from pandas import DataFrame
 from sklearn.feature_extraction.text import TfidfVectorizer
-from sklearn.preprocessing import RobustScaler, PowerTransformer, QuantileTransformer, KBinsDiscretizer
+from sklearn.preprocessing import KBinsDiscretizer, PowerTransformer, QuantileTransformer, RobustScaler
 
 
 class WontEncodeError(Exception):
     pass
 
 
 class EncBase:
@@ -29,30 +29,30 @@
     @property
     def cat_dim(self):
         return len(self.cat_cards)
 
     def clean_data(self, data, dtype=None) -> list:
         if isinstance(data, pd.Series):
             data = data.replace({np.nan: None}).to_list()
-            if dtype == 'float':
+            if dtype == "float":
                 unclean_data = data
                 data = []
                 for i in unclean_data:
                     try:
                         data.append(float(i))
                     except (ValueError, TypeError):
                         data.append(None)
             return data
 
     def fit(self, data: pd.Series, dtype=None):
         """
         If dtype == 'float', clean_data will cast the contents of data to floats
         """
         if len(pd.unique(data)) == 1:
-            raise WontEncodeError('Column contains only one value')
+            raise WontEncodeError("Column contains only one value")
         data = self.clean_data(data, dtype)
         return data
 
     def enc_cat(self, data: Iterable):
         raise NotImplementedError
 
     def enc_cont(self, data: Iterable):
@@ -107,32 +107,31 @@
 
 
 class ScalarQuantileOrdinalEnc(EncBase):
     def __init__(self, n_bins_=None, bin_edges_=None):
         if n_bins_ is not None and bin_edges_ is not None:
             self.disc = self.get_new_base_enc()
             self.disc.n_bins_ = np.array([n_bins_])
-            self.disc.bin_edges_ = np.array([np.array(bin_edges_), np.array(bin_edges_[:-1])])[
-                                   :1]  # Dumb hack, but it's what sklearn needs
+            self.disc.bin_edges_ = np.array([np.array(bin_edges_), np.array(bin_edges_[:-1])])[:1]  # Dumb hack, but it's what sklearn needs
             self.cat_cards = [n_bins_ + 1]
 
     def fit(self, data):
 
-        data = super().fit(data, dtype='float')
+        data = super().fit(data, dtype="float")
         fit_data = [i for i in data if i is not None]
         fit_data = np.array(fit_data).reshape(-1, 1)
         self.disc = self.get_new_base_enc()
         self.disc.fit(fit_data)
         self.cat_cards = [self.disc.n_bins_.item() + 1]
 
     def enc_cat(self, data):
         """
         Missing values are returned as category 1.  0 is reserved for padding.
         """
-        data = self.clean_data(data, dtype='float')
+        data = self.clean_data(data, dtype="float")
         data = np.array(data).reshape(-1, 1)
         if None in data:
             idxs = np.full(len(data), -1, dtype=int)
             null_idxs = np.where(data == None)[0]
             val_idxs = np.where(data != None)[0]
             if len(val_idxs) > 0:
                 vals = self.disc.transform(data[val_idxs]).reshape(-1)
@@ -143,17 +142,15 @@
         return torch.LongTensor(idxs).unsqueeze(1)
 
     def enc_cont(self, data):
         pass
 
     @staticmethod
     def get_new_base_enc():
-        return KBinsDiscretizer(n_bins=8,
-                                encode='ordinal',
-                                strategy='quantile')
+        return KBinsDiscretizer(n_bins=8, encode="ordinal", strategy="quantile")
 
     def get_base_enc_params(self):
         return self.disc.n_bins_, self.disc.bin_edges_
 
 
 class ScalarRescaleEnc(EncBase):
     cont_dim = 2
@@ -162,15 +159,15 @@
     def enc_cat(self, data):
         pass
 
     def enc_cont(self, scalars):
         """
         Returns len(scalars) x 2 tensor, where the second column is a one-hot flag for missing data values
         """
-        scalars = self.clean_data(scalars, dtype='float')
+        scalars = self.clean_data(scalars, dtype="float")
         null_flag = np.full(len(scalars), np.nan, dtype=np.float32)
         vals = np.full(len(scalars), np.nan, dtype=np.float32)
         null_idxs = np.where(np.array(scalars) == None)[0]
         val_idxs = np.where(np.array(scalars) != None)[0]
 
         # One-hot flag for missing values
         null_flag[null_idxs] = 1
@@ -199,15 +196,15 @@
     def __init__(self, center_=None, scale_=None):
         if center_ is not None and scale_ is not None:
             self.scaler = self.get_new_base_enc()
             self.scaler.center_ = center_
             self.scaler.scale_ = scale_
 
     def fit(self, data: pd.Series):
-        data = super().fit(data, dtype='float')
+        data = super().fit(data, dtype="float")
         data = np.array(data).reshape(-1, 1)
         self.scaler = self.get_new_base_enc()
         self.scaler.fit(data)
         if any(sum(np.isnan(p) for p in self.get_base_enc_params())):
             self.scaler.center_ = 0
             self.scaler.scale_ = 1
 
@@ -219,46 +216,45 @@
         return self.scaler.center_, self.scaler.scale_
 
 
 class ScalarPowerTransformerEnc(ScalarRescaleEnc):
     def __init__(self, lambdas_=None, scale_=None, mean_=None, var_=None, n_samples_seen_=None):
         if all(a is not None for a in [lambdas_, scale_, mean_, var_, n_samples_seen_]):
             self.scaler = self.get_new_base_enc()
-            self.scaler.fit(
-                [[0.0]])  # This is just to make the PowerTransformer initialize before we overwrite its params
+            self.scaler.fit([[0.0]])  # This is just to make the PowerTransformer initialize before we overwrite its params
             self.scaler.lambdas_ = np.array([lambdas_])
             self.scaler._scaler.scale_ = np.array([scale_])
             self.scaler._scaler.mean_ = np.array([mean_])
             self.scaler._scaler.var_ = np.array([var_])
             self.scaler._scaler.n_samples_seen_ = n_samples_seen_
 
     def fit(self, data):
-        data = super().fit(data, dtype='float')
+        data = super().fit(data, dtype="float")
         data = np.array(data).reshape(-1, 1)
         self.scaler = self.get_new_base_enc()
         self.scaler.fit(data)
 
     @staticmethod
     def get_new_base_enc():
-        return PowerTransformer(method='yeo-johnson', standardize=True, copy=True)
+        return PowerTransformer(method="yeo-johnson", standardize=True, copy=True)
 
     def get_base_enc_params(self):
         return self.scaler.lambdas_, self.scaler._scaler.scale_, self.scaler._scaler.mean_, self.scaler._scaler.var_, self.scaler._scaler.n_samples_seen_
 
 
 class ScalarQuantileTransformerEnc(ScalarRescaleEnc):
     def __init__(self, n_quantiles_=None, quantiles_=None, references_=None):
         if all(a is not None for a in [n_quantiles_, quantiles_, references_]):
             self.scaler = self.get_new_base_enc()
             self.scaler.n_quantiles_ = n_quantiles_
             self.scaler.quantiles_ = np.array(quantiles_).reshape(-1, 1)
             self.scaler.references_ = np.array(references_)
 
     def fit(self, data):
-        data = super().fit(data, dtype='float')
+        data = super().fit(data, dtype="float")
         data = np.array(data).reshape(-1, 1)
         self.scaler = self.get_new_base_enc()
         self.scaler.fit(data)
 
     @staticmethod
     def get_new_base_enc():
         return QuantileTransformer()
@@ -266,90 +262,90 @@
     def get_base_enc_params(self):
         return self.scaler.n_quantiles_, self.scaler.quantiles_, self.scaler.references_
 
 
 class DatetimeScalarEnc(EncBase):
     # int for type refers to the cardinality of the one-hot
     cols_types = [
-        ('Year', 'float'),
-        ('Month', 12),
-        ('Week', 53),
-        ('Day', 31),
-        ('Dayofweek', 7),
-        ('Dayofyear', 'float'),
-        ('Is_month_end', 2),
-        ('Is_month_start', 2),
-        ('Is_quarter_end', 2),
-        ('Is_quarter_start', 2),
-        ('Is_year_end', 2),
-        ('Is_year_start', 2),
-        ('weekday_cos', 'float'),
-        ('weekday_sin', 'float'),
-        ('day_month_cos', 'float'),
-        ('day_month_sin', 'float'),
-        ('month_year_cos', 'float'),
-        ('month_year_sin', 'float'),
-        ('day_year_cos', 'float'),
-        ('day_year_sin', 'float'),
+        ("Year", "float"),
+        ("Month", 12),
+        ("Week", 53),
+        ("Day", 31),
+        ("Dayofweek", 7),
+        ("Dayofyear", "float"),
+        ("Is_month_end", 2),
+        ("Is_month_start", 2),
+        ("Is_quarter_end", 2),
+        ("Is_quarter_start", 2),
+        ("Is_year_end", 2),
+        ("Is_year_start", 2),
+        ("weekday_cos", "float"),
+        ("weekday_sin", "float"),
+        ("day_month_cos", "float"),
+        ("day_month_sin", "float"),
+        ("month_year_cos", "float"),
+        ("month_year_sin", "float"),
+        ("day_year_cos", "float"),
+        ("day_year_sin", "float"),
     ]
     cont_dim = sum([n if type(n) == int else 1 for _, n in cols_types])
 
     def enc_cat(self, data):
         pass
 
     def enc_cont(self, datetimes):
         datetimes = self.clean_data(datetimes)
-        df = pd.DataFrame({'dt': datetimes})
-        add_datepart(df, field_name='dt', prefix='', drop=False)
-        df = add_cyclic_datepart(df, field_name='dt', prefix='', drop=False)
+        df = pd.DataFrame({"dt": datetimes})
+        add_datepart(df, field_name="dt", prefix="", drop=False)
+        df = add_cyclic_datepart(df, field_name="dt", prefix="", drop=False)
         enc = torch.empty(len(datetimes), self.cont_dim)
         feats_done = 0
         for c, t in self.cols_types:
-            feats_doing = (1 if t == 'float' else t)
-            if t == 'float':
+            feats_doing = 1 if t == "float" else t
+            if t == "float":
                 feats = torch.FloatTensor(df[c].to_numpy()).view(-1, 1)
-                if c == 'Year':
+                if c == "Year":
                     feats = (feats - 2000) / 10
-                elif c == 'Dayofyear':
+                elif c == "Dayofyear":
                     feats /= 365
             else:
-                feats = torch.LongTensor(df[c].to_numpy().astype('int32')).view(-1, 1)
-                if c in ['Month', 'Week', 'Day']:
+                feats = torch.LongTensor(df[c].to_numpy().astype("int32")).view(-1, 1)
+                if c in ["Month", "Week", "Day"]:
                     feats -= 1
                 feats = one_hot(feats, t)
-            enc[:, feats_done: feats_done + feats_doing] = feats
+            enc[:, feats_done : feats_done + feats_doing] = feats
             feats_done += feats_doing
         return enc
 
 
 class DatetimeOrdinalEnc(EncBase):
     # These are all 1 larger than you'd expect to support missing values
     cols_types = [
-        ('Month', 13),
-        ('Week', 54),
-        ('Day', 32),
-        ('Dayofweek', 8),
-        ('Is_month_end', 3),
-        ('Is_month_start', 3),
-        ('Is_quarter_end', 3),
-        ('Is_quarter_start', 3),
-        ('Is_year_end', 3),
-        ('Is_year_start', 3)
+        ("Month", 13),
+        ("Week", 54),
+        ("Day", 32),
+        ("Dayofweek", 8),
+        ("Is_month_end", 3),
+        ("Is_month_start", 3),
+        ("Is_quarter_end", 3),
+        ("Is_quarter_start", 3),
+        ("Is_year_end", 3),
+        ("Is_year_start", 3),
     ]
     cat_cards = [n for _, n in cols_types]
 
     def enc_cat(self, datetimes):
         # todo: add support for missing values, which should get encoded as 1.
         datetimes = self.clean_data(datetimes)
-        df = pd.DataFrame({'dt': datetimes})
-        add_datepart(df, field_name='dt', prefix='', drop=False)
+        df = pd.DataFrame({"dt": datetimes})
+        add_datepart(df, field_name="dt", prefix="", drop=False)
         feats = []
         for c, t in self.cols_types:
-            f = torch.LongTensor(df[c].to_numpy().astype('int32'))
-            if c in ['Month', 'Week', 'Day']:
+            f = torch.LongTensor(df[c].to_numpy().astype("int32"))
+            if c in ["Month", "Week", "Day"]:
                 f -= 1
             feats.append(f)
         feats = torch.stack(feats, dim=1) + 2  # + 2 for missing and padding
         return feats
 
     def enc_cont(self, data):
         pass
@@ -362,15 +358,15 @@
         pass
 
     def enc_cont(self, latlongs):
         latlongs = self.clean_data(latlongs)
         if isinstance(latlongs[0], str):
             fixed = []
             for ll in latlongs:
-                lat, long = ll.strip('()').split(',')
+                lat, long = ll.strip("()").split(",")
                 lat, long = float(lat), float(long)
                 fixed.append((lat, long))
             latlongs = fixed
         latlongs = np.array(latlongs)
         lats, longs = latlongs[:, 0:1], latlongs[:, 1:2]
         x = np.cos(lats) * np.cos(longs)
         y = np.cos(lats) * np.sin(longs)
@@ -413,17 +409,15 @@
         return torch.LongTensor(feats)
 
     def enc_cont(self, data):
         pass
 
     @staticmethod
     def get_new_base_enc():
-        return [KBinsDiscretizer(n_bins=8,
-                                 encode='ordinal',
-                                 strategy='quantile') for _ in range(LatLongScalarEnc.cont_dim)]
+        return [KBinsDiscretizer(n_bins=8, encode="ordinal", strategy="quantile") for _ in range(LatLongScalarEnc.cont_dim)]
 
     def get_base_enc_params(self):
         return [(disc.n_bins_, disc.bin_edges_) for disc in self.discs]
 
 
 class TfidfEnc(EncBase):
     def __init__(self, vocabulary_=None, idf_=None):
@@ -434,85 +428,91 @@
             self.cont_dim = len(vocabulary_)
 
     def enc_cat(self, data):
         pass
 
     def enc_cont(self, data):
         data = self.clean_data(data)
-        text_strings = np.array([d if d is not None else '' for d in data])
+        text_strings = np.array([d if d is not None else "" for d in data])
         encoded = self.tfidf.transform(text_strings)
         encoded = torch.Tensor(encoded.todense())
         # todo: wait until pytorch lets you use multiproc with sparse tensors
         # encoded = encoded.tocoo()
         # i = torch.LongTensor(np.vstack((encoded.row, encoded.col)))
         # v = torch.FloatTensor(encoded.data)
         # encoded = torch.sparse.FloatTensor(i, v, torch.Size(encoded.shape))
         return encoded
 
     def fit(self, data):
         data = super().fit(data)
-        data = [d if d is not None else '' for d in data]
+        data = [d if d is not None else "" for d in data]
         self.tfidf = self.get_new_base_enc().fit(data)
         self.cont_dim = len(self.tfidf.vocabulary_)
 
     @staticmethod
     def get_new_base_enc():
-        return TfidfVectorizer(input='content',
-                               decode_error='replace',
-                               strip_accents='ascii',
-                               lowercase=True,
-                               analyzer='word',
-                               min_df=5 / 100000)
+        return TfidfVectorizer(input="content", decode_error="replace", strip_accents="ascii", lowercase=True, analyzer="word", min_df=5 / 100000)
 
     def get_base_enc_params(self):
         return self.tfidf.vocabulary_, self.tfidf.idf_
 
 
 class TextSummaryScalarEnc(EncBase):
     """
     Returns the featuretools summary statistics about the text (num words and num_chars), but normalized
     """
+
     cont_dim = 2
 
     def __init__(self, center_=None, scale_=None):
         if center_ is not None and scale_ is not None:
             self.scaler = RobustScaler()
             self.scaler.center_ = center_
             self.scaler.scale_ = scale_
 
     def enc_cat(self, data):
         pass
 
     def enc_cont(self, data):
         data = self.clean_data(data)
-        text_strings = [s if s is not None else '' for s in data]
+        text_strings = [s if s is not None else "" for s in data]
         encoded = self.get_encoded(text_strings)
         encoded = self.scaler.transform(encoded)
         encoded = torch.Tensor(encoded)
         return encoded
 
     def get_encoded(self, text_strings):
-        text_strings = [ts if ts is not None else '' for ts in text_strings]
+        text_strings = [ts if ts is not None else "" for ts in text_strings]
         num_chars = [len(ts) for ts in text_strings]
         num_words = [len(ts.split()) for ts in text_strings]
         return np.array((num_chars, num_words)).T
 
     def fit(self, data):
         data = super().fit(data)
         encoded = self.get_encoded(data)
         self.scaler = RobustScaler().fit(encoded)
 
     def get_base_enc_params(self):
         return self.scaler.center_, self.scaler.scale_
 
 
 class EmbeddingInitializer(nn.Module):
-    def __init__(self, num_embeddings, max_emb_dim, p_dropout, minimize_emb_dim=True, drop_whole_embeddings=False,
-                 one_hot=False, out_dim=None, shared_embedding=False, n_shared_embs=8,
-                 shared_embedding_added=False):
+    def __init__(
+        self,
+        num_embeddings,
+        max_emb_dim,
+        p_dropout,
+        minimize_emb_dim=True,
+        drop_whole_embeddings=False,
+        one_hot=False,
+        out_dim=None,
+        shared_embedding=False,
+        n_shared_embs=8,
+        shared_embedding_added=False,
+    ):
         """
         :param minimize_emb_dim:
             Whether to set embedding_dim = max_emb_dim or to make embedding_dim smaller is num_embeddings is small
         :param drop_whole_embeddings:
             If True, dropout pretends the embedding was a missing value. If false, dropout sets embed features to 0
         :param one_hot:
             If True, one-hot encode variables whose cardinality is < max_emb_dim. Also, set reqiures_grad = False
@@ -535,48 +535,45 @@
         self.shared_embedding_added = shared_embedding_added
         if minimize_emb_dim or one_hot:
             self.emb_dim = min(max_emb_dim, num_embeddings)  # Don't use a crazy huge embedding if not needed
         else:
             self.emb_dim = max_emb_dim
         self.reshape_out = nn.Identity()
         if out_dim is not None:
-            assert self.emb_dim <= out_dim, 'Makes no sense: just set max_emb_dim = out_dim and out_dim = None'
+            assert self.emb_dim <= out_dim, "Makes no sense: just set max_emb_dim = out_dim and out_dim = None"
             if num_embeddings > self.emb_dim:
                 self.reshape_out = nn.Linear(self.emb_dim, out_dim, bias=True)
             else:
                 self.emb_dim = out_dim
         # Note: if you change the name of self.embed, or initialize an embedding elsewhere in a model,
         # the function get_optim will not work properly
-        self.embed = nn.Embedding(num_embeddings=num_embeddings + 1,
-                                  embedding_dim=self.emb_dim,
-                                  padding_idx=0)
+        self.embed = nn.Embedding(num_embeddings=num_embeddings + 1, embedding_dim=self.emb_dim, padding_idx=0)
         self.embed.weight.data.clamp_(-2, 2)  # Use truncated normal init
         if one_hot:
             self.embed.weight.requires_grad = False
             if num_embeddings <= max_emb_dim:
                 self.embed.weight.data[1:, :] = torch.eye(self.emb_dim)
         if shared_embedding:
             assert not one_hot
-            ce_dim = self.emb_dim if shared_embedding_added else (
-                                                                     out_dim if out_dim else self.emb_dim) // n_shared_embs  # used to be //8
+            ce_dim = self.emb_dim if shared_embedding_added else (out_dim if out_dim else self.emb_dim) // n_shared_embs  # used to be //8
             self.shared_emb = nn.Parameter(torch.empty(1, ce_dim).uniform_(-1, 1))
         self.do = nn.Dropout(p=p_dropout)
 
     def forward(self, input):
         if self.drop_whole_embeddings and self.training:
             mask = torch.zeros_like(input).bernoulli_(1 - self.p_dropout)
             input = input * mask
         out = self.embed(input)
         if not self.drop_whole_embeddings:
             out = self.do(out)
         out = self.reshape_out(out)
         if self.shared_embedding:
             shared_emb = self.shared_emb.expand(out.shape[0], -1)
             if not self.shared_embedding_added:
-                out[:, :shared_emb.shape[1]] = shared_emb
+                out[:, : shared_emb.shape[1]] = shared_emb
             else:
                 out += shared_emb
         return out
 
 
 def one_hot(x, card):
     assert isinstance(x, torch.LongTensor)
@@ -600,29 +597,46 @@
         df[date_field] = pd.to_datetime(df[date_field], infer_datetime_format=True)
 
 
 def add_datepart(df: DataFrame, field_name: str, prefix: str = None, drop: bool = True, time: bool = False):
     "Helper function that adds columns relevant to a date in the column `field_name` of `df`."
     make_date(df, field_name)
     field = df[field_name]
-    prefix = re.sub('[Dd]ate$', '', field_name) if prefix is None else prefix
-    attr = ['Year', 'Month', 'Week', 'Day', 'Dayofweek', 'Dayofyear', 'Is_month_end', 'Is_month_start',
-            'Is_quarter_end', 'Is_quarter_start', 'Is_year_end', 'Is_year_start']
-    if time: attr = attr + ['Hour', 'Minute', 'Second']
-    for n in attr: df[prefix + n] = getattr(field.dt, n.lower())
-    if drop: df.drop(field_name, axis=1, inplace=True)
+    prefix = re.sub("[Dd]ate$", "", field_name) if prefix is None else prefix
+    attr = [
+        "Year",
+        "Month",
+        "Week",
+        "Day",
+        "Dayofweek",
+        "Dayofyear",
+        "Is_month_end",
+        "Is_month_start",
+        "Is_quarter_end",
+        "Is_quarter_start",
+        "Is_year_end",
+        "Is_year_start",
+    ]
+    if time:
+        attr = attr + ["Hour", "Minute", "Second"]
+    for n in attr:
+        df[prefix + n] = getattr(field.dt, n.lower())
+    if drop:
+        df.drop(field_name, axis=1, inplace=True)
     return df
 
 
 def cyclic_dt_feat_names(time: bool = True, add_linear: bool = False) -> List[str]:
     "Return feature names of date/time cycles as produced by `cyclic_dt_features`."
-    fs = ['cos', 'sin']
-    attr = [f'{r}_{f}' for r in 'weekday day_month month_year day_year'.split() for f in fs]
-    if time: attr += [f'{r}_{f}' for r in 'hour clock min sec'.split() for f in fs]
-    if add_linear: attr.append('year_lin')
+    fs = ["cos", "sin"]
+    attr = [f"{r}_{f}" for r in "weekday day_month month_year day_year".split() for f in fs]
+    if time:
+        attr += [f"{r}_{f}" for r in "hour clock min sec".split() for f in fs]
+    if add_linear:
+        attr.append("year_lin")
     return attr
 
 
 def cyclic_dt_features(d: Union[date, datetime], time: bool = True, add_linear: bool = False) -> List[float]:
     "Calculate the cos and sin of date/time cycles."
     tt, fs = d.timetuple(), [np.cos, np.sin]
     day_year, days_month = tt.tm_yday, calendar.monthrange(d.year, d.month)[1]
@@ -637,19 +651,19 @@
             feats.append(d.year + rs[-1])
         else:
             secs_in_year = (datetime(d.year + 1, 1, 1) - datetime(d.year, 1, 1)).total_seconds()
             feats.append(d.year + ((d - datetime(d.year, 1, 1)).total_seconds() / secs_in_year))
     return feats
 
 
-def add_cyclic_datepart(df: DataFrame, field_name: str, prefix: str = None, drop: bool = True, time: bool = False,
-                        add_linear: bool = False):
+def add_cyclic_datepart(df: DataFrame, field_name: str, prefix: str = None, drop: bool = True, time: bool = False, add_linear: bool = False):
     "Helper function that adds trigonometric date/time features to a date in the column `field_name` of `df`."
     make_date(df, field_name)
     field = df[field_name]
-    prefix = re.sub('[Dd]ate$', '', field_name) if prefix is None else prefix
+    prefix = re.sub("[Dd]ate$", "", field_name) if prefix is None else prefix
     series = field.apply(partial(cyclic_dt_features, time=time, add_linear=add_linear))
     columns = [prefix + c for c in cyclic_dt_feat_names(time, add_linear)]
     df_feats = pd.DataFrame([item for item in series], columns=columns)
     df = pd.concat([df, df_feats], axis=1)
-    if drop: df.drop(field_name, axis=1, inplace=True)
+    if drop:
+        df.drop(field_name, axis=1, inplace=True)
     return df
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,47 @@
 import os
 import time
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
-from autogluon.common.features.types import R_OBJECT, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY
+from autogluon.common.features.types import R_OBJECT, S_TEXT_AS_CATEGORY, S_TEXT_NGRAM
 from autogluon.common.utils.try_import import try_import_torch
-from autogluon.core.constants import BINARY, REGRESSION, MULTICLASS
-from autogluon.core.utils.loaders import load_pkl
+from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION
 from autogluon.core.models.abstract.abstract_nn_model import AbstractNeuralNetworkModel
+from autogluon.core.utils.loaders import load_pkl
 
 from .hyperparameters.parameters import get_default_param
 from .hyperparameters.searchspaces import get_default_searchspace
 
 logger = logging.getLogger(__name__)
 
 """
 TODO: Fix Mac OS X warning spam.
 The error message is:
 Cannot set number of intraop threads after parallel work has started or after set_num_threads call when using native parallel backend (function set_num_threads)
 This has been investigated to be a harmless warning for training and running inference on TabTransformer.
 This warning can occur with a very specific environment: torch 1.7, Mac OS X, Python 3.6/3.7, when using torch DataLoader.
 https://github.com/pytorch/pytorch/issues/46409
 """
+
+
 class TabTransformerModel(AbstractNeuralNetworkModel):
     """
     Main TabTransformer model that inherits from AbstractModel.
 
     This model includes the full torch pipeline (TabNet) and the internal Transformer embeddings (TabTransformer).
     This file serves as the connection of all these internal models and architectures to AutoGluon.
 
     TabTransformer uses modifications to the typical Transformer architecture and the pretraining in BERT
     and applies them to the use case of tabular data. Specifically, this makes TabTransformer suitable for unsupervised
     training of Tabular data with a subsequent fine-tuning step on labeled data.
     """
+
     params_file_name = "tab_trans_params.pth"
 
     def __init__(self, **kwargs):
         try_import_torch()
         super().__init__(**kwargs)
         self._verbosity = None
         self._temp_file_name = "tab_trans_temp.pth"
@@ -58,17 +61,17 @@
             ignored_type_group_special=[S_TEXT_NGRAM, S_TEXT_AS_CATEGORY],
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     def _get_model(self):
         from .tab_model_base import TabNet
+
         # If we have already initialized the model, we don't need to do it again.
-        model = TabNet(self.params['n_classes'], self.params['feature_dim'],
-                       self.params['num_output_layers'], self.device, self.params)
+        model = TabNet(self.params["n_classes"], self.params["feature_dim"], self.params["num_output_layers"], self.device, self.params)
         if self.device.type == "cuda":
             model = model.cuda()
 
         return model
 
     # NOTE: Making an assumption that X_unlabeled will not have a different schema. Otherwise, we would need two
     # period_columns_mapping fields. One for X/X_val, another for X_unlabeled, which may have different columns.
@@ -84,28 +87,28 @@
             if new_col_name in rename_columns:
                 for i in range(1, 100):
                     append_col_name = new_col_name + "_" + str(i)
                     if append_col_name not in rename_columns:
                         new_col_name = append_col_name
                         break
                 else:
-                    raise RuntimeError("Tried 100 column renames to eliminate duplicates.\n"
-                                       "Please check similar columns with . or _ in them.")
+                    raise RuntimeError("Tried 100 column renames to eliminate duplicates.\n" "Please check similar columns with . or _ in them.")
 
             # Mapping for every column
             rename_columns[col] = new_col_name
 
         return rename_columns
 
     def _preprocess(self, X, **kwargs):
         from .utils import TabTransformerDataset
+
         X = super()._preprocess(X=X, **kwargs)
 
         X = X.rename(columns=self._period_columns_mapping)
-        encoders = self.params['encoders']
+        encoders = self.params["encoders"]
         data = TabTransformerDataset(X, encoders=encoders, problem_type=self.problem_type, col_info=self._types_of_features)
         data.encode(self.fe)
 
         return data
 
     def _preprocess_train(self, X, X_val=None, X_unlabeled=None, fe=None):
         """
@@ -116,31 +119,30 @@
 
         X = self._preprocess_nonadaptive(X)
         if X_val is not None:
             X_val = self._preprocess_nonadaptive(X_val)
         if X_unlabeled is not None:
             X_unlabeled = self._preprocess_nonadaptive(X_unlabeled)
 
-
         self._period_columns_mapping = self._get_no_period_columns(X.columns)
         X = X.rename(columns=self._period_columns_mapping)
 
         if X_val is not None:
             X_val = X_val.rename(columns=self._period_columns_mapping)
         if X_unlabeled is not None:
             X_unlabeled = X_unlabeled.rename(columns=self._period_columns_mapping)
 
         self._types_of_features, _ = self._get_types_of_features(X, needs_extra_types=False)
 
         # Also need to rename the feature names in the types_of_features dictionary.
         for feature_dict in self._types_of_features:
             # Need to check that the value is in the mapping. Otherwise, we could be updating columns that have been dropped.
-            feature_dict.update(('name', self._period_columns_mapping[v]) for k, v in feature_dict.items() if k == 'name' and v in self._period_columns_mapping)
+            feature_dict.update(("name", self._period_columns_mapping[v]) for k, v in feature_dict.items() if k == "name" and v in self._period_columns_mapping)
 
-        encoders = self.params['encoders']
+        encoders = self.params["encoders"]
         data = TabTransformerDataset(X, encoders=encoders, problem_type=self.problem_type, col_info=self._types_of_features)
         self.fe = fe
         if self.fe is not None:
             if X_unlabeled is None:
                 unlab_data = None
             elif X_unlabeled is not None:
                 unlab_data = TabTransformerDataset(X_unlabeled, encoders=encoders, problem_type=self.problem_type, col_info=self._types_of_features)
@@ -163,39 +165,42 @@
             val_data = None
 
         if unlab_data is not None:
             unlab_data.encode(self.fe)
 
         return data, val_data, unlab_data
 
-    def _epoch(self, net, loader_train, loader_val, y_val, optimizers, loss_criterion, pretext, state, scheduler, epoch,
-               epochs, databar_disable, reporter, params):
+    def _epoch(
+        self, net, loader_train, loader_val, y_val, optimizers, loss_criterion, pretext, state, scheduler, epoch, epochs, databar_disable, reporter, params
+    ):
         """
         Helper function to run one epoch of training, essentially the "inner loop" of training.
         """
         import torch
+
         from .utils import augmentation
-        is_train = (optimizers is not None)
+
+        is_train = optimizers is not None
         net.train() if is_train else net.eval()
         total_loss, total_correct, total_num = 0.0, 0.0, 0
         data_bar = tqdm(loader_train, disable=databar_disable) if is_train else tqdm(loader_val, disable=databar_disable)
 
         with (torch.enable_grad() if is_train else torch.no_grad()):
             for data, target in data_bar:
                 data, target = pretext.get(data, target)
 
                 if self.device.type == "cuda":
                     data, target = data.cuda(), target.cuda()
                     pretext = pretext.cuda()
 
-                if state in [None, 'finetune']:
-                    if self.params['num_augs'] > 0:
+                if state in [None, "finetune"]:
+                    if self.params["num_augs"] > 0:
                         data, target = augmentation(data, target, **params)
                     out, _ = net(data)
-                elif state == 'pretrain':
+                elif state == "pretrain":
                     _, out = net(data)
                 else:
                     raise NotImplementedError("state must be one of [None, 'pretrain', 'finetune']")
 
                 loss, correct = pretext(out, target)
 
                 if is_train:
@@ -205,30 +210,32 @@
                     for optimizer in optimizers:
                         optimizer.step()
 
                 total_num += 1
                 total_loss += loss.item()
 
                 if epochs == 1:
-                    train_test = 'Test'
+                    train_test = "Test"
                 else:
-                    train_test = 'Train'
+                    train_test = "Train"
 
                 val_metric = None
-                if loader_val is not None and state != 'pretrain':
+                if loader_val is not None and state != "pretrain":
                     val_metric = self.score(X=loader_val, y=y_val, metric=self.stopping_metric)
-                    data_bar.set_description('{} Epoch: [{}/{}] Train Loss: {:.4f} Validation {}: {:.2f}'.format(
-                        train_test, epoch, epochs, total_loss / total_num, self.stopping_metric.name, val_metric))
+                    data_bar.set_description(
+                        "{} Epoch: [{}/{}] Train Loss: {:.4f} Validation {}: {:.2f}".format(
+                            train_test, epoch, epochs, total_loss / total_num, self.stopping_metric.name, val_metric
+                        )
+                    )
 
                     if reporter is not None:
-                        reporter(epoch=epoch+1, validation_performance=val_metric, train_loss=total_loss)
+                        reporter(epoch=epoch + 1, validation_performance=val_metric, train_loss=total_loss)
 
                 else:
-                    data_bar.set_description(
-                        '{} Epoch: [{}/{}] Loss: {:.4f}'.format(train_test, epoch, epochs, total_loss / total_num))
+                    data_bar.set_description("{} Epoch: [{}/{}] Loss: {:.4f}".format(train_test, epoch, epochs, total_loss / total_num))
 
             return total_loss / total_num, val_metric
 
         if scheduler is not None:
             scheduler.step()
         return total_loss / total_num
 
@@ -240,78 +247,91 @@
         pretrain: discriminative task will be a pretext task
         finetune: same as supervised learning except that the model base has
                   exponentially decaying learning rate.
         """
         import torch
         import torch.nn as nn
         import torch.optim as optim
+
         from . import pretexts
 
         start_time = time.time()
         pretext_tasks = pretexts.__dict__
         optimizers = []
-        lr = self.params['lr']
-        weight_decay = self.params['weight_decay']
-        epochs = self.params['pretrain_epochs'] if state == 'pretrain' else self.params['epochs']
-        epochs_wo_improve = self.params['epochs_wo_improve']
+        lr = self.params["lr"]
+        weight_decay = self.params["weight_decay"]
+        epochs = self.params["pretrain_epochs"] if state == "pretrain" else self.params["epochs"]
+        epochs_wo_improve = self.params["epochs_wo_improve"]
 
         if state is None:
             optimizers = [optim.Adam(self.model.parameters(), lr=lr, weight_decay=weight_decay)]
-            pretext = pretext_tasks['SupervisedPretext'](self.problem_type, self.device)
-        elif state == 'pretrain':
+            pretext = pretext_tasks["SupervisedPretext"](self.problem_type, self.device)
+        elif state == "pretrain":
             optimizers = [optim.Adam(self.model.parameters(), lr=lr, weight_decay=weight_decay)]
-            pretext = pretext_tasks['BERTPretext'](self.cat_feat_origin_cards, self.device, self.params['hidden_dim'])
-        elif state == 'finetune':
-            base_exp_decay = self.params['base_exp_decay']
+            pretext = pretext_tasks["BERTPretext"](self.cat_feat_origin_cards, self.device, self.params["hidden_dim"])
+        elif state == "finetune":
+            base_exp_decay = self.params["base_exp_decay"]
             optimizer_fc = [optim.Adam(fc_layer.parameters(), lr=lr, weight_decay=weight_decay) for fc_layer in self.model.fc]
             optimizer_embeds = optim.Adam(self.model.embed.parameters(), lr=lr, weight_decay=weight_decay)
-            scheduler = optim.lr_scheduler.ExponentialLR(optimizer_embeds, gamma=base_exp_decay) # TODO: Should we be using this in _epoch()?
+            scheduler = optim.lr_scheduler.ExponentialLR(optimizer_embeds, gamma=base_exp_decay)  # TODO: Should we be using this in _epoch()?
             optimizers.extend(optimizer_fc)
             optimizers.append(optimizer_embeds)
 
-            pretext = pretext_tasks['SupervisedPretext'](self.problem_type, self.device)
+            pretext = pretext_tasks["SupervisedPretext"](self.problem_type, self.device)
 
         else:
             raise NotImplementedError("state must be one of [None, 'pretrain', 'finetune']")
 
         if self.problem_type == REGRESSION:
             loss_criterion = nn.MSELoss()
         else:
             loss_criterion = nn.CrossEntropyLoss()
 
         best_val_metric = -np.inf  # higher = better
         best_val_epoch = 0
         best_loss = np.inf
-        
+
         if self._verbosity <= 1:
             verbose_eval = -1
         elif self._verbosity == 2:
             verbose_eval = 50
         elif self._verbosity == 3:
             verbose_eval = 10
         else:
             verbose_eval = 1
-        
+
         if verbose_eval <= 0:
             databar_disable = True  # Whether or not we want to suppress output based on our verbosity
         else:
             databar_disable = False
-        
+
         for e in range(epochs):
             if e == 0:
                 logger.log(15, "TabTransformer architecture:")
                 logger.log(15, str(self.model))
 
-            train_loss, val_metric = self._epoch(net=self.model, loader_train=loader_train, loader_val=loader_val, y_val=y_val,
-                                                 optimizers=optimizers, loss_criterion=loss_criterion, \
-                                                 pretext=pretext, state=state, scheduler=None, epoch=e, epochs=epochs,
-                                                 databar_disable=databar_disable, reporter=reporter, params=self.params)
+            train_loss, val_metric = self._epoch(
+                net=self.model,
+                loader_train=loader_train,
+                loader_val=loader_val,
+                y_val=y_val,
+                optimizers=optimizers,
+                loss_criterion=loss_criterion,
+                pretext=pretext,
+                state=state,
+                scheduler=None,
+                epoch=e,
+                epochs=epochs,
+                databar_disable=databar_disable,
+                reporter=reporter,
+                params=self.params,
+            )
 
             # Early stopping for pretrain'ing based on loss.
-            if state == 'pretrain':
+            if state == "pretrain":
                 if train_loss < best_loss or e == 0:
                     if train_loss < best_loss:
                         best_loss = train_loss
                     best_val_epoch = e
             else:
                 if val_metric >= best_val_metric or e == 0:
                     if loader_val is not None:
@@ -336,28 +356,19 @@
             try:
                 self.model = torch.load(self.path + self._temp_file_name)
                 os.remove(self.path + self._temp_file_name)
             except:
                 pass
             logger.log(15, "Best model found in epoch %d" % best_val_epoch)
 
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             X_unlabeled=None,
-             time_limit=None,
-             sample_weight=None,
-             reporter=None,
-             **kwargs):
+    def _fit(self, X, y, X_val=None, y_val=None, X_unlabeled=None, time_limit=None, sample_weight=None, reporter=None, **kwargs):
         import torch
-        
-        self._verbosity = kwargs.get('verbosity', 2)
-        num_gpus = kwargs.get('num_gpus', None)
+
+        self._verbosity = kwargs.get("verbosity", 2)
+        num_gpus = kwargs.get("num_gpus", None)
         if num_gpus is None:
             if torch.cuda.is_available():
                 self.device = torch.device("cuda")
             else:
                 self.device = torch.device("cpu")
         elif num_gpus == 0:
             self.device = torch.device("cpu")
@@ -366,81 +377,83 @@
 
             if num_gpus > 1:
                 logger.warning("TabTransformer not yet configured to use more than 1 GPU. 'num_gpus' set to >1, but we will be using only 1 GPU.")
 
         if sample_weight is not None:
             logger.log(15, "sample_weight not yet supported for TabTransformerModel, this model will ignore them in training.")
 
-        if self.problem_type ==REGRESSION:
-            self.params['n_classes'] = 1
+        if self.problem_type == REGRESSION:
+            self.params["n_classes"] = 1
         elif self.problem_type == BINARY:
-            self.params['n_classes'] = 2
+            self.params["n_classes"] = 2
         elif self.problem_type == MULTICLASS:
-            self.params['n_classes'] = y.nunique()
+            self.params["n_classes"] = y.nunique()
 
         train, val, unlab = self._preprocess_train(X, X_val, X_unlabeled)
 
         num_cols = len(train.columns)
-        if num_cols > self.params['max_columns']:
+        if num_cols > self.params["max_columns"]:
             raise NotImplementedError(
                 f"This dataset has {num_cols} columns and exceeds 'max_columns' == {self.params['max_columns']}.\n"
                 f"Which is set by default to ensure the TabTransformer model will not run out of memory.\n"
-                f"If you are confident you will have enough memory, set the 'max_columns' hyperparameter higher and try again.\n")
+                f"If you are confident you will have enough memory, set the 'max_columns' hyperparameter higher and try again.\n"
+            )
 
         if self.problem_type == REGRESSION:
             train.targets = torch.FloatTensor(list(y))
             val.targets = torch.FloatTensor(list(y_val))
         else:
             train.targets = torch.LongTensor(list(y))
             val.targets = torch.LongTensor(list(y_val))
 
-        batch_size = self.params['batch_size']
-        num_workers = self.params['num_workers']
+        batch_size = self.params["batch_size"]
+        num_workers = self.params["num_workers"]
 
         loader_train = train.build_loader(batch_size, num_workers, shuffle=True)
         loader_val = val.build_loader(batch_size, num_workers)
         loader_unlab = unlab.build_loader(batch_size, num_workers) if unlab is not None else None
 
         self.cat_feat_origin_cards = loader_train.cat_feat_origin_cards
-        self.params['cat_feat_origin_cards'] = self.cat_feat_origin_cards
+        self.params["cat_feat_origin_cards"] = self.cat_feat_origin_cards
 
         self.model = self._get_model()
 
         if X_unlabeled is not None:
             # Can't spend all the time in pretraining, have to split it up.
             pretrain_time_limit = time_limit / 2 if time_limit is not None else time_limit
             pretrain_before_time = time.time()
-            self.tt_fit(loader_unlab, loader_val, y_val, state='pretrain', time_limit=pretrain_time_limit, reporter=reporter)
+            self.tt_fit(loader_unlab, loader_val, y_val, state="pretrain", time_limit=pretrain_time_limit, reporter=reporter)
             finetune_time_limit = time_limit - (time.time() - pretrain_before_time) if time_limit is not None else time_limit
-            self.tt_fit(loader_train, loader_val, y_val, state='finetune', time_limit=finetune_time_limit, reporter=reporter)
+            self.tt_fit(loader_train, loader_val, y_val, state="finetune", time_limit=finetune_time_limit, reporter=reporter)
         else:
             self.tt_fit(loader_train, loader_val, y_val, time_limit=time_limit, reporter=reporter)
 
     def _predict_proba(self, X, **kwargs):
         """
         X (torch.tensor or pd.dataframe): data for model to give prediction probabilities
         returns: np.array of k-probabilities for each of the k classes. If k=2 we drop the second probability.
         """
         import torch
         import torch.nn as nn
-        from torch.utils.data import DataLoader
         from torch.autograd import Variable
+        from torch.utils.data import DataLoader
 
         if isinstance(X, pd.DataFrame):
             # Preprocess here also calls our _preprocess, which creates a TTDataset.
             X = self.preprocess(X, **kwargs)
-            loader = X.build_loader(self.params['batch_size'], self.params['num_workers'])
+            loader = X.build_loader(self.params["batch_size"], self.params["num_workers"])
         elif isinstance(X, DataLoader):
             loader = X
         elif isinstance(X, torch.Tensor):
             X = X.rename(columns=self._get_no_period_columns(X))
-            loader = X.build_loader(self.params['batch_size'], self.params['num_workers'])
+            loader = X.build_loader(self.params["batch_size"], self.params["num_workers"])
         else:
             raise NotImplementedError(
-                "Attempting to predict against a non-supported data type. \nNeeds to be a pandas DataFrame, torch DataLoader or torch Tensor.")
+                "Attempting to predict against a non-supported data type. \nNeeds to be a pandas DataFrame, torch DataLoader or torch Tensor."
+            )
 
         self.model.eval()
         softmax = nn.Softmax(dim=1)
 
         if self.problem_type == REGRESSION:
             outputs = torch.zeros([len(loader.dataset), 1])
         else:
@@ -453,29 +466,30 @@
             with torch.no_grad():
                 data = Variable(data)
                 prob, _ = self.model(data)
                 batch_size = len(prob)
                 if self.problem_type != REGRESSION:
                     prob = softmax(prob)
 
-            outputs[iter:(iter + batch_size)] = prob
+            outputs[iter : (iter + batch_size)] = prob
             iter += batch_size
 
         if self.problem_type == BINARY:
             return outputs[:, 1].cpu().numpy()
         elif self.problem_type == REGRESSION:
             outputs = outputs.flatten()
 
         return outputs.cpu().numpy()
 
     def _get_default_searchspace(self):
         return get_default_searchspace()
 
     def save(self, path: str = None, verbose=True) -> str:
         import torch
+
         if path is None:
             path = self.path
 
         params_filepath = path + self.params_file_name
 
         os.makedirs(os.path.dirname(path), exist_ok=True)
 
@@ -489,14 +503,15 @@
         self.model = temp_model
 
         return modelobj_filepath
 
     @classmethod
     def load(cls, path: str, reset_paths=False, verbose=True):
         import torch
+
         obj: TabTransformerModel = load_pkl.load(path=path + cls.model_file_name, verbose=verbose)
         if reset_paths:
             obj.set_contexts(path)
 
         obj.model = torch.load(path + cls.params_file_name)
 
         return obj
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import logging
+
 import torch
-from torch.utils.data import Dataset, DataLoader
+from torch.utils.data import DataLoader, Dataset
 
 from . import tab_transformer_encoder
-from .tab_transformer_encoder import WontEncodeError, NullEnc
-import logging
+from .tab_transformer_encoder import NullEnc, WontEncodeError
 
 logger = logging.getLogger(__name__)
 
 
 def augmentation(data, target, **params):
     shape = data.shape
-    cat_data = torch.cat([data for _ in range(params['num_augs'])])
-    target = torch.cat([target for _ in range(params['num_augs'])]).view(-1)
-    locs_to_mask = torch.empty_like(cat_data, dtype=float).uniform_() < params['aug_mask_prob']
+    cat_data = torch.cat([data for _ in range(params["num_augs"])])
+    target = torch.cat([target for _ in range(params["num_augs"])]).view(-1)
+    locs_to_mask = torch.empty_like(cat_data, dtype=float).uniform_() < params["aug_mask_prob"]
     cat_data[locs_to_mask] = 0
     cat_data = cat_data.view(-1, shape[-1])
     return cat_data, target
 
 
 def get_col_info(X):
     """
@@ -59,46 +60,45 @@
     def n_cont_features(self):
         return len(self.cont_feat_origin) if self.encoders is not None else None
 
     def fit_feat_encoders(self):
         if self.encoders is not None:
             self.feature_encoders = {}
             for c in self.columns:
-                col = self.raw_data[c['name']]
-                enc = tab_transformer_encoder.__dict__[self.encoders[c['type']]]()
+                col = self.raw_data[c["name"]]
+                enc = tab_transformer_encoder.__dict__[self.encoders[c["type"]]]()
 
-                if c['type'] == 'SCALAR' and col.nunique() < 32:
+                if c["type"] == "SCALAR" and col.nunique() < 32:
                     logger.log(15, f"Column {c['name']} shouldn't be encoded as SCALAR. Switching to CATEGORICAL.")
-                    enc = tab_transformer_encoder.__dict__[self.encoders['CATEGORICAL']]()
+                    enc = tab_transformer_encoder.__dict__[self.encoders["CATEGORICAL"]]()
                 try:
                     enc.fit(col)
                 except WontEncodeError as e:
                     logger.log(15, f"Not encoding column '{c['name']}': {e}")
                     enc = NullEnc()
-                self.feature_encoders[c['name']] = enc
+                self.feature_encoders[c["name"]] = enc
 
     def encode(self, feature_encoders):
         if self.encoders is not None:
             self.feature_encoders = feature_encoders
 
             self.cat_feat_origin_cards = []
             cat_features = []
             self.cont_feat_origin = []
             cont_features = []
             for c in self.columns:
-                enc = feature_encoders[c['name']]
-                col = self.raw_data[c['name']]
+                enc = feature_encoders[c["name"]]
+                col = self.raw_data[c["name"]]
                 cat_feats = enc.enc_cat(col)
                 if cat_feats is not None:
-                    self.cat_feat_origin_cards += [(f'{c["name"]}_{i}_{c["type"]}', card) for i, card in
-                                                   enumerate(enc.cat_cards)]
+                    self.cat_feat_origin_cards += [(f'{c["name"]}_{i}_{c["type"]}', card) for i, card in enumerate(enc.cat_cards)]
                     cat_features.append(cat_feats)
                 cont_feats = enc.enc_cont(col)
                 if cont_feats is not None:
-                    self.cont_feat_origin += [c['name']] * enc.cont_dim
+                    self.cont_feat_origin += [c["name"]] * enc.cont_dim
                     cont_features.append(cont_feats)
             if cat_features:
                 self.cat_data = torch.cat(cat_features, dim=1)
             else:
                 self.cat_data = None
             if cont_features:
                 self.cont_data = torch.cat(cont_features, dim=1)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 
-from autogluon.features.generators import LabelEncoderFeatureGenerator
 from autogluon.core.constants import BINARY, MULTICLASS
 from autogluon.core.models import AbstractModel
 from autogluon.core.utils import generate_train_test_split
+from autogluon.features.generators import LabelEncoderFeatureGenerator
 
 
 class TabPFNModel(AbstractModel):
     """
     AutoGluon model wrapper to the TabPFN model: https://github.com/automl/TabPFN
 
     Paper: "TabPFN: A Transformer That Solves Small Tabular Classification Problems in a Second"
@@ -18,44 +18,43 @@
     and the number of rows of training data is less than 10,000.
 
     Additionally, TabPFN is only available for classification tasks with up to 10 classes and 100 features.
 
     To use this model, `tabpfn` must be installed.
     To install TabPFN, you can run `pip install autogluon.tabular[tabpfn]` or `pip install tabpfn`.
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._feature_generator = None
 
     def _fit(self, X: pd.DataFrame, y: pd.Series, **kwargs):
         from tabpfn import TabPFNClassifier
+
         ag_params = self._get_ag_params()
-        sample_rows = ag_params.get('sample_rows')
-        max_features = ag_params.get('max_features')
-        max_classes = ag_params.get('max_classes')
+        sample_rows = ag_params.get("sample_rows")
+        max_features = ag_params.get("max_features")
+        max_classes = ag_params.get("max_classes")
         if max_classes is not None and self.num_classes > max_classes:
             # TODO: Move to earlier stage when problem_type is checked
-            raise AssertionError(f'Max allowed classes for the model is {max_classes}, '
-                                 f'but found {self.num_classes} classes.')
+            raise AssertionError(f"Max allowed classes for the model is {max_classes}, " f"but found {self.num_classes} classes.")
 
         # TODO: Make sample_rows generic
         if sample_rows is not None and len(X) > sample_rows:
             X, y = self._subsample_train(X=X, y=y, num_rows=sample_rows)
         X = self.preprocess(X)
         num_features = X.shape[1]
         # TODO: Make max_features generic
         if max_features is not None and num_features > max_features:
-            raise AssertionError(f'Max allowed features for the model is {max_features}, '
-                                 f'but found {num_features} features.')
+            raise AssertionError(f"Max allowed features for the model is {max_features}, " f"but found {num_features} features.")
         hyp = self._get_model_params()
-        N_ensemble_configurations = hyp.get('N_ensemble_configurations')
-        self.model = TabPFNClassifier(
-            device='cpu',  # TODO: Add GPU option
-            N_ensemble_configurations=N_ensemble_configurations
-        ).fit(X, y, overwrite_warning=True)
+        N_ensemble_configurations = hyp.get("N_ensemble_configurations")
+        self.model = TabPFNClassifier(device="cpu", N_ensemble_configurations=N_ensemble_configurations).fit(  # TODO: Add GPU option
+            X, y, overwrite_warning=True
+        )
 
     # TODO: Make this generic by creating a generic `preprocess_train` and putting this logic prior to `_preprocess`.
     def _subsample_train(self, X: pd.DataFrame, y: pd.Series, num_rows: int, random_state=0) -> (pd.DataFrame, pd.Series):
         num_rows_to_drop = len(X) - num_rows
         X, _, y, _ = generate_train_test_split(
             X=X,
             y=y,
@@ -85,24 +84,24 @@
         """
         By default, we only use 1 ensemble configurations to speed up inference times.
         Increase the value to improve model quality while linearly increasing inference time.
 
         Model quality improvement diminishes significantly beyond `N_ensemble_configurations=8`.
         """
         default_params = {
-            'N_ensemble_configurations': 1,
+            "N_ensemble_configurations": 1,
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     @classmethod
     def _get_default_ag_args(cls) -> dict:
         default_ag_args = super()._get_default_ag_args()
         extra_ag_args = {
-            'problem_types': [BINARY, MULTICLASS],
+            "problem_types": [BINARY, MULTICLASS],
         }
         default_ag_args.update(extra_ag_args)
         return default_ag_args
 
     def _get_default_auxiliary_params(self) -> dict:
         """
         TabPFN was originally learned on synthetic datasets with 1024 rows, and struggles to
@@ -115,40 +114,40 @@
          Not implemented yet, first move this logic to the trainer level to avoid `refit_full` edge-case crashes.
         TabPFN only works on datasets with at most 100 features, so we set `max_features=100`.
         TabPFN only works on datasets with at most 10 classes, so we set `max_classes=10`.
         """
         default_auxiliary_params = super()._get_default_auxiliary_params()
         default_auxiliary_params.update(
             {
-                'sample_rows': 4096,
+                "sample_rows": 4096,
                 # 'max_rows': 20000,
-                'max_features': 100,
-                'max_classes': 10,
+                "max_features": 100,
+                "max_classes": 10,
             }
         )
         return default_auxiliary_params
 
     # FIXME: Enabling parallel bagging TabPFN creates a lot of warnings / potential failures from Ray
     # TODO: Consider not setting `max_sets=1`, and only setting it in the preset hyperparameter definition.
     @classmethod
     def _get_default_ag_args_ensemble(cls, **kwargs) -> dict:
         """
         Set max_sets to 1 when bagging, otherwise inference time could become extremely slow.
         Set fold_fitting_strategy to sequential_local, as parallel folding causing many warnings / potential errors from Ray.
         """
         default_ag_args_ensemble = super()._get_default_ag_args_ensemble(**kwargs)
         extra_ag_args_ensemble = {
-            'max_sets': 1,
-            'fold_fitting_strategy': 'sequential_local',
+            "max_sets": 1,
+            "fold_fitting_strategy": "sequential_local",
         }
         default_ag_args_ensemble.update(extra_ag_args_ensemble)
         return default_ag_args_ensemble
 
     def _ag_params(self) -> set:
-        return {'sample_rows', 'max_features', 'max_classes'}
+        return {"sample_rows", "max_features", "max_classes"}
 
     def _more_tags(self) -> dict:
         """
         Because TabPFN doesn't use validation data for early stopping, it supports refit_full natively.
         """
-        tags = {'can_refit_full': True}
+        tags = {"can_refit_full": True}
         return tags
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pickle
 
 
 class AbstractNativeCompiler:
-    name = 'native'
+    name = "native"
     save_in_pkl = True
 
     @staticmethod
     def can_compile():
         return True
 
     @staticmethod
@@ -27,19 +27,19 @@
             The compiler would optimize the model to perform best with the given input type.
         """
         AbstractNativeCompiler.save(model, path)
 
     @staticmethod
     def save(model, path: str):
         os.makedirs(os.path.dirname(path), exist_ok=True)
-        with open(os.path.join(path, 'model_native.pkl'), 'wb') as fp:
+        with open(os.path.join(path, "model_native.pkl"), "wb") as fp:
             fp.write(pickle.dumps(model))
 
     @staticmethod
     def load(path: str):
         pkl = None
-        with open(os.path.join(path, 'model_native.pkl'), 'rb') as fp:
+        with open(os.path.join(path, "model_native.pkl"), "rb") as fp:
             pkl = fp.read()
         return pickle.loads(pkl)
 
 
 TabularNeuralNetTorchNativeCompiler = AbstractNativeCompiler
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,16 @@
             OnnxReshape(idx, np.array([batch_size, n_quantiles], dtype=np.int64), op_version=opv),
             axis=1,
             op_version=opv,
             output_names=[f"argmin_col{feature_idx}"],
         )
         references = np.clip(norm.ppf(op.references_), -5.2, 5.2).astype(dtype)
         cst = np.broadcast_to(references, (batch_size, n_quantiles))
-        argmin_reshaped = OnnxReshape(
-            argmin, np.array([batch_size, 1], dtype=np.int64), output_names=[f"reshape_col{feature_idx}"]
-        )
-        ref = OnnxGatherElements(
-            cst, argmin_reshaped, axis=1, op_version=opv, output_names=[f"gathernd_col{feature_idx}"]
-        )
+        argmin_reshaped = OnnxReshape(argmin, np.array([batch_size, 1], dtype=np.int64), output_names=[f"reshape_col{feature_idx}"])
+        ref = OnnxGatherElements(cst, argmin_reshaped, axis=1, op_version=opv, output_names=[f"gathernd_col{feature_idx}"])
         Y_col.append(OnnxReshape(ref, np.array([batch_size, 1], dtype=np.int64), output_names=[f"Y_col{feature_idx}"]))
     Y = OnnxConcat(*Y_col, axis=1, op_version=opv, output_names=out[:1])
     Y.add_to(scope, container)
 
 
 def onehot_handle_unknown_transformer_shape_calculator(operator):
     op = operator.raw_operator
@@ -136,17 +132,15 @@
     # about types, every constant should have the same
     # type as the input.
     dtype = guess_numpy_type(X.type)
     batch_size = X.type.shape[0]
     num_categories = len(op.categories_)
 
     C_col = op.categories_
-    X_col = OnnxSplit(
-        X, axis=1, output_names=[f"{name_prefix}X_col{x}" for x in range(num_categories)], op_version=opv
-    )
+    X_col = OnnxSplit(X, axis=1, output_names=[f"{name_prefix}X_col{x}" for x in range(num_categories)], op_version=opv)
     X_col.add_to(scope, container)
     Y_col = []
     for feature_idx in range(num_categories):
         # This implements
         # > X_col = np.searchsorted(X_col_finite, self.references_)
         #
         # Specifically, for yi = np.searchsorted(xi, x), we implement
@@ -401,35 +395,25 @@
             # Useful shortcut, skips the case when end is None
             # (unknown dimension)
             return 0, 0
         vi = 0
         pos = 0
         end = inputs[0].type.shape[1] if isinstance(inputs[0].type, TensorType) else 1
         if end is None:
-            raise RuntimeError(
-                "Cannot extract a specific column {0} when "
-                "one input ('{1}') has unknown "
-                "dimension.".format(i, inputs[0])
-            )
+            raise RuntimeError("Cannot extract a specific column {0} when " "one input ('{1}') has unknown " "dimension.".format(i, inputs[0]))
         while True:
             if pos <= i < end:
                 return (vi, i - pos)
             vi += 1
             pos = end
             if vi >= len(inputs):
-                raise RuntimeError(
-                    "Input {} (i={}, end={}) is not available in\n{}".format(vi, i, end, pprint.pformat(inputs))
-                )
+                raise RuntimeError("Input {} (i={}, end={}) is not available in\n{}".format(vi, i, end, pprint.pformat(inputs)))
             rel_end = inputs[vi].type.shape[1] if isinstance(inputs[vi].type, TensorType) else 1
             if rel_end is None:
-                raise RuntimeError(
-                    "Cannot extract a specific column {0} when "
-                    "one input ('{1}') has unknown "
-                    "dimension.".format(i, inputs[vi])
-                )
+                raise RuntimeError("Cannot extract a specific column {0} when " "one input ('{1}') has unknown " "dimension.".format(i, inputs[vi]))
             end += rel_end
     else:
         for ind, inp in enumerate(inputs):
             if inp.raw_name == i:
                 return ind, 0
         raise RuntimeError(
             "Unable to find column name %r among names %r. "
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 """ Default (fixed) hyperparameter values used in Tabular Neural Network models.
     A value of None typically indicates an adaptive value for the hyperparameter will be chosen based on the data.
 """
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION
 
 
 def get_fixed_params(framework):
-    """ Parameters that currently cannot be searched during HPO """
+    """Parameters that currently cannot be searched during HPO"""
     fixed_params = {
         # 'seed_value': 0,  # random seed for reproducibility (set = None to ignore)
     }
     pytorch_fixed_params = {
-        'num_epochs': 500,  # maximum number of epochs (passes over full dataset) for training NN
-        'epochs_wo_improve': 20,  # we terminate training if validation performance hasn't improved in the last 'epochs_wo_improve' # of epochs
+        "num_epochs": 500,  # maximum number of epochs (passes over full dataset) for training NN
+        "epochs_wo_improve": 20,  # we terminate training if validation performance hasn't improved in the last 'epochs_wo_improve' # of epochs
     }
     return merge_framework_params(framework=framework, shared_params=fixed_params, pytorch_params=pytorch_fixed_params)
 
 
 def get_hyper_params(framework):
-    """ Parameters that currently can be tuned during HPO """
+    """Parameters that currently can be tuned during HPO"""
     hyper_params = {
         ## Hyperparameters for neural net architecture:
-        'activation': 'relu',  # Activation function
+        "activation": "relu",  # Activation function
         # Options: ['relu', 'softrelu', 'tanh', 'softsign'], options for pytorch: ['relu', 'elu', 'tanh']
-        'embedding_size_factor': 1.0,  # scaling factor to adjust size of embedding layers (float > 0)
+        "embedding_size_factor": 1.0,  # scaling factor to adjust size of embedding layers (float > 0)
         # Options: range[0.01 - 100] on log-scale
-        'embed_exponent': 0.56,  # exponent used to determine size of embedding layers based on # categories.
-        'max_embedding_dim': 100,  # maximum size of embedding layer for a single categorical feature (int > 0).
+        "embed_exponent": 0.56,  # exponent used to determine size of embedding layers based on # categories.
+        "max_embedding_dim": 100,  # maximum size of embedding layer for a single categorical feature (int > 0).
         ## Regression-specific hyperparameters:
-        'y_range': None,  # Tuple specifying whether Y is constrained to (min_y, max_y). Can be = (-np.inf, np.inf).
+        "y_range": None,  # Tuple specifying whether Y is constrained to (min_y, max_y). Can be = (-np.inf, np.inf).
         # If None, inferred based on training labels. Note: MUST be None for classification tasks!
-        'y_range_extend': 0.05,  # Only used to extend size of inferred y_range when y_range = None.
+        "y_range_extend": 0.05,  # Only used to extend size of inferred y_range when y_range = None.
         ## Hyperparameters for neural net training:
-        'dropout_prob': 0.1,  # dropout probability, = 0 turns off Dropout.
+        "dropout_prob": 0.1,  # dropout probability, = 0 turns off Dropout.
         # Options: range(0.0, 0.5)
-        'optimizer': 'adam',  # Which optimizer to use for training
+        "optimizer": "adam",  # Which optimizer to use for training
         # Options include: ['adam','sgd']
-        'learning_rate': 3e-4,  # learning rate used for NN training (float > 0)
-        'weight_decay': 1e-6,  # weight decay regularizer (float > 0)
+        "learning_rate": 3e-4,  # learning rate used for NN training (float > 0)
+        "weight_decay": 1e-6,  # weight decay regularizer (float > 0)
         ## Hyperparameters for data processing:
-        'proc.embed_min_categories': 4,  # apply embedding layer to categorical features with at least this many levels. Features with fewer levels are one-hot encoded. Choose big value to avoid use of Embedding layers
+        "proc.embed_min_categories": 4,  # apply embedding layer to categorical features with at least this many levels. Features with fewer levels are one-hot encoded. Choose big value to avoid use of Embedding layers
         # Options: [3,4,10, 100, 1000]
-        'proc.impute_strategy': 'median',  # strategy argument of sklearn.SimpleImputer() used to impute missing numeric values
+        "proc.impute_strategy": "median",  # strategy argument of sklearn.SimpleImputer() used to impute missing numeric values
         # Options: ['median', 'mean', 'most_frequent']
-        'proc.max_category_levels': 100,  # maximum number of allowed levels per categorical feature
+        "proc.max_category_levels": 100,  # maximum number of allowed levels per categorical feature
         # Options: [10, 100, 200, 300, 400, 500, 1000, 10000]
-        'proc.skew_threshold': 0.99,  # numerical features whose absolute skewness is greater than this receive special power-transform preprocessing. Choose big value to avoid using power-transforms
+        "proc.skew_threshold": 0.99,  # numerical features whose absolute skewness is greater than this receive special power-transform preprocessing. Choose big value to avoid using power-transforms
         # Options: [0.2, 0.3, 0.5, 0.8, 0.9, 0.99, 0.999, 1.0, 10.0, 100.0]
-        'use_ngram_features': False,  # If False, will drop automatically generated ngram features from language features. This results in worse model quality but far faster inference and training times.
+        "use_ngram_features": False,  # If False, will drop automatically generated ngram features from language features. This results in worse model quality but far faster inference and training times.
         # Options: [True, False]
     }
     pytorch_hyper_params = {
-        'num_layers': 4,  # number of layers
+        "num_layers": 4,  # number of layers
         # Options: [2, 3, 4, 5]
-        'hidden_size': 128,  # number of hidden units in each layer
+        "hidden_size": 128,  # number of hidden units in each layer
         # Options: [128, 256, 512]
-        'max_batch_size': 512,  # maximum batch-size, actual batch size may be slightly smaller.
-        'use_batchnorm': False,  # whether or not to utilize batch normalization
+        "max_batch_size": 512,  # maximum batch-size, actual batch size may be slightly smaller.
+        "use_batchnorm": False,  # whether or not to utilize batch normalization
         # Options: [True, False]
-        'loss_function': 'auto',  # Pytorch loss function minimized during training
+        "loss_function": "auto",  # Pytorch loss function minimized during training
         # Example options for regression: nn.MSELoss(), nn.L1Loss()
     }
     return merge_framework_params(framework=framework, shared_params=hyper_params, pytorch_params=pytorch_hyper_params)
 
 
 def get_quantile_hyper_params(framework):
-    """ Parameters that currently can be searched during HPO """
+    """Parameters that currently can be searched during HPO"""
     hyper_params = get_hyper_params(framework)
     new_hyper_params = {
-        'gamma': 5.0,  # margin loss weight which helps ensure noncrossing quantile estimates
+        "gamma": 5.0,  # margin loss weight which helps ensure noncrossing quantile estimates
         # Options: range(0.1, 10.0)
-        'alpha': 0.01,  # used for smoothing huber pinball loss
+        "alpha": 0.01,  # used for smoothing huber pinball loss
     }
     hyper_params.update(new_hyper_params)
     return hyper_params
 
 
 # Note: params for original NNTabularModel were:
 # weight_decay=0.01, dropout_prob = 0.1, batch_size = 2048, lr = 1e-2, epochs=30, layers= [200, 100] (semi-equivalent to our layers = [100],numeric_embed_dim=200)
@@ -86,14 +86,15 @@
     elif problem_type == REGRESSION:
         return get_param_regression(framework)
     elif problem_type == QUANTILE:
         return get_param_quantile(framework)
     else:
         return get_param_binary(framework)
 
+
 def get_param_binary(framework):
     params = get_fixed_params(framework)
     params.update(get_hyper_params(framework))
     return params
 
 
 def get_param_multiclass(framework, num_classes):
@@ -101,20 +102,20 @@
 
 
 def get_param_regression(framework):
     return get_param_binary(framework)  # Use same hyperparameters as for binary classification for now.
 
 
 def get_param_quantile(framework):
-    if framework != 'pytorch':
+    if framework != "pytorch":
         raise ValueError("Only pytorch tabular neural network is currently supported for quantile regression.")
     params = get_fixed_params(framework)
     params.update(get_quantile_hyper_params(framework))
     return params
 
 
 def merge_framework_params(framework, shared_params, pytorch_params):
-    if framework == 'pytorch':
+    if framework == "pytorch":
         shared_params.update(pytorch_params)
     else:
         raise ValueError("framework must be 'pytorch'")
     return shared_params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """ Default (fixed) hyperparameter search spaces used in Tabular Neural Network models.
 """
 from autogluon.common import space
-
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION
 
 from .parameters import merge_framework_params
 
 
 def get_default_searchspace(problem_type, framework, num_classes=None):
     params = {
-        'learning_rate': space.Real(1e-4, 3e-2, default=3e-4, log=True),
-        'weight_decay': space.Real(1e-12, 0.1, default=1e-6, log=True),
-        'dropout_prob': space.Categorical(0.1, 0.0, 0.5, 0.2, 0.3, 0.4),
-        'embedding_size_factor': space.Categorical(1.0, 0.5, 1.5, 0.7, 0.6, 0.8, 0.9, 1.1, 1.2, 1.3, 1.4),
-        'proc.embed_min_categories': space.Categorical(4, 3, 10, 100, 1000),
-        'proc.impute_strategy': space.Categorical('median', 'mean', 'most_frequent'),
-        'proc.max_category_levels': space.Categorical(100, 10, 20, 200, 300, 400, 500, 1000, 10000),
-        'proc.skew_threshold': space.Categorical(0.99, 0.2, 0.3, 0.5, 0.8, 0.9, 0.999, 1.0, 10.0, 100.0),
+        "learning_rate": space.Real(1e-4, 3e-2, default=3e-4, log=True),
+        "weight_decay": space.Real(1e-12, 0.1, default=1e-6, log=True),
+        "dropout_prob": space.Categorical(0.1, 0.0, 0.5, 0.2, 0.3, 0.4),
+        "embedding_size_factor": space.Categorical(1.0, 0.5, 1.5, 0.7, 0.6, 0.8, 0.9, 1.1, 1.2, 1.3, 1.4),
+        "proc.embed_min_categories": space.Categorical(4, 3, 10, 100, 1000),
+        "proc.impute_strategy": space.Categorical("median", "mean", "most_frequent"),
+        "proc.max_category_levels": space.Categorical(100, 10, 20, 200, 300, 400, 500, 1000, 10000),
+        "proc.skew_threshold": space.Categorical(0.99, 0.2, 0.3, 0.5, 0.8, 0.9, 0.999, 1.0, 10.0, 100.0),
     }
     pytorch_params = {
-        'use_batchnorm': space.Categorical(False, True),
-        'num_layers': space.Categorical(2, 3, 4),
-        'hidden_size': space.Categorical(128, 256, 512),
-        'activation': space.Categorical('relu', 'elu'),
+        "use_batchnorm": space.Categorical(False, True),
+        "num_layers": space.Categorical(2, 3, 4),
+        "hidden_size": space.Categorical(128, 256, 512),
+        "activation": space.Categorical("relu", "elu"),
     }
     params = merge_framework_params(framework=framework, shared_params=params, pytorch_params=pytorch_params)
     if problem_type == QUANTILE:
-        problem_params =  get_searchspace_quantile(framework)
+        problem_params = get_searchspace_quantile(framework)
     elif problem_type == BINARY:
         problem_params = get_searchspace_binary(framework)
     elif problem_type == MULTICLASS:
         problem_params = get_searchspace_multiclass(framework, num_classes=num_classes)
     elif problem_type == REGRESSION:
         problem_params = get_searchspace_regression(framework)
     params.update(problem_params)
@@ -43,25 +42,25 @@
 
 def get_searchspace_binary(framework):
     return {}
 
 
 def get_searchspace_regression(framework):
     params = {
-        'weight_decay': space.Real(1e-12, 1.0, default=1e-6, log=True),
+        "weight_decay": space.Real(1e-12, 1.0, default=1e-6, log=True),
     }
     pytorch_params = {
-        'activation': space.Categorical('relu', 'elu', 'tanh'),
+        "activation": space.Categorical("relu", "elu", "tanh"),
     }
     return merge_framework_params(framework=framework, shared_params=params, pytorch_params=pytorch_params)
 
 
 def get_searchspace_quantile(framework):
-    if framework != 'pytorch':
+    if framework != "pytorch":
         raise ValueError("Only pytorch tabular neural network is currently supported for quantile regression.")
     params = {
-        'activation': space.Categorical('relu', 'elu', 'tanh'),
-        'weight_decay': space.Real(1e-12, 1.0, default=1e-6, log=True),
-        'gamma': space.Real(0.1, 10.0, default=5.0),
-        'alpha': space.Categorical(0.001, 0.01, 0.1, 1.0),
+        "activation": space.Categorical("relu", "elu", "tanh"),
+        "weight_decay": space.Real(1e-12, 1.0, default=1e-6, log=True),
+        "gamma": space.Real(0.1, 10.0, default=5.0),
+        "alpha": space.Categorical(0.001, 0.01, 0.1, 1.0),
     }
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 import logging
 import os
 import random
 import time
 import warnings
+from typing import Dict, Union
+
 import numpy as np
 import pandas as pd
 
-from typing import Dict, Union
-
-from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY
+from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT, S_TEXT_AS_CATEGORY, S_TEXT_NGRAM
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_torch
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 from autogluon.core.hpo.constants import RAY_BACKEND
-from autogluon.core.utils.exceptions import TimeLimitExceeded
 from autogluon.core.models.abstract.abstract_nn_model import AbstractNeuralNetworkModel
+from autogluon.core.utils.exceptions import TimeLimitExceeded
 
 from ..compilers.native import TabularNeuralNetTorchNativeCompiler
 from ..compilers.onnx import TabularNeuralNetTorchOnnxCompiler
 from ..hyperparameters.parameters import get_default_param
 from ..hyperparameters.searchspaces import get_default_searchspace
 from ..utils.data_preprocessor import create_preprocessor, get_feature_arraycol_map, get_feature_type_map
 from ..utils.nn_architecture_utils import infer_y_range
@@ -31,15 +31,15 @@
 class TabularNeuralNetTorchModel(AbstractNeuralNetworkModel):
     """
     PyTorch neural network models for classification/regression with tabular data.
     """
 
     # Constants used throughout this class:
     unique_category_str = np.nan  # string used to represent missing values and unknown categories for categorical features.
-    temp_file_name = 'temp_model.pt'  # Stores temporary network parameters (eg. during the course of training)
+    temp_file_name = "temp_model.pt"  # Stores temporary network parameters (eg. during the course of training)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.feature_arraycol_map = None
         self.feature_type_map = None
         self.features_to_drop = []  # may change between different bagging folds. TODO: consider just removing these from self._features_internal
         self.processor = None  # data processor
@@ -47,45 +47,46 @@
         self._architecture_desc = None
         self.optimizer = None
         self.device = None
         self.max_batch_size = None
         self._num_cpus_infer = None
 
     def _set_default_params(self):
-        """ Specifies hyperparameter values to use by default """
-        default_params = get_default_param(problem_type=self.problem_type, framework='pytorch')
+        """Specifies hyperparameter values to use by default"""
+        default_params = get_default_param(problem_type=self.problem_type, framework="pytorch")
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             valid_raw_types=[R_BOOL, R_INT, R_FLOAT, R_CATEGORY],
             ignored_type_group_special=[S_TEXT_NGRAM, S_TEXT_AS_CATEGORY],
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     def _get_default_searchspace(self):
-        return get_default_searchspace(problem_type=self.problem_type, framework='pytorch')
+        return get_default_searchspace(problem_type=self.problem_type, framework="pytorch")
 
     def _get_num_net_outputs(self):
         if self.problem_type in [MULTICLASS, SOFTCLASS]:
             return self.num_classes
         elif self.problem_type == BINARY:
             return 2
         elif self.problem_type == REGRESSION:
             return 1
         elif self.problem_type == QUANTILE:
             return len(self.quantile_levels)
         else:
-            raise ValueError(f'Unknown problem_type: {self.problem_type}')
+            raise ValueError(f"Unknown problem_type: {self.problem_type}")
 
     def _get_device(self, num_gpus):
         import torch
+
         if num_gpus is not None and num_gpus >= 1:
             if torch.cuda.is_available():
                 device = torch.device("cuda")
                 logger.log(15, "Training on GPU")
                 if num_gpus > 1:
                     logger.warning(f"{self.__class__.__name__} not yet able to use more than 1 GPU. 'num_gpus' is set to >1, but we will be using only 1 GPU.")
             else:
@@ -94,100 +95,103 @@
         else:
             device = torch.device("cpu")
             logger.log(15, "Training on CPU")
         return device
 
     def _set_net_defaults(self, train_dataset, params):
         params = params.copy()
-        y_range_extend = params.pop('y_range_extend', None)
+        y_range_extend = params.pop("y_range_extend", None)
         """ Sets dataset-adaptive default values to use for our neural network """
         if self.problem_type in [REGRESSION, QUANTILE]:
-            if params['y_range'] is None:
-                params['y_range'] = infer_y_range(y_vals=train_dataset.data_list[train_dataset.label_index], y_range_extend=y_range_extend)
+            if params["y_range"] is None:
+                params["y_range"] = infer_y_range(y_vals=train_dataset.data_list[train_dataset.label_index], y_range_extend=y_range_extend)
         return params
 
     def _get_default_loss_function(self):
         import torch
+
         if self.problem_type == REGRESSION:
             return torch.nn.L1Loss()  # or torch.nn.MSELoss()
         elif self.problem_type in [BINARY, MULTICLASS]:
             return torch.nn.CrossEntropyLoss()
         elif self.problem_type == SOFTCLASS:
             return torch.nn.KLDivLoss()  # compares log-probability prediction vs probability target.
 
     @staticmethod
     def _prepare_params(params):
         params = params.copy()
 
-        processor_param_keys = {'proc.embed_min_categories', 'proc.impute_strategy', 'proc.max_category_levels', 'proc.skew_threshold', 'use_ngram_features'}
+        processor_param_keys = {"proc.embed_min_categories", "proc.impute_strategy", "proc.max_category_levels", "proc.skew_threshold", "use_ngram_features"}
         processor_kwargs = {k: v for k, v in params.items() if k in processor_param_keys}
         for key in processor_param_keys:
             params.pop(key, None)
 
-        optimizer_param_keys = {'optimizer', 'learning_rate', 'weight_decay'}
+        optimizer_param_keys = {"optimizer", "learning_rate", "weight_decay"}
         optimizer_kwargs = {k: v for k, v in params.items() if k in optimizer_param_keys}
         for key in optimizer_param_keys:
             params.pop(key, None)
 
-        fit_param_keys = {'num_epochs', 'epochs_wo_improve'}
+        fit_param_keys = {"num_epochs", "epochs_wo_improve"}
         fit_kwargs = {k: v for k, v in params.items() if k in fit_param_keys}
         for key in fit_param_keys:
             params.pop(key, None)
 
-        loss_param_keys = {'loss_function', 'gamma'}
+        loss_param_keys = {"loss_function", "gamma"}
         loss_kwargs = {k: v for k, v in params.items() if k in loss_param_keys}
         for key in loss_param_keys:
             params.pop(key, None)
 
         return processor_kwargs, optimizer_kwargs, fit_kwargs, loss_kwargs, params
 
-    def _fit(self, X, y, X_val=None, y_val=None,
-             time_limit=None, sample_weight=None, num_cpus=1, num_gpus=0, reporter=None, verbosity=2, **kwargs):
+    def _fit(self, X, y, X_val=None, y_val=None, time_limit=None, sample_weight=None, num_cpus=1, num_gpus=0, reporter=None, verbosity=2, **kwargs):
         try_import_torch()
         import torch
+
         torch.set_num_threads(num_cpus)
         from .tabular_torch_dataset import TabularTorchDataset
 
         start_time = time.time()
 
         params = self._get_model_params()
 
         processor_kwargs, optimizer_kwargs, fit_kwargs, loss_kwargs, params = self._prepare_params(params=params)
 
-        seed_value = params.pop('seed_value', 0)
+        seed_value = params.pop("seed_value", 0)
 
-        self._num_cpus_infer = params.pop('_num_cpus_infer', 1)
+        self._num_cpus_infer = params.pop("_num_cpus_infer", 1)
         if seed_value is not None:  # Set seeds
             random.seed(seed_value)
             np.random.seed(seed_value)
             torch.manual_seed(seed_value)
 
         if sample_weight is not None:  # TODO: support
-            logger.log(15, f"sample_weight not yet supported for {self.__class__.__name__},"
-                           " this model will ignore them in training.")
+            logger.log(15, f"sample_weight not yet supported for {self.__class__.__name__}," " this model will ignore them in training.")
 
         if num_cpus is not None:
-            self.num_dataloading_workers = max(1, int(num_cpus/2.0))
+            self.num_dataloading_workers = max(1, int(num_cpus / 2.0))
         else:
             self.num_dataloading_workers = 1
         if self.num_dataloading_workers == 1:
             self.num_dataloading_workers = 0  # TODO: verify 0 is typically faster and uses less memory than 1 in pytorch
         self.num_dataloading_workers = 0  # TODO: >0 crashes on MacOS
-        self.max_batch_size = params.pop('max_batch_size', 512)
-        batch_size = params.pop('batch_size', None)
+        self.max_batch_size = params.pop("max_batch_size", 512)
+        batch_size = params.pop("batch_size", None)
         if batch_size is None:
             if isinstance(X, TabularTorchDataset):
                 batch_size = min(int(2 ** (3 + np.floor(np.log10(len(X))))), self.max_batch_size)
             else:
                 batch_size = min(int(2 ** (3 + np.floor(np.log10(X.shape[0])))), self.max_batch_size)
 
         train_dataset, val_dataset = self._generate_datasets(X=X, y=y, params=processor_kwargs, X_val=X_val, y_val=y_val)
-        logger.log(15, f"Training data for {self.__class__.__name__} has: "
-                       f"{train_dataset.num_examples} examples, {train_dataset.num_features} features "
-                       f"({len(train_dataset.feature_groups['vector'])} vector, {len(train_dataset.feature_groups['embed'])} embedding)")
+        logger.log(
+            15,
+            f"Training data for {self.__class__.__name__} has: "
+            f"{train_dataset.num_examples} examples, {train_dataset.num_features} features "
+            f"({len(train_dataset.feature_groups['vector'])} vector, {len(train_dataset.feature_groups['embed'])} embedding)",
+        )
 
         self.device = self._get_device(num_gpus=num_gpus)
 
         self._get_net(train_dataset, params=params)
         self.optimizer = self._init_optimizer(**optimizer_kwargs)
 
         if time_limit is not None:
@@ -196,53 +200,53 @@
             time_limit = time_limit - time_elapsed
 
             # if 60% of time was spent preprocessing, likely not enough time to train model
             if time_limit <= time_limit_orig * 0.4:
                 raise TimeLimitExceeded
 
         # train network
-        self._train_net(train_dataset=train_dataset,
-                        loss_kwargs=loss_kwargs,
-                        batch_size=batch_size,
-                        val_dataset=val_dataset,
-                        time_limit=time_limit,
-                        reporter=reporter,
-                        verbosity=verbosity,
-                        **fit_kwargs)
+        self._train_net(
+            train_dataset=train_dataset,
+            loss_kwargs=loss_kwargs,
+            batch_size=batch_size,
+            val_dataset=val_dataset,
+            time_limit=time_limit,
+            reporter=reporter,
+            verbosity=verbosity,
+            **fit_kwargs,
+        )
 
     def _get_net(self, train_dataset, params):
         from .torch_network_modules import EmbedNet
 
         # set network params
         params = self._set_net_defaults(train_dataset, params)
-        self.model = EmbedNet(problem_type=self.problem_type, num_net_outputs=self._get_num_net_outputs(), quantile_levels=self.quantile_levels,
-                              train_dataset=train_dataset, device=self.device, **params)
+        self.model = EmbedNet(
+            problem_type=self.problem_type,
+            num_net_outputs=self._get_num_net_outputs(),
+            quantile_levels=self.quantile_levels,
+            train_dataset=train_dataset,
+            device=self.device,
+            **params,
+        )
         self.model = self.model.to(self.device)
         if not os.path.exists(self.path):
             os.makedirs(self.path)
 
-    def _train_net(self,
-                   train_dataset,
-                   loss_kwargs,
-                   batch_size,
-                   num_epochs,
-                   epochs_wo_improve,
-                   val_dataset=None,
-                   time_limit=None,
-                   reporter=None,
-                   verbosity=2):
+    def _train_net(self, train_dataset, loss_kwargs, batch_size, num_epochs, epochs_wo_improve, val_dataset=None, time_limit=None, reporter=None, verbosity=2):
         import torch
+
         start_time = time.time()
         logging.debug("initializing neural network...")
         self.model.init_params()
         logging.debug("initialized")
         train_dataloader = train_dataset.build_loader(batch_size, self.num_dataloading_workers, is_test=False)
 
-        if isinstance(loss_kwargs.get('loss_function', 'auto'), str) and loss_kwargs.get('loss_function', 'auto') == 'auto':
-            loss_kwargs['loss_function'] = self._get_default_loss_function()
+        if isinstance(loss_kwargs.get("loss_function", "auto"), str) and loss_kwargs.get("loss_function", "auto") == "auto":
+            loss_kwargs["loss_function"] = self._get_default_loss_function()
 
         if val_dataset is not None:
             y_val = val_dataset.get_labels()
             if y_val.ndim == 2 and y_val.shape[1] == 1:
                 y_val = y_val.flatten()
         else:
             y_val = None
@@ -275,15 +279,15 @@
             logger.log(15, "Untrained Tabular Neural Network saved to file")
             return
 
         # start training loop:
         logger.log(15, f"Training tabular neural network for up to {num_epochs} epochs...")
         total_updates = 0
         num_updates_per_epoch = max(round(len(train_dataset) / batch_size) + 1, 1)
-        update_to_check_time = min(10, max(1, int(num_updates_per_epoch/10)))
+        update_to_check_time = min(10, max(1, int(num_updates_per_epoch / 10)))
         do_update = True
         epoch = 0
         best_epoch = 0
         best_val_metric = -np.inf  # higher = better
         best_val_update = 0
         val_improve_epoch = 0  # most recent epoch where validation-score strictly improved
         start_fit_time = time.time()
@@ -311,16 +315,18 @@
                 if time_limit is not None:
                     time_cur = time.time()
                     update_cur = batch_idx + 1
                     if epoch == 0 and update_cur == update_to_check_time:
                         time_elapsed_epoch = time_cur - time_start_epoch
                         estimated_time = time_elapsed_epoch / update_cur * num_updates_per_epoch
                         if estimated_time > time_limit:
-                            logger.log(30, f"\tNot enough time to train first epoch. "
-                                           f"(Time Required: {round(estimated_time, 2)}s, Time Left: {round(time_limit, 2)}s)")
+                            logger.log(
+                                30,
+                                f"\tNot enough time to train first epoch. " f"(Time Required: {round(estimated_time, 2)}s, Time Left: {round(time_limit, 2)}s)",
+                            )
                             raise TimeLimitExceeded
                     time_elapsed = time_cur - start_fit_time
                     if time_limit < time_elapsed:
                         logger.log(15, f"\tRan out of time, stopping training early. (Stopped on Update {total_updates} (Epoch {epoch}))")
                         do_update = False
                         break
 
@@ -331,93 +337,101 @@
 
             # validation
             if val_dataset is not None:
                 # compute validation score
                 val_metric = self.score(X=val_dataset, y=y_val, metric=self.stopping_metric, _reset_threads=False)
                 if np.isnan(val_metric):
                     if best_epoch == 0:
-                        raise RuntimeError(f"NaNs encountered in {self.__class__.__name__} training. "
-                                           "Features/labels may be improperly formatted, "
-                                           "or NN weights may have diverged.")
+                        raise RuntimeError(
+                            f"NaNs encountered in {self.__class__.__name__} training. "
+                            "Features/labels may be improperly formatted, "
+                            "or NN weights may have diverged."
+                        )
                     else:
-                        logger.warning(f"Warning: NaNs encountered in {self.__class__.__name__} training. "
-                                       "Reverting model to last checkpoint without NaNs.")
+                        logger.warning(f"Warning: NaNs encountered in {self.__class__.__name__} training. " "Reverting model to last checkpoint without NaNs.")
                         break
 
                 # update best validation
                 if (val_metric >= best_val_metric) or best_epoch == 0:
                     if val_metric > best_val_metric:
                         val_improve_epoch = epoch
                     best_val_metric = val_metric
                     os.makedirs(os.path.dirname(self.path), exist_ok=True)
                     torch.save(self.model, net_filename)
                     best_epoch = epoch
                     best_val_update = total_updates
                 if verbose_eval:
-                    logger.log(15, f"Epoch {epoch} (Update {total_updates}).\t"
-                                   f"Train loss: {round(total_train_loss / total_train_size, 4)}, "
-                                   f"Val {self.stopping_metric.name}: {round(val_metric, 4)}, "
-                                   f"Best Epoch: {best_epoch}")
+                    logger.log(
+                        15,
+                        f"Epoch {epoch} (Update {total_updates}).\t"
+                        f"Train loss: {round(total_train_loss / total_train_size, 4)}, "
+                        f"Val {self.stopping_metric.name}: {round(val_metric, 4)}, "
+                        f"Best Epoch: {best_epoch}",
+                    )
 
                 if reporter is not None:
-                    reporter(epoch=total_updates,
-                             validation_performance=val_metric,  # Higher val_metric = better
-                             train_loss=total_train_loss / total_train_size,
-                             eval_metric=self.eval_metric.name,
-                             greater_is_better=self.eval_metric.greater_is_better)
+                    reporter(
+                        epoch=total_updates,
+                        validation_performance=val_metric,  # Higher val_metric = better
+                        train_loss=total_train_loss / total_train_size,
+                        eval_metric=self.eval_metric.name,
+                        greater_is_better=self.eval_metric.greater_is_better,
+                    )
 
                 # no improvement
                 if epoch - val_improve_epoch >= epochs_wo_improve:
                     break
 
             if epoch >= num_epochs:
                 break
 
             if time_limit is not None:
                 time_elapsed = time.time() - start_fit_time
-                time_epoch_average = time_elapsed / (epoch+1)
+                time_epoch_average = time_elapsed / (epoch + 1)
                 time_left = time_limit - time_elapsed
                 if time_left < time_epoch_average:
                     logger.log(20, f"\tRan out of time, stopping training early. (Stopping on epoch {epoch})")
                     break
 
         if epoch == 0:
-            raise AssertionError('0 epochs trained!')
+            raise AssertionError("0 epochs trained!")
 
         # revert back to best model
         if val_dataset is not None:
             logger.log(15, f"Best model found on Epoch {best_epoch} (Update {best_val_update}). Val {self.stopping_metric.name}: {best_val_metric}")
             try:
                 self.model = torch.load(net_filename)
                 os.remove(net_filename)
             except FileNotFoundError:
                 pass
         else:
             logger.log(15, f"Best model found on Epoch {best_epoch} (Update {best_val_update}).")
-        self.params_trained['batch_size'] = batch_size
-        self.params_trained['num_epochs'] = best_epoch
+        self.params_trained["batch_size"] = batch_size
+        self.params_trained["num_epochs"] = best_epoch
 
     def _predict_proba(self, X, **kwargs):
-        """ To align predict with abstract_model API.
-            Preprocess here only refers to feature processing steps done by all AbstractModel objects,
-            not tabularNN-specific preprocessing steps.
-            If X is not DataFrame but instead TabularNNDataset object, we can still produce predictions,
-            but cannot use preprocess in this case (needs to be already processed).
+        """To align predict with abstract_model API.
+        Preprocess here only refers to feature processing steps done by all AbstractModel objects,
+        not tabularNN-specific preprocessing steps.
+        If X is not DataFrame but instead TabularNNDataset object, we can still produce predictions,
+        but cannot use preprocess in this case (needs to be already processed).
         """
         from .tabular_torch_dataset import TabularTorchDataset
+
         if isinstance(X, TabularTorchDataset):
             return self._predict_tabular_data(new_data=X, process=False)
         elif isinstance(X, pd.DataFrame):
             X = self.preprocess(X, **kwargs)
             return self._predict_tabular_data(new_data=X, process=True)
         else:
             raise ValueError("X must be of type pd.DataFrame or TabularTorchDataset, not type: %s" % type(X))
 
     def _predict_tabular_data(self, new_data, process=True):
         from .tabular_torch_dataset import TabularTorchDataset
+
         if process:
             new_data = self._process_test_data(new_data)
         if not isinstance(new_data, TabularTorchDataset):
             raise ValueError("new_data must of of type TabularTorchDataset if process=False")
         val_dataloader = new_data.build_loader(self.max_batch_size, self.num_dataloading_workers, is_test=True)
         preds_dataset = []
         for data_batch in val_dataloader:
@@ -425,149 +439,146 @@
             preds_dataset.append(preds_batch)
         preds_dataset = np.concatenate(preds_dataset, 0)
         return preds_dataset
 
     def _generate_datasets(self, X, y, params, X_val=None, y_val=None):
         from .tabular_torch_dataset import TabularTorchDataset
 
-        impute_strategy = params['proc.impute_strategy']
-        max_category_levels = params['proc.max_category_levels']
-        skew_threshold = params['proc.skew_threshold']
-        embed_min_categories = params['proc.embed_min_categories']
-        use_ngram_features = params['use_ngram_features']
+        impute_strategy = params["proc.impute_strategy"]
+        max_category_levels = params["proc.max_category_levels"]
+        skew_threshold = params["proc.skew_threshold"]
+        embed_min_categories = params["proc.embed_min_categories"]
+        use_ngram_features = params["use_ngram_features"]
 
         if isinstance(X, TabularTorchDataset):
             train_dataset = X
         else:
             X = self.preprocess(X)
-            train_dataset = self._process_train_data(df=X, labels=y,
-                                                     impute_strategy=impute_strategy,
-                                                     max_category_levels=max_category_levels,
-                                                     skew_threshold=skew_threshold,
-                                                     embed_min_categories=embed_min_categories,
-                                                     use_ngram_features=use_ngram_features)
+            train_dataset = self._process_train_data(
+                df=X,
+                labels=y,
+                impute_strategy=impute_strategy,
+                max_category_levels=max_category_levels,
+                skew_threshold=skew_threshold,
+                embed_min_categories=embed_min_categories,
+                use_ngram_features=use_ngram_features,
+            )
         if X_val is not None:
             if isinstance(X_val, TabularTorchDataset):
                 val_dataset = X_val
             else:
                 X_val = self.preprocess(X_val)
                 val_dataset = self._process_test_data(df=X_val, labels=y_val)
         else:
             val_dataset = None
         return train_dataset, val_dataset
 
     def _process_test_data(self, df, labels=None):
-        """ Process train or test DataFrame into a form fit for neural network models.
-            Args:
-                df (pd.DataFrame): Data to be processed (X)
-                labels (pd.Series): labels to be processed (y)
-            Returns:
-                Dataset object
+        """Process train or test DataFrame into a form fit for neural network models.
+        Args:
+            df (pd.DataFrame): Data to be processed (X)
+            labels (pd.Series): labels to be processed (y)
+        Returns:
+            Dataset object
         """
         from .tabular_torch_dataset import TabularTorchDataset
 
         # sklearn processing n_quantiles warning
-        warnings.filterwarnings("ignore", module='sklearn.preprocessing')
+        warnings.filterwarnings("ignore", module="sklearn.preprocessing")
         if labels is not None and len(labels) != len(df):
             raise ValueError("Number of examples in Dataframe does not match number of labels")
-        if (self.processor is None or self._types_of_features is None
-           or self.feature_arraycol_map is None or self.feature_type_map is None):
+        if self.processor is None or self._types_of_features is None or self.feature_arraycol_map is None or self.feature_type_map is None:
             raise ValueError("Need to process training data before test data")
         if self.features_to_drop:
             drop_cols = [col for col in df.columns if col in self.features_to_drop]
             if drop_cols:
                 df = df.drop(columns=drop_cols)
 
         # self.feature_arraycol_map, self.feature_type_map have been previously set while processing training data.
         df = self.processor.transform(df)
         return TabularTorchDataset(df, self.feature_arraycol_map, self.feature_type_map, self.problem_type, labels)
 
-    def _process_train_data(self, df, impute_strategy, max_category_levels, skew_threshold,
-                            embed_min_categories, use_ngram_features, labels):
+    def _process_train_data(self, df, impute_strategy, max_category_levels, skew_threshold, embed_min_categories, use_ngram_features, labels):
         from .tabular_torch_dataset import TabularTorchDataset
 
         # sklearn processing n_quantiles warning
-        warnings.filterwarnings("ignore", module='sklearn.preprocessing')
+        warnings.filterwarnings("ignore", module="sklearn.preprocessing")
         if labels is None:
             raise ValueError("Attempting process training data without labels")
         if len(labels) != len(df):
             raise ValueError("Number of examples in Dataframe does not match number of labels")
 
         # dict with keys: : 'continuous', 'skewed', 'onehot', 'embed', values = column-names of df
-        self._types_of_features, df = self._get_types_of_features(df, skew_threshold=skew_threshold,
-                                                                  embed_min_categories=embed_min_categories,
-                                                                  use_ngram_features=use_ngram_features)
+        self._types_of_features, df = self._get_types_of_features(
+            df, skew_threshold=skew_threshold, embed_min_categories=embed_min_categories, use_ngram_features=use_ngram_features
+        )
         logger.log(15, "Tabular Neural Network treats features as the following types:")
         logger.log(15, json.dumps(self._types_of_features, indent=4))
         logger.log(15, "\n")
         if self.processor is not None:
             Warning(f"Attempting to process training data for {self.__class__.__name__}, but previously already did this.")
         self.processor = create_preprocessor(
             impute_strategy=impute_strategy,
             max_category_levels=max_category_levels,
             unique_category_str=self.unique_category_str,
-            continuous_features=self._types_of_features['continuous'],
-            skewed_features=self._types_of_features['skewed'],
-            onehot_features=self._types_of_features['onehot'],
-            embed_features=self._types_of_features['embed'],
-            bool_features=self._types_of_features['bool']
+            continuous_features=self._types_of_features["continuous"],
+            skewed_features=self._types_of_features["skewed"],
+            onehot_features=self._types_of_features["onehot"],
+            embed_features=self._types_of_features["embed"],
+            bool_features=self._types_of_features["bool"],
         )
         df = self.processor.fit_transform(df)
         # OrderedDict of feature-name -> list of column-indices in df corresponding to this feature
         self.feature_arraycol_map = get_feature_arraycol_map(processor=self.processor, max_category_levels=max_category_levels)
         num_array_cols = np.sum([len(self.feature_arraycol_map[key]) for key in self.feature_arraycol_map])  # should match number of columns in processed array
         if num_array_cols != df.shape[1]:
-            raise ValueError("Error during one-hot encoding data processing for neural network. "
-                             "Number of columns in df array does not match feature_arraycol_map.")
+            raise ValueError(
+                "Error during one-hot encoding data processing for neural network. " "Number of columns in df array does not match feature_arraycol_map."
+            )
 
         # OrderedDict of feature-name -> feature_type string (options: 'vector', 'embed')
         self.feature_type_map = get_feature_type_map(feature_arraycol_map=self.feature_arraycol_map, types_of_features=self._types_of_features)
         return TabularTorchDataset(df, self.feature_arraycol_map, self.feature_type_map, self.problem_type, labels)
 
     def _init_optimizer(self, optimizer, learning_rate, weight_decay):
         """
         Set up optimizer needed for training.
         Network must first be initialized before this.
         """
         import torch
 
-        if optimizer == 'sgd':
-            optimizer = torch.optim.SGD(params=self.model.parameters(),
-                                        lr=learning_rate,
-                                        weight_decay=weight_decay)
-        elif optimizer == 'adam':
-            optimizer = torch.optim.Adam(params=self.model.parameters(),
-                                         lr=learning_rate,
-                                         weight_decay=weight_decay)
+        if optimizer == "sgd":
+            optimizer = torch.optim.SGD(params=self.model.parameters(), lr=learning_rate, weight_decay=weight_decay)
+        elif optimizer == "adam":
+            optimizer = torch.optim.Adam(params=self.model.parameters(), lr=learning_rate, weight_decay=weight_decay)
         else:
             raise ValueError(f"Unknown optimizer specified: {optimizer}")
         return optimizer
 
     def reduce_memory_size(self, remove_fit=True, requires_save=True, **kwargs):
         super().reduce_memory_size(remove_fit=remove_fit, requires_save=requires_save, **kwargs)
         if remove_fit and requires_save:
             self.optimizer = None
 
     def _get_default_stopping_metric(self):
         return self.eval_metric
-    
+
     def _get_maximum_resources(self) -> Dict[str, Union[int, float]]:
         # torch model trains slower when utilizing virtual cores and this issue scale up when the number of cpu cores increases
-        return {
-            "num_cpus": ResourceManager.get_cpu_count_psutil(logical=False)
-        }
+        return {"num_cpus": ResourceManager.get_cpu_count_psutil(logical=False)}
 
     def _get_default_resources(self):
         # logical=False is faster in training
         num_cpus = ResourceManager.get_cpu_count_psutil(logical=False)
         num_gpus = 0
         return num_cpus, num_gpus
 
     def save(self, path: str = None, verbose=True) -> str:
         import torch
+
         # Save on CPU to ensure the model can be loaded on a box without GPU
         if self.model is not None:
             self.model = self.model.to(torch.device("cpu"))
         path = super().save(path, verbose)
         # Put the model back to the device after the save
         if self.model is not None:
             self.model.to(self.device)
@@ -602,58 +613,57 @@
         import torch
 
         model: TabularNeuralNetTorchModel = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
 
         # Put the model on the same device it was train on (GPU/MPS) if it is available; otherwise use CPU
         if model.model is not None:
             original_device_type = model.device.type
-            if 'cuda' in original_device_type:
+            if "cuda" in original_device_type:
                 # cuda: nvidia GPU
-                device = torch.device(original_device_type if torch.cuda.is_available() else 'cpu')
-            elif 'mps' in original_device_type:
+                device = torch.device(original_device_type if torch.cuda.is_available() else "cpu")
+            elif "mps" in original_device_type:
                 # mps: Apple Silicon
-                device = torch.device(original_device_type if torch.backends.mps.is_available() else 'cpu')
+                device = torch.device(original_device_type if torch.backends.mps.is_available() else "cpu")
             else:
                 device = torch.device(original_device_type)
 
             if verbose and (original_device_type != device.type):
-                logger.log(15, f'Model is trained on {original_device_type}, but the device is not available - loading on {device.type}')
+                logger.log(15, f"Model is trained on {original_device_type}, but the device is not available - loading on {device.type}")
 
             model.device = device
             model.model = model.model.to(model.device)
             model.model.device = model.device
 
         # Compiled models handling
-        if hasattr(model, '_compiler') and model._compiler and model._compiler.name != 'native':
+        if hasattr(model, "_compiler") and model._compiler and model._compiler.name != "native":
             model.model.eval()
             model.processor = model._compiler.load(path=model.path)
         return model
-    
+
     def _get_hpo_backend(self):
         """Choose which backend(Ray or Custom) to use for hpo"""
         return RAY_BACKEND
 
     def get_minimum_resources(self, is_gpu_available=False):
         minimum_resources = {
-            'num_cpus': 1,
+            "num_cpus": 1,
         }
         if is_gpu_available:
             # Our custom implementation does not support partial GPU. No gpu usage according to nvidia-smi when the `num_gpus` passed to fit is fractional`
-            minimum_resources['num_gpus'] = 1
+            minimum_resources["num_gpus"] = 1
         return minimum_resources
 
     def _more_tags(self):
         # `can_refit_full=True` because batch_size and num_epochs is communicated at end of `_fit`:
         #  self.params_trained['batch_size'] = batch_size
         #  self.params_trained['num_epochs'] = best_epoch
-        return {'can_refit_full': True}
+        return {"can_refit_full": True}
 
     def _valid_compilers(self):
-        return [TabularNeuralNetTorchNativeCompiler,
-                TabularNeuralNetTorchOnnxCompiler]
+        return [TabularNeuralNetTorchNativeCompiler, TabularNeuralNetTorchOnnxCompiler]
 
     def _default_compiler(self):
         return TabularNeuralNetTorchNativeCompiler
 
     def _get_input_types(self, batch_size=None):
         input_types = []
         for f in self._features:
@@ -684,13 +694,12 @@
         This overrides the _compile() in AbstractModel, since we won't
         overwrite self.model in the compilation process.
         Instead, self.processor would be converted from sklearn ColumnTransformer
         to TabularNeuralNetTorchOnnxTransformer.
         """
         from sklearn.compose._column_transformer import ColumnTransformer
 
-        input_types = kwargs.get('input_types', self._get_input_types(batch_size=self.max_batch_size))
-        assert isinstance(self.processor, ColumnTransformer), f"unexpected processor type {type(self.processor)}, " \
-            "expecting processor type to be sklearn.compose._column_transformer.ColumnTransformer"
-        self.processor = self._compiler.compile(model=(self.processor, self.model),
-                                                path=self.path,
-                                                input_types=input_types)
+        input_types = kwargs.get("input_types", self._get_input_types(batch_size=self.max_batch_size))
+        assert isinstance(self.processor, ColumnTransformer), (
+            f"unexpected processor type {type(self.processor)}, " "expecting processor type to be sklearn.compose._column_transformer.ColumnTransformer"
+        )
+        self.processor = self._compiler.compile(model=(self.processor, self.model), path=self.path, input_types=input_types)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,133 +1,134 @@
-import os
 import logging
+import os
 
-import torch
 import numpy as np
+import torch
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
 logger = logging.getLogger(__name__)
 
 
 class TabularTorchDataset(torch.utils.data.IterableDataset):
     """
-        This class follows the structure of TabularNNDataset in tabular_nn_dataset.py,
+    This class follows the structure of TabularNNDataset in tabular_nn_dataset.py,
 
-        Class for preprocessing & storing/feeding data batches used by pytorch neural networks for tabular data.
-        Assumes entire dataset can be loaded into numpy arrays.
-        Original data table may contain numeric and categorical fields and missing values.
-
-        Attributes:
-            data_list (list[np.array]): Contains the raw data. Different indices in this list correspond to different
-                                        types of inputs to the neural network (each is 2D array). All vector-valued
-                                        (continuous & one-hot) features are concatenated together into a single index
-                                        of the dataset.
-            data_desc (list[str]): Describes the data type of each index of dataset
-                                   (options: 'vector','embed_<featname>')
-            embed_indices (list): which columns in dataset correspond to embed features (order matters!)
-            vecfeature_col_map (dict): maps vector_feature_name ->  columns of dataset._data[vector] array that
-                                       contain the data for this feature
-            feature_dataindex_map (dict): maps feature_name -> i such that dataset._data[i] = data array for
-                                          this feature. Cannot be used for vector-valued features,
-                                          instead use vecfeature_col_map
-            feature_groups (dict): maps feature_type (ie. 'vector' or 'embed') to list of feature
-                                   names of this type (empty list if there are no features of this type)
-            vectordata_index (int): describes which element of the dataset._data list holds the vector data matrix
-                                    (access via self.data_list[self.vectordata_index]); None if no vector features
-            label_index (int): describing which element of the dataset._data list holds labels
-                               (access via self.data_list[self.label_index]); None if no labels
-            num_categories_per_embedfeature (list): Number of categories for each embedding feature (order matters!)
-            num_examples (int): number of examples in this dataset
-            num_features (int): number of features (we only consider original variables as features, so num_features
-                                may not correspond to dimensionality of the data eg in the case of one-hot encoding)
-        Note: Default numerical data-type is converted to float32.
+    Class for preprocessing & storing/feeding data batches used by pytorch neural networks for tabular data.
+    Assumes entire dataset can be loaded into numpy arrays.
+    Original data table may contain numeric and categorical fields and missing values.
+
+    Attributes:
+        data_list (list[np.array]): Contains the raw data. Different indices in this list correspond to different
+                                    types of inputs to the neural network (each is 2D array). All vector-valued
+                                    (continuous & one-hot) features are concatenated together into a single index
+                                    of the dataset.
+        data_desc (list[str]): Describes the data type of each index of dataset
+                               (options: 'vector','embed_<featname>')
+        embed_indices (list): which columns in dataset correspond to embed features (order matters!)
+        vecfeature_col_map (dict): maps vector_feature_name ->  columns of dataset._data[vector] array that
+                                   contain the data for this feature
+        feature_dataindex_map (dict): maps feature_name -> i such that dataset._data[i] = data array for
+                                      this feature. Cannot be used for vector-valued features,
+                                      instead use vecfeature_col_map
+        feature_groups (dict): maps feature_type (ie. 'vector' or 'embed') to list of feature
+                               names of this type (empty list if there are no features of this type)
+        vectordata_index (int): describes which element of the dataset._data list holds the vector data matrix
+                                (access via self.data_list[self.vectordata_index]); None if no vector features
+        label_index (int): describing which element of the dataset._data list holds labels
+                           (access via self.data_list[self.label_index]); None if no labels
+        num_categories_per_embedfeature (list): Number of categories for each embedding feature (order matters!)
+        num_examples (int): number of examples in this dataset
+        num_features (int): number of features (we only consider original variables as features, so num_features
+                            may not correspond to dimensionality of the data eg in the case of one-hot encoding)
+    Note: Default numerical data-type is converted to float32.
     """
+
     # hard-coded names for files. This file contains pickled torch.util.data.Dataset object
-    DATAOBJ_SUFFIX = '_tabdataset_torch.pt'
+    DATAOBJ_SUFFIX = "_tabdataset_torch.pt"
 
     def __init__(self, processed_array, feature_arraycol_map, feature_type_map, problem_type, labels=None):
-        """ Args:
-            processed_array: 2D numpy array returned by preprocessor. Contains raw data of all features as columns
-            feature_arraycol_map (OrderedDict): Mapsfeature-name -> list of column-indices in processed_array
-                                                corresponding to this feature
-            feature_type_map (OrderedDict): Maps feature-name -> feature_type string
-                                            (options: 'vector', 'embed')
-            problem_type (str): what prediction task this data is used for.
-            labels (pd.Series): list of labels (y) if available
+        """Args:
+        processed_array: 2D numpy array returned by preprocessor. Contains raw data of all features as columns
+        feature_arraycol_map (OrderedDict): Mapsfeature-name -> list of column-indices in processed_array
+                                            corresponding to this feature
+        feature_type_map (OrderedDict): Maps feature-name -> feature_type string
+                                        (options: 'vector', 'embed')
+        problem_type (str): what prediction task this data is used for.
+        labels (pd.Series): list of labels (y) if available
         """
         self.problem_type = problem_type
         self.num_examples = processed_array.shape[0]
         self.num_features = len(feature_arraycol_map)
         if feature_arraycol_map.keys() != feature_type_map.keys():
             raise ValueError("feature_arraycol_map and feature_type_map must share same keys")
-        self.feature_groups = {'vector': [], 'embed': []}
+        self.feature_groups = {"vector": [], "embed": []}
         self.feature_type_map = feature_type_map
         for feature in feature_type_map:
-            if feature_type_map[feature] == 'vector':
-                self.feature_groups['vector'].append(feature)
-            elif feature_type_map[feature] == 'embed':
-                self.feature_groups['embed'].append(feature)
+            if feature_type_map[feature] == "vector":
+                self.feature_groups["vector"].append(feature)
+            elif feature_type_map[feature] == "embed":
+                self.feature_groups["embed"].append(feature)
             else:
                 raise ValueError("unknown feature type: %s" % feature)
         if labels is not None and len(labels) != self.num_examples:
             raise ValueError("number of labels and training examples do not match")
 
         self.data_desc = []
         self.data_list = []
         self.label_index = None
         self.vectordata_index = None
         self.vecfeature_col_map = {}
         self.feature_dataindex_map = {}
         self.num_classes = None
 
         # numerical data
-        if len(self.feature_groups['vector']) > 0:
+        if len(self.feature_groups["vector"]) > 0:
             vector_inds = []
             for feature in feature_type_map:
-                if feature_type_map[feature] == 'vector':
+                if feature_type_map[feature] == "vector":
                     current_last_ind = len(vector_inds)
                     vector_inds += feature_arraycol_map[feature]
                     new_last_ind = len(vector_inds)
                     self.vecfeature_col_map[feature] = list(range(current_last_ind, new_last_ind))
-            self.data_list.append(processed_array[:, vector_inds].astype('float32'))
-            self.data_desc.append('vector')
+            self.data_list.append(processed_array[:, vector_inds].astype("float32"))
+            self.data_desc.append("vector")
             self.vectordata_index = len(self.data_list) - 1
 
         # embedding data
-        if len(self.feature_groups['embed']) > 0:
+        if len(self.feature_groups["embed"]) > 0:
             for feature in feature_type_map:
-                if feature_type_map[feature] == 'embed':
+                if feature_type_map[feature] == "embed":
                     feature_colind = feature_arraycol_map[feature]
-                    self.data_list.append(processed_array[:, feature_colind].astype('int64').flatten())
-                    self.data_desc.append('embed')
+                    self.data_list.append(processed_array[:, feature_colind].astype("int64").flatten())
+                    self.data_desc.append("embed")
                     self.feature_dataindex_map[feature] = len(self.data_list) - 1
 
         # output (target) data
         if labels is not None:
             labels = np.array(labels)
             self.data_desc.append("label")
             self.label_index = len(self.data_list)
             if self.problem_type == SOFTCLASS:
                 self.num_classes = labels.shape[1]
-                self.data_list.append(labels.astype('float32'))
+                self.data_list.append(labels.astype("float32"))
             else:
                 if self.problem_type in [REGRESSION, QUANTILE] and labels.dtype != np.float32:
-                    labels = labels.astype('float32')  # Convert to proper float-type if not already
+                    labels = labels.astype("float32")  # Convert to proper float-type if not already
                 elif self.problem_type in [BINARY, MULTICLASS]:
                     self.num_classes = len(set(labels))
-                    labels = labels.astype('long')
+                    labels = labels.astype("long")
                 self.data_list.append(labels.reshape(-1, 1))
 
-        self.embed_indices = [i for i in range(len(self.data_desc)) if 'embed' in self.data_desc[i]]
+        self.embed_indices = [i for i in range(len(self.data_desc)) if "embed" in self.data_desc[i]]
         self.num_categories_per_embed_feature = None
         self.num_categories_per_embedfeature = self.getNumCategoriesEmbeddings()
 
         self.has_vector_features = self.vectordata_index is not None
-        self.has_embed_features = len(self.feature_groups['embed']) > 0
+        self.has_embed_features = len(self.feature_groups["embed"]) > 0
 
     def __iter__(self):
         """
         Iterate through the iterable dataset, and return a subsample of it.
 
         This overrides the `__iter__` function in IterableDataset.
         This is typically useful when we are using :class:`torch.utils.data.DataLoader` to
@@ -166,87 +167,86 @@
                 output_list.append(self.data_list[self.label_index][idx])
             yield tuple(output_list)
 
     def __len__(self):
         return self.num_examples
 
     def has_vector_features(self):
-        """ Returns boolean indicating whether this dataset contains vector features """
+        """Returns boolean indicating whether this dataset contains vector features"""
         return self.vectordata_index is not None
 
     def num_embed_features(self):
-        """ Returns number of embed features in this dataset """
-        return len(self.feature_groups['embed'])
+        """Returns number of embed features in this dataset"""
+        return len(self.feature_groups["embed"])
 
     def num_vector_features(self):
-        """ Number of vector features (each onehot feature counts = 1, regardless of how many categories) """
-        return len(self.feature_groups['vector'])
+        """Number of vector features (each onehot feature counts = 1, regardless of how many categories)"""
+        return len(self.feature_groups["vector"])
 
     def get_labels(self):
-        """ Returns numpy array of labels for this dataset """
+        """Returns numpy array of labels for this dataset"""
         if self.label_index is not None:
             return self.data_list[self.label_index]
         else:
             return None
 
     def getNumCategoriesEmbeddings(self):
-        """ Returns number of categories for each embedding feature.
-            Should only be applied to training data.
-            If training data feature contains unique levels 1,...,n-1, there are actually n categories,
-            since category n is reserved for unknown test-time categories.
+        """Returns number of categories for each embedding feature.
+        Should only be applied to training data.
+        If training data feature contains unique levels 1,...,n-1, there are actually n categories,
+        since category n is reserved for unknown test-time categories.
         """
         if self.num_categories_per_embed_feature is not None:
             return self.num_categories_per_embedfeature
         else:
             num_embed_feats = self.num_embed_features()
             num_categories_per_embedfeature = [0] * num_embed_feats
             for i in range(num_embed_feats):
-                feat_i = self.feature_groups['embed'][i]
+                feat_i = self.feature_groups["embed"][i]
                 feat_i_data = self.get_feature_data(feat_i).flatten().tolist()
-                num_categories_i = len(set(feat_i_data)) # number of categories for ith feature
-                num_categories_per_embedfeature[i] = num_categories_i + 1 # to account for unknown test-time categories
+                num_categories_i = len(set(feat_i_data))  # number of categories for ith feature
+                num_categories_per_embedfeature[i] = num_categories_i + 1  # to account for unknown test-time categories
             return num_categories_per_embedfeature
 
     def get_feature_data(self, feature):
-        """ Returns all data for this feature.
-            Args:
-                feature (str): name of feature of interest (in processed dataframe)
+        """Returns all data for this feature.
+        Args:
+            feature (str): name of feature of interest (in processed dataframe)
         """
-        nonvector_featuretypes = set(['embed'])
+        nonvector_featuretypes = set(["embed"])
         if feature not in self.feature_type_map:
             raise ValueError("unknown feature encountered: %s" % feature)
-        if self.feature_type_map[feature] == 'vector':
+        if self.feature_type_map[feature] == "vector":
             vector_datamatrix = self.data_list[self.vectordata_index]
             feature_data = vector_datamatrix[:, self.vecfeature_col_map[feature]]
         elif self.feature_type_map[feature] in nonvector_featuretypes:
             feature_idx = self.feature_dataindex_map[feature]
             feature_data = self.data_list[feature_idx]
         else:
             raise ValueError("Unknown feature specified: " % feature)
         return feature_data
 
     def save(self, file_prefix=""):
-        """ Additional naming changes will be appended to end of file_prefix (must contain full absolute path) """
+        """Additional naming changes will be appended to end of file_prefix (must contain full absolute path)"""
         dataobj_file = file_prefix + self.DATAOBJ_SUFFIX
         if not os.path.exists(os.path.dirname(dataobj_file)):
             os.makedirs(os.path.dirname(dataobj_file))
         torch.save(self, dataobj_file)
         logger.debug("TabularPyTorchDataset Dataset saved to a file: \n %s" % dataobj_file)
 
     @classmethod
     def load(cls, file_prefix=""):
-        """ Additional naming changes will be appended to end of file_prefix (must contain full absolute path) """
+        """Additional naming changes will be appended to end of file_prefix (must contain full absolute path)"""
         dataobj_file = file_prefix + cls.DATAOBJ_SUFFIX
         dataset: TabularTorchDataset = torch.load(dataobj_file)
         logger.debug("TabularNN Dataset loaded from a file: \n %s" % dataobj_file)
         return dataset
 
     def build_loader(self, batch_size, num_workers, is_test=False):
         def worker_init_fn(worker_id):
             np.random.seed(np.random.get_state()[1][0] + worker_id)
+
         self.batch_size = batch_size
         self.shuffle = False if is_test else True
         self.drop_last = False if is_test else True
-        loader = torch.utils.data.DataLoader(self, num_workers=num_workers,
-                                             batch_size=None, # no collation
-                                             worker_init_fn=worker_init_fn)
+        loader = torch.utils.data.DataLoader(self, num_workers=num_workers, batch_size=None, worker_init_fn=worker_init_fn)  # no collation
         return loader
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,143 +1,142 @@
 import logging
+
+import numpy as np
 import torch
 import torch.nn as nn
-import numpy as np
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
 from ..utils.nn_architecture_utils import get_embed_sizes
 
 logger = logging.getLogger(__name__)
 
 
 class EmbedNet(nn.Module):
     """
     y_range: Used specifically for regression. = None for classification.
     """
-    def __init__(self,
-                 problem_type,
-                 num_net_outputs=None,
-                 quantile_levels=None,
-                 train_dataset=None,
-                 architecture_desc=None,
-                 device=None,
-                 **kwargs):
+
+    def __init__(self, problem_type, num_net_outputs=None, quantile_levels=None, train_dataset=None, architecture_desc=None, device=None, **kwargs):
         if (architecture_desc is None) and (train_dataset is None):
             raise ValueError("train_dataset cannot = None if architecture_desc=None")
         super().__init__()
         self.problem_type = problem_type
-        if self. problem_type == QUANTILE:
-            self.register_buffer('quantile_levels', torch.Tensor(quantile_levels).float().reshape(1, -1))
-        self.device = torch.device('cpu') if device is None else device
+        if self.problem_type == QUANTILE:
+            self.register_buffer("quantile_levels", torch.Tensor(quantile_levels).float().reshape(1, -1))
+        self.device = torch.device("cpu") if device is None else device
         if architecture_desc is None:
             params = self._set_params(**kwargs)
             # adpatively specify network architecture based on training dataset
             self.from_logits = False
             self.has_vector_features = train_dataset.has_vector_features
             self.has_embed_features = train_dataset.has_embed_features
             if self.has_embed_features:
                 num_categs_per_feature = train_dataset.getNumCategoriesEmbeddings()
                 embed_dims = get_embed_sizes(train_dataset, params, num_categs_per_feature)
             if self.has_vector_features:
                 vector_dims = train_dataset.data_list[train_dataset.vectordata_index].shape[-1]
         else:
             # ignore train_dataset, params, etc. Recreate architecture based on description:
             self.architecture_desc = architecture_desc
-            self.has_vector_features = architecture_desc['has_vector_features']
-            self.has_embed_features = architecture_desc['has_embed_features']
-            self.from_logits = architecture_desc['from_logits']
-            params = architecture_desc['params']
+            self.has_vector_features = architecture_desc["has_vector_features"]
+            self.has_embed_features = architecture_desc["has_embed_features"]
+            self.from_logits = architecture_desc["from_logits"]
+            params = architecture_desc["params"]
             if self.has_embed_features:
-                num_categs_per_feature = architecture_desc['num_categs_per_feature']
-                embed_dims = architecture_desc['embed_dims']
+                num_categs_per_feature = architecture_desc["num_categs_per_feature"]
+                embed_dims = architecture_desc["embed_dims"]
             if self.has_vector_features:
-                vector_dims = architecture_desc['vector_dims']
+                vector_dims = architecture_desc["vector_dims"]
         # init input size
         input_size = 0
 
         # define embedding layer:
         if self.has_embed_features:
             self.embed_blocks = nn.ModuleList()
             for i in range(len(num_categs_per_feature)):
-                self.embed_blocks.append(nn.Embedding(num_embeddings=num_categs_per_feature[i],
-                                                      embedding_dim=embed_dims[i]))
+                self.embed_blocks.append(nn.Embedding(num_embeddings=num_categs_per_feature[i], embedding_dim=embed_dims[i]))
                 input_size += embed_dims[i]
 
         # update input size
         if self.has_vector_features:
             input_size += vector_dims
 
         # activation
         act_fn = nn.Identity()
-        if params['activation'] == 'elu':
+        if params["activation"] == "elu":
             act_fn = nn.ELU()
-        elif params['activation'] == 'relu':
+        elif params["activation"] == "relu":
             act_fn = nn.ReLU()
-        elif params['activation'] == 'tanh':
+        elif params["activation"] == "tanh":
             act_fn = nn.Tanh()
 
         layers = []
-        if params['use_batchnorm']:
+        if params["use_batchnorm"]:
             layers.append(nn.BatchNorm1d(input_size))
-        layers.append(nn.Linear(input_size, params['hidden_size']))
+        layers.append(nn.Linear(input_size, params["hidden_size"]))
         layers.append(act_fn)
-        for _ in range(params['num_layers'] - 1):
-            if params['use_batchnorm']:
-                layers.append(nn.BatchNorm1d(params['hidden_size']))
-            layers.append(nn.Dropout(params['dropout_prob']))
-            layers.append(nn.Linear(params['hidden_size'], params['hidden_size']))
+        for _ in range(params["num_layers"] - 1):
+            if params["use_batchnorm"]:
+                layers.append(nn.BatchNorm1d(params["hidden_size"]))
+            layers.append(nn.Dropout(params["dropout_prob"]))
+            layers.append(nn.Linear(params["hidden_size"], params["hidden_size"]))
             layers.append(act_fn)
-        layers.append(nn.Linear(params['hidden_size'], num_net_outputs))
+        layers.append(nn.Linear(params["hidden_size"], num_net_outputs))
         self.main_block = nn.Sequential(*layers)
 
         if self.problem_type in [REGRESSION, QUANTILE]:  # set range for output
-            y_range = params['y_range']  # Used specifically for regression. = None for classification.
+            y_range = params["y_range"]  # Used specifically for regression. = None for classification.
             self.y_constraint = None  # determines if Y-predictions should be constrained
             if y_range is not None:
                 if y_range[0] == -np.inf and y_range[1] == np.inf:
                     self.y_constraint = None  # do not worry about Y-range in this case
                 elif y_range[0] >= 0 and y_range[1] == np.inf:
-                    self.y_constraint = 'nonnegative'
+                    self.y_constraint = "nonnegative"
                 elif y_range[0] == -np.inf and y_range[1] <= 0:
-                    self.y_constraint = 'nonpositive'
+                    self.y_constraint = "nonpositive"
                 else:
-                    self.y_constraint = 'bounded'
+                    self.y_constraint = "bounded"
                 self.y_lower = y_range[0]
                 self.y_upper = y_range[1]
                 self.y_span = self.y_upper - self.y_lower
 
         if self.problem_type == QUANTILE:
-            self.alpha = params['alpha']  # for huber loss
+            self.alpha = params["alpha"]  # for huber loss
         if self.problem_type == SOFTCLASS:
             self.log_softmax = torch.nn.LogSoftmax(dim=1)
         if self.problem_type in [BINARY, MULTICLASS, SOFTCLASS]:
             self.softmax = torch.nn.Softmax(dim=1)
         if architecture_desc is None:  # Save Architecture description
-            self.architecture_desc = {'has_vector_features': self.has_vector_features,
-                                      'has_embed_features': self.has_embed_features,
-                                      'params': params, 'num_net_outputs': num_net_outputs,
-                                      'from_logits': self.from_logits}
+            self.architecture_desc = {
+                "has_vector_features": self.has_vector_features,
+                "has_embed_features": self.has_embed_features,
+                "params": params,
+                "num_net_outputs": num_net_outputs,
+                "from_logits": self.from_logits,
+            }
             if self.has_embed_features:
-                self.architecture_desc['num_categs_per_feature'] = num_categs_per_feature
-                self.architecture_desc['embed_dims'] = embed_dims
+                self.architecture_desc["num_categs_per_feature"] = num_categs_per_feature
+                self.architecture_desc["embed_dims"] = embed_dims
             if self.has_vector_features:
-                self.architecture_desc['vector_dims'] = vector_dims
+                self.architecture_desc["vector_dims"] = vector_dims
 
-    def _set_params(self,
-                    num_layers=4,
-                    hidden_size=128,
-                    activation='relu',
-                    use_batchnorm=False,
-                    dropout_prob=0.1,
-                    y_range=None,
-                    alpha=0.01,
-                    max_embedding_dim=100,
-                    embed_exponent=0.56,
-                    embedding_size_factor=1.0):
+    def _set_params(
+        self,
+        num_layers=4,
+        hidden_size=128,
+        activation="relu",
+        use_batchnorm=False,
+        dropout_prob=0.1,
+        y_range=None,
+        alpha=0.01,
+        max_embedding_dim=100,
+        embed_exponent=0.56,
+        embedding_size_factor=1.0,
+    ):
         return dict(
             num_layers=num_layers,
             hidden_size=hidden_size,
             activation=activation,
             use_batchnorm=use_batchnorm,
             dropout_prob=dropout_prob,
             y_range=y_range,
@@ -145,15 +144,15 @@
             max_embedding_dim=max_embedding_dim,
             embed_exponent=embed_exponent,
             embedding_size_factor=embedding_size_factor,
         )
 
     def init_params(self):
         for layer in self.children():
-            if hasattr(layer, 'reset_parameters'):
+            if hasattr(layer, "reset_parameters"):
                 layer.reset_parameters()
 
     def forward(self, data_batch):
         input_data = []
         input_offset = 0
         if self.has_vector_features:
             input_data.append(data_batch[0].to(self.device))
@@ -169,38 +168,34 @@
             input_data = input_data[0]
 
         output_data = self.main_block(input_data)
         if self.problem_type in [REGRESSION, QUANTILE]:  # output with y-range
             if self.y_constraint is None:
                 return output_data
             else:
-                if self.y_constraint == 'nonnegative':
+                if self.y_constraint == "nonnegative":
                     return self.y_lower + torch.abs(output_data)
-                elif self.y_constraint == 'nonpositive':
+                elif self.y_constraint == "nonpositive":
                     return self.y_upper - torch.abs(output_data)
                 else:
                     return torch.sigmoid(output_data) * self.y_span + self.y_lower
         elif self.problem_type == SOFTCLASS:
             return self.log_softmax(output_data)  # KLDivLoss takes in log-probabilities as predictions.
         else:
             return output_data
 
     def huber_pinball_loss(self, input_data, target_data):
         error_data = target_data.contiguous().reshape(-1, 1) - input_data
         if self.alpha == 0.0:
             loss_data = torch.max(self.quantile_levels * error_data, (self.quantile_levels - 1) * error_data)
             return loss_data.mean()
 
-        loss_data = torch.where(torch.abs(error_data) < self.alpha,
-                                0.5 * error_data * error_data,
-                                self.alpha * (torch.abs(error_data) - 0.5 * self.alpha))
+        loss_data = torch.where(torch.abs(error_data) < self.alpha, 0.5 * error_data * error_data, self.alpha * (torch.abs(error_data) - 0.5 * self.alpha))
         loss_data /= self.alpha
-        scale = torch.where(error_data >= 0,
-                            torch.ones_like(error_data) * self.quantile_levels,
-                            torch.ones_like(error_data) * (1 - self.quantile_levels))
+        scale = torch.where(error_data >= 0, torch.ones_like(error_data) * self.quantile_levels, torch.ones_like(error_data) * (1 - self.quantile_levels))
         loss_data *= scale
         return loss_data.mean()
 
     def margin_loss(self, input_data, margin_scale=0.0001):
         # number of samples
         batch_size, num_quantiles = input_data.size()
 
@@ -238,21 +233,20 @@
             return loss_function(predict_data, target_data)
         else:
             target_data = target_data.flatten()
             if self.problem_type == REGRESSION:
                 predict_data = predict_data.flatten()
             return loss_function(predict_data, target_data)
 
-
     def predict(self, input_data):
         self.eval()
         with torch.no_grad():
             predict_data = self(input_data)
             if self.problem_type == QUANTILE:
                 predict_data = torch.sort(predict_data, -1)[0]  # sorting ensures monotonicity of quantile estimates
             elif self.problem_type in [BINARY, MULTICLASS, SOFTCLASS]:
                 predict_data = self.softmax(predict_data)  # convert NN output to probability
             elif self.problem_type == REGRESSION:
                 predict_data = predict_data.flatten()
             if self.problem_type == BINARY:
-                predict_data = predict_data[:,1]
+                predict_data = predict_data[:, 1]
             return predict_data.data.cpu().numpy()
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,21 @@
 Unknown categories are returned as None in inverse transforms. Always converts input list X to list of the same type elements first (string typically)
 """
 import copy
 from numbers import Integral
 
 import numpy as np
 from scipy import sparse
-
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
 
 from autogluon.features.generators import LabelEncoderFeatureGenerator
 
-
-__all__ = [
-    'OneHotMergeRaresHandleUnknownEncoder',
-    'OrdinalMergeRaresHandleUnknownEncoder'
-]
+__all__ = ["OneHotMergeRaresHandleUnknownEncoder", "OrdinalMergeRaresHandleUnknownEncoder"]
 
 
 def _encode_numpy(values, uniques=None, encode=False, check_unknown=True):
     # only used in _encode below, see docstring there for details
     if uniques is None:
         if encode:
             uniques, encoded = np.unique(values, return_inverse=True)
@@ -31,16 +26,15 @@
         else:
             # unique sorts
             return np.unique(values)
     if encode:
         if check_unknown:
             diff = _encode_check_unknown(values, uniques)
             if diff:
-                raise ValueError("y contains previously unseen labels: %s"
-                                 % str(diff))
+                raise ValueError("y contains previously unseen labels: %s" % str(diff))
         encoded = np.searchsorted(uniques, values)
         return uniques, encoded
     else:
         return uniques
 
 
 def _encode_python(values, uniques=None, encode=False):
@@ -49,16 +43,15 @@
         uniques = sorted(set(values))
         uniques = np.array(uniques, dtype=values.dtype)
     if encode:
         table = {val: i for i, val in enumerate(uniques)}
         try:
             encoded = np.array([table[v] for v in values])
         except KeyError as e:
-            raise ValueError("y contains previously unseen labels: %s"
-                             % str(e))
+            raise ValueError("y contains previously unseen labels: %s" % str(e))
         return uniques, encoded
     else:
         return uniques
 
 
 def _encode(values, uniques=None, encode=False, check_unknown=True):
     """Helper function to factorize (find uniques) and encode values.
@@ -95,16 +88,15 @@
     if values.dtype == object:
         try:
             res = _encode_python(values, uniques, encode)
         except TypeError:
             raise TypeError("argument must be a string or number")
         return res
     else:
-        return _encode_numpy(values, uniques, encode,
-                             check_unknown=check_unknown)
+        return _encode_numpy(values, uniques, encode, check_unknown=check_unknown)
 
 
 def _encode_check_unknown(values, uniques, return_mask=False):
     """
     Helper function to check for unknowns in values to be encoded.
     Uses pure python method for object dtype, and numpy method for
     all other dtypes.
@@ -150,151 +142,143 @@
 
 
 class _BaseEncoder(BaseEstimator, TransformerMixin):
     """
     Base class for encoders that includes the code to categorize and
     transform the input features.
     """
-    
+
     def _check_X(self, X):
         """
         Perform custom check_array:
         - convert list of strings to object dtype
         - check for missing values for object dtype data (check_array does
           not do that)
         - return list of features (arrays): this list of features is
           constructed feature by feature to preserve the data types
           of pandas DataFrame columns, as otherwise information is lost
           and cannot be used, eg for the `categories_` attribute.
-        
+
         """
-        if not (hasattr(X, 'iloc') and getattr(X, 'ndim', 0) == 2):
+        if not (hasattr(X, "iloc") and getattr(X, "ndim", 0) == 2):
             # if not a dataframe, do normal check_array validation
             X_temp = check_array(X, dtype=None, force_all_finite=False)
-            if (not hasattr(X, 'dtype')
-                    and np.issubdtype(X_temp.dtype, np.str_)):
+            if not hasattr(X, "dtype") and np.issubdtype(X_temp.dtype, np.str_):
                 X = check_array(X, dtype=object)
             else:
                 X = X_temp
             needs_validation = False
         else:
             # pandas dataframe, do validation later column by column, in order
             # to keep the dtype information to be used in the encoder.
             needs_validation = True
-        
+
         n_samples, n_features = X.shape
         X_columns = []
-        
+
         for i in range(n_features):
             Xi = self._get_feature(X, feature_idx=i)
-            Xi = check_array(Xi, ensure_2d=False, dtype=None,
-                             force_all_finite=needs_validation)
+            Xi = check_array(Xi, ensure_2d=False, dtype=None, force_all_finite=needs_validation)
             X_columns.append(Xi)
-        
+
         return X_columns, n_samples, n_features
-    
+
     def _get_feature(self, X, feature_idx):
-        if hasattr(X, 'iloc'):
+        if hasattr(X, "iloc"):
             # pandas dataframes
             return X.iloc[:, feature_idx]
         # numpy arrays, sparse arrays
         return X[:, feature_idx]
-    
-    def _fit(self, X, handle_unknown='error'):
+
+    def _fit(self, X, handle_unknown="error"):
         X_list, n_samples, n_features = self._check_X(X)
-        
-        if self.categories != 'auto':
+
+        if self.categories != "auto":
             if len(self.categories) != n_features:
-                raise ValueError("Shape mismatch: if categories is an array,"
-                                 " it has to be of shape (n_features,).")
-        
+                raise ValueError("Shape mismatch: if categories is an array," " it has to be of shape (n_features,).")
+
         if self.max_levels is not None:
-            if (not isinstance(self.max_levels, Integral) or
-                    self.max_levels <= 0):
-                raise ValueError("max_levels must be None or a strictly "
-                                 "positive int, got {}.".format(
-                                     self.max_levels))
-        
+            if not isinstance(self.max_levels, Integral) or self.max_levels <= 0:
+                raise ValueError("max_levels must be None or a strictly " "positive int, got {}.".format(self.max_levels))
+
         self.categories_ = []
         self.infrequent_indices_ = []
-        
+
         for i in range(n_features):
             Xi = X_list[i]
-            if self.categories == 'auto':
+            if self.categories == "auto":
                 cats = _encode(Xi)
             else:
                 cats = np.array(self.categories[i], dtype=Xi.dtype)
                 if Xi.dtype != object:
                     if not np.all(np.sort(cats) == cats):
-                        raise ValueError("Unsorted categories are not "
-                                         "supported for numerical categories")
-                if handle_unknown == 'error':
+                        raise ValueError("Unsorted categories are not " "supported for numerical categories")
+                if handle_unknown == "error":
                     diff = _encode_check_unknown(Xi, cats)
                     if diff:
-                        msg = ("Found unknown categories {0} in column {1}"
-                               " during fit".format(diff, i))
+                        msg = "Found unknown categories {0} in column {1}" " during fit".format(diff, i)
                         raise ValueError(msg)
             self.categories_.append(cats)
-            
+
             if self.max_levels is not None:
                 infrequent_indices = self._find_infrequent_category_indices(Xi)
             else:
                 infrequent_indices = np.array([])
             self.infrequent_indices_.append(infrequent_indices)
-    
+
     def _find_infrequent_category_indices(self, Xi):
         # TODO: this is using unique on X again. Ideally we should integrate
         # this into _encode()
         _, counts = np.unique(Xi, return_counts=True)
-        return np.argsort(counts)[:-self.max_levels]
-    
-    def _transform(self, X, handle_unknown='error'):
+        return np.argsort(counts)[: -self.max_levels]
+
+    def _transform(self, X, handle_unknown="error"):
         X_list, n_samples, n_features = self._check_X(X)
-        
+
         X_int = np.zeros((n_samples, n_features), dtype=int)
         X_mask = np.ones((n_samples, n_features), dtype=bool)
-        
+
         if n_features != len(self.categories_):
             raise ValueError(
                 "The number of features in X is different to the number of "
                 "features of the fitted data. The fitted data had {} features "
-                "and the X has {} features."
-                .format(len(self.categories_,), n_features)
+                "and the X has {} features.".format(
+                    len(
+                        self.categories_,
+                    ),
+                    n_features,
+                )
             )
-        
+
         for i in range(n_features):
             Xi = X_list[i]
-            diff, valid_mask = _encode_check_unknown(Xi, self.categories_[i],
-                                                     return_mask=True)
-            
+            diff, valid_mask = _encode_check_unknown(Xi, self.categories_[i], return_mask=True)
+
             if not np.all(valid_mask):
-                if handle_unknown == 'error':
-                    msg = ("Found unknown categories {0} in column {1}"
-                           " during transform".format(diff, i))
+                if handle_unknown == "error":
+                    msg = "Found unknown categories {0} in column {1}" " during transform".format(diff, i)
                     raise ValueError(msg)
                 else:
                     # Set the problematic rows to an acceptable value and
                     # continue `The rows are marked `X_mask` and will be
                     # removed later.
                     X_mask[:, i] = valid_mask
                     # cast Xi into the largest string type necessary
                     # to handle different lengths of numpy strings
-                    if (self.categories_[i].dtype.kind in ('U', 'S')
-                            and self.categories_[i].itemsize > Xi.itemsize):
+                    if self.categories_[i].dtype.kind in ("U", "S") and self.categories_[i].itemsize > Xi.itemsize:
                         Xi = Xi.astype(self.categories_[i].dtype)
                     else:
                         Xi = Xi.copy()
-                    
+
                     Xi[~valid_mask] = self.categories_[i][0]
             # We use check_unknown=False, since _encode_check_unknown was
             # already called above.
-            _, encoded = _encode(Xi, self.categories_[i], encode=True,
-                                 check_unknown=False)
+            _, encoded = _encode(Xi, self.categories_[i], encode=True, check_unknown=False)
             X_int[:, i] = encoded
-        
+
         # We need to take care of infrequent categories here. We want all the
         # infrequent categories to end up in a specific column, after all the
         # frequent ones. Let's say we have 4 categories with 2 infrequent
         # categories (and 2 frequent categories): we want the value in X_int
         # for the infrequent categories to be 2 (third and last column), and
         # the values for the frequent ones to be 0 and 1. The piece of code
         # below performs this mapping.
@@ -305,39 +289,39 @@
             if self.infrequent_indices_[feature_idx].size > 0:
                 mapping = np.arange(len(self.categories_[feature_idx]))
                 # Trick: set the infrequent cats columns to a very big int and
                 # encode again.
                 for ordinal_cat in self.infrequent_indices_[feature_idx]:
                     mapping[ordinal_cat] = huge_int
                 _, mapping = _encode_numpy(mapping, encode=True)
-                
+
                 # update X_int and save mapping for later (for dropping logic)
                 X_int[:, feature_idx] = mapping[X_int[:, feature_idx]]
                 self._infrequent_mappings[feature_idx] = mapping
-        
+
         return X_int, X_mask
-    
+
     def _more_tags(self):
-        return {'X_types': ['categorical']}
+        return {"X_types": ["categorical"]}
 
 
 class OneHotMergeRaresHandleUnknownEncoder(_BaseEncoder):
     """Encode categorical integer features as a one-hot numeric array.
-    
+
     The input to this transformer should be an array-like of integers or
     strings, denoting the values taken on by categorical (discrete) features.
     The features are encoded using a one-hot (aka 'one-of-K' or 'dummy')
     encoding scheme. This creates a binary column for each category and
     returns a sparse matrix or dense array (depending on the ``sparse``
     parameter)
-    
+
     By default, the encoder derives the categories based on the unique values
     in each feature. Alternatively, you can also specify the `categories`
     manually.
-    
+
     Always uses handle_unknown='ignore' which maps unknown test-time categories to all zeros vector.
 
     Parameters
     ----------
     categories : 'auto' or a list of lists/arrays of values, default='auto'.
         Categories (unique values) per feature:
 
@@ -366,20 +350,20 @@
           ``max_levels`` parameter).
 
     sparse : boolean, default=True
         Will return sparse matrix if set True else will return an array.
 
     dtype : number type, default=float
         Desired dtype of output.
-        
+
     max_levels : int, default=None
-        One less than the maximum number of categories to keep (max_levels = 2 means we keep 3 distinct categories). 
+        One less than the maximum number of categories to keep (max_levels = 2 means we keep 3 distinct categories).
         Infrequent categories are grouped together and mapped into a single column, which counts as extra category.
         Unknown categories encountered at test time are mapped to all zeros vector.
-    
+
     Attributes
     ----------
     categories_ : list of arrays
         The categories of each feature determined during fitting
         (in order of the features in X and corresponding with the output
         of ``transform``). This includes the category specified in ``drop``
         (if any).
@@ -390,140 +374,122 @@
         be retained.
 
     infrequent_indices_: list of arrays of shape(n_infrequent_categories)
         ``infrequent_indices_[i]`` contains a list of indices in
         ``categories_[i]`` corresponding to the infrequent categories.
 
     """
-    
-    def __init__(self, categories='auto', drop=None, sparse=True,
-                 dtype=np.float64, max_levels=None):
+
+    def __init__(self, categories="auto", drop=None, sparse=True, dtype=np.float64, max_levels=None):
         self.categories = categories
         self.sparse = sparse
         self.dtype = dtype
-        self.handle_unknown = 'ignore'
+        self.handle_unknown = "ignore"
         self.drop = drop
         self.max_levels = max_levels
         self._label_encoder = None
         self._cat_cols = None
-    
+
     def _validate_keywords(self):
-        if self.handle_unknown not in ('error', 'ignore'):
-            msg = ("handle_unknown should be either 'error' or 'ignore', "
-                   "got {0}.".format(self.handle_unknown))
+        if self.handle_unknown not in ("error", "ignore"):
+            msg = "handle_unknown should be either 'error' or 'ignore', " "got {0}.".format(self.handle_unknown)
             raise ValueError(msg)
         # If we have both dropped columns and ignored unknown
         # values, there will be ambiguous cells. This creates difficulties
         # in interpreting the model.
-        if self.drop is not None and self.handle_unknown != 'error':
-            raise ValueError(
-                "`handle_unknown` must be 'error' when the drop parameter is "
-                "specified, as both would create categories that are all "
-                "zero.")
-    
+        if self.drop is not None and self.handle_unknown != "error":
+            raise ValueError("`handle_unknown` must be 'error' when the drop parameter is " "specified, as both would create categories that are all " "zero.")
+
     def _compute_drop_idx(self):
         if self.drop is None:
             return None
-        elif (isinstance(self.drop, str) and
-                self.drop in ('first', 'infrequent')):
+        elif isinstance(self.drop, str) and self.drop in ("first", "infrequent"):
             return np.zeros(len(self.categories_), dtype=np.int_)
         elif not isinstance(self.drop, str):
             try:
                 self.drop = np.asarray(self.drop, dtype=object)
                 droplen = len(self.drop)
             except (ValueError, TypeError):
-                msg = ("Wrong input for parameter `drop`. Expected "
-                       "'first', None or array of objects, got {}")
+                msg = "Wrong input for parameter `drop`. Expected " "'first', None or array of objects, got {}"
                 raise ValueError(msg.format(type(self.drop)))
             if droplen != len(self.categories_):
-                msg = ("`drop` should have length equal to the number "
-                       "of features ({}), got {}")
-                raise ValueError(msg.format(len(self.categories_),
-                                            len(self.drop)))
-            missing_drops = [(i, val) for i, val in enumerate(self.drop)
-                             if val not in self.categories_[i]]
+                msg = "`drop` should have length equal to the number " "of features ({}), got {}"
+                raise ValueError(msg.format(len(self.categories_), len(self.drop)))
+            missing_drops = [(i, val) for i, val in enumerate(self.drop) if val not in self.categories_[i]]
             if any(missing_drops):
-                msg = ("The following categories were supposed to be "
-                       "dropped, but were not found in the training "
-                       "data.\n{}".format(
-                           "\n".join(
-                                ["Category: {}, Feature: {}".format(c, v)
-                                    for c, v in missing_drops])))
+                msg = (
+                    "The following categories were supposed to be "
+                    "dropped, but were not found in the training "
+                    "data.\n{}".format("\n".join(["Category: {}, Feature: {}".format(c, v) for c, v in missing_drops]))
+                )
                 raise ValueError(msg)
-            return np.array([np.where(cat_list == val)[0][0]
-                             for (val, cat_list) in
-                             zip(self.drop, self.categories_)], dtype=np.int_)
+            return np.array([np.where(cat_list == val)[0][0] for (val, cat_list) in zip(self.drop, self.categories_)], dtype=np.int_)
         else:
-            msg = ("Wrong input for parameter `drop`. Expected "
-                   "'first', None or array of objects, got {}")
+            msg = "Wrong input for parameter `drop`. Expected " "'first', None or array of objects, got {}"
             raise ValueError(msg.format(type(self.drop)))
 
     def _convert_cat_to_int(self, X):
         if self._cat_cols:
             X = copy.deepcopy(X)
             X[self._cat_cols] = self._label_encoder.transform(X[self._cat_cols])
         return X
 
     def fit(self, X, y=None):
         """Fit OneHotEncoder to X.
-    
+
         Parameters
         ----------
         X : array-like, shape [n_samples, n_features]
             The data to determine the categories of each feature.
-    
+
         Returns
         -------
         self
         """
         self._label_encoder = LabelEncoderFeatureGenerator(verbosity=0)
-        self._cat_cols = list(X.select_dtypes(include='category').columns)
+        self._cat_cols = list(X.select_dtypes(include="category").columns)
         if self._cat_cols:
             self._label_encoder.fit(X=X[self._cat_cols])
         X = self._convert_cat_to_int(X=X)
-        X = np.array(X).tolist() # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
+        X = np.array(X).tolist()  # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
         self._validate_keywords()
         self._fit(X, handle_unknown=self.handle_unknown)
         self.drop_idx_ = self._compute_drop_idx()
         # check if user wants to manually drop a feature that is
         # infrequent: this is not allowed
         if self.drop is not None and not isinstance(self.drop, str):
-            for feature_idx, (infrequent_indices, drop_idx) in enumerate(
-                    zip(self.infrequent_indices_, self.drop_idx_)):
+            for feature_idx, (infrequent_indices, drop_idx) in enumerate(zip(self.infrequent_indices_, self.drop_idx_)):
                 if drop_idx in infrequent_indices:
                     raise ValueError(
                         "Category {} of feature {} is infrequent and thus "
                         "cannot be dropped. Use drop='infrequent' "
-                        "instead.".format(
-                            self.categories_[feature_idx][drop_idx],
-                            feature_idx
-                        )
+                        "instead.".format(self.categories_[feature_idx][drop_idx], feature_idx)
                     )
         return self
 
     def transform(self, X):
         """Transform X using one-hot encoding.
-        
+
         Parameters
         ----------
         X : array-like, shape [n_samples, n_features]
             The data to encode.
-        
+
         Returns
         -------
         X_out : sparse matrix if sparse=True else a 2-d array
             Transformed input.
         """
         X = self._convert_cat_to_int(X=X)
-        X = np.array(X).tolist() # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
-        check_is_fitted(self, 'categories_')
+        X = np.array(X).tolist()  # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
+        check_is_fitted(self, "categories_")
         # validation of X happens in _check_X called by _transform
         X_int, X_mask = self._transform(X, handle_unknown=self.handle_unknown)
         n_samples, n_features = X_int.shape
-        
+
         # n_columns indicates, for each feature, how many columns are used in
         # X_trans. By default this corresponds to the number of categories, but
         # will differ if we drop some of them, or if there are infrequent
         # categories (all mapped to the same column)
         n_columns = [len(cats) for cats in self.categories_]
         for feature_idx in range(n_features):
             n_infrequent = self.infrequent_indices_[feature_idx].size
@@ -531,22 +497,21 @@
                 # still add 1 for the infrequent column
                 n_columns[feature_idx] += 1 - n_infrequent
             if self.drop is not None:
                 # if drop is not None we always drop one column in general,
                 # except when drop is 'infrequent' and there is no infrequent
                 # category.
                 n_columns[feature_idx] -= 1
-                if (isinstance(self.drop, str) and self.drop == 'infrequent'
-                        and n_infrequent == 0):
+                if isinstance(self.drop, str) and self.drop == "infrequent" and n_infrequent == 0:
                     n_columns[feature_idx] += 1  # revert decrement from above
-        
+
         if self.drop is not None:
             to_drop = self.drop_idx_.copy()
             if isinstance(self.drop, str):
-                if self.drop == 'infrequent':
+                if self.drop == "infrequent":
                     for feature_idx in range(n_features):
                         if self.infrequent_indices_[feature_idx].size > 0:
                             # drop the infrequent column (i.e. the last one)
                             to_drop[feature_idx] = n_columns[feature_idx]
                         else:
                             # no infrequent category, use special marker -1
                             # so that no dropping happens for this feature
@@ -555,154 +520,145 @@
                 # self.drop is an array of categories. we need to remap the
                 # dropped indexes if some of the categories are infrequent.
                 # see _transform() for details about the mapping.
                 for feature_idx in range(n_features):
                     if self.infrequent_indices_[feature_idx].size > 0:
                         mapping = self._infrequent_mappings[feature_idx]
                         to_drop[feature_idx] = mapping[to_drop[feature_idx]]
-            
+
             # We remove all the dropped categories from mask, and decrement
             # all categories that occur after them to avoid an empty column.
             to_drop = to_drop.reshape(1, -1)
             keep_cells = (X_int != to_drop) | (to_drop == -1)
             X_mask &= keep_cells
             X_int[(X_int > to_drop) & (to_drop != -1)] -= 1
-        
+
         mask = X_mask.ravel()
         n_values = np.array([0] + n_columns)
         feature_indices = np.cumsum(n_values)
         indices = (X_int + feature_indices[:-1]).ravel()[mask]
         indptr = X_mask.sum(axis=1).cumsum()
         indptr = np.insert(indptr, 0, 0)
         data = np.ones(n_samples * n_features)[mask]
-        
-        out = sparse.csr_matrix((data, indices, indptr),
-                                shape=(n_samples, feature_indices[-1]),
-                                dtype=self.dtype)
+
+        out = sparse.csr_matrix((data, indices, indptr), shape=(n_samples, feature_indices[-1]), dtype=self.dtype)
         if not self.sparse:
             return out.toarray()
         else:
             return out
-    
+
     def inverse_transform(self, X):
         """Convert the back data to the original representation.
-        
+
         In case unknown categories are encountered (all zeros in the
         one-hot encoding), ``None`` is used to represent this category.
-        
+
         Parameters
         ----------
         X : array-like or sparse matrix, shape [n_samples, n_encoded_features]
             The transformed data.
-        
+
         Returns
         -------
         X_tr : array-like, shape [n_samples, n_features]
             Inverse transformed array.
-        
+
         """
-        check_is_fitted(self, 'categories_')
-        X = check_array(X, accept_sparse='csr')
-        
+        check_is_fitted(self, "categories_")
+        X = check_array(X, accept_sparse="csr")
+
         n_samples, _ = X.shape
         n_features = len(self.categories_)
         if self.drop is None:
-            n_transformed_features = sum(len(cats)
-                                         for cats in self.categories_)
+            n_transformed_features = sum(len(cats) for cats in self.categories_)
         else:
-            n_transformed_features = sum(len(cats) - 1
-                                         for cats in self.categories_)
-        
+            n_transformed_features = sum(len(cats) - 1 for cats in self.categories_)
+
         # validate shape of passed X
-        msg = ("Shape of the passed X data is not correct. Expected {0} "
-               "columns, got {1}.")
+        msg = "Shape of the passed X data is not correct. Expected {0} " "columns, got {1}."
         if X.shape[1] != n_transformed_features:
             raise ValueError(msg.format(n_transformed_features, X.shape[1]))
-        
+
         # create resulting array of appropriate dtype
         dt = np.find_common_type([cat.dtype for cat in self.categories_], [])
         X_tr = np.empty((n_samples, n_features), dtype=dt)
         j = 0
         found_unknown = {}
-        
+
         for i in range(n_features):
             if self.drop is None:
                 cats = self.categories_[i]
             else:
                 cats = np.delete(self.categories_[i], self.drop_idx_[i])
             n_categories = len(cats)
-        
+
             # Only happens if there was a column with a unique
             # category. In this case we just fill the column with this
             # unique category value.
             if n_categories == 0:
                 X_tr[:, i] = self.categories_[i][self.drop_idx_[i]]
                 j += n_categories
                 continue
-            sub = X[:, j:j + n_categories]  # for sparse X argmax returns 2D matrix, ensure 1D array
+            sub = X[:, j : j + n_categories]  # for sparse X argmax returns 2D matrix, ensure 1D array
             labels = np.asarray(sub.argmax(axis=1)).flatten()
             X_tr[:, i] = cats[labels]
-            if self.handle_unknown == 'ignore':
+            if self.handle_unknown == "ignore":
                 unknown = np.asarray(sub.sum(axis=1) == 0).flatten()
                 # ignored unknown categories: we have a row of all zero
                 if unknown.any():
                     found_unknown[i] = unknown
             # drop will either be None or handle_unknown will be error. If
             # self.drop is not None, then we can safely assume that all of
             # the nulls in each column are the dropped value
             elif self.drop is not None:
                 dropped = np.asarray(sub.sum(axis=1) == 0).flatten()
                 if dropped.any():
                     X_tr[dropped, i] = self.categories_[i][self.drop_idx_[i]]
-            
+
             j += n_categories
-        
+
         # if ignored are found: potentially need to upcast result to
         # insert None values
         if found_unknown:
             if X_tr.dtype != object:
                 X_tr = X_tr.astype(object)
-        
+
             for idx, mask in found_unknown.items():
                 X_tr[mask, idx] = None
-        
+
         return X_tr
-    
+
     def get_feature_names(self, input_features=None):
         """Return feature names for output features.
-    
+
         Parameters
         ----------
         input_features : list of string, length n_features, optional
             String names for input features if available. By default,
             "x0", "x1", ... "xn_features" is used.
-        
+
         Returns
         -------
         output_feature_names : array of string, length n_output_features
-        
+
         """
-        check_is_fitted(self, 'categories_')
+        check_is_fitted(self, "categories_")
         cats = self.categories_
         if input_features is None:
-            input_features = ['x%d' % i for i in range(len(cats))]
+            input_features = ["x%d" % i for i in range(len(cats))]
         elif len(input_features) != len(self.categories_):
-            raise ValueError(
-                "input_features should have length equal to number of "
-                "features ({}), got {}".format(len(self.categories_),
-                                               len(input_features)))
-        
+            raise ValueError("input_features should have length equal to number of " "features ({}), got {}".format(len(self.categories_), len(input_features)))
+
         feature_names = []
         for i in range(len(cats)):
-            names = [
-                input_features[i] + '_' + str(t) for t in cats[i]]
+            names = [input_features[i] + "_" + str(t) for t in cats[i]]
             if self.drop is not None:
                 names.pop(self.drop_idx_[i])
             feature_names.extend(names)
-        
+
         return np.array(feature_names, dtype=object)
 
 
 class OrdinalMergeRaresHandleUnknownEncoder(_BaseEncoder):
     """Encode categorical features as an integer array.
 
     The input to this transformer should be an array-like of integers or
@@ -724,118 +680,119 @@
 
         The used categories can be found in the ``categories_`` attribute.
 
     dtype : number type, default np.float64
         Desired dtype of output.
 
     max_levels : int, default=None
-        One less than the maximum number of categories to keep (max_levels = 2 means we keep 3 distinct categories). 
+        One less than the maximum number of categories to keep (max_levels = 2 means we keep 3 distinct categories).
         Infrequent categories are grouped together and mapped to the highest int
         Unknown categories encountered at test time are mapped to another extra category. Embedding layers should be able to take in max_levels + 1 categories!
 
     Attributes
     ----------
     categories_ : list of arrays
         The categories of each feature determined during fitting
         (in order of the features in X and corresponding with the output
         of ``transform``).
 
     infrequent_indices_: list of arrays of shape(n_infrequent_categories)
         ``infrequent_indices_[i]`` contains a list of indices in
         ``categories_[i]`` corresponding to the infrequent categories.
-    
+
     """
-    
-    def __init__(self, categories='auto', dtype=np.float64, max_levels=None):
+
+    def __init__(self, categories="auto", dtype=np.float64, max_levels=None):
         self.categories = categories
         self.dtype = dtype
         self.max_levels = max_levels
         self._label_encoder = None
-    
+
     def fit(self, X, y=None):
         """Fit the OrdinalEncoder to X.
-        
+
         Parameters
         ----------
         X : array-like, shape [n_samples, n_features]
             The data to determine the categories of each feature.
-        
+
         Returns
         -------
         self
-        
+
         """
         self._label_encoder = LabelEncoderFeatureGenerator(verbosity=0)
         self._label_encoder.fit(X=X)
         X = self._label_encoder.transform(X)
         X = np.array(X).tolist()  # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
-        self._fit(X, handle_unknown='ignore')
+        self._fit(X, handle_unknown="ignore")
 
         self.categories_as_sets_ = [np.array(list(set(categories))) for categories in self.categories_]
         # new level introduced to account for unknown categories, always = 1 + total number of categories seen during training
         self.categories_unknown_level_ = [min(len(categories), self.max_levels) for categories in self.categories_]
         self.categories_len_ = [len(categories) for categories in self.categories_]
         return self
-    
+
     def transform(self, X):
         """Transform X to ordinal codes.
-        
+
         Parameters
         ----------
         X : array-like, shape [n_samples, n_features]
             The data to encode.
-        
+
         Returns
         -------
         X_out : sparse matrix or a 2-d array
             Transformed input.
-        
+
         """
         X = self._label_encoder.transform(X)
         X_og_array = np.array(X)  # original X array before transform
-        X_int, _ = self._transform(X, handle_unknown='ignore')  # will contain zeros for 0th category as well as unknown values.
+        X_int, _ = self._transform(X, handle_unknown="ignore")  # will contain zeros for 0th category as well as unknown values.
 
         for i in range(X_int.shape[1]):
             X_col_data = X_og_array[:, i]
             cat_set = self.categories_as_sets_[i]
             unknown_elements = np.isin(X_col_data, cat_set, invert=True)
-            X_int[unknown_elements, i] = self.categories_unknown_level_[i]  # replace entries with unknown categories with feature_i_numlevels + 1 value. Do NOT modify self.categories_
+            X_int[unknown_elements, i] = self.categories_unknown_level_[
+                i
+            ]  # replace entries with unknown categories with feature_i_numlevels + 1 value. Do NOT modify self.categories_
 
         return X_int.astype(self.dtype, copy=False)
-    
+
     def inverse_transform(self, X):
         """Convert the data back to the original representation.
             In case unknown categories are encountered (all zeros in the one-hot encoding), ``None`` is used to represent this category.
-        
+
         Parameters
         ----------
         X : array-like or sparse matrix, shape [n_samples, n_encoded_features]
             The transformed data.
-        
+
         Returns
         -------
         X_tr : array-like, shape [n_samples, n_features]
             Inverse transformed array.
-        
+
         """
-        check_is_fitted(self, 'categories_')
-        X = check_array(X, accept_sparse='csr')
-        
+        check_is_fitted(self, "categories_")
+        X = check_array(X, accept_sparse="csr")
+
         n_samples, _ = X.shape
         n_features = len(self.categories_)
-        
+
         # validate shape of passed X
-        msg = ("Shape of the passed X data is not correct. Expected {0} "
-               "columns, got {1}.")
+        msg = "Shape of the passed X data is not correct. Expected {0} " "columns, got {1}."
         if X.shape[1] != n_features:
             raise ValueError(msg.format(n_features, X.shape[1]))
-        
+
         # create resulting array of appropriate dtype
         dt = np.find_common_type([cat.dtype for cat in self.categories_], [])
         X_tr = np.empty((n_samples, n_features), dtype=dt)
-        
+
         for i in range(n_features):
             possible_categories = np.append(self.categories_[i], None)
-            labels = X[:, i].astype('int64', copy=False)
+            labels = X[:, i].astype("int64", copy=False)
             X_tr[:, i] = self.categories_[i][labels]
-        
+
         return X_tr
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,90 @@
 """ Data preprocessing helper functions for tabular neural network models """
 
 from collections import OrderedDict
+
 from sklearn.compose import ColumnTransformer
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
-from sklearn.preprocessing import StandardScaler, QuantileTransformer, FunctionTransformer  # can also consider: PowerTransformer
+from sklearn.preprocessing import (  # can also consider: PowerTransformer
+    FunctionTransformer,
+    QuantileTransformer,
+    StandardScaler,
+)
 
 from .categorical_encoders import OneHotMergeRaresHandleUnknownEncoder, OrdinalMergeRaresHandleUnknownEncoder
 
-def create_preprocessor(impute_strategy, max_category_levels, unique_category_str, continuous_features, skewed_features, onehot_features, embed_features, bool_features):
-    """ Creates sklearn ColumnTransformer that can be fit to training data to preprocess it for tabular neural network. """
+
+def create_preprocessor(
+    impute_strategy, max_category_levels, unique_category_str, continuous_features, skewed_features, onehot_features, embed_features, bool_features
+):
+    """Creates sklearn ColumnTransformer that can be fit to training data to preprocess it for tabular neural network."""
     transformers = []  # order of various column transformers in this list is important!
     if continuous_features:
-        continuous_transformer = Pipeline(steps=[
-            ('imputer', SimpleImputer(strategy=impute_strategy)),
-            ('scaler', StandardScaler())])
-        transformers.append( ('continuous', continuous_transformer, continuous_features) )
+        continuous_transformer = Pipeline(steps=[("imputer", SimpleImputer(strategy=impute_strategy)), ("scaler", StandardScaler())])
+        transformers.append(("continuous", continuous_transformer, continuous_features))
     if skewed_features:
-        power_transformer = Pipeline(steps=[
-            ('imputer', SimpleImputer(strategy=impute_strategy)),
-            ('quantile', QuantileTransformer(output_distribution='normal')) ])  # Or output_distribution = 'uniform'
-        transformers.append( ('skewed', power_transformer, skewed_features) )
+        power_transformer = Pipeline(
+            steps=[("imputer", SimpleImputer(strategy=impute_strategy)), ("quantile", QuantileTransformer(output_distribution="normal"))]
+        )  # Or output_distribution = 'uniform'
+        transformers.append(("skewed", power_transformer, skewed_features))
     if onehot_features:
-        onehot_transformer = Pipeline(steps=[
-            ('onehot', OneHotMergeRaresHandleUnknownEncoder(max_levels=max_category_levels, sparse=False))])  # test-time unknown values will be encoded as all zeros vector
-        transformers.append( ('onehot', onehot_transformer, onehot_features) )
+        onehot_transformer = Pipeline(
+            steps=[("onehot", OneHotMergeRaresHandleUnknownEncoder(max_levels=max_category_levels, sparse=False))]
+        )  # test-time unknown values will be encoded as all zeros vector
+        transformers.append(("onehot", onehot_transformer, onehot_features))
     if embed_features:  # Ordinal transformer applied to convert to-be-embedded categorical features to integer levels
-        ordinal_transformer = Pipeline(steps=[
-            ('ordinal', OrdinalMergeRaresHandleUnknownEncoder(max_levels=max_category_levels))])  # returns 0-n when max_category_levels = n-1. category n is reserved for unknown test-time categories.
-        transformers.append( ('ordinal', ordinal_transformer, embed_features) )
-    return ColumnTransformer(transformers=transformers, remainder='passthrough')  # numeric features are processed in the same order as in numeric_features vector, so feature-names remain the same.
+        ordinal_transformer = Pipeline(
+            steps=[("ordinal", OrdinalMergeRaresHandleUnknownEncoder(max_levels=max_category_levels))]
+        )  # returns 0-n when max_category_levels = n-1. category n is reserved for unknown test-time categories.
+        transformers.append(("ordinal", ordinal_transformer, embed_features))
+    return ColumnTransformer(
+        transformers=transformers, remainder="passthrough"
+    )  # numeric features are processed in the same order as in numeric_features vector, so feature-names remain the same.
+
 
 def convert_df_dtype_to_str(df):
     return df.astype(str)
 
+
 def get_feature_arraycol_map(processor, max_category_levels):
-    """ Returns OrderedDict of feature-name -> list of column-indices in processed data array corresponding to this feature """
-    feature_preserving_transforms = set(['continuous','skewed', 'ordinal','bool','remainder'])  # these transforms do not alter dimensionality of feature
+    """Returns OrderedDict of feature-name -> list of column-indices in processed data array corresponding to this feature"""
+    feature_preserving_transforms = set(["continuous", "skewed", "ordinal", "bool", "remainder"])  # these transforms do not alter dimensionality of feature
     feature_arraycol_map = {}  # unordered version
     current_colindex = 0
     for transformer in processor.transformers_:
         transformer_name = transformer[0]
         transformed_features = transformer[2]
         if transformer_name in feature_preserving_transforms:
             for feature in transformed_features:
                 if feature in feature_arraycol_map:
                     raise ValueError("same feature is processed by two different column transformers: %s" % feature)
                 feature_arraycol_map[feature] = [current_colindex]
                 current_colindex += 1
-        elif transformer_name == 'onehot':
-            oh_encoder = [step for (name, step) in transformer[1].steps if name == 'onehot'][0]
+        elif transformer_name == "onehot":
+            oh_encoder = [step for (name, step) in transformer[1].steps if name == "onehot"][0]
             for i in range(len(transformed_features)):
                 feature = transformed_features[i]
                 if feature in feature_arraycol_map:
                     raise ValueError("same feature is processed by two different column transformers: %s" % feature)
-                oh_dimensionality = min(len(oh_encoder.categories_[i]), max_category_levels+1)
-                feature_arraycol_map[feature] = list(range(current_colindex, current_colindex+oh_dimensionality))
+                oh_dimensionality = min(len(oh_encoder.categories_[i]), max_category_levels + 1)
+                feature_arraycol_map[feature] = list(range(current_colindex, current_colindex + oh_dimensionality))
                 current_colindex += oh_dimensionality
         else:
             raise ValueError("unknown transformer encountered: %s" % transformer_name)
     return OrderedDict([(key, feature_arraycol_map[key]) for key in feature_arraycol_map])
 
+
 def get_feature_type_map(feature_arraycol_map, types_of_features):
-    """ Returns OrderedDict of feature-name -> feature_type string (options: 'vector', 'embed'). """
+    """Returns OrderedDict of feature-name -> feature_type string (options: 'vector', 'embed')."""
     if feature_arraycol_map is None:
         raise ValueError("Must first call get_feature_arraycol_map() to set feature_arraycol_map before calling get_feature_type_map()")
-    vector_features = types_of_features['continuous'] + types_of_features['skewed'] + types_of_features['onehot'] + types_of_features['bool']
+    vector_features = types_of_features["continuous"] + types_of_features["skewed"] + types_of_features["onehot"] + types_of_features["bool"]
     feature_type_map = OrderedDict()
     for feature_name in feature_arraycol_map:
         if feature_name in vector_features:
-            feature_type_map[feature_name] = 'vector'
-        elif feature_name in types_of_features['embed']:
-            feature_type_map[feature_name] = 'embed'
+            feature_type_map[feature_name] = "vector"
+        elif feature_name in types_of_features["embed"]:
+            feature_type_map[feature_name] = "embed"
         else:
-            feature_type_map[feature_name] = 'vector'
+            feature_type_map[feature_name] = "vector"
     return feature_type_map
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,54 +2,57 @@
 
 import numpy as np
 
 from autogluon.core.constants import REGRESSION
 
 
 def get_embed_sizes(train_dataset, params, num_categs_per_feature):
-    """ Returns list of embedding sizes for each categorical variable.
-        Selects this adaptively based on training_dataset.
-        Note: Assumes there is at least one embed feature.
+    """Returns list of embedding sizes for each categorical variable.
+    Selects this adaptively based on training_dataset.
+    Note: Assumes there is at least one embed feature.
     """
-    max_embedding_dim = params['max_embedding_dim']
-    embed_exponent = params['embed_exponent']
-    size_factor = params['embedding_size_factor']
-    embed_dims = [int(size_factor*max(2, min(max_embedding_dim,
-                                      1.6 * num_categs_per_feature[i]**embed_exponent)))
-                   for i in range(len(num_categs_per_feature))]
+    max_embedding_dim = params["max_embedding_dim"]
+    embed_exponent = params["embed_exponent"]
+    size_factor = params["embedding_size_factor"]
+    embed_dims = [
+        int(size_factor * max(2, min(max_embedding_dim, 1.6 * num_categs_per_feature[i] ** embed_exponent))) for i in range(len(num_categs_per_feature))
+    ]
     return embed_dims
 
+
 def infer_y_range(y_vals, y_range_extend):
-    """ Infers good output range for neural network when used for regression. """
+    """Infers good output range for neural network when used for regression."""
     min_y = float(min(y_vals))
     max_y = float(max(y_vals))
     std_y = np.std(y_vals)
     y_ext = y_range_extend * std_y
     if min_y >= 0:  # infer y must be nonnegative
-        min_y = max(0, min_y-y_ext)
+        min_y = max(0, min_y - y_ext)
     else:
-        min_y = min_y-y_ext
+        min_y = min_y - y_ext
     if max_y <= 0:  # infer y must be non-positive
-        max_y = min(0, max_y+y_ext)
+        max_y = min(0, max_y + y_ext)
     else:
-        max_y = max_y+y_ext
+        max_y = max_y + y_ext
     return (min_y, max_y)
 
+
 def get_default_layers(problem_type, num_net_outputs, max_layer_width):
-    """ Default sizes for NN layers. """
+    """Default sizes for NN layers."""
     if problem_type == REGRESSION:
         default_layer_sizes = [256, 128]  # overall network will have 4 layers. Input layer, 256-unit hidden layer, 128-unit hidden layer, output layer.
     else:
         default_sizes = [256, 128]  # will be scaled adaptively
         # base_size = max(1, min(num_net_outputs, 20)/2.0) # scale layer width based on number of classes
         base_size = max(1, min(num_net_outputs, 100) / 50)  # TODO: Updated because it improved model quality and made training far faster
-        default_layer_sizes = [defaultsize*base_size for defaultsize in default_sizes]
+        default_layer_sizes = [defaultsize * base_size for defaultsize in default_sizes]
     layer_expansion_factor = 1  # TODO: consider scaling based on num_rows, eg: layer_expansion_factor = 2-np.exp(-max(0,train_dataset.num_examples-10000))
-    return [int(min(max_layer_width, layer_expansion_factor*defaultsize)) for defaultsize in default_layer_sizes]
+    return [int(min(max_layer_width, layer_expansion_factor * defaultsize)) for defaultsize in default_layer_sizes]
+
 
 def default_numeric_embed_dim(train_dataset, max_layer_width, first_layer_width):
-    """ Default embedding dimensionality for numeric features. """
+    """Default embedding dimensionality for numeric features."""
     vector_dim = train_dataset.dataset._data[train_dataset.vectordata_index].shape[1]  # total dimensionality of vector features
     prop_vector_features = train_dataset.num_vector_features() / float(train_dataset.num_features)  # Fraction of features that are numeric
     min_numeric_embed_dim = 32
     max_numeric_embed_dim = max_layer_width
-    return int(min(max_numeric_embed_dim, max(min_numeric_embed_dim, first_layer_width*prop_vector_features*np.log10(vector_dim+10))))
+    return int(min(max_numeric_embed_dim, max(min_numeric_embed_dim, first_layer_width * prop_vector_features * np.log10(vector_dim + 10))))
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 import logging
 import time
 
 import numpy as np
 import pandas as pd
 
-from autogluon.core.models import AbstractModel
-from autogluon.common.features.types import R_INT, R_FLOAT, R_CATEGORY, R_OBJECT, S_IMAGE_PATH, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY, S_TEXT_SPECIAL
+from autogluon.common.features.types import (
+    R_CATEGORY,
+    R_FLOAT,
+    R_INT,
+    R_OBJECT,
+    S_IMAGE_PATH,
+    S_TEXT_AS_CATEGORY,
+    S_TEXT_NGRAM,
+    S_TEXT_SPECIAL,
+)
 from autogluon.common.utils.try_import import try_import_vowpalwabbit
-from autogluon.core.constants import BINARY, REGRESSION, MULTICLASS, \
-    PROBLEM_TYPES_CLASSIFICATION, PROBLEM_TYPES_REGRESSION
+from autogluon.core.constants import (
+    BINARY,
+    MULTICLASS,
+    PROBLEM_TYPES_CLASSIFICATION,
+    PROBLEM_TYPES_REGRESSION,
+    REGRESSION,
+)
+from autogluon.core.models import AbstractModel
 from autogluon.core.utils.exceptions import TimeLimitExceeded
+
 from .vowpalwabbit_utils import VWFeaturesConverter
 
 logger = logging.getLogger(__name__)
 
 
 class VowpalWabbitModel(AbstractModel):
     """
     VowpalWabbit Model: https://vowpalwabbit.org/
 
     VowpalWabbit Command Line args: https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Command-line-arguments
 
     """
-    model_internals_file_name = 'model-internals.pkl'
+
+    model_internals_file_name = "model-internals.pkl"
 
     # Ref: https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Loss-functions
-    CLASSIFICATION_LOSS_FUNCTIONS = ['logistic', 'hinge']
-    REGRESSION_LOSS_FUNCTIONS = ['squared', 'quantile', 'poisson', 'classic']
+    CLASSIFICATION_LOSS_FUNCTIONS = ["logistic", "hinge"]
+    REGRESSION_LOSS_FUNCTIONS = ["squared", "quantile", "poisson", "classic"]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._load_model = None  # Used for saving and loading internal model file
 
     # The `_preprocess` method takes the input data and transforms it to the internal representation usable by the model.
     # `_preprocess` is called by `preprocess` and is used during model fit and model inference.
@@ -40,66 +56,64 @@
             self._features_converter = VWFeaturesConverter()
             self._feature_metadata_dict = self._feature_metadata.to_dict()
         # self._feature_metadata contains the information related to features metadata.
         X_series = self._features_converter.convert_features_to_vw_format(X, self._feature_metadata_dict)
         return X_series
 
     # The `_fit` method takes the input training data (and optionally the validation data) and trains the model.
-    def _fit(self,
-             X: pd.DataFrame,  # training data
-             y: pd.Series,  # training labels
-             time_limit=None,
-             verbosity=2,
-             **kwargs):  # kwargs includes many other potential inputs, refer to AbstractModel documentation for details
+    def _fit(
+        self, X: pd.DataFrame, y: pd.Series, time_limit=None, verbosity=2, **kwargs  # training data  # training labels
+    ):  # kwargs includes many other potential inputs, refer to AbstractModel documentation for details
         time_start = time.time()
         try_import_vowpalwabbit()
         import vowpalwabbit
+
         seed = 0  # Random seed
 
         # Valid self.problem_type values include ['binary', 'multiclass', 'regression', 'quantile', 'softclass']
         if self.problem_type not in PROBLEM_TYPES_REGRESSION + PROBLEM_TYPES_CLASSIFICATION:
             raise TypeError(f"Vowpal Wabbit does not support {self.problem_type}")
 
         # Certain parameters like passes are passed as hyperparameters but are not used
         # while initialising the model.
         # passes: Used as epochs
 
         params = self._get_model_params()
-        params['loss_function'] = params.get('loss_function', self._get_default_loss_function())
-        passes = params.pop('passes')
+        params["loss_function"] = params.get("loss_function", self._get_default_loss_function())
+        passes = params.pop("passes")
 
         # Make sure to call preprocess on X near the start of `_fit`.
         # This is necessary because the data is converted via preprocess during predict, and needs to be in the same format as during fit.
         X_series = self.preprocess(X, is_train=True)
 
-        self._validate_loss_function(loss_function=params['loss_function'])
+        self._validate_loss_function(loss_function=params["loss_function"])
 
         # VW expects label from 1 to N for Binary and Multiclass classification problems
         # AutoGluon does label encoding from 0 to N-1, hence we increment the value of y by 1
         if self.problem_type != REGRESSION:
             y = y.apply(lambda row: row + 1)
-        y = y.astype(str) + ' '
+        y = y.astype(str) + " "
 
         # Concatenate y and X to get the training data in VW format
         final_training_data = y + X_series
         final_training_data = final_training_data.tolist()
 
         extra_params = {
-            'cache_file': 'train.cache',
-            'holdout_off': True,
+            "cache_file": "train.cache",
+            "holdout_off": True,
         }
 
         if verbosity <= 3:
-            extra_params['quiet'] = True
+            extra_params["quiet"] = True
 
         # Initialize the model
         if self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
             # Ref: https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Predicting-probabilities#multi-class---oaa
-            extra_params['oaa'] = self.num_classes
-            extra_params['probabilities'] = True
+            extra_params["oaa"] = self.num_classes
+            extra_params["probabilities"] = True
         self.model = vowpalwabbit.Workspace(**params, **extra_params)
 
         time_start_fit = time.time()
         if time_limit is not None:
             time_limit_fit = time_limit - (time_start_fit - time_start) - 0.3  # Account for 0.3s overhead
             if time_limit_fit <= 0:
                 raise TimeLimitExceeded
@@ -113,45 +127,45 @@
         for epoch in range(1, passes + 1):
             # TODO: Add Early Stopping support via validation
             self._train_single_epoch(training_data=final_training_data)
             if time_limit_fit is not None and epoch < passes:
                 time_fit_used = time.time() - time_start_fit
                 time_fit_used_per_epoch = time_fit_used / epoch
                 time_left = time_limit_fit - time_fit_used
-                if time_left <= (time_fit_used_per_epoch*2):
-                    logger.log(30, f'\tEarly stopping due to lack of time. Fit {epoch}/{passes} passes...')
+                if time_left <= (time_fit_used_per_epoch * 2):
+                    logger.log(30, f"\tEarly stopping due to lack of time. Fit {epoch}/{passes} passes...")
                     break
 
-        self.params_trained['passes'] = epoch
+        self.params_trained["passes"] = epoch
 
     def _train_single_epoch(self, training_data):
         row_order = np.arange(0, len(training_data))
         row_order = np.random.permutation(row_order)
         for row_i in row_order:
             row = training_data[row_i]
             self.model.learn(row)
 
     def _validate_loss_function(self, loss_function):
         # Ref: https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Loss-functions
         if loss_function:
             if self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
-                assert loss_function in self.CLASSIFICATION_LOSS_FUNCTIONS, \
-                    f'For {self.problem_type} problem, VW supports: {self.CLASSIFICATION_LOSS_FUNCTIONS}. ' \
-                    f'Got loss_function:{loss_function}'
+                assert loss_function in self.CLASSIFICATION_LOSS_FUNCTIONS, (
+                    f"For {self.problem_type} problem, VW supports: {self.CLASSIFICATION_LOSS_FUNCTIONS}. " f"Got loss_function:{loss_function}"
+                )
             elif self.problem_type in PROBLEM_TYPES_REGRESSION:
-                assert loss_function in self.REGRESSION_LOSS_FUNCTIONS, \
-                    f'For {self.problem_type} problem, VW supports: {self.REGRESSION_LOSS_FUNCTIONS}. ' \
-                    f'Got loss_function:{loss_function}'
+                assert loss_function in self.REGRESSION_LOSS_FUNCTIONS, (
+                    f"For {self.problem_type} problem, VW supports: {self.REGRESSION_LOSS_FUNCTIONS}. " f"Got loss_function:{loss_function}"
+                )
 
     def _get_default_loss_function(self) -> str:
         # Ref: https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Loss-functions
         if self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
-            return 'logistic'
+            return "logistic"
         else:
-            return 'squared'
+            return "squared"
 
     def save(self, path: str = None, verbose=True) -> str:
         """
         AutoGluon by default saves the complete Abstract Model in a pickle file format.
         This includes the internal self.model which is the actual model.
         However, saving VW model in pickle is not possible.
         Hence, we dump the Abstract Model by setting setting self.model as None
@@ -179,25 +193,26 @@
         """
         There are two files which needs to be loaded.
         First is the Abstract Model pickle dump and second is the internal model file.
         For VW, based on different problem_type/hyperparams, loading arguments will be different
         """
         try_import_vowpalwabbit()
         import vowpalwabbit
+
         # Load Abstract Model. This is without the internal model
         model = super().load(path, reset_paths=reset_paths, verbose=verbose)
         params = model._get_model_params()
         # Load the internal model file
         if model._load_model:
             file_path = path + cls.model_internals_file_name
 
             model_load_params = f" -i {file_path} --quiet"
             if model.problem_type in PROBLEM_TYPES_CLASSIFICATION:
                 model_load_params += " --probabilities --loss_function=logistic"
-            if params['sparse_weights']:
+            if params["sparse_weights"]:
                 model_load_params += " --sparse_weights"
 
             model.model = vowpalwabbit.Workspace(model_load_params)
         model._load_model = None
         return model
 
     def _predict_proba(self, X, **kwargs):
@@ -212,47 +227,46 @@
         # Returning 5MB as the value
         return int(5e6)
 
     # The `_set_default_params` method defines the default hyperparameters of the model.
     # User-specified parameters will override these values on a key-by-key basis.
     def _set_default_params(self):
         default_params = {
-            'passes': 10,  # TODO: Much better if 500+, revisit this if wanting to use VW to get strong results
-            'bit_precision': 32,
-            'ngram': 2,
-            'skips': 1,
-            'learning_rate': 1,
-            'sparse_weights': True,
+            "passes": 10,  # TODO: Much better if 500+, revisit this if wanting to use VW to get strong results
+            "bit_precision": 32,
+            "ngram": 2,
+            "skips": 1,
+            "learning_rate": 1,
+            "sparse_weights": True,
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     # The `_get_default_auxiliary_params` method defines various model-agnostic parameters such as maximum memory usage and valid input column dtypes.
     # For most users who build custom models, they will only need to specify the valid/invalid dtypes to the model here.
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         # Ignore the below mentioned special types. Only those features that are not of the below mentioned
         # type are passed to the model for training list are passed features
         extra_auxiliary_params = dict(
-            valid_raw_types=[R_INT, R_FLOAT, R_CATEGORY, R_OBJECT],
-            ignored_type_group_special=[S_IMAGE_PATH, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY, S_TEXT_SPECIAL]
+            valid_raw_types=[R_INT, R_FLOAT, R_CATEGORY, R_OBJECT], ignored_type_group_special=[S_IMAGE_PATH, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY, S_TEXT_SPECIAL]
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     @classmethod
     def _get_default_ag_args(cls) -> dict:
         default_ag_args = super()._get_default_ag_args()
         extra_ag_args = {
-            'valid_stacker': False,
-            'problem_types': [BINARY, MULTICLASS, REGRESSION],
+            "valid_stacker": False,
+            "problem_types": [BINARY, MULTICLASS, REGRESSION],
         }
         default_ag_args.update(extra_ag_args)
         return default_ag_args
 
     def _more_tags(self):
         # `can_refit_full=True` because best epoch is communicated at end of `_fit`: `self.params_trained['passes'] = epoch`
-        return {'can_refit_full': True}
+        return {"can_refit_full": True}
 
     @classmethod
     def _class_tags(cls):
-        return {'handles_text': True}
+        return {"handles_text": True}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pandas as pd
-from autogluon.common.features.types import S_TEXT, R_INT, R_FLOAT, R_CATEGORY
+
+from autogluon.common.features.types import R_CATEGORY, R_FLOAT, R_INT, S_TEXT
 
 
 class VWFeaturesConverter:
     """
     Converts features in PandasDataFrame to VW format
     Ref: https://github.com/VowpalWabbit/vowpal_wabbit/wiki/Input-format
     """
 
-    PIPE = '|'
-    SPACE = ' '
+    PIPE = "|"
+    SPACE = " "
 
     # TODO: Add support for different namespaces
 
     def convert_features_to_vw_format(self, X, feature_metadata) -> pd.Series:
         """
         Converts features to VW format.
         :param X: features
@@ -22,31 +23,27 @@
         """
 
         X_out: pd.Series = None
 
         for feature in feature_metadata:
             raw_feature, special_feature = feature_metadata[feature]
             if X_out is None:
-                X_out = self.PIPE + self.SPACE + self.__generate_namespace_based_on_ml_type(
-                    X[feature],
-                    raw_feature,
-                    special_feature,
-                    feature
-                ).astype('str') + self.SPACE
+                X_out = (
+                    self.PIPE
+                    + self.SPACE
+                    + self.__generate_namespace_based_on_ml_type(X[feature], raw_feature, special_feature, feature).astype("str")
+                    + self.SPACE
+                )
             else:
-                X_out += '' + self.SPACE + self.__generate_namespace_based_on_ml_type(
-                    X[feature],
-                    raw_feature,
-                    special_feature,
-                    feature
-                ).astype('str') + self.SPACE
+                X_out += (
+                    "" + self.SPACE + self.__generate_namespace_based_on_ml_type(X[feature], raw_feature, special_feature, feature).astype("str") + self.SPACE
+                )
         return X_out
 
-    def __generate_namespace_based_on_ml_type(self, input_series, raw_feature, special_feature,
-                                              feature_name=None):
+    def __generate_namespace_based_on_ml_type(self, input_series, raw_feature, special_feature, feature_name=None):
         """
         Based on the type of feature, preprocess/sanify these features so that it is in VW format
         Only use raw text, numeric integer, numeric decimals, and category
         Ref: https://github.com/autogluon/autogluon/blob/master/common/src/autogluon/common/features/types.py
 
         :param input_series: A single feature as Pandas Series
         :param raw_feature: Raw feature Type
@@ -64,33 +61,33 @@
             raise ValueError(
                 f"Received unsupported raw_feature_type '{str(raw_feature)}' special_feature_type '{str(special_feature)}'"
                 f" for feature '{feature_name}' for class {self.__class__.__name__}."
             )
 
     def __preprocess_text(self, s) -> str:
         if pd.isnull(s):
-            return ''
+            return ""
         s = " ".join(str(s).split())
         # Added split to remove tabs spaces since tab is used as separator
         text = self.__sanify(s)
         return text
 
     def __sanify(self, s) -> str:
-        '''
+        """
         The sanify is performed because : and | are reserved by vowpal wabbit for distinguishing namespaces and numeric
         data
         @param s: input string
         @returns string
-        '''
-        return str(s).replace(":", ";").replace('|', '/')
+        """
+        return str(s).replace(":", ";").replace("|", "/")
 
     def __numeric_namespace_generator(self, feature, feature_name) -> str:
         if pd.isnull(feature):
-            return ''
-        return feature_name + ':' + str(feature)
+            return ""
+        return feature_name + ":" + str(feature)
 
     def __categorical_namespace_generator(self, feature, feature_name) -> str:
         if pd.isnull(feature):
-            return ''
+            return ""
         else:
-            feature = str(feature).replace(' ', '_')
-            return feature_name + '=' + self.__sanify(feature)
+            feature = str(feature).replace(" ", "_")
+            return feature_name + "=" + self.__sanify(feature)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import time
 import logging
+import time
 
 from xgboost.callback import EarlyStopping
 
 from autogluon.common.utils.lite import disable_if_lite_mode
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.core.utils.early_stopping import SimpleES
 
@@ -16,14 +16,15 @@
 
     Parameters
     ----------
     rounds : int or tuple
        If int, The possible number of rounds without the trend occurrence.
        If tuple, contains early stopping class as first element and class init kwargs as second element.
     """
+
     def __init__(self, rounds, time_limit=None, start_time=None, verbose=False, min_delta=2e-6, **kwargs):
         if rounds is None:
             # Disable early stopping via rounds
             rounds = 999999
         # Add a tiny min_delta so training doesn't go on for extremely long if only tiny improvements are being made
         #  (can occur when validation error is almost 0, such as val log_loss <0.00005)
         super().__init__(rounds=999999, min_delta=min_delta, **kwargs)
@@ -62,15 +63,18 @@
 
     def _time_check(self, model, epoch):
         if self.time_limit is not None:
             time_elapsed = time.time() - self.start_time
             time_left = self.time_limit - time_elapsed
             if time_left <= 0:
                 if self.verbose:
-                    logger.log(20, f"Ran out of time, early stopping on iteration {epoch}. Best iteration is: \t[{model.attr('best_iteration')}]\t{model.attr('best_score')}")
+                    logger.log(
+                        20,
+                        f"Ran out of time, early stopping on iteration {epoch}. Best iteration is: \t[{model.attr('best_iteration')}]\t{model.attr('best_score')}",
+                    )
                 return True
         return False
 
     @disable_if_lite_mode(ret=False)
     def _memory_check(self, model):
         available = ResourceManager.get_available_virtual_mem()
         cur_rss = self._mem_status.memory_info().rss
@@ -78,18 +82,20 @@
             self._mem_init_rss = cur_rss
         estimated_model_size_mb = (cur_rss - self._mem_init_rss) >> 20
         available_mb = available >> 20
 
         model_size_memory_ratio = estimated_model_size_mb / available_mb
 
         if (model_size_memory_ratio > 1.0) or (available_mb < 512):
-            logger.warning('Warning: Large XGB model size may cause OOM error if training continues')
-            logger.warning(f'Available Memory: {available_mb} MB')
-            logger.warning(f'Estimated XGB model size: {estimated_model_size_mb} MB')
+            logger.warning("Warning: Large XGB model size may cause OOM error if training continues")
+            logger.warning(f"Available Memory: {available_mb} MB")
+            logger.warning(f"Estimated XGB model size: {estimated_model_size_mb} MB")
             if self.verbose:
-                logger.warning(f'Warning: Early stopped XGB model prior to optimal result to avoid OOM error. Please increase available memory to avoid subpar model quality.\n')
+                logger.warning(
+                    f"Warning: Early stopped XGB model prior to optimal result to avoid OOM error. Please increase available memory to avoid subpar model quality.\n"
+                )
                 logger.warning(f"Early stopping. Best iteration is: \t[{model.attr('best_iteration')}]\t{model.attr('best_score')}")
             return True
         elif self.verbose and (model_size_memory_ratio > 0.25):
-            logger.log(15, f'Available Memory: {available_mb} MB')
-            logger.log(15, f'Estimated XGB model size: {estimated_model_size_mb} MB')
+            logger.log(15, f"Available Memory: {available_mb} MB")
+            logger.log(15, f"Estimated XGB model size: {estimated_model_size_mb} MB")
         return False
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autogluon.core.constants import BINARY, MULTICLASS, SOFTCLASS, REGRESSION
+from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS
 
 DEFAULT_NUM_BOOST_ROUND = 10000
 MAX_CATEGORY_LEVELS = 100  # maximum number of allowed levels per categorical feature
 # Options: [10, 100, 200, 300, 400, 500, 1000, 10000]
 
 
 def get_param_baseline(problem_type, num_classes=None):
@@ -16,44 +16,44 @@
         return get_param_regression_baseline()
     else:
         return get_param_binary_baseline()
 
 
 def get_base_params():
     base_params = {
-        'n_estimators': DEFAULT_NUM_BOOST_ROUND,
-        'learning_rate': 0.1,
-        'n_jobs': -1,
-        'proc.max_category_levels': MAX_CATEGORY_LEVELS,
+        "n_estimators": DEFAULT_NUM_BOOST_ROUND,
+        "learning_rate": 0.1,
+        "n_jobs": -1,
+        "proc.max_category_levels": MAX_CATEGORY_LEVELS,
     }
     return base_params
 
 
 def get_param_binary_baseline():
     params = get_base_params()
     baseline_params = {
-        'objective': 'binary:logistic',
-        'booster': 'gbtree',
+        "objective": "binary:logistic",
+        "booster": "gbtree",
     }
     params.update(baseline_params)
     return params
 
 
 def get_param_multiclass_baseline(num_classes):
     params = get_base_params()
     baseline_params = {
-        'objective': 'multi:softprob',
-        'booster': 'gbtree',
-        'num_class': num_classes,
+        "objective": "multi:softprob",
+        "booster": "gbtree",
+        "num_class": num_classes,
     }
     params.update(baseline_params)
     return params
 
 
 def get_param_regression_baseline():
     params = get_base_params()
     baseline_params = {
-        'objective': 'reg:squarederror',
-        'booster': 'gbtree',
+        "objective": "reg:squarederror",
+        "booster": "gbtree",
     }
     params.update(baseline_params)
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Default hyperparameter search spaces used in XGBoost Boosting model """
 from autogluon.common import space
-
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION
 
 DEFAULT_NUM_BOOST_ROUND = 10000  # default for HPO
 
 
 def get_default_searchspace(problem_type, num_classes=None):
     if problem_type == BINARY:
@@ -15,49 +14,49 @@
         return get_searchspace_regression_baseline()
     else:
         return get_searchspace_binary_baseline()
 
 
 def get_base_searchspace():
     base_params = {
-        'n_estimators': DEFAULT_NUM_BOOST_ROUND,
-        'booster': 'gbtree',
-        'n_jobs': -1,
-        'learning_rate': space.Real(lower=5e-3, upper=0.2, default=0.1, log=True),
-        'max_depth': space.Int(lower=3, upper=10, default=6),
-        'min_child_weight': space.Int(lower=1, upper=5, default=1),
-        'colsample_bytree': space.Real(lower=0.5, upper=1.0, default=1.0),
+        "n_estimators": DEFAULT_NUM_BOOST_ROUND,
+        "booster": "gbtree",
+        "n_jobs": -1,
+        "learning_rate": space.Real(lower=5e-3, upper=0.2, default=0.1, log=True),
+        "max_depth": space.Int(lower=3, upper=10, default=6),
+        "min_child_weight": space.Int(lower=1, upper=5, default=1),
+        "colsample_bytree": space.Real(lower=0.5, upper=1.0, default=1.0),
         # Below lines are commented out as they made search worse. Refine ranges before considering reintroducing these hyperparameters.
         # 'gamma': Real(lower=0, upper=5, default=0),
         # 'subsample': Real(lower=0.5, upper=1.0, default=1.0),
         # 'reg_alpha': Real(lower=0.0, upper=10.0, default=0.0),
         # 'reg_lambda': Real(lower=0.0, upper=10.0, default=1.0),
     }
     return base_params
 
 
 def get_searchspace_multiclass_baseline(num_classes):
     params = get_base_searchspace()
     baseline_params = {
-        'objective': 'multi:softmax',
-        'num_class': num_classes,
+        "objective": "multi:softmax",
+        "num_class": num_classes,
     }
     params.update(baseline_params)
     return params
 
 
 def get_searchspace_binary_baseline():
     params = get_base_searchspace()
     baseline_params = {
-        'objective': 'binary:logistic',
+        "objective": "binary:logistic",
     }
     params.update(baseline_params)
     return params
 
 
 def get_searchspace_regression_baseline():
     params = get_base_searchspace()
     baseline_params = {
-        'objective': 'reg:squarederror',
+        "objective": "reg:squarederror",
     }
     params.update(baseline_params)
     return params
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import time
 import logging
+import time
 
-from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY
+from autogluon.common.features.types import R_BOOL, R_CATEGORY, R_FLOAT, R_INT
 from autogluon.common.utils.lite import disable_if_lite_mode
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_xgboost
-from autogluon.core.constants import MULTICLASS, REGRESSION, SOFTCLASS, PROBLEM_TYPES_CLASSIFICATION
+from autogluon.core.constants import MULTICLASS, PROBLEM_TYPES_CLASSIFICATION, REGRESSION, SOFTCLASS
 from autogluon.core.models import AbstractModel
 from autogluon.core.models._utils import get_early_stopping_rounds
 
 from . import xgboost_utils
 from .hyperparameters.parameters import get_param_baseline
 from .hyperparameters.searchspaces import get_default_searchspace
 
@@ -19,14 +19,15 @@
 
 class XGBoostModel(AbstractModel):
     """
     XGBoost model: https://xgboost.readthedocs.io/en/latest/
 
     Hyperparameter options: https://xgboost.readthedocs.io/en/latest/parameter.html
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._ohe: bool = True
         self._ohe_generator = None
         self._xgb_model_type = None
 
     def _set_default_params(self):
@@ -61,34 +62,23 @@
                 self._ohe_generator.fit(X)
 
         if self._ohe:
             X = self._ohe_generator.transform(X)
 
         return X
 
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             time_limit=None,
-             num_gpus=0,
-             num_cpus=None,
-             sample_weight=None,
-             sample_weight_val=None,
-             verbosity=2,
-             **kwargs):
+    def _fit(self, X, y, X_val=None, y_val=None, time_limit=None, num_gpus=0, num_cpus=None, sample_weight=None, sample_weight_val=None, verbosity=2, **kwargs):
         # TODO: utilize sample_weight_val in early-stopping if provided
         start_time = time.time()
         ag_params = self._get_ag_params()
         params = self._get_model_params()
         if num_cpus:
-            params['n_jobs'] = num_cpus
-        max_category_levels = params.pop('proc.max_category_levels', 100)
-        enable_categorical = params.get('enable_categorical', False)
+            params["n_jobs"] = num_cpus
+        max_category_levels = params.pop("proc.max_category_levels", 100)
+        enable_categorical = params.get("enable_categorical", False)
         if enable_categorical:
             """Skip one-hot-encoding and pass categoricals directly to XGBoost"""
             self._ohe = False
         else:
             """One-hot-encode categorical features"""
             self._ohe = True
 
@@ -102,76 +92,73 @@
             verbose = True
             log_period = 1
 
         X = self.preprocess(X, is_train=True, max_category_levels=max_category_levels)
         num_rows_train = X.shape[0]
 
         eval_set = []
-        if 'eval_metric' not in params:
+        if "eval_metric" not in params:
             eval_metric = self.get_eval_metric()
             if eval_metric is not None:
-                params['eval_metric'] = eval_metric
+                params["eval_metric"] = eval_metric
 
         if X_val is None:
             early_stopping_rounds = None
             eval_set = None
         else:
             X_val = self.preprocess(X_val, is_train=False)
             eval_set.append((X_val, y_val))
-            early_stopping_rounds = ag_params.get('early_stop', 'adaptive')
+            early_stopping_rounds = ag_params.get("early_stop", "adaptive")
             if isinstance(early_stopping_rounds, (str, tuple, list)):
                 early_stopping_rounds = self._get_early_stopping_rounds(num_rows_train=num_rows_train, strategy=early_stopping_rounds)
 
         if num_gpus != 0:
-            params['tree_method'] = 'gpu_hist'
-            if 'gpu_id' not in params:
-                params['gpu_id'] = 0
-        elif 'tree_method' not in params:
-            params['tree_method'] = 'hist'
+            params["tree_method"] = "gpu_hist"
+            if "gpu_id" not in params:
+                params["gpu_id"] = 0
+        elif "tree_method" not in params:
+            params["tree_method"] = "hist"
 
         try_import_xgboost()
-        from .callbacks import EarlyStoppingCustom
         from xgboost.callback import EvaluationMonitor
-        if eval_set is not None and 'callbacks' not in params:
+
+        from .callbacks import EarlyStoppingCustom
+
+        if eval_set is not None and "callbacks" not in params:
             callbacks = []
             if log_period is not None:
                 callbacks.append(EvaluationMonitor(period=log_period))
             callbacks.append(EarlyStoppingCustom(early_stopping_rounds, start_time=start_time, time_limit=time_limit, verbose=verbose))
-            params['callbacks'] = callbacks
+            params["callbacks"] = callbacks
 
         from xgboost import XGBClassifier, XGBRegressor
+
         model_type = XGBClassifier if self.problem_type in PROBLEM_TYPES_CLASSIFICATION else XGBRegressor
         self.model = model_type(**params)
-        self.model.fit(
-            X=X,
-            y=y,
-            eval_set=eval_set,
-            verbose=False,
-            sample_weight=sample_weight
-        )
+        self.model.fit(X=X, y=y, eval_set=eval_set, verbose=False, sample_weight=sample_weight)
 
         bst = self.model.get_booster()
         # TODO: Investigate speed-ups from GPU inference
         # bst.set_param({"predictor": "gpu_predictor"})
 
-        self.params_trained['n_estimators'] = bst.best_ntree_limit
+        self.params_trained["n_estimators"] = bst.best_ntree_limit
         # Don't save the callback or eval_metric objects
         self.model.set_params(callbacks=None, eval_metric=None)
 
     def _predict_proba(self, X, num_cpus=-1, **kwargs):
         X = self.preprocess(X, **kwargs)
         self.model.set_params(n_jobs=num_cpus)
 
         if self.problem_type == REGRESSION:
             return self.model.predict(X)
 
         y_pred_proba = self.model.predict_proba(X)
         return self._convert_proba_to_unified_form(y_pred_proba)
 
-    def _get_early_stopping_rounds(self, num_rows_train, strategy='auto'):
+    def _get_early_stopping_rounds(self, num_rows_train, strategy="auto"):
         return get_early_stopping_rounds(num_rows_train=num_rows_train, strategy=strategy)
 
     def _get_num_classes(self, y):
         if self.problem_type == MULTICLASS:
             if self.num_classes is not None:
                 num_classes = self.num_classes
             else:
@@ -179,34 +166,33 @@
         elif self.problem_type == SOFTCLASS:  # TODO: delete this elif if it's unnecessary.
             num_classes = y.shape[1]
         else:
             num_classes = 1
         return num_classes
 
     def _ag_params(self) -> set:
-        return {'early_stop'}
+        return {"early_stop"}
 
     def _estimate_memory_usage(self, X, **kwargs):
         num_classes = self.num_classes if self.num_classes else 1  # self.num_classes could be None after initialization if it's a regression problem
         data_mem_usage = get_approximate_df_mem_usage(X).sum()
         approx_mem_size_req = data_mem_usage * 7 + data_mem_usage / 4 * num_classes  # TODO: Extremely crude approximation, can be vastly improved
         return approx_mem_size_req
 
     def _validate_fit_memory_usage(self, mem_error_threshold: float = 1.0, mem_warning_threshold: float = 0.75, mem_size_threshold: int = 1e9, **kwargs):
-        return super()._validate_fit_memory_usage(mem_error_threshold=mem_error_threshold,
-                                                  mem_warning_threshold=mem_warning_threshold,
-                                                  mem_size_threshold=mem_size_threshold,
-                                                  **kwargs)
+        return super()._validate_fit_memory_usage(
+            mem_error_threshold=mem_error_threshold, mem_warning_threshold=mem_warning_threshold, mem_size_threshold=mem_size_threshold, **kwargs
+        )
 
     def get_minimum_resources(self, is_gpu_available=False):
         minimum_resources = {
-            'num_cpus': 1,
+            "num_cpus": 1,
         }
         if is_gpu_available:
-            minimum_resources['num_gpus'] = 0.5
+            minimum_resources["num_gpus"] = 0.5
         return minimum_resources
 
     @disable_if_lite_mode(ret=(1, 0))
     def _get_default_resources(self):
         # logical=False is faster in training
         num_cpus = ResourceManager.get_cpu_count_psutil(logical=False)
         num_gpus = 0
@@ -216,25 +202,25 @@
         _model = self.model
         self.model = None
         if _model is not None:
             self._xgb_model_type = _model.__class__
         path = super().save(path=path, verbose=verbose)
         if _model is not None:
             # Halves disk usage compared to .json / .pkl
-            _model.save_model(path + 'xgb.ubj')
+            _model.save_model(path + "xgb.ubj")
         self.model = _model
         return path
 
     @classmethod
     def load(cls, path: str, reset_paths=True, verbose=True):
         model = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
         if model._xgb_model_type is not None:
             model.model = model._xgb_model_type()
             # Much faster to load using .ubj than .json (10x+ speedup)
-            model.model.load_model(path + 'xgb.ubj')
+            model.model.load_model(path + "xgb.ubj")
             model._xgb_model_type = None
         return model
 
     def _more_tags(self):
         # `can_refit_full=True` because n_estimators is communicated at end of `_fit`:
         #  self.params_trained['n_estimators'] = bst.best_ntree_limit
-        return {'can_refit_full': True}
+        return {"can_refit_full": True}
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-import numpy as np
 from collections import OrderedDict
-from scipy.sparse import hstack, csr_matrix
+
+import numpy as np
+from scipy.sparse import csr_matrix, hstack
 from sklearn.base import BaseEstimator, TransformerMixin
+
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS
 
 from ..tabular_nn.utils.categorical_encoders import OneHotMergeRaresHandleUnknownEncoder
 
-
 _ag_to_xgbm_metric_dict = {
-    BINARY: dict(
-        accuracy='error',
-        log_loss='logloss',
-        roc_auc='auc'
-    ),
+    BINARY: dict(accuracy="error", log_loss="logloss", roc_auc="auc"),
     MULTICLASS: dict(
-        accuracy='merror',
-        log_loss='mlogloss',
+        accuracy="merror",
+        log_loss="mlogloss",
     ),
     REGRESSION: dict(
-        mean_absolute_error='mae',
-        mean_squared_error='rmse',
-        root_mean_squared_error='rmse',
+        mean_absolute_error="mae",
+        mean_squared_error="rmse",
+        root_mean_squared_error="rmse",
     ),
 }
 
 
 def convert_ag_metric_to_xgbm(ag_metric_name, problem_type):
     return _ag_to_xgbm_metric_dict.get(problem_type, dict()).get(ag_metric_name, None)
 
 
 def func_generator(metric, problem_type: str):
     """Create a custom metric compatible with XGBoost, based on the XGBoost 1.6+ API"""
     sign = -1 if metric.greater_is_better else 1
     needs_pred_proba = not metric.needs_pred
     if needs_pred_proba:
+
         def custom_metric(y_true, y_hat):
             return sign * metric(y_true, y_hat)
+
     else:
         if problem_type in [MULTICLASS, SOFTCLASS]:
+
             def custom_metric(y_true, y_hat):
                 y_hat = y_hat.argmax(axis=1)
                 return sign * metric(y_true, y_hat)
+
         elif problem_type == BINARY:
+
             def custom_metric(y_true, y_hat):
                 y_hat = np.round(y_hat)
                 return sign * metric(y_true, y_hat)
+
         else:
+
             def custom_metric(y_true, y_hat):
                 return sign * metric(y_true, y_hat)
 
     return custom_metric
 
 
 class OheFeatureGenerator(BaseEstimator, TransformerMixin):
     def __init__(self, max_levels=None):
         self._feature_map = OrderedDict()  # key: feature_name, value: feature_type
         self.labels = OrderedDict()
         self.cat_cols = []
         self.other_cols = []
         self.ohe_encs = None
-        self.max_levels=max_levels
+        self.max_levels = max_levels
 
     def fit(self, X, y=None):
-        self.cat_cols = list(X.select_dtypes(include='category').columns)
-        self.other_cols = list(X.select_dtypes(exclude='category').columns)
+        self.cat_cols = list(X.select_dtypes(include="category").columns)
+        self.other_cols = list(X.select_dtypes(exclude="category").columns)
         self.ohe_encs = OneHotMergeRaresHandleUnknownEncoder(max_levels=self.max_levels)
 
         if self.cat_cols:
             self.ohe_encs.fit(X[self.cat_cols])
             assert len(self.cat_cols) == len(self.ohe_encs.categories_)
-            
+
             for cat_col, categories in zip(self.cat_cols, self.ohe_encs.categories_):
                 categories_ = categories.tolist()
                 self.labels[cat_col] = categories_
                 # Update feature map ({name: type})
                 for category in categories_:
-                    self._feature_map[f"{cat_col}_{category}"] = 'i'  # one-hot encoding data type is boolean
+                    self._feature_map[f"{cat_col}_{category}"] = "i"  # one-hot encoding data type is boolean
 
         if self.other_cols:
             for c in self.other_cols:
-                self._feature_map[c] = 'int' if X[c].dtypes == int else 'float'
+                self._feature_map[c] = "int" if X[c].dtypes == int else "float"
         return self
 
     def transform(self, X, y=None):
         X_list = []
         if self.cat_cols:
             X_list.append(self.ohe_encs.transform(X[self.cat_cols]))
         if self.other_cols:
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from autogluon.core.constants import REGRESSION, QUANTILE
+from autogluon.core.constants import QUANTILE, REGRESSION
+
 from ..rf.rf_model import RFModel
 
 
 class XTModel(RFModel):
     """
     Extra Trees model (scikit-learn): https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.ExtraTreesClassifier.html#sklearn.ensemble.ExtraTreesClassifier
     """
+
     def _get_model_type(self):
         if self.problem_type == REGRESSION:
             from sklearn.ensemble import ExtraTreesRegressor
+
             return ExtraTreesRegressor
         elif self.problem_type == QUANTILE:
             from ..rf.rf_quantile import ExtraTreesQuantileRegressor
+
             return ExtraTreesQuantileRegressor
         else:
             from sklearn.ensemble import ExtraTreesClassifier
+
             return ExtraTreesClassifier
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,45 +20,43 @@
     InterpretableTabularPredictor should be used when accuracy is not important,
     and instead interpretability is the key requirement.
 
     Categorical features are one-hot-encoded to preserve interpretability.
 
     Stacking and bagging are not available in this predictor to preserve interpretability.
     """
-    def fit(self,
-            train_data,
-            tuning_data=None,
-            time_limit=None,
-            *,
-            presets='interpretable',
-            **kwargs):
-        logger.log(30, f'EXPERIMENTAL WARNING: Fitting {self.__class__.__name__}\n'
-                       f'\tThis class is experimental and could be removed without warning in a future release.\n'
-                       f'\tTo avoid confusing results, please only provide categorical and numeric features.\n'
-                       f'\tText and datetime features will result in confusing rules that are hard to interpret.')
+
+    def fit(self, train_data, tuning_data=None, time_limit=None, *, presets="interpretable", **kwargs):
+        logger.log(
+            30,
+            f"EXPERIMENTAL WARNING: Fitting {self.__class__.__name__}\n"
+            f"\tThis class is experimental and could be removed without warning in a future release.\n"
+            f"\tTo avoid confusing results, please only provide categorical and numeric features.\n"
+            f"\tText and datetime features will result in confusing rules that are hard to interpret.",
+        )
 
         return super().fit(
             train_data=train_data,
             tuning_data=tuning_data,
             time_limit=time_limit,
             presets=presets,
             **kwargs,
         )
 
     def _validate_fit_extra_kwargs(self, kwargs, extra_valid_keys=None) -> dict:
         kwargs = super()._validate_fit_extra_kwargs(kwargs=kwargs, extra_valid_keys=extra_valid_keys)
         print(kwargs)
-        if 'num_bag_folds' in kwargs and kwargs['num_bag_folds'] is not None and kwargs['num_bag_folds'] > 1:
-            raise ValueError(f'{self.__class__.__name__} does not support `num_bag_folds`.')
-        if 'num_bag_sets' in kwargs and kwargs['num_bag_sets'] is not None and kwargs['num_bag_sets'] > 1:
-            raise ValueError(f'{self.__class__.__name__} does not support `num_bag_sets`.')
-        if 'num_stack_levels' in kwargs and kwargs['num_stack_levels'] is not None and kwargs['num_stack_levels'] >= 1:
-            raise ValueError(f'{self.__class__.__name__} does not support `num_stack_levels`.')
-        if 'auto_stack' in kwargs and kwargs['auto_stack']:
-            raise ValueError(f'{self.__class__.__name__} does not support `auto_stack`.')
+        if "num_bag_folds" in kwargs and kwargs["num_bag_folds"] is not None and kwargs["num_bag_folds"] > 1:
+            raise ValueError(f"{self.__class__.__name__} does not support `num_bag_folds`.")
+        if "num_bag_sets" in kwargs and kwargs["num_bag_sets"] is not None and kwargs["num_bag_sets"] > 1:
+            raise ValueError(f"{self.__class__.__name__} does not support `num_bag_sets`.")
+        if "num_stack_levels" in kwargs and kwargs["num_stack_levels"] is not None and kwargs["num_stack_levels"] >= 1:
+            raise ValueError(f"{self.__class__.__name__} does not support `num_stack_levels`.")
+        if "auto_stack" in kwargs and kwargs["auto_stack"]:
+            raise ValueError(f"{self.__class__.__name__} does not support `auto_stack`.")
         return kwargs
 
     def leaderboard_interpretable(self, silent=False, **kwargs) -> pd.DataFrame:
         """
         Leaderboard of fitted interpretable models along with their corresponding complexities.
         Identical to `.leaderboard`, but with an additional 'complexity' column indicating
         the number of rules used in the model.
@@ -66,22 +64,22 @@
         Models which do not support calculating 'complexity' will be filtered from this result.
         """
         leaderboard = self.leaderboard(silent=True, **kwargs)
 
         complexities = []
         info = self.info()
         for i in range(leaderboard.shape[0]):
-            model_name = leaderboard.iloc[i]['model']
-            complexities.append(info['model_info'][model_name].get('complexity', np.nan))
-        leaderboard.insert(2, 'complexity', complexities)  # insert directly after score_test/score_val
+            model_name = leaderboard.iloc[i]["model"]
+            complexities.append(info["model_info"][model_name].get("complexity", np.nan))
+        leaderboard.insert(2, "complexity", complexities)  # insert directly after score_test/score_val
         leaderboard = leaderboard[~pd.isna(leaderboard.complexity)]  # remove non-interpretable models
-        score_col = 'score_test' if 'score_test' in leaderboard.columns else 'score_val'
-        leaderboard = leaderboard.sort_values(by=[score_col, 'complexity'], ascending=[False, True], ignore_index=True)
+        score_col = "score_test" if "score_test" in leaderboard.columns else "score_val"
+        leaderboard = leaderboard.sort_values(by=[score_col, "complexity"], ascending=[False, True], ignore_index=True)
         if not silent:
-            with pd.option_context('display.max_rows', None, 'display.max_columns', None, 'display.width', 1000):
+            with pd.option_context("display.max_rows", None, "display.max_columns", None, "display.width", 1000):
                 print(leaderboard)
         return leaderboard
 
     def print_interpretable_rules(self, complexity_threshold: int = 10, model_name: str = None):
         """
         Print the rules of the highest performing model below the complexity threshold.
 
@@ -94,22 +92,22 @@
             Optionally print rules for a particular model, ignoring the complexity threshold.
         """
         if model_name is None:
             summaries = self.leaderboard_interpretable(silent=True)
             summaries_filtered = summaries[summaries.complexity <= complexity_threshold]
             if summaries_filtered.shape[0] == 0:
                 summaries_filtered = summaries
-            model_name = summaries_filtered.iloc[0]['model']  # best model is at top
+            model_name = summaries_filtered.iloc[0]["model"]  # best model is at top
         agmodel = self._trainer.load_model(model_name)
         imodel = agmodel.model
         print(imodel)
 
     # TODO: I have not been able to extract any insight from the output of this method.
     #  I don't see how it is useful.
-    def explain_classification_errors(self, data, model = None, print_rules: bool = True):
+    def explain_classification_errors(self, data, model=None, print_rules: bool = True):
         """Explain classification errors by fitting a rule-based model to them
 
         Parameters
         ----------
         data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
             The data to make predictions for. Should contain same column names as training Dataset and follow same format
             (may contain extra columns that won't be used by Predictor, including the label-column itself).
@@ -122,14 +120,15 @@
 
         Returns
         -------
         cls : imodels.classifier
             Interpretable rule-based classifier with fit/predict methods
         """
         import imodels
+
         if model is None:
             model = self.get_model_best()
         data = self._get_dataset(data)
         predictions = self.predict(data=data, model=model, as_pandas=True)
         labels = data[self.label]
         data_transformed = self.transform_features(data=data, model=model)
         labels_transformed = self.transform_labels(labels=labels)
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/predictor/predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,45 +4,63 @@
 import inspect
 import logging
 import math
 import os
 import pprint
 import shutil
 import time
-from typing import Union, List, Tuple, Optional
 import warnings
+from typing import List, Optional, Tuple, Union
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from autogluon.common.loaders import load_json
 from autogluon.common.savers import save_json
 from autogluon.common.utils.file_utils import get_directory_size, get_directory_size_per_file
 from autogluon.common.utils.log_utils import add_log_to_file, set_logger_verbosity
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
-from autogluon.common.utils.utils import setup_outputdir, get_autogluon_metadata, compare_autogluon_metadata, check_saved_predictor_version
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, AUTO_WEIGHT, BALANCE_WEIGHT, PSEUDO_MODEL_SUFFIX, PROBLEM_TYPES_CLASSIFICATION
+from autogluon.common.utils.utils import (
+    check_saved_predictor_version,
+    compare_autogluon_metadata,
+    get_autogluon_metadata,
+    setup_outputdir,
+)
+from autogluon.core.constants import (
+    AUTO_WEIGHT,
+    BALANCE_WEIGHT,
+    BINARY,
+    MULTICLASS,
+    PROBLEM_TYPES_CLASSIFICATION,
+    PSEUDO_MODEL_SUFFIX,
+    QUANTILE,
+    REGRESSION,
+)
 from autogluon.core.data.label_cleaner import LabelCleanerMulticlassToBinary
 from autogluon.core.dataset import TabularDataset
 from autogluon.core.metrics import Scorer
 from autogluon.core.problem_type import problem_type_info
-from autogluon.core.pseudolabeling.pseudolabeling import filter_pseudo, filter_ensemble_pseudo
+from autogluon.core.pseudolabeling.pseudolabeling import filter_ensemble_pseudo, filter_pseudo
 from autogluon.core.scheduler.scheduler_factory import scheduler_factory
 from autogluon.core.trainer import AbstractTrainer
-from autogluon.core.utils import get_pred_from_proba_df
-from autogluon.core.utils import plot_performance_vs_trials, plot_summary_of_models, plot_tabular_models
+from autogluon.core.utils import (
+    get_pred_from_proba_df,
+    plot_performance_vs_trials,
+    plot_summary_of_models,
+    plot_tabular_models,
+)
 from autogluon.core.utils.decorators import apply_presets
 from autogluon.core.utils.loaders import load_pkl, load_str
 from autogluon.core.utils.savers import save_pkl, save_str
 from autogluon.core.utils.utils import default_holdout_frac
 
 from ..configs.feature_generator_presets import get_default_feature_generator
 from ..configs.hyperparameter_configs import get_hyperparameter_config
-from ..configs.presets_configs import tabular_presets_dict, tabular_presets_alias
+from ..configs.presets_configs import tabular_presets_alias, tabular_presets_dict
 from ..learner import AbstractTabularLearner, DefaultLearner
 from ..trainer.model_presets.presets import MODEL_TYPES
 
 logger = logging.getLogger(__name__)  # return autogluon root logger
 
 
 # TODO: num_bag_sets -> ag_args
@@ -55,14 +73,15 @@
 # TODO: Add logging comments that models are serialized on disk after fit
 # TODO: consider adding kwarg option for data which has already been preprocessed by feature generator to skip feature generation.
 # TODO: Resolve raw text feature usage in default feature generator
 
 # Done for Tabular
 # TODO: Remove all `time_limits` in project, replace with `time_limit`
 
+
 class TabularPredictor:
     """
     AutoGluon TabularPredictor predicts values in a column of a tabular dataset (classification or regression).
 
     Parameters
     ----------
     label : str
@@ -195,62 +214,65 @@
             Therefore, class_labels_internal_map would equal {'True': 1, 'False': 0}
         For other problem types, will equal None.
         For multiclass, it is possible for not all of the label values to have a mapping.
             This indicates that the internal models will never predict those missing labels, and training rows associated with the missing labels were dropped.
     """
 
     Dataset = TabularDataset
-    predictor_file_name = 'predictor.pkl'
-    _predictor_version_file_name = '__version__'
-    _predictor_metadata_file_name = 'metadata.json'
-    _predictor_log_file_name = 'predictor_log.txt'
+    predictor_file_name = "predictor.pkl"
+    _predictor_version_file_name = "__version__"
+    _predictor_metadata_file_name = "metadata.json"
+    _predictor_log_file_name = "predictor_log.txt"
 
     def __init__(
-            self,
-            label,
-            problem_type=None,
-            eval_metric=None,
-            path=None,
-            verbosity=2,
-            log_to_file=False,
-            log_file_path='auto',
-            sample_weight=None,
-            weight_evaluation=False,
-            groups=None,
-            **kwargs
+        self,
+        label,
+        problem_type=None,
+        eval_metric=None,
+        path=None,
+        verbosity=2,
+        log_to_file=False,
+        log_file_path="auto",
+        sample_weight=None,
+        weight_evaluation=False,
+        groups=None,
+        **kwargs,
     ):
         self.verbosity = verbosity
         set_logger_verbosity(self.verbosity)
         if sample_weight == AUTO_WEIGHT:  # TODO: update auto_weight strategy and make it the default
             sample_weight = None
             logger.log(15, f"{AUTO_WEIGHT} currently does not use any sample weights.")
         self.sample_weight = sample_weight
         self.weight_evaluation = weight_evaluation  # TODO: sample_weight and weight_evaluation can both be properties that link to self._learner.sample_weight, self._learner.weight_evaluation
         self._decision_threshold = None  # TODO: Each model should have its own decision threshold instead of one global threshold
         if self.sample_weight in [AUTO_WEIGHT, BALANCE_WEIGHT] and self.weight_evaluation:
             logger.warning(
-                f"We do not recommend specifying weight_evaluation when sample_weight='{self.sample_weight}', instead specify appropriate eval_metric.")
+                f"We do not recommend specifying weight_evaluation when sample_weight='{self.sample_weight}', instead specify appropriate eval_metric."
+            )
         self._validate_init_kwargs(kwargs)
         path = setup_outputdir(path)
-        self._setup_log_to_file(
-            path=path,
-            log_to_file=log_to_file,
-            log_file_path=log_file_path
-        )
-
-        learner_type = kwargs.pop('learner_type', DefaultLearner)
-        learner_kwargs = kwargs.pop('learner_kwargs', dict())
-        quantile_levels = kwargs.get('quantile_levels', None)
-
-        self._learner: AbstractTabularLearner = learner_type(path_context=path, label=label, feature_generator=None,
-                                                             eval_metric=eval_metric, problem_type=problem_type,
-                                                             quantile_levels=quantile_levels,
-                                                             sample_weight=self.sample_weight,
-                                                             weight_evaluation=self.weight_evaluation, groups=groups,
-                                                             **learner_kwargs)
+        self._setup_log_to_file(path=path, log_to_file=log_to_file, log_file_path=log_file_path)
+
+        learner_type = kwargs.pop("learner_type", DefaultLearner)
+        learner_kwargs = kwargs.pop("learner_kwargs", dict())
+        quantile_levels = kwargs.get("quantile_levels", None)
+
+        self._learner: AbstractTabularLearner = learner_type(
+            path_context=path,
+            label=label,
+            feature_generator=None,
+            eval_metric=eval_metric,
+            problem_type=problem_type,
+            quantile_levels=quantile_levels,
+            sample_weight=self.sample_weight,
+            weight_evaluation=self.weight_evaluation,
+            groups=groups,
+            **learner_kwargs,
+        )
         self._learner_type = type(self._learner)
         self._trainer = None
 
     @property
     def class_labels(self):
         return self._learner.class_labels
 
@@ -301,40 +323,43 @@
         """
         Set `predictor.decision_threshold`. Problem type must be 'binary', and the value must be between 0 and 1.
         """
         assert self.problem_type == BINARY
         assert decision_threshold >= 0
         assert decision_threshold <= 1
         if decision_threshold != self.decision_threshold:
-            logger.log(20, f'Updating predictor.decision_threshold from {self.decision_threshold} -> {decision_threshold}\n'
-                           f'\tThis will impact how prediction probabilities are converted to predictions in binary classification.\n'
-                           f'\tPrediction probabilities of the positive class >{decision_threshold} '
-                           f'will be predicted as the positive class ({self.positive_class}). '
-                           f'This can significantly impact metric scores.\n'
-                           f'\tYou can update this value via `predictor.set_decision_threshold`.\n'
-                           f'\tYou can calculate an optimal decision threshold on the validation data via `predictor.calibrate_decision_threshold()`.')
+            logger.log(
+                20,
+                f"Updating predictor.decision_threshold from {self.decision_threshold} -> {decision_threshold}\n"
+                f"\tThis will impact how prediction probabilities are converted to predictions in binary classification.\n"
+                f"\tPrediction probabilities of the positive class >{decision_threshold} "
+                f"will be predicted as the positive class ({self.positive_class}). "
+                f"This can significantly impact metric scores.\n"
+                f"\tYou can update this value via `predictor.set_decision_threshold`.\n"
+                f"\tYou can calculate an optimal decision threshold on the validation data via `predictor.calibrate_decision_threshold()`.",
+            )
         self._decision_threshold = decision_threshold
 
-    def features(self, feature_stage: str = 'original'):
+    def features(self, feature_stage: str = "original"):
         """
         Returns a list of feature names dependent on the value of feature_stage.
 
         Parameters
         ----------
         feature_stage : str, default = 'original'
             If 'original', returns the list of features specified in the original training data. This feature set is required in input data when making predictions.
             If 'transformed', returns the list of features after pre-processing by the feature generator.
 
         Returns
         -------
         Returns a list of feature names
         """
-        if feature_stage == 'original':
+        if feature_stage == "original":
             return self.feature_metadata_in.get_features()
-        elif feature_stage == 'transformed':
+        elif feature_stage == "transformed":
             return self.feature_metadata.get_features()
         else:
             raise ValueError(f"Unknown feature_stage: '{feature_stage}'. Must be one of {['original', 'transformed']}")
 
     @property
     def feature_metadata(self):
         return self._trainer.feature_metadata
@@ -348,28 +373,30 @@
         return self._learner.label
 
     @property
     def path(self):
         return self._learner.path
 
     @apply_presets(tabular_presets_dict, tabular_presets_alias)
-    def fit(self,
-            train_data,
-            tuning_data=None,
-            time_limit=None,
-            presets=None,
-            hyperparameters=None,
-            feature_metadata='infer',
-            infer_limit=None,
-            infer_limit_batch_size=None,
-            fit_weighted_ensemble=True,
-            calibrate_decision_threshold=False,
-            num_cpus='auto',
-            num_gpus='auto',
-            **kwargs):
+    def fit(
+        self,
+        train_data,
+        tuning_data=None,
+        time_limit=None,
+        presets=None,
+        hyperparameters=None,
+        feature_metadata="infer",
+        infer_limit=None,
+        infer_limit_batch_size=None,
+        fit_weighted_ensemble=True,
+        calibrate_decision_threshold=False,
+        num_cpus="auto",
+        num_gpus="auto",
+        **kwargs,
+    ):
         """
         Fit models to predict a column of a data table (label) based on the other columns (features).
 
         Parameters
         ----------
         train_data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
             Table of the training data, which is similar to a pandas DataFrame.
@@ -826,223 +853,245 @@
         To maximize predictive performance, use the following:
 
         >>> eval_metric = 'roc_auc'  # set this to the metric you ultimately care about
         >>> time_limit = 3600  # set as long as you are willing to wait (in sec)
         >>> predictor = TabularPredictor(label=label, eval_metric=eval_metric).fit(train_data, presets=['best_quality'], time_limit=time_limit)
         """
         if self._learner.is_fit:
-            raise AssertionError(
-                'Predictor is already fit! To fit additional models, refer to `predictor.fit_extra`, or create a new `Predictor`.')
+            raise AssertionError("Predictor is already fit! To fit additional models, refer to `predictor.fit_extra`, or create a new `Predictor`.")
         kwargs_orig = kwargs.copy()
         kwargs = self._validate_fit_kwargs(kwargs)
 
-        verbosity = kwargs.get('verbosity', self.verbosity)
+        verbosity = kwargs.get("verbosity", self.verbosity)
         set_logger_verbosity(verbosity)
 
         if presets:
             if not isinstance(presets, list):
                 presets = [presets]
-            logger.log(20, f'Presets specified: {presets}')
+            logger.log(20, f"Presets specified: {presets}")
 
         if verbosity >= 3:
-            logger.log(20, '============ fit kwarg info ============')
-            logger.log(20, 'User Specified kwargs:')
-            logger.log(20, f'{pprint.pformat(kwargs_orig)}')
-            logger.log(20, 'Full kwargs:')
-            logger.log(20, f'{pprint.pformat(kwargs)}')
-            logger.log(20, '========================================')
-
-        holdout_frac = kwargs['holdout_frac']
-        num_bag_folds = kwargs['num_bag_folds']
-        num_bag_sets = kwargs['num_bag_sets']
-        num_stack_levels = kwargs['num_stack_levels']
-        auto_stack = kwargs['auto_stack']
-        feature_generator = kwargs['feature_generator']
-        unlabeled_data = kwargs['unlabeled_data']
-        ag_args = kwargs['ag_args']
-        ag_args_fit = kwargs['ag_args_fit']
-        ag_args_ensemble = kwargs['ag_args_ensemble']
-        included_model_types = kwargs['included_model_types']
-        excluded_model_types = kwargs['excluded_model_types']
-        use_bag_holdout = kwargs['use_bag_holdout']
+            logger.log(20, "============ fit kwarg info ============")
+            logger.log(20, "User Specified kwargs:")
+            logger.log(20, f"{pprint.pformat(kwargs_orig)}")
+            logger.log(20, "Full kwargs:")
+            logger.log(20, f"{pprint.pformat(kwargs)}")
+            logger.log(20, "========================================")
+
+        holdout_frac = kwargs["holdout_frac"]
+        num_bag_folds = kwargs["num_bag_folds"]
+        num_bag_sets = kwargs["num_bag_sets"]
+        num_stack_levels = kwargs["num_stack_levels"]
+        auto_stack = kwargs["auto_stack"]
+        feature_generator = kwargs["feature_generator"]
+        unlabeled_data = kwargs["unlabeled_data"]
+        ag_args = kwargs["ag_args"]
+        ag_args_fit = kwargs["ag_args_fit"]
+        ag_args_ensemble = kwargs["ag_args_ensemble"]
+        included_model_types = kwargs["included_model_types"]
+        excluded_model_types = kwargs["excluded_model_types"]
+        use_bag_holdout = kwargs["use_bag_holdout"]
 
         if ag_args is None:
             ag_args = {}
-        ag_args = self._set_hyperparameter_tune_kwargs_in_ag_args(kwargs['hyperparameter_tune_kwargs'], ag_args,
-                                                                  time_limit=time_limit)
+        ag_args = self._set_hyperparameter_tune_kwargs_in_ag_args(kwargs["hyperparameter_tune_kwargs"], ag_args, time_limit=time_limit)
 
-        feature_generator_init_kwargs = kwargs['_feature_generator_kwargs']
+        feature_generator_init_kwargs = kwargs["_feature_generator_kwargs"]
         if feature_generator_init_kwargs is None:
             feature_generator_init_kwargs = dict()
 
-        train_data, tuning_data, unlabeled_data = self._validate_fit_data(train_data=train_data,
-                                                                          tuning_data=tuning_data,
-                                                                          unlabeled_data=unlabeled_data)
+        train_data, tuning_data, unlabeled_data = self._validate_fit_data(train_data=train_data, tuning_data=tuning_data, unlabeled_data=unlabeled_data)
         infer_limit, infer_limit_batch_size = self._validate_infer_limit(infer_limit=infer_limit, infer_limit_batch_size=infer_limit_batch_size)
 
         if hyperparameters is None:
-            hyperparameters = 'default'
+            hyperparameters = "default"
         if isinstance(hyperparameters, str):
             hyperparameters = get_hyperparameter_config(hyperparameters)
 
         # TODO: Hyperparam could have non-serializble objects. Save as pkl and loaded on demand
         # in case the hyperprams are large in memory
         self.fit_hyperparameters_ = hyperparameters
 
-        if 'enable_raw_text_features' not in feature_generator_init_kwargs:
+        if "enable_raw_text_features" not in feature_generator_init_kwargs:
             if self._check_if_hyperparameters_handle_text(hyperparameters=hyperparameters):
-                feature_generator_init_kwargs['enable_raw_text_features'] = True
+                feature_generator_init_kwargs["enable_raw_text_features"] = True
 
-        if feature_metadata is not None and isinstance(feature_metadata, str) and feature_metadata == 'infer':
+        if feature_metadata is not None and isinstance(feature_metadata, str) and feature_metadata == "infer":
             feature_metadata = None
-        self._set_feature_generator(feature_generator=feature_generator, feature_metadata=feature_metadata,
-                                    init_kwargs=feature_generator_init_kwargs)
+        self._set_feature_generator(feature_generator=feature_generator, feature_metadata=feature_metadata, init_kwargs=feature_generator_init_kwargs)
 
         if self.problem_type is not None:
             inferred_problem_type = self.problem_type
         else:
             inferred_problem_type = self._learner.infer_problem_type(y=train_data[self.label], silent=True)
 
         num_bag_folds, num_bag_sets, num_stack_levels = self._sanitize_stack_args(
-            num_bag_folds=num_bag_folds, num_bag_sets=num_bag_sets, num_stack_levels=num_stack_levels,
-            time_limit=time_limit, auto_stack=auto_stack, num_train_rows=len(train_data), problem_type=inferred_problem_type,
+            num_bag_folds=num_bag_folds,
+            num_bag_sets=num_bag_sets,
+            num_stack_levels=num_stack_levels,
+            time_limit=time_limit,
+            auto_stack=auto_stack,
+            num_train_rows=len(train_data),
+            problem_type=inferred_problem_type,
         )
         if auto_stack:
-            logger.log(20, f'Stack configuration (auto_stack={auto_stack}): '
-                           f'num_stack_levels={num_stack_levels}, num_bag_folds={num_bag_folds}, num_bag_sets={num_bag_sets}')
+            logger.log(
+                20,
+                f"Stack configuration (auto_stack={auto_stack}): "
+                f"num_stack_levels={num_stack_levels}, num_bag_folds={num_bag_folds}, num_bag_sets={num_bag_sets}",
+            )
 
         if holdout_frac is None:
-            holdout_frac = default_holdout_frac(len(train_data),
-                                                ag_args.get('hyperparameter_tune_kwargs', None) is not None)
+            holdout_frac = default_holdout_frac(len(train_data), ag_args.get("hyperparameter_tune_kwargs", None) is not None)
 
-        if kwargs['_save_bag_folds'] is not None:
-            if use_bag_holdout and not kwargs['_save_bag_folds']:
-                logger.log(30,
-                           f'WARNING: Attempted to disable saving of bagged fold models when `use_bag_holdout=True`. Forcing `save_bag_folds=True` to avoid errors.')
+        if kwargs["_save_bag_folds"] is not None:
+            if use_bag_holdout and not kwargs["_save_bag_folds"]:
+                logger.log(
+                    30,
+                    f"WARNING: Attempted to disable saving of bagged fold models when `use_bag_holdout=True`. Forcing `save_bag_folds=True` to avoid errors.",
+                )
             else:
                 if ag_args_ensemble is None:
                     ag_args_ensemble = {}
-                ag_args_ensemble['save_bag_folds'] = kwargs['_save_bag_folds']
+                ag_args_ensemble["save_bag_folds"] = kwargs["_save_bag_folds"]
 
         if time_limit is None:
             mb_mem_usage_train_data = get_approximate_df_mem_usage(train_data, sample_ratio=0.2).sum() / 1e6
             num_rows_train = len(train_data)
             if mb_mem_usage_train_data >= 50 or num_rows_train >= 100000:
-                logger.log(20,
-                           f'Warning: Training may take a very long time because `time_limit` was not specified and `train_data` is large ({num_rows_train} samples, {round(mb_mem_usage_train_data, 2)} MB).')
-                logger.log(20,
-                           f'\tConsider setting `time_limit` to ensure training finishes within an expected duration or experiment with a small portion of `train_data` to identify an ideal `presets` and `hyperparameters` configuration.')
+                logger.log(
+                    20,
+                    f"Warning: Training may take a very long time because `time_limit` was not specified and `train_data` is large ({num_rows_train} samples, {round(mb_mem_usage_train_data, 2)} MB).",
+                )
+                logger.log(
+                    20,
+                    f"\tConsider setting `time_limit` to ensure training finishes within an expected duration or experiment with a small portion of `train_data` to identify an ideal `presets` and `hyperparameters` configuration.",
+                )
 
         core_kwargs = {
-            'total_resources': {
-                'num_cpus': num_cpus,
-                'num_gpus': num_gpus,
+            "total_resources": {
+                "num_cpus": num_cpus,
+                "num_gpus": num_gpus,
             },
-            'ag_args': ag_args,
-            'ag_args_ensemble': ag_args_ensemble,
-            'ag_args_fit': ag_args_fit,
-            'included_model_types': included_model_types,
-            'excluded_model_types': excluded_model_types,
-            'feature_prune_kwargs': kwargs.get('feature_prune_kwargs', None)
+            "ag_args": ag_args,
+            "ag_args_ensemble": ag_args_ensemble,
+            "ag_args_fit": ag_args_fit,
+            "included_model_types": included_model_types,
+            "excluded_model_types": excluded_model_types,
+            "feature_prune_kwargs": kwargs.get("feature_prune_kwargs", None),
         }
         aux_kwargs = {}
         if fit_weighted_ensemble is False:
-            aux_kwargs['fit_weighted_ensemble'] = False
+            aux_kwargs["fit_weighted_ensemble"] = False
         self.save(silent=True)  # Save predictor to disk to enable prediction and training after interrupt
-        self._learner.fit(X=train_data, X_val=tuning_data, X_unlabeled=unlabeled_data,
-                          holdout_frac=holdout_frac, num_bag_folds=num_bag_folds, num_bag_sets=num_bag_sets,
-                          num_stack_levels=num_stack_levels,
-                          hyperparameters=hyperparameters, core_kwargs=core_kwargs, aux_kwargs=aux_kwargs,
-                          time_limit=time_limit, infer_limit=infer_limit, infer_limit_batch_size=infer_limit_batch_size,
-                          verbosity=verbosity, use_bag_holdout=use_bag_holdout)
+        self._learner.fit(
+            X=train_data,
+            X_val=tuning_data,
+            X_unlabeled=unlabeled_data,
+            holdout_frac=holdout_frac,
+            num_bag_folds=num_bag_folds,
+            num_bag_sets=num_bag_sets,
+            num_stack_levels=num_stack_levels,
+            hyperparameters=hyperparameters,
+            core_kwargs=core_kwargs,
+            aux_kwargs=aux_kwargs,
+            time_limit=time_limit,
+            infer_limit=infer_limit,
+            infer_limit_batch_size=infer_limit_batch_size,
+            verbosity=verbosity,
+            use_bag_holdout=use_bag_holdout,
+        )
         self._set_post_fit_vars()
 
         self._post_fit(
-            keep_only_best=kwargs['keep_only_best'],
-            refit_full=kwargs['refit_full'],
-            set_best_to_refit_full=kwargs['set_best_to_refit_full'],
-            save_space=kwargs['save_space'],
-            calibrate=kwargs['calibrate'],
+            keep_only_best=kwargs["keep_only_best"],
+            refit_full=kwargs["refit_full"],
+            set_best_to_refit_full=kwargs["set_best_to_refit_full"],
+            save_space=kwargs["save_space"],
+            calibrate=kwargs["calibrate"],
             calibrate_decision_threshold=calibrate_decision_threshold,
             infer_limit=infer_limit,
         )
         self.save()
         return self
 
-    def _post_fit(self, keep_only_best=False, refit_full=False, set_best_to_refit_full=False, save_space=False,
-                  calibrate=False, calibrate_decision_threshold=False, infer_limit=None):
+    def _post_fit(
+        self,
+        keep_only_best=False,
+        refit_full=False,
+        set_best_to_refit_full=False,
+        save_space=False,
+        calibrate=False,
+        calibrate_decision_threshold=False,
+        infer_limit=None,
+    ):
         if refit_full is True:
             if keep_only_best is True:
                 if set_best_to_refit_full is True:
-                    refit_full = 'best'
+                    refit_full = "best"
                 else:
                     logger.warning(
-                        f'refit_full was set to {refit_full}, but keep_only_best=True and set_best_to_refit_full=False. Disabling refit_full to avoid training models which would be automatically deleted.')
+                        f"refit_full was set to {refit_full}, but keep_only_best=True and set_best_to_refit_full=False. Disabling refit_full to avoid training models which would be automatically deleted."
+                    )
                     refit_full = False
             else:
-                refit_full = 'all'
+                refit_full = "all"
 
         if refit_full is not False:
             if infer_limit is not None:
                 infer_limit = infer_limit - self._learner.preprocess_1_time
             trainer_model_best = self._trainer.get_model_best(infer_limit=infer_limit)
-            logger.log(20, 'Automatically performing refit_full as a post-fit operation (due to `.fit(..., refit_full=True)`')
+            logger.log(20, "Automatically performing refit_full as a post-fit operation (due to `.fit(..., refit_full=True)`")
             self.refit_full(model=refit_full, set_best_to_refit_full=False)
             if set_best_to_refit_full:
                 model_full_dict = self._trainer.get_model_full_dict()
                 if trainer_model_best in model_full_dict:
                     self._trainer.model_best = model_full_dict[trainer_model_best]
                     # Note: model_best will be overwritten if additional training is done with new models, since model_best will have validation score of None and any new model will have a better validation score.
                     # This has the side-effect of having the possibility of model_best being overwritten by a worse model than the original model_best.
                     self._trainer.save()
                 elif trainer_model_best in model_full_dict.values():
                     self._trainer.model_best = trainer_model_best
                     self._trainer.save()
                 else:
                     logger.warning(
-                        f'Best model ({trainer_model_best}) is not present in refit_full dictionary. Training may have failed on the refit model. AutoGluon will default to using {trainer_model_best} for predictions.')
+                        f"Best model ({trainer_model_best}) is not present in refit_full dictionary. Training may have failed on the refit model. AutoGluon will default to using {trainer_model_best} for predictions."
+                    )
 
-        if calibrate == 'auto':
+        if calibrate == "auto":
             if self.problem_type in PROBLEM_TYPES_CLASSIFICATION and self.eval_metric.needs_proba:
                 calibrate = True
             elif self.problem_type == QUANTILE:
                 calibrate = True
             else:
                 calibrate = False
 
         if calibrate:
             if self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
                 self._trainer.calibrate_model()
             elif self.problem_type == QUANTILE:
                 self._trainer.calibrate_model()
             else:
-                logger.log(30, 'WARNING: `calibrate=True` is only applicable to classification or quantile regression problems. Skipping calibration...')
+                logger.log(30, "WARNING: `calibrate=True` is only applicable to classification or quantile regression problems. Skipping calibration...")
 
         if calibrate_decision_threshold:
             if self.problem_type != BINARY:
-                logger.log(30, 'WARNING: `calibrate_decision_threshold=True` is only applicable to binary classification. Skipping calibration...')
+                logger.log(30, "WARNING: `calibrate_decision_threshold=True` is only applicable to binary classification. Skipping calibration...")
             else:
                 best_threshold = self.calibrate_decision_threshold()
                 self.set_decision_threshold(decision_threshold=best_threshold)
 
         if keep_only_best:
-            self.delete_models(models_to_keep='best', dry_run=False)
+            self.delete_models(models_to_keep="best", dry_run=False)
 
         if save_space:
             self.save_space()
 
     # TODO: Consider adding infer_limit to fit_extra
-    def fit_extra(self,
-                  hyperparameters,
-                  time_limit=None,
-                  base_model_names=None,
-                  fit_weighted_ensemble=True,
-                  num_cpus='auto',
-                  num_gpus='auto',
-                  **kwargs):
+    def fit_extra(self, hyperparameters, time_limit=None, base_model_names=None, fit_weighted_ensemble=True, num_cpus="auto", num_gpus="auto", **kwargs):
         """
         Fits additional models after the original :meth:`TabularPredictor.fit` call.
         The original train_data and tuning_data will be used to train the models.
 
         Parameters
         ----------
         hyperparameters : str or dict
@@ -1073,173 +1122,186 @@
         **kwargs :
             Refer to kwargs documentation in :meth:`TabularPredictor.fit`.
             Note that the following kwargs are not available in `fit_extra` as they cannot be changed from their values set in `fit()`:
                 [`holdout_frac`, `num_bag_folds`, `auto_stack`, `feature_generator`, `unlabeled_data`]
             pseudo_data : pd.DataFrame, default = None
                 Data that has been self labeled by Autogluon model and will be incorporated into training during 'fit_extra'
         """
-        self._assert_is_fit('fit_extra')
+        self._assert_is_fit("fit_extra")
         time_start = time.time()
 
         kwargs_orig = kwargs.copy()
         kwargs = self._validate_fit_extra_kwargs(kwargs)
 
-        verbosity = kwargs.get('verbosity', self.verbosity)
+        verbosity = kwargs.get("verbosity", self.verbosity)
         set_logger_verbosity(verbosity)
 
         if verbosity >= 3:
-            logger.log(20, '============ fit kwarg info ============')
-            logger.log(20, 'User Specified kwargs:')
-            logger.log(20, f'{pprint.pformat(kwargs_orig)}')
-            logger.log(20, 'Full kwargs:')
-            logger.log(20, f'{pprint.pformat(kwargs)}')
-            logger.log(20, '========================================')
+            logger.log(20, "============ fit kwarg info ============")
+            logger.log(20, "User Specified kwargs:")
+            logger.log(20, f"{pprint.pformat(kwargs_orig)}")
+            logger.log(20, "Full kwargs:")
+            logger.log(20, f"{pprint.pformat(kwargs)}")
+            logger.log(20, "========================================")
 
         # TODO: Allow disable aux (default to disabled)
         # TODO: num_bag_sets
         # num_bag_sets = kwargs['num_bag_sets']
-        num_stack_levels = kwargs['num_stack_levels']
+        num_stack_levels = kwargs["num_stack_levels"]
         # save_bag_folds = kwargs['save_bag_folds']  # TODO: Enable
 
-        ag_args = kwargs['ag_args']
-        ag_args_fit = kwargs['ag_args_fit']
-        ag_args_ensemble = kwargs['ag_args_ensemble']
-        excluded_model_types = kwargs['excluded_model_types']
-        pseudo_data = kwargs.get('pseudo_data', None)
+        ag_args = kwargs["ag_args"]
+        ag_args_fit = kwargs["ag_args_fit"]
+        ag_args_ensemble = kwargs["ag_args_ensemble"]
+        excluded_model_types = kwargs["excluded_model_types"]
+        pseudo_data = kwargs.get("pseudo_data", None)
 
         # TODO: Since data preprocessor is fitted on original train_data it cannot account for if
         # labeled pseudo data has new labels unseen in the original train. Probably need to refit
         # data preprocessor if this is the case.
         if pseudo_data is not None:
             if self.label not in pseudo_data.columns:
-                raise ValueError('\'pseudo_data\' does not contain the labeled column.')
+                raise ValueError("'pseudo_data' does not contain the labeled column.")
 
             if self.sample_weight is not None:
-                raise ValueError('Applying \'sample_weight\' while calling \'fit_pseudolabel\' is not supported')
+                raise ValueError("Applying 'sample_weight' while calling 'fit_pseudolabel' is not supported")
 
             X_pseudo = pseudo_data.drop(columns=[self.label])
             y_pseudo_og = pseudo_data[self.label]
             X_pseudo = self._learner.transform_features(X_pseudo)
             y_pseudo = self._learner.label_cleaner.transform(y_pseudo_og)
 
             if np.isnan(y_pseudo.unique()).any():
-                raise Exception('NaN was found in the label column for pseudo labeled data.'
-                                'Please ensure no NaN values in target column')
+                raise Exception("NaN was found in the label column for pseudo labeled data." "Please ensure no NaN values in target column")
         else:
             X_pseudo = None
             y_pseudo = None
 
         if ag_args is None:
             ag_args = {}
-        ag_args = self._set_hyperparameter_tune_kwargs_in_ag_args(kwargs['hyperparameter_tune_kwargs'], ag_args,
-                                                                  time_limit=time_limit)
+        ag_args = self._set_hyperparameter_tune_kwargs_in_ag_args(kwargs["hyperparameter_tune_kwargs"], ag_args, time_limit=time_limit)
 
         fit_new_weighted_ensemble = False  # TODO: Add as option
         aux_kwargs = {}
         if fit_weighted_ensemble is False:
-            aux_kwargs = {'fit_weighted_ensemble': False}
+            aux_kwargs = {"fit_weighted_ensemble": False}
 
         if isinstance(hyperparameters, str):
             hyperparameters = get_hyperparameter_config(hyperparameters)
 
         if num_stack_levels is None:
             hyperparameter_keys = list(hyperparameters.keys())
             highest_level = 1
             for key in hyperparameter_keys:
                 if isinstance(key, int):
                     highest_level = max(key, highest_level)
             num_stack_levels = highest_level
 
         # TODO: make core_kwargs a kwargs argument to predictor.fit, add aux_kwargs to predictor.fit
         core_kwargs = {
-            'total_resources': {
-                'num_cpus': num_cpus,
-                'num_gpus': num_gpus,
+            "total_resources": {
+                "num_cpus": num_cpus,
+                "num_gpus": num_gpus,
             },
-            'ag_args': ag_args,
-            'ag_args_ensemble': ag_args_ensemble,
-            'ag_args_fit': ag_args_fit,
-            'excluded_model_types': excluded_model_types
+            "ag_args": ag_args,
+            "ag_args_ensemble": ag_args_ensemble,
+            "ag_args_fit": ag_args_fit,
+            "excluded_model_types": excluded_model_types,
         }
 
         if X_pseudo is not None and y_pseudo is not None:
-            core_kwargs['X_pseudo'] = X_pseudo
-            core_kwargs['y_pseudo'] = y_pseudo
+            core_kwargs["X_pseudo"] = X_pseudo
+            core_kwargs["y_pseudo"] = y_pseudo
 
         # TODO: Add special error message if called and training/val data was not cached.
         X, y, X_val, y_val = self._trainer.load_data()
 
         if y_pseudo is not None and self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
             y_og = self._learner.label_cleaner.inverse_transform(y)
             y_og_classes = y_og.unique()
             y_pseudo_classes = y_pseudo_og.unique()
             matching_classes = np.in1d(y_pseudo_classes, y_og_classes)
 
             if not matching_classes.all():
-                raise Exception(f'Pseudo training data contains classes not in original train data: {y_pseudo_classes[~matching_classes]}')
+                raise Exception(f"Pseudo training data contains classes not in original train data: {y_pseudo_classes[~matching_classes]}")
 
-        name_suffix = kwargs.get('name_suffix', '')
+        name_suffix = kwargs.get("name_suffix", "")
 
         fit_models = self._trainer.train_multi_levels(
-            X=X, y=y, hyperparameters=hyperparameters, X_val=X_val, y_val=y_val,
-            base_model_names=base_model_names, time_limit=time_limit, relative_stack=True, level_end=num_stack_levels,
-            core_kwargs=core_kwargs, aux_kwargs=aux_kwargs, name_suffix=name_suffix
+            X=X,
+            y=y,
+            hyperparameters=hyperparameters,
+            X_val=X_val,
+            y_val=y_val,
+            base_model_names=base_model_names,
+            time_limit=time_limit,
+            relative_stack=True,
+            level_end=num_stack_levels,
+            core_kwargs=core_kwargs,
+            aux_kwargs=aux_kwargs,
+            name_suffix=name_suffix,
         )
 
         if time_limit is not None:
             time_limit = time_limit - (time.time() - time_start)
 
         if fit_new_weighted_ensemble:
             if time_limit is not None:
                 time_limit_weighted = max(time_limit, 60)
             else:
                 time_limit_weighted = None
             fit_models += self.fit_weighted_ensemble(time_limit=time_limit_weighted)
 
         self._post_fit(
-            keep_only_best=kwargs['keep_only_best'],
-            refit_full=kwargs['refit_full'],
-            set_best_to_refit_full=kwargs['set_best_to_refit_full'],
-            save_space=kwargs['save_space'],
-            calibrate=kwargs['calibrate']
+            keep_only_best=kwargs["keep_only_best"],
+            refit_full=kwargs["refit_full"],
+            set_best_to_refit_full=kwargs["set_best_to_refit_full"],
+            save_space=kwargs["save_space"],
+            calibrate=kwargs["calibrate"],
         )
         self.save()
         return self
 
     def _get_all_fit_extra_args(self):
         ret = list(self._fit_extra_kwargs_dict().keys()) + list(inspect.signature(self.fit_extra).parameters.keys())
-        ret.remove('kwargs')
+        ret.remove("kwargs")
 
         return ret
 
     def _fit_weighted_ensemble_pseudo(self):
         """
         Fits weighted ensemble on top models trained with pseudo labeling, then if new
         weighted ensemble model is best model then sets `model_best` in trainer to
         weighted ensemble model.
         """
-        logger.log(15, 'Fitting weighted ensemble using top models')
+        logger.log(15, "Fitting weighted ensemble using top models")
         weighted_ensemble_model_name = self.fit_weighted_ensemble()[0]
 
         # TODO: This is a hack! self.predict_prob does not update to use weighted ensemble
         # if it's the best model.
         # TODO: There should also be PL added to weighted ensemble model name to notify
         # users it is a model trained with PL models if they are indeed ensembled
-        model_best_name = self._trainer.leaderboard().iloc[0]['model']
+        model_best_name = self._trainer.leaderboard().iloc[0]["model"]
         if model_best_name == weighted_ensemble_model_name:
             self._trainer.model_best = model_best_name
             self._trainer.save()
-            logger.log(15, 'Weighted ensemble was the best model for current iteration of pseudo labeling')
+            logger.log(15, "Weighted ensemble was the best model for current iteration of pseudo labeling")
         else:
-            logger.log(15, 'Weighted ensemble was not the best model for current iteration of pseudo labeling')
+            logger.log(15, "Weighted ensemble was not the best model for current iteration of pseudo labeling")
 
-    def _run_pseudolabeling(self, unlabeled_data: pd.DataFrame, max_iter: int,
-                            return_pred_prob: bool = False, use_ensemble: bool = False,
-                            fit_ensemble: bool = False, fit_ensemble_every_iter: bool = False,
-                            **kwargs):
+    def _run_pseudolabeling(
+        self,
+        unlabeled_data: pd.DataFrame,
+        max_iter: int,
+        return_pred_prob: bool = False,
+        use_ensemble: bool = False,
+        fit_ensemble: bool = False,
+        fit_ensemble_every_iter: bool = False,
+        **kwargs,
+    ):
         """
         Runs pseudolabeling algorithm using the same hyperparameters and model and fit settings
         used in original model unless specified by the user. This is an internal function that iteratively
         self labels unlabeled test data then incorporates all self labeled data above a threshold into training.
         Will keep incorporating self labeled data into training until validation score does not improve
 
         Parameters:
@@ -1263,35 +1325,34 @@
             for every iteration of pseudo label algorithm. If False and fit_ensemble
             is True, will just do it at the very end of training pseudo labeled models.
 
         Returns:
         --------
         self: TabularPredictor
         """
-        previous_score = self.info()['best_model_score_val']
+        previous_score = self.info()["best_model_score_val"]
         y_pseudo_og = pd.Series()
         if return_pred_prob:
             if self.problem_type is REGRESSION:
                 y_pred_proba_og = pd.Series()
             else:
                 y_pred_proba_og = pd.DataFrame()
         X_test = unlabeled_data.copy()
 
         for i in range(max_iter):
             if len(X_test) == 0:
-                logger.log(20, f'No more unlabeled data to pseudolabel. Done with pseudolabeling...')
+                logger.log(20, f"No more unlabeled data to pseudolabel. Done with pseudolabeling...")
                 break
 
             iter_print = str(i + 1)
-            logger.log(20, f'Beginning iteration {iter_print} of pseudolabeling out of max: {max_iter}')
+            logger.log(20, f"Beginning iteration {iter_print} of pseudolabeling out of max: {max_iter}")
 
             if use_ensemble:
                 if self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
-                    test_pseudo_idxes_true, y_pred_proba, y_pred = filter_ensemble_pseudo(predictor=self,
-                                                                                          unlabeled_data=X_test)
+                    test_pseudo_idxes_true, y_pred_proba, y_pred = filter_ensemble_pseudo(predictor=self, unlabeled_data=X_test)
                 else:
                     test_pseudo_idxes_true, y_pred = filter_ensemble_pseudo(predictor=self, unlabeled_data=X_test)
                     y_pred_proba = y_pred.copy()
             else:
                 if self.can_predict_proba:
                     y_pred_proba = self.predict_proba(data=X_test, as_multiclass=True)
                     y_pred = get_pred_from_proba_df(y_pred_proba, problem_type=self.problem_type)
@@ -1303,39 +1364,43 @@
             if return_pred_prob:
                 if i == 0:
                     y_pred_proba_og = y_pred_proba
                 else:
                     y_pred_proba_og.loc[test_pseudo_idxes_true.index] = y_pred_proba.loc[test_pseudo_idxes_true.index]
 
             if len(test_pseudo_idxes_true) < 1:
-                logger.log(20,
-                           f'Could not confidently assign pseudolabels for any of the provided rows in iteration: {iter_print}. Done with pseudolabeling...')
+                logger.log(
+                    20, f"Could not confidently assign pseudolabels for any of the provided rows in iteration: {iter_print}. Done with pseudolabeling..."
+                )
                 break
             else:
-                logger.log(20,
-                           f'Pseudolabeling algorithm confidently assigned pseudolabels to: {len(test_pseudo_idxes_true)} rows of data'
-                           f'on iteration: {iter_print}. Adding to train data')
+                logger.log(
+                    20,
+                    f"Pseudolabeling algorithm confidently assigned pseudolabels to: {len(test_pseudo_idxes_true)} rows of data"
+                    f"on iteration: {iter_print}. Adding to train data",
+                )
 
             test_pseudo_idxes = pd.Series(data=False, index=y_pred_proba.index)
             test_pseudo_idxes[test_pseudo_idxes_true.index] = True
 
             y_pseudo_og = y_pseudo_og.append(y_pred.loc[test_pseudo_idxes_true.index], verify_integrity=True)
 
             pseudo_data = unlabeled_data.loc[y_pseudo_og.index]
             pseudo_data[self.label] = y_pseudo_og
-            self.fit_extra(pseudo_data=pseudo_data, name_suffix=PSEUDO_MODEL_SUFFIX.format(iter=(i + 1)),
-                           **kwargs)
+            self.fit_extra(pseudo_data=pseudo_data, name_suffix=PSEUDO_MODEL_SUFFIX.format(iter=(i + 1)), **kwargs)
 
             if fit_ensemble and fit_ensemble_every_iter:
                 self._fit_weighted_ensemble_pseudo()
 
-            current_score = self.info()['best_model_score_val']
-            logger.log(20,
-                       f'Pseudolabeling algorithm changed validation score from: {previous_score}, to: {current_score}'
-                       f' using evaluation metric: {self.eval_metric.name}')
+            current_score = self.info()["best_model_score_val"]
+            logger.log(
+                20,
+                f"Pseudolabeling algorithm changed validation score from: {previous_score}, to: {current_score}"
+                f" using evaluation metric: {self.eval_metric.name}",
+            )
 
             if previous_score >= current_score:
                 break
             else:
                 # Cut down X_test to not include pseudo labeled data
                 X_test = X_test.loc[test_pseudo_idxes[~test_pseudo_idxes].index]
                 previous_score = current_score
@@ -1348,17 +1413,24 @@
                 y_pred_proba_og = self.predict(unlabeled_data)
 
         if return_pred_prob:
             return self, y_pred_proba_og
         else:
             return self
 
-    def fit_pseudolabel(self, pseudo_data: pd.DataFrame, max_iter: int = 5, return_pred_prob: bool = False,
-                        use_ensemble: bool = False, fit_ensemble: bool = False, fit_ensemble_every_iter: bool = False,
-                        **kwargs):
+    def fit_pseudolabel(
+        self,
+        pseudo_data: pd.DataFrame,
+        max_iter: int = 5,
+        return_pred_prob: bool = False,
+        use_ensemble: bool = False,
+        fit_ensemble: bool = False,
+        fit_ensemble_every_iter: bool = False,
+        **kwargs,
+    ):
         """
         If 'pseudo_data' is labeled then incorporates all test_data into train_data for
         newly fit models. If 'pseudo_data' is unlabeled then 'fit_pseudolabel' will self label the
         data and will augment the original training data by adding all the self labeled
         data that meets a criteria (For example all rows with predictive prob above 95%). If
         predictor is fit then will call fit_extra with added training data, if predictor
         is not fit then will fit model on train_data then run.
@@ -1394,73 +1466,85 @@
 
         Returns
         -------
         self : TabularPredictor
             Returns self, which is a Python class of TabularPredictor
         """
         if len(pseudo_data) < 1:
-            raise Exception('No pseudo data given')
+            raise Exception("No pseudo data given")
 
-        self._validate_unique_indices(pseudo_data, 'pseudo_data')
+        self._validate_unique_indices(pseudo_data, "pseudo_data")
 
         if not self._learner.is_fit:
-            if 'train_data' not in kwargs.keys():
-                Exception('Autogluon is required to be fit or given \'train_data\' in order to run \'fit_pseudolabel\'.'
-                          ' Autogluon is not fit and \'train_data\' was not given')
+            if "train_data" not in kwargs.keys():
+                Exception(
+                    "Autogluon is required to be fit or given 'train_data' in order to run 'fit_pseudolabel'."
+                    " Autogluon is not fit and 'train_data' was not given"
+                )
 
-            logger.log(20,
-                       f'Predictor not fit prior to pseudolabeling. Fitting now...')
+            logger.log(20, f"Predictor not fit prior to pseudolabeling. Fitting now...")
             self.fit(**kwargs)
 
-        if self.problem_type is MULTICLASS and self.eval_metric.name != 'accuracy':
-            logger.warning('AutoGluon has detected the problem type as \'multiclass\' and '
-                           f'eval_metric is {self.eval_metric.name}, we recommend using'
-                           f'fit_pseudolabeling when eval metric is \'accuracy\'')
+        if self.problem_type is MULTICLASS and self.eval_metric.name != "accuracy":
+            logger.warning(
+                "AutoGluon has detected the problem type as 'multiclass' and "
+                f"eval_metric is {self.eval_metric.name}, we recommend using"
+                f"fit_pseudolabeling when eval metric is 'accuracy'"
+            )
 
         is_labeled = self.label in pseudo_data.columns
 
-        hyperparameters = kwargs.get('hyperparameters', None)
+        hyperparameters = kwargs.get("hyperparameters", None)
         if hyperparameters is None:
             if self._learner.is_fit:
                 hyperparameters = self.fit_hyperparameters_
         elif isinstance(hyperparameters, str):
             hyperparameters = get_hyperparameter_config(hyperparameters)
 
-        kwargs['hyperparameters'] = hyperparameters
+        kwargs["hyperparameters"] = hyperparameters
         fit_extra_args = self._get_all_fit_extra_args()
         fit_extra_kwargs = {key: value for key, value in kwargs.items() if key in fit_extra_args}
         if is_labeled:
             logger.log(20, "Fitting predictor using the provided pseudolabeled examples as extra training data...")
-            self.fit_extra(pseudo_data=pseudo_data, name_suffix=PSEUDO_MODEL_SUFFIX.format(iter='')[:-1],
-                           **fit_extra_kwargs)
+            self.fit_extra(pseudo_data=pseudo_data, name_suffix=PSEUDO_MODEL_SUFFIX.format(iter="")[:-1], **fit_extra_kwargs)
 
             if fit_ensemble:
-                logger.log(15, 'Fitting weighted ensemble model using best models')
+                logger.log(15, "Fitting weighted ensemble model using best models")
                 self.fit_weighted_ensemble()
 
             if return_pred_prob:
                 y_pred_proba = self.predict_proba(pseudo_data) if self.can_predict_proba else self.predict(pseudo_data)
                 return self, y_pred_proba
             else:
                 return self
         else:
-            logger.log(20, 'Given test_data for pseudo labeling did not contain labels. '
-                           'AutoGluon will assign pseudo labels to data and use it for extra training data...')
-            return self._run_pseudolabeling(unlabeled_data=pseudo_data, max_iter=max_iter,
-                                            return_pred_prob=return_pred_prob, use_ensemble=use_ensemble,
-                                            fit_ensemble=fit_ensemble, fit_ensemble_every_iter=fit_ensemble_every_iter,
-                                            **fit_extra_kwargs)
-
-    def predict(self,
-                data: str | TabularDataset | pd.DataFrame,
-                model: str | None = None,
-                as_pandas: bool = True,
-                transform_features: bool = True,
-                *,
-                decision_threshold: float | None = None):
+            logger.log(
+                20,
+                "Given test_data for pseudo labeling did not contain labels. "
+                "AutoGluon will assign pseudo labels to data and use it for extra training data...",
+            )
+            return self._run_pseudolabeling(
+                unlabeled_data=pseudo_data,
+                max_iter=max_iter,
+                return_pred_prob=return_pred_prob,
+                use_ensemble=use_ensemble,
+                fit_ensemble=fit_ensemble,
+                fit_ensemble_every_iter=fit_ensemble_every_iter,
+                **fit_extra_kwargs,
+            )
+
+    def predict(
+        self,
+        data: str | TabularDataset | pd.DataFrame,
+        model: str | None = None,
+        as_pandas: bool = True,
+        transform_features: bool = True,
+        *,
+        decision_threshold: float | None = None,
+    ):
         """
         Use trained models to produce predictions of `label` column values for new data.
 
         Parameters
         ----------
         data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
             The data to make predictions for. Should contain same column names as training Dataset and follow same format
@@ -1484,26 +1568,28 @@
             Useful to set for metrics such as `balanced_accuracy` and `f1` as `0.5` is often not an optimal threshold.
             Predictions are calculated via the following logic on the positive class: `1 if pred > decision_threshold else 0`
 
         Returns
         -------
         Array of predictions, one corresponding to each row in given dataset. Either :class:`np.ndarray` or :class:`pd.Series` depending on `as_pandas` argument.
         """
-        self._assert_is_fit('predict')
+        self._assert_is_fit("predict")
         data = self._get_dataset(data)
         if decision_threshold is None:
             decision_threshold = self.decision_threshold
         return self._learner.predict(X=data, model=model, as_pandas=as_pandas, transform_features=transform_features, decision_threshold=decision_threshold)
 
-    def predict_proba(self,
-                      data: str | TabularDataset | pd.DataFrame,
-                      model: str | None = None,
-                      as_pandas: bool = True,
-                      as_multiclass: bool = True,
-                      transform_features: bool = True):
+    def predict_proba(
+        self,
+        data: str | TabularDataset | pd.DataFrame,
+        model: str | None = None,
+        as_pandas: bool = True,
+        as_multiclass: bool = True,
+        transform_features: bool = True,
+    ):
         """
         Use trained models to produce predicted class probabilities rather than class-labels (if task is classification).
         If `predictor.problem_type` is regression or quantile, this will raise an AssertionError.
 
         Parameters
         ----------
         data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
@@ -1530,25 +1616,25 @@
 
         Returns
         -------
         Array of predicted class-probabilities, corresponding to each row in the given data.
         May be a :class:`np.ndarray` or :class:`pd.DataFrame` / :class:`pd.Series` depending on `as_pandas` and `as_multiclass` arguments and the type of prediction problem.
         For binary classification problems, the output contains for each datapoint the predicted probabilities of the negative and positive classes, unless you specify `as_multiclass=False`.
         """
-        self._assert_is_fit('predict_proba')
+        self._assert_is_fit("predict_proba")
         if not self.can_predict_proba:
-            raise AssertionError(f'`predictor.predict_proba` is not supported when problem_type="{self.problem_type}". '
-                                 f'Please call `predictor.predict` instead. '
-                                 f'You can check the value of `predictor.can_predict_proba` to tell if predict_proba is valid.')
+            raise AssertionError(
+                f'`predictor.predict_proba` is not supported when problem_type="{self.problem_type}". '
+                f"Please call `predictor.predict` instead. "
+                f"You can check the value of `predictor.can_predict_proba` to tell if predict_proba is valid."
+            )
         data = self._get_dataset(data)
         return self._learner.predict_proba(X=data, model=model, as_pandas=as_pandas, as_multiclass=as_multiclass, transform_features=transform_features)
 
-    def get_pred_from_proba(self,
-                            y_pred_proba: pd.DataFrame | np.ndarray,
-                            decision_threshold: float | None = None) -> pd.Series | np.array:
+    def get_pred_from_proba(self, y_pred_proba: pd.DataFrame | np.ndarray, decision_threshold: float | None = None) -> pd.Series | np.array:
         """
         Given prediction probabilities, convert to predictions.
 
         Parameters
         ----------
         y_pred_proba : :class:`pd.DataFrame` or :class:`np.ndarray`
             The prediction probabilities to convert to predictions.
@@ -1584,15 +1670,15 @@
 
     @property
     def can_predict_proba(self) -> bool:
         """
         Return True if predictor can return prediction probabilities via `.predict_proba`, otherwise return False.
         Raises an AssertionError if called before fitting.
         """
-        self._assert_is_fit('can_predict_proba')
+        self._assert_is_fit("can_predict_proba")
         return problem_type_info.can_predict_proba(problem_type=self.problem_type)
 
     def evaluate(self, data, model=None, decision_threshold=None, silent=False, auxiliary_metrics=True, detailed_report=False) -> dict:
         """
         Report the predictive performance evaluated over a given dataset.
         This is basically a shortcut for: `pred_proba = predict_proba(data); evaluate_predictions(data[label], pred_proba)`.
 
@@ -1619,31 +1705,39 @@
 
         Returns
         -------
         Returns dict where keys = metrics, values = performance along each metric. To get the `eval_metric` score, do `output[predictor.eval_metric.name]`
         NOTE: Metrics scores always show in higher is better form.
         This means that metrics such as log_loss and root_mean_squared_error will have their signs FLIPPED, and values will be negative.
         """
-        self._assert_is_fit('evaluate')
+        self._assert_is_fit("evaluate")
         data = self._get_dataset(data)
         if decision_threshold is None:
             decision_threshold = self.decision_threshold
         if self.can_predict_proba:
             y_pred = self.predict_proba(data=data, model=model)
         else:
             y_pred = self.predict(data=data, model=model)
         if self.sample_weight is not None and self.weight_evaluation and self.sample_weight in data:
             sample_weight = data[self.sample_weight]
         else:
             sample_weight = None
-        return self.evaluate_predictions(y_true=data[self.label], y_pred=y_pred, sample_weight=sample_weight,
-                                         decision_threshold=decision_threshold, silent=silent,
-                                         auxiliary_metrics=auxiliary_metrics, detailed_report=detailed_report)
+        return self.evaluate_predictions(
+            y_true=data[self.label],
+            y_pred=y_pred,
+            sample_weight=sample_weight,
+            decision_threshold=decision_threshold,
+            silent=silent,
+            auxiliary_metrics=auxiliary_metrics,
+            detailed_report=detailed_report,
+        )
 
-    def evaluate_predictions(self, y_true, y_pred, sample_weight=None, decision_threshold=None, silent=False, auxiliary_metrics=True, detailed_report=False) -> dict:
+    def evaluate_predictions(
+        self, y_true, y_pred, sample_weight=None, decision_threshold=None, silent=False, auxiliary_metrics=True, detailed_report=False
+    ) -> dict:
         """
         Evaluate the provided prediction probabilities against ground truth labels.
         Evaluation is based on the `eval_metric` previously specified in init, or default metrics if none was specified.
 
         Parameters
         ----------
         y_true : :class:`np.array` or :class:`pd.Series`
@@ -1670,26 +1764,34 @@
         -------
         Returns dict where keys = metrics, values = performance along each metric.
         NOTE: Metrics scores always show in higher is better form.
         This means that metrics such as log_loss and root_mean_squared_error will have their signs FLIPPED, and values will be negative.
         """
         if decision_threshold is None:
             decision_threshold = self.decision_threshold
-        return self._learner.evaluate_predictions(y_true=y_true, y_pred=y_pred, sample_weight=sample_weight,
-                                                  decision_threshold=decision_threshold, silent=silent,
-                                                  auxiliary_metrics=auxiliary_metrics, detailed_report=detailed_report)
-
-    def leaderboard(self,
-                    data: str | TabularDataset | pd.DataFrame | None = None,
-                    extra_info: bool = False,
-                    extra_metrics: list | None = None,
-                    decision_threshold: float | None = None,
-                    only_pareto_frontier: bool = False,
-                    skip_score: bool = False,
-                    silent: bool = False) -> pd.DataFrame:
+        return self._learner.evaluate_predictions(
+            y_true=y_true,
+            y_pred=y_pred,
+            sample_weight=sample_weight,
+            decision_threshold=decision_threshold,
+            silent=silent,
+            auxiliary_metrics=auxiliary_metrics,
+            detailed_report=detailed_report,
+        )
+
+    def leaderboard(
+        self,
+        data: str | TabularDataset | pd.DataFrame | None = None,
+        extra_info: bool = False,
+        extra_metrics: list | None = None,
+        decision_threshold: float | None = None,
+        only_pareto_frontier: bool = False,
+        skip_score: bool = False,
+        silent: bool = False,
+    ) -> pd.DataFrame:
         """
         Output summary of information about models produced during `fit()` as a :class:`pd.DataFrame`.
         Includes information on test and validation scores for all models, model training times, inference times, and stack levels.
         Output DataFrame columns include:
             'model': The name of the model.
 
             'score_val': The validation score of the model on the 'eval_metric'.
@@ -1813,28 +1915,37 @@
         silent : bool, default = False
             Should leaderboard DataFrame be printed?
 
         Returns
         -------
         :class:`pd.DataFrame` of model performance summary information.
         """
-        self._assert_is_fit('leaderboard')
+        self._assert_is_fit("leaderboard")
         data = self._get_dataset(data, allow_nan=True)
         if decision_threshold is None:
             decision_threshold = self.decision_threshold
-        return self._learner.leaderboard(X=data, extra_info=extra_info, extra_metrics=extra_metrics, decision_threshold=decision_threshold,
-                                         only_pareto_frontier=only_pareto_frontier, skip_score=skip_score, silent=silent)
+        return self._learner.leaderboard(
+            X=data,
+            extra_info=extra_info,
+            extra_metrics=extra_metrics,
+            decision_threshold=decision_threshold,
+            only_pareto_frontier=only_pareto_frontier,
+            skip_score=skip_score,
+            silent=silent,
+        )
 
-    def predict_proba_multi(self,
-                            data=None,
-                            models: List[str] = None,
-                            as_pandas: bool = True,
-                            as_multiclass: bool = True,
-                            transform_features: bool = True,
-                            inverse_transform: bool = True) -> dict:
+    def predict_proba_multi(
+        self,
+        data=None,
+        models: List[str] = None,
+        as_pandas: bool = True,
+        as_multiclass: bool = True,
+        transform_features: bool = True,
+        inverse_transform: bool = True,
+    ) -> dict:
         """
         Returns a dictionary of prediction probabilities where the key is
         the model name and the value is the model's prediction probabilities on the data.
 
         Equivalent output to:
         ```
         predict_proba_dict = {}
@@ -1873,35 +1984,36 @@
             If True, will return prediction probabilities in the original format.
             If False (advanced), will return prediction probabilities in AutoGluon's internal format.
 
         Returns
         -------
         Dictionary with model names as keys and model prediction probabilities as values.
         """
-        self._assert_is_fit('predict_proba_multi')
+        self._assert_is_fit("predict_proba_multi")
         if not self.can_predict_proba:
-            raise AssertionError(f'`predictor.predict_proba_multi` is not supported when problem_type="{self.problem_type}". '
-                                 f'Please call `predictor.predict_multi` instead. '
-                                 f'You can check the value of `predictor.can_predict_proba` to tell if predict_proba_multi is valid.')
+            raise AssertionError(
+                f'`predictor.predict_proba_multi` is not supported when problem_type="{self.problem_type}". '
+                f"Please call `predictor.predict_multi` instead. "
+                f"You can check the value of `predictor.can_predict_proba` to tell if predict_proba_multi is valid."
+            )
         data = self._get_dataset(data, allow_nan=True)
-        return self._learner.predict_proba_multi(X=data,
-                                                 models=models,
-                                                 as_pandas=as_pandas,
-                                                 as_multiclass=as_multiclass,
-                                                 transform_features=transform_features,
-                                                 inverse_transform=inverse_transform)
-
-    def predict_multi(self,
-                      data=None,
-                      models: List[str] = None,
-                      as_pandas: bool = True,
-                      transform_features: bool = True,
-                      inverse_transform: bool = True,
-                      *,
-                      decision_threshold: float = None) -> dict:
+        return self._learner.predict_proba_multi(
+            X=data, models=models, as_pandas=as_pandas, as_multiclass=as_multiclass, transform_features=transform_features, inverse_transform=inverse_transform
+        )
+
+    def predict_multi(
+        self,
+        data=None,
+        models: List[str] = None,
+        as_pandas: bool = True,
+        transform_features: bool = True,
+        inverse_transform: bool = True,
+        *,
+        decision_threshold: float = None,
+    ) -> dict:
         """
         Returns a dictionary of predictions where the key is
         the model name and the value is the model's prediction probabilities on the data.
 
         Equivalent output to:
         ```
         predict_dict = {}
@@ -1942,24 +2054,26 @@
             Useful to set for metrics such as `balanced_accuracy` and `f1` as `0.5` is often not an optimal threshold.
             Predictions are calculated via the following logic on the positive class: `1 if pred > decision_threshold else 0`
 
         Returns
         -------
         Dictionary with model names as keys and model predictions as values.
         """
-        self._assert_is_fit('predict_multi')
+        self._assert_is_fit("predict_multi")
         if decision_threshold is None:
             decision_threshold = self.decision_threshold
         data = self._get_dataset(data, allow_nan=True)
-        return self._learner.predict_multi(X=data,
-                                           models=models,
-                                           as_pandas=as_pandas,
-                                           transform_features=transform_features,
-                                           inverse_transform=inverse_transform,
-                                           decision_threshold=decision_threshold)
+        return self._learner.predict_multi(
+            X=data,
+            models=models,
+            as_pandas=as_pandas,
+            transform_features=transform_features,
+            inverse_transform=inverse_transform,
+            decision_threshold=decision_threshold,
+        )
 
     def fit_summary(self, verbosity=3, show_plot=False):
         """
         Output summary of information about models produced during `fit()`.
         May create various generated summary plots and store them in folder: `predictor.path`.
 
         Parameters
@@ -1971,114 +2085,118 @@
         show_plot : bool, default = False
             If True, shows the model summary plot in browser when verbosity > 1.
 
         Returns
         -------
         Dict containing various detailed information. We do not recommend directly printing this dict as it may be very large.
         """
-        self._assert_is_fit('fit_summary')
+        self._assert_is_fit("fit_summary")
         # hpo_used = len(self._trainer.hpo_results) > 0
         hpo_used = False  # Disabled until a more memory efficient hpo_results object is implemented.
-        model_types = self._trainer.get_models_attribute_dict(attribute='type')
-        model_inner_types = self._trainer.get_models_attribute_dict(attribute='type_inner')
+        model_types = self._trainer.get_models_attribute_dict(attribute="type")
+        model_inner_types = self._trainer.get_models_attribute_dict(attribute="type_inner")
         model_typenames = {key: model_types[key].__name__ for key in model_types}
         model_innertypenames = {key: model_inner_types[key].__name__ for key in model_types if key in model_inner_types}
-        MODEL_STR = 'Model'
-        ENSEMBLE_STR = 'Ensemble'
+        MODEL_STR = "Model"
+        ENSEMBLE_STR = "Ensemble"
         for model in model_typenames:
-            if (model in model_innertypenames) and (ENSEMBLE_STR not in model_innertypenames[model]) and (
-                    ENSEMBLE_STR in model_typenames[model]):
+            if (model in model_innertypenames) and (ENSEMBLE_STR not in model_innertypenames[model]) and (ENSEMBLE_STR in model_typenames[model]):
                 new_model_typename = model_typenames[model] + "_" + model_innertypenames[model]
                 if new_model_typename.endswith(MODEL_STR):
-                    new_model_typename = new_model_typename[:-len(MODEL_STR)]
+                    new_model_typename = new_model_typename[: -len(MODEL_STR)]
                 model_typenames[model] = new_model_typename
 
         unique_model_types = set(model_typenames.values())  # no more class info
         # all fit() information that is returned:
         results = {
-            'model_types': model_typenames,  # dict with key = model-name, value = type of model (class-name)
-            'model_performance': self._trainer.get_models_attribute_dict('val_score'),
+            "model_types": model_typenames,  # dict with key = model-name, value = type of model (class-name)
+            "model_performance": self._trainer.get_models_attribute_dict("val_score"),
             # dict with key = model-name, value = validation performance
-            'model_best': self._trainer.model_best,  # the name of the best model (on validation data)
-            'model_paths': self._trainer.get_models_attribute_dict('path'),
+            "model_best": self._trainer.model_best,  # the name of the best model (on validation data)
+            "model_paths": self._trainer.get_models_attribute_dict("path"),
             # dict with key = model-name, value = path to model file
-            'model_fit_times': self._trainer.get_models_attribute_dict('fit_time'),
-            'model_pred_times': self._trainer.get_models_attribute_dict('predict_time'),
-            'num_bag_folds': self._trainer.k_fold,
-            'max_stack_level': self._trainer.get_max_level(),
+            "model_fit_times": self._trainer.get_models_attribute_dict("fit_time"),
+            "model_pred_times": self._trainer.get_models_attribute_dict("predict_time"),
+            "num_bag_folds": self._trainer.k_fold,
+            "max_stack_level": self._trainer.get_max_level(),
         }
         if self.problem_type == QUANTILE:
-            results['num_quantiles'] = len(self.quantile_levels)
+            results["num_quantiles"] = len(self.quantile_levels)
         elif self.problem_type != REGRESSION:
-            results['num_classes'] = self._trainer.num_classes
+            results["num_classes"] = self._trainer.num_classes
         # if hpo_used:
         #     results['hpo_results'] = self._trainer.hpo_results
         # get dict mapping model name to final hyperparameter values for each model:
         model_hyperparams = {}
         for model_name in self._trainer.get_model_names():
             model_obj = self._trainer.load_model(model_name)
             model_hyperparams[model_name] = model_obj.params
-        results['model_hyperparams'] = model_hyperparams
+        results["model_hyperparams"] = model_hyperparams
 
         if verbosity > 0:  # print stuff
             print("*** Summary of fit() ***")
             print("Estimated performance of each model:")
-            results['leaderboard'] = self._learner.leaderboard(silent=False)
+            results["leaderboard"] = self._learner.leaderboard(silent=False)
             # self._summarize('model_performance', 'Validation performance of individual models', results)
             #  self._summarize('model_best', 'Best model (based on validation performance)', results)
             # self._summarize('hyperparameter_tune', 'Hyperparameter-tuning used', results)
-            print("Number of models trained: %s" % len(results['model_performance']))
+            print("Number of models trained: %s" % len(results["model_performance"]))
             print("Types of models trained:")
             print(unique_model_types)
             num_fold_str = ""
-            bagging_used = results['num_bag_folds'] > 0
+            bagging_used = results["num_bag_folds"] > 0
             if bagging_used:
                 num_fold_str = f" (with {results['num_bag_folds']} folds)"
             print("Bagging used: %s %s" % (bagging_used, num_fold_str))
             num_stack_str = ""
-            stacking_used = results['max_stack_level'] > 2
+            stacking_used = results["max_stack_level"] > 2
             if stacking_used:
                 num_stack_str = f" (with {results['max_stack_level']} levels)"
             print("Multi-layer stack-ensembling used: %s %s" % (stacking_used, num_stack_str))
             hpo_str = ""
             # if hpo_used and verbosity <= 2:
             #     hpo_str = " (call fit_summary() with verbosity >= 3 to see detailed HPO info)"
             # print("Hyperparameter-tuning used: %s %s" % (hpo_used, hpo_str))
             # TODO: uncomment once feature_prune is functional:  self._summarize('feature_prune', 'feature-selection used', results)
             print("Feature Metadata (Processed):")
             print("(raw dtype, special dtypes):")
             print(self.feature_metadata)
         if verbosity > 1:  # create plots
-            plot_tabular_models(results, output_directory=self.path,
-                                save_file="SummaryOfModels.html",
-                                plot_title="Models produced during fit()",
-                                show_plot=show_plot)
+            plot_tabular_models(
+                results, output_directory=self.path, save_file="SummaryOfModels.html", plot_title="Models produced during fit()", show_plot=show_plot
+            )
             if hpo_used:
-                for model_type in results['hpo_results']:
-                    if 'trial_info' in results['hpo_results'][model_type]:
+                for model_type in results["hpo_results"]:
+                    if "trial_info" in results["hpo_results"][model_type]:
                         plot_summary_of_models(
-                            results['hpo_results'][model_type],
-                            output_directory=self.path, save_file=model_type + "_HPOmodelsummary.html",
-                            plot_title=f"Models produced during {model_type} HPO", show_plot=show_plot)
+                            results["hpo_results"][model_type],
+                            output_directory=self.path,
+                            save_file=model_type + "_HPOmodelsummary.html",
+                            plot_title=f"Models produced during {model_type} HPO",
+                            show_plot=show_plot,
+                        )
                         plot_performance_vs_trials(
-                            results['hpo_results'][model_type],
-                            output_directory=self.path, save_file=model_type + "_HPOperformanceVStrials.png",
-                            plot_title=f"HPO trials for {model_type} models", show_plot=show_plot)
+                            results["hpo_results"][model_type],
+                            output_directory=self.path,
+                            save_file=model_type + "_HPOperformanceVStrials.png",
+                            plot_title=f"HPO trials for {model_type} models",
+                            show_plot=show_plot,
+                        )
         if verbosity > 2:  # print detailed information
             if hpo_used:
-                hpo_results = results['hpo_results']
+                hpo_results = results["hpo_results"]
                 print("*** Details of Hyperparameter optimization ***")
                 for model_type in hpo_results:
                     hpo_model = hpo_results[model_type]
-                    if 'trial_info' in hpo_model:
+                    if "trial_info" in hpo_model:
                         print(
-                            f"HPO for {model_type} model:  Num. configurations tried = {len(hpo_model['trial_info'])}, Time spent = {hpo_model['total_time']}s, Search strategy = {hpo_model['search_strategy']}")
-                        print(
-                            f"Best hyperparameter-configuration (validation-performance: {self.eval_metric} = {hpo_model['validation_performance']}):")
-                        print(hpo_model['best_config'])
+                            f"HPO for {model_type} model:  Num. configurations tried = {len(hpo_model['trial_info'])}, Time spent = {hpo_model['total_time']}s, Search strategy = {hpo_model['search_strategy']}"
+                        )
+                        print(f"Best hyperparameter-configuration (validation-performance: {self.eval_metric} = {hpo_model['validation_performance']}):")
+                        print(hpo_model["best_config"])
             """
             if bagging_used:
                 pass # TODO: print detailed bagging info
             if stacking_used:
                 pass # TODO: print detailed stacking info, like how much it improves validation performance
             if results['feature_prune']:
                 pass # TODO: print detailed feature-selection info once feature-selection is functional.
@@ -2149,18 +2267,17 @@
         >>> from autogluon.tabular import TabularPredictor
         >>> predictor = TabularPredictor(label='class').fit('train.csv', label='class', auto_stack=True)  # predictor is in bagged mode.
         >>> model = 'WeightedEnsemble_L2'
         >>> train_data_transformed = predictor.transform_features(model=model)  # Internal training DataFrame used as input to `model.fit()` for each model trained in predictor.fit()`
         >>> test_data_transformed = predictor.transform_features('test.csv', model=model)  # Internal test DataFrame used as input to `model.predict_proba()` during `predictor.predict_proba(test_data, model=model)`
 
         """
-        self._assert_is_fit('transform_features')
+        self._assert_is_fit("transform_features")
         data = self._get_dataset(data, allow_nan=True)
-        return self._learner.get_inputs_to_stacker(dataset=data, model=model, base_models=base_models,
-                                                   use_orig_features=return_original_features)
+        return self._learner.get_inputs_to_stacker(dataset=data, model=model, base_models=base_models, use_orig_features=return_original_features)
 
     def transform_labels(self, labels, inverse=False, proba=False):
         """
         Transforms data labels to the internal label representation.
         This can be useful for training your own models on the same data label representation as AutoGluon.
         Regression problems do not differ between original and internal representation, and thus this method will return the provided labels.
         Warning: When `inverse=False`, it is possible for the output to contain NaN label values in multiclass problems if the provided label was dropped during training.
@@ -2184,20 +2301,30 @@
                 In this case, it is expected that `labels` be a :class:`pd.Series` or :class:`np.ndarray`.
 
         Returns
         -------
         :class:`pd.Series` of labels if `proba=False` or :class:`pd.DataFrame` of label probabilities if `proba=True`.
 
         """
-        self._assert_is_fit('transform_labels')
+        self._assert_is_fit("transform_labels")
         return self._learner.transform_labels(y=labels, inverse=inverse, proba=proba)
 
-    def feature_importance(self, data=None, model=None, features=None, feature_stage='original', subsample_size=5000,
-                           time_limit=None, num_shuffle_sets=None, include_confidence_band=True, confidence_level=0.99,
-                           silent=False):
+    def feature_importance(
+        self,
+        data=None,
+        model=None,
+        features=None,
+        feature_stage="original",
+        subsample_size=5000,
+        time_limit=None,
+        num_shuffle_sets=None,
+        include_confidence_band=True,
+        confidence_level=0.99,
+        silent=False,
+    ):
         """
         Calculates feature importance scores for the given model via permutation importance. Refer to https://explained.ai/rf-importance/ for an explanation of permutation importance.
         A feature's importance score represents the performance drop that results when the model makes predictions on a perturbed copy of the data where this feature's values have been randomly shuffled across rows.
         A feature score of 0.01 would indicate that the predictive performance dropped by 0.01 when the feature was randomly shuffled.
         The higher the score a feature has, the more important it is to the model's performance.
         If a feature has a negative score, this means that the feature is likely harmful to the final model, and a model trained with the feature removed would be expected to achieve a better predictive performance.
         Note that calculating feature importance can be a very computationally expensive process, particularly if the model uses hundreds or thousands of features. In many cases, this can take longer than the original model training.
@@ -2279,59 +2406,67 @@
                 Features with low p-value appear confidently useful to the predictor, while the other features may be useless to the predictor (or even harmful to include in its training data).
                 A p-value of 0.01 indicates that there is a 1% chance that the feature is useless or harmful, and a 99% chance that the feature is useful.
                 A p-value of 0.99 indicates that there is a 99% chance that the feature is useless or harmful, and a 1% chance that the feature is useful.
             'n': The number of shuffles performed to estimate importance score (corresponds to sample-size used to determine confidence interval for true score).
             'pXX_high': Upper end of XX% confidence interval for true feature importance score (where XX=99 by default).
             'pXX_low': Lower end of XX% confidence interval for true feature importance score.
         """
-        self._assert_is_fit('feature_importance')
+        self._assert_is_fit("feature_importance")
         data = self._get_dataset(data, allow_nan=True)
         if (data is None) and (not self._trainer.is_data_saved):
             raise AssertionError(
-                'No data was provided and there is no cached data to load for feature importance calculation. `cache_data=True` must be set in the `TabularPredictor` init `learner_kwargs` argument call to enable this functionality when data is not specified.')
+                "No data was provided and there is no cached data to load for feature importance calculation. `cache_data=True` must be set in the `TabularPredictor` init `learner_kwargs` argument call to enable this functionality when data is not specified."
+            )
         if data is not None:
-            self._validate_unique_indices(data, 'data')
+            self._validate_unique_indices(data, "data")
 
         if num_shuffle_sets is None:
             num_shuffle_sets = 10 if time_limit else 5
 
-        fi_df = self._learner.get_feature_importance(model=model, X=data, features=features,
-                                                     feature_stage=feature_stage,
-                                                     subsample_size=subsample_size, time_limit=time_limit,
-                                                     num_shuffle_sets=num_shuffle_sets, silent=silent)
+        fi_df = self._learner.get_feature_importance(
+            model=model,
+            X=data,
+            features=features,
+            feature_stage=feature_stage,
+            subsample_size=subsample_size,
+            time_limit=time_limit,
+            num_shuffle_sets=num_shuffle_sets,
+            silent=silent,
+        )
 
         if include_confidence_band:
             if confidence_level <= 0.5 or confidence_level >= 1.0:
                 raise ValueError("confidence_level must lie between 0.5 and 1.0")
             ci_str = "{:0.0f}".format(confidence_level * 100)
             import scipy.stats
+
             num_features = len(fi_df)
             ci_low_dict = dict()
             ci_high_dict = dict()
             for i in range(num_features):
                 fi = fi_df.iloc[i]
-                mean = fi['importance']
-                stddev = fi['stddev']
-                n = fi['n']
+                mean = fi["importance"]
+                stddev = fi["stddev"]
+                n = fi["n"]
                 if stddev == np.nan or n == np.nan or mean == np.nan or n == 1:
                     ci_high = np.nan
                     ci_low = np.nan
                 else:
                     t_val = scipy.stats.t.ppf(1 - (1 - confidence_level) / 2, n - 1)
                     ci_high = mean + t_val * stddev / math.sqrt(n)
                     ci_low = mean - t_val * stddev / math.sqrt(n)
                 ci_high_dict[fi.name] = ci_high
                 ci_low_dict[fi.name] = ci_low
-            high_str = 'p' + ci_str + '_high'
-            low_str = 'p' + ci_str + '_low'
+            high_str = "p" + ci_str + "_high"
+            low_str = "p" + ci_str + "_low"
             fi_df[high_str] = pd.Series(ci_high_dict)
             fi_df[low_str] = pd.Series(ci_low_dict)
         return fi_df
 
-    def compile_models(self, models='best', with_ancestors=True, compiler_configs="auto"):
+    def compile_models(self, models="best", with_ancestors=True, compiler_configs="auto"):
         """
         Compile models for accelerated prediction.
         This can be helpful to reduce prediction latency and improve throughput.
 
         Note that this is currently an experimental feature, the supported compilers can be ['native', 'onnx'].
 
         In order to compile with a specific compiler, that compiler must be installed in the Python environment.
@@ -2364,27 +2499,27 @@
                     The batch size that is optimized for model prediction.
                     By default, the batch size is None. This means the compiler would try to leverage dynamic shape for prediction.
                     Using batch_size=1 would be more suitable for online prediction, which expects a result from one data point.
                     However, it can be slow for batch processing, because of the overhead of multiple kernel execution.
                     Increasing batch size to a number that is larger than 1 would help increase the prediction throughput.
                     This comes with an expense of utilizing larger memory for prediction.
         """
-        self._assert_is_fit('compile_models')
+        self._assert_is_fit("compile_models")
         if isinstance(compiler_configs, str):
-            if compiler_configs == 'auto':
+            if compiler_configs == "auto":
                 compiler_configs = {
                     "RF": {"compiler": "onnx"},
                     "XT": {"compiler": "onnx"},
                     "NN_TORCH": {"compiler": "onnx"},
                 }
             else:
                 raise ValueError(f'Unknown compiler_configs preset: "{compiler_configs}"')
         self._trainer.compile_models(model_names=models, with_ancestors=with_ancestors, compiler_configs=compiler_configs)
 
-    def persist_models(self, models='best', with_ancestors=True, max_memory=0.4) -> list:
+    def persist_models(self, models="best", with_ancestors=True, max_memory=0.4) -> list:
         """
         Persist models in memory for reduced inference latency. This is particularly important if the models are being used for online-inference where low latency is critical.
         If models are not persisted in memory, they are loaded from disk every time they are asked to make predictions.
 
         Parameters
         ----------
         models : list of str or str, default = 'best'
@@ -2401,19 +2536,18 @@
             If the models' summed memory usage requires a larger proportion of memory than max_memory, they are not persisted. In this case, the output will be an empty list.
             If None, then models are persisted regardless of estimated memory usage. This can cause out-of-memory errors.
 
         Returns
         -------
         List of persisted model names.
         """
-        self._assert_is_fit('persist_models')
-        return self._learner.persist_trainer(low_memory=False, models=models, with_ancestors=with_ancestors,
-                                             max_memory=max_memory)
+        self._assert_is_fit("persist_models")
+        return self._learner.persist_trainer(low_memory=False, models=models, with_ancestors=with_ancestors, max_memory=max_memory)
 
-    def unpersist_models(self, models='all') -> list:
+    def unpersist_models(self, models="all") -> list:
         """
         Unpersist models in memory for reduced memory usage.
         If models are not persisted in memory, they are loaded from disk every time they are asked to make predictions.
         Note: Another way to reset the predictor and unpersist models is to reload the predictor from disk via `predictor = TabularPredictor.load(predictor.path)`.
 
         Parameters
         ----------
@@ -2422,18 +2556,18 @@
             If 'all' then all models are unpersisted.
             Valid models are listed in this `predictor` by calling `predictor.get_model_names_persisted()`.
 
         Returns
         -------
         List of unpersisted model names.
         """
-        self._assert_is_fit('unpersist_models')
+        self._assert_is_fit("unpersist_models")
         return self._learner.load_trainer().unpersist_models(model_names=models)
 
-    def refit_full(self, model='all', set_best_to_refit_full=True):
+    def refit_full(self, model="all", set_best_to_refit_full=True):
         """
         Retrain model on all of the data (training + validation).
         For bagged models:
             Optimizes a model's inference time by collapsing bagged ensembles into a single model fit on all of the training data.
             This process will typically result in a slight accuracy reduction and a large inference speedup.
             The inference speedup will generally be between 10-200x faster than the original bagged ensemble model.
                 The inference speedup factor is equivalent to (k * n), where k is the number of folds (`num_bag_folds`) and n is the number of finished repeats (`num_bag_sets`) in the bagged ensemble.
@@ -2464,47 +2598,57 @@
             This means the model used when `predictor.predict(data)` is called will be the refit_full version instead of the original version of the model.
             Ignored if `model` is not the best model.
 
         Returns
         -------
         Dictionary of original model names -> refit_full model names.
         """
-        self._assert_is_fit('refit_full')
+        self._assert_is_fit("refit_full")
         ts = time.time()
         model_best = self._get_model_best(can_infer=None)
-        logger.log(20, 'Refitting models via `predictor.refit_full` using all of the data (combined train and validation)...\n'
-                       '\tModels trained in this way will have the suffix "_FULL" and have NaN validation score.\n'
-                       '\tThis process is not bound by time_limit, but should take less time than the original `predictor.fit` call.\n'
-                       '\tTo learn more, refer to the `.refit_full` method docstring which explains how "_FULL" models differ from normal models.')
+        logger.log(
+            20,
+            "Refitting models via `predictor.refit_full` using all of the data (combined train and validation)...\n"
+            '\tModels trained in this way will have the suffix "_FULL" and have NaN validation score.\n'
+            "\tThis process is not bound by time_limit, but should take less time than the original `predictor.fit` call.\n"
+            '\tTo learn more, refer to the `.refit_full` method docstring which explains how "_FULL" models differ from normal models.',
+        )
         refit_full_dict = self._learner.refit_ensemble_full(model=model)
 
         if set_best_to_refit_full:
             model_full_dict = self._trainer.get_model_full_dict()
             if model_best in model_full_dict:
                 self._trainer.model_best = model_full_dict[model_best]
                 # Note: model_best will be overwritten if additional training is done with new models,
                 # since model_best will have validation score of None and any new model will have a better validation score.
                 # This has the side-effect of having the possibility of model_best being overwritten by a worse model than the original model_best.
                 self._trainer.save()
-                logger.log(20, f'Updated best model to "{self._trainer.model_best}" (Previously "{model_best}"). '
-                               f'AutoGluon will default to using "{self._trainer.model_best}" for predict() and predict_proba().')
+                logger.log(
+                    20,
+                    f'Updated best model to "{self._trainer.model_best}" (Previously "{model_best}"). '
+                    f'AutoGluon will default to using "{self._trainer.model_best}" for predict() and predict_proba().',
+                )
             elif model_best in model_full_dict.values():
                 # Model best is already a refit full model
                 prev_best = self._trainer.model_best
                 self._trainer.model_best = model_best
                 self._trainer.save()
-                logger.log(20, f'Updated best model to "{self._trainer.model_best}" (Previously "{prev_best}"). '
-                               f'AutoGluon will default to using "{self._trainer.model_best}" for predict() and predict_proba().')
+                logger.log(
+                    20,
+                    f'Updated best model to "{self._trainer.model_best}" (Previously "{prev_best}"). '
+                    f'AutoGluon will default to using "{self._trainer.model_best}" for predict() and predict_proba().',
+                )
             else:
                 logger.warning(
                     f'Best model ("{model_best}") is not present in refit_full dictionary. '
-                    f'Training may have failed on the refit model. AutoGluon will default to using "{model_best}" for predict() and predict_proba().')
+                    f'Training may have failed on the refit model. AutoGluon will default to using "{model_best}" for predict() and predict_proba().'
+                )
 
         te = time.time()
-        logger.log(20, f'Refit complete, total runtime = {round(te - ts, 2)}s')
+        logger.log(20, f"Refit complete, total runtime = {round(te - ts, 2)}s")
         return refit_full_dict
 
     def get_model_best(self):
         """
         Returns the string model name of the best model by validation score that can infer.
         This is the same model used during inference when `predictor.predict` is called without specifying a model.
         This can be updated to be a model other than the model with best validation score by methods such as refit_full and set_model_best.
@@ -2512,15 +2656,15 @@
         Returns
         -------
         String model name of the best model
         """
         return self._get_model_best(can_infer=True)
 
     def _get_model_best(self, can_infer=None):
-        self._assert_is_fit('get_model_best')
+        self._assert_is_fit("get_model_best")
         # TODO: Set self._trainer.model_best to the best model at end of fit instead of best WeightedEnsemble.
         if self._trainer.model_best is not None:
             models = self._trainer.get_model_names(can_infer=can_infer)
             if self._trainer.model_best in models:
                 return self._trainer.model_best
         return self._trainer.get_model_best(can_infer=can_infer)
 
@@ -2533,15 +2677,15 @@
         Parameters
         ----------
         model : str
             Name of model to set to best. If model does not exist or cannot infer, raises an AssertionError.
         save_trainer : bool, default = False
             If True, self._trainer is saved with the new model_best value, such that it is reflected when predictor is loaded in future from disk.
         """
-        self._assert_is_fit('set_model_best')
+        self._assert_is_fit("set_model_best")
         models = self._trainer.get_model_names(can_infer=True)
         if model in models:
             self._trainer.model_best = model
         else:
             raise AssertionError(f'Model "{model}" is not a valid model to specify as best! Valid models: {models}')
         if save_trainer:
             self._trainer.save()
@@ -2557,15 +2701,15 @@
         inverse : bool, default = False
             If True, instead returns a dictionary of refit full model name -> original model name (Swap keys with values)
 
         Returns
         -------
         Dictionary of original model name -> refit full model name.
         """
-        self._assert_is_fit('get_model_full_dict')
+        self._assert_is_fit("get_model_full_dict")
         return self._trainer.get_model_full_dict(inverse=inverse)
 
     def info(self):
         """
         [EXPERIMENTAL] Returns a dictionary of `predictor` metadata.
         Warning: This functionality is currently in preview mode.
             The metadata information returned may change in structure in future versions without warning.
@@ -2573,24 +2717,23 @@
             The output of this function should not be used for programmatic decisions.
         Contains information such as row count, column count, model training time, validation scores, hyperparameters, and much more.
 
         Returns
         -------
         Dictionary of `predictor` metadata.
         """
-        self._assert_is_fit('info')
+        self._assert_is_fit("info")
         return self._learner.get_info(include_model_info=True)
 
     # TODO: Add data argument
     # TODO: Add option to disable OOF generation of newly fitted models
     # TODO: Move code logic to learner/trainer
     # TODO: Add fit() arg to perform this automatically at end of training
     # TODO: Consider adding cutoff arguments such as top-k models
-    def fit_weighted_ensemble(self, base_models: list = None, name_suffix='Best', expand_pareto_frontier=False,
-                              time_limit=None, refit_full=False):
+    def fit_weighted_ensemble(self, base_models: list = None, name_suffix="Best", expand_pareto_frontier=False, time_limit=None, refit_full=False):
         """
         Fits new weighted ensemble models to combine predictions of previously-trained models.
         `cache_data` must have been set to `True` during the original training to enable this functionality.
 
         Parameters
         ----------
         base_models : list, default = None
@@ -2613,71 +2756,78 @@
             Identical to calling `predictor.refit_full(model=predictor.fit_weighted_ensemble(...))`
 
         Returns
         -------
         List of newly trained weighted ensemble model names.
         If an exception is encountered while training an ensemble model, that model's name will be absent from the list.
         """
-        self._assert_is_fit('fit_weighted_ensemble')
+        self._assert_is_fit("fit_weighted_ensemble")
         trainer = self._learner.load_trainer()
 
         if trainer.bagged_mode:
             X = trainer.load_X()
             y = trainer.load_y()
             fit = True
         else:
             X = trainer.load_X_val()
             y = trainer.load_y_val()
             fit = False
 
-        stack_name = 'aux1'
+        stack_name = "aux1"
         if base_models is None:
-            base_models = trainer.get_model_names(stack_name='core')
+            base_models = trainer.get_model_names(stack_name="core")
 
-        X_stack_preds = trainer.get_inputs_to_stacker(X=X,
-                                                      base_models=base_models,
-                                                      fit=fit,
-                                                      use_orig_features=False,
-                                                      use_val_cache=True
-                                                      )
+        X_stack_preds = trainer.get_inputs_to_stacker(X=X, base_models=base_models, fit=fit, use_orig_features=False, use_val_cache=True)
 
         models = []
 
         if expand_pareto_frontier:
             leaderboard = self.leaderboard(silent=True)
-            leaderboard = leaderboard[leaderboard['model'].isin(base_models)]
-            leaderboard = leaderboard.sort_values(by='pred_time_val')
-            models_to_check = leaderboard['model'].tolist()
+            leaderboard = leaderboard[leaderboard["model"].isin(base_models)]
+            leaderboard = leaderboard.sort_values(by="pred_time_val")
+            models_to_check = leaderboard["model"].tolist()
             for i in range(1, len(models_to_check) - 1):
-                models_to_check_now = models_to_check[:i + 1]
+                models_to_check_now = models_to_check[: i + 1]
                 max_base_model_level = max([trainer.get_model_level(base_model) for base_model in models_to_check_now])
                 weighted_ensemble_level = max_base_model_level + 1
-                models += trainer.generate_weighted_ensemble(X=X_stack_preds, y=y, level=weighted_ensemble_level,
-                                                             stack_name=stack_name,
-                                                             base_model_names=models_to_check_now,
-                                                             name_suffix=name_suffix + '_Pareto' + str(i),
-                                                             time_limit=time_limit)
+                models += trainer.generate_weighted_ensemble(
+                    X=X_stack_preds,
+                    y=y,
+                    level=weighted_ensemble_level,
+                    stack_name=stack_name,
+                    base_model_names=models_to_check_now,
+                    name_suffix=name_suffix + "_Pareto" + str(i),
+                    time_limit=time_limit,
+                )
 
         max_base_model_level = max([trainer.get_model_level(base_model) for base_model in base_models])
         weighted_ensemble_level = max_base_model_level + 1
-        models += trainer.generate_weighted_ensemble(X=X_stack_preds, y=y, level=weighted_ensemble_level,
-                                                     stack_name=stack_name, base_model_names=base_models,
-                                                     name_suffix=name_suffix, time_limit=time_limit)
+        models += trainer.generate_weighted_ensemble(
+            X=X_stack_preds,
+            y=y,
+            level=weighted_ensemble_level,
+            stack_name=stack_name,
+            base_model_names=base_models,
+            name_suffix=name_suffix,
+            time_limit=time_limit,
+        )
 
         if refit_full:
             models += self.refit_full(model=models)
 
         return models
 
-    def calibrate_decision_threshold(self,
-                                     data: str | TabularDataset | pd.DataFrame | None = None,
-                                     metric: str | Scorer | None = None,
-                                     model: str = 'best',
-                                     decision_thresholds: int | List[float] = 50,
-                                     verbose: bool = True) -> float:
+    def calibrate_decision_threshold(
+        self,
+        data: str | TabularDataset | pd.DataFrame | None = None,
+        metric: str | Scorer | None = None,
+        model: str = "best",
+        decision_thresholds: int | List[float] = 50,
+        verbose: bool = True,
+    ) -> float:
         """
         Calibrate the decision threshold in binary classification to optimize a given metric.
         You can pass the output of this method as input to `predictor.set_decision_threshold` to update the predictor.
         Will raise an AssertionError if `predictor.problem_type != 'binary'`.
 
         Note that while calibrating the decision threshold can help to improve a given metric,
         other metrics may end up having worse scores.
@@ -2719,28 +2869,24 @@
         #  make threshold calibration part of internal optimization, such as during fit_weighted_ensemble.
         #  precision has strange edge-cases where it flips from 1.0 to 0.0 score due to becoming undefined
         #    consider warning users who pass this metric,
         #    or edit this metric so they do not flip value when undefined.
         #      UndefinedMetricWarning: Precision is ill-defined and being set to 0.0 due to no predicted samples.
         #      Use `zero_division` parameter to control this behavior.
 
-        self._assert_is_fit('calibrate_decision_threshold')
+        self._assert_is_fit("calibrate_decision_threshold")
         assert self.problem_type == BINARY, f'calibrate_decision_threshold is only available for `problem_type="{BINARY}"`'
         data = self._get_dataset(data, allow_nan=True)
 
         if metric is None:
             metric = self.eval_metric
-        if model == 'best':
+        if model == "best":
             model = self.get_model_best()
 
-        return self._learner.calibrate_decision_threshold(data=data,
-                                                          metric=metric,
-                                                          model=model,
-                                                          decision_thresholds=decision_thresholds,
-                                                          verbose=verbose)
+        return self._learner.calibrate_decision_threshold(data=data, metric=metric, model=model, decision_thresholds=decision_thresholds, verbose=verbose)
 
     def get_oof_pred(self, model: str = None, transformed=False, train_data=None, internal_oof=False, decision_threshold=None, can_infer=None) -> pd.Series:
         """
         Note: This is advanced functionality not intended for normal usage.
 
         Returns the out-of-fold (OOF) predictions for every row in the training data.
 
@@ -2761,35 +2907,31 @@
         can_infer : bool, default = None
             Refer to `get_oof_pred_proba()` documentation.
 
         Returns
         -------
         :class:`pd.Series` object of the out-of-fold training predictions of the model.
         """
-        self._assert_is_fit('get_oof_pred')
+        self._assert_is_fit("get_oof_pred")
         if decision_threshold is None:
             decision_threshold = self.decision_threshold
-        y_pred_proba_oof = self.get_oof_pred_proba(model=model,
-                                                   transformed=transformed,
-                                                   as_multiclass=True,
-                                                   train_data=train_data,
-                                                   internal_oof=internal_oof,
-                                                   can_infer=can_infer)
-        y_pred_oof = get_pred_from_proba_df(y_pred_proba_oof,
-                                            problem_type=self.problem_type,
-                                            decision_threshold=decision_threshold)
+        y_pred_proba_oof = self.get_oof_pred_proba(
+            model=model, transformed=transformed, as_multiclass=True, train_data=train_data, internal_oof=internal_oof, can_infer=can_infer
+        )
+        y_pred_oof = get_pred_from_proba_df(y_pred_proba_oof, problem_type=self.problem_type, decision_threshold=decision_threshold)
         if transformed:
             return self._learner.label_cleaner.to_transformed_dtype(y_pred_oof)
         return y_pred_oof
 
     # TODO: Improve error messages when trying to get oof from refit_full and distilled models.
     # TODO: v0.1 add tutorial related to this method, as it is very powerful.
     # TODO: Remove train_data argument once we start caching the raw original data: Can just load that instead.
-    def get_oof_pred_proba(self, model: str = None, transformed=False, as_multiclass=True, train_data=None,
-                           internal_oof=False, can_infer=None) -> Union[pd.DataFrame, pd.Series]:
+    def get_oof_pred_proba(
+        self, model: str = None, transformed=False, as_multiclass=True, train_data=None, internal_oof=False, can_infer=None
+    ) -> Union[pd.DataFrame, pd.Series]:
         """
         Note: This is advanced functionality not intended for normal usage.
 
         Returns the out-of-fold (OOF) predicted class probabilities for every row in the training data.
         OOF prediction probabilities may provide unbiased estimates of generalization accuracy (reflecting how predictions will behave on new data)
         Predictions for each row are only made using models that were fit to a subset of data where this row was held-out.
 
@@ -2830,73 +2972,75 @@
             This is used to determine if the best model must be one that is able to predict on new data (True).
             If None, the best model does not need to be able to infer on new data.
 
         Returns
         -------
         :class:`pd.Series` or :class:`pd.DataFrame` object of the out-of-fold training prediction probabilities of the model.
         """
-        self._assert_is_fit('get_oof_pred_proba')
+        self._assert_is_fit("get_oof_pred_proba")
         if model is None:
             model = self._get_model_best(can_infer=can_infer)
         if not self._trainer.bagged_mode:
-            raise AssertionError('Predictor must be in bagged mode to get out-of-fold predictions.')
-        if self._trainer.get_model_attribute(model=model, attribute='refit_full', default=False):
-            model_to_get_oof = self._trainer.get_model_attribute(model=model, attribute='refit_full_parent')
+            raise AssertionError("Predictor must be in bagged mode to get out-of-fold predictions.")
+        if self._trainer.get_model_attribute(model=model, attribute="refit_full", default=False):
+            model_to_get_oof = self._trainer.get_model_attribute(model=model, attribute="refit_full_parent")
             # TODO: bagged-with-holdout refit to bagged-no-holdout should still be able to return out-of-fold predictions
         else:
             model_to_get_oof = model
         if model != model_to_get_oof:
             logger.log(20, f'Using OOF from "{model_to_get_oof}" as a proxy for "{model}".')
-        if self._trainer.get_model_attribute_full(model=model_to_get_oof, attribute='val_in_fit', func=max):
-            raise AssertionError(
-                f'Model {model_to_get_oof} does not have out-of-fold predictions because it used a validation set during training.')
+        if self._trainer.get_model_attribute_full(model=model_to_get_oof, attribute="val_in_fit", func=max):
+            raise AssertionError(f"Model {model_to_get_oof} does not have out-of-fold predictions because it used a validation set during training.")
         y_pred_proba_oof_transformed = self.transform_features(base_models=[model_to_get_oof], return_original_features=False)
         if not internal_oof:
-            is_duplicate_index = y_pred_proba_oof_transformed.index.duplicated(keep='first')
+            is_duplicate_index = y_pred_proba_oof_transformed.index.duplicated(keep="first")
             if is_duplicate_index.any():
-                logger.log(20,
-                           'Detected duplicate indices... This means that data rows may have been duplicated during training. '
-                           'Removing all duplicates except for the first instance.')
+                logger.log(
+                    20,
+                    "Detected duplicate indices... This means that data rows may have been duplicated during training. "
+                    "Removing all duplicates except for the first instance.",
+                )
                 y_pred_proba_oof_transformed = y_pred_proba_oof_transformed[is_duplicate_index == False]
             if self._learner._pre_X_rows is not None and len(y_pred_proba_oof_transformed) < self._learner._pre_X_rows:
                 len_diff = self._learner._pre_X_rows - len(y_pred_proba_oof_transformed)
                 if train_data is None:
-                    logger.warning(f'WARNING: {len_diff} rows of training data were dropped internally during fit. '
-                                   f'The output will not contain all original training rows.\n'
-                                   f'If attempting to get `oof_pred_proba`, DO NOT pass `train_data` into `predictor.predict_proba` or `predictor.transform_features`!\n'
-                                   f'Instead this can be done by the following '
-                                   f'(Ensure `train_data` is identical to when it was used in fit):\n'
-                                   f'oof_pred_proba = predictor.get_oof_pred_proba(train_data=train_data)\n'
-                                   f'oof_pred = predictor.get_oof_pred(train_data=train_data)\n')
+                    logger.warning(
+                        f"WARNING: {len_diff} rows of training data were dropped internally during fit. "
+                        f"The output will not contain all original training rows.\n"
+                        f"If attempting to get `oof_pred_proba`, DO NOT pass `train_data` into `predictor.predict_proba` or `predictor.transform_features`!\n"
+                        f"Instead this can be done by the following "
+                        f"(Ensure `train_data` is identical to when it was used in fit):\n"
+                        f"oof_pred_proba = predictor.get_oof_pred_proba(train_data=train_data)\n"
+                        f"oof_pred = predictor.get_oof_pred(train_data=train_data)\n"
+                    )
                 else:
                     missing_idx = list(train_data.index.difference(y_pred_proba_oof_transformed.index))
                     if len(missing_idx) > 0:
                         missing_idx_data = train_data.loc[missing_idx]
-                        missing_pred_proba = self.transform_features(data=missing_idx_data, base_models=[model],
-                                                                     return_original_features=False)
+                        missing_pred_proba = self.transform_features(data=missing_idx_data, base_models=[model], return_original_features=False)
                         y_pred_proba_oof_transformed = pd.concat([y_pred_proba_oof_transformed, missing_pred_proba])
                         y_pred_proba_oof_transformed = y_pred_proba_oof_transformed.reindex(list(train_data.index))
 
         if self.problem_type == MULTICLASS and self._learner.label_cleaner.problem_type_transform == MULTICLASS:
-            y_pred_proba_oof_transformed.columns = copy.deepcopy(
-                self._learner.label_cleaner.ordered_class_labels_transformed)
+            y_pred_proba_oof_transformed.columns = copy.deepcopy(self._learner.label_cleaner.ordered_class_labels_transformed)
         elif self.problem_type == QUANTILE:
             y_pred_proba_oof_transformed.columns = self.quantile_levels
         else:
             y_pred_proba_oof_transformed.columns = [self.label]
             y_pred_proba_oof_transformed = y_pred_proba_oof_transformed[self.label]
             if as_multiclass and self.problem_type == BINARY:
                 y_pred_proba_oof_transformed = LabelCleanerMulticlassToBinary.convert_binary_proba_to_multiclass_proba(
-                    y_pred_proba_oof_transformed, as_pandas=True)
+                    y_pred_proba_oof_transformed, as_pandas=True
+                )
             elif self.problem_type == MULTICLASS:
                 if transformed:
                     y_pred_proba_oof_transformed = LabelCleanerMulticlassToBinary.convert_binary_proba_to_multiclass_proba(
-                        y_pred_proba_oof_transformed, as_pandas=True)
-                    y_pred_proba_oof_transformed.columns = copy.deepcopy(
-                        self._learner.label_cleaner.ordered_class_labels_transformed)
+                        y_pred_proba_oof_transformed, as_pandas=True
+                    )
+                    y_pred_proba_oof_transformed.columns = copy.deepcopy(self._learner.label_cleaner.ordered_class_labels_transformed)
         if transformed:
             return y_pred_proba_oof_transformed
         else:
             return self.transform_labels(labels=y_pred_proba_oof_transformed, inverse=True, proba=True)
 
     @property
     def positive_class(self):
@@ -2907,15 +3051,15 @@
 
         Returns
         -------
         The positive class name in binary classification or None if the problem is not binary classification.
         """
         return self._learner.positive_class
 
-    def load_data_internal(self, data='train', return_X=True, return_y=True):
+    def load_data_internal(self, data="train", return_X=True, return_y=True):
         """
         Loads the internal data representation used during model training.
         Individual AutoGluon models like the neural network may apply additional feature transformations that are not reflected in this method.
         This method only applies universal transforms employed by all AutoGluon models.
         Warning, the internal representation may:
             Have different features compared to the original data.
             Have different row counts compared to the original data.
@@ -2944,23 +3088,23 @@
             If set to `False`, then the second element in the returned tuple will be None.
 
         Returns
         -------
         Tuple of (:class:`pd.DataFrame`, :class:`pd.Series`) corresponding to the internal data features and internal data labels, respectively.
 
         """
-        self._assert_is_fit('load_data_internal')
-        if data == 'train':
+        self._assert_is_fit("load_data_internal")
+        if data == "train":
             load_X = self._trainer.load_X
             load_y = self._trainer.load_y
-        elif data == 'val':
+        elif data == "val":
             load_X = self._trainer.load_X_val
             load_y = self._trainer.load_y_val
         else:
-            raise ValueError(f'data must be one of: [\'train\', \'val\'], but was \'{data}\'.')
+            raise ValueError(f"data must be one of: ['train', 'val'], but was '{data}'.")
         X = load_X() if return_X else None
         y = load_y() if return_y else None
         return X, y
 
     def save_space(self, remove_data=True, remove_fit_stack=True, requires_save=True, reduce_children=False):
         """
         Reduces the memory and disk size of predictor by deleting auxiliary model files that aren't needed for prediction on new data.
@@ -2988,21 +3132,25 @@
             Typically this only includes flag variables that don't have significant impact on memory or disk usage, but should technically be updated due to the removal of more important information.
                 An example is the `is_data_saved` boolean variable in `trainer`, which should be updated to `False` if `remove_data=True` was set.
         reduce_children : bool, default = False
             Whether to apply the reduction rules to bagged ensemble children models. These are the models trained for each fold of the bagged ensemble.
             This should generally be kept as `False` since the most important memory and disk reduction techniques are automatically applied to these models during the original `fit()` call.
 
         """
-        self._assert_is_fit('save_space')
-        self._trainer.reduce_memory_size(remove_data=remove_data, remove_fit_stack=remove_fit_stack, remove_fit=True,
-                                         remove_info=False, requires_save=requires_save,
-                                         reduce_children=reduce_children)
+        self._assert_is_fit("save_space")
+        self._trainer.reduce_memory_size(
+            remove_data=remove_data,
+            remove_fit_stack=remove_fit_stack,
+            remove_fit=True,
+            remove_info=False,
+            requires_save=requires_save,
+            reduce_children=reduce_children,
+        )
 
-    def delete_models(self, models_to_keep=None, models_to_delete=None, allow_delete_cascade=False,
-                      delete_from_disk=True, dry_run=True):
+    def delete_models(self, models_to_keep=None, models_to_delete=None, allow_delete_cascade=False, delete_from_disk=True, dry_run=True):
         """
         Deletes models from `predictor`.
         This can be helpful to minimize memory usage and disk usage, particularly for model deployment.
         This will remove all references to the models in `predictor`.
             For example, removed models will not appear in `predictor.leaderboard()`.
         WARNING: If `delete_from_disk=True`, this will DELETE ALL FILES in the deleted model directories, regardless if they were created by AutoGluon or not.
             DO NOT STORE FILES INSIDE OF THE MODEL DIRECTORY THAT ARE UNRELATED TO AUTOGLUON.
@@ -3029,31 +3177,32 @@
             WARNING: This deletes the entire directory for the deleted models, and ALL FILES located there.
                 It is highly recommended to first run with `dry_run=True` to understand which directories will be deleted.
         dry_run : bool, default = True
             If `True`, then deletions don't occur, and logging statements are printed describing what would have occurred.
             Set `dry_run=False` to perform the deletions.
 
         """
-        self._assert_is_fit('delete_models')
-        if models_to_keep == 'best':
+        self._assert_is_fit("delete_models")
+        if models_to_keep == "best":
             models_to_keep = self.get_model_best()
-        self._trainer.delete_models(models_to_keep=models_to_keep, models_to_delete=models_to_delete,
-                                    allow_delete_cascade=allow_delete_cascade, delete_from_disk=delete_from_disk,
-                                    dry_run=dry_run)
+        self._trainer.delete_models(
+            models_to_keep=models_to_keep,
+            models_to_delete=models_to_delete,
+            allow_delete_cascade=allow_delete_cascade,
+            delete_from_disk=delete_from_disk,
+            dry_run=dry_run,
+        )
 
     def get_size_disk(self) -> int:
         """
         Returns the combined size of all files under the `predictor.path` directory in bytes.
         """
         return get_directory_size(self.path)
 
-    def get_size_disk_per_file(self,
-                               *,
-                               sort_by: str = "size",
-                               include_path_in_name: bool = False) -> pd.Series:
+    def get_size_disk_per_file(self, *, sort_by: str = "size", include_path_in_name: bool = False) -> pd.Series:
         """
         Returns the size of each file under the `predictor.path` directory in bytes.
 
         Parameters
         ----------
         sort_by : str, default = "size"
             If None, output files will be ordered based on order of search in os.walk(path).
@@ -3067,33 +3216,41 @@
                 If True, index will be `foo/bar/model.pkl`
                 If False, index will be `bar/model.pkl`
 
         Returns
         -------
         pd.Series with index file path and value file size in bytes.
         """
-        return get_directory_size_per_file(self.path,
-                                           sort_by=sort_by,
-                                           include_path_in_name=include_path_in_name)
+        return get_directory_size_per_file(self.path, sort_by=sort_by, include_path_in_name=include_path_in_name)
 
     # TODO: v0.1 add documentation for arguments
     def get_model_names(self, stack_name=None, level=None, can_infer: bool = None, models: list = None) -> list:
         """Returns the list of model names trained in this `predictor` object."""
-        self._assert_is_fit('get_model_names')
+        self._assert_is_fit("get_model_names")
         return self._trainer.get_model_names(stack_name=stack_name, level=level, can_infer=can_infer, models=models)
 
     def get_model_names_persisted(self) -> list:
         """Returns the list of model names which are persisted in memory."""
-        self._assert_is_fit('get_model_names_persisted')
+        self._assert_is_fit("get_model_names_persisted")
         return list(self._learner.load_trainer().models.keys())
 
-    def distill(self, train_data=None, tuning_data=None, augmentation_data=None, time_limit=None, hyperparameters=None,
-                holdout_frac=None,
-                teacher_preds='soft', augment_method='spunge', augment_args={'size_factor': 5, 'max_size': int(1e5)},
-                models_name_suffix=None, verbosity=None):
+    def distill(
+        self,
+        train_data=None,
+        tuning_data=None,
+        augmentation_data=None,
+        time_limit=None,
+        hyperparameters=None,
+        holdout_frac=None,
+        teacher_preds="soft",
+        augment_method="spunge",
+        augment_args={"size_factor": 5, "max_size": int(1e5)},
+        models_name_suffix=None,
+        verbosity=None,
+    ):
         """
         Distill AutoGluon's most accurate ensemble-predictor into single models which are simpler/faster and require less memory/compute.
         Distillation can produce a model that is more accurate than the same model fit directly on the original training data.
         After calling `distill()`, there will be more models available in this Predictor, which can be evaluated using `predictor.leaderboard(test_data)` and deployed with: `predictor.predict(test_data, model=MODEL_NAME)`.
         This will raise an exception if `cache_data=False` was previously set in `fit()`.
 
         NOTE: Until catboost v0.24 is released, `distill()` with CatBoost students in multiclass classification requires you to first install catboost-dev: `pip install catboost-dev`
@@ -3160,35 +3317,38 @@
         >>> distilled_model_names = predictor.distill()
         >>> test_data = TabularDataset('test.csv')
         >>> ldr = predictor.leaderboard(test_data)
         >>> model_to_deploy = distilled_model_names[0]
         >>> predictor.predict(test_data, model=model_to_deploy)
 
         """
-        self._assert_is_fit('distill')
+        self._assert_is_fit("distill")
         if isinstance(hyperparameters, str):
             hyperparameters = get_hyperparameter_config(hyperparameters)
-        return self._learner.distill(X=train_data, X_val=tuning_data, time_limit=time_limit,
-                                     hyperparameters=hyperparameters, holdout_frac=holdout_frac,
-                                     verbosity=verbosity, models_name_suffix=models_name_suffix,
-                                     teacher_preds=teacher_preds,
-                                     augmentation_data=augmentation_data, augment_method=augment_method,
-                                     augment_args=augment_args)
+        return self._learner.distill(
+            X=train_data,
+            X_val=tuning_data,
+            time_limit=time_limit,
+            hyperparameters=hyperparameters,
+            holdout_frac=holdout_frac,
+            verbosity=verbosity,
+            models_name_suffix=models_name_suffix,
+            teacher_preds=teacher_preds,
+            augmentation_data=augmentation_data,
+            augment_method=augment_method,
+            augment_args=augment_args,
+        )
 
     # TODO: v1.0 Move core logic to `trainer` level.
     # TODO: v1.0 Make it use leaderboard directly, allow to specify columns to include in the plot.
     # TODO: See if we can incorporate into tutorials (without causing crashes for users who try them)
     #  Might require using a different tool than pygraphviz to avoid the apt-get commands
     # TODO: v1.0 Rename to `plot_model_graph`
     # TODO: v1.0 Maybe add ensemble weights to the edges.
-    def plot_ensemble_model(self,
-                            model: str = 'best',
-                            *,
-                            prune_unused_nodes: bool = True,
-                            filename: str = 'ensemble_model.png') -> str:
+    def plot_ensemble_model(self, model: str = "best", *, prune_unused_nodes: bool = True, filename: str = "ensemble_model.png") -> str:
         """
         Output the visualized stack ensemble architecture of a model trained by `fit()`.
         The plot is stored to a file, `ensemble_model.png` in folder `predictor.path` (or by the name specified in `filename`)
 
         This function requires `graphviz` and `pygraphviz` to be installed because this visualization depends on those package.
         Unless this function will raise `ImportError` without being able to generate the visual of the ensemble model.
 
@@ -3222,83 +3382,82 @@
         >>> path_to_png = predictor.plot_ensemble_model()
         >>>
         >>> # To view the plot inside a Jupyter Notebook, use the below code:
         >>> from IPython.display import Image, display
         >>> display(Image(filename=path_to_png))
 
         """
-        self._assert_is_fit('plot_ensemble_model')
+        self._assert_is_fit("plot_ensemble_model")
         try:
             import pygraphviz
         except:
-            raise ImportError('Visualizing ensemble network architecture requires the `pygraphviz` library. '
-                              'Try `sudo apt-get install graphviz graphviz-dev` followed by `pip install pygraphviz` to install on Linux, '
-                              'or refer to the method docstring for detailed installation instructions for other operating systems.')
+            raise ImportError(
+                "Visualizing ensemble network architecture requires the `pygraphviz` library. "
+                "Try `sudo apt-get install graphviz graphviz-dev` followed by `pip install pygraphviz` to install on Linux, "
+                "or refer to the method docstring for detailed installation instructions for other operating systems."
+            )
 
         G = self._trainer.model_graph.copy()
 
         primary_model = model
-        if primary_model == 'best':
+        if primary_model == "best":
             primary_model = self.get_model_best()
         all_models = self.get_model_names()
         assert primary_model in all_models, f'Unknown model "{primary_model}"! Valid models: {all_models}'
         if prune_unused_nodes == True:
             models_to_keep = self._trainer.get_minimum_model_set(model=primary_model)
             G = nx.subgraph(G, models_to_keep)
 
         models = list(G.nodes)
-        fit_times = self._trainer.get_models_attribute_full(models=models, attribute='fit_time')
-        predict_times = self._trainer.get_models_attribute_full(models=models, attribute='predict_time')
+        fit_times = self._trainer.get_models_attribute_full(models=models, attribute="fit_time")
+        predict_times = self._trainer.get_models_attribute_full(models=models, attribute="predict_time")
 
         A = nx.nx_agraph.to_agraph(G)
 
         for node in A.iternodes():
             node_name = node.name
             fit_time = fit_times[node_name]
             predict_time = predict_times[node_name]
             if fit_time is None:
-                fit_time_str = 'NaN'
+                fit_time_str = "NaN"
             else:
                 fit_time_str = f"{fit_time:.1f}s"
             if predict_time is None:
-                predict_time_str = 'NaN'
+                predict_time_str = "NaN"
             else:
                 predict_time_str = f"{predict_time:.2f}s"
 
-            node_val_score = node.attr['val_score']
-            if node_val_score is None or (isinstance(node_val_score, str) and node_val_score == 'None'):
-                node_val_score_str = 'NaN'
+            node_val_score = node.attr["val_score"]
+            if node_val_score is None or (isinstance(node_val_score, str) and node_val_score == "None"):
+                node_val_score_str = "NaN"
             else:
                 node_val_score_str = f"{float(node.attr['val_score']):.4f}"
-            label = f"{node.name}" \
-                    f"\nscore_val: {node_val_score_str}" \
-                    f"\nfit_time: {fit_time_str}" \
-                    f"\npred_time_val: {predict_time_str}"
+            label = f"{node.name}" f"\nscore_val: {node_val_score_str}" f"\nfit_time: {fit_time_str}" f"\npred_time_val: {predict_time_str}"
             # Remove unnecessary attributes
             node.attr.clear()
-            node.attr['label'] = label
+            node.attr["label"] = label
 
-        A.graph_attr.update(rankdir='BT')
+        A.graph_attr.update(rankdir="BT")
         A.node_attr.update(fontsize=10)
-        A.node_attr.update(shape='rectangle')
+        A.node_attr.update(shape="rectangle")
 
         for node in A.iternodes():
             if node.name == primary_model:
                 # Golden Orange
-                node.attr['style'] = 'filled'
-                node.attr['fillcolor'] = '#ff9900'
-                node.attr['shape'] = 'box3d'
+                node.attr["style"] = "filled"
+                node.attr["fillcolor"] = "#ff9900"
+                node.attr["shape"] = "box3d"
             elif nx.has_path(G, node.name, primary_model):
                 # Yellow
-                node.attr['style'] = 'filled'
-                node.attr['fillcolor'] = '#ffcc00'
+                node.attr["style"] = "filled"
+                node.attr["fillcolor"] = "#ffcc00"
             # Else: White
 
         model_image_fname = os.path.join(self.path, filename)
-        A.draw(model_image_fname, format='png', prog='dot')
+        A.draw(model_image_fname, format="png", prog="dot")
         return model_image_fname
 
     @staticmethod
     def _summarize(key, msg, results):
         if key in results:
             print(msg + ": " + str(results[key]))
 
@@ -3312,57 +3471,56 @@
         elif isinstance(data, TabularDataset):
             return data
         elif isinstance(data, pd.DataFrame):
             return TabularDataset(data)
         elif isinstance(data, str):
             return TabularDataset(data)
         elif isinstance(data, pd.Series):
-            raise TypeError("data must be TabularDataset or pandas.DataFrame, not pandas.Series. \
-                   To predict on just single example (ith row of table), use data.iloc[[i]] rather than data.iloc[i]")
+            raise TypeError(
+                "data must be TabularDataset or pandas.DataFrame, not pandas.Series. \
+                   To predict on just single example (ith row of table), use data.iloc[[i]] rather than data.iloc[i]"
+            )
         else:
             raise TypeError("data must be TabularDataset or pandas.DataFrame or str file path to data")
 
     def _validate_hyperparameter_tune_kwargs(self, hyperparameter_tune_kwargs, time_limit=None):
         """
         Returns True if hyperparameter_tune_kwargs is None or can construct a valid scheduler.
         Returns False if hyperparameter_tune_kwargs results in an invalid scheduler.
         """
         if hyperparameter_tune_kwargs is None:
             return True
 
-        scheduler_cls, scheduler_params = scheduler_factory(hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
-                                                            time_out=time_limit,
-                                                            nthreads_per_trial='auto', ngpus_per_trial='auto')
+        scheduler_cls, scheduler_params = scheduler_factory(
+            hyperparameter_tune_kwargs=hyperparameter_tune_kwargs, time_out=time_limit, nthreads_per_trial="auto", ngpus_per_trial="auto"
+        )
 
-        if scheduler_params.get('dist_ip_addrs', None):
-            logger.warning(
-                'Warning: dist_ip_addrs does not currently work for Tabular. Distributed instances will not be utilized.')
+        if scheduler_params.get("dist_ip_addrs", None):
+            logger.warning("Warning: dist_ip_addrs does not currently work for Tabular. Distributed instances will not be utilized.")
 
-        if scheduler_params['num_trials'] == 1:
+        if scheduler_params["num_trials"] == 1:
             logger.warning(
-                'Warning: Specified num_trials == 1 for hyperparameter tuning, disabling HPO. This can occur if time_limit was not specified in `fit()`.')
+                "Warning: Specified num_trials == 1 for hyperparameter tuning, disabling HPO. This can occur if time_limit was not specified in `fit()`."
+            )
             return False
 
-        scheduler_ngpus = scheduler_params['resource'].get('num_gpus', 0)
+        scheduler_ngpus = scheduler_params["resource"].get("num_gpus", 0)
         if scheduler_ngpus is not None and isinstance(scheduler_ngpus, int) and scheduler_ngpus > 1:
-            logger.warning(
-                f"Warning: TabularPredictor currently doesn't use >1 GPU per training run. Detected {scheduler_ngpus} GPUs.")
+            logger.warning(f"Warning: TabularPredictor currently doesn't use >1 GPU per training run. Detected {scheduler_ngpus} GPUs.")
 
         return True
 
     def _set_hyperparameter_tune_kwargs_in_ag_args(self, hyperparameter_tune_kwargs, ag_args, time_limit):
-        if hyperparameter_tune_kwargs is not None and 'hyperparameter_tune_kwargs' not in ag_args:
-            if 'hyperparameter_tune_kwargs' in ag_args:
-                AssertionError(
-                    'hyperparameter_tune_kwargs was specified in both ag_args and in kwargs. Please only specify once.')
-            else:
-                ag_args['hyperparameter_tune_kwargs'] = hyperparameter_tune_kwargs
-        if ag_args.get('hyperparameter_tune_kwargs', None) is not None:
-            logger.log(30,
-                       'Warning: hyperparameter tuning is currently experimental and may cause the process to hang.')
+        if hyperparameter_tune_kwargs is not None and "hyperparameter_tune_kwargs" not in ag_args:
+            if "hyperparameter_tune_kwargs" in ag_args:
+                AssertionError("hyperparameter_tune_kwargs was specified in both ag_args and in kwargs. Please only specify once.")
+            else:
+                ag_args["hyperparameter_tune_kwargs"] = hyperparameter_tune_kwargs
+        if ag_args.get("hyperparameter_tune_kwargs", None) is not None:
+            logger.log(30, "Warning: hyperparameter tuning is currently experimental and may cause the process to hang.")
         return ag_args
 
     def _set_post_fit_vars(self, learner: AbstractTabularLearner = None):
         if learner is not None:
             self._learner: AbstractTabularLearner = learner
         self._learner_type = type(self._learner)
         if self._learner.trainer_path is not None:
@@ -3378,30 +3536,31 @@
     @classmethod
     def _load_metadata_file(cls, path: str, silent=True):
         metadata_file_path = path + cls._predictor_metadata_file_name
         return load_json.load(path=metadata_file_path, verbose=not silent)
 
     def _save_version_file(self, silent=False):
         from ..version import __version__
-        version_file_contents = f'{__version__}'
+
+        version_file_contents = f"{__version__}"
         version_file_path = self.path + self._predictor_version_file_name
         save_str.save(path=version_file_path, data=version_file_contents, verbose=not silent)
 
     def _save_metadata_file(self, silent=False):
         """
         Save metadata json file to disk containing information such as
         python version, autogluon version, installed packages, operating system, etc.
         """
         metadata_file_path = self.path + self._predictor_metadata_file_name
 
         metadata = get_autogluon_metadata()
 
         save_json.save(path=metadata_file_path, obj=metadata)
         if not silent:
-            logger.log(15, f'Saving {metadata_file_path}')
+            logger.log(15, f"Saving {metadata_file_path}")
 
     def save(self, silent=False):
         """
         Save this Predictor to file in directory specified by this Predictor's `path`.
         Note that :meth:`TabularPredictor.fit` already saves the predictor object automatically
         (we do not recommend modifying the Predictor object yourself as it tracks many trained models).
 
@@ -3419,15 +3578,15 @@
         save_pkl.save(path=path + self.predictor_file_name, object=self)
         self._learner = tmp_learner
         self._trainer = tmp_trainer
         self._save_version_file(silent=silent)
         try:
             self._save_metadata_file(silent=silent)
         except Exception as e:
-            logger.log(30, f'Failed to save metadata file due to exception {e}, skipping...')
+            logger.log(30, f"Failed to save metadata file due to exception {e}, skipping...")
         if not silent:
             logger.log(20, f'TabularPredictor saved. To load, use: predictor = TabularPredictor.load("{self.path}")')
 
     @classmethod
     def _load(cls, path: str):
         """
         Inner load method, called in `load`.
@@ -3466,65 +3625,71 @@
         if verbosity is not None:
             set_logger_verbosity(verbosity)  # Reset logging after load (may be in new Python session)
         if path is None:
             raise ValueError("path cannot be None in load()")
 
         try:
             from ..version import __version__
+
             version_current = __version__
         except:
             version_current = None
 
         path = setup_outputdir(path, warn_if_exist=False)  # replace ~ with absolute path if it exists
         try:
             version_saved = cls._load_version_file(path=path)
         except:
-            logger.warning(f'WARNING: Could not find version file at "{path + cls._predictor_version_file_name}".\n'
-                           f'This means that the predictor was fit in a version `<=0.3.1`.')
+            logger.warning(
+                f'WARNING: Could not find version file at "{path + cls._predictor_version_file_name}".\n'
+                f"This means that the predictor was fit in a version `<=0.3.1`."
+            )
             version_saved = None
 
         if version_saved is None:
             predictor = cls._load(path=path)
             try:
                 version_saved = predictor._learner.version
             except:
                 version_saved = None
         else:
             predictor = None
         if version_saved is None:
-            version_saved = 'Unknown (Likely <=0.0.11)'
+            version_saved = "Unknown (Likely <=0.0.11)"
 
         check_saved_predictor_version(
             version_current=version_current,
             version_saved=version_saved,
             require_version_match=require_version_match,
             logger=logger,
         )
 
         try:
             metadata_init = cls._load_metadata_file(path=path)
         except:
-            logger.warning(f'WARNING: Could not find metadata file at "{path + cls._predictor_metadata_file_name}".\n'
-                           f'This could mean that the predictor was fit in a version `<=0.5.2`.')
+            logger.warning(
+                f'WARNING: Could not find metadata file at "{path + cls._predictor_metadata_file_name}".\n'
+                f"This could mean that the predictor was fit in a version `<=0.5.2`."
+            )
             metadata_init = None
 
         metadata_load = get_autogluon_metadata()
 
         if metadata_init is not None:
             try:
                 compare_autogluon_metadata(original=metadata_init, current=metadata_load, check_packages=check_packages)
             except:
-                logger.log(30, 'WARNING: Exception raised while comparing metadata files, skipping comparison...')
+                logger.log(30, "WARNING: Exception raised while comparing metadata files, skipping comparison...")
             if require_py_version_match:
-                if metadata_init['py_version'] != metadata_load['py_version']:
+                if metadata_init["py_version"] != metadata_load["py_version"]:
                     raise AssertionError(
                         f'Predictor was created on Python version {metadata_init["py_version"]} '
                         f'but is being loaded with Python version {metadata_load["py_version"]}. '
-                        f'Please ensure the versions match to avoid instability. While it is NOT recommended, '
-                        f'this error can be bypassed by specifying `require_py_version_match=False`.')
+                        f"Please ensure the versions match to avoid instability. While it is NOT recommended, "
+                        f"this error can be bypassed by specifying `require_py_version_match=False`."
+                    )
 
         if predictor is None:
             predictor = cls._load(path=path)
 
         return predictor
 
     @classmethod
@@ -3564,24 +3729,24 @@
             log_file_path = os.path.abspath(os.path.normpath(log_file_path))
             os.makedirs(os.path.dirname(log_file_path), exist_ok=True)
             add_log_to_file(log_file_path)
 
     @staticmethod
     def _validate_init_kwargs(kwargs):
         valid_kwargs = {
-            'learner_type',
-            'learner_kwargs',
-            'quantile_levels',
+            "learner_type",
+            "learner_kwargs",
+            "quantile_levels",
         }
         invalid_keys = []
         for key in kwargs:
             if key not in valid_kwargs:
                 invalid_keys.append(key)
         if invalid_keys:
-            raise ValueError(f'Invalid kwargs passed: {invalid_keys}\nValid kwargs: {list(valid_kwargs)}')
+            raise ValueError(f"Invalid kwargs passed: {invalid_keys}\nValid kwargs: {list(valid_kwargs)}")
 
     def _validate_fit_kwargs(self, kwargs):
         # TODO:
         #  Valid core_kwargs values:
         #  ag_args, ag_args_fit, ag_args_ensemble, stack_name, ensemble_type, name_suffix, time_limit
         #  Valid aux_kwargs values:
         #  name_suffix, time_limit, stack_name, aux_hyperparameters, ag_args, ag_args_ensemble, fit_weighted_ensemble
@@ -3591,17 +3756,16 @@
         fit_kwargs_default = dict(
             # data split / ensemble architecture kwargs -> Don't nest but have nested documentation -> Actually do nesting
             holdout_frac=None,  # TODO: Potentially error if num_bag_folds is also specified
             num_bag_folds=None,
             # TODO: Potentially move to fit_extra, raise exception if value too large / invalid in fit_extra.
             auto_stack=False,
             use_bag_holdout=False,
-
             # other
-            feature_generator='auto',
+            feature_generator="auto",
             unlabeled_data=None,
             _feature_generator_kwargs=None,
         )
 
         kwargs = self._validate_fit_extra_kwargs(kwargs, extra_valid_keys=list(fit_kwargs_default.keys()))
 
         kwargs_sanitized = fit_kwargs_default.copy()
@@ -3619,78 +3783,68 @@
                          but not used in validation
             name_suffix: A suffix string to be added to the individual model names
         """
         return dict(
             # data split / ensemble architecture kwargs -> Don't nest but have nested documentation -> Actually do nesting
             num_bag_sets=None,
             num_stack_levels=None,
-
             hyperparameter_tune_kwargs=None,
-
             # core_kwargs -> +1 nest
             ag_args=None,
             ag_args_fit=None,
             ag_args_ensemble=None,
             included_model_types=None,
             excluded_model_types=None,
-
             # aux_kwargs -> +1 nest
-
             # post_fit_kwargs -> +1 nest
             set_best_to_refit_full=False,
             keep_only_best=False,
             save_space=False,
             refit_full=False,
-
             # other
             verbosity=self.verbosity,
             feature_prune_kwargs=None,
-
             # private
             _save_bag_folds=None,
-
-            calibrate='auto',
-
+            calibrate="auto",
             # pseudo label
             pseudo_data=None,
-
-            name_suffix=None
+            name_suffix=None,
         )
 
     def _validate_fit_extra_kwargs(self, kwargs, extra_valid_keys=None):
         fit_extra_kwargs_default = self._fit_extra_kwargs_dict()
 
         allowed_kwarg_names = list(fit_extra_kwargs_default.keys())
         if extra_valid_keys is not None:
             allowed_kwarg_names += extra_valid_keys
         for kwarg_name in kwargs.keys():
             if kwarg_name not in allowed_kwarg_names:
-                public_kwarg_options = [kwarg for kwarg in allowed_kwarg_names if kwarg[0] != '_']
+                public_kwarg_options = [kwarg for kwarg in allowed_kwarg_names if kwarg[0] != "_"]
                 public_kwarg_options.sort()
-                raise ValueError(
-                    f"Unknown `.fit` keyword argument specified: '{kwarg_name}'\nValid kwargs: {public_kwarg_options}")
+                raise ValueError(f"Unknown `.fit` keyword argument specified: '{kwarg_name}'\nValid kwargs: {public_kwarg_options}")
 
         kwargs_sanitized = fit_extra_kwargs_default.copy()
         kwargs_sanitized.update(kwargs)
 
         # Deepcopy args to avoid altering outer context
-        deepcopy_args = ['ag_args', 'ag_args_fit', 'ag_args_ensemble', 'included_model_types', 'excluded_model_types']
+        deepcopy_args = ["ag_args", "ag_args_fit", "ag_args_ensemble", "included_model_types", "excluded_model_types"]
         for deepcopy_arg in deepcopy_args:
             kwargs_sanitized[deepcopy_arg] = copy.deepcopy(kwargs_sanitized[deepcopy_arg])
 
-        refit_full = kwargs_sanitized['refit_full']
-        set_best_to_refit_full = kwargs_sanitized['set_best_to_refit_full']
+        refit_full = kwargs_sanitized["refit_full"]
+        set_best_to_refit_full = kwargs_sanitized["set_best_to_refit_full"]
         if refit_full and not self._learner.cache_data:
-            raise ValueError(
-                '`refit_full=True` is only available when `cache_data=True`. Set `cache_data=True` to utilize `refit_full`.')
+            raise ValueError("`refit_full=True` is only available when `cache_data=True`. Set `cache_data=True` to utilize `refit_full`.")
         if set_best_to_refit_full and not refit_full:
             raise ValueError(
-                '`set_best_to_refit_full=True` is only available when `refit_full=True`. Set `refit_full=True` to utilize `set_best_to_refit_full`.')
-        valid_calibrate_options = [True, False, 'auto']
-        calibrate = kwargs_sanitized['calibrate']
+                "`set_best_to_refit_full=True` is only available when `refit_full=True`. Set `refit_full=True` to utilize `set_best_to_refit_full`."
+            )
+        valid_calibrate_options = [True, False, "auto"]
+        calibrate = kwargs_sanitized["calibrate"]
         if calibrate not in valid_calibrate_options:
             raise ValueError(f"`calibrate` must be a value in {valid_calibrate_options}, but is: {calibrate}")
 
         return kwargs_sanitized
 
     def _prune_data_features(self, train_features: pd.DataFrame, other_features: pd.DataFrame, is_labeled: bool):
         """
@@ -3721,100 +3875,98 @@
             train_data = TabularDataset(train_data)
         if tuning_data is not None and isinstance(tuning_data, str):
             tuning_data = TabularDataset(tuning_data)
         if unlabeled_data is not None and isinstance(unlabeled_data, str):
             unlabeled_data = TabularDataset(unlabeled_data)
 
         if not isinstance(train_data, pd.DataFrame):
-            raise AssertionError(
-                f'train_data is required to be a pandas DataFrame, but was instead: {type(train_data)}')
+            raise AssertionError(f"train_data is required to be a pandas DataFrame, but was instead: {type(train_data)}")
 
         if len(set(train_data.columns)) < len(train_data.columns):
             raise ValueError(
-                "Column names are not unique, please change duplicated column names (in pandas: train_data.rename(columns={'current_name':'new_name'})")
+                "Column names are not unique, please change duplicated column names (in pandas: train_data.rename(columns={'current_name':'new_name'})"
+            )
         if tuning_data is not None:
             if not isinstance(tuning_data, pd.DataFrame):
-                raise AssertionError(
-                    f'tuning_data is required to be a pandas DataFrame, but was instead: {type(tuning_data)}')
-            self._validate_unique_indices(data=tuning_data, name='tuning_data')
+                raise AssertionError(f"tuning_data is required to be a pandas DataFrame, but was instead: {type(tuning_data)}")
+            self._validate_unique_indices(data=tuning_data, name="tuning_data")
             train_features = [column for column in train_data.columns if column != self.label]
             tuning_features = [column for column in tuning_data.columns if column != self.label]
-            train_features, tuning_features = self._prune_data_features(train_features=train_features,
-                                                                        other_features=tuning_features,
-                                                                        is_labeled=True)
+            train_features, tuning_features = self._prune_data_features(train_features=train_features, other_features=tuning_features, is_labeled=True)
             train_features = np.array(train_features)
             tuning_features = np.array(tuning_features)
             if np.any(train_features != tuning_features):
                 raise ValueError("Column names must match between training and tuning data")
 
             if self.label in tuning_data:
                 train_label_type = train_data[self.label].dtype
                 tuning_label_type = tuning_data[self.label].dtype
 
                 if train_label_type != tuning_label_type:
-                    logger.warning(f'WARNING: train_data and tuning_data have mismatched label column dtypes! '
-                                   f'train_label_type={train_label_type}, tuning_data_type={tuning_label_type}.\n'
-                                   f'\tYou should ensure the dtypes match to avoid bugs or instability.\n'
-                                   f'\tAutoGluon will attempt to convert the dtypes to align.')
+                    logger.warning(
+                        f"WARNING: train_data and tuning_data have mismatched label column dtypes! "
+                        f"train_label_type={train_label_type}, tuning_data_type={tuning_label_type}.\n"
+                        f"\tYou should ensure the dtypes match to avoid bugs or instability.\n"
+                        f"\tAutoGluon will attempt to convert the dtypes to align."
+                    )
 
         if unlabeled_data is not None:
             if not isinstance(unlabeled_data, pd.DataFrame):
-                raise AssertionError(
-                    f'unlabeled_data is required to be a pandas DataFrame, but was instead: {type(unlabeled_data)}')
-            self._validate_unique_indices(data=unlabeled_data, name='unlabeled_data')
+                raise AssertionError(f"unlabeled_data is required to be a pandas DataFrame, but was instead: {type(unlabeled_data)}")
+            self._validate_unique_indices(data=unlabeled_data, name="unlabeled_data")
             train_features = [column for column in train_data.columns if column != self.label]
             unlabeled_features = [column for column in unlabeled_data.columns]
-            train_features, unlabeled_features = self._prune_data_features(train_features=train_features,
-                                                                           other_features=unlabeled_features,
-                                                                           is_labeled=False)
+            train_features, unlabeled_features = self._prune_data_features(train_features=train_features, other_features=unlabeled_features, is_labeled=False)
             train_features = sorted(np.array(train_features))
             unlabeled_features = sorted(np.array(unlabeled_features))
             if np.any(train_features != unlabeled_features):
-                raise ValueError("Column names must match between training and unlabeled data.\n"
-                                 "Unlabeled data must have not the label column specified in it.\n")
+                raise ValueError(
+                    "Column names must match between training and unlabeled data.\n" "Unlabeled data must have not the label column specified in it.\n"
+                )
         return train_data, tuning_data, unlabeled_data
 
     @staticmethod
     def _validate_unique_indices(data, name: str):
         is_duplicate_index = data.index.duplicated(keep=False)
         if is_duplicate_index.any():
             duplicate_count = is_duplicate_index.sum()
-            raise AssertionError(f'{name} contains {duplicate_count} duplicated indices. '
-                                 'Please ensure DataFrame indices are unique.\n'
-                                 f'\tYou can identify the indices which are duplicated via `{name}.index.duplicated(keep=False)`')
+            raise AssertionError(
+                f"{name} contains {duplicate_count} duplicated indices. "
+                "Please ensure DataFrame indices are unique.\n"
+                f"\tYou can identify the indices which are duplicated via `{name}.index.duplicated(keep=False)`"
+            )
 
     @staticmethod
     def _validate_infer_limit(infer_limit: float, infer_limit_batch_size: int) -> Tuple[float, int]:
         if infer_limit_batch_size is not None:
             if not isinstance(infer_limit_batch_size, int):
-                raise ValueError(f'infer_limit_batch_size must be type int, but was instead type {type(infer_limit_batch_size)}')
+                raise ValueError(f"infer_limit_batch_size must be type int, but was instead type {type(infer_limit_batch_size)}")
             elif infer_limit_batch_size < 1:
-                raise AssertionError(f'infer_limit_batch_size must be >=1, value: {infer_limit_batch_size}')
+                raise AssertionError(f"infer_limit_batch_size must be >=1, value: {infer_limit_batch_size}")
         if infer_limit is not None:
             if not isinstance(infer_limit, (int, float)):
-                raise ValueError(f'infer_limit must be type int or float, but was instead type {type(infer_limit)}')
+                raise ValueError(f"infer_limit must be type int or float, but was instead type {type(infer_limit)}")
             if infer_limit <= 0:
-                raise AssertionError(f'infer_limit must be greater than zero! (infer_limit={infer_limit})')
+                raise AssertionError(f"infer_limit must be greater than zero! (infer_limit={infer_limit})")
         if infer_limit is not None and infer_limit_batch_size is None:
             infer_limit_batch_size = 10000
-            logger.log(20, f'infer_limit specified, but infer_limit_batch_size was not specified. Setting infer_limit_batch_size={infer_limit_batch_size}')
+            logger.log(20, f"infer_limit specified, but infer_limit_batch_size was not specified. Setting infer_limit_batch_size={infer_limit_batch_size}")
         return infer_limit, infer_limit_batch_size
 
-    def _set_feature_generator(self, feature_generator='auto', feature_metadata=None, init_kwargs=None):
+    def _set_feature_generator(self, feature_generator="auto", feature_metadata=None, init_kwargs=None):
         if self._learner.feature_generator is not None:
-            if isinstance(feature_generator, str) and feature_generator == 'auto':
+            if isinstance(feature_generator, str) and feature_generator == "auto":
                 feature_generator = self._learner.feature_generator
             else:
-                raise AssertionError('FeatureGenerator already exists!')
-        self._learner.feature_generator = get_default_feature_generator(feature_generator=feature_generator,
-                                                                        feature_metadata=feature_metadata,
-                                                                        init_kwargs=init_kwargs)
+                raise AssertionError("FeatureGenerator already exists!")
+        self._learner.feature_generator = get_default_feature_generator(
+            feature_generator=feature_generator, feature_metadata=feature_metadata, init_kwargs=init_kwargs
+        )
 
-    def _sanitize_stack_args(self, num_bag_folds, num_bag_sets, num_stack_levels, time_limit, auto_stack,
-                             num_train_rows, problem_type):
+    def _sanitize_stack_args(self, num_bag_folds, num_bag_sets, num_stack_levels, time_limit, auto_stack, num_train_rows, problem_type):
         if auto_stack:
             # TODO: What about datasets that are 100k+? At a certain point should we not bag?
             # TODO: What about time_limit? Metalearning can tell us expected runtime of each model, then we can select optimal folds + stack levels to fit time constraint
             if num_bag_folds is None:
                 num_bag_folds = min(8, max(5, math.floor(num_train_rows / 100)))
             # TODO: Leverage use_bag_holdout when data is large to enable multi-layer stacking
             #  if num_train_rows >= 100000 and num_val_rows is None and use_bag_holdout is None:
@@ -3829,42 +3981,37 @@
                 else:
                     num_stack_levels = min(1, max(0, math.floor(num_train_rows / 750)))
         if num_bag_folds is None:
             num_bag_folds = 0
         if num_stack_levels is None:
             num_stack_levels = 0
         if not isinstance(num_bag_folds, int):
-            raise ValueError(f'num_bag_folds must be an integer. (num_bag_folds={num_bag_folds})')
+            raise ValueError(f"num_bag_folds must be an integer. (num_bag_folds={num_bag_folds})")
         if not isinstance(num_stack_levels, int):
-            raise ValueError(f'num_stack_levels must be an integer. (num_stack_levels={num_stack_levels})')
+            raise ValueError(f"num_stack_levels must be an integer. (num_stack_levels={num_stack_levels})")
         if num_bag_folds < 2 and num_bag_folds != 0:
-            raise ValueError(f'num_bag_folds must be equal to 0 or >=2. (num_bag_folds={num_bag_folds})')
+            raise ValueError(f"num_bag_folds must be equal to 0 or >=2. (num_bag_folds={num_bag_folds})")
         if num_stack_levels != 0 and num_bag_folds == 0:
-            raise ValueError(
-                f'num_stack_levels must be 0 if num_bag_folds is 0. (num_stack_levels={num_stack_levels}, num_bag_folds={num_bag_folds})')
+            raise ValueError(f"num_stack_levels must be 0 if num_bag_folds is 0. (num_stack_levels={num_stack_levels}, num_bag_folds={num_bag_folds})")
         if num_bag_sets is None:
             if num_bag_folds >= 2:
                 if time_limit is not None:
                     num_bag_sets = 20  # TODO: v0.1 Reduce to 5 or 3 as 20 is unnecessarily extreme as a default.
                 else:
                     num_bag_sets = 1
             else:
                 num_bag_sets = 1
         if not isinstance(num_bag_sets, int):
-            raise ValueError(f'num_bag_sets must be an integer. (num_bag_sets={num_bag_sets})')
+            raise ValueError(f"num_bag_sets must be an integer. (num_bag_sets={num_bag_sets})")
         return num_bag_folds, num_bag_sets, num_stack_levels
 
     # TODO: Add .delete() method to easily clean-up clones?
     #  Would need to be careful that user doesn't delete important things accidentally.
     # TODO: Add .save_zip() and load_zip() methods to pack and unpack artifacts into a single file to simplify deployment code?
-    def clone(self,
-              path: str,
-              *,
-              return_clone: bool = False,
-              dirs_exist_ok: bool = False):
+    def clone(self, path: str, *, return_clone: bool = False, dirs_exist_ok: bool = False):
         """
         Clone the predictor and all of its artifacts to a new location on local disk.
         This is ideal for use-cases where saving a snapshot of the predictor is desired before performing
         more advanced operations (such as fit_extra and refit_full).
 
         Parameters
         ----------
@@ -3881,24 +4028,22 @@
         -------
         If return_clone == True, returns the loaded cloned TabularPredictor object.
         If return_clone == False, returns the local path to the cloned TabularPredictor object.
 
         """
         assert path != self.path, f"Cannot clone into the same directory as the original predictor! (path='{path}')"
         path_clone = shutil.copytree(src=self.path, dst=path, dirs_exist_ok=dirs_exist_ok)
-        logger.log(30, f"Cloned {self.__class__.__name__} located in '{self.path}' to '{path_clone}'.\n"
-                       f"\tTo load the cloned predictor: predictor_clone = {self.__class__.__name__}.load(path=\"{path_clone}\")")
+        logger.log(
+            30,
+            f"Cloned {self.__class__.__name__} located in '{self.path}' to '{path_clone}'.\n"
+            f'\tTo load the cloned predictor: predictor_clone = {self.__class__.__name__}.load(path="{path_clone}")',
+        )
         return self.__class__.load(path=path_clone) if return_clone else path_clone
 
-    def clone_for_deployment(self,
-                             path: str,
-                             *,
-                             model: str = 'best',
-                             return_clone: bool = False,
-                             dirs_exist_ok: bool = False):
+    def clone_for_deployment(self, path: str, *, model: str = "best", return_clone: bool = False, dirs_exist_ok: bool = False):
         """
         Clone the predictor and all of its artifacts to a new location on local disk,
         then delete the clones artifacts unnecessary during prediction.
         This is ideal for use-cases where saving a snapshot of the predictor is desired before performing
         more advanced operations (such as fit_extra and refit_full).
 
         Note that the clone can no longer fit new models,
@@ -3929,34 +4074,37 @@
 
         Returns
         -------
         If return_clone == True, returns the loaded cloned TabularPredictor object.
         If return_clone == False, returns the local path to the cloned TabularPredictor object.
         """
         predictor_clone = self.clone(path=path, return_clone=True, dirs_exist_ok=dirs_exist_ok)
-        if model == 'best':
+        if model == "best":
             model = predictor_clone.get_model_best()
             logger.log(30, f"Clone: Keeping minimum set of models required to predict with best model '{model}'...")
         else:
             logger.log(30, f"Clone: Keeping minimum set of models required to predict with model '{model}'...")
         predictor_clone.delete_models(models_to_keep=model, dry_run=False)
         if isinstance(model, str) and model in predictor_clone.get_model_names(can_infer=True):
             predictor_clone.set_model_best(model=model, save_trainer=True)
-        logger.log(30, f"Clone: Removing artifacts unnecessary for prediction. "
-                       f"NOTE: Clone can no longer fit new models, and most functionality except for predict and predict_proba will no longer work")
+        logger.log(
+            30,
+            f"Clone: Removing artifacts unnecessary for prediction. "
+            f"NOTE: Clone can no longer fit new models, and most functionality except for predict and predict_proba will no longer work",
+        )
         predictor_clone.save_space()
         return predictor_clone if return_clone else predictor_clone.path
 
     @staticmethod
     def _check_if_hyperparameters_handle_text(hyperparameters: dict) -> bool:
         """Check if hyperparameters contain a model that supports raw text features as input"""
         models_in_hyperparameters = set()
         is_advanced_hyperparameter_type = False
         for key in hyperparameters:
-            if isinstance(key, int) or key == 'default':
+            if isinstance(key, int) or key == "default":
                 is_advanced_hyperparameter_type = True
                 break
         if is_advanced_hyperparameter_type:
             for key in hyperparameters:
                 for m in hyperparameters[key]:
                     models_in_hyperparameters.add(m)
         else:
@@ -3967,15 +4115,15 @@
             if isinstance(m, str):
                 # TODO: Technically the use of MODEL_TYPES here is a hack since we should derive valid types from trainer,
                 #  but this is required prior to trainer existing.
                 if m in MODEL_TYPES:
                     m = MODEL_TYPES[m]
                 else:
                     continue
-            if m._get_class_tags().get('handles_text', False):
+            if m._get_class_tags().get("handles_text", False):
                 models_in_hyperparameters_raw_text_compatible.append(m)
 
         if models_in_hyperparameters_raw_text_compatible:
             return True
         else:
             return False
 
@@ -3991,15 +4139,15 @@
 
 # Location to store WIP functionality that will be later added to TabularPredictor
 class _TabularPredictorExperimental(TabularPredictor):
     # TODO: Documentation, flesh out capabilities
     # TODO: Rename feature_generator -> feature_pipeline for users?
     # TODO: Return transformed data?
     # TODO: feature_generator_kwargs?
-    def fit_feature_generator(self, data: pd.DataFrame, feature_generator='auto', feature_metadata=None):
+    def fit_feature_generator(self, data: pd.DataFrame, feature_generator="auto", feature_metadata=None):
         self._set_feature_generator(feature_generator=feature_generator, feature_metadata=feature_metadata)
         self._learner.fit_transform_features(data)
 
     # TODO: rename to `advice`
     # TODO: Add documentation
     def _advice(self):
         is_feature_generator_fit = self._learner.feature_generator.is_fit()
@@ -4011,36 +4159,35 @@
             is_learner_fit=is_learner_fit,
             exists_trainer=exists_trainer,
             # TODO
         )
 
         advice_list = []
 
-        if not advice_dict['is_feature_generator_fit']:
-            advice_list.append(
-                'FeatureGenerator has not been fit, consider calling `predictor.fit_feature_generator(data)`.')
-        if not advice_dict['is_learner_fit']:
-            advice_list.append('Learner is not fit, consider calling `predictor.fit(...)`')
-        if not advice_dict['exists_trainer']:
-            advice_list.append('Trainer is not initialized, consider calling `predictor.fit(...)`')
+        if not advice_dict["is_feature_generator_fit"]:
+            advice_list.append("FeatureGenerator has not been fit, consider calling `predictor.fit_feature_generator(data)`.")
+        if not advice_dict["is_learner_fit"]:
+            advice_list.append("Learner is not fit, consider calling `predictor.fit(...)`")
+        if not advice_dict["exists_trainer"]:
+            advice_list.append("Trainer is not initialized, consider calling `predictor.fit(...)`")
         # TODO: Advice on unused features (if no model uses a feature)
         # TODO: Advice on fit_extra
         # TODO: Advice on distill
         # TODO: Advice on leaderboard
         # TODO: Advice on persist
         # TODO: Advice on refit_full
         # TODO: Advice on feature_importance
         # TODO: Advice on dropping poor models
 
-        logger.log(20, '======================= AutoGluon Advice =======================')
+        logger.log(20, "======================= AutoGluon Advice =======================")
         if advice_list:
             for advice in advice_list:
                 logger.log(20, advice)
         else:
-            logger.log(20, 'No further advice found.')
-        logger.log(20, '================================================================')
+            logger.log(20, "No further advice found.")
+        logger.log(20, "================================================================")
 
     @classmethod
     def from_learner(cls, learner: AbstractTabularLearner):
         predictor = cls(label=learner.label, path=learner.path)
         predictor._set_post_fit_vars(learner=learner)
         return predictor
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,132 +1,142 @@
 import logging
 from typing import Dict, List
 
 from autogluon.core.models import AbstractModel
 from autogluon.core.trainer.abstract_trainer import AbstractTrainer
 from autogluon.core.utils import generate_train_test_split
 
-from .model_presets.presets import get_preset_models, MODEL_TYPES
-from .model_presets.presets_distill import get_preset_models_distillation
 from ..models.lgb.lgb_model import LGBModel
+from .model_presets.presets import MODEL_TYPES, get_preset_models
+from .model_presets.presets_distill import get_preset_models_distillation
 
 logger = logging.getLogger(__name__)
 
 
 # This Trainer handles model training details
 class AutoTrainer(AbstractTrainer):
     def construct_model_templates(self, hyperparameters, **kwargs):
-        path = kwargs.pop('path', self.path)
-        problem_type = kwargs.pop('problem_type', self.problem_type)
-        eval_metric = kwargs.pop('eval_metric', self.eval_metric)
-        quantile_levels = kwargs.pop('quantile_levels', self.quantile_levels)
-        invalid_model_names = kwargs.pop('invalid_model_names', self._get_banned_model_names())
-        silent = kwargs.pop('silent', self.verbosity < 3)
-        ag_args_fit = kwargs.pop('ag_args_fit', None)
+        path = kwargs.pop("path", self.path)
+        problem_type = kwargs.pop("problem_type", self.problem_type)
+        eval_metric = kwargs.pop("eval_metric", self.eval_metric)
+        quantile_levels = kwargs.pop("quantile_levels", self.quantile_levels)
+        invalid_model_names = kwargs.pop("invalid_model_names", self._get_banned_model_names())
+        silent = kwargs.pop("silent", self.verbosity < 3)
+        ag_args_fit = kwargs.pop("ag_args_fit", None)
         if quantile_levels is not None:
             if ag_args_fit is None:
                 ag_args_fit = dict()
             ag_args_fit = ag_args_fit.copy()
-            ag_args_fit['quantile_levels'] = quantile_levels
+            ag_args_fit["quantile_levels"] = quantile_levels
 
-        return get_preset_models(path=path,
-                                 problem_type=problem_type,
-                                 eval_metric=eval_metric,
-                                 hyperparameters=hyperparameters,
-                                 ag_args_fit=ag_args_fit,
-                                 invalid_model_names=invalid_model_names,
-                                 silent=silent, **kwargs)
-
-    def fit(self,
-            X,
-            y,
-            hyperparameters,
-            X_val=None,
-            y_val=None,
-            X_unlabeled=None,
-            holdout_frac=0.1,
-            num_stack_levels=0,
-            core_kwargs: dict = None,
-            aux_kwargs: dict = None,
-            time_limit=None,
-            infer_limit=None,
-            infer_limit_batch_size=None,
-            use_bag_holdout=False,
-            groups=None,
-            **kwargs):
+        return get_preset_models(
+            path=path,
+            problem_type=problem_type,
+            eval_metric=eval_metric,
+            hyperparameters=hyperparameters,
+            ag_args_fit=ag_args_fit,
+            invalid_model_names=invalid_model_names,
+            silent=silent,
+            **kwargs,
+        )
+
+    def fit(
+        self,
+        X,
+        y,
+        hyperparameters,
+        X_val=None,
+        y_val=None,
+        X_unlabeled=None,
+        holdout_frac=0.1,
+        num_stack_levels=0,
+        core_kwargs: dict = None,
+        aux_kwargs: dict = None,
+        time_limit=None,
+        infer_limit=None,
+        infer_limit_batch_size=None,
+        use_bag_holdout=False,
+        groups=None,
+        **kwargs,
+    ):
         for key in kwargs:
-            logger.warning(f'Warning: Unknown argument passed to `AutoTrainer.fit()`. Argument: {key}')
+            logger.warning(f"Warning: Unknown argument passed to `AutoTrainer.fit()`. Argument: {key}")
 
         if use_bag_holdout:
             if self.bagged_mode:
-                logger.log(20, f'use_bag_holdout={use_bag_holdout}, will use tuning_data as holdout (will not be used for early stopping).')
+                logger.log(20, f"use_bag_holdout={use_bag_holdout}, will use tuning_data as holdout (will not be used for early stopping).")
             else:
-                logger.warning(f'Warning: use_bag_holdout={use_bag_holdout}, but bagged mode is not enabled. use_bag_holdout will be ignored.')
+                logger.warning(f"Warning: use_bag_holdout={use_bag_holdout}, but bagged mode is not enabled. use_bag_holdout will be ignored.")
 
         if (y_val is None) or (X_val is None):
             if not self.bagged_mode or use_bag_holdout:
                 if groups is not None:
-                    raise AssertionError(f'Validation data must be manually specified if use_bag_holdout and groups are both specified.')
+                    raise AssertionError(f"Validation data must be manually specified if use_bag_holdout and groups are both specified.")
                 if self.bagged_mode:
                     # Need at least 2 samples of each class in train data after split for downstream k-fold splits
                     # to ensure each k-fold has at least 1 sample of each class in training data
                     min_cls_count_train = 2
                 else:
                     min_cls_count_train = 1
                 X, X_val, y, y_val = generate_train_test_split(
                     X,
                     y,
                     problem_type=self.problem_type,
                     test_size=holdout_frac,
                     random_state=self.random_state,
                     min_cls_count_train=min_cls_count_train,
                 )
-                logger.log(20, f'Automatically generating train/validation split with holdout_frac={holdout_frac}, Train Rows: {len(X)}, Val Rows: {len(X_val)}')
+                logger.log(
+                    20, f"Automatically generating train/validation split with holdout_frac={holdout_frac}, Train Rows: {len(X)}, Val Rows: {len(X_val)}"
+                )
         elif self.bagged_mode:
             if not use_bag_holdout:
                 # TODO: User could be intending to blend instead. Add support for blend stacking.
                 #  This error message is necessary because when calculating out-of-fold predictions for user, we want to return them in the form given in train_data,
                 #  but if we merge train and val here, it becomes very confusing from a users perspective, especially because we reset index, making it impossible to match
                 #  the original train_data to the out-of-fold predictions from `predictor.get_oof_pred_proba()`.
-                raise AssertionError('X_val, y_val is not None, but bagged mode was specified. '
-                                     'If calling from `TabularPredictor.fit()`, `tuning_data` should be None.\n'
-                                     'Default bagged mode does not use tuning data / validation data. '
-                                     'Instead, all data (`train_data` and `tuning_data`) should be combined and specified as `train_data`.\n'
-                                     'To avoid this error and use `tuning_data` as holdout data in bagged mode, '
-                                     'specify the following:\n'
-                                     '\tpredictor.fit(..., tuning_data=tuning_data, use_bag_holdout=True)')
+                raise AssertionError(
+                    "X_val, y_val is not None, but bagged mode was specified. "
+                    "If calling from `TabularPredictor.fit()`, `tuning_data` should be None.\n"
+                    "Default bagged mode does not use tuning data / validation data. "
+                    "Instead, all data (`train_data` and `tuning_data`) should be combined and specified as `train_data`.\n"
+                    "To avoid this error and use `tuning_data` as holdout data in bagged mode, "
+                    "specify the following:\n"
+                    "\tpredictor.fit(..., tuning_data=tuning_data, use_bag_holdout=True)"
+                )
 
         # Log the hyperparameters dictionary so it easy to edit if the user wants.
-        log_str = f'User-specified model hyperparameters to be fit:\n' \
-                  '{\n'
+        log_str = f"User-specified model hyperparameters to be fit:\n" "{\n"
         for k in hyperparameters.keys():
             log_str += f"\t'{k}': {hyperparameters[k]},\n"
-        log_str += '}'
+        log_str += "}"
         logger.log(20, log_str)
 
-        self._train_multi_and_ensemble(X=X,
-                                       y=y,
-                                       X_val=X_val,
-                                       y_val=y_val,
-                                       X_unlabeled=X_unlabeled,
-                                       hyperparameters=hyperparameters,
-                                       num_stack_levels=num_stack_levels,
-                                       time_limit=time_limit,
-                                       core_kwargs=core_kwargs,
-                                       aux_kwargs=aux_kwargs,
-                                       infer_limit=infer_limit,
-                                       infer_limit_batch_size=infer_limit_batch_size,
-                                       groups=groups)
+        self._train_multi_and_ensemble(
+            X=X,
+            y=y,
+            X_val=X_val,
+            y_val=y_val,
+            X_unlabeled=X_unlabeled,
+            hyperparameters=hyperparameters,
+            num_stack_levels=num_stack_levels,
+            time_limit=time_limit,
+            core_kwargs=core_kwargs,
+            aux_kwargs=aux_kwargs,
+            infer_limit=infer_limit,
+            infer_limit_batch_size=infer_limit_batch_size,
+            groups=groups,
+        )
 
     def construct_model_templates_distillation(self, hyperparameters, **kwargs):
-        path = kwargs.pop('path', self.path)
-        problem_type = kwargs.pop('problem_type', self.problem_type)
-        eval_metric = kwargs.pop('eval_metric', self.eval_metric)
-        invalid_model_names = kwargs.pop('invalid_model_names', self._get_banned_model_names())
-        silent = kwargs.pop('silent', self.verbosity < 3)
+        path = kwargs.pop("path", self.path)
+        problem_type = kwargs.pop("problem_type", self.problem_type)
+        eval_metric = kwargs.pop("eval_metric", self.eval_metric)
+        invalid_model_names = kwargs.pop("invalid_model_names", self._get_banned_model_names())
+        silent = kwargs.pop("silent", self.verbosity < 3)
 
         # TODO: QUANTILE VERSION?
 
         return get_preset_models_distillation(
             path=path,
             problem_type=problem_type,
             eval_metric=eval_metric,
@@ -135,15 +145,15 @@
             silent=silent,
             **kwargs,
         )
 
     def _get_default_proxy_model_class(self):
         return LGBModel
 
-    def compile_models(self, model_names='all', with_ancestors=False, compiler_configs: dict = None) -> List[str]:
+    def compile_models(self, model_names="all", with_ancestors=False, compiler_configs: dict = None) -> List[str]:
         """Ensures that compiler_configs maps to the correct models if the user specified the same keys as in hyperparameters such as RT, XT, etc."""
         if compiler_configs is not None:
             model_types_map = self._get_model_types_map()
             compiler_configs_new = dict()
             for k in compiler_configs:
                 if k in model_types_map:
                     compiler_configs_new[model_types_map[k]] = compiler_configs[k]
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,57 @@
 import copy
 import inspect
 import logging
 from collections import defaultdict
 
 from autogluon.common.model_filter import ModelFilter
-from autogluon.core.constants import AG_ARGS, AG_ARGS_FIT, AG_ARGS_ENSEMBLE, BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
-from autogluon.core.models import AbstractModel, GreedyWeightedEnsembleModel, StackerEnsembleModel, SimpleWeightedEnsembleModel, DummyModel
+from autogluon.core.constants import (
+    AG_ARGS,
+    AG_ARGS_ENSEMBLE,
+    AG_ARGS_FIT,
+    BINARY,
+    MULTICLASS,
+    QUANTILE,
+    REGRESSION,
+    SOFTCLASS,
+)
+from autogluon.core.models import (
+    AbstractModel,
+    DummyModel,
+    GreedyWeightedEnsembleModel,
+    SimpleWeightedEnsembleModel,
+    StackerEnsembleModel,
+)
 from autogluon.core.trainer.utils import process_hyperparameters
 
-from .presets_custom import get_preset_custom
-from ...models import LGBModel, CatBoostModel, XGBoostModel, RFModel, XTModel, KNNModel, LinearModel,\
-    TabularNeuralNetTorchModel, NNFastAiTabularModel, FastTextModel, TextPredictorModel, \
-    ImagePredictorModel, VowpalWabbitModel, \
-    RuleFitModel, GreedyTreeModel, HSTreeModel, FigsModel, BoostedRulesModel, MultiModalPredictorModel, \
-    FTTransformerModel, TabPFNModel
+from ...models import (
+    BoostedRulesModel,
+    CatBoostModel,
+    FastTextModel,
+    FigsModel,
+    FTTransformerModel,
+    GreedyTreeModel,
+    HSTreeModel,
+    ImagePredictorModel,
+    KNNModel,
+    LGBModel,
+    LinearModel,
+    MultiModalPredictorModel,
+    NNFastAiTabularModel,
+    RFModel,
+    RuleFitModel,
+    TabPFNModel,
+    TabularNeuralNetTorchModel,
+    TextPredictorModel,
+    VowpalWabbitModel,
+    XGBoostModel,
+    XTModel,
+)
 from ...models.tab_transformer.tab_transformer_model import TabTransformerModel
+from .presets_custom import get_preset_custom
 
 logger = logging.getLogger(__name__)
 
 # Higher values indicate higher priority, priority dictates the order models are trained for a given level.
 DEFAULT_MODEL_PRIORITY = dict(
     TABPFN=110,  # highest priority due to its very fast training time
     KNN=100,
@@ -33,15 +66,14 @@
     VW=10,
     FASTTEXT=0,
     AG_TEXT_NN=0,
     AG_IMAGE_NN=0,
     AG_AUTOMM=0,
     TRANSF=0,
     custom=0,
-
     # interpretable models
     IM_RULEFIT=0,
     IM_GREEDYTREE=0,
     IM_FIGS=0,
     IM_HSTREE=0,
     IM_BOOSTEDRULES=0,
 )
@@ -59,15 +91,15 @@
     CAT=60,
     custom=0,
 )
 
 DEFAULT_CUSTOM_MODEL_PRIORITY = 0
 
 # FIXME: v0.7 : Remove this, it is a hack. Model classes should define what problem types they support instead of using this
-DEFAULT_QUANTILE_MODEL = ['DUMMY', 'RF', 'XT', 'FASTAI', 'NN_TORCH', 'ENS_WEIGHTED', 'CAT', 'GBM']  # TODO: OTHERS will be added
+DEFAULT_QUANTILE_MODEL = ["DUMMY", "RF", "XT", "FASTAI", "NN_TORCH", "ENS_WEIGHTED", "CAT", "GBM"]  # TODO: OTHERS will be added
 
 MODEL_TYPES = dict(
     RF=RFModel,
     XT=XTModel,
     KNN=KNNModel,
     GBM=LGBModel,
     CAT=CatBoostModel,
@@ -75,80 +107,73 @@
     NN_TORCH=TabularNeuralNetTorchModel,
     LR=LinearModel,
     FASTAI=NNFastAiTabularModel,
     TRANSF=TabTransformerModel,
     AG_TEXT_NN=TextPredictorModel,
     AG_IMAGE_NN=ImagePredictorModel,
     AG_AUTOMM=MultiModalPredictorModel,
-
     FT_TRANSFORMER=FTTransformerModel,
     TABPFN=TabPFNModel,
-
     FASTTEXT=FastTextModel,
     ENS_WEIGHTED=GreedyWeightedEnsembleModel,
     SIMPLE_ENS_WEIGHTED=SimpleWeightedEnsembleModel,
-
     # interpretable models
     IM_RULEFIT=RuleFitModel,
     IM_GREEDYTREE=GreedyTreeModel,
     IM_FIGS=FigsModel,
     IM_HSTREE=HSTreeModel,
     IM_BOOSTEDRULES=BoostedRulesModel,
     VW=VowpalWabbitModel,
-
     DUMMY=DummyModel,
 )
 
 
 # TODO: v1.0 Have this be defined in the model class
 DEFAULT_MODEL_NAMES = {
-    RFModel: 'RandomForest',
-    XTModel: 'ExtraTrees',
-    KNNModel: 'KNeighbors',
-    LGBModel: 'LightGBM',
-    CatBoostModel: 'CatBoost',
-    XGBoostModel: 'XGBoost',
-    TabularNeuralNetTorchModel: 'NeuralNetTorch',
-    LinearModel: 'LinearModel',
-    NNFastAiTabularModel: 'NeuralNetFastAI',
-    TabTransformerModel: 'Transformer',
-    TextPredictorModel: 'TextPredictor',
-    ImagePredictorModel: 'ImagePredictor',
-    MultiModalPredictorModel: 'MultiModalPredictor',
-
-    FTTransformerModel: 'FTTransformer',
-    TabPFNModel: 'TabPFN',
-
-    FastTextModel: 'FastText',
-    VowpalWabbitModel: 'VowpalWabbit',
-    GreedyWeightedEnsembleModel: 'WeightedEnsemble',
-    SimpleWeightedEnsembleModel: 'WeightedEnsemble',
-
+    RFModel: "RandomForest",
+    XTModel: "ExtraTrees",
+    KNNModel: "KNeighbors",
+    LGBModel: "LightGBM",
+    CatBoostModel: "CatBoost",
+    XGBoostModel: "XGBoost",
+    TabularNeuralNetTorchModel: "NeuralNetTorch",
+    LinearModel: "LinearModel",
+    NNFastAiTabularModel: "NeuralNetFastAI",
+    TabTransformerModel: "Transformer",
+    TextPredictorModel: "TextPredictor",
+    ImagePredictorModel: "ImagePredictor",
+    MultiModalPredictorModel: "MultiModalPredictor",
+    FTTransformerModel: "FTTransformer",
+    TabPFNModel: "TabPFN",
+    FastTextModel: "FastText",
+    VowpalWabbitModel: "VowpalWabbit",
+    GreedyWeightedEnsembleModel: "WeightedEnsemble",
+    SimpleWeightedEnsembleModel: "WeightedEnsemble",
     # Interpretable models
-    RuleFitModel: 'RuleFit',
-    GreedyTreeModel: 'GreedyTree',
-    FigsModel: 'Figs',
-    HSTreeModel: 'HierarchicalShrinkageTree',
-    BoostedRulesModel: 'BoostedRules',
+    RuleFitModel: "RuleFit",
+    GreedyTreeModel: "GreedyTree",
+    FigsModel: "Figs",
+    HSTreeModel: "HierarchicalShrinkageTree",
+    BoostedRulesModel: "BoostedRules",
 }
 
 
 VALID_AG_ARGS_KEYS = {
-    'name',
-    'name_main',
-    'name_prefix',
-    'name_suffix',
-    'name_bag_suffix',
-    'model_type',
-    'priority',
-    'problem_types',
-    'disable_in_hpo',
-    'valid_stacker',
-    'valid_base',
-    'hyperparameter_tune_kwargs',
+    "name",
+    "name_main",
+    "name_prefix",
+    "name_suffix",
+    "name_bag_suffix",
+    "model_type",
+    "priority",
+    "problem_types",
+    "disable_in_hpo",
+    "valid_stacker",
+    "valid_base",
+    "hyperparameter_tune_kwargs",
 }
 
 
 # DONE: Add levels, including 'default'
 # DONE: Add lists
 # DONE: Add custom which can append to lists
 # DONE: Add special optional AG args for things like name prefix, name suffix, name, etc.
@@ -173,20 +198,20 @@
     ensemble_type=StackerEnsembleModel,
     ensemble_kwargs: dict = None,
     ag_args_fit=None,
     ag_args=None,
     ag_args_ensemble=None,
     name_suffix: str = None,
     default_priorities=None,
-    invalid_model_names: list = None, 
+    invalid_model_names: list = None,
     included_model_types: list = None,
     excluded_model_types: list = None,
     hyperparameter_preprocess_func=None,
     hyperparameter_preprocess_kwargs=None,
-    silent=True
+    silent=True,
 ):
     hyperparameters = process_hyperparameters(hyperparameters)
     if hyperparameter_preprocess_func is not None:
         if hyperparameter_preprocess_kwargs is None:
             hyperparameter_preprocess_kwargs = dict()
         hyperparameters = hyperparameter_preprocess_func(hyperparameters, **hyperparameter_preprocess_kwargs)
     if problem_type not in [BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE]:
@@ -196,87 +221,100 @@
         invalid_name_set.update(invalid_model_names)
 
     if default_priorities is None:
         default_priorities = copy.deepcopy(DEFAULT_MODEL_PRIORITY)
         if problem_type in PROBLEM_TYPE_MODEL_PRIORITY:
             default_priorities.update(PROBLEM_TYPE_MODEL_PRIORITY[problem_type])
 
-    level_key = level if level in hyperparameters.keys() else 'default'
-    if level_key not in hyperparameters.keys() and level_key == 'default':
-        hyperparameters = {'default': hyperparameters}
+    level_key = level if level in hyperparameters.keys() else "default"
+    if level_key not in hyperparameters.keys() and level_key == "default":
+        hyperparameters = {"default": hyperparameters}
     hp_level = hyperparameters[level_key]
-    hp_level = ModelFilter.filter_models(
-        models=hp_level,
-        included_model_types=included_model_types,
-        excluded_model_types=excluded_model_types
-    )
+    hp_level = ModelFilter.filter_models(models=hp_level, included_model_types=included_model_types, excluded_model_types=excluded_model_types)
     model_cfg_priority_dict = defaultdict(list)
     model_type_list = list(hp_level.keys())
     for model_type in model_type_list:
         models_of_type = hp_level[model_type]
         if not isinstance(models_of_type, list):
             models_of_type = [models_of_type]
         model_cfgs_to_process = []
         for model_cfg in models_of_type:
             if isinstance(model_cfg, str):
-                if model_type == 'AG_TEXT_NN' or model_type == 'AG_AUTOMM':
+                if model_type == "AG_TEXT_NN" or model_type == "AG_AUTOMM":
                     model_cfgs_to_process.append({})
                 else:
                     model_cfgs_to_process += get_preset_custom(name=model_cfg, problem_type=problem_type)
             else:
                 model_cfgs_to_process.append(model_cfg)
         for model_cfg in model_cfgs_to_process:
-            model_cfg = clean_model_cfg(model_cfg=model_cfg, model_type=model_type, ag_args=ag_args, ag_args_ensemble=ag_args_ensemble, ag_args_fit=ag_args_fit, problem_type=problem_type)
-            model_cfg[AG_ARGS]['priority'] = model_cfg[AG_ARGS].get('priority', default_priorities.get(model_type, DEFAULT_CUSTOM_MODEL_PRIORITY))
-            model_priority = model_cfg[AG_ARGS]['priority']
+            model_cfg = clean_model_cfg(
+                model_cfg=model_cfg,
+                model_type=model_type,
+                ag_args=ag_args,
+                ag_args_ensemble=ag_args_ensemble,
+                ag_args_fit=ag_args_fit,
+                problem_type=problem_type,
+            )
+            model_cfg[AG_ARGS]["priority"] = model_cfg[AG_ARGS].get("priority", default_priorities.get(model_type, DEFAULT_CUSTOM_MODEL_PRIORITY))
+            model_priority = model_cfg[AG_ARGS]["priority"]
             # Check if model_cfg is valid
             is_valid = is_model_cfg_valid(model_cfg, level=level, problem_type=problem_type)
             if AG_ARGS_FIT in model_cfg and not model_cfg[AG_ARGS_FIT]:
                 model_cfg.pop(AG_ARGS_FIT)
             if is_valid:
                 model_cfg_priority_dict[model_priority].append(model_cfg)
 
     model_cfg_priority_list = [model for priority in sorted(model_cfg_priority_dict.keys(), reverse=True) for model in model_cfg_priority_dict[priority]]
 
     if not silent:
-        logger.log(20, 'Model configs that will be trained (in order):')
+        logger.log(20, "Model configs that will be trained (in order):")
     models = []
     model_args_fit = {}
     for model_cfg in model_cfg_priority_list:
-        model = model_factory(model_cfg, path=path, problem_type=problem_type, eval_metric=eval_metric,
-                              name_suffix=name_suffix, ensemble_type=ensemble_type, ensemble_kwargs=ensemble_kwargs,
-                              invalid_name_set=invalid_name_set, level=level)
+        model = model_factory(
+            model_cfg,
+            path=path,
+            problem_type=problem_type,
+            eval_metric=eval_metric,
+            name_suffix=name_suffix,
+            ensemble_type=ensemble_type,
+            ensemble_kwargs=ensemble_kwargs,
+            invalid_name_set=invalid_name_set,
+            level=level,
+        )
         invalid_name_set.add(model.name)
-        if 'hyperparameter_tune_kwargs' in model_cfg[AG_ARGS]:
-            model_args_fit[model.name] = {'hyperparameter_tune_kwargs': model_cfg[AG_ARGS]['hyperparameter_tune_kwargs']}
-        if 'ag_args_ensemble' in model_cfg and not model_cfg['ag_args_ensemble']:
-            model_cfg.pop('ag_args_ensemble')
+        if "hyperparameter_tune_kwargs" in model_cfg[AG_ARGS]:
+            model_args_fit[model.name] = {"hyperparameter_tune_kwargs": model_cfg[AG_ARGS]["hyperparameter_tune_kwargs"]}
+        if "ag_args_ensemble" in model_cfg and not model_cfg["ag_args_ensemble"]:
+            model_cfg.pop("ag_args_ensemble")
         if not silent:
-            logger.log(20, f'\t{model.name}: \t{model_cfg}')
+            logger.log(20, f"\t{model.name}: \t{model_cfg}")
         models.append(model)
     return models, model_args_fit
 
 
 def clean_model_cfg(model_cfg: dict, model_type=None, ag_args=None, ag_args_ensemble=None, ag_args_fit=None, problem_type=None):
     model_cfg = copy.deepcopy(model_cfg)
     if AG_ARGS not in model_cfg:
         model_cfg[AG_ARGS] = dict()
-    if 'model_type' not in model_cfg[AG_ARGS]:
-        model_cfg[AG_ARGS]['model_type'] = model_type
-    if model_cfg[AG_ARGS]['model_type'] is None:
-        raise AssertionError(f'model_type was not specified for model! Model: {model_cfg}')
-    model_type = model_cfg[AG_ARGS]['model_type']
+    if "model_type" not in model_cfg[AG_ARGS]:
+        model_cfg[AG_ARGS]["model_type"] = model_type
+    if model_cfg[AG_ARGS]["model_type"] is None:
+        raise AssertionError(f"model_type was not specified for model! Model: {model_cfg}")
+    model_type = model_cfg[AG_ARGS]["model_type"]
     if not inspect.isclass(model_type):
         model_type = MODEL_TYPES[model_type]
     elif not issubclass(model_type, AbstractModel):
-        logger.warning(f'Warning: Custom model type {model_type} does not inherit from {AbstractModel}. This may lead to instability. Consider wrapping {model_type} with an implementation of {AbstractModel}!')
+        logger.warning(
+            f"Warning: Custom model type {model_type} does not inherit from {AbstractModel}. This may lead to instability. Consider wrapping {model_type} with an implementation of {AbstractModel}!"
+        )
     else:
-        logger.log(20, f'Custom Model Type Detected: {model_type}')
-    model_cfg[AG_ARGS]['model_type'] = model_type
-    model_type_real = model_cfg[AG_ARGS]['model_type']
+        logger.log(20, f"Custom Model Type Detected: {model_type}")
+    model_cfg[AG_ARGS]["model_type"] = model_type
+    model_type_real = model_cfg[AG_ARGS]["model_type"]
     if not inspect.isclass(model_type_real):
         model_type_real = MODEL_TYPES[model_type_real]
     default_ag_args = model_type_real._get_default_ag_args()
     if ag_args is not None:
         model_extra_ag_args = ag_args.copy()
         model_extra_ag_args.update(model_cfg[AG_ARGS])
         model_cfg[AG_ARGS] = model_extra_ag_args
@@ -301,62 +339,68 @@
 
 
 # Check if model is valid
 def is_model_cfg_valid(model_cfg, level=1, problem_type=None):
     is_valid = True
     for key in model_cfg.get(AG_ARGS, {}):
         if key not in VALID_AG_ARGS_KEYS:
-            logger.warning(f'WARNING: Unknown ag_args key: {key}')
+            logger.warning(f"WARNING: Unknown ag_args key: {key}")
     if AG_ARGS not in model_cfg:
         is_valid = False  # AG_ARGS is required
-    elif model_cfg[AG_ARGS].get('model_type', None) is None:
+    elif model_cfg[AG_ARGS].get("model_type", None) is None:
         is_valid = False  # model_type is required
-    elif model_cfg[AG_ARGS].get('hyperparameter_tune_kwargs', None) and model_cfg[AG_ARGS].get('disable_in_hpo', False):
+    elif model_cfg[AG_ARGS].get("hyperparameter_tune_kwargs", None) and model_cfg[AG_ARGS].get("disable_in_hpo", False):
         is_valid = False
-    elif not model_cfg[AG_ARGS].get('valid_stacker', True) and level > 1:
+    elif not model_cfg[AG_ARGS].get("valid_stacker", True) and level > 1:
         is_valid = False  # Not valid as a stacker model
-    elif not model_cfg[AG_ARGS].get('valid_base', True) and level == 1:
+    elif not model_cfg[AG_ARGS].get("valid_base", True) and level == 1:
         is_valid = False  # Not valid as a base model
-    elif problem_type is not None and problem_type not in model_cfg[AG_ARGS].get('problem_types', [problem_type]):
+    elif problem_type is not None and problem_type not in model_cfg[AG_ARGS].get("problem_types", [problem_type]):
         is_valid = False  # Not valid for this problem_type
     return is_valid
 
 
 def model_factory(
-        model, path, problem_type, eval_metric,
-        name_suffix=None, ensemble_type=StackerEnsembleModel, ensemble_kwargs=None,
-        invalid_name_set=None, level=1,
+    model,
+    path,
+    problem_type,
+    eval_metric,
+    name_suffix=None,
+    ensemble_type=StackerEnsembleModel,
+    ensemble_kwargs=None,
+    invalid_name_set=None,
+    level=1,
 ):
     if invalid_name_set is None:
         invalid_name_set = set()
-    model_type = model[AG_ARGS]['model_type']
+    model_type = model[AG_ARGS]["model_type"]
     if not inspect.isclass(model_type):
         model_type = MODEL_TYPES[model_type]
-    name_orig = model[AG_ARGS].get('name', None)
+    name_orig = model[AG_ARGS].get("name", None)
     if name_orig is None:
-        name_main = model[AG_ARGS].get('name_main', DEFAULT_MODEL_NAMES.get(model_type, model_type.__name__))
-        name_prefix = model[AG_ARGS].get('name_prefix', '')
-        name_suff = model[AG_ARGS].get('name_suffix', '')
+        name_main = model[AG_ARGS].get("name_main", DEFAULT_MODEL_NAMES.get(model_type, model_type.__name__))
+        name_prefix = model[AG_ARGS].get("name_prefix", "")
+        name_suff = model[AG_ARGS].get("name_suffix", "")
         name_orig = name_prefix + name_main + name_suff
     name_stacker = None
     num_increment = 2
     if name_suffix is None:
-        name_suffix = ''
+        name_suffix = ""
     if ensemble_kwargs is None:
-        name = f'{name_orig}{name_suffix}'
+        name = f"{name_orig}{name_suffix}"
         while name in invalid_name_set:  # Ensure name is unique
-            name = f'{name_orig}_{num_increment}{name_suffix}'
+            name = f"{name_orig}_{num_increment}{name_suffix}"
             num_increment += 1
     else:
         name = name_orig
-        name_bag_suffix = model[AG_ARGS].get('name_bag_suffix', '_BAG')
-        name_stacker = f'{name}{name_bag_suffix}_L{level}{name_suffix}'
+        name_bag_suffix = model[AG_ARGS].get("name_bag_suffix", "_BAG")
+        name_stacker = f"{name}{name_bag_suffix}_L{level}{name_suffix}"
         while name_stacker in invalid_name_set:  # Ensure name is unique
-            name = f'{name_orig}_{num_increment}'
-            name_stacker = f'{name}{name_bag_suffix}_L{level}{name_suffix}'
+            name = f"{name_orig}_{num_increment}"
+            name_stacker = f"{name}{name_bag_suffix}_L{level}{name_suffix}"
             num_increment += 1
     model_params = copy.deepcopy(model)
     model_params.pop(AG_ARGS, None)
     model_params.pop(AG_ARGS_ENSEMBLE, None)
 
     model_init_kwargs = dict(
         path=path,
@@ -365,47 +409,54 @@
         eval_metric=eval_metric,
         hyperparameters=model_params,
     )
 
     if ensemble_kwargs is not None:
         ensemble_kwargs_model = copy.deepcopy(ensemble_kwargs)
         extra_ensemble_hyperparameters = copy.deepcopy(model.get(AG_ARGS_ENSEMBLE, dict()))
-        ensemble_kwargs_model['hyperparameters'] = ensemble_kwargs_model.get('hyperparameters', {})
-        if ensemble_kwargs_model['hyperparameters'] is None:
-            ensemble_kwargs_model['hyperparameters'] = {}
-        ensemble_kwargs_model['hyperparameters'].update(extra_ensemble_hyperparameters)
-        model_init = ensemble_type(path=path, name=name_stacker, model_base=model_type, model_base_kwargs=model_init_kwargs,
-                                   **ensemble_kwargs_model)
+        ensemble_kwargs_model["hyperparameters"] = ensemble_kwargs_model.get("hyperparameters", {})
+        if ensemble_kwargs_model["hyperparameters"] is None:
+            ensemble_kwargs_model["hyperparameters"] = {}
+        ensemble_kwargs_model["hyperparameters"].update(extra_ensemble_hyperparameters)
+        model_init = ensemble_type(path=path, name=name_stacker, model_base=model_type, model_base_kwargs=model_init_kwargs, **ensemble_kwargs_model)
     else:
         model_init = model_type(**model_init_kwargs)
 
     return model_init
 
 
 # TODO: v0.1 cleanup and avoid hardcoded logic with model names
 def get_preset_models_softclass(hyperparameters, invalid_model_names: list = None, **kwargs):
     from autogluon.core.metrics.softclass_metrics import soft_log_loss
-    model_types_standard = ['GBM', 'NN_TORCH', 'CAT', 'ENS_WEIGHTED']
+
+    model_types_standard = ["GBM", "NN_TORCH", "CAT", "ENS_WEIGHTED"]
     hyperparameters = copy.deepcopy(hyperparameters)
 
     hyperparameters_standard = {key: hyperparameters[key] for key in hyperparameters if key in model_types_standard}
-    hyperparameters_rf = {key: hyperparameters[key] for key in hyperparameters if key == 'RF'}
+    hyperparameters_rf = {key: hyperparameters[key] for key in hyperparameters if key == "RF"}
 
     # Swap RF criterion for MSE:
-    if 'RF' in hyperparameters_rf:
-        rf_params = hyperparameters_rf['RF']
-        rf_newparams = {'criterion': 'squared_error', 'ag_args': {'name_suffix': 'MSE'}}
+    if "RF" in hyperparameters_rf:
+        rf_params = hyperparameters_rf["RF"]
+        rf_newparams = {"criterion": "squared_error", "ag_args": {"name_suffix": "MSE"}}
         for i in range(len(rf_params)):
             rf_params[i].update(rf_newparams)
-        rf_params = [j for n, j in enumerate(rf_params) if j not in rf_params[(n+1):]]  # Remove duplicates which may arise after overwriting criterion
-        hyperparameters_standard['RF'] = rf_params
-    models, model_args_fit = get_preset_models(problem_type=SOFTCLASS, eval_metric=soft_log_loss,
-                                               hyperparameters=hyperparameters_standard,
-                                               default_priorities=DEFAULT_SOFTCLASS_PRIORITY, invalid_model_names=invalid_model_names, **kwargs)
+        rf_params = [j for n, j in enumerate(rf_params) if j not in rf_params[(n + 1) :]]  # Remove duplicates which may arise after overwriting criterion
+        hyperparameters_standard["RF"] = rf_params
+    models, model_args_fit = get_preset_models(
+        problem_type=SOFTCLASS,
+        eval_metric=soft_log_loss,
+        hyperparameters=hyperparameters_standard,
+        default_priorities=DEFAULT_SOFTCLASS_PRIORITY,
+        invalid_model_names=invalid_model_names,
+        **kwargs,
+    )
     if len(models) == 0:
-        raise ValueError("At least one of the following model-types must be present in hyperparameters: ['GBM','CAT','RF'], "
-                         "These are the only supported models for softclass prediction problems. "
-                         "Softclass problems are also not yet supported for fit() with per-stack level hyperparameters.")
+        raise ValueError(
+            "At least one of the following model-types must be present in hyperparameters: ['GBM','CAT','RF'], "
+            "These are the only supported models for softclass prediction problems. "
+            "Softclass problems are also not yet supported for fit() with per-stack level hyperparameters."
+        )
     for model in models:
         model.normalize_pred_probas = True  # FIXME: Do we need to do this for child models too?
 
     return models, model_args_fit
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from autogluon.core.constants import AG_ARGS
+
 from ...models.lgb.hyperparameters.parameters import get_param_baseline_custom
 
 
 # Returns list of models created by a custom name preset.
 def get_preset_custom(name, problem_type):
     if not isinstance(name, str):
-        raise ValueError(f'Expected string value for custom model, but was given {name}')
+        raise ValueError(f"Expected string value for custom model, but was given {name}")
     # Custom model
-    if name == 'GBMLarge':
+    if name == "GBMLarge":
         model = get_param_baseline_custom(problem_type)
-        model[AG_ARGS] = dict(model_type='GBM', name_suffix='Large', hyperparameter_tune_kwargs=None, priority=0)
+        model[AG_ARGS] = dict(model_type="GBM", name_suffix="Large", hyperparameter_tune_kwargs=None, priority=0)
         return [model]
     else:
-        raise ValueError(f'Unknown custom model preset: {name}')
+        raise ValueError(f"Unknown custom model preset: {name}")
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,52 +13,63 @@
     GBM=100,
     CAT=80,
     RF=70,
     custom=0,
 )
 
 
-def get_preset_models_distillation(path, problem_type, eval_metric, hyperparameters,
-                                   level=1, name_suffix='_DSTL', invalid_model_names: list = None, **kwargs):
+def get_preset_models_distillation(path, problem_type, eval_metric, hyperparameters, level=1, name_suffix="_DSTL", invalid_model_names: list = None, **kwargs):
     hyperparameters = process_hyperparameters(hyperparameters)
-    level_key = level if level in hyperparameters.keys() else 'default'
-    if level_key not in hyperparameters.keys() and level_key == 'default':
-        hyperparameters = {'default': hyperparameters}
+    level_key = level if level in hyperparameters.keys() else "default"
+    if level_key not in hyperparameters.keys() and level_key == "default":
+        hyperparameters = {"default": hyperparameters}
     hyperparameters = hyperparameters[level_key]
     if problem_type == BINARY:  # convert to regression in distillation
         eval_metric = mean_squared_error
         # Constrain output-range of NN:
-        nn_outputrange = {'y_range': (0.0,1.0), 'y_range_extend': 0.0}
+        nn_outputrange = {"y_range": (0.0, 1.0), "y_range_extend": 0.0}
         nn_hyperparameters = None
         if isinstance(nn_hyperparameters, list):
             for i in range(len(nn_hyperparameters)):
                 nn_hyperparameters[i].update(nn_outputrange)
         elif nn_hyperparameters is not None:
             nn_hyperparameters.update(nn_outputrange)
         # Swap RF criterion for MSE:
-        rf_newparams = {'criterion': 'squared_error', 'ag_args': {'name_suffix': 'MSE'}}
-        if 'RF' in hyperparameters:
-            rf_hyperparameters = hyperparameters['RF']
+        rf_newparams = {"criterion": "squared_error", "ag_args": {"name_suffix": "MSE"}}
+        if "RF" in hyperparameters:
+            rf_hyperparameters = hyperparameters["RF"]
         else:
             rf_hyperparameters = None
         if isinstance(rf_hyperparameters, list):
             for i in range(len(rf_hyperparameters)):
                 rf_hyperparameters[i].update(rf_newparams)
-            rf_hyperparameters = [j for n, j in enumerate(rf_hyperparameters) if j not in rf_hyperparameters[(n+1):]]  # Remove duplicates which may arise after overwriting criterion
+            rf_hyperparameters = [
+                j for n, j in enumerate(rf_hyperparameters) if j not in rf_hyperparameters[(n + 1) :]
+            ]  # Remove duplicates which may arise after overwriting criterion
         elif rf_hyperparameters is not None:
             rf_hyperparameters.update(rf_newparams)
-        if 'RF' in hyperparameters:
-            hyperparameters['RF'] = rf_hyperparameters
+        if "RF" in hyperparameters:
+            hyperparameters["RF"] = rf_hyperparameters
 
     if problem_type == MULTICLASS:
-        models, model_args_fit = get_preset_models_softclass(path=path, hyperparameters=hyperparameters, level=level,
-                                                             name_suffix=name_suffix, invalid_model_names=invalid_model_names, **kwargs)
+        models, model_args_fit = get_preset_models_softclass(
+            path=path, hyperparameters=hyperparameters, level=level, name_suffix=name_suffix, invalid_model_names=invalid_model_names, **kwargs
+        )
     else:  # BINARY or REGRESSION
-        models, model_args_fit = get_preset_models(path=path, problem_type=REGRESSION, eval_metric=eval_metric, hyperparameters=hyperparameters, level=level,
-                                                   name_suffix=name_suffix, default_priorities=DEFAULT_DISTILL_PRIORITY, invalid_model_names=invalid_model_names, **kwargs)
+        models, model_args_fit = get_preset_models(
+            path=path,
+            problem_type=REGRESSION,
+            eval_metric=eval_metric,
+            hyperparameters=hyperparameters,
+            level=level,
+            name_suffix=name_suffix,
+            default_priorities=DEFAULT_DISTILL_PRIORITY,
+            invalid_model_names=invalid_model_names,
+            **kwargs,
+        )
 
     if problem_type in [MULTICLASS, BINARY]:
         for model in models:
             model.normalize_pred_probas = True
 
     logger.log(20, f"Distilling with each of these student models: {[model.name for model in models]}")
     return models, model_args_fit
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.8.1b20230623/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import copy, logging
+import copy
+import logging
+
 import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: currently is buggy
 class FeaturePruner:
@@ -22,45 +24,45 @@
         self.threshold = self.threshold_baseline
         self.cur_iteration = 0
         self.tuned = False
         self.early_stopping_rounds = 2
 
     def evaluate(self):
         untuned_score = self.score_in_iter[0]
-        logger.debug('untuned_score: %s' % untuned_score)
-        logger.debug('best_score: %s' % self.best_score)
-        logger.debug('best_iteration: %s' % self.best_iteration)
+        logger.debug("untuned_score: %s" % untuned_score)
+        logger.debug("best_score: %s" % self.best_score)
+        logger.debug("best_iteration: %s" % self.best_iteration)
 
         data_dict = {
-            'score': self.score_in_iter,
-            'feature_count': self.valid_feature_counts,
-            'threshold': self.thresholds,
+            "score": self.score_in_iter,
+            "feature_count": self.valid_feature_counts,
+            "threshold": self.thresholds,
         }
         logger.debug(self.gain_dfs[self.best_iteration])
         z = pd.DataFrame(data=data_dict)
         # logger.debug(z)
-        z_sorted = z.sort_values(by=['score'], ascending=False)
+        z_sorted = z.sort_values(by=["score"], ascending=False)
         # logger.debug(z_sorted)
 
     # TODO: CV5 instead of holdout? Should be better
     # TODO: Add holdout here, it is overfitting with Logistic Regression
     def tune(self, X, y, X_val, y_val, X_holdout, y_holdout, total_runs=999):
         objective_goal_is_negative = False  # Fixed to false if using sklearn scorers # self.model_base.problem_type == REGRESSION  # TODO: if objective function goal = lower (logloss, MAE, etc.)
-        logger.log(15, 'Feature-pruning '+str(self.model_base.name)+' for '+str(total_runs)+' runs...')
+        logger.log(15, "Feature-pruning " + str(self.model_base.name) + " for " + str(total_runs) + " runs...")
 
         if len(self.features_in_iter) == 0:
             valid_features = X.columns.values
         else:
             valid_features = self.features_in_iter[-1]
 
         iter_since_best = 0
         iter_start = self.cur_iteration
         for iteration in range(self.cur_iteration, total_runs):
             self.cur_iteration = iteration
-            logger.debug('iteration: %s ' % iteration)
+            logger.debug("iteration: %s " % iteration)
             X_subset = X[valid_features].copy()
             X_val_subset = X_val[valid_features].copy()
             self.thresholds.append(self.threshold)
             self.valid_feature_counts.append(len(valid_features))
             self.features_in_iter.append(valid_features)
 
             if self.is_fit and (iteration == iter_start):
@@ -68,40 +70,40 @@
             else:
                 model_iter = copy.deepcopy(self.model_base)
                 model_iter.fit(X=X_subset, y=y, X_val=X_val_subset, y_val=y_val)
 
             banned_features = []
 
             feature_importance = None
-            if hasattr(model_iter.model, 'feature_importances_'):
+            if hasattr(model_iter.model, "feature_importances_"):
                 feature_importance = model_iter.model.feature_importances_
-            elif hasattr(model_iter.model, 'feature_importance'):
+            elif hasattr(model_iter.model, "feature_importance"):
                 feature_importance = model_iter.model.feature_importance()
 
             if feature_importance is not None:
                 a = pd.Series(data=feature_importance, index=X_subset.columns)
                 unused_features = a[a == 0]
 
-                logger.log(15, 'Unused features after pruning: '+ str(list(unused_features.index)))
+                logger.log(15, "Unused features after pruning: " + str(list(unused_features.index)))
                 features_to_use = [feature for feature in valid_features if feature not in unused_features.index]
                 banned_features += list(unused_features.index)
             else:
                 features_to_use = list(valid_features)
 
             cur_score_val = model_iter.score(X=X_val_subset, y=y_val)
             cur_score = model_iter.score(X=X_holdout[valid_features], y=y_holdout)
 
-            logger.log(15, 'Iter '+str(iteration)+'  Score: '+str(cur_score))
-            logger.log(15, 'Iter '+str(iteration)+ '  Score Val: '+str(cur_score_val))
+            logger.log(15, "Iter " + str(iteration) + "  Score: " + str(cur_score))
+            logger.log(15, "Iter " + str(iteration) + "  Score Val: " + str(cur_score_val))
             if objective_goal_is_negative:
                 cur_score = -cur_score
 
             if self.best_score == 0 or cur_score > self.best_score:
                 logger.log(15, "New best score found!")
-                logger.log(15, str(cur_score)+ ' > '+str(self.best_score))
+                logger.log(15, str(cur_score) + " > " + str(self.best_score))
                 self.best_score = cur_score
                 self.best_iteration = iteration
                 iter_since_best = 0
             else:
                 iter_since_best += 1
 
             self.score_in_iter.append(cur_score)
@@ -121,43 +123,43 @@
             # TODO: Save gain_df, banned_features
 
             self.threshold = self.adjust_threshold(gain_df, self.threshold)
 
             banned_df = gain_df.loc[gain_df >= self.threshold].index
             banned_features += list(banned_df)
 
-            logger.log(15, "Banned features: "+str(banned_features))
+            logger.log(15, "Banned features: " + str(banned_features))
             self.banned_features_in_iter.append(banned_features)
             valid_features = [feature for feature in valid_features if feature not in banned_features]
 
             if len(valid_features) == 0:
-                logger.log(15, 'No more features to remove, Feature pruning complete')
-                logger.log(15, "score_in_iter: "+str(self.score_in_iter))
+                logger.log(15, "No more features to remove, Feature pruning complete")
+                logger.log(15, "score_in_iter: " + str(self.score_in_iter))
                 self.tuned = True
                 break
         self.tuned = True
 
     @staticmethod
     def adjust_threshold(gain_df, threshold):
         if gain_df.shape[0] == 0:
-            raise BaseException('ran out of features to prune!')
+            raise BaseException("ran out of features to prune!")
         banned_df = gain_df.loc[gain_df >= threshold].index
         banned_features = list(banned_df)
 
         if len(banned_features) == 0:
             if threshold < -100000000:  # FIXME: Hacked for regression
-                raise BaseException('threshold already max!')
+                raise BaseException("threshold already max!")
             elif threshold > 0.000001:
                 threshold_new = threshold / 2
             elif threshold > 0:
                 threshold_new = 0
             elif threshold == 0:
                 threshold_new = -0.00000001
             elif (threshold < 0) and (threshold > -0.0001):
                 threshold_new = threshold * 2
             else:
                 threshold_new = gain_df.max()
 
-            logger.log(10, 'Adjusting threshold to %s' % threshold_new)
+            logger.log(10, "Adjusting threshold to %s" % threshold_new)
             return FeaturePruner.adjust_threshold(gain_df=gain_df, threshold=threshold_new)
         else:
             return threshold
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.8.1b20230622
+Version: 0.8.1b20230623
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.1b20230622/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-0.8.1b20230623/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 numpy<1.27,>=1.21
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 networkx<4,>=3.0
-autogluon.core==0.8.1b20230622
-autogluon.features==0.8.1b20230622
+autogluon.core==0.8.1b20230623
+autogluon.features==0.8.1b20230623
 
 [all]
-torch<1.14,>=1.9
 xgboost<1.8,>=1.6
+torch<1.14,>=1.9
+fastai<2.8,>=2.3.1
 catboost<1.3,>=1.1
 lightgbm<3.4,>=3.3
-fastai<2.8,>=2.3.1
-autogluon.core[all]==0.8.1b20230622
+autogluon.core[all]==0.8.1b20230623
 
 [all:sys_platform == "darwin"]
 catboost<1.2,>=1.1
 
 [catboost]
 catboost<1.3,>=1.1
 
@@ -30,15 +30,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<3.4,>=3.3
 
 [ray]
-autogluon.core[all]==0.8.1b20230622
+autogluon.core[all]==0.8.1b20230623
 
 [skex]
 scikit-learn-intelex<2023.2,>=2021.7
 
 [skl2onnx]
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
```

