# Comparing `tmp/arize-7.0.5rc0.tar.gz` & `tmp/arize-7.0.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.5rc0.tar", last modified: Tue Jun 13 23:05:38 2023, max compression
+gzip compressed data, was "arize-7.0.6rc0.tar", last modified: Fri Jun 23 21:43:04 2023, max compression
```

## Comparing `arize-7.0.5rc0.tar` & `arize-7.0.6rc0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.671826 arize-7.0.5rc0/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-12 17:30:40.000000 arize-7.0.5rc0/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-12 17:30:40.000000 arize-7.0.5rc0/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-13 23:05:38.672087 arize-7.0.5rc0/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-12 17:30:40.000000 arize-7.0.5rc0/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.573876 arize-7.0.5rc0/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    28890 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.605977 arize-7.0.5rc0/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.607396 arize-7.0.5rc0/arize/exporter/
--rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.612206 arize-7.0.5rc0/arize/exporter/core/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/core/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    10541 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/exporter/core/client.py
--rw-r--r--   0 kiko       (501) staff       (20)      470 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/core/endpoint.py
--rw-r--r--   0 kiko       (501) staff       (20)     1285 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/exporter/core/query.py
--rw-r--r--   0 kiko       (501) staff       (20)     3931 2023-06-13 23:03:26.000000 arize-7.0.5rc0/arize/exporter/core/session.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.616857 arize-7.0.5rc0/arize/exporter/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1349 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)       99 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)     4678 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 kiko       (501) staff       (20)      552 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/exporter/utils/validation.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.618761 arize-7.0.5rc0/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.629714 arize-7.0.5rc0/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.630616 arize-7.0.5rc0/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.633999 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    23005 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.635777 arize-7.0.5rc0/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     5058 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.656288 arize-7.0.5rc0/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    69574 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-12 19:46:43.000000 arize-7.0.5rc0/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.666095 arize-7.0.5rc0/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    24227 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-12 17:30:40.000000 arize-7.0.5rc0/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.580009 arize-7.0.5rc0/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1874 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      433 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-13 23:05:38.000000 arize-7.0.5rc0/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-12 17:30:40.000000 arize-7.0.5rc0/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-06-13 23:05:38.673446 arize-7.0.5rc0/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-13 23:05:38.670941 arize-7.0.5rc0/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    49447 2023-06-12 17:30:40.000000 arize-7.0.5rc0/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-12 17:30:40.000000 arize-7.0.5rc0/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.347779 arize-7.0.6rc0/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-06-23 05:09:35.000000 arize-7.0.6rc0/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-06-23 05:09:35.000000 arize-7.0.6rc0/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-23 21:43:04.348231 arize-7.0.6rc0/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-06-23 05:09:35.000000 arize-7.0.6rc0/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.227032 arize-7.0.6rc0/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-06-23 21:42:13.000000 arize-7.0.6rc0/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    28894 2023-06-23 20:55:39.000000 arize-7.0.6rc0/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.249539 arize-7.0.6rc0/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.253717 arize-7.0.6rc0/arize/exporter/
+-rw-r--r--   0 kiko       (501) staff       (20)      146 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/exporter/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.277355 arize-7.0.6rc0/arize/exporter/core/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/exporter/core/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    10940 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/core/client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1343 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/core/query.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3464 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/core/session.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2406 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/publicexporter_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.286621 arize-7.0.6rc0/arize/exporter/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/exporter/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1422 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)      727 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5793 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 kiko       (501) staff       (20)      778 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/exporter/utils/validation.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.288909 arize-7.0.6rc0/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.304876 arize-7.0.6rc0/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6988 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.323799 arize-7.0.6rc0/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.327477 arize-7.0.6rc0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22779 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.330029 arize-7.0.6rc0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5090 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.335211 arize-7.0.6rc0/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    70456 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)    50888 2023-06-23 20:55:39.000000 arize-7.0.6rc0/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.344001 arize-7.0.6rc0/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      619 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5725 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    24659 2023-06-23 18:59:38.000000 arize-7.0.6rc0/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7620 2023-06-23 05:09:35.000000 arize-7.0.6rc0/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.237682 arize-7.0.6rc0/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-06-23 21:43:04.000000 arize-7.0.6rc0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1879 2023-06-23 21:43:04.000000 arize-7.0.6rc0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-23 21:43:04.000000 arize-7.0.6rc0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      481 2023-06-23 21:43:04.000000 arize-7.0.6rc0/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-06-23 21:43:04.000000 arize-7.0.6rc0/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-06-23 05:09:35.000000 arize-7.0.6rc0/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1571 2023-06-23 21:43:04.350031 arize-7.0.6rc0/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-23 21:43:04.346420 arize-7.0.6rc0/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    49474 2023-06-23 20:55:39.000000 arize-7.0.6rc0/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-06-23 05:09:35.000000 arize-7.0.6rc0/tests/test_utils.py
```

### Comparing `arize-7.0.5rc0/LICENSE.md` & `arize-7.0.6rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/PKG-INFO` & `arize-7.0.6rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.5rc0
+Version: 7.0.6rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.5rc0/README.md` & `arize-7.0.6rc0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/api.py` & `arize-7.0.6rc0/arize/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,25 +97,25 @@
             raise TypeError(f"space_key {space_key} is type {type(space_key)}, but must be a str")
         self._uri = f"{uri}/log"
         self._api_key = api_key
         self._space_key = space_key
         self._timeout = timeout
         self._session = FuturesSession(executor=BoundedExecutor(max_queue_bound, max_workers))
         # Grpc-Metadata prefix is required to pass non-standard md through via grpc-gateway
-        self._header = {
+        self._headers = {
             "authorization": api_key,
             "Grpc-Metadata-space": space_key,
             "Grpc-Metadata-sdk-language": "python",
             "Grpc-Metadata-language-version": get_python_version(),
             "Grpc-Metadata-sdk-version": __version__,
         }
         if additional_headers is not None:
-            if conflicting_keys := self._header.keys() & additional_headers.keys():
+            if conflicting_keys := self._headers.keys() & additional_headers.keys():
                 raise InvalidAdditionalHeaders(conflicting_keys)
-            self._header.update(additional_headers)
+            self._headers.update(additional_headers)
 
     def log(
         self,
         model_id: str,
         model_type: ModelTypes,
         environment: Environments,
         model_version: Optional[str] = None,
@@ -369,15 +369,15 @@
             environment_params=env_params,
         )
         return self._post(record=rec, uri=self._uri, indexes=None)
 
     def _post(self, record, uri, indexes):
         resp = self._session.post(
             uri,
-            headers=self._header,
+            headers=self._headers,
             timeout=self._timeout,
             json=MessageToDict(message=record, preserving_proto_field_name=True),
         )
         if indexes is not None and len(indexes) == 2:
             resp.starting_index = indexes[0]
             resp.ending_index = indexes[1]
         return resp
```

### Comparing `arize-7.0.5rc0/arize/bounded_executor.py` & `arize-7.0.6rc0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/examples/bulk_client.py` & `arize-7.0.6rc0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/examples/bulk_client_shap.py` & `arize-7.0.6rc0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/examples/client_shap_values.py` & `arize-7.0.6rc0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/examples/log_client.py` & `arize-7.0.6rc0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/examples/log_pandas_dataframe.py` & `arize-7.0.6rc0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/examples/preproduction_client.py` & `arize-7.0.6rc0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/exporter/core/client.py` & `arize-7.0.6rc0/arize/exporter/core/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,85 @@
+# type: ignore[pb2]
+from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional, Tuple
 
 import pandas as pd
 import pyarrow.parquet as pq
 from arize.utils.types import Environments
+from google.protobuf.timestamp_pb2 import Timestamp
 from pyarrow import flight
 from tqdm import tqdm
 
+from .. import publicexporter_pb2 as exp_pb2
+from ..utils.constants import (
+    ARIZE_PROFILE,
+    DEFAULT_ARIZE_FLIGHT_HOST,
+    DEFAULT_ARIZE_FLIGHT_PORT,
+    DEFAULT_CONFIG_PATH,
+    DEFAULT_PROFILE_NAME,
+    DEFAULT_TRANSPORT_SCHEME,
+)
 from ..utils.validation import Validator
-from .endpoint import Endpoint
+from .query import Query
 from .session import Session
 
 
+@dataclass
 class ArizeExportClient:
-    def __init__(
+    api_key: Optional[str] = None
+    arize_profile: str = ARIZE_PROFILE or DEFAULT_PROFILE_NAME
+    arize_config_path: Optional[str] = DEFAULT_CONFIG_PATH
+    host: str = DEFAULT_ARIZE_FLIGHT_HOST
+    port: int = DEFAULT_ARIZE_FLIGHT_PORT
+    scheme: str = DEFAULT_TRANSPORT_SCHEME
+
+    def __post_init__(
         self,
-        api_key: Optional[str] = None,
-        arize_profile: Optional[str] = None,
-        arize_config_path: Optional[str] = None,
-        host: Optional[str] = None,
-        port: Optional[int] = None,
     ) -> None:
-        """
+        f"""
         Initializes the Arize Export Client.
 
         Arguments:
         ----------
             api_key (str, optional): Arize provided personal API key associated with your user profile,
                 located on the API Explorer page. API key is required to initiate a new client, it can
                 be passed in explicitly, or set up as an environment variable or in profile file.
             arize_profile (str, optional): profile name for ArizeExportClient credentials and endpoint.
-                Defaults to 'default'.
+                Defaults to '{DEFAULT_PROFILE_NAME}'.
             arize_config_path (str, optional): path to the config file that stores ArizeExportClient
                 credentials and endpoint. Defaults to '~/.arize'.
             host (str, optional): URI endpoint host to send your export request to Arize AI. Defaults to
-                "https://flight.arize.com".
+                "{DEFAULT_ARIZE_FLIGHT_HOST}".
             port (int, optional): URI endpoint port to send your export request to Arize AI. Defaults to
-                443.
+                {DEFAULT_ARIZE_FLIGHT_PORT}.
         """
-        self._session = Session(api_key, arize_profile, arize_config_path, host, port)
-        self.done = False
+        self.__session = Session(
+            self.api_key,
+            self.arize_profile,
+            self.arize_config_path,
+            self.host,
+            self.port,
+            self.scheme,
+        )
 
-    def __call__(self, query: str) -> flight.FlightStreamReader:
-        arize_flight_endpoint = Endpoint(self._session)
-        flight_client = arize_flight_endpoint.connect()
-        reader = arize_flight_endpoint.execute_query(flight_client, query)
-        return reader
+    @property
+    def session(self) -> Session:
+        return self.__session
 
     def export_model_to_df(
         self,
         space_id: str,
         model_id: str,
         environment: Environments,
         start_time: datetime,
         end_time: datetime,
-        include_actuals: Optional[bool] = False,
-        model_version: Optional[str] = "",
-        batch_id: Optional[str] = "",
+        include_actuals: bool = False,
+        model_version: Optional[str] = None,
+        batch_id: Optional[str] = None,
     ) -> pd.DataFrame:
         """
         Exports data of a specific model in the Arize platform to a pandas dataframe for a defined
         time interval and model environment, optionally by model version and/or batch id.
 
         Arguments:
         ----------
@@ -70,29 +89,29 @@
                 tab in the Arize UI.
             environment (Environments): The environment for the model to export (can be Production,
                 Training, or Validation).
             start_time (datetime): The start time for the data to export for the model, start time
                 is inclusive. Time interval has hourly granularity.
             end_time (datetime): The end time for the data to export for the model, end time is not
                 inclusive. Time interval has hourly granularity.
-            include_actuals (bool, optional): An optional input to indicate whether to include actuals
+            include_actuals (bool): An optional input to indicate whether to include actuals
                 / ground truth in the data to export. `include_actuals` only applies to the Production
                 environment and defaults to 'False'.
             model_version (str, optional): An optional input to indicate the version of the model to
                 export. Model versions for all model environments can be found in the Datasets tab on
-                the model page in the Arize UI.
+                the model page in the Arize UI. Defaults to None.
             batch_id (str, optional): An optional input to indicate the batch name of the model to export.
                 Batches only apply to the Validation environment, and can be found in the Datasets tab on
-                the model page in the Arize UI.
+                the model page in the Arize UI. Defaults to None.
 
         Returns:
         --------
             A pandas dataframe
         """
-        stream_reader, num_recs = self.get_model_stream_reader(
+        stream_reader, num_recs = self._get_model_stream_reader(
             space_id=space_id,
             model_id=model_id,
             environment=environment,
             start_time=start_time,
             end_time=end_time,
             include_actuals=include_actuals,
             model_version=model_version,
@@ -101,35 +120,37 @@
         if stream_reader is None:
             return pd.DataFrame()
         progress_bar = self.get_progress_bar(num_recs)
         list_of_df = []
         while True:
             try:
                 flight_batch = stream_reader.read_chunk()
-                record_batch = flight_batch.data
-                data_to_pandas = record_batch.to_pandas()
-                list_of_df.append(data_to_pandas)
-                progress_bar.update(data_to_pandas.shape[0])
+                batch_df = flight_batch.data.to_pandas()
+                list_of_df.append(batch_df)
+                progress_bar.update(batch_df.shape[0])
             except StopIteration:
-                self.done = True
                 break
         progress_bar.close()
-        return pd.concat(list_of_df)
+        df = pd.concat(list_of_df)
+        null_columns = df.columns[df.isnull().all()]
+        df.drop(null_columns, axis=1, inplace=True)
+        df.sort_values(by=["time"], inplace=True)
+        return df.reset_index(drop=True)
 
     def export_model_to_parquet(
         self,
         path: str,
         space_id: str,
         model_id: str,
         environment: Environments,
         start_time: datetime,
         end_time: datetime,
-        include_actuals: Optional[bool] = False,
-        model_version: Optional[str] = "",
-        batch_id: Optional[str] = "",
+        include_actuals: bool = False,
+        model_version: Optional[str] = None,
+        batch_id: Optional[str] = None,
     ) -> None:
         """
         Exports data of a specific model in the Arize platform to a parquet file for a defined time
         interval and model environment, optionally by model version and/or batch id.
 
         Arguments:
         ----------
@@ -141,30 +162,30 @@
                 tab in the Arize UI.
             environment (Environments): The environment for the model to export (can be Production,
                 Training, or Validation).
             start_time (datetime): The start time for the data to export for the model, start time
                 is inclusive. Time interval has hourly granularity.
             end_time (datetime): The end time for the data to export for the model, end time is not
                 inclusive. Time interval has hourly granularity.
-            include_actuals (bool, optional): An optional input to indicate whether to include actuals
+            include_actuals (bool): An optional input to indicate whether to include actuals
                 / ground truth in the data to export. `include_actuals` only applies to the Production
                 environment and defaults to 'False'.
             model_version (str, optional): An optional input to indicate the version of the model to
                 export. Model versions for all model environments can be found in the Datasets tab on
-                the model page in the Arize UI.
+                the model page in the Arize UI. Defaults to None.
             batch_id (str, optional): An optional input to indicate the batch name of the model to export.
                 Batches only apply to the Validation environment, and can be found in the Datasets tab on
-                the model page in the Arize UI.
+                the model page in the Arize UI. Defaults to None.
 
         Returns:
         --------
             None
         """
         Validator.validate_input_type(path, "path", str)
-        stream_reader, num_recs = self.get_model_stream_reader(
+        stream_reader, num_recs = self._get_model_stream_reader(
             space_id=space_id,
             model_id=model_id,
             environment=environment,
             start_time=start_time,
             end_time=end_time,
             include_actuals=include_actuals,
             model_version=model_version,
@@ -177,55 +198,54 @@
             while True:
                 try:
                     flight_batch = stream_reader.read_chunk()
                     record_batch = flight_batch.data
                     writer.write_batch(record_batch)
                     progress_bar.update(record_batch.num_rows)
                 except StopIteration:
-                    self.done = True
                     break
         progress_bar.close()
 
-    def get_model_stream_reader(
+    def _get_model_stream_reader(
         self,
         space_id: str,
         model_id: str,
         environment: Environments,
         start_time: datetime,
         end_time: datetime,
-        include_actuals: Optional[bool] = False,
-        model_version: Optional[str] = "",
-        batch_id: Optional[str] = "",
+        include_actuals: bool = False,
+        model_version: Optional[str] = None,
+        batch_id: Optional[str] = None,
     ) -> Tuple[flight.FlightStreamReader, int]:
         Validator.validate_input_type(space_id, "space_id", str)
         Validator.validate_input_type(model_id, "model_id", str)
         Validator.validate_input_type(environment, "environment", Environments)
         Validator.validate_input_type(include_actuals, "include_actuals", bool)
         Validator.validate_input_type(start_time, "start_time", datetime)
         Validator.validate_input_type(end_time, "end_time", datetime)
         Validator.validate_input_type(model_version, "model_version", str)
         Validator.validate_input_type(batch_id, "batch_id", str)
+        Validator.validate_start_end_time(start_time, end_time)
 
-        if environment == Environments.PRODUCTION:
-            env = "PRODUCTION"
-        elif environment == Environments.TRAINING:
-            env = "TRAINING"
-        elif environment == Environments.VALIDATION:
-            env = "VALIDATION"
-        else:
-            raise TypeError("Invalid environment")
-
-        start_time_str = start_time.strftime("%Y-%m-%dT%H:%M:%SZ")
-        end_time_str = end_time.strftime("%Y-%m-%dT%H:%M:%SZ")
-        cmd = (
-            f'{{"spaceId":"{space_id}","modelId":"{model_id}", "environment":"{env}", '
-            f'"modelVersion":"{model_version}", "batchId":"{batch_id}", "startTime":"{start_time_str}", '
-            f'"endTime":"{end_time_str}", "includeActuals": {str(include_actuals).lower()}}}'
+        # Create query descriptor
+        query_descriptor = exp_pb2.RecordQueryDescriptor(
+            space_id=space_id,
+            model_id=model_id,
+            environment=environment.name,
+            model_version=model_version,
+            batch_id=batch_id,
+            include_actuals=include_actuals,
+            start_time=Timestamp(seconds=int(start_time.timestamp())),
+            end_time=Timestamp(seconds=int(end_time.timestamp())),
         )
-        return self(query=cmd)
+
+        flight_client = self.session.connect()
+        query = Query(query_descriptor)
+        reader = query.execute(flight_client, self.session.call_options)
+        return reader
 
     def get_progress_bar(self, num_recs):
         return tqdm(
             total=num_recs,
             desc=f"  exporting {num_recs} rows",
             bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt} [{elapsed}, {rate_fmt}{postfix}]",
             ncols=80,
```

### Comparing `arize-7.0.5rc0/arize/exporter/core/session.py` & `arize-7.0.6rc0/arize/exporter/core/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,91 @@
 import configparser
 import os
 import uuid
-from dataclasses import InitVar, dataclass, field
+from dataclasses import dataclass, field
+from typing import Optional
 
+from arize.__init__ import __version__
 from arize.utils.logging import logger
+from arize.utils.utils import get_python_version
 from pyarrow import flight
 
 from ..utils.constants import (
     ARIZE_API_KEY,
-    ARIZE_PROFILE,
     DEFAULT_ARIZE_API_KEY_CONFIG_KEY,
-    DEFAULT_ARIZE_FLIGHT_HOST,
-    DEFAULT_ARIZE_FLIGHT_PORT,
-    DEFAULT_CONFIG_PATH,
     DEFAULT_PACKAGE_NAME,
-    DEFAULT_PROFILE_NAME,
     PROFILE_FILE_NAME,
 )
 from ..utils.errors import InvalidConfigFileError, InvalidSessionError
 
 
 @dataclass
 class Session:
-    api_key: InitVar[str] = None
-    arize_profile: InitVar[str] = None
-    arize_config_path: InitVar[str] = DEFAULT_CONFIG_PATH
-    host: InitVar[str] = DEFAULT_ARIZE_FLIGHT_HOST
-    port: InitVar[int] = DEFAULT_ARIZE_FLIGHT_PORT
-    arize_api_key: str = field(init=False)
+    api_key: Optional[str]
+    arize_profile: str
+    arize_config_path: str
+    host: str
+    port: int
+    scheme: str
     session_name: str = field(init=False)
+    call_options: flight.FlightCallOptions = field(init=False)
 
-    def __post_init__(
-        self, api_key: str, arize_profile: str, arize_config_path: str, host: str, port: int
-    ):
-        self.headers = []
-        self.call_options = None
+    def __post_init__(self):
         self.session_name = f"python-sdk-{DEFAULT_PACKAGE_NAME}-{uuid.uuid4()}"
         logger.info(f"Creating named session as '{self.session_name}'.")
-        api_key = api_key or ARIZE_API_KEY
-        if api_key:
-            self.arize_api_key = api_key
-        else:
-            self._read_config(arize_profile, arize_config_path)
-
-        if host:
-            self.host = host
-        else:
-            self.host = DEFAULT_ARIZE_FLIGHT_HOST
-
-        if port:
-            self.port = port
-        else:
-            self.port = DEFAULT_ARIZE_FLIGHT_PORT
+        # If api_key is not passed, try reading from environment variable.
+        # If api_key is also not set as environment variable, read from config file
+        self.api_key = self.api_key or ARIZE_API_KEY or self._read_config()
+        if self.api_key is None:
+            logger.error(InvalidSessionError.error_message())
+            raise InvalidSessionError
 
         logger.debug(
-            f"Created session with Arize API Token '{self.arize_api_key}' at '{self.host}':'{self.port}'"
+            f"Created session with Arize API Token '{self.api_key}' at '{self.host}':'{self.port}'"
         )
+        self._set_headers()
 
-    def _read_config(self, arize_profile: str, arize_config_path: str):
-        arize_profile = arize_profile or ARIZE_PROFILE or DEFAULT_PROFILE_NAME
-        arize_config_path = arize_config_path or DEFAULT_CONFIG_PATH
-
+    def _read_config(self) -> Optional[str]:
         config_parser = Session._get_config_parser()
-        file_path = os.path.join(arize_config_path, PROFILE_FILE_NAME)
+        file_path = os.path.join(self.arize_config_path, PROFILE_FILE_NAME)
         logger.debug(
-            f"No provided connection details. Looking up session values from '{arize_profile}' in "
+            f"No provided connection details. Looking up session values from '{self.arize_profile}' in "
             f"'{file_path}'."
         )
         try:
             config_parser.read(file_path)
-            self.arize_api_key = config_parser.get(arize_profile, DEFAULT_ARIZE_API_KEY_CONFIG_KEY)
-        except configparser.NoSectionError:
-            raise InvalidSessionError(
-                "Credentials not provided or invalid. Please pass in the correct api_key when"
-                " initiating a new client or set up credentials in profile or as env variables"
-            )
+            return config_parser.get(self.arize_profile, DEFAULT_ARIZE_API_KEY_CONFIG_KEY)
+        except configparser.NoSectionError as err:
+            # Missing api key error is raised in the __post_init__ method
+            logger.warning(f"Can't extract API key from config file. {err.message}")
+            return None
         except Exception as err:
+            logger.error(InvalidConfigFileError.error_message())
             raise InvalidConfigFileError from err
 
     @staticmethod
     def _get_config_parser() -> configparser.ConfigParser:
         return configparser.ConfigParser()
 
     def connect(self) -> flight.FlightClient:
         """Connects to Arize Flight server public endpoint with the
         provided api key."""
         try:
-            # Default to use an unencrypted TCP connection.
-            scheme = "grpc+tls"
-            if self.host.lower() == "localhost":
-                disable_cert = True
-            else:
-                disable_cert = False
-            if self.arize_api_key:
-                client = flight.FlightClient(
-                    location=f"{scheme}://{self.host}:{self.port}",
-                    disable_server_verification=disable_cert,
-                )
-                self.headers.append((b"auth-token-bin", f"{self.arize_api_key}".encode("utf-8")))
-                self.call_options = flight.FlightCallOptions(timeout=600, headers=self.headers)
-                return client
-            raise ConnectionError("arize api key must be supplied.")
+            disable_cert = True if self.host.lower() == "localhost" else False
+            client = flight.FlightClient(
+                location=f"{self.scheme}://{self.host}:{self.port}",
+                disable_server_verification=disable_cert,
+            )
+            self.call_options = flight.FlightCallOptions(headers=self._headers)
+            return client
         except Exception:
             logger.error("There was an error trying to connect to the Arize Flight Endpoint")
             raise
+
+    def _set_headers(self) -> None:
+        self._headers = [
+            (b"origin", b"arize-python-exporter"),
+            (b"auth-token-bin", f"{self.api_key}".encode("utf-8")),
+            (b"sdk-language", b"python"),
+            (b"language-version", get_python_version().encode("utf-8")),
+            (b"sdk-version", __version__.encode("utf-8")),
+        ]
```

### Comparing `arize-7.0.5rc0/arize/exporter/utils/constants.py` & `arize-7.0.6rc0/arize/exporter/utils/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ARIZE_API_KEY = os.getenv("ARIZE_API_KEY")
 
 
 """Internal Use"""
 
 # Default API endpoint when not provided through env variable nor profile
 DEFAULT_ARIZE_FLIGHT_HOST = "flight.arize.com"
-DEFAULT_ARIZE_FLIGHT_PORT = "443"
+DEFAULT_ARIZE_FLIGHT_PORT = 443
 
 # Name of the current package.
 DEFAULT_PACKAGE_NAME = "arize_python_export_client"
 
 # Default config keys for the Arize config file. Created via the CLI.
 DEFAULT_ARIZE_API_KEY_CONFIG_KEY = "api_key"
 
@@ -37,7 +37,10 @@
 DEFAULT_CONFIG_PATH = os.path.join(str(Path.home()), ".arize")
 
 # Default initial wait time for retries in seconds.
 DEFAULT_RETRY_INITIAL_WAIT_TIME = 0.25
 
 # Default maximum wait time for retries in seconds.
 DEFAULT_RETRY_MAX_WAIT_TIME = 10.0
+
+# Default to use grpc + tls scheme.
+DEFAULT_TRANSPORT_SCHEME = "grpc+tls"
```

### Comparing `arize-7.0.5rc0/arize/exporter/utils/schema_parser.py` & `arize-7.0.6rc0/arize/exporter/utils/schema_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-from typing import Dict, Iterable, List, Optional
+from typing import Callable, Dict, Iterable, List, Optional
 
 import pandas as pd
 from arize.pandas.logger import Schema
 from arize.utils.types import EmbeddingColumnNames, ObjectDetectionColumnNames
 
 PREDICTION_ID_COL = "predictionID"
 TIME_COL = "time"
 
 
 def _get_suffix(suffix):
     return lambda colname: colname[-1 * len(suffix) :] == suffix
 
 
-def _get_colname(colname):
+def _get_prefix(prefix):
+    return lambda colname: colname[: len(prefix)] == prefix
+
+
+def _get_colname(colname) -> Callable:
     return lambda columns: colname if colname in columns else None
 
 
-# Helper functions for embeddings:
+# Helper functions for data types:
 is_vector = _get_suffix("__embVector")
 is_raw_data = _get_suffix("__rawData")
 is_link = _get_suffix("__linkToData")
 is_tag = _get_suffix("__tag")
+is_prompt = _get_prefix("prompt")
+is_response = _get_prefix("response")
 
 
 # Object detection columns:
 get_box_pred_scores = _get_colname("boxPredictionScores")
 get_box_pred_labels = _get_colname("boxPredictionLabel")
 
 get_box_actual_scores = _get_colname("boxActualScores")
@@ -47,49 +53,72 @@
 # Ranking columns:
 get_pred_group_id = _get_colname("predictionGroupID")
 get_ranking_category = _get_colname("ranking:category")
 get_ranking_relevance = _get_colname("ranking:relevance")
 get_ranking_label = _get_colname("ranking:label")
 get_rank = _get_colname("ranking:rank")
 
-# LLM
-get_prompt = _get_colname("prompt")
-get_response = _get_colname("response")
-
 
 def get_tags(df_columns: Iterable) -> List[str]:
     return [c for c in df_columns if is_tag(c)]
 
 
 def get_embedding_dict(
     vector_col_name: str, df_columns: Iterable[str]
 ) -> Dict[str, EmbeddingColumnNames]:
     embedding_dict = {"vector_column_name": vector_col_name}
 
-    prefix = vector_col_name[:-11]
+    prefix = vector_col_name.split("__embVector")[0]
     for other_col in df_columns:
         if prefix in other_col:
             if is_raw_data(other_col):
                 embedding_dict["data_column_name"] = other_col
             elif is_link(other_col):
                 embedding_dict["link_to_data_column_name"] = other_col
 
     return {prefix: EmbeddingColumnNames(**embedding_dict)}
 
 
 def get_embeddings(df_columns: Iterable[str]) -> Dict[str, EmbeddingColumnNames]:
     embed_dict = {}
     for col in df_columns:
-        if is_vector(col):
+        # We exclude prompt/response from embedding features
+        if is_vector(col) and not (is_prompt(col) or is_response(col)):
             single_embed = get_embedding_dict(col, df_columns)
             embed_dict = {**embed_dict, **single_embed}
 
     return embed_dict
 
 
+def _get_prompt_or_response(
+    prefix: str, df_columns: Iterable[str]
+) -> Optional[EmbeddingColumnNames]:
+    vec = _get_colname(f"{prefix}__embVector")(df_columns)
+    if vec is None:
+        return None
+
+    embedding_dict = {"vector_column_name": vec}
+    if f"{prefix}__rawData" in df_columns:
+        embedding_dict["data_column_name"] = _get_colname(f"{prefix}__rawData")(df_columns)
+    if f"{prefix}__linkToData" in df_columns:
+        embedding_dict["link_to_data_column_name"] = _get_colname(f"{prefix}__linkToData")(
+            df_columns
+        )
+
+    return EmbeddingColumnNames(**embedding_dict)
+
+
+def get_prompt(df_columns: Iterable[str]) -> Optional[EmbeddingColumnNames]:
+    return _get_prompt_or_response("prompt", df_columns)
+
+
+def get_response(df_columns: Iterable[str]) -> Optional[EmbeddingColumnNames]:
+    return _get_prompt_or_response("response", df_columns)
+
+
 def get_object_detection_prediction(cols: Iterable[str]) -> Optional[ObjectDetectionColumnNames]:
     if "boxPredictionCoordinates" in cols:
         return ObjectDetectionColumnNames(
             bounding_boxes_coordinates_column_name="boxPredictionCoordinates",
             categories_column_name=get_box_pred_labels(cols),
             scores_column_name=get_box_pred_scores(cols),
         )
```

### Comparing `arize-7.0.5rc0/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.6rc0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/embeddings/base_generators.py` & `arize-7.0.6rc0/arize/pandas/embeddings/base_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     from PIL import Image
     from transformers import (  # type: ignore
         AutoFeatureExtractor,
         AutoModel,
         AutoTokenizer,
         BatchEncoding,
     )
-    from transformers.utils import logging as transformer_logging  # type: ignore
+    from transformers.utils import logging as transformer_logging
 except ImportError:
     raise ImportError(IMPORT_ERROR_MESSAGE)
 
 transformer_logging.set_verbosity(50)
 transformer_logging.enable_progress_bar()
 
 
@@ -95,15 +95,15 @@
 
     @staticmethod
     def check_invalid_index(field: Union[pd.Series, pd.DataFrame]) -> None:
         if (field.index != field.reset_index(drop=True).index).any():
             if isinstance(field, pd.DataFrame):
                 raise err.InvalidIndexError("DataFrame")
             else:
-                raise err.InvalidIndexError(field.name)
+                raise err.InvalidIndexError(str(field.name))
 
     @abstractmethod
     def __repr__(self) -> str:
         pass
 
 
 class NLPEmbeddingGenerator(BaseEmbeddingGenerator):
```

### Comparing `arize-7.0.5rc0/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.6rc0/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/embeddings/errors.py` & `arize-7.0.6rc0/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/embeddings/models.py` & `arize-7.0.6rc0/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.6rc0/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.6rc0/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.6rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/logger.py` & `arize-7.0.6rc0/arize/pandas/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,28 +50,29 @@
                 "https://api.arize.com/v1".
             additional_headers (Dict[str, str], optional): Dictionary of additional headers to
                 append to request
         """
         self._api_key = api_key
         self._space_key = space_key
         self._files_uri = uri + "/pandas_arrow"
-        self._additional_headers = {}
+        self._headers = {
+            "authorization": self._api_key,
+            "space": self._space_key,
+            "sdk-language": "python",
+            "language-version": get_python_version(),
+            "sdk-version": __version__,
+            "sync": "0",  # Defaults to async logging
+        }
         if additional_headers is not None:
-            reserved_headers = {
-                "authorization",
-                "space",
-                "sdk-version",
-                "schema",
-                "sdk",
-                "python-version",
-                "sync",
-            }
+            reserved_headers = set(self._headers.keys())
+            # The header 'schema' is updated in the _post_file method
+            reserved_headers.add("schema")
             if conflicting_keys := reserved_headers & additional_headers.keys():
                 raise err.InvalidAdditionalHeaders(conflicting_keys)
-            self._additional_headers.update(additional_headers)
+            self._headers.update(additional_headers)
 
     def log(
         self,
         dataframe: pd.DataFrame,
         schema: Schema,
         environment: Environments,
         model_id: str,
@@ -221,14 +222,16 @@
 
         # pyarrow will err if a mixed type column exist in the dataset even if
         # the column is not specified in schema. Caveat: There may be other
         # error conditions that we're currently not aware of.
         try:
             if verbose:
                 logger.info("Getting pyarrow schema from pandas dataframe.")
+            # TODO: Addition of column for GENERATIVE models should occur at the
+            # beginning of the log function, so validations are applied to the resulting schema
             if (
                 model_type == ModelTypes.GENERATIVE_LLM
                 and schema.prediction_label_column_name is None
             ):
                 dataframe = self._add_default_prediction_label_column(dataframe)
                 schema = schema.replace(prediction_label_column_name="default_prediction_label")
             pa_schema = pa.Schema.from_pandas(dataframe)
@@ -432,21 +435,15 @@
         finally:
             if path is None:
                 f.close()
 
         try:
             logger.info(f"Success! Check out your data at {reconstruct_url(response)}")
 
-            if (
-                schema.prediction_score_column_name is None
-                and schema.prediction_label_column_name is None
-                and schema.rank_column_name is None
-                and schema.prediction_group_id_column_name is None
-                and schema.object_detection_prediction_column_names is None
-            ):
+            if not schema.has_prediction_columns():
                 logger.warning(
                     "Logging actuals without any predictions may result in "
                     "unexpected behavior if corresponding predictions have not been logged prior. "
                     "Please see the docs at https://docs.arize.com/arize/sending-data/sending-data-faq"
                     "#what-happens-after-i-send-in-actual-data"
                 )
 
@@ -459,30 +456,21 @@
         self,
         path: str,
         schema: bytes,
         sync: Optional[bool],
         timeout: Optional[float] = None,
     ) -> requests.Response:
         with open(path, "rb") as f:
-            headers = {
-                "authorization": self._api_key,
-                "space": self._space_key,
-                "schema": schema,
-                "sdk-language": "python",
-                "language-version": get_python_version(),
-                "sdk-version": __version__,
-            }
-            headers.update(self._additional_headers)
-            if sync:
-                headers["sync"] = "1"
+            self._headers.update({"schema": schema})
+            self._headers.update({"sync": "1" if sync is True else "0"})
             return requests.post(
                 self._files_uri,
                 timeout=timeout,
                 data=f,
-                headers=headers,
+                headers=self._headers,
             )
 
     def _add_default_prediction_label_column(self, df: pd.DataFrame) -> pd.DataFrame:
         df["default_prediction_label"] = [1] * len(df)
         return df
 
     def _remove_extraneous_columns(self, df: pd.DataFrame, schema: Schema) -> pd.DataFrame:
```

### Comparing `arize-7.0.5rc0/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.6rc0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 raise ValueError(
                     f"To calculate surrogate explainability for {model_type}, "
                     f"prediction scores must be between 0 and 1, but current "
                     f"prediction scores range from {_min} to {_max}."
                 )
 
             # model func requires 1 positional argument
-            def model_func(_):
+            def model_func(_):  # type: ignore
                 return np.column_stack((1 - y, y))
 
         elif model_type in NUMERIC_MODEL_TYPES:
             y_col_name = schema.prediction_label_column_name
             if schema.prediction_score_column_name is not None:
                 y_col_name = schema.prediction_score_column_name
             y = df[y_col_name].to_numpy()
@@ -73,15 +73,15 @@
                 raise ValueError(
                     f"To calculate surrogate explainability for {model_type}, "
                     f"predictions must not contain NaN or infinite values, but "
                     f"{len(y) - _finite_count} NaN or infinite value(s) are found in {y_col_name}."
                 )
 
             # model func requires 1 positional argument
-            def model_func(_):
+            def model_func(_):  # type: ignore
                 return y
 
         else:
             raise ValueError(
                 "Surrogate explainability is not supported for the specified "
                 f"model type {model_type}."
             )
```

### Comparing `arize-7.0.5rc0/arize/pandas/validation/errors.py` & `arize-7.0.6rc0/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/pandas/validation/validator.py` & `arize-7.0.6rc0/arize/pandas/validation/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from itertools import chain
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-import arize.pandas.validation.errors as err
 import numpy as np
 import pandas as pd
 import pyarrow as pa
+from arize.pandas.validation import errors as err
 from arize.utils.constants import (
     MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
     MAX_PAST_YEARS_FROM_CURRENT_TIME,
     MAX_PREDICTION_ID_LEN,
     MAX_TAG_LENGTH,
     MIN_PREDICTION_ID_LEN,
     MODEL_MAPPING_CONFIG,
@@ -56,15 +56,15 @@
         metric_families: Optional[List[Metrics]] = None,
         model_version: Optional[str] = None,
         batch_id: Optional[str] = None,
     ) -> List[err.ValidationError]:
         # general checks
         general_checks = chain(
             Validator._check_column_names_for_empty_strings(schema),
-            Validator._check_existence_prediction_id_column_delayed_schema(schema),
+            Validator._check_existence_prediction_id_column_delayed_schema(schema, model_type),
             Validator._check_invalid_model_id(model_id),
             Validator._check_invalid_model_version(model_version),
             Validator._check_invalid_model_type(model_type),
             Validator._check_invalid_environment(environment),
             Validator._check_invalid_batch_id(batch_id, environment),
             Validator._check_missing_columns(dataframe, schema),
             Validator._check_dataframe_for_duplicate_columns(schema, dataframe),
@@ -168,15 +168,15 @@
             Validator._check_value_timestamp(dataframe, schema),
             Validator._check_invalid_missing_values(dataframe, schema, model_type),
             Validator._check_id_field_str_length(
                 dataframe, "prediction_id_column_name", schema.prediction_id_column_name
             ),
             Validator._check_embedding_features_dimensionality(dataframe, schema),
             Validator._check_invalid_record_prod(dataframe, environment, schema, model_type),
-            Validator._check_invalid_record_training(dataframe, environment, schema, model_type),
+            Validator._check_invalid_record_preprod(dataframe, environment, schema, model_type),
             Validator._check_value_tag(dataframe, schema),
         )
         if model_type == ModelTypes.RANKING:
             r_checks = chain(
                 Validator._check_value_rank(dataframe, schema),
                 Validator._check_id_field_str_length(
                     dataframe,
@@ -266,17 +266,17 @@
 
     # ----------------
     # Parameter checks
     # ----------------
 
     @staticmethod
     def _check_model_type_and_metrics(
-        model_type: ModelTypes, metric_families: List[Metrics], schema: Schema
+        model_type: ModelTypes, metric_families: Optional[List[Metrics]], schema: Schema
     ) -> List[err.ValidationError]:
-        if not metric_families:
+        if metric_families is None:
             return []
 
         external_model_types = MODEL_MAPPING_CONFIG.get("external_model_types")
         if not external_model_types:
             return []
         if model_type.name.lower() not in external_model_types:
             # model_type is an old model type, e.g. SCORE_CATEGORICAL.
@@ -318,69 +318,78 @@
         required_columns_map: List[Dict[str, Any]],
     ) -> Tuple[bool, List[str], List[List[str]]]:
         missing_columns = []
         for item in required_columns_map:
             if model_type.name.lower() == item.get("external_model_type"):
                 is_valid_combination = False
                 metric_combinations = []
-                for mapping in item.get("mappings"):
-                    # This is a list of lists of metrics.
-                    # There may be a few metric combinations that map to the same column
-                    # enforcement rules.
-                    for metrics_list in mapping.get("metrics"):
-                        metric_combinations.append([metric.upper() for metric in metrics_list])
-                        if set(metrics_list) == set(
-                            metric_family.name.lower() for metric_family in metric_families
-                        ):
-                            # This is a valid combination of model type + metrics.
-                            # Now validate that required columns are in the schema.
-                            is_valid_combination = True
-                            # If no prediction values are present, then delayed actuals are being
-                            # logged, and we can't validate required columns.
-                            if schema.has_prediction_columns():
-                                # This is a list of lists.
-                                # In some cases, either one set of columns OR another set of
-                                # columns is required.
-                                required_columns = (
-                                    mapping.get("required_columns").get("arrow").get("required")
-                                )
-                                for column_combination in required_columns:
-                                    missing_columns = []
-                                    if None in {
-                                        getattr(schema, column, None)
-                                        for column in column_combination
-                                    }:
-                                        for column in column_combination:
-                                            if not getattr(schema, column, None):
-                                                missing_columns.append(column)
-                                    else:
-                                        break
+                mappings = item.get("mappings")
+                if mappings is not None:
+                    for mapping in mappings:
+                        # This is a list of lists of metrics.
+                        # There may be a few metric combinations that map to the same column
+                        # enforcement rules.
+                        for metrics_list in mapping.get("metrics"):
+                            metric_combinations.append([metric.upper() for metric in metrics_list])
+                            if set(metrics_list) == set(
+                                metric_family.name.lower() for metric_family in metric_families
+                            ):
+                                # This is a valid combination of model type + metrics.
+                                # Now validate that required columns are in the schema.
+                                is_valid_combination = True
+                                # If no prediction values are present, then delayed actuals are being
+                                # logged, and we can't validate required columns.
+                                if schema.has_prediction_columns():
+                                    # This is a list of lists.
+                                    # In some cases, either one set of columns OR another set of
+                                    # columns is required.
+                                    required_columns = (
+                                        mapping.get("required_columns").get("arrow").get("required")
+                                    )
+                                    for column_combination in required_columns:
+                                        missing_columns = []
+                                        if None in {
+                                            getattr(schema, column, None)
+                                            for column in column_combination
+                                        }:
+                                            for column in column_combination:
+                                                if not getattr(schema, column, None):
+                                                    missing_columns.append(column)
+                                        else:
+                                            break
                 if not is_valid_combination:
                     return False, [], metric_combinations
         return True, missing_columns, []
 
     @staticmethod
     def _check_existence_prediction_id_column_delayed_schema(
-        schema: Schema,
+        schema: Schema, model_type: ModelTypes
     ) -> List[err.MissingPredictionIdColumnForDelayedRecords]:
         if schema.prediction_id_column_name is not None:
             return []
-        if is_delayed_schema(schema):
+        # TODO: Revise logic once predicion_label column addition (for generative models)
+        # is moved to beginning of log function
+        if is_delayed_schema(schema) and model_type is not ModelTypes.GENERATIVE_LLM:
+            # We skip GENERATIVE model types since they are assigned a default
+            # prediction label column with values equal 1
             return [
                 err.MissingPredictionIdColumnForDelayedRecords(
                     schema.has_actual_columns(), schema.has_feature_importance_columns()
                 )
             ]
-        # Warning for when prediction_id is not provided by the user and we generate the default
-        # prediction ids
-        logger.warning(
-            "Prediction ID is not specified. Arize generates UUIDs for the model's predictions "
-            "if not provided by the user. Please note, you won't be able to send delayed data for "
-            "joining if a Prediction ID is not provided."
-        )
+        # We don't allow delayed actuals for generative models, since we give a default prediction
+        # label column with 1 as default value
+        if model_type is not ModelTypes.GENERATIVE_LLM:
+            # Warning for when prediction_id is not provided by the user and we generate the default
+            # prediction ids
+            logger.warning(
+                "Prediction ID is not specified. Arize generates UUIDs for the model's predictions "
+                "if not provided by the user. Please note, you won't be able to send delayed data for "
+                "joining if a Prediction ID is not provided."
+            )
 
         return []
 
     @staticmethod
     def _check_missing_columns(
         dataframe: pd.DataFrame,
         schema: Schema,
@@ -649,17 +658,17 @@
     @staticmethod
     def _check_dataframe_for_duplicate_columns(
         schema: Schema, dataframe: pd.DataFrame
     ) -> List[err.DuplicateColumnsInDataframe]:
         # Get the columns used in the schema
         schema_col_used = schema.get_used_columns()
         # Get the duplicated column names from the dataframe
-        df_duplicate_cols = dataframe.loc[:, dataframe.columns.duplicated()].columns.to_list()
+        duplicate_columns = dataframe.columns[dataframe.columns.duplicated()]
         # These are the duplicated columns from the dataframe that are referred to by the schema
-        schema_duplicate_cols = [col for col in df_duplicate_cols if col in schema_col_used]
+        schema_duplicate_cols = [col for col in duplicate_columns if col in schema_col_used]
         if schema_duplicate_cols:
             return [err.DuplicateColumnsInDataframe(schema_duplicate_cols)]
         return []
 
     # -----------
     # Type checks
     # -----------
@@ -1229,15 +1238,15 @@
         if schema.relevance_labels_column_name is not None:
             col = schema.relevance_labels_column_name
         elif schema.attributions_column_name is not None:
             col = schema.attributions_column_name
         else:
             col = schema.actual_label_column_name
         if col is not None and col in dataframe.columns and len(dataframe):
-            if dataframe[col].isnull().values.any():
+            if dataframe[col].isnull().values.any():  # type: ignore
                 # do not attach duplicated missing value error
                 # which would be caught by _check_value_missing
                 return []
             if dataframe[col].astype(str).str.len().min() == 0:
                 return [err.InvalidRankingCategoryValue(col)]
             # empty list
             not_null_filter = dataframe[col].notnull()
@@ -1256,15 +1265,15 @@
         # hitting the same check on server side, there's a some chance for a false
         # result, i.e. the check here suceeeds but the same check on server side fails.
         col = schema.timestamp_column_name
         if col is not None and col in dataframe.columns and len(dataframe):
             # When a timestamp column has Date and NaN, pyarrow will be fine, but
             # pandas min/max will fail due to type incompatibility. So we check for
             # missing value first.
-            if dataframe[col].isnull().values.any():
+            if dataframe[col].isnull().values.any():  # type: ignore
                 return [err.InvalidValueMissingValue("Prediction timestamp", "missing")]
 
             now_t = datetime.datetime.now()
             lbound, ubound = (
                 (
                     now_t - datetime.timedelta(days=MAX_PAST_YEARS_FROM_CURRENT_TIME * 365)
                 ).timestamp(),
@@ -1392,27 +1401,30 @@
                 schema.actual_label_column_name,
                 schema.actual_score_column_name,
                 schema.relevance_score_column_name,
                 schema.relevance_labels_column_name,
             ]
         else:
             columns_to_validate = []
-            # TODO: add separate logic for objective detection and generative model types
+        # TODO: add separate logic for objective detection and generative model types
 
         if schema.shap_values_column_names is not None:
             columns_to_validate.extend(list(schema.shap_values_column_names.values()))
 
         return Validator._check_invalid_record_helper(dataframe, columns_to_validate)
 
-    # _check_invalid_record_training validates there's not a single row in the dataframe
-    # with pred_label, pred_score all evaluates to null OR with actual_label, actual_score
-    # all evaluates to null and returns errors if either of the two cases exists
-    def _check_invalid_record_training(
+    @staticmethod
+    def _check_invalid_record_preprod(
         dataframe: pd.DataFrame, environment: Environments, schema: Schema, model_type: ModelTypes
     ) -> List[err.InvalidRecord]:
+        """
+        Validates there's not a single row in the dataframe with pred_label, pred_score all
+        evaluates to null OR with actual_label, actual_score all evaluates to null and returns
+        errors if either of the two cases exists
+        """
         if environment == Environments.PRODUCTION:
             return []
 
         if model_type in CATEGORICAL_MODEL_TYPES or model_type in NUMERIC_MODEL_TYPES:
             pred_columns_to_validate = [
                 schema.prediction_label_column_name,
                 schema.prediction_score_column_name,
@@ -1439,16 +1451,17 @@
             actual_columns_to_validate = []
             # TODO: add separate logic for objective detection and generative model types
 
         return Validator._check_invalid_record_helper(
             dataframe, pred_columns_to_validate
         ) + Validator._check_invalid_record_helper(dataframe, actual_columns_to_validate)
 
+    @staticmethod
     def _check_invalid_record_helper(
-        dataframe: pd.DataFrame, column_names: List[str]
+        dataframe: pd.DataFrame, column_names: List[Optional[str]]
     ) -> List[err.InvalidRecord]:
         """
         This function checks that there are no null values in a subset of columns,
         returning an error if so. The column subset is computed from the input list of
         columns `column_names` that are not None and that are present in the dataframe
 
         Returns:
@@ -1461,15 +1474,15 @@
                 columns_subset.append(col)
         if len(columns_subset) == 0:
             return []
         null_filter = dataframe[columns_subset].isnull().all(axis=1)
         null_index = null_filter[null_filter].index.values
         if len(null_index) == 0:
             return []
-        return [err.InvalidRecord(columns_subset, null_index)]
+        return [err.InvalidRecord(columns_subset, null_index)]  # type: ignore
 
     @staticmethod
     def _check_type_prediction_group_id(
         schema: Schema, column_types: Dict[str, Any]
     ) -> List[err.InvalidType]:
         col = schema.prediction_group_id_column_name
         if col in column_types:
```

### Comparing `arize-7.0.5rc0/arize/public_pb2.py` & `arize-7.0.6rc0/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/utils/constants.py` & `arize-7.0.6rc0/arize/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/utils/logging.py` & `arize-7.0.6rc0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/utils/model_mapping.json` & `arize-7.0.6rc0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize/utils/types.py` & `arize-7.0.6rc0/arize/utils/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,19 +106,19 @@
         """
 
         if self.vector is not None:
             self._validate_embedding_vector(emb_name)
 
         # Validate embedding raw data, if present
         if self.data is not None:
-            self._validate_embedding_data(emb_name)
+            self._validate_embedding_data(emb_name, self.data)
 
         # Validate embedding link to data, if present
         if self.link_to_data is not None:
-            self._validate_embedding_link_to_data(emb_name)
+            self._validate_embedding_link_to_data(emb_name, self.link_to_data)
 
         return None
 
     def _validate_embedding_vector(
         self,
         emb_name: Union[str, int, float],
     ) -> None:
@@ -141,70 +141,76 @@
             raise TypeError(
                 f'Embedding feature "{emb_name}" has vector type {type(self.vector)}. Must be '
                 f"list, "
                 f"np.ndarray or pd.Series"
             )
         # Fail if not all elements in list are floats
         allowed_types = (int, float, np.int16, np.int32, np.float16, np.float32)
-        if not all(isinstance(val, allowed_types) for val in self.vector):
+        if not all(isinstance(val, allowed_types) for val in self.vector):  # type: ignore
             raise TypeError(
                 f"Embedding vector must be a vector of integers and/or floats. Got "
                 f"{emb_name}.vector = {self.vector}"
             )
         # Fail if the length of the vector is 1
         if len(self.vector) == 1:
             raise ValueError("Embedding vector must not have a size of 1")
 
+    @staticmethod
     def _validate_embedding_data(
-        self,
-        emb_name: Union[str, int, float],
+        emb_name: Union[str, int, float], data: Union[str, List[str]]
     ) -> None:
         """
         Validates that the embedding raw data field is of the correct format. That is:
             1. Must be string or list of strings (NLP case)
 
         Arguments:
         ----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
+            data (str, int, float): Raw data associated with the embedding feature. Typically raw text.
 
         Raises:
         -------
             TypeError: If the embedding does not satisfy requirements above
         """
         # Validate that data is a string or iterable of strings
-        is_string = isinstance(self.data, str)
-        is_allowed_iterable = not is_string and Embedding._is_valid_iterable(self.data)
+        is_string = isinstance(data, str)
+        is_allowed_iterable = not is_string and Embedding._is_valid_iterable(data)
         if not (is_string or is_allowed_iterable):
             raise TypeError(
                 f'Embedding feature "{emb_name}" data field must be str, list, np.ndarray or '
                 f"pd.Series"
             )
 
         if is_allowed_iterable:
             # Fail if not all elements in iterable are strings
-            if not all(isinstance(val, str) for val in self.data):
+            if not all(isinstance(val, str) for val in data):
                 raise TypeError("Embedding data field must contain strings")
 
-    def _validate_embedding_link_to_data(self, emb_name: Union[str, int, float]) -> None:
+    @staticmethod
+    def _validate_embedding_link_to_data(
+        emb_name: Union[str, int, float], link_to_data: str
+    ) -> None:
         """
         Validates that the embedding link to data field is of the correct format. That is:
             1. Must be string
 
         Arguments:
         ----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
+            link_to_data (str): Link to source data of embedding feature, typically an image file on
+                cloud storage
 
         Raises:
         -------
             TypeError: If the embedding does not satisfy requirements above
         """
-        if not isinstance(self.link_to_data, str):
+        if not isinstance(link_to_data, str):
             raise TypeError(
                 f'Embedding feature "{emb_name}" link_to_data field must be str and got '
-                f"{type(self.link_to_data)}"
+                f"{type(link_to_data)}"
             )
 
     @staticmethod
     def _is_valid_iterable(data: Union[str, List[str], List[float], np.ndarray, pd.Series]) -> bool:
         """
         Validates that the input data field is of the correct iterable type. That is:
             1. List or
@@ -233,15 +239,15 @@
     Arguments:
     ----------
         bounding_boxes_coordinates_column_name (str): Column name containing the coordinates of the
             rectangular outline that locates an object within an image or video. Pascal VOC format
             required. The contents of this column must be a List[List[float]].
         categories_column_name (str): Column name containing the predefined classes or labels used
             by the model to classify the detected objects. The contents of this column must be List[str].
-        scores_column_names (str, optional): Column name containint the confidence scores that the
+        scores_column_names (str, optional): Column name containing the confidence scores that the
             model assigns to it's predictions, indicating how certain the model is that the predicted
             class is contained within the bounding box. This argument is only applicable for prediction
             values. The contents of this column must be List[float].
     """
 
 
 class ObjectDetectionLabel(NamedTuple):
@@ -386,27 +392,29 @@
 class RankingActualLabel(NamedTuple):
     relevance_labels: Optional[List[str]] = None
     relevance_score: Optional[float] = None
 
     def validate(self):
         # Validate relevance_labels type
         if self.relevance_labels is not None:
-            self._validate_relevance_labels()
+            self._validate_relevance_labels(self.relevance_labels)
         # Validate relevance score type
         if self.relevance_score is not None:
-            self._validate_relevance_score()
+            self._validate_relevance_score(self.relevance_score)
 
-    def _validate_relevance_labels(self):
-        if not is_list_of(self.relevance_labels, str):
+    @staticmethod
+    def _validate_relevance_labels(relevance_labels: List[str]):
+        if not is_list_of(relevance_labels, str):
             raise TypeError("Actual Relevance Labels must be a list of strings")
-        if any(label == "" for label in self.relevance_labels):
+        if any(label == "" for label in relevance_labels):
             raise ValueError("Actual Relevance Labels must be not contain empty strings")
 
-    def _validate_relevance_score(self):
-        if not isinstance(self.relevance_score, (float, int)):
+    @staticmethod
+    def _validate_relevance_score(relevance_score: float):
+        if not isinstance(relevance_score, (float, int)):
             raise TypeError("Actual Relevance score must be a float or an int")
 
 
 @dataclass(frozen=True)
 class Schema:
     prediction_id_column_name: Optional[str] = None
     feature_column_names: Optional[List[str]] = None
@@ -468,18 +476,18 @@
             ground truth values. The content of this column must be a string.
         object_detection_prediction_column_names (ObjectDetectionColumnNames, optional):
             ObjectDetectionColumnNames object containing information defining the predicted bounding
             boxes' coordinates, categories, and scores.
         object_detection_actual_column_names (ObjectDetectionColumnNames, optional):
             ObjectDetectionColumnNames object containing information defining the actual bounding
             boxes' coordinates, categories, and scores.
-        prompt_column_names (EmbeddingCoulumnNames, optional): EmbeddingCoulumnNames object containing
+        prompt_column_names (EmbeddingColumnNames, optional): EmbeddingColumnNames object containing
             the embedding vector data (required) and raw text (optional) for the input text your
             model acts on.
-        response_column_names (EmbeddingCoulumnNames, optional): EmbeddingCoulumnNames object
+        response_column_names (EmbeddingColumnNames, optional): EmbeddingColumnNames object
             containing the embedding vector data (required) and raw text (optional) for the text
             your model generates.
 
     Methods:
     --------
         replace(**changes):
             Replaces fields of the schema
```

### Comparing `arize-7.0.5rc0/arize/utils/utils.py` & `arize-7.0.6rc0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.5rc0/arize.egg-info/PKG-INFO` & `arize-7.0.6rc0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.5rc0
+Version: 7.0.6rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.5rc0/arize.egg-info/SOURCES.txt` & `arize-7.0.6rc0/arize.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 arize/examples/bulk_client.py
 arize/examples/bulk_client_shap.py
 arize/examples/client_shap_values.py
 arize/examples/log_client.py
 arize/examples/log_pandas_dataframe.py
 arize/examples/preproduction_client.py
 arize/exporter/__init__.py
+arize/exporter/publicexporter_pb2.py
 arize/exporter/core/__init__.py
 arize/exporter/core/client.py
-arize/exporter/core/endpoint.py
 arize/exporter/core/query.py
 arize/exporter/core/session.py
 arize/exporter/utils/__init__.py
 arize/exporter/utils/constants.py
 arize/exporter/utils/errors.py
 arize/exporter/utils/schema_parser.py
 arize/exporter/utils/validation.py
```

### Comparing `arize-7.0.5rc0/setup.cfg` & `arize-7.0.6rc0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -29,22 +29,24 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	requests_futures==1.0.0
 	googleapis_common_protos~=1.51
-	protobuf>=3.12, <5
+	protobuf>=3.12,<5
 	pandas>=0.25.3,<2
 	pyarrow>=5.0.0
+	tqdm>=4.60.0,<5
 
 [options.extras_require]
 MimicExplainer = 
 	numpy<1.24.0
 	scikit-learn>=0.12.0,<2
+	interpret-core[required]==0.2.7
 	interpret>=0.2.7,<1
 	interpret-community>=0.22.0,<1
 	lightgbm>=2.2.3,<4
 AutoEmbeddings = 
 	transformers>=4.25, <5
 	tokenizers>=0.13, <1
 	datasets>=2.8, <3
```

### Comparing `arize-7.0.5rc0/tests/test_api.py` & `arize-7.0.6rc0/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 from pathlib import Path
 
 import arize.public_pb2 as pb2
 import numpy as np
 import pandas as pd
 import pytest
+from arize import __version__ as arize_version
 from arize.api import Client, Embedding
 from arize.pandas.validation.errors import InvalidAdditionalHeaders
 from arize.utils.constants import (
     MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
     MAX_PAST_YEARS_FROM_CURRENT_TIME,
     MAX_PREDICTION_ID_LEN,
     MAX_TAG_LENGTH,
@@ -1277,22 +1278,21 @@
         "Found invalid additional header, cannot use reserved headers named: authorization."
         in str(excinfo.value)
     )
 
 
 def test_instantiating_client_additional_header():
     c = get_stubbed_client({"JWT": "FAKE_VALUE"})
-    import arize
 
     expected = {
         "authorization": inputs["api_key"],
         "Grpc-Metadata-space": inputs["space_key"],
         "Grpc-Metadata-sdk-language": "python",
         "Grpc-Metadata-language-version": get_python_version(),
-        "Grpc-Metadata-sdk-version": arize.__version__,
+        "Grpc-Metadata-sdk-version": arize_version,
         "JWT": "FAKE_VALUE",
     }
-    assert c._header == expected
+    assert c._headers == expected
 
 
 if __name__ == "__main__":
     raise SystemExit(pytest.main([__file__]))
```

### Comparing `arize-7.0.5rc0/tests/test_utils.py` & `arize-7.0.6rc0/tests/test_utils.py`

 * *Files identical despite different names*

