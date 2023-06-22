# Comparing `tmp/fiddler-client-2.0.0.dev3.tar.gz` & `tmp/fiddler-client-2.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-2.0.0.dev3.tar", last modified: Mon May  8 21:17:31 2023, max compression
+gzip compressed data, was "fiddler-client-2.0.0.dev5.tar", last modified: Fri Jun 16 00:06:47 2023, max compression
```

## Comparing `fiddler-client-2.0.0.dev3.tar` & `fiddler-client-2.0.0.dev5.tar`

### file list

```diff
@@ -1,97 +1,89 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    19268 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    15712 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)    30845 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11453 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/api/monitoring.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6393 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/aws_utils.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5098 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    21386 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/connection.py
--rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   128650 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16945 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/experimental.py
--rw-r--r--   0 runner    (1000) docker    (1001)    26153 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/fiddler_api.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5149 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7444 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/model_info_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    17870 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/monitoring_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/packtools/template_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/project.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4352 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3208 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)      775 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/logging.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4996 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/utils/pandas.py
--rw-r--r--   0 runner    (1000) docker    (1001)    18490 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v1_v2_compat.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/v2/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14039 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2063 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5923 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15065 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14721 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15444 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4472 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3105 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14627 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2664 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/api/project_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1203 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/constants.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.991416 fiddler-client-2.0.0.dev3/fiddler/v2/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4600 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      462 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3135 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/fiddler/v2/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1237 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4127 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2283 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2004 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/utils/validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/fiddler/v2/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1523 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/v2/validators/dataset_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13965 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/fiddler/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    19268 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     2260 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      212 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-05-08 21:17:30.000000 fiddler-client-2.0.0.dev3/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1395 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:30.995416 fiddler-client-2.0.0.dev3/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1757 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/tests/test_fiddler_api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3721 2023-05-08 21:17:25.000000 fiddler-client-2.0.0.dev3/tests/test_v1_v2_compat.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    19816 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    16156 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.650751 fiddler-client-2.0.0.dev5/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)     9468 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.650751 fiddler-client-2.0.0.dev5/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5105 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    21393 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/connection.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   128501 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2786 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    26077 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6446 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    17897 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/monitoring_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/packtools/template_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/project.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4370 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3213 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      782 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/logging.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5010 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/utils/pandas.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16048 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2140 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6602 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15923 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14948 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15328 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4502 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3066 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16988 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2937 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/api/project_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1241 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/constants.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4923 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      490 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3071 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3144 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2306 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1835 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/utils/validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler/v2/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1498 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/v2/validators/dataset_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13986 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/fiddler/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.654751 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    19816 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     2073 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      203 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-06-16 00:06:47.000000 fiddler-client-2.0.0.dev5/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1375 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:47.658751 fiddler-client-2.0.0.dev5/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/tests/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1787 2023-06-16 00:06:42.000000 fiddler-client-2.0.0.dev5/tests/test_fiddler_api.py
```

### Comparing `fiddler-client-2.0.0.dev3/PKG-INFO` & `fiddler-client-2.0.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev3
+Version: 2.0.0.dev5
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -18,15 +18,15 @@
         Installation
         ------------
         
             $ pip3 install fiddler-client
         
         API Example Usage
         -------------
-        Documentation for the API can be found [here](https://api.fiddler.ai/#introduction). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/quick-start/) as well as the work notebooks found on our [Samples Github](https://github.com/fiddler-labs/fiddler-samples).
+        Documentation for the API can be found [here](https://docs.fiddler.ai/reference/about-the-fiddler-client). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/docs/quick-start) as well as the notebooks found on our [Examples Github](https://github.com/fiddler-labs/fiddler-examples).
         
         Version History
         -------------
         
         ### 2.0.0
           - #### **Removed**
             - Following methods are removed
@@ -41,20 +41,33 @@
               - list_org_roles
               - unshare_project
               - share_project
               - process_avro
               - process_csv
           - #### **New Features**
             - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
-        
+            - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
         ### 1.8.0
           - #### **Modifications**
+            - Add new alert type -  `statistic` for setting alerts
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
         
+        ### 1.7.4
+          - #### **Modification**
+            - Do not typecast column with strings in get_slice()
+        
+        ### 1.7.3
+          - #### **Modification**
+            - Send row and column count information to dataset upload api
+        
+        ### 1.7.2
+          - #### **Modification**
+            - Bring back `WeightingParams` object
+        
         ### 1.7.1
           - #### **Modification**
             - Relaxed boto3 version constraint
         
         ### 1.7.0
           - #### **Removed**
             - Remove support for initializing fiddler client with version=1
```

### Comparing `fiddler-client-2.0.0.dev3/PUBLIC.md` & `fiddler-client-2.0.0.dev5/PUBLIC.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Installation
 ------------
 
     $ pip3 install fiddler-client
 
 API Example Usage
 -------------
-Documentation for the API can be found [here](https://api.fiddler.ai/#introduction). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/quick-start/) as well as the work notebooks found on our [Samples Github](https://github.com/fiddler-labs/fiddler-samples).
+Documentation for the API can be found [here](https://docs.fiddler.ai/reference/about-the-fiddler-client). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/docs/quick-start) as well as the notebooks found on our [Examples Github](https://github.com/fiddler-labs/fiddler-examples).
 
 Version History
 -------------
 
 ### 2.0.0
   - #### **Removed**
     - Following methods are removed
@@ -34,20 +34,33 @@
       - list_org_roles
       - unshare_project
       - share_project
       - process_avro
       - process_csv
   - #### **New Features**
     - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
-
+    - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
 ### 1.8.0
   - #### **Modifications**
+    - Add new alert type -  `statistic` for setting alerts
     - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
       `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
 
+### 1.7.4
+  - #### **Modification**
+    - Do not typecast column with strings in get_slice()
+
+### 1.7.3
+  - #### **Modification**
+    - Send row and column count information to dataset upload api
+
+### 1.7.2
+  - #### **Modification**
+    - Bring back `WeightingParams` object
+
 ### 1.7.1
   - #### **Modification**
     - Relaxed boto3 version constraint
 
 ### 1.7.0
   - #### **Removed**
     - Remove support for initializing fiddler client with version=1
```

### Comparing `fiddler-client-2.0.0.dev3/README.md` & `fiddler-client-2.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/assets/pg_reserved_words.py` & `fiddler-client-2.0.0.dev5/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/client.py` & `fiddler-client-2.0.0.dev5/fiddler/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import absolute_import
 
 import json
 from collections import namedtuple
 
 import requests
 
-from .utils.exceptions import FiddlerException
+from fiddler.utils.exceptions import FiddlerException
 
 API_BASE_URL = 'https://dev.fiddler.ai'
 
 
 # A PredictionEventBundle represents a batch of inferences and their input
 # features. All of these share schema, latency, and success status. A bundle
 # can consist just one event as well.
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/connection.py` & `fiddler-client-2.0.0.dev5/fiddler/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from fiddler.v2.constants import FIDDLER_CLIENT_VERSION_HEADER
 
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json import JSONDecodeError
 
-from .utils.exceptions import JSONException, ResourceNotFound
+from fiddler.utils.exceptions import JSONException, ResourceNotFound
 
 LOG = logging.getLogger(__name__)
 
 SIMPLE_RES_API = ['slice_query', 'parse_slice_query']
 
 
 class Connection:
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/core_objects.py` & `fiddler-client-2.0.0.dev5/fiddler/core_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import enum
 import functools
 import json
 import logging
 import textwrap
 import warnings
 from dataclasses import asdict, dataclass
-from pathlib import Path
 from typing import (
     Any,
     Dict,
     Iterable,
     List,
     NamedTuple,
     Optional,
@@ -21,25 +20,20 @@
     Union,
     cast,
 )
 
 import numpy as np
 import pandas as pd
 import pandas.api.types
-from deprecated import deprecated
 
-from ._version import __version__
-from .utils.exceptions import MalformedSchemaException
-from .utils.formatting import prettyprint_number, validate_sanitized_names
-from .utils.general_checks import (
-    is_greater_than_max_value,
-    is_less_than_min_value,
-    type_enforce,
-)
-from .utils.pandas import is_datetime
+from fiddler._version import __version__
+from fiddler.utils.exceptions import MalformedSchemaException
+from fiddler.utils.formatting import prettyprint_number, validate_sanitized_names
+from fiddler.utils.general_checks import type_enforce
+from fiddler.utils.pandas import is_datetime
 
 MAX_VECTOR_DIMENSION = 1024
 MAX_NUMBER_OF_CLUSTERS = 100
 MAX_NUMBER_OF_CUSTOM_FEATURES = 100
 DEFAULT_MAX_INFERRED_CARDINALITY = 100
 
 # default for DatasetInfo.data_type_version and ModelInfo.data_type_version
@@ -70,32 +64,14 @@
 
     def __init__(self, _type, desc):
         self.type = _type
         self.desc = desc
 
 
 @enum.unique
-class InitMonitoringModifications(enum.Enum):
-    """various checks to perform for init_monitoring. Used to specify to the
-    Fiddler `init_monitoring` endpoint whether or not modify (write) access
-    is being given. See FNG-1152 for more details"""
-
-    # only support monitoring int, float, category, or boolean types
-    MODEL_INFO__COLUMN_TYPE = 'model_info::column_type'
-    # ensure that model_info has min-max for all numeric types, and possible-values for all categorical types
-    MODEL_INFO__BIN_CONFIG = 'model_info::bin_config'
-
-
-possible_init_monitoring_modifications = (
-    InitMonitoringModifications.MODEL_INFO__COLUMN_TYPE,
-    InitMonitoringModifications.MODEL_INFO__BIN_CONFIG,
-)
-
-
-@enum.unique
 class MonitoringViolationType(enum.Enum):
     """Fatal violations would cause monitoring to not work whereas warning violation
     can cause one or more monitoring features to not work.
     """
 
     FATAL = 'fatal'
     WARNING = 'warning'
@@ -178,14 +154,15 @@
 
     FLOAT = 'float'
     INTEGER = 'int'
     BOOLEAN = 'bool'
     STRING = 'str'
     CATEGORY = 'category'
     TIMESTAMP = 'timestamp'
+    EMBEDDINGS = 'embeddings'
 
     def is_numeric(self):
         return self.value in (DataType.INTEGER.value, DataType.FLOAT.value)
 
     def is_bool_or_cat(self):
         return self.value in (DataType.BOOLEAN.value, DataType.CATEGORY.value)
 
@@ -423,15 +400,15 @@
 
     @classmethod
     def from_columns(
         cls,
         cols: List[str],
         custom_name: str,
         transformation: Optional[str] = None,
-        n_clusters: Optional[int] = None,
+        n_clusters: Optional[int] = 10,
         monitor: bool = True,
         monitor_components: bool = False,
     ):
         """Creates a custom feature from multiple numerical columns.
         :param cols: A list of column names that define this custom feature.
         :param custom_name: The name of this custom feature as it will appear in the monitoring tab.
         :param transformation: [Optional] An optional transformation step (eg, dimensionality reduction via SVD).
@@ -612,15 +589,14 @@
             res['is-nullable'] = self.is_nullable
         if self.value_range_min is not None:
             res['value-range-min'] = self.value_range_min
         if self.value_range_max is not None:
             res['value-range-max'] = self.value_range_max
         return res
 
-
     @staticmethod
     def _value_is_na_or_none(value):
         if value is None:
             return True
         # This needs to be added because when we add `pandas._libs.missing.NAType` type in rabbitmq.
         # When we read the message, it converts the value to the "<NA>".
         if isinstance(value, str):
@@ -765,14 +741,16 @@
             return DataType.FLOAT
         if pd.api.types.is_integer_dtype(pd_dtype):
             return DataType.INTEGER
         if pd.api.types.is_bool_dtype(pd_dtype):
             return DataType.BOOLEAN
         if pd.api.types.is_categorical_dtype(pd_dtype):
             return DataType.CATEGORY
+        if pd_dtype == 'ndarray':
+            return DataType.EMBEDDINGS
 
         return DataType.STRING
 
     @classmethod
     def update_stats_for_existing_schema(
         cls, dataset: dict, info, max_inferred_cardinality: Optional[int] = None
     ):
@@ -880,47 +858,54 @@
             df = df.reset_index(inplace=False)
         name_series_iter = df.items()
         for column_name, column_series in name_series_iter:
             column_info = cls._calculate_stats_for_col(
                 column_name,
                 column_series,
                 max_inferred_cardinality,
-                data_type_version=CURRENT_DATA_TYPE_VERSION
+                data_type_version=CURRENT_DATA_TYPE_VERSION,
             )
             columns.append(column_info)
         return cls(
             display_name,
             columns,
             dataset_id=dataset_id,
             data_type_version=CURRENT_DATA_TYPE_VERSION,
         )
 
     @staticmethod
     def _calculate_stats_for_col(
         column_name,
         column_series,
         max_inferred_cardinality,
-        data_type_version:Optional[str]='v0'):
+        data_type_version: Optional[str] = 'v0',
+    ):
         # @TODO Automatically drop the empty column with warning and proceed instead of aborting the upload
         if column_series.isna().all():
             raise ValueError(
                 f'Column {column_name} is empty. '
                 f'Please remove it and re-upload the dataset.'
             )
 
         # if we infer string or categorical, ensure that the underlying data
         # is also string by casting it.
 
         # FDL-10905: dropna is needed to take care of cases where having None changes
         # data type of int, float, bool to category. dropna() won't change
         # is_nullable detection as column_series.dropna() returns a new instance.
         column_series_dropped_na = column_series.dropna()
-        column_dtype = DatasetInfo.datatype_from_pandas_dtype(
-            column_series_dropped_na.infer_objects().dtype
-        )
+        pd_column_dtype = column_series_dropped_na.infer_objects().dtype
+        if pd_column_dtype == 'object':
+            column_count = column_series_dropped_na.shape[0]
+            for i in range(column_count):
+                if isinstance(column_series_dropped_na[i], np.ndarray):
+                    pd_column_dtype = 'ndarray'
+                    break
+
+        column_dtype = DatasetInfo.datatype_from_pandas_dtype(pd_column_dtype)
         # get nullability before any datatype modifications like 'astype'
         # which distorts None values.
         is_nullable = bool(column_series.isna().any())
 
         if column_dtype in [DataType.CATEGORY, DataType.STRING]:
             if 'mixed' in pd.api.types.infer_dtype(column_series):
                 LOG.warning(
@@ -940,15 +925,17 @@
             column_dtype = DataType.CATEGORY
 
         # get possible values for categorical type
         if column_dtype.is_bool_or_cat():
             # Only when data_type_version is 'v0',
             # categorical column values undergo int/bool -> float -> string conversion.
             if data_type_version == 'v0':
-                possible_values = np.sort(column_series_dropped_na.astype(str).unique()).tolist()
+                possible_values = np.sort(
+                    column_series_dropped_na.astype(str).unique()
+                ).tolist()
                 possible_values_floats = None
                 if column_dtype.value == DataType.CATEGORY.value:
                     try:
                         possible_values_floats = [
                             str(float(raw_val)) for raw_val in possible_values
                         ]
                     except ValueError:
@@ -1258,15 +1245,16 @@
         self.data_type_version = data_type_version
 
         self.is_binary_ranking_model = is_binary_ranking_model
 
         self._validate_columns()
 
         self.target_class_order = self.get_target_class_order(
-            self.target_class_order, self.model_task, self.targets[0])
+            self.target_class_order, self.model_task, self.targets[0]
+        )
 
         if model_task == ModelTask.RANKING:
             if group_by is None:
                 raise ValueError(
                     'The argument group_by cannot be empty for Ranking models'
                 )
             self.is_binary_ranking_model = len(self.target_class_order) == 2
@@ -1360,23 +1348,28 @@
                 )
             if len(self.custom_features) > MAX_NUMBER_OF_CUSTOM_FEATURES:
                 raise ValueError(
                     f'The maximum number of custom features in a project cannot exceed {MAX_NUMBER_OF_CUSTOM_FEATURES}. {len(self.custom_features)} custom features are defined.'
                 )
 
             available_cols = (
-                self.get_input_names() + self.get_target_names() + self.get_metadata_names()
+                self.get_input_names()
+                + self.get_target_names()
+                + self.get_metadata_names()
             )
             numeric_cols = self.get_input_pandas_dtypes()
             if self.metadata:
                 numeric_cols.update(self.get_metadata_pandas_dtypes())
             if self.targets:
                 numeric_cols.update(self.get_target_pandas_dtypes())
-            valid_col_names = [k for k, v in numeric_cols.items() if
-                               v in (DataType.INTEGER.value, DataType.FLOAT.value)]
+            valid_col_names = [
+                k
+                for k, v in numeric_cols.items()
+                if v in (DataType.INTEGER.value, DataType.FLOAT.value)
+            ]
 
             unique_cf_names = []
             for feature in self.custom_features:
 
                 if not isinstance(feature, CustomFeature):
                     raise ValueError(
                         'The custom_features argument only accepts a list of CustomFeature objects.'
@@ -1417,15 +1410,15 @@
         res = {
             'name': self.display_name,
             'input-type': self.input_type.value,
             'model-task': self.model_task.value,
             'inputs': [c.to_dict() for c in self.inputs],
             'outputs': [c.to_dict() for c in self.outputs],
             'datasets': self.datasets or [],
-            'targets': [target_col.to_dict() for target_col in self.targets]
+            'targets': [target_col.to_dict() for target_col in self.targets],
         }
         if self.target_class_order is not None:
             res['target-class-order'] = self.target_class_order
         if self.metadata:
             res['metadata'] = [metadata_col.to_dict() for metadata_col in self.metadata]
         if self.decisions:
             res['decisions'] = [
@@ -2299,15 +2292,14 @@
             return None
 
         output_columns = []
         ds_info_names_columns = {}
         for ds_column in dataset_info.columns:
             ds_info_names_columns[ds_column.name] = ds_column
 
-
         if model_task.is_classification():
             if isinstance(output_names, dict):
                 output_names = list(output_names.keys())
             for name in output_names:
                 if name in ds_info_names_columns:
                     output_columns.append(ds_info_names_columns[name])
                 else:
@@ -2329,15 +2321,18 @@
                     raise ValueError(
                         f'If outputs is a dictionary, the values should '
                         f'be a tuple of 2 values. Currently passing: '
                         f'{values} for output {name}. Please correct.'
                     )
                 if name in ds_info_names_columns:
                     column = ds_info_names_columns[name]
-                    if not (column.data_type == DataType.FLOAT or column.data_type == DataType.INTEGER):
+                    if not (
+                        column.data_type == DataType.FLOAT
+                        or column.data_type == DataType.INTEGER
+                    ):
                         raise ValueError(
                             f'Column {name} with type {column.data_type} can not be specified as output.'
                             f'Output column type has to be either INTEGER or FLOAT.'
                             f'Please correct.'
                         )
                     column.value_range_min = min(values)
                     column.value_range_max = max(values)
@@ -2363,15 +2358,18 @@
                         col = target_column.name
                     else:
                         raise ValueError(
                             f'Output {name} is not present in the dataset. '
                             f'Please provide a dictionary with the range: '
                             f'{name}: (min_value, max_value).'
                         )
-                if dataset_info[col].value_range_min is None or dataset_info[col].value_range_max is None:
+                if (
+                    dataset_info[col].value_range_min is None
+                    or dataset_info[col].value_range_max is None
+                ):
                     raise ValueError(
                         f'Column {name} with value_range_min or value_range_max as None can not be specified as output.'
                         f'Please correct.'
                     )
                 output_columns.append(
                     Column(
                         name=name,
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/dataset.py` & `fiddler-client-2.0.0.dev5/fiddler/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/fiddler_api.py` & `fiddler-client-2.0.0.dev5/fiddler/fiddler_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 from collections import namedtuple
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
 from deprecated import deprecated
 
+from fiddler import constants
 from fiddler.connection import Connection
-from fiddler.experimental import ExperimentalFeatures
-from fiddler.project import Project
-from fiddler.utils import logging
-
-from . import constants
-from .core_objects import (
+from fiddler.core_objects import (
     DatasetInfo,
     FiddlerTimestamp,
     ModelInfo,
     MonitoringViolation,
     MonitoringViolationType,
 )
-from .monitoring_validator import MonitoringValidator
-from .utils import cast_input_data
-from .utils.general_checks import do_not_proceed, safe_name_check, type_enforce
-from .utils.pandas import df_size_exceeds
+from fiddler.monitoring_validator import MonitoringValidator
+from fiddler.project import Project
+from fiddler.utils import cast_input_data
+from fiddler.utils import logging
+from fiddler.utils.general_checks import do_not_proceed, safe_name_check, type_enforce
+from fiddler.utils.pandas import df_size_exceeds
 
 LOG = logging.getLogger(__name__)
 
 SUCCESS_STATUS = Connection.SUCCESS_STATUS
 FAILURE_STATUS = Connection.FAILURE_STATUS
 FIDDLER_ARGS_KEY = Connection.FIDDLER_ARGS_KEY
 STREAMING_HEADER_KEY = Connection.STREAMING_HEADER_KEY
@@ -103,15 +101,14 @@
         self.org_id = org_id
         self.strict_mode = True
         self.connection = Connection(
             url, org_id, auth_token, proxies, verbose, timeout, verify=verify
         )
 
         self.monitoring_validator = MonitoringValidator()
-        self.experimental = ExperimentalFeatures(client=self)
 
     def __getattr__(self, function_name):
         """
         Overriding allows us to point unrecognized use cases to the documentation page
         """
 
         def method(*args, **kwargs):
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/model.py` & `fiddler-client-2.0.0.dev5/fiddler/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/monitoring_validator.py` & `fiddler-client-2.0.0.dev5/fiddler/monitoring_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
 from typing import List
 
-from . import constants
-from .core_objects import (
+from fiddler import constants
+from fiddler.core_objects import (
     DataType,
     EventTypes,
     FiddlerEventColumns,
     ModelInputType,
     ModelTask,
     MonitoringViolation,
     MonitoringViolationType,
 )
-from .utils.formatting import formatted_utcnow, pad_timestamp
-from .utils.general_checks import is_int_type
+from fiddler.utils.formatting import formatted_utcnow, pad_timestamp
+from fiddler.utils.general_checks import is_int_type
 
 
 class MonitoringValidator:
     def __init__(self):
         pass
 
     def pre_flight_monitoring_check(
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/packtools/gem.py` & `fiddler-client-2.0.0.dev5/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-2.0.0.dev5/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-2.0.0.dev5/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/packtools/template_model.py` & `fiddler-client-2.0.0.dev5/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/project.py` & `fiddler-client-2.0.0.dev5/fiddler/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/utils/__init__.py` & `fiddler-client-2.0.0.dev5/fiddler/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
 import logging
-from typing import Dict, List
+from typing import List
 
 import pandas as pd
 
-from .. import constants
-from ..core_objects import Column, DatasetInfo, DataType, ModelInfo
-from .pandas import is_datetime, try_series_retype
+from fiddler import constants
+from fiddler.core_objects import Column, DatasetInfo, DataType, ModelInfo
+from fiddler.utils.pandas import is_datetime, try_series_retype
 
 LOG = logging.getLogger(__name__)
 pd.set_option('mode.chained_assignment', None)
 
 
 def df_from_json_rows(
     dataset_rows_json: List[dict],
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/utils/exceptions.py` & `fiddler-client-2.0.0.dev5/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/utils/formatting.py` & `fiddler-client-2.0.0.dev5/fiddler/utils/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import sys
 from datetime import datetime
 
-from .. import constants
+from fiddler import constants
 
 
 def prettyprint_number(number, n_significant_figures=4):
     n_digits = len(f'{number:.0f}')
     return f'{round(number, n_significant_figures - n_digits):,}'
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/utils/general_checks.py` & `fiddler-client-2.0.0.dev5/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/utils/helper.py` & `fiddler-client-2.0.0.dev5/fiddler/utils/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from typing import Union
+
 import pandas as pd
 
-from ..core_objects import BatchPublishType
+from fiddler.core_objects import BatchPublishType
 
 
 def infer_data_source(source: Union[str, pd.DataFrame]):
     """
     Attempts to infer the type of object based on type
     """
     if isinstance(source, pd.DataFrame):
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/utils/pandas.py` & `fiddler-client-2.0.0.dev5/fiddler/utils/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from datetime import datetime
 from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-from .. import constants
+from fiddler import constants
 
 LOG = logging.getLogger(__name__)
 TIMESTAMP = 'TIMESTAMP'
 
 
 def is_datetime(pandas_series):
     """
@@ -55,15 +55,15 @@
                     df[col], format=constants.TIMESTAMP_FORMAT, utc=True
                 ).dt.tz_localize(None)
                 df[col] = df[col].astype('string')
     return df
 
 
 def try_series_retype(series: pd.Series, new_type) -> Union[pd.DataFrame, pd.Series]:
-    if new_type == 'unknown':
+    if new_type in ['unknown', 'str']:
         # Do not retype data
         return series
 
     try:
         return series.astype(new_type)
     except (TypeError, ValueError) as e:
         if new_type == 'int':
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v1_v2_compat.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/model_mixin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,448 +1,496 @@
+import os
+import shutil
+import tempfile
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
 
-import pandas as pd
-import yaml
+from pydantic import parse_obj_as
 
-from fiddler.core_objects import (
-    BatchPublishType,
-    Column,
-    DatasetInfo,
-    FiddlerTimestamp,
-    ModelInfo,
-)
+from fiddler import ModelInfo
+from fiddler.core_objects import BaselineType
+from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
-from fiddler.v2.api.api import Client
-from fiddler.v2.constants import FiddlerTimestamp as V2FiddlerTimestamp
-from fiddler.v2.constants import FileType
-from fiddler.v2.schema.dataset import Dataset
-
-DATASET_MAX_ROWS = 50_000
-
+from fiddler.v2.api.baseline_mixin import BaselineMixin
+from fiddler.v2.api.model_artifact_deploy import (
+    ModelArtifactDeployer,
+    MultiPartModelArtifactDeployer,
+)
+from fiddler.v2.constants import MULTI_PART_CHUNK_SIZE
+from fiddler.v2.schema.model import Model
+from fiddler.v2.schema.model_deployment import ArtifactType, DeploymentParams
+from fiddler.v2.utils.decorators import check_version, handle_api_error_response
+from fiddler.v2.utils.helpers import get_model_artifact_info, read_model_yaml
+from fiddler.v2.utils.response_handler import (
+    APIResponseHandler,
+    PaginatedResponseHandler,
+)
+from fiddler.v2.utils.validations import validate_artifact_dir
 
 logger = logging.getLogger(__name__)
 
 
-class V1V2Compat:
-    def __init__(self, client_v2: Client):
-        self.client_v2 = client_v2
+class ModelMixin:
+    ADD_SURROGATE_MODEL_API_VERSION = '>=22.12.0'
+    ADD_MODEL_ARTIFACT_API_VERSION = '>=22.12.0'
+    DELETE_MODEL_API_VERSION = '>=22.12.0'
+
+    client: RequestClient
+    organization_name: str
+
+    @handle_api_error_response
+    def get_models(self, project_name: str) -> List[Model]:
+        """
+        Get list of all models belonging to a project
+
+        :params project_name: The project for which you want to get the models
+        :returns: List containing Model objects
+        """
+        response = self.client.get(
+            url='models',
+            params={
+                'organization_name': self.organization_name,
+                'project_name': project_name,
+            },
+        )
+        items = PaginatedResponseHandler(response).get_pagination_items()
+        return parse_obj_as(List[Model], items)
 
-    # Projects
-    def get_projects(self, get_project_details: bool = False) -> List[str]:
-        """List the ids of all projects in the organization.
+    @handle_api_error_response
+    def get_model_names(self, project_name: str) -> List[str]:
+        """List the ids of all models in the project.
 
-        :param get_project_details: Unused argument to maintain compatibility
-        :returns: List of strings containing the ids of each project.
+        :param project_name: The unique identifier of the project on Fiddler
+        :returns: List of strings containing the ids of each model.
         """
-        projects = self.client_v2.get_projects()
-        return [p.name for p in projects]
-
-    def add_project(self, project_id: str) -> Dict[str, str]:
-        """Create a new project.
+        models = self.get_models(project_name=project_name)
+        return [m.name for m in models]
 
-        :param project_id: The unique identifier of the model's project on the
-            Fiddler engine. Must be a short string without whitespace.
+    @handle_api_error_response
+    def get_model(self, project_name: str, model_name: str) -> Model:
+        """
+        Get the details of a model.
 
-        :returns: Server response for creation action.
+        :params project_name: The project to which the model belongs to
+        :params model_name: The model name of which you need the details
+        :returns: Model object which contains the details
         """
-        project = self.client_v2.add_project(project_name=project_id)
-        return {'project_name': project.name}
+        response = self.client.get(
+            url=f'models/{self.organization_name}:{project_name}:{model_name}',
+        )
+        response_handler = APIResponseHandler(response)
+        return Model.deserialize(response_handler)
 
-    def delete_project(self, project_id: str) -> None:
-        """Permanently delete a project.
+    def get_model_info(self, project_name: str, model_name: str) -> ModelInfo:
+        """Get ModelInfo for a model.
 
-        :param project_id: The unique identifier of the project on the Fiddler
-            engine.
+        :params project_name: The project to which the model belongs to
+        :params model_name: The model name of which you need the details
 
-        :returns: None
+        :returns: A fiddler.ModelInfo object describing the model.
         """
-        self.client_v2.delete_project(project_name=project_id)
+        model_info_dict = self.get_model(
+            project_name=project_name, model_name=model_name
+        ).info
+        return ModelInfo.from_dict(model_info_dict)
 
-    # Datasets
-    def get_datasets(self, project_id: str) -> List[str]:
-        """List the ids of all datasets in the organization.
+    @handle_api_error_response
+    def _add_model_call(
+        self, project_name: str, model_name: str, info: ModelInfo
+    ) -> Model:
+        """
+        Function to add a model to fiddler for monitoring
+
+        :param project_name: project name where the model will be added
+        :type project_name: string
+        :param model_name: name of the model
+        :type model_name: string
+        :param info: model related information
+        :type info: ModelInfo
+
+        :return: Model object which contains the model details
+        """
+        if not isinstance(info, ModelInfo):
+            raise ValueError(
+                f'The value passed to the info parameter must be a ModelInfo object.'
+                f'Instead, found value of type {type(info)}'
+            )
 
-        :param project_id: The unique identifier of the project on Fiddler
-        :returns: List of strings containing the ids of each dataset.
-        """
-        datasets = self.client_v2.get_datasets(project_name=project_id)
-        return [d.name for d in datasets]
+        request_body = {
+            'name': model_name,
+            'project_name': project_name,
+            'organization_name': self.organization_name,
+            'info': info.to_dict(),
+            'model_type': None,
+            'file_list': None,
+        }
+
+        response = self.client.post(
+            url='models',
+            data=request_body,
+        )
+        logger.info('Model %s added to %s project', model_name, project_name)
 
-    def get_dataset_artifact(
+        return Model.deserialize(APIResponseHandler(response))
+
+    def add_model(
         self,
-        project_id: str,
-        dataset_id: str,
-        max_rows: int = 1_000,
-        splits: Optional[List[str]] = None,
-        sampling=False,
-        dataset_info: Optional[DatasetInfo] = None,
-        include_fiddler_id=False,
-    ) -> Dict[str, pd.DataFrame]:
-        raise NotImplementedError('This method is currently not implemented')
-
-    def get_dataset(self, project_id: str, dataset_id: str) -> Dataset:
-        dataset = self.client_v2.get_dataset(
-            project_name=project_id, dataset_name=dataset_id
-        )
-        return dataset  # @todo: Make the response compatible with dataset info
-
-    def get_dataset_info(self, project_id: str, dataset_id: str) -> DatasetInfo:
-        """Get DatasetInfo for a dataset.
-
-        :param project_id: The unique identifier of the project on Fiddler
-        :param dataset_id: The unique identifier of the dataset on the Fiddler
-            engine.
-
-        :returns: A fiddler.DatasetInfo object describing the dataset.
-        """
-        dataset = self.get_dataset(project_id, dataset_id)
-        return dataset.info
-
-    def delete_dataset(self, project_id: str, dataset_id: str) -> None:
-        """Permanently delete a dataset.
-
-        :param project_id: The unique identifier of the project on the Fiddler
-            engine.
-        :param dataset_id: The unique identifier of the dataset on the Fiddler
-            engine.
+        project_name: str,
+        model_name: str,
+        dataset_name: str,
+        model_info: ModelInfo,
+    ) -> None:
+        """
+        Function to add a model to fiddler for monitoring
 
-        :returns: None
+        :param project_name: project name where the model will be added
+        :param model_name: name of the model
+        :param dataset_name: name of the dataset
+        :param model_info: model related information from user
         """
-        # @todo: FDL-5366
-        # check that on the server side
-        # 1. Delete the table in CH
-        # 2. Delete the files from blob store
-        # 3. Delete the entry from postgres table
-        self.client_v2.delete_dataset(project_name=project_id, dataset_name=dataset_id)
 
-    # Model
-    def get_models(self, project_id: str) -> List[str]:
-        """List the ids of all models in the project.
+        if not isinstance(model_info, ModelInfo):
+            raise ValueError(
+                f'The value passed to the model_info parameter must be a ModelInfo '
+                f'object. Instead, found value of type {type(model_info)}'
+            )
 
-        :param project_id: The unique identifier of the project on Fiddler
-        :returns: List of strings containing the ids of each model.
-        """
-        models = self.client_v2.get_models(project_name=project_id)
-        return [m.name for m in models]
+        # associate dataset_id with model_info. This was not done during
+        # from_dataset_info call.
+        model_info.datasets = [dataset_name]
+
+        model = self.add_model_call(
+            model_name=model_name,
+            project_name=project_name,
+            info=model_info,
+        )
+        BaselineMixin.add_baseline(
+            project_name=project_name,
+            model_name=model_name,
+            baseline_name='DEFAULT',
+            type=BaselineType.PRE_PRODUCTION,
+            run_async=True,
+            wait=True,
+        )
+        logger.info(f'Successfully added model {model.name} to project {project_name}')
 
-    def get_model_info(self, project_id: str, model_id: str) -> ModelInfo:
-        """Get ModelInfo for a model.
+    @handle_api_error_response
+    def update_model(
+        self,
+        model_name: str,
+        project_name: str,
+        info: Optional[ModelInfo] = None,
+        file_list: Optional[List[Dict[str, Any]]] = None,
+        framework: Optional[str] = None,
+        requirements: Optional[str] = None,
+    ) -> Model:
+        """
+        Update model metadata like model info, file
+
+        :param project_name: project name where the model will be added
+        :type project_name: string
+        :param model_name: name of the model
+        :type model_name: string
+        :param info: model related information passed as dictionary from user
+        :type info: ModelInfo object
+        :param file_list: Artifact file list
+        :type info: List of dictionaries
+        :param framework: Model framework name
+        :type framework: string
+        :param requirements: Requirements
+        :type requirements: string
+        :return: Model object which contains the model details
+        """
+        body = {}
+
+        if info:
+            body['info'] = info.to_dict()
+
+        if file_list:
+            body['file_list'] = file_list
+
+        if framework:
+            body['framework'] = framework
+
+        if requirements:
+            body['requirements'] = requirements
+
+        response = self.client.patch(
+            url=f'models/{self.organization_name}:{project_name}:{model_name}',
+            data=body,
+        )
+        logger.info('Model[%s/%s] - Updated model', project_name, model_name)
 
-        :param project_id: The unique identifier of the project on Fiddler
-        :param model_id: The unique identifier of the model on Fiddler
+        return Model.deserialize(APIResponseHandler(response))
 
-        :returns: A fiddler.ModelInfo object describing the model.
+    @handle_api_error_response
+    def delete_model(self, model_name: str, project_name: str) -> None:
         """
-        model_info_dict = self.client_v2.get_model(
-            project_name=project_id, model_name=model_id
-        ).info
-        return ModelInfo.from_dict(model_info_dict)
+        Delete a model
 
-    # Uploading Dataset
-    def upload_dataset_dataframe(
-        self,
-        project_id: str,
-        dataset: Dict[str, pd.DataFrame],
-        dataset_id: str,
-        info: Optional[DatasetInfo] = None,
-        size_check_enabled: bool = True,
-    ) -> Dict[str, str]:
-        """Uploads a representative dataset to the Fiddler engine.
-
-        :param project_id: The unique identifier of the model's project on the
-            Fiddler engine.
-        :param dataset: A dictionary mapping name -> DataFrame
-            containing data to be uploaded to the Fiddler engine.
-        :param dataset_id: The unique identifier of the dataset on the Fiddler
-            engine. Must be a short string without whitespace.
-        :param info: A DatasetInfo object specifying all the details of the
-            dataset.
-        :param size_check_enabled: Unused argument to maintain compatibility
-
-        :returns: The server response for the upload.
-        """
-        return self.client_v2.upload_dataset_dataframe(
-            project_name=project_id,
-            dataset_name=dataset_id,
-            datasets=dataset,
-            info=info,
-            is_sync=True,
-        )
+        :params model_name: Model name to be deleted
+        :params project_name: Project name to which the model belongs to.
 
-    def upload_dataset(
-        self,
-        project_id: str,
-        dataset_id: str,
-        file_path: str,
-        file_type: str = 'csv',
-        file_schema=Dict[str, Any],
-        info: Optional[DatasetInfo] = None,
-        size_check_enabled: bool = False,
-    ) -> Dict[str, str]:
-        """Uploads a representative dataset to the Fiddler engine from directory.
-
-        :param project_id: The unique identifier of the model's project on the
-            Fiddler engine.
-        :param dataset_id: The unique identifier of the dataset on the Fiddler
-            engine. Must be a short string without whitespace.
-        :param file_path: str pointing to the dataset to be uploaded
-        :param file_type: str representing the file type of the uploading dataset. Supported type 'csv'
-        :param file_schema: <TBD>
-        :param info: A DatasetInfo object specifying all the details of the
-            dataset.
-        :param size_check_enabled: Unused argument to maintain compatibility
-
-        :returns: The server response for the upload.
-        """
-        file_name = file_path.split('/')[-1]
-        files = {file_name: Path(file_path)}
-        if file_type == 'csv':
-            return self.client_v2.upload_dataset(
-                project_name=project_id,
-                dataset_name=dataset_id,
-                files=files,
-                info=info,
-                file_type=FileType.CSV,
-                file_schema=file_schema,
-            )
-        else:
-            raise NotImplementedError('Only csv is supported in current implementation')
+        :returns: None
+        """
+        logger.info('Deleting model %s from %s project', model_name, project_name)
+        self.client.delete(
+            url=f'models/{self.organization_name}:{project_name}:{model_name}',
+        )
+        logger.info('Deleted model %s from %s project', model_name, project_name)
 
-    def upload_dataset_dir(
+    @handle_api_error_response
+    def add_model_surrogate(
         self,
-        project_id: str,
-        dataset_id: str,
-        dataset_dir: Path,
-        file_type: str = 'csv',
-        file_schema=None,
-        size_check_enabled: bool = False,
-    ) -> Dict[str, str]:
-        # Input checks
-        if file_type != 'csv':
-            raise NotImplementedError('Only CSV filetype is supported')
-
-        if not dataset_dir.is_dir():
-            raise ValueError(f'{dataset_dir} is not a directory')
-
-        dataset_yaml = dataset_dir / f'{dataset_id}.yaml'
-        if not dataset_yaml.is_file():
-            raise ValueError(f'Dataset YAML file not found: {dataset_yaml}')
-
-        with dataset_yaml.open() as f:
-            dataset_info = DatasetInfo.from_dict(yaml.safe_load(f))
-
-        # Convert files into dataframes
-        files = dataset_dir.glob(f'*.{FileType.CSV}')
-        csv_files = [x for x in files if x.is_file()]
-
-        dataset = {}
-        csv_paths = []
-        for file in csv_files:
-            csv_name = str(file).split('/')[-1]
-            csv_paths.append(csv_name)
-            name = csv_name[:-4]
-
-            # @TODO Change the flow so that we can read the CSV in chunks
-            dataset[name] = pd.read_csv(file, dtype=dataset_info.get_pandas_dtypes())
-
-        # size check
-        size_exceeds = False
-        for name, df in dataset.items():
-            if df.shape[0] > DATASET_MAX_ROWS:
-                size_exceeds = True
-        if size_exceeds:
-            raise RuntimeError(
-                f'Dataset upload aborted as size exceeds {DATASET_MAX_ROWS}.'
-            )
-
-        return self.upload_dataset_dataframe(
-            project_id=project_id,
-            dataset_id=dataset_id,
-            dataset=dataset,
-            info=dataset_info,
-            size_check_enabled=size_check_enabled,
+        model_name: str,
+        project_name: str,
+        deployment_params: Optional[DeploymentParams] = None,
+        wait: bool = True,
+    ) -> str:
+        """
+        Add surrogate model to an existing model
+        :param model_name: Model name
+        :param project_name: Project name
+        :param deployment_params: Model deployment parameters
+        :param wait: Whether to wait for job to complete or return after submitting
+            the job
+        :return: Async job uuid
+        """
+        return self._deploy_surrogate_model(
+            model_name=model_name,
+            project_name=project_name,
+            deployment_params=deployment_params,
+            wait=wait,
+            update=False,
         )
 
-    def upload_dataset_from_dir(
+    @check_version(version_expr='>=23.1.0')
+    @handle_api_error_response
+    def update_model_surrogate(
         self,
-        project_id: str,
-        dataset_id: str,
-        dataset_dir: Path,
-        file_type: str = 'csv',
-        file_schema=None,
-        size_check_enabled: bool = False,
-    ) -> Dict[str, str]:
-        """Uploads a representative dataset to the Fiddler engine from directory.
-
-        :param project_id: The unique identifier of the model's project on the
-            Fiddler engine.
-        :param dataset_id: The unique identifier of the dataset on the Fiddler
-            engine. Must be a short string without whitespace.
-        :param dataset_dir: pathlib.Path pointing to the dir that contains the dataset
-            and dataset info yaml to be uploaded.
-        :param file_type: File type of the dataset being uploaded. Supported type: 'csv'
-        :param file_schema: <TBD>
-        :param size_check_enabled: Unused argument to maintain compatibility
-
-        :returns: The server response for the upload.
-        """
-        if file_type != 'csv':
-            raise NotImplementedError('Only CSV filetype is supported')
-
-        info_yaml = dataset_dir / f'{dataset_id}.yaml'
-
-        if not info_yaml.exists():
-            raise ValueError(f'DatasetInfo yaml ({info_yaml}) not found.')
-
-        with open(info_yaml) as f:
-            dataset_info = DatasetInfo.from_dict(yaml.safe_load(f))
-
-        return self.client_v2.upload_dataset_from_dir(
-            project_id,
-            dataset_id,
-            dataset_dir,
-            dataset_info,
-            FileType.CSV,
-            file_schema,
-            is_sync=True,
+        model_name: str,
+        project_name: str,
+        deployment_params: Optional[DeploymentParams] = None,
+        wait: bool = True,
+    ) -> str:
+        """
+        Re-generate surrogate model
+        :param model_name: Model name
+        :param project_name: Project name
+        :param deployment_params: Model deployment parameters
+        :param wait: Whether to wait for job to complete or return after submitting
+            the job
+        :return: Async job uuid
+        """
+        return self._deploy_surrogate_model(
+            model_name=model_name,
+            project_name=project_name,
+            deployment_params=deployment_params,
+            wait=wait,
+            update=True,
         )
 
-    def publish_events_batch_schema(
+    def _deploy_surrogate_model(
         self,
-        batch_source: Union[Path, str],
-        publish_schema: Dict[str, Any],
-        data_source: Optional[BatchPublishType] = None,
-    ) -> None:
-        return self.client_v2.publish_events_batch_schema(
-            batch_source, publish_schema, data_source
+        model_name: str,
+        project_name: str,
+        deployment_params: Optional[DeploymentParams] = None,
+        wait: bool = True,
+        update: bool = False,
+    ) -> str:
+        """
+        Add surrogate model to an existing model
+        :param model_name: Model name
+        :param project_name: Project name
+        :param deployment_params: Model deployment parameters
+        :param wait: Whether to wait for job to complete or return after submitting
+            the job
+        :param update: Set True for re-generating surrogate model, otherwise False
+        :return: Async job uuid
+        """
+        payload = {
+            'model_name': model_name,
+            'project_name': project_name,
+            'organization_name': self.organization_name,
+        }
+
+        if deployment_params:
+            deployment_params.artifact_type = ArtifactType.SURROGATE
+            payload['deployment_params'] = deployment_params.dict(exclude_unset=True)
+
+        model_id = f'{self.organization_name}:{project_name}:{model_name}'
+        url = f'models/{model_id}/deploy-surrogate'
+        method = self.client.put if update else self.client.post
+        response = method(url=url, data=payload)
+
+        data = APIResponseHandler(response).get_data()
+        job_uuid = data['job_uuid']
+
+        logger.info(
+            'Model[%s/%s] - Submitted job (%s) for deploying a surrogate model',
+            project_name,
+            model_name,
+            job_uuid,
         )
 
-    def publish_events_batch(  # noqa
+        if wait:
+            job_name = f'Model[{project_name}/{model_name}] - Deploy a surrogate model'
+            self.wait_for_job(uuid=job_uuid, job_name=job_name)  # noqa
+
+        return job_uuid
+
+    def _deploy_model_artifact(
         self,
-        project_id: str,
-        model_id: str,
-        batch_source: Union[pd.DataFrame, str],
-        id_field: Optional[str] = None,
-        update_event: Optional[bool] = False,
-        timestamp_field: Optional[str] = None,
-        timestamp_format: FiddlerTimestamp = FiddlerTimestamp.INFER,
-        data_source: Optional[BatchPublishType] = None,
-        casting_type: Optional[bool] = False,
-        credentials: Optional[dict] = None,
-        group_by: Optional[str] = None,
-    ) -> Dict[str, str]:
-        """
-        Publishes a batch events object to Fiddler Service.
-        :param project_id:    The project to which the model whose events are being published belongs.
-        :param model_id:      The model whose events are being published.
-        :param batch_source:  Batch object to be published. Can be one of: Pandas DataFrame, CSV file
-        :param id_field:  Column to extract id value from.
-        :param update_event: Bool indicating if the events are updates to previously published rows
-        :param timestamp_field:     Column to extract timestamp value from.
-                              Timestamp must match the specified format in `timestamp_format`.
-        :param timestamp_format:   Format of timestamp within batch object. Can be one of:
-                                - FiddlerTimestamp.INFER
-                                - FiddlerTimestamp.EPOCH_MILLISECONDS
-                                - FiddlerTimestamp.EPOCH_SECONDS
-                                - FiddlerTimestamp.ISO_8601
-        :param data_source:   Source of batch object. In case of failed inference, can be one of:
-                                - BatchPublishType.DATAFRAME
-                                - BatchPublishType.LOCAL_DISK
-                                - BatchPublishType.AWS_S3
-                                - BatchPublishType.GCP_STORAGE
-        :param casting_type: Unused argument to maintain compatibility
-        :param credentials: Unused argument to maintain compatibility
-        :param group_by: Column to group events together for Model Performance metrics. For example,
-                         in ranking models that column should be query_id or session_id, used to
-                         compute NDCG and MAP. Be aware that the batch_source file/dataset provided should have
-                         events belonging to the SAME query_id/session_id TOGETHER and cannot be mixed
-                         in the file. For example, having a file with rows belonging to query_id 31,31,31,2,2,31,31,31
-                         would not work. Please sort the file by group_by group first to have rows with
-                         the following order: query_id 31,31,31,31,31,31,2,2.
-        """
-        v2_timestamp_format = V2FiddlerTimestamp(timestamp_format.value)
-        if type(batch_source) == pd.DataFrame and (
-            data_source is None or BatchPublishType.DATAFRAME == data_source
+        project_name: str,
+        model_name: str,
+        artifact_dir: str,
+        deployment_params: Optional[DeploymentParams] = None,
+        wait: bool = True,
+        update: bool = False,
+    ) -> str:
+        """
+        Upload and deploy model artifact for an existing model
+        :param model_name: Model name
+        :param project_name: Project name
+        :param artifact_dir: Model artifact directory
+        :param deployment_params: Model deployment parameters
+        :param wait: Whether to wait for async job to finish or return
+        :param update: Set True for updating artifact, False for adding artifact
+        :return: Async job uuid
+        """
+        artifact_dir = Path(artifact_dir)
+        validate_artifact_dir(artifact_dir)
+
+        if (
+            deployment_params
+            and deployment_params.artifact_type == ArtifactType.SURROGATE
         ):
-            if batch_source.empty:
-                raise ValueError("The batch provided is empty. Please retry with at least one row of data.")
+            raise ValueError(
+                f'{ArtifactType.SURROGATE} artifact_type is an invalid value for this '
+                f'method. Use {ArtifactType.PYTHON_PACKAGE} instead.'
+            )
+
+        self._update_model_on_artifact_upload(
+            model_name=model_name, project_name=project_name, artifact_dir=artifact_dir
+        )
 
-            return self.client_v2.publish_events_batch_dataframe(
-                project_name=project_id,
-                model_name=model_id,
-                events_df=batch_source,
-                id_field=id_field,
-                is_update=update_event,
-                timestamp_field=timestamp_field,
-                timestamp_format=v2_timestamp_format,
-                group_by=group_by,
-                is_sync=False,
+        with tempfile.TemporaryDirectory() as tmp:
+            # Archive model artifact directory
+            logger.info(
+                'Model[%s/%s] - Tarring model artifact directory - %s',
+                project_name,
+                model_name,
+                artifact_dir,
             )
-        elif type(batch_source) == str and (
-            data_source is None or BatchPublishType.LOCAL_DISK == data_source
-        ):
-            return self.client_v2.publish_events_batch(
-                project_name=project_id,
-                model_name=model_id,
-                events_path=Path(batch_source),
-                id_field=id_field,
-                is_update=update_event,
-                timestamp_field=timestamp_field,
-                timestamp_format=v2_timestamp_format,
-                group_by=group_by,
-                file_type=FileType.CSV,
-                is_sync=False,
+            file_path = shutil.make_archive(
+                base_name=str(Path(tmp) / 'files'),
+                format='tar',
+                root_dir=str(artifact_dir),
+                base_dir='.',
+            )
+
+            logger.info(
+                'Model[%s/%s] - Model artifact tar file created at %s',
+                project_name,
+                model_name,
+                file_path,
             )
-        else:
-            if data_source is not None:
-                if (data_source not in [BatchPublishType.LOCAL_DISK, BatchPublishType.DATAFRAME]):
-                    raise NotImplementedError(
-                        f'support for data_source type of {data_source} is not yet implemented'
-                    )
-                elif BatchPublishType.DATAFRAME == data_source and not isinstance(batch_source, pd.DataFrame):
-                    raise ValueError(f'based on the provided data_source type ({data_source}), expecting batch_source to be a pandas DataFrame, but instead found a {type(batch_source)}')
-                elif BatchPublishType.LOCAL_DISK == data_source and not isinstance(batch_source, str):
-                    raise ValueError(f'based on the provided data_source type ({data_source}), expecting batch_source to be a filepath string, but instead found a {type(batch_source)}')
+
+            # Choose deployer based on archive file size
+            if os.path.getsize(file_path) < MULTI_PART_CHUNK_SIZE:
+                deployer_class = ModelArtifactDeployer
             else:
-                raise ValueError('batch_source must be either a filepath string or a pandas DataFrame')
-                            
+                deployer_class = MultiPartModelArtifactDeployer
+
+            deployer = deployer_class(
+                client=self.client,
+                model_name=model_name,
+                project_name=project_name,
+                organization_name=self.organization_name,
+                update=update,
+            )
+
+            job_uuid = deployer.deploy(
+                file_path=Path(file_path), deployment_params=deployment_params
+            )
+
+        logger.info(
+            'Model[%s/%s] - Submitted job (%s) for deploying model artifact',
+            project_name,
+            model_name,
+            job_uuid,
+        )
 
-    def publish_event(
+        if wait:
+            job_name = f'Model[{project_name}/{model_name}] - Deploy model artifact'
+            self.wait_for_job(uuid=job_uuid, job_name=job_name)  # noqa
+
+        return job_uuid
+
+    @handle_api_error_response
+    def add_model_artifact(
+        self,
+        model_name: str,
+        project_name: str,
+        artifact_dir: str,
+        deployment_params: Optional[DeploymentParams] = None,
+        wait: bool = True,
+    ) -> str:
+        """
+        Add model artifact to an existing model
+        :param model_name: Model name
+        :param project_name: Project name
+        :param artifact_dir: Model artifact directory
+        :param deployment_params: Model deployment parameters
+        :param wait: Whether to wait for async job to finish or return
+        :return: Async job uuid
+        """
+        return self._deploy_model_artifact(
+            project_name=project_name,
+            model_name=model_name,
+            artifact_dir=artifact_dir,
+            deployment_params=deployment_params,
+            wait=wait,
+            update=False,
+        )
+
+    @check_version(version_expr='>=22.12.0')
+    @handle_api_error_response
+    def update_model_artifact(
         self,
-        project_id: str,
-        model_id: str,
-        event: dict,
-        event_id: Optional[str] = None,
-        update_event: Optional[bool] = None,
-        event_timestamp: Optional[int] = None,
-        timestamp_format: FiddlerTimestamp = FiddlerTimestamp.INFER,
-        casting_type: Optional[bool] = False,
-        dry_run: Optional[bool] = False,
+        model_name: str,
+        project_name: str,
+        artifact_dir: str,
+        deployment_params: Optional[DeploymentParams] = None,
+        wait: bool = True,
     ) -> str:
         """
-        Publishes an event to Fiddler Service.
-        :param project_id: The project to which the model whose events are being published belongs
-        :param model_id: The model whose events are being published
-        :param dict event: Dictionary of event details, such as features and predictions.
-        :param event_id: Unique str event id for the event
-        :param update_event: Bool indicating if the event is an update to a previously published row
-        :param event_timestamp: The UTC timestamp of the event in epoch milliseconds (e.g. 1609462800000)
-        :param timestamp_format:   Format of timestamp within batch object. Can be one of:
-                                - FiddlerTimestamp.INFER
-                                - FiddlerTimestamp.EPOCH_MILLISECONDS
-                                - FiddlerTimestamp.EPOCH_SECONDS
-                                - FiddlerTimestamp.ISO_8601
-        :param casting_type: Unused argument to maintain compatibility
-        :param dry_run: Unused argument to maintain compatibility
-
-        """
-        v2_timestamp_format = V2FiddlerTimestamp(timestamp_format.value)
-        return self.client_v2.publish_event(
-            project_name=project_id,
-            model_name=model_id,
-            event=event,
-            event_id=event_id,
-            is_update=update_event,
-            event_timestamp=event_timestamp,
-            timestamp_format=v2_timestamp_format,
+        Update model artifact of an existing model
+        :param model_name: Model name
+        :param project_name: Project name
+        :param artifact_dir: Model artifact directory
+        :param deployment_params: Model deployment parameters
+        :param wait: Whether to wait for async job to finish or return
+        :return: Async job uuid
+        """
+        return self._deploy_model_artifact(
+            project_name=project_name,
+            model_name=model_name,
+            artifact_dir=artifact_dir,
+            deployment_params=deployment_params,
+            wait=wait,
+            update=True,
+        )
+
+    def _update_model_on_artifact_upload(
+        self, model_name: str, project_name: str, artifact_dir: Path
+    ) -> None:
+        """Update model metadata based on artifact dir contents"""
+        file_list = get_model_artifact_info(artifact_dir=artifact_dir)
+        model_info = read_model_yaml(artifact_dir=artifact_dir)
+
+        self.update_model(
+            model_name=model_name,
+            project_name=project_name,
+            info=model_info,
+            file_list=file_list,
         )
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/alert_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/alert_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from datetime import datetime, timedelta
+import warnings
 from typing import Any, Dict, List, Optional
 
 from pydantic import parse_obj_as
 
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.schema.alert import (
@@ -14,26 +15,27 @@
     BinSize,
     ComparePeriod,
     CompareTo,
     Metric,
     Priority,
     TriggeredAlerts,
 )
-from fiddler.v2.utils.exceptions import handle_api_error_response
+from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.helpers import match_semvar
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class AlertMixin:
     FILTER_ALERT_RULES_API_VERSION = '>=23.1.0'
+    GROUP_OF_COLUMNS_API_VERSION = '>=23.3.0'
 
     client: RequestClient
     organization_name: str
 
     @handle_api_error_response
     def add_alert_rule(
         self,
@@ -46,14 +48,15 @@
         priority: Priority,
         critical_threshold: float,
         condition: AlertCondition,
         bin_size: BinSize = BinSize.ONE_DAY,
         baseline_id: Optional[str] = None,
         compare_period: Optional[ComparePeriod] = None,
         column: Optional[str] = None,
+        columns: Optional[List[str]] = None,
         warning_threshold: Optional[float] = None,
         notifications_config: Optional[Dict[str, Dict[str, Any]]] = None,
     ) -> AlertRule:
         """
         To add an alert rule
         :param project_id: Unique project name for which the alert rule is created
         :param model_id: Unique model name for which the alert rule is created
@@ -108,50 +111,70 @@
                 3) Priority.HIGH
         :param warning_threshold: Threshold value to crossing which a warning level severity alert will be triggered
         :param critical_threshold: Threshold value to crossing which a critical level severity alert will be triggered
         :param condition: Select from:
                 1) AlertCondition.LESSER
                 2) AlertCondition.GREATER
         :param column: column name on which alert rule is to be created. It can take '__ANY__' to check for all columns
+        :param columns: List of column names on which alert rule is to be created. It can take ['__ANY__'] to check for all columns
         :param notifications_config: notifications config object created using helper method build_notifications_config()
         :param baseline_id: Name of the baselne, whose histogram is compared against the same derived from current data.
                             Used only when alert type is AlertType.DATA_DRIFT.
         :return: created alert rule object
         """
+        if columns and not match_semvar(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
+            raise ValueError(f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}')
+
+        if column:
+            warnings.warn(
+                'WARNING: column is deprecated in 1.8 and will be removed '
+                'from version 2.0.0. As a replacement, use columns while constructing AlertRule.',
+                DeprecationWarning,
+            )
+
+        if column and columns:
+            raise ValueError(f'Both column and columns are specified. Please use one of them.')
 
         if not notifications_config:
             notifications_config = self.build_notifications_config()
 
         if bin_size not in BinSize.keys():
             raise ValueError(f'bin_size: {bin_size} should be one of: {BinSize.keys()}')
         if compare_to == CompareTo.TIME_PERIOD and not compare_period:
             raise ValueError(
                 f'compare_period is required when compare_to is {CompareTo.TIME_PERIOD}'
             )
         if compare_period and compare_period not in ComparePeriod.keys():
             raise ValueError(f'compare_period should be one of{ComparePeriod.keys()}')
 
+        feature_name:str = None
+        feature_names:str = None
+        if match_semvar(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
+            feature_names = ",".join(columns) if columns else column
+        else:
+            feature_name = column
         request_body = AlertRulePayload(
-            organization_name=self.organization_name,
-            project_name=project_id,
-            model_name=model_id,
-            name=name,
-            alert_type=alert_type,
-            metric=metric,
-            compare_to=compare_to,
-            compare_period=compare_period,
-            priority=priority,
-            baseline_name=baseline_id,
-            warning_threshold=warning_threshold,
-            critical_threshold=critical_threshold,
-            condition=condition,
-            feature_name=column,
-            time_bucket=bin_size,
-            notifications=notifications_config,
-        ).dict()
+                organization_name=self.organization_name,
+                project_name=project_id,
+                model_name=model_id,
+                name=name,
+                alert_type=alert_type,
+                metric=metric,
+                compare_to=compare_to,
+                compare_period=compare_period,
+                priority=priority,
+                baseline_name=baseline_id,
+                feature_name=feature_name,
+                feature_names=feature_names,
+                warning_threshold=warning_threshold,
+                critical_threshold=critical_threshold,
+                condition=condition,
+                time_bucket=bin_size,
+                notifications=notifications_config,
+            ).dict()
         response = self.client.post(
             url='alert-configs',
             data=request_body,
         )
         response_data = APIResponseHandler(response)
         alert_rule_id = response_data.get_data().get('uuid')
 
@@ -176,14 +199,15 @@
     def get_alert_rules(
         self,
         project_id: Optional[str] = None,
         model_id: Optional[str] = None,
         alert_type: Optional[AlertType] = None,
         metric: Optional[Metric] = None,
         column: Optional[str] = None,
+        columns: Optional[List[str]] = None,
         baseline_id: Optional[str] = None,
         ordering: Optional[List[str]] = None,
         offset: int = 0,
         limit: int = 20,
     ) -> List[AlertRule]:
         """
         Get a list of alert rules with respect to the filtering parameters
@@ -216,21 +240,35 @@
                     2) MetricType.JSD
 
                 For data_integrity:
                     1) MetricType.RANGE_VIOLATION
                     2) MetricType.MISSING_VALUE
                     3) MetricType.TYPE_VIOLATION
         :param column: Filter based on the column
+        :param columns: Filter based on a list of column names
         :param limit: Number of records to be retrieved per page, also referred as page_size
         :param offset: Pointer to the starting of the page index. offset of the first page is 0
                         and it increments by limit for each page, for e.g., 5th pages offset when
                         limit=100 will be (5 - 1) * 100 = 400. This means 5th page will contain
                         records from index 400 to 499.
         :return: paginated list of alert rules for the set filters
         """
+        if columns and not match_semvar(self.server_info.server_version, self.GROUP_OF_COLUMNS_API_VERSION):
+            raise ValueError(f'columns parameter works with server version {self.GROUP_OF_COLUMNS_API_VERSION}')
+
+        if column:
+            warnings.warn(
+                'WARNING: column is deprecated in 1.8 and will be removed '
+                'from version 2.0.0. As a replacement, use columns while constructing AlertRule.',
+                DeprecationWarning,
+            )
+
+        if column and columns:
+            raise ValueError(f'Both column and columns are specified. Please use one of them.')
+
         alert_params = {
             'organization_name': self.organization_name,
             'offset': offset,
             'limit': limit,
         }
 
         if match_semvar(
@@ -253,18 +291,18 @@
                 )
 
             if metric:
                 filter_by_rules.append(
                     {'field': 'metric', 'operator': 'equal', 'value': metric}
                 )
 
-            if column:
-                filter_by_rules.append(
-                    {'field': 'feature_name', 'operator': 'equal', 'value': column}
-                )
+            if columns:
+                filter_by_rules.append({'field': 'feature_names', 'operator': 'contains', 'value': columns})
+            elif column:
+                filter_by_rules.append({'field': 'feature_name', 'operator': 'equal', 'value': column})
 
             if baseline_id:
                 filter_by_rules.append(
                     {
                         'field': 'baseline_name',
                         'operator': 'equal',
                         'value': baseline_id,
@@ -280,25 +318,24 @@
         else:
             alert_params.update(
                 {
                     'project_name': project_id,
                     'model_name': model_id,
                     'alert_type': alert_type,
                     'metric': metric,
-                    'feature_name': column,
                     'baseline_name': baseline_id,
                     'ordering': ordering,
                 }
             )
 
         response = self.client.get(
             url='alert-configs',
             params=alert_params,
         )
-        _, items = PaginatedResponseHandler(response).get_pagination_details_and_items()
+        items = PaginatedResponseHandler(response).get_pagination_items()
 
         return parse_obj_as(List[AlertRule], items)
 
     @handle_api_error_response
     def get_triggered_alerts(
         self,
         alert_rule_uuid: str,
@@ -327,15 +364,15 @@
                 'start_time': start_time,
                 'end_time': end_time,
                 'offset': offset,
                 'limit': limit,
                 'ordering': ordering,
             },
         )
-        _, items = PaginatedResponseHandler(response).get_pagination_details_and_items()
+        items = PaginatedResponseHandler(response).get_pagination_items()
         return parse_obj_as(List[TriggeredAlerts], items)
 
     def build_notifications_config(
         self,
         emails: str = '',
         pagerduty_services: str = '',
         pagerduty_severity: str = '',
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/api.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from typing import Optional
 from urllib.parse import urljoin
 
 from fiddler._version import __version__
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.api.alert_mixin import AlertMixin
 from fiddler.v2.api.baseline_mixin import BaselineMixin
-
 # @todo: This is v1 implementation needs to have a proper v2 approach
 from fiddler.v2.api.dataset_mixin import DatasetMixin
 from fiddler.v2.api.events_mixin import EventsMixin
 from fiddler.v2.api.explainability_mixin import ExplainabilityMixin
 from fiddler.v2.api.job_mixin import JobMixin
 from fiddler.v2.api.model_deployment_mixin import ModelDeploymentMixin
 from fiddler.v2.api.model_mixin import ModelMixin
 from fiddler.v2.api.project_mixin import ProjectMixin
-from fiddler.v2.constants import FIDDLER_CLIENT_VERSION_HEADER
+from fiddler.v2.constants import CURRENT_API_VERSION, FIDDLER_CLIENT_VERSION_HEADER
 from fiddler.v2.schema.server_info import ServerInfo
 
 logger = logging.getLogger(__name__)
-VERSION = '/v2'
-
 
-class Client(
+class FiddlerClient(
     ModelMixin,
     DatasetMixin,
     ProjectMixin,
     EventsMixin,
     JobMixin,
     BaselineMixin,
     AlertMixin,
@@ -37,27 +33,30 @@
         self,
         url: str,
         organization_name: str,
         auth_token: str,
         timeout: int = None,
         verify: bool = True,
     ) -> None:
-        self.url = urljoin(url, VERSION)
+        self.url = (
+            url
+            if url.endswith(CURRENT_API_VERSION)
+            else urljoin(url, CURRENT_API_VERSION)
+        )
         self.auth_token = auth_token
         self.organization_name = organization_name
         self.request_headers = {'Authorization': f'Bearer {auth_token}'}
         self.request_headers.update({FIDDLER_CLIENT_VERSION_HEADER: f'{__version__}'})
         self.timeout = timeout
         self.client = RequestClient(
             base_url=self.url, headers=self.request_headers, verify=verify
         )
 
-        self.server_info: Optional[ServerInfo] = self._get_server_info()
+        self.server_info: ServerInfo = self._get_server_info()
 
     def _get_server_info(self) -> ServerInfo:
-
         response = self.client.get(
             url='server-info',
             params={'organization_name': self.organization_name},
         )
 
         return ServerInfo(**response.json().get('data'))
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/baseline_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/baseline_mixin.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pydantic import parse_obj_as
 
 from fiddler.core_objects import BaselineType, WindowSize
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.schema.baseline import Baseline
-from fiddler.v2.utils.exceptions import handle_api_error_response
+from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -34,15 +34,15 @@
             url='baselines/',
             params={
                 'organization_name': self.organization_name,
                 'project_name': project_id,
                 'model_name': model_id,
             },
         )
-        _, items = PaginatedResponseHandler(response).get_pagination_details_and_items()
+        items = PaginatedResponseHandler(response).get_pagination_items()
         return parse_obj_as(List[Baseline], items)
 
     @handle_api_error_response
     def get_baseline(
         self, project_id: str, model_id: str, baseline_id: str
     ) -> Baseline:
         """Get the details of a Baseline.
@@ -61,86 +61,104 @@
             params={
                 'organization_name': self.organization_name,
                 'project_name': project_id,
                 'model_name': model_id,
                 'baseline_name': baseline_id,
             },
         )
-        _, items = PaginatedResponseHandler(response).get_pagination_details_and_items()
+        items = PaginatedResponseHandler(response).get_pagination_items()
 
         # If a baseline exists, only a single baseline should be returned
         if len(items) == 1:
             return parse_obj_as(Baseline, items[0])
         else:
             return None
 
     @handle_api_error_response
     def add_baseline(
         self,
-        project_id: str,
-        model_id: str,
-        baseline_id: str,
+        project_name: str,
+        model_name: str,
+        baseline_name: str,
         type: BaselineType,
-        dataset_id: str = None,
+        dataset_name: str = None,
         start_time: int = None,
         end_time: int = None,
         offset: WindowSize = None,
         window_size: WindowSize = None,
+        wait: bool = False,
     ) -> Baseline:
         """Function to add a Baseline to fiddler for monitoring
 
-        :param project_id: unique identifier for the project
-        :type project_id: string
-        :param model_id: unique identifier for the model
-        :type model_id: string
-        :param baseline_id: unique identifier for the baseline
-        :type baseline_id: string
+        :param project_name: unique name for the project
+        :type project_name: string
+        :param model_name: unique name for the model
+        :type model_name: string
+        :param baseline_name: unique name for the baseline
+        :type baseline_name: string
         :param type: type of the Baseline
         :type type: BaselineType
-        :param dataset_id: (optional) dataset to be used as baseline
-        :type dataset_id: string
+        :param dataset_name: (optional) dataset to be used as baseline
+        :type dataset_name: string
         :param start_time: (optional) seconds since epoch to be used as start time for STATIC_PRODUCTION baseline
         :type start_time: int
         :param end_time: (optional) seconds since epoch to be used as end time for STATIC_PRODUCTION baseline
         :type end_time: int
         :param offset: (optional) offset in seconds relative to current time to be used for ROLLING_PRODUCTION baseline
         :type offset: WindowSize
         :param window_size: (optional) width of window in seconds to be used for ROLLING_PRODUCTION baseline
         :type window_size: WindowSize
+        :type run_async: Boolean
+        :type wait: Boolean
 
 
         :return: Baseline object which contains the Baseline details
         """
         if window_size:
             window_size = int(window_size)  # ensure enum is converted to int
 
         request_body = Baseline(
             organization_name=self.organization_name,
-            project_name=project_id,
-            name=baseline_id,
+            project_name=project_name,
+            name=baseline_name,
             type=str(type),
-            model_name=model_id,
-            dataset_name=dataset_id,
+            model_name=model_name,
+            dataset_name=dataset_name,
             start_time=start_time,
             end_time=end_time,
             offset=offset,
             window_size=window_size,
+            run_async=True,
         ).dict()
 
         if 'id' in request_body:
             request_body.pop('id')
 
         response = self.client.post(
             url='baselines/',
             data=request_body,
         )
 
         if response.status_code == HTTPStatus.OK:
-            logger.info(f'{baseline_id} setup successful')
+            logger.info(f'{baseline_name} setup successful')
             return Baseline.deserialize(APIResponseHandler(response))
+        if response.status_code == HTTPStatus.ACCEPTED:
+            data = APIResponseHandler(response).get_data()
+            job_uuid = data['job_uuid']
+            logger.info(
+                'Model[%s/%s] - Submitted job (%s) for adding default baseline',
+                project_name,
+                model_name,
+                job_uuid,
+            )
+            if wait:
+                job_name = f'Model[{project_name}/{model_name}] - create Default Baseline'
+                self.wait_for_job(uuid=job_uuid, job_name=job_name)  # noqa
+            return job_uuid
+
 
     @handle_api_error_response
     def delete_baseline(self, project_id: str, model_id: str, baseline_id: str) -> None:
         """Delete a Baseline
 
         :param project_id: unique identifier for the project
         :type project_id: string
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/dataset_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/dataset_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import os
 import tempfile
 import time
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional
 
-import numpy as np
 import pandas as pd
-from pydantic import parse_obj_as
+import yaml
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
-from fiddler.core_objects import Column, DataType, DatasetInfo, DEFAULT_MAX_INFERRED_CARDINALITY
+from fiddler.core_objects import DatasetInfo, DEFAULT_MAX_INFERRED_CARDINALITY
+from fiddler.exceptions import FiddlerAPIHTTPException
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.api.helpers import multipart_upload
 from fiddler.v2.constants import FileType, UploadType
 from fiddler.v2.schema.dataset import Dataset, DatasetIngest
-from fiddler.v2.utils.exceptions import FiddlerAPIException, handle_api_error_response
+from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 from fiddler.v2.validators.dataset_validator import (
     validate_dataset_columns,
     validate_dataset_info,
@@ -47,30 +47,30 @@
         """
         response = self.client.get(
             url='datasets',
             params={
                 'organization_name': self.organization_name,
                 'project_name': project_name,
             },
-        )        
-        _, items = PaginatedResponseHandler(response).get_pagination_details_and_items()
-        datasets:List[Dataset] = []
-        for item in items:
-            try :
-                datasets.append(Dataset.from_dict(item))
-            except KeyError as ke:
-                raise FiddlerAPIException(
-                    status_code=response.status_code,
-                    error_code=response.status_code,
-                    message=f'Invalid response content. {str(ke)} in the response.',
-                    errors=[],
-                )   
+        )
+        items = PaginatedResponseHandler(response).get_pagination_items()
+        datasets = [Dataset.from_dict(item) for item in items]
         return datasets
 
     @handle_api_error_response
+    def get_dataset_names(self, project_name: str) -> List[str]:
+        """List the names of all datasets in the organization.
+
+        :param project_name: The project for which you want to get the datasets
+        :returns: List of strings containing the names of each dataset.
+        """
+        datasets = self.get_datasets(project_name=project_name)
+        return [d.name for d in datasets]
+
+    @handle_api_error_response
     def get_dataset(self, project_name: str, dataset_name: str) -> Dataset:
         """
         Get all the details for a given dataset
 
         :param project_name:    The project to which the dataset belongs to
         :param dataset_name:    The dataset name of which you need the details
 
@@ -80,14 +80,27 @@
         response = self.client.get(
             url=f'datasets/{self.organization_name}:{project_name}:{dataset_name}',
         )
         response_handler = APIResponseHandler(response)
         return Dataset.deserialize(response_handler)
 
     @handle_api_error_response
+    def get_dataset_info(self, project_name: str, dataset_name: str) -> DatasetInfo:
+        """
+        Get DatasetInfo for a dataset.
+
+        :param project_name:    The project to which the dataset belongs to
+        :param dataset_name:    The dataset name of which you need the details
+
+        :returns: A fiddler.DatasetInfo object describing the dataset.
+        """
+        dataset = self.get_dataset(project_name, dataset_name)
+        return dataset.info
+
+    @handle_api_error_response
     def add_dataset(
         self,
         name: str,
         project_name: str,
         info: Optional[DatasetInfo] = None,
     ) -> Dataset:
         request_body = dict(
@@ -134,23 +147,26 @@
         file_type: Optional[FileType] = None,
         file_schema: Optional[dict] = None,
         is_sync: Optional[bool] = True,
     ) -> Dict[str, str]:
         """
         Upload a dataset.
 
-        :param project_name:    The project to which the dataset belongs to
-        :param dataset_name:    Dataset name used for upload
-        :param files:           A dictionary of file name and key and file path as value. Eg `{'train': pathlib.Path('datasets/train.csv')}`
-        :param info:            DatasetInfo object
-        :param file_type:       FileType which specifices the filetype csv etc.
-        :param file_schema:     <TBD>
-        :param is_sync:         A boolean value which determines if the upload method works in synchronous mode or async mode
+        :param project_name:   The project to which the dataset belongs to
+        :param dataset_name:   Dataset name used for upload
+        :param files:          A dictionary of file name and key and file path as value.
+                               Eg `{'train': pathlib.Path('datasets/train.csv')}`
+        :param info:           DatasetInfo object
+        :param file_type:      FileType which specifices the filetype csv etc.
+        :param file_schema:    <TBD>
+        :param is_sync:        A boolean value which determines if the upload method
+                               works in synchronous mode or async mode
 
-        :returns:               Dictionary containing details of the job used to publish events incase of 202 response from the server.
+        :returns:              Dictionary containing details of the job used to publish
+                               events incase of 202 response from the server.
         """
         validate_dataset_info(info)
         validate_dataset_shape(files)
 
         file_names = []
         for _, file_path in files.items():
             _, file_name = os.path.split(file_path)
@@ -193,17 +209,17 @@
                 job = self.wait_for_job(uuid=job_uuid, job_name=job_name).get_data()
                 job.pop('extras', None)
                 time.sleep(20)
                 return job
             else:
                 return resp
         else:
-            # raising a generic FiddlerAPIException
+            # raising a generic FiddlerAPIHTTPException
             logger.error(f'Failed to upload dataset {dataset_name}.')
-            raise FiddlerAPIException(
+            raise FiddlerAPIHTTPException(
                 response.status_code,
                 error_code=response.status_code,
                 message=response.content,
                 errors=[],
             )
 
     @handle_api_error_response
@@ -231,92 +247,102 @@
             raise ValueError('`files` is empty. Please enter a valid input')
 
         return self.upload_dataset(
             project_name, dataset_name, files, info, FileType.CSV, file_schema, is_sync
         )
 
     @handle_api_error_response
-    def upload_dataset_dataframe(
+    def upload_dataset_from_dataframe(
         self,
         project_name: str,
         dataset_name: str,
         datasets: Dict[str, pd.DataFrame],
         info: Optional[DatasetInfo] = None,
-        is_sync: Optional[bool] = True,
+        wait: Optional[bool] = True,
     ) -> Dict[str, str]:
         """
         Upload dataset as pd.DataFrame
 
         :param project_name:    The project to which the dataset belongs to
         :param dataset_name:    Dataset name used for upload
         :param datasets:        A dictionary of dataframe as value and name as key. Eg `{'train': train_df}`
         :param info:            DatasetInfo object
-        :param is_sync:         A boolean value which determines if the upload method works in synchronous mode or async mode
+        :param wait:         A boolean value which determines if the upload method works in synchronous mode or async mode
 
         :returns:               Dictionary containing details of the job used to publish events incase of 202 response from the server.
         """
         if not datasets:
             raise ValueError('`datasets` is empty. Please enter a valid dataset')
 
-        # will throw FiddlerAPIException if project does not exist
+        # will throw FiddlerAPIHTTPException if project does not exist
         self.client.get(url=f'projects/{self.organization_name}:{project_name}')
 
         with tempfile.TemporaryDirectory() as tmp:
             files = {}
             file_type = FileType.CSV
             for name, df in datasets.items():
-                file_path = Path(tmp) / f'{name}{file_type}'
+                file_path = Path(tmp) / f'{name}{file_type.value}'
                 df.to_csv(file_path, index=False)
                 files[name] = file_path
 
             return self.upload_dataset(
                 project_name,
                 dataset_name,
                 files=files,
                 info=info,
                 file_type=file_type,
-                is_sync=is_sync,
+                is_sync=wait,
             )
 
     @handle_api_error_response
     def upload_dataset_from_dir(
         self,
         project_name: str,
         dataset_name: str,
         dataset_dir: Path,
-        info: Optional[DatasetInfo] = None,
         file_type: FileType = FileType.CSV,
         file_schema: Optional[dict] = None,
         is_sync: bool = True,
     ) -> Dict[str, str]:
         """
         Upload dataset artefacts (data file and dataset info yaml) from a directory
 
         :param project_name:    The project to which the dataset belongs to
         :param dataset_name:    Dataset name used for upload
         :param dataset_dir:     pathlib.Path pointing to the dataset dir to be uploaded
-        :param info:            DatasetInfo object
         :param file_type:       FileType
         :param file_schema:     <TBD>
         :param is_sync:         A boolean value which determines if the upload method works in synchronous mode or async mode
 
         :returns:               Dictionary containing details of the job used to publish events incase of 202 response from the server.
         """
         # @TODO: Move repetative input validation used accross different methods to utils
+
+        if file_type != FileType.CSV:
+            raise NotImplementedError('Only CSV filetype is supported')
+
         if not dataset_dir.is_dir():
             raise ValueError(f'{dataset_dir} is not a directory')
 
         files = {
             data_file.name: data_file
             for data_file in dataset_dir.glob(f'*{file_type.value}')
         }
 
         if not files:
             raise ValueError(f'No data files found in {dataset_dir}.')
 
+        info_yaml = dataset_dir / f'{dataset_name}.yaml'
+
+        if not info_yaml.exists():
+            raise ValueError(f'DatasetInfo yaml ({info_yaml}) not found.')
+
+        with open(info_yaml) as f:
+            info = DatasetInfo.from_dict(yaml.safe_load(f))
+
         return self.upload_dataset(
             project_name=project_name,
             dataset_name=dataset_name,
             files=files,
             info=info,
             file_schema=file_schema,
             is_sync=is_sync,
@@ -332,29 +358,29 @@
         sample_size: Optional[int] = DEFAULT_SAMPLE_SIZE,
         chunk_size: Optional[int] = DEFAULT_NROWS_PER_CHUNK,
     ) -> DatasetInfo:
         """
         Derives DatasetInfo from the given csv file
 
         :param file_path:       Relative or absolute path of the file in string format, for example, 'datasets/train.csv'
-        :param display_name:    A name for user-facing display (different from an id). 
+        :param display_name:    A name for user-facing display (different from an id).
         :param dataset_id:      Dataset Id
 
         :returns:               DatasetInfo derived from the input file_path
         """
         if not file_path:
             raise ValueError('`file_path` is empty. Please enter a valid input.')
 
         file_path = Path(file_path)
 
         if not file_path.exists():
             raise ValueError('`file_path` does not exist. Please enter a valid input.')
 
         # TODO (pradhuman): Read from dir
-        
+
         dataset_infos:List[DatasetInfo] = []
         # 1. read file
         with pd.read_csv(file_path, chunksize=chunk_size) as reader:
             for df in reader:
                 logger.info(f'Read a chunk from input {df.shape}')
                 # 2. take random sample
                 if df.shape[0] > sample_size:
@@ -384,8 +410,8 @@
                 response = self.client.post(
                     url='infer-data-types', data=request_body, files_encoders=files_encoders
                 )
                 api_response = APIResponseHandler(response)
                 logger.info(api_response.get_status_code)
                 dataset_infos.append(DatasetInfo.from_dict(api_response.get_data()))
         logger.info(f'combining {len(dataset_infos)} DatasetInfo objects')
-        return DatasetInfo.as_combination(infos=dataset_infos, display_name=display_name)
+        return DatasetInfo.as_combination(infos=dataset_infos, display_name=display_name)
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/events_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/events_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import pandas as pd
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from fiddler.core_objects import BatchPublishType
+from fiddler.exceptions import FiddlerAPIHTTPException
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.api.helpers import multipart_upload
 from fiddler.v2.constants import FiddlerTimestamp, FileType, UploadType
 from fiddler.v2.schema.events import EventIngest, EventsIngest
-from fiddler.v2.utils.exceptions import FiddlerAPIException, handle_api_error_response
+from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
 logger = logging.getLogger(__name__)
 
 
 class EventsMixin:
     client: RequestClient
@@ -108,17 +109,17 @@
 
                 job = self.wait_for_job(uuid=job_uuid, job_name=job_name).get_data()
                 job.pop('extras', None)
                 return job
             else:
                 return resp
         else:
-            # raising a generic FiddlerAPIException
+            # raising a generic FiddlerAPIHTTPException
             logger.error('Failed to publish events')
-            raise FiddlerAPIException(
+            raise FiddlerAPIHTTPException(
                 response.status_code,
                 error_code=response.status_code,
                 message=response.content,
                 errors=[],
             )
 
     @handle_api_error_response
@@ -161,17 +162,17 @@
             data=request_body,
         )
         if response.status_code == HTTPStatus.ACCEPTED:
             response_dict = APIResponseHandler(response).get_data()
             logger.info(response_dict.get('message'))
             return response_dict.get('__fiddler_id')
         else:
-            # raising a generic FiddlerAPIException
+            # raising a generic FiddlerAPIHTTPException
             logger.error('Failed to publish events')
-            raise FiddlerAPIException(
+            raise FiddlerAPIHTTPException(
                 response.status_code,
                 error_code=response.status_code,
                 message=response.content,
                 errors=[],
             )
 
     @handle_api_error_response
@@ -211,15 +212,17 @@
                         in the file. For example, having a file with rows belonging to query_id 31,31,31,2,2,31,31,31
                         would not work. Please sort the file by group_by group first to have rows with
                         the following order: query_id 31,31,31,31,31,31,2,2.
         :param is_sync: A boolean value which determines if the upload method works in synchronous mode or async mode
         :returns: Dictionary containing details of the job used to publish events incase of 202 response from the server.
         """
         if events_df is None or events_df.empty:
-            raise ValueError("The batch provided is empty. Please retry with at least one row of data.")
+            raise ValueError(
+                'The batch provided is empty. Please retry with at least one row of data.'
+            )
 
         file_type = FileType.CSV
         with tempfile.NamedTemporaryFile(suffix=file_type) as temp:
             events_df.to_csv(temp, index=False)
             events_path = Path(temp.name)
             return self.publish_events_batch(
                 project_name=project_name,
@@ -240,35 +243,40 @@
         batch_source: Union[Path, str],
         publish_schema: Dict[str, Any],
         data_source: Optional[BatchPublishType] = None,
         is_sync: Optional[bool] = False,
     ) -> Dict[str, str]:
         """
         Publishes a batch events object to Fiddler Service.
-        :param events_path: pathlib.Path pointing to the events file to be uploaded
+        :param batch_source: pathlib.Path pointing to the events file to be uploaded
         :param publish_schema: Dict object specifying layout of data.
-        :param is_sync: A boolean value which determines if the upload method works in synchronous mode or async mode
-        :returns: Dictionary containing details of the job used to publish events incase of 202 response from the server.
+        :param data_source: path of the source file of type BatchPublishType
+        :param is_sync: A boolean value which determines if the upload method works in
+                        synchronous mode or async mode
+        :returns: Dictionary containing details of the job used to publish events incase
+                  of 202 response from the server.
         """
-        events_path = batch_source
         request_body_json = {}
         request_body_json['schema'] = publish_schema
-        if data_source == BatchPublishType.AWS_S3 and isinstance(events_path, str):
-            request_body = {'s3_url': events_path, 'schema': json.dumps(publish_schema)}
+        if data_source == BatchPublishType.AWS_S3 and isinstance(batch_source, str):
+            request_body = {
+                's3_url': batch_source,
+                'schema': json.dumps(publish_schema),
+            }
             response = self.client.post(
                 url=f'events/{self.organization_name}/ingest/schema',
                 headers={'Content-Type': 'application/json'},
                 data=request_body,
             )
         else:
-            if isinstance(events_path, str):
-                events_path = Path(events_path)
-            file_name = events_path.name
+            if isinstance(batch_source, str):
+                batch_source = Path(batch_source)
+            file_name = batch_source.name
             files = {}
-            files[file_name] = events_path
+            files[file_name] = batch_source
             request_body = {
                 file_path.name: (
                     file_path.name,
                     open(file_path, 'rb'),
                 )
                 for _, file_path in files.items()
             }
@@ -304,15 +312,15 @@
                 job = self.wait_for_job(uuid=job_uuid, job_name=job_name).get_data()
                 job.pop('extras', None)
                 return job
             else:
                 return resp
 
         else:
-            # raising a generic FiddlerAPIException
+            # raising a generic FiddlerAPIHTTPException
             logger.error('Failed to upload events schema.')
-            raise FiddlerAPIException(
+            raise FiddlerAPIHTTPException(
                 response.status_code,
                 error_code=response.status_code,
                 message=response.content,
                 errors=[],
             )
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/explainability_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/explainability_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pandas as pd
 from pydantic import BaseModel
 
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.utils.pandas import try_series_retype
-from fiddler.v2.utils.exceptions import handle_api_error_response
+from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
 logger = logging.getLogger(__name__)
 
 
 class DatasetDataSource(BaseModel):
     source_type = 'DATASET'
@@ -106,15 +106,15 @@
         ci_level: Optional[float] = None,
         output_columns: Optional[List[str]] = None,
         min_support: Optional[int] = None,
         overwrite_cache: bool = False,
     ) -> NamedTuple:
         """
         Get global feature impact for a model over a dataset or a slice
-        ::param model_name: The unique identifier of the model
+        :param model_name: The unique identifier of the model
         :param project_name: The unique identifier of the model's project
         :param data_source: DataSource for the input dataset to compute feature
             impact on (DatasetDataSource or SqlSliceQueryDataSource)
         :param num_iterations: The maximum number of ablated model inferences
             *per feature*.
         :param num_refs: number of reference points used in the explanation
         :param ci_level: The confidence level (between 0 and 1)
@@ -204,27 +204,27 @@
             model_name=model_name,
             project_name=project_name,
             organization_name=self.organization_name,
             input_data_source=input_data_source.dict(),
             convert_to_gem=False,
         )
 
-        if ref_data_source is not None:
+        if ref_data_source:
             request_body['ref_data_source'] = ref_data_source.dict()
 
-        if explanation_type is not None:
+        if explanation_type:
             request_body['explanation_type'] = explanation_type
 
-        if num_permutations is not None:
+        if num_permutations:
             request_body['num_permutations'] = num_permutations
 
-        if ci_level is not None:
+        if ci_level:
             request_body['ci_level'] = ci_level
 
-        if top_n_class is not None:
+        if top_n_class:
             request_body['top_n_class'] = top_n_class
 
         response = self.client.post(
             url='explain',
             data=request_body,
         )
 
@@ -263,28 +263,28 @@
             project_name=project_name,
             organization_name=self.organization_name,
             data_source=data_source.dict(),
             protected_features=protected_features,
             positive_outcome=positive_outcome,
         )
 
-        if score_threshold is not None:
+        if score_threshold:
             request_body['score_threshold'] = score_threshold
 
         response = self.client.post(
             url='fairness',
             data=request_body,
         )
 
         response_dict = APIResponseHandler(response).get_data()
 
         return namedtuple('FairnessResult', response_dict)(**response_dict)
 
     @handle_api_error_response
-    def run_slice_query(
+    def get_slice(
         self,
         project_name: str,
         query: str,
         columns: Optional[List[str]] = None,
         sample: Optional[bool] = None,
         max_rows: Optional[int] = None,
     ) -> pd.DataFrame:
@@ -303,34 +303,33 @@
 
         request_body = dict(
             project_name=project_name,
             organization_name=self.organization_name,
             query=query,
         )
 
-        if sample is not None:
+        if sample:
             request_body['sample'] = sample
-        if max_rows is not None:
+        if max_rows:
             request_body['max_rows'] = max_rows
-        if columns is not None:
+        if columns:
             request_body['columns'] = columns
 
         response = self.client.post(
             url='slice-query/fetch',
             data=request_body,
         )
 
         response_dict = APIResponseHandler(response).get_data()
 
         column_names = response_dict['meta']['columns']
         dtype_strings = response_dict['meta']['dtypes']
         df = pd.DataFrame(response_dict['rows'], columns=column_names)
         for column_name, dtype in zip(column_names, dtype_strings):
             df[column_name] = try_series_retype(df[column_name], dtype)
-
         return df
 
     @handle_api_error_response
     def get_predictions(
         self,
         model_name: str,
         project_name: str,
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/helpers.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/job_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/job_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import time
 from http import HTTPStatus
 from typing import Iterator, List, Optional
 
 from requests.exceptions import ConnectionError
 
+from fiddler.exceptions import AsyncJobFailed
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.schema.job import JobStatus
-from fiddler.v2.utils.exceptions import AsyncJobFailed, handle_api_error_response
+from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import JobResponseHandler
 
 logger = logging.getLogger(__name__)
 
 
 class JobMixin:
     DEFAULT_POLL_INTERVAL = 3  # In seconds
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/model_artifact_deploy.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/model_artifact_deploy.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/model_deployment_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/model_deployment_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional
 
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.schema.model_deployment import ModelDeployment
-from fiddler.v2.utils.decorators import check_version
-from fiddler.v2.utils.exceptions import handle_api_error_response
+from fiddler.v2.utils.decorators import check_version, handle_api_error_response
 
 logger = logging.getLogger(__name__)
 
 
 class ModelDeploymentMixin:
     """Model deployment api handler"""
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/api/project_mixin.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/api/project_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from pydantic import parse_obj_as
 
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.schema.project import Project
-from fiddler.v2.utils.exceptions import handle_api_error_response
+from fiddler.v2.utils.decorators import handle_api_error_response
 from fiddler.v2.utils.response_handler import (
     APIResponseHandler,
     PaginatedResponseHandler,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -33,17 +33,27 @@
             params={
                 'organization_name': self.organization_name,
                 'limit': limit,
                 'offset': offset,
             },
         )
         # @TODO:  abstracted as an iter object so user doesn't have to manage pagination manually
-        _, items = PaginatedResponseHandler(response).get_pagination_details_and_items()
+        items = PaginatedResponseHandler(response).get_pagination_items()
         return parse_obj_as(List[Project], items)
 
+    # Projects
+    def get_project_names(self) -> List[str]:
+        """List the ids of all projects in the organization.
+
+        :returns: List of strings containing the ids of each project.
+        """
+        projects = self.get_projects()
+        return [p.name for p in projects]
+
+
     @handle_api_error_response
     def delete_project(self, project_name: str) -> None:
         """
         Delete a project
 
         :params project_name: Name of the project to delete
         :returns: None
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/constants.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 MULTI_PART_UPLOAD_SIZE_THRESHOLD = 5 * 1024 * 1024  # 5MB in bytes
 MULTI_PART_CHUNK_SIZE = 100 * 1024 * 1024  # 100MB in bytes
 
 # File processor
 SUPPORTABLE_FILE_EXTENSIONS = ['.csv']
 CSV_EXTENSION = 'csv'
 
+# Version
+CURRENT_API_VERSION = 'v2'
+
 @enum.unique
 class FiddlerTimestamp(str, enum.Enum):
     """Supported timestamp formats for events published to Fiddler"""
 
     EPOCH_MILLISECONDS = 'epoch milliseconds'
     EPOCH_SECONDS = 'epoch seconds'
     ISO_8601 = '%Y-%m-%d %H:%M:%S.%f'
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/schema/alert.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/schema/alert.py`

 * *Files 16% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 @enum.unique
 class ComparePeriod(enum.IntEnum):
     """Time period values for comparison with previous window"""
 
     ONE_DAY = 86400000
     SEVEN_DAYS = 604800000
-    ONE_MONTH = 2629743000
+    ONE_MONTH = 2592000000
     THREE_MONTHS = 7776000000
 
     @classmethod
     def keys(cls) -> List[str]:
         return list(cls.__members__.values())
 
     def __repr__(self) -> str:
@@ -136,14 +136,15 @@
     organization_name: str
     project_name: str
     model_name: str
     name: str
     alert_type: AlertType
     metric: Metric
     feature_name: Optional[str]
+    feature_names: Optional[str]
     priority: Priority
     compare_to: CompareTo
     baseline_name: Optional[str]
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
@@ -155,15 +156,15 @@
     alert_rule_uuid: str = Field(alias='uuid')
     organization_name: str
     project_id: str = Field(alias='project_name')
     model_id: str = Field(alias='model_name')
     name: Optional[str]
     alert_type: AlertType
     metric: Metric
-    column: str = Field(alias='feature_name')
+    columns: Optional[List[str]]
     baseline_id: Optional[str] = Field(alias='baseline_name')
     priority: Priority
     compare_to: CompareTo
     compare_period: Optional[ComparePeriod]
     warning_threshold: Optional[float]
     critical_threshold: float
     condition: AlertCondition
@@ -172,14 +173,21 @@
     @root_validator(pre=True)
     def set_compare_period(cls, values) -> Optional[ComparePeriod]:
 
         if values['compare_period'] == 0:
             values['compare_period'] = None
         return values
 
+    @root_validator(pre=True)
+    def set_feature_names(cls, values) -> Optional[List[str]]:
+        if 'feature_names' in values:
+            values['columns'] = list(map(lambda x: x.strip(), values['feature_names'].split(",")))
+        else:
+            values['columns'] = None
+        return values
 
 class TriggeredAlerts(BaseDataSchema):
     id: int
     triggered_alert_id: str = Field(alias='uuid')
     alert_rule_uuid: str = Field(alias='alert_config_uuid')
     alert_run_start_time: int
     alert_time_bucket: int
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/schema/dataset.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/schema/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import re
 from typing import Any, Dict, List, Optional
 
-from fiddler.v2.constants import FileType, UploadType
-from fiddler.v2.schema.base import BaseDataSchema
 from fiddler.core_objects import DatasetInfo
+from fiddler.exceptions import FiddlerAPIHTTPException
+from fiddler.v2.constants import FileType, UploadType
 from fiddler.v2.utils.response_handler import APIResponseHandler
-from fiddler.v2.utils.exceptions import FiddlerAPIException
 
 
 class Dataset:
     def __init__(
             self,
         id: int,
         name: str,
@@ -29,30 +27,30 @@
 
     @classmethod
     def deserialize(cls, response: APIResponseHandler):
         data = response.get_data()
         try:
             return cls.from_dict(data)
         except KeyError as ke:
-            raise FiddlerAPIException(
+            raise FiddlerAPIHTTPException(
                 status_code=response.status_code,
                 error_code=response.status_code,
                 message=f'Invalid response content. {str(ke)} in the response.',
                 errors=[],
             )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]):
         for required_field in ['id', 'name', 'version', 'info', 'file_list', 'organization_name', 'project_name']:
             if required_field not in data:
                 raise KeyError("Required {required_field} in not found")
-        # v2 version of DatasetInfo required only columns 
-        # core_objects.DatasetInfo requires display_name 
+        # v2 version of DatasetInfo required only columns
+        # core_objects.DatasetInfo requires display_name
         # Hence to keep python-client backward compatible with fiddler-server, name is added.
-        datasetinfo_json = data['info'] 
+        datasetinfo_json = data['info']
         if 'name' not in datasetinfo_json:
             datasetinfo_json['name'] = data['name']
         return cls(
             id=data['id'],
             name=data['name'],
             version=data['version'],
             info=DatasetInfo.from_dict(datasetinfo_json),
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/schema/events.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/schema/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/schema/model_deployment.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/schema/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/utils/exceptions.py` & `fiddler-client-2.0.0.dev5/fiddler/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from collections import namedtuple
-from functools import wraps
-from http import HTTPStatus
 from typing import List, NamedTuple
 
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json import JSONDecodeError
 
@@ -32,37 +30,43 @@
         )
 
     def get_error_details(self) -> NamedTuple:
         status_code = self.response.status_code
         try:
             error_details = self.response.json().get('error', {})
         except JSONDecodeError:
-            raise FiddlerAPIException(
+            raise FiddlerAPIHTTPException(
                 status_code=self.response.status_code,
                 error_code=self.response.status_code,
                 message=f'Invalid response content-type. {self.response.status_code}:{self.response.content}',
                 errors=[],
             )
         error_code = error_details.get('code')
         message = error_details.get('message')
         errors = error_details.get('errors')
         return self.ErrorResponse(status_code, error_code, message, errors)
 
 
-class BaseException(Exception):
+class FiddlerBaseException(Exception):
     pass
 
 
-class FiddlerException(BaseException):
+class FiddlerException(FiddlerBaseException):
     '''
     Exception class to handle non API response exceptions
     '''
 
 
-class FiddlerAPIException(BaseException):
+class FiddlerAPICallException(FiddlerBaseException):
+    def __init__(self, message: str) -> None:
+        self.message = message
+        super().__init__(self.message)
+
+
+class FiddlerAPIHTTPException(FiddlerBaseException):
     '''
     Exception class to specifically handle Fiddler's API error responses structure.
     This is a generic API response exception class
     '''
 
     # @TODO: Handle standard API error response.
     # How to surface error messages coming form the server. Server responds error messages in a list. Which error to surface?
@@ -72,63 +76,26 @@
         self.status_code = status_code
         self.error_code = error_code
         self.message = message
         self.errors = errors
         super().__init__(self.message)
 
 
-class FiddlerAPIBadRequestException(FiddlerAPIException):
+class FiddlerAPIBadRequestException(FiddlerAPIHTTPException):
     pass
 
 
-class FiddlerAPINotFoundException(FiddlerAPIException):
+class FiddlerAPINotFoundException(FiddlerAPIHTTPException):
     pass
 
 
-class FiddlerAPIConflictException(FiddlerAPIException):
+class FiddlerAPIConflictException(FiddlerAPIHTTPException):
     pass
 
 
-class FiddlerAPIForbiddenException(FiddlerAPIException):
+class FiddlerAPIForbiddenException(FiddlerAPIHTTPException):
     pass
 
 
-class FiddlerAPIInternalServerErrorException(FiddlerAPIException):
+class FiddlerAPIInternalServerErrorException(FiddlerAPIHTTPException):
     pass
 
-
-map_except_resp_code = {
-    HTTPStatus.BAD_REQUEST: FiddlerAPIBadRequestException,  # 400
-    HTTPStatus.FORBIDDEN: FiddlerAPIForbiddenException,  # 403
-    HTTPStatus.NOT_FOUND: FiddlerAPINotFoundException,  # 404
-    HTTPStatus.CONFLICT: FiddlerAPIConflictException,  # 409
-    HTTPStatus.INTERNAL_SERVER_ERROR: FiddlerAPIInternalServerErrorException,  # 500
-}
-
-
-def handle_api_error_response(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        try:
-            return func(*args, **kwargs)
-        except HTTPError as error:
-            logger.error(
-                'HTTP request to %s failed with %s - %s',
-                getattr(error.request, 'url', 'unknown'),
-                getattr(error.response, 'status_code', 'unknown'),
-                getattr(error.response, 'content', 'missing'),
-            )
-            error_response = ErrorResponseHandler(error).get_error_details()
-            # raise status_code specific exceptions else raise generic FiddlerAPIException
-            exec_class = map_except_resp_code.get(
-                error_response.status_code, FiddlerAPIException
-            )
-            raise exec_class(
-                error_response.status_code,
-                error_response.error_code,
-                error_response.message,
-                error_response.errors,
-            ) from None
-            # disabling automatic exception chaining
-            # ref: https://docs.python.org/3/tutorial/errors.html#exception-chaining
-
-    return wrapper
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/utils/helpers.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/utils/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import yaml
 
-from ...core_objects import ModelInfo
-from ..schema.server_info import Version
-from .exceptions import NotSupported
+from fiddler.core_objects import ModelInfo
+from fiddler.exceptions import NotSupported
+from fiddler.v2.schema.server_info import Version
 
 
 def match_semvar(version: Optional[Version], match_expr: str) -> bool:
     """
     Match the version with match_expr
     :param version: Server version
     :param match_expr: Version to match with. Read more at VersionInfo.match
@@ -21,15 +21,15 @@
 
     if version.prerelease:
         return Version(version.major, version.minor, version.patch).match(match_expr)
 
     return version.match(match_expr)
 
 
-def raise_not_support(
+def raise_not_supported(
     compatible_client_version: str,
     client_version: str,
     server_version: Version
 ):
     """
     Raise error when client version is not compatible with the server version.
     :param compatible_client_version: Max client version supported for the server
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/utils/response_handler.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/utils/response_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List
 
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json import JSONDecodeError
 
 import requests
 
 from fiddler.utils import logging
-from fiddler.v2.utils.exceptions import FiddlerAPIException
+from fiddler.exceptions import FiddlerAPIHTTPException
 
 logger = logging.getLogger(__name__)
 
 
 class BaseResponseHandler:
     def __init__(self, response: requests.Response) -> None:
         self.response = response
         logger.debug(self.response.content)
 
     def get_data(self) -> Dict[str, Any]:
         try:
             dict_response = self.response.json().get('data')
         except JSONDecodeError:
-            raise FiddlerAPIException(
+            raise FiddlerAPIHTTPException(
                 status_code=self.response.status_code,
                 error_code=self.response.status_code,
                 message=f'Invalid response content-type. {self.response.status_code}:{self.response.content}',
                 errors=[],
             )
-        dict_response.pop('created_at', None)
-        dict_response.pop('updated_at', None)
         return dict_response
 
     def get_status_code(self) -> int:
         return self.response.status_code
 
 
 class PaginatedResponseHandler(BaseResponseHandler):
     '''
     Handle fiddler OAS's standard Paginated response
     '''
 
-    def get_pagination_details_and_items(self) -> Tuple[dict, List[dict]]:
-        data = self.get_data()
-        items = data.pop('items')
-        return data, items
+    def get_pagination_items(self) -> List[dict]:
+        return self.get_data().get('items', [])
 
 
 class APIResponseHandler(BaseResponseHandler):
     '''
     Handle fiddler OAS's standard API Response
     '''
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/v2/validators/dataset_validator.py` & `fiddler-client-2.0.0.dev5/fiddler/v2/validators/dataset_validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from pathlib import Path
 from typing import Dict
 
 import pandas as pd
-import pandas.errors
 
 from fiddler.core_objects import DatasetInfo
 
 LOG = logging.getLogger(__name__)
 
 NUM_ROWS = 1
 JUST_THE_HEADER = 0
@@ -25,15 +24,15 @@
     rows = 0
     columns = 0
 
     for _, file_path in files.items():
         try:
             df = pd.read_csv(file_path, nrows=NUM_ROWS)
             rows, columns = df.shape
-        except pandas.errors.EmptyDataError:
+        except pd.errors.EmptyDataError:
             rows = 0
             columns = 0
 
         # empty checks.
         if columns == 0:
             raise ValueError('No columns found in dataset provided.')
         if rows == 0:
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler/validator.py` & `fiddler-client-2.0.0.dev5/fiddler/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import pathlib
 import pickle
 import urllib.request
 from typing import Dict, List, NamedTuple, Tuple, Type
 
 import pandas as pd
 
-from .assets.pg_reserved_words import pg_reserved_words
-from .core_objects import DatasetInfo, DataType, ModelInfo, ModelTask
-from .utils import ColorLogger
+from fiddler.assets.pg_reserved_words import pg_reserved_words
+from fiddler.core_objects import DatasetInfo, DataType, ModelInfo, ModelTask
+from fiddler.utils import ColorLogger
 
 PG_COLUMN_NAME_MAX_LENGTH = 63
 
 # Validation core objects
 
 
 class ValidationError:
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-2.0.0.dev5/fiddler_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 2.0.0.dev3
+Version: 2.0.0.dev5
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -18,15 +18,15 @@
         Installation
         ------------
         
             $ pip3 install fiddler-client
         
         API Example Usage
         -------------
-        Documentation for the API can be found [here](https://api.fiddler.ai/#introduction). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/quick-start/) as well as the work notebooks found on our [Samples Github](https://github.com/fiddler-labs/fiddler-samples).
+        Documentation for the API can be found [here](https://docs.fiddler.ai/reference/about-the-fiddler-client). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/docs/quick-start) as well as the notebooks found on our [Examples Github](https://github.com/fiddler-labs/fiddler-examples).
         
         Version History
         -------------
         
         ### 2.0.0
           - #### **Removed**
             - Following methods are removed
@@ -41,20 +41,33 @@
               - list_org_roles
               - unshare_project
               - share_project
               - process_avro
               - process_csv
           - #### **New Features**
             - Add `monitor_components` as an attribute of `CustomFeature`. Default to `False`
-        
+            - Add `columns` as a parameter in `add_alert_rule` and `get_alert_rules` functions
         ### 1.8.0
           - #### **Modifications**
+            - Add new alert type -  `statistic` for setting alerts
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
         
+        ### 1.7.4
+          - #### **Modification**
+            - Do not typecast column with strings in get_slice()
+        
+        ### 1.7.3
+          - #### **Modification**
+            - Send row and column count information to dataset upload api
+        
+        ### 1.7.2
+          - #### **Modification**
+            - Bring back `WeightingParams` object
+        
         ### 1.7.1
           - #### **Modification**
             - Relaxed boto3 version constraint
         
         ### 1.7.0
           - #### **Removed**
             - Remove support for initializing fiddler client with version=1
```

### Comparing `fiddler-client-2.0.0.dev3/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-2.0.0.dev5/fiddler_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 MANIFEST.in
 PUBLIC.md
 README.md
 setup.py
 fiddler/__init__.py
 fiddler/_version.py
-fiddler/aws_utils.py
 fiddler/client.py
 fiddler/connection.py
 fiddler/constants.py
 fiddler/core_objects.py
 fiddler/dataset.py
-fiddler/experimental.py
+fiddler/exceptions.py
 fiddler/fiddler_api.py
 fiddler/model.py
-fiddler/model_info_validator.py
 fiddler/monitoring_validator.py
 fiddler/project.py
-fiddler/v1_v2_compat.py
 fiddler/validator.py
-fiddler/api/__init__.py
-fiddler/api/monitoring.py
 fiddler/assets/__init__.py
 fiddler/assets/pg_reserved_words.py
 fiddler/libs/__init__.py
 fiddler/libs/http_client.py
 fiddler/packtools/__init__.py
 fiddler/packtools/gem.py
 fiddler/packtools/keras_ig_helpers.py
@@ -61,21 +56,19 @@
 fiddler/v2/schema/model.py
 fiddler/v2/schema/model_deployment.py
 fiddler/v2/schema/project.py
 fiddler/v2/schema/server_info.py
 fiddler/v2/schema/user.py
 fiddler/v2/utils/__init__.py
 fiddler/v2/utils/decorators.py
-fiddler/v2/utils/exceptions.py
 fiddler/v2/utils/helpers.py
 fiddler/v2/utils/response_handler.py
 fiddler/v2/utils/validations.py
 fiddler/v2/validators/__init__.py
 fiddler/v2/validators/dataset_validator.py
 fiddler_client.egg-info/PKG-INFO
 fiddler_client.egg-info/SOURCES.txt
 fiddler_client.egg-info/dependency_links.txt
 fiddler_client.egg-info/requires.txt
 fiddler_client.egg-info/top_level.txt
 tests/__init__.py
-tests/test_fiddler_api.py
-tests/test_v1_v2_compat.py
+tests/test_fiddler_api.py
```

### Comparing `fiddler-client-2.0.0.dev3/setup.py` & `fiddler-client-2.0.0.dev5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,18 @@
     long_description_content_type='text/markdown',
     url='https://fiddler.ai',
     packages=setuptools.find_packages(),
     install_requires=[
         'pip>=21.0',
         'requests<3',
         'requests-toolbelt',
-        'pandas>=1.2.5,<=1.5.3',
+        'pandas>=1.2.5,<1.6',
         'pyyaml',
         'packaging',
         'deepdiff',
-        'boto3',
         'importlib-resources',
         'Werkzeug',
         'deprecation==2.1.0',
         'pydantic>=1.9.0',
         'urllib3<2',
         'deprecated==1.2.13',
         'semver>=2,<3',
```

### Comparing `fiddler-client-2.0.0.dev3/tests/test_fiddler_api.py` & `fiddler-client-2.0.0.dev5/tests/test_fiddler_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import pytest
 from pytest_mock import MockFixture
 
 from fiddler import FiddlerApi
-from fiddler.v2.api.api import Client
+from fiddler.v2.api.api import FiddlerClient
 from fiddler.v2.schema.server_info import ServerInfo, Version
 
 
 def test_client_v1_creation_fail():
     with pytest.raises(ValueError):
         FiddlerApi('', '', '')
 
 
 def test_client_v2_creation_fail():
     with pytest.raises(ValueError):
-        FiddlerApi('', '', '', version=2)
+        FiddlerApi('', '', '', version='v2')
 
 
 def test_get_server_info_without_server_version(mocker: MockFixture):
     mocker.patch('fiddler.connection.Connection.check_connection', return_value='OK')
 
     server_info_dict = {
         'feature_flags': {
             'fairness': False,
         },
     }
 
-    mock_get_server_info = mocker.patch.object(Client, '_get_server_info')
+    mock_get_server_info = mocker.patch.object(FiddlerClient, '_get_server_info')
     mock_get_server_info.return_value = ServerInfo(**server_info_dict)
 
-    client = FiddlerApi('https://test.fiddler.ai', 'test', 'foo-token', version=2)
+    client = FiddlerApi('https://test.fiddler.ai', 'test', 'foo-token', version='v2')
 
     assert client.v2.server_info.server_version is None
     assert client.v2.server_info.feature_flags == server_info_dict['feature_flags']
 
 
 def test_get_server_info_with_server_version(mocker: MockFixture):
     mocker.patch('fiddler.connection.Connection.check_connection', return_value='OK')
@@ -40,16 +40,16 @@
     server_info_dict = {
         'feature_flags': {
             'fairness': False,
         },
         'server_version': '23.1.1',
     }
 
-    mock_get_server_info = mocker.patch.object(Client, '_get_server_info')
+    mock_get_server_info = mocker.patch.object(FiddlerClient, '_get_server_info')
     mock_get_server_info.return_value = ServerInfo(**server_info_dict)
 
-    client = FiddlerApi('https://test.fiddler.ai', 'test', 'foo-token', version=2)
+    client = FiddlerApi('https://test.fiddler.ai', 'test', 'foo-token', version='v2')
 
     assert client.v2.server_info.server_version == Version.parse(
         server_info_dict['server_version']
     )
     assert client.v2.server_info.feature_flags == server_info_dict['feature_flags']
```

