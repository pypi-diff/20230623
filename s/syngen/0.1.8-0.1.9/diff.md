# Comparing `tmp/syngen-0.1.8.tar.gz` & `tmp/syngen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.1.8.tar", last modified: Thu May 25 08:00:47 2023, max compression
+gzip compressed data, was "syngen-0.1.9.tar", last modified: Thu May 25 13:48:35 2023, max compression
```

## Comparing `syngen-0.1.8.tar` & `syngen-0.1.9.tar`

### file list

```diff
@@ -1,78 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.588250 syngen-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 07:58:47.000000 syngen-0.1.8/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-25 07:58:47.000000 syngen-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-25 07:58:47.000000 syngen-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-25 08:00:47.588250 syngen-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-05-25 07:58:47.000000 syngen-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-25 07:58:47.000000 syngen-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-25 08:00:47.588250 syngen-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.564250 syngen-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.572250 syngen-0.1.8/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.572250 syngen-0.1.8/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.572250 syngen-0.1.8/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.576250 syngen-0.1.8/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.576250 syngen-0.1.8/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.576250 syngen-0.1.8/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.576250 syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.568250 syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.576250 syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.580250 syngen-0.1.8/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43552 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.580250 syngen-0.1.8/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.580250 syngen-0.1.8/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6255 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33156 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.584250 syngen-0.1.8/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13244 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-05-25 07:58:47.000000 syngen-0.1.8/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:00:47.572250 syngen-0.1.8/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-25 08:00:47.000000 syngen-0.1.8/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-25 08:00:47.000000 syngen-0.1.8/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 08:00:47.000000 syngen-0.1.8/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-25 08:00:47.000000 syngen-0.1.8/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-25 08:00:47.000000 syngen-0.1.8/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-25 08:00:47.000000 syngen-0.1.8/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.556030 syngen-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 13:41:59.000000 syngen-0.1.9/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-25 13:41:59.000000 syngen-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-25 13:41:59.000000 syngen-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-25 13:48:35.556030 syngen-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-05-25 13:41:59.000000 syngen-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-25 13:41:59.000000 syngen-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-25 13:48:35.556030 syngen-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.544030 syngen-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/custom_logger/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/custom_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/custom_logger/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.544030 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43552 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6053 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33156 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.552030 syngen-0.1.9/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.556030 syngen-0.1.9/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.556030 syngen-0.1.9/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13244 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4681 2023-05-25 13:41:59.000000 syngen-0.1.9/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 13:48:35.548030 syngen-0.1.9/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    17434 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-25 13:48:35.000000 syngen-0.1.9/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.1.8/LICENSE` & `syngen-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/PKG-INFO` & `syngen-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.8
+Version: 0.1.9
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.8 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.9 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.8/README.md` & `syngen-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/setup.cfg` & `syngen-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/infer.py` & `syngen-0.1.9/src/syngen/infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import click
 from loguru import logger
 
 from syngen.ml.worker import Worker
-from syngen.ml.utils import setup_logger
+from syngen.ml.custom_logger import setup_logger
 
 
 @click.command()
 @click.option("--metadata_path", type=str, default=None, help="Path to the metadata file")
 @click.option("--size", default=100, type=click.IntRange(1),
               help="Desired number of rows to generate. If absent, it's defaulted to 100")
 @click.option("--table_name", default=None, type=str, help="Name of the table, same as in training")
```

### Comparing `syngen-0.1.8/src/syngen/ml/config/configurations.py` & `syngen-0.1.9/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/convertor/convertor.py` & `syngen-0.1.9/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.1.9/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/__init__.py` & `syngen-0.1.9/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.1.9/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.1.9/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.1.9/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/metrics/utils.py` & `syngen-0.1.9/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/reporters/reporters.py` & `syngen-0.1.9/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/strategies/strategies.py` & `syngen-0.1.9/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.1.9/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/utils/utils.py` & `syngen-0.1.9/src/syngen/ml/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,15 +202,7 @@
 
 def fetch_training_config(train_config_pickle_path):
     """
     Fetch the parameters of the training configuration
     """
     with open(train_config_pickle_path, "rb") as f:
         return pkl.load(f)
-
-def setup_logger(log_level: str):
-    """
-    Setup logger depending on the log level
-    :param log_level: the level of logging
-    """
-    logger.remove()
-    logger.add(sys.stdout, level=log_level)
```

### Comparing `syngen-0.1.8/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.1.9/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/vae/models/dataset.py` & `syngen-0.1.9/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/vae/models/features.py` & `syngen-0.1.9/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/vae/models/model.py` & `syngen-0.1.9/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.1.9/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.1.9/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/ml/worker/worker.py` & `syngen-0.1.9/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.8/src/syngen/train.py` & `syngen-0.1.9/src/syngen/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
 import click
 from loguru import logger
 
 from syngen.ml.worker import Worker
-from syngen.ml.utils import setup_logger
+from syngen.ml.custom_logger import setup_logger
 
 
 @click.command()
 @click.option("--metadata_path", type=str, default=None, help="Path to the metadata file")
 @click.option("--source", type=str, default=None, help="Path to the table that you want to use as a reference")
 @click.option("--table_name", type=str, default=None, help="Arbitrary string to name the directories")
 @click.option("--epochs", default=10, type=click.IntRange(1),
```

### Comparing `syngen-0.1.8/src/syngen.egg-info/PKG-INFO` & `syngen-0.1.9/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.8
+Version: 0.1.9
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.8 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.9 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.8/src/syngen.egg-info/SOURCES.txt` & `syngen-0.1.9/src/syngen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 src/syngen.egg-info/requires.txt
 src/syngen.egg-info/top_level.txt
 src/syngen/ml/__init__.py
 src/syngen/ml/config/__init__.py
 src/syngen/ml/config/configurations.py
 src/syngen/ml/convertor/__init__.py
 src/syngen/ml/convertor/convertor.py
+src/syngen/ml/custom_logger/__init__.py
+src/syngen/ml/custom_logger/custom_logger.py
 src/syngen/ml/data_loaders/__init__.py
 src/syngen/ml/data_loaders/data_loaders.py
 src/syngen/ml/metrics/__init__.py
 src/syngen/ml/metrics/utils.py
 src/syngen/ml/metrics/accuracy_test/__init__.py
 src/syngen/ml/metrics/accuracy_test/accuracy_report.html
 src/syngen/ml/metrics/accuracy_test/accuracy_test.py
```

