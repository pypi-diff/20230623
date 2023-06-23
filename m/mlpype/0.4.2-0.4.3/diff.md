# Comparing `tmp/mlpype-0.4.2.tar.gz` & `tmp/mlpype-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-0.4.2.tar", last modified: Tue Jun 20 17:14:56 2023, max compression
+gzip compressed data, was "mlpype-0.4.3.tar", last modified: Fri Jun 23 07:13:54 2023, max compression
```

## Comparing `mlpype-0.4.2.tar` & `mlpype-0.4.3.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.775354 mlpype-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-20 17:11:28.000000 mlpype-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-20 17:14:56.775354 mlpype-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-20 17:11:28.000000 mlpype-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.711354 mlpype-0.4.2/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.715354 mlpype-0.4.2/mlpype/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.715354 mlpype-0.4.2/mlpype/base/data/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/data/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/data/data_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/data/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.719354 mlpype-0.4.2/mlpype/base/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.723354 mlpype-0.4.2/mlpype/base/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/wheel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/wheel/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/wheel/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.723354 mlpype-0.4.2/mlpype/base/deploy/wheel/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/wheel/helpers/setup_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/wheel/helpers/wheel_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/deploy/wheel/wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.727354 mlpype-0.4.2/mlpype/base/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/evaluate/base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/evaluate/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.727354 mlpype-0.4.2/mlpype/base/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/experiment/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.731354 mlpype-0.4.2/mlpype/base/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/logger/experiment_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/logger/local_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.731354 mlpype-0.4.2/mlpype/base/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.735354 mlpype-0.4.2/mlpype/base/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/pipeline/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/pipeline/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/pipeline/type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.735354 mlpype-0.4.2/mlpype/base/serialiser/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/serialiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/serialiser/joblib_serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/serialiser/serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.739354 mlpype-0.4.2/mlpype/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/base/utils/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.739354 mlpype-0.4.2/mlpype/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.739354 mlpype-0.4.2/mlpype/fastapi/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/fastapi/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/fastapi/deploy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.739354 mlpype-0.4.2/mlpype/fastapi/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/fastapi/deploy/wheel/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/fastapi/deploy/wheel_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/fastapi/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.743354 mlpype-0.4.2/mlpype/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/hyperopt/optimise.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/hyperopt/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.743354 mlpype-0.4.2/mlpype/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/mlflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.743354 mlpype-0.4.2/mlpype/mlflow/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/mlflow/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/mlflow/deploy/load_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.743354 mlpype-0.4.2/mlpype/mlflow/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/mlflow/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/mlflow/logger/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/mlflow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.743354 mlpype-0.4.2/mlpype/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.751354 mlpype-0.4.2/mlpype/sklearn/data/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/data/data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/data/sklearn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/data/sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.755354 mlpype-0.4.2/mlpype/sklearn/model/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/model/linear_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/model/logistic_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/model/sklearn_base_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/model/sklearn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.755354 mlpype-0.4.2/mlpype/sklearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/pipeline/numpy_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/pipeline/pandas_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/sklearn/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.755354 mlpype-0.4.2/mlpype/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.759354 mlpype-0.4.2/mlpype/spark/data/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/data/spark_data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/data/spark_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/data/spark_sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.759354 mlpype-0.4.2/mlpype/spark/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/evaluate/spark_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.763354 mlpype-0.4.2/mlpype/spark/model/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/model/linear_spark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/model/spark_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.763354 mlpype-0.4.2/mlpype/spark/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/pipeline/spark_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/pipeline/spark_type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.763354 mlpype-0.4.2/mlpype/spark/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/serialisation/spark_serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/spark/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.767354 mlpype-0.4.2/mlpype/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.767354 mlpype-0.4.2/mlpype/tensorflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/data/tensor_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.771354 mlpype-0.4.2/mlpype/tensorflow/model/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/model/keras_pype_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/model/mlp_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/model/mlp_pype_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.771354 mlpype-0.4.2/mlpype/tensorflow/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/pipeline/tensor_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/tensorflow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.771354 mlpype-0.4.2/mlpype/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/xgboost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.775354 mlpype-0.4.2/mlpype/xgboost/model/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/xgboost/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/xgboost/model/xgboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/xgboost/model/xgboost_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 17:11:28.000000 mlpype-0.4.2/mlpype/xgboost/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:14:56.711354 mlpype-0.4.2/mlpype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-20 17:14:56.000000 mlpype-0.4.2/mlpype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 17:14:56.000000 mlpype-0.4.2/mlpype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:14:56.000000 mlpype-0.4.2/mlpype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 17:14:56.000000 mlpype-0.4.2/mlpype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-20 17:11:28.000000 mlpype-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 17:14:56.775354 mlpype-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-20 17:11:28.000000 mlpype-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.569264 mlpype-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 07:11:18.000000 mlpype-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 07:13:54.569264 mlpype-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-23 07:11:18.000000 mlpype-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.537263 mlpype-0.4.3/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.537263 mlpype-0.4.3/mlpype/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.541263 mlpype-0.4.3/mlpype/base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/data/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/data/data_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/data/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.541263 mlpype-0.4.3/mlpype/base/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.541263 mlpype-0.4.3/mlpype/base/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/wheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/wheel/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/wheel/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.541263 mlpype-0.4.3/mlpype/base/deploy/wheel/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/wheel/helpers/setup_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/wheel/helpers/wheel_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/deploy/wheel/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.545263 mlpype-0.4.3/mlpype/base/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/evaluate/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/evaluate/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.545263 mlpype-0.4.3/mlpype/base/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/experiment/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.545263 mlpype-0.4.3/mlpype/base/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/logger/experiment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/logger/local_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.545263 mlpype-0.4.3/mlpype/base/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.549263 mlpype-0.4.3/mlpype/base/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/pipeline/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/pipeline/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/pipeline/type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.549263 mlpype-0.4.3/mlpype/base/serialiser/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/serialiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/serialiser/joblib_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/serialiser/serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.549263 mlpype-0.4.3/mlpype/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/base/utils/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.549263 mlpype-0.4.3/mlpype/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.553264 mlpype-0.4.3/mlpype/fastapi/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/fastapi/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/fastapi/deploy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.553264 mlpype-0.4.3/mlpype/fastapi/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/fastapi/deploy/wheel/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/fastapi/deploy/wheel_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/fastapi/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.553264 mlpype-0.4.3/mlpype/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/hyperopt/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/hyperopt/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.553264 mlpype-0.4.3/mlpype/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/mlflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.553264 mlpype-0.4.3/mlpype/mlflow/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/mlflow/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/mlflow/deploy/load_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.553264 mlpype-0.4.3/mlpype/mlflow/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/mlflow/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/mlflow/logger/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/mlflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.553264 mlpype-0.4.3/mlpype/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.557263 mlpype-0.4.3/mlpype/sklearn/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/data/data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/data/sklearn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/data/sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.557263 mlpype-0.4.3/mlpype/sklearn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/model/linear_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/model/logistic_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/model/sklearn_base_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/model/sklearn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.557263 mlpype-0.4.3/mlpype/sklearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/pipeline/numpy_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/pipeline/pandas_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/sklearn/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.557263 mlpype-0.4.3/mlpype/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.561264 mlpype-0.4.3/mlpype/spark/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/data/spark_data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/data/spark_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/data/spark_sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.561264 mlpype-0.4.3/mlpype/spark/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/evaluate/spark_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.561264 mlpype-0.4.3/mlpype/spark/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/model/linear_spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/model/spark_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.561264 mlpype-0.4.3/mlpype/spark/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/pipeline/spark_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/pipeline/spark_type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.565264 mlpype-0.4.3/mlpype/spark/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/serialisation/spark_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/spark/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.565264 mlpype-0.4.3/mlpype/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.565264 mlpype-0.4.3/mlpype/tensorflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/data/tensor_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.565264 mlpype-0.4.3/mlpype/tensorflow/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/model/keras_pype_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/model/mlp_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/model/mlp_pype_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.565264 mlpype-0.4.3/mlpype/tensorflow/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/pipeline/tensor_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/tensorflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.565264 mlpype-0.4.3/mlpype/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/xgboost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.569264 mlpype-0.4.3/mlpype/xgboost/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/xgboost/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/xgboost/model/xgboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/xgboost/model/xgboost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 07:11:18.000000 mlpype-0.4.3/mlpype/xgboost/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:13:54.537263 mlpype-0.4.3/mlpype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-23 07:13:54.000000 mlpype-0.4.3/mlpype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-23 07:13:54.000000 mlpype-0.4.3/mlpype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:13:54.000000 mlpype-0.4.3/mlpype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 07:13:54.000000 mlpype-0.4.3/mlpype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-23 07:11:18.000000 mlpype-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-23 07:13:54.569264 mlpype-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 07:11:18.000000 mlpype-0.4.3/setup.py
```

### Comparing `mlpype-0.4.2/LICENSE.txt` & `mlpype-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/PKG-INFO` & `mlpype-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.2
+Version: 0.4.3
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.2/README.md` & `mlpype-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/data/data_catalog.py` & `mlpype-0.4.3/mlpype/base/data/data_catalog.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/data/dataset.py` & `mlpype-0.4.3/mlpype/base/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/deploy/inference.py` & `mlpype-0.4.3/mlpype/base/deploy/inference.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/deploy/wheel/builder.py` & `mlpype-0.4.3/mlpype/base/deploy/wheel/builder.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/deploy/wheel/extensions.py` & `mlpype-0.4.3/mlpype/base/deploy/wheel/extensions.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/deploy/wheel/helpers/setup_template.py` & `mlpype-0.4.3/mlpype/base/deploy/wheel/helpers/setup_template.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/deploy/wheel/wheel.py` & `mlpype-0.4.3/mlpype/base/deploy/wheel/wheel.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/evaluate/base_evaluator.py` & `mlpype-0.4.3/mlpype/base/evaluate/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/evaluate/evaluator.py` & `mlpype-0.4.3/mlpype/base/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/experiment/argument_parsing.py` & `mlpype-0.4.3/mlpype/base/experiment/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/experiment/experiment.py` & `mlpype-0.4.3/mlpype/base/experiment/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 import sys
 from argparse import ArgumentParser
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Type, Union
 
 from mlpype.base.constants import Constants
-from mlpype.base.data.data_catalog import DataCatalog
+from mlpype.base.data import DataCatalog, DataSet
 from mlpype.base.evaluate import BaseEvaluator
 from mlpype.base.experiment.argument_parsing import add_args_to_parser_for_pipeline
 from mlpype.base.logger import ExperimentLogger
 from mlpype.base.model import Model
 from mlpype.base.pipeline import Pipeline
 from mlpype.base.pipeline.type_checker import TypeCheckerPipe
 from mlpype.base.serialiser import JoblibSerialiser, Serialiser
 from mlpype.base.utils.parsing import get_args_for_prefix
 
 
 class Experiment:
     def __init__(
         self,
-        data_sources: Dict[str, DataCatalog],
+        data_sources: Dict[str, Union[DataCatalog, DataSet]],
         model: Model,
         pipeline: Pipeline,
         evaluator: BaseEvaluator,
         logger: ExperimentLogger,
         input_type_checker: TypeCheckerPipe,
         output_type_checker: TypeCheckerPipe,
         serialiser: Optional[Serialiser] = None,
@@ -38,16 +38,20 @@
 
         It is highly recommended to use one of the class methods to initialise this object:
             - from_dictionary: If you've already got your parameters in the right form:
                 - `model__<arg>` for model parameters
                 - `pipeline__<pipe_name>__<arg> for pipeline parameters.
 
         Args:
-            data_sources (Dict[str, DataCatalog]): The DataSets to use, in DataSource form.
-                Should contain at least a 'train' DataSet. These will be initialised in the beginning of the run.
+            data_sources (Dict[str, Dict[str, Union[DataCatalog, DataSet]]]): The
+                DataCatalog or DataSets to use, in DataSource form. Should contain at least a 'train' DataSet.
+                DataCatalogs will be initialised (`read`) in the beginning of the run. It is recommended to use
+                DataCatalog in distributed cases, but for quick experimentation DataSets tend to be more useful.
+                Please note that the DataSet will be changed by the Pipeline and Model. If you want to use a
+                DataSet, you should make sure you don't modify the original data by reference or by key.
             model (Model): The Model to fit.
             pipeline (Pipeline): The Pipeline to use to transform data before feeding it to the Model.
             evaluator (BaseEvaluator): The evaluator to test how good your Model performs.
             logger (ExperimentLogger): The experiment logger to make sure you record how well your experiment worked,
                 and log any artifacts such as the trained model.
             serialiser (Optional[Serialiser]): The serialiser to serialise any Python objects (expect the Model).
                 Defaults to a joblib serialiser.
@@ -97,15 +101,18 @@
         """Execute the experiment.
 
         Returns:
             Dict[str, Union[str, float, int, bool]]: The performance metrics of this run.
         """
         with self.experiment_logger:
             self.logger.info("Load data")
-            datasets = {name: data_source_set.read() for name, data_source_set in self.data_sources.items()}
+            datasets = {
+                name: data_source_set.read() if isinstance(data_source_set, DataCatalog) else data_source_set
+                for name, data_source_set in self.data_sources.items()
+            }
 
             self.logger.info("Create input type checker")
             self.input_type_checker.fit(datasets["train"])
             for ds in datasets.values():
                 self.input_type_checker.transform(ds)
 
             self.logger.info("Fit pipeline")
@@ -200,43 +207,49 @@
 
     def copy(self, parameters: Dict[str, Any], seed: int = 1) -> "Experiment":
         """Create a fresh copy of this Experiment.
 
         The Model & Pipeline will be recreated, so any trained versions will be
         re-initialised.
 
+        Old parameters will be kept, but overwritten if new values are provided.
+        This makes it easier to make templates for hyperparameter tuning.
+
         Args:
             parameters (Dict[str, Any]): New parameters for the Model and Pipeline
                 to be re-initialised with.
             seed (int, optional): Training seed. Defaults to 1.
 
         Returns:
-            Experiment: _description_
+            Experiment: A copy of this experiment, intialised with the new set
+                of parameters.
         """
+        new_params = self.parameters.copy()
+        new_params.update(parameters)
         model_class = self.model.__class__
 
-        model_args = get_args_for_prefix("model__", parameters)
+        model_args = get_args_for_prefix("model__", new_params)
         model = model_class(seed=seed, inputs=self.model.inputs, outputs=self.model.outputs, **model_args)
 
-        pipeline_args = get_args_for_prefix("pipeline__", parameters)
+        pipeline_args = get_args_for_prefix("pipeline__", new_params)
         new_pipeline = self.pipeline.copy(pipeline_args)
 
         return Experiment(
             # We might want to also deep copy data_sources, evaluator, type checkers, and experiment_logger.
             data_sources=self.data_sources,
             model=model,
             pipeline=new_pipeline,
             evaluator=self.evaluator,
             logger=self.experiment_logger,
             serialiser=self.serialiser,
             output_folder=self.output_folder,
             input_type_checker=self.input_type_checker,
             output_type_checker=self.output_type_checker,
             additional_files_to_store=self.additional_files_to_store,
-            parameters=parameters,
+            parameters=new_params,
         )
 
     @classmethod
     def from_dictionary(
         cls,
         data_sources: Dict[str, DataCatalog],
         model_class: Type[Model],
```

### Comparing `mlpype-0.4.2/mlpype/base/logger/experiment_logger.py` & `mlpype-0.4.3/mlpype/base/logger/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/logger/local_logger.py` & `mlpype-0.4.3/mlpype/base/logger/local_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/model/model.py` & `mlpype-0.4.3/mlpype/base/model/model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/pipeline/operator.py` & `mlpype-0.4.3/mlpype/base/pipeline/operator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/pipeline/pipe.py` & `mlpype-0.4.3/mlpype/base/pipeline/pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/pipeline/pipeline.py` & `mlpype-0.4.3/mlpype/base/pipeline/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+import logging
 from typing import Any, Dict, List, Optional, Union
 
 from mlpype.base.data import DataSet
 from mlpype.base.pipeline.pipe import Pipe
 from mlpype.base.utils.parsing import get_args_for_prefix
 
 
 class Pipeline:
     def __init__(self, pipes: List[Union[Pipe, "Pipeline"]]) -> None:
         """A pipeline of operations that can be re-applied to new, similar Data.
 
+        By default, we'll log at INFO level which step we're at in fit, transform,
+        and inverse_transform.
+
         Args:
             pipes (List[Union[Pipe, Pipeline]]): A list of either Pipes
                 or other Pipelines. These form the steps that should be applied.
         """
         self.pipes = pipes
         self._assert_all_names_different()
+        self.logger = logging.getLogger(__name__)
 
     def _assert_all_names_different(self, names: Optional[set] = None) -> None:
         if names is None:
             names = set()
 
         for pipe in self.pipes:
             if isinstance(pipe, Pipeline):
@@ -33,14 +38,16 @@
         Args:
             data (DataSet): The DataSet to use in fitting.
 
         Returns:
             Pipeline: This object.
         """
         for pipe in self.pipes:
+            if isinstance(pipe, Pipe):
+                self.logger.info(f"\tFitting step: `{pipe.name}`")
             pipe.fit(data)
             data = pipe.transform(data, is_inference=False)
         return self
 
     def transform(self, data: DataSet, is_inference: bool = False) -> DataSet:
         """Transforms the given data using this Pipeline.
 
@@ -52,14 +59,16 @@
                 mode for this transformation. We'll skip this step if
                 skip_on_inference was set to True.
 
         Returns:
             DataSet: The Transformed Data.
         """
         for pipe in self.pipes:
+            if isinstance(pipe, Pipe):
+                self.logger.info(f"\tTransforming step: `{pipe.name}`")
             data = pipe.transform(data, is_inference=is_inference)
         return data
 
     def inverse_transform(self, data: DataSet, is_inference: bool = False) -> DataSet:
         """Inverse transforms the DataSet using this Pipeline.
 
         Note that this is automatically done in reverse: the inverse steps
@@ -71,14 +80,16 @@
                 mode for this transformation. We'll skip this step if
                 skip_on_inference was set to True.
 
         Returns:
             DataSet: The inverse transformed DataSet
         """
         for pipe in reversed(self.pipes):
+            if isinstance(pipe, Pipe):
+                self.logger.info(f"\tInverse transforming step: `{pipe.name}`")
             data = pipe.inverse_transform(data, is_inference=is_inference)
         return data
 
     def reinitialise(self, args: Dict[str, Any]) -> None:
         """Re-initialises this Pipeline's Pipes using the given dictionary.
 
         Args:
@@ -108,18 +119,17 @@
         """
         result = Pipeline([])
         for pipe in self.pipes:
             if isinstance(pipe, Pipeline):
                 extra_pipeline = pipe.copy(args)
                 result += extra_pipeline
             else:
-                if args is None:
-                    pipe_args = {}
-                else:
-                    pipe_args = get_args_for_prefix(f"{pipe.name}__", args)
+                pipe_args = pipe.args.copy()
+                if args is not None:
+                    pipe_args.update(get_args_for_prefix(f"{pipe.name}__", args))
                 new_pipe = pipe.copy(pipe_args)
                 result += new_pipe
         return result
 
     def __iter__(self) -> "Pipeline":
         """Prepares this object for iteration using next().
```

### Comparing `mlpype-0.4.2/mlpype/base/pipeline/type_checker.py` & `mlpype-0.4.3/mlpype/base/pipeline/type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/serialiser/joblib_serialiser.py` & `mlpype-0.4.3/mlpype/base/serialiser/joblib_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/serialiser/serialiser.py` & `mlpype-0.4.3/mlpype/base/serialiser/serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/setup.py` & `mlpype-0.4.3/mlpype/base/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
     deps = [
         f"mlpype=={version}",
         "docstring_parser>=0.14.1",
         "pydantic>=1.9.1",
```

### Comparing `mlpype-0.4.2/mlpype/base/utils/parsing.py` & `mlpype-0.4.3/mlpype/base/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/base/utils/workspace.py` & `mlpype-0.4.3/mlpype/base/utils/workspace.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/fastapi/deploy/app.py` & `mlpype-0.4.3/mlpype/fastapi/deploy/app.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/fastapi/deploy/wheel/helpers.py` & `mlpype-0.4.3/mlpype/fastapi/deploy/wheel/helpers.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/fastapi/setup.py` & `mlpype-0.4.3/mlpype/fastapi/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

### Comparing `mlpype-0.4.2/mlpype/hyperopt/optimise.py` & `mlpype-0.4.3/mlpype/hyperopt/optimise.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/mlflow/deploy/load_experiment.py` & `mlpype-0.4.3/mlpype/mlflow/deploy/load_experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         experiment_name (str): The name of the experiment. Used to verify that the
             run_id is the correct one.
         run_id (str): The run id. Used to pull the actual experiment.
         directory (Optional[Union[Path, str]]): Optional directory to store the results
             in. By default, a temporary directory is used.
 
     Returns:
-        Inferencer: _description_
+        Inferencer: The Inferencer loaded from the trained model.
     """
     set_tracking_uri(url)
 
     # verify the run ID provided is part of the given experiment.
     exp_id = get_experiment_by_name(experiment_name)
     assert exp_id is not None, f"Experiment {experiment_name} does not exist in {url}."
     assert run_id in [
```

### Comparing `mlpype-0.4.2/mlpype/mlflow/logger/mlflow_logger.py` & `mlpype-0.4.3/mlpype/mlflow/logger/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/mlflow/setup.py` & `mlpype-0.4.3/mlpype/mlflow/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
 
     deps = [
         f"mlpype-base=={version}",
         "mlflow>=1.28.0, <2.0",
         "GitPython>=3.1.27",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
```

### Comparing `mlpype-0.4.2/mlpype/sklearn/data/data_frame_source.py` & `mlpype-0.4.3/mlpype/sklearn/data/data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/sklearn/data/sql_source.py` & `mlpype-0.4.3/mlpype/sklearn/data/sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/sklearn/model/sklearn_model.py` & `mlpype-0.4.3/mlpype/sklearn/model/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/sklearn/pipeline/numpy_type_checker.py` & `mlpype-0.4.3/mlpype/sklearn/pipeline/numpy_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/sklearn/pipeline/pandas_type_checker.py` & `mlpype-0.4.3/mlpype/sklearn/pipeline/pandas_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/sklearn/setup.py` & `mlpype-0.4.3/mlpype/sklearn/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
 
     deps = [
         f"mlpype-base=={version}",
         "numpy>=1.23.0",
         "scikit-learn>=1.1.1",
         "pandas>=1.4.3",
     ]
```

### Comparing `mlpype-0.4.2/mlpype/spark/data/spark_data_frame_source.py` & `mlpype-0.4.3/mlpype/spark/data/spark_data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/spark/data/spark_read.py` & `mlpype-0.4.3/mlpype/spark/data/spark_read.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/spark/data/spark_sql_source.py` & `mlpype-0.4.3/mlpype/spark/data/spark_sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/spark/evaluate/spark_evaluator.py` & `mlpype-0.4.3/mlpype/spark/evaluate/spark_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/spark/model/spark_model.py` & `mlpype-0.4.3/mlpype/spark/model/spark_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/spark/pipeline/spark_pipe.py` & `mlpype-0.4.3/mlpype/spark/pipeline/spark_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def __setstate__(self, state: Dict[str, Any]) -> None:
         """Sets the state of this object from a dictionary.
 
         Used by pickle to properly prepare the "fitted" and "operator" fields as None's.
 
         Args:
-            state (Dict[str, Any]): _description_
+            state (Dict[str, Any]): The set of parameters that this Pipe should be set to.
         """
         state["fitted"] = None
         state["operator"] = None
         self.__dict__ = state
 
     def __getstate__(self) -> Dict[str, Any]:
         """Gets the state of this object, excluding any Spark objects.
```

### Comparing `mlpype-0.4.2/mlpype/spark/pipeline/spark_type_checker.py` & `mlpype-0.4.3/mlpype/spark/pipeline/spark_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/spark/serialisation/spark_serialiser.py` & `mlpype-0.4.3/mlpype/spark/serialisation/spark_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/spark/setup.py` & `mlpype-0.4.3/mlpype/spark/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```

### Comparing `mlpype-0.4.2/mlpype/tensorflow/data/tensor_source.py` & `mlpype-0.4.3/mlpype/tensorflow/data/tensor_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/tensorflow/model/keras_pype_model.py` & `mlpype-0.4.3/mlpype/tensorflow/model/keras_pype_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/tensorflow/model/mlp_keras.py` & `mlpype-0.4.3/mlpype/tensorflow/model/mlp_keras.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/tensorflow/pipeline/tensor_checker.py` & `mlpype-0.4.3/mlpype/tensorflow/pipeline/tensor_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/tensorflow/setup.py` & `mlpype-0.4.3/mlpype/tensorflow/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
 
     deps = [
         f"mlpype-base=={version}",
         # on mac, it is recommended to use conda/mamba or source to install tensorflow
         "tensorflow>=2.12",
         "numpy>=1.23.0",
         "protobuf>=3.20.3",
```

### Comparing `mlpype-0.4.2/mlpype/xgboost/model/xgboost_classifier.py` & `mlpype-0.4.3/mlpype/xgboost/model/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype/xgboost/model/xgboost_regressor.py` & `mlpype-0.4.3/mlpype/xgboost/model/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/mlpype.egg-info/PKG-INFO` & `mlpype-0.4.3/mlpype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.2
+Version: 0.4.3
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.2/mlpype.egg-info/SOURCES.txt` & `mlpype-0.4.3/mlpype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.2/pyproject.toml` & `mlpype-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "mlpype"
 authors = [
     {name = "Jeroen van den Hoven"},
 ]
 description = "Standardise model training across libraries"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.4.2"
+version = "0.4.3"
 dynamic = ["license"]
 
 [tool.kedro]
 package_name = "data_cube_pipeline"
 project_name = "Data Cube Pipeline"
 project_version = "0.17.0"
```

