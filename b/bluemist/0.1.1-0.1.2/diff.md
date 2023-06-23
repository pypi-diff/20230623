# Comparing `tmp/bluemist-0.1.1.tar.gz` & `tmp/bluemist-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluemist-0.1.1.tar", last modified: Sun Feb 26 19:41:13 2023, max compression
+gzip compressed data, was "bluemist-0.1.2.tar", last modified: Fri Jun 23 10:58:25 2023, max compression
```

## Comparing `bluemist-0.1.1.tar` & `bluemist-0.1.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.679382 bluemist-0.1.1/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1068 2023-02-18 08:16:06.000000 bluemist-0.1.1/LICENSE
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      212 2023-02-25 02:11:51.000000 bluemist-0.1.1/MANIFEST.in
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4988 2023-02-26 19:41:13.679382 bluemist-0.1.1/PKG-INFO
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     3494 2023-02-26 19:21:49.000000 bluemist-0.1.1/README.md
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.655382 bluemist-0.1.1/bluemist/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      214 2023-02-18 08:18:03.000000 bluemist-0.1.1/bluemist/__init__.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.643382 bluemist-0.1.1/bluemist/artifacts/
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.659382 bluemist-0.1.1/bluemist/artifacts/api/
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.659382 bluemist-0.1.1/bluemist/artifacts/api/__pycache__/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      175 2023-02-26 19:40:15.000000 bluemist-0.1.1/bluemist/artifacts/api/__pycache__/predict.cpython-39.pyc
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:40:16.000000 bluemist-0.1.1/bluemist/artifacts/api/predict.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.659382 bluemist-0.1.1/bluemist/artifacts/logs/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    11024 2023-02-26 19:40:16.000000 bluemist-0.1.1/bluemist/artifacts/logs/bluemist.log
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    11271 2023-02-26 19:40:12.000000 bluemist-0.1.1/bluemist/artifacts/logs/bluemist.log.1
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1471 2023-02-26 19:39:56.000000 bluemist-0.1.1/bluemist/artifacts/logs/bluemist.log.2
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.659382 bluemist-0.1.1/bluemist/classification/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2022-06-19 06:15:36.000000 bluemist-0.1.1/bluemist/classification/__init__.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.643382 bluemist-0.1.1/bluemist/datasets/
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.663382 bluemist-0.1.1/bluemist/datasets/auto-mpg/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      161 2022-06-19 06:26:43.000000 bluemist-0.1.1/bluemist/datasets/auto-mpg/Index
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    18131 2023-01-22 08:20:03.000000 bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.csv
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    30286 2022-06-19 06:26:45.000000 bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.data
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    32149 2022-06-19 06:26:46.000000 bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.data-original
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1660 2022-06-19 06:26:47.000000 bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.names
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.667382 bluemist-0.1.1/bluemist/datasource/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      184 2023-02-06 07:11:36.000000 bluemist-0.1.1/bluemist/datasource/__init__.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2043 2023-02-26 07:03:38.000000 bluemist-0.1.1/bluemist/datasource/aws.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      146 2023-02-18 07:23:39.000000 bluemist-0.1.1/bluemist/datasource/azure.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4578 2023-02-26 07:07:19.000000 bluemist-0.1.1/bluemist/datasource/database.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1650 2023-02-26 07:05:50.000000 bluemist-0.1.1/bluemist/datasource/file.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      153 2023-02-18 07:24:04.000000 bluemist-0.1.1/bluemist/datasource/gcp.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.671382 bluemist-0.1.1/bluemist/eda/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)       83 2023-02-13 08:49:20.000000 bluemist-0.1.1/bluemist/eda/__init__.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     3188 2023-02-25 05:49:59.000000 bluemist-0.1.1/bluemist/eda/analyze_data.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     3872 2023-02-24 22:35:31.000000 bluemist-0.1.1/bluemist/environment.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      482 2023-02-19 23:48:31.000000 bluemist-0.1.1/bluemist/logging.config
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4271 2023-02-26 19:40:07.000000 bluemist-0.1.1/bluemist/main.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.671382 bluemist-0.1.1/bluemist/pipeline/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      207 2023-02-18 07:24:27.000000 bluemist-0.1.1/bluemist/pipeline/__init__.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1798 2023-02-18 07:24:21.000000 bluemist-0.1.1/bluemist/pipeline/bluemist_pipeline.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.675382 bluemist-0.1.1/bluemist/preprocessing/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      214 2023-02-18 07:24:35.000000 bluemist-0.1.1/bluemist/preprocessing/__init__.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2405 2023-02-18 07:24:40.000000 bluemist-0.1.1/bluemist/preprocessing/categorical_transformer.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2058 2023-02-18 07:24:47.000000 bluemist-0.1.1/bluemist/preprocessing/numeric_transformer.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    10689 2023-02-22 03:21:09.000000 bluemist-0.1.1/bluemist/preprocessing/preprocessor.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.675382 bluemist-0.1.1/bluemist/regression/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      310 2023-02-18 07:25:01.000000 bluemist-0.1.1/bluemist/regression/__init__.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      455 2023-02-18 07:25:06.000000 bluemist-0.1.1/bluemist/regression/constant.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    17473 2023-02-26 19:35:00.000000 bluemist-0.1.1/bluemist/regression/regressor.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.675382 bluemist-0.1.1/bluemist/regression/tuning/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      160 2023-02-18 07:25:19.000000 bluemist-0.1.1/bluemist/regression/tuning/__init__.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    10266 2023-02-25 06:41:00.000000 bluemist-0.1.1/bluemist/regression/tuning/constant.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.675382 bluemist-0.1.1/bluemist/tests/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-04 21:21:02.000000 bluemist-0.1.1/bluemist/tests/__init__.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.679382 bluemist-0.1.1/bluemist/utils/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-04 04:35:53.000000 bluemist-0.1.1/bluemist/utils/__init__.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2502 2023-02-22 11:51:48.000000 bluemist-0.1.1/bluemist/utils/generate_api.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     3094 2023-02-06 06:57:33.000000 bluemist-0.1.1/bluemist/utils/metrics.py
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      562 2023-01-22 03:36:45.000000 bluemist-0.1.1/bluemist/utils/scaler.py
-drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-26 19:41:13.655382 bluemist-0.1.1/bluemist.egg-info/
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4988 2023-02-26 19:41:13.000000 bluemist-0.1.1/bluemist.egg-info/PKG-INFO
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1564 2023-02-26 19:41:13.000000 bluemist-0.1.1/bluemist.egg-info/SOURCES.txt
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        1 2023-02-26 19:41:13.000000 bluemist-0.1.1/bluemist.egg-info/dependency_links.txt
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      337 2023-02-26 19:41:13.000000 bluemist-0.1.1/bluemist.egg-info/requires.txt
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        9 2023-02-26 19:41:13.000000 bluemist-0.1.1/bluemist.egg-info/top_level.txt
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)       80 2023-02-25 05:50:51.000000 bluemist-0.1.1/requirements-optional.txt
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      243 2023-02-25 06:11:53.000000 bluemist-0.1.1/requirements.txt
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      500 2023-02-26 19:41:13.683382 bluemist-0.1.1/setup.cfg
--rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      399 2023-02-25 05:51:28.000000 bluemist-0.1.1/setup.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.010639 bluemist-0.1.2/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1073 2023-06-21 09:29:13.000000 bluemist-0.1.2/LICENSE
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      212 2023-02-25 02:11:51.000000 bluemist-0.1.2/MANIFEST.in
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     8205 2023-06-23 10:58:25.014639 bluemist-0.1.2/PKG-INFO
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     6706 2023-06-23 10:32:10.000000 bluemist-0.1.2/README.md
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.986639 bluemist-0.1.2/bluemist/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      214 2023-02-18 08:18:03.000000 bluemist-0.1.2/bluemist/__init__.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.974639 bluemist-0.1.2/bluemist/artifacts/
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.990639 bluemist-0.1.2/bluemist/artifacts/api/
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.990639 bluemist-0.1.2/bluemist/artifacts/api/__pycache__/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      175 2023-06-23 10:47:03.000000 bluemist-0.1.2/bluemist/artifacts/api/__pycache__/predict.cpython-39.pyc
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:38:08.000000 bluemist-0.1.2/bluemist/artifacts/api/predict.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.990639 bluemist-0.1.2/bluemist/artifacts/logs/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:55:09.000000 bluemist-0.1.2/bluemist/artifacts/logs/bluemist.log
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.990639 bluemist-0.1.2/bluemist/classification/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2022-06-19 06:15:36.000000 bluemist-0.1.2/bluemist/classification/__init__.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.974639 bluemist-0.1.2/bluemist/datasets/
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.994639 bluemist-0.1.2/bluemist/datasets/auto-mpg/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      161 2022-06-19 06:26:43.000000 bluemist-0.1.2/bluemist/datasets/auto-mpg/Index
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    18131 2023-01-22 08:20:03.000000 bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.csv
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    30286 2022-06-19 06:26:45.000000 bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.data
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    32149 2022-06-19 06:26:46.000000 bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.data-original
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1660 2022-06-19 06:26:47.000000 bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.names
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.998639 bluemist-0.1.2/bluemist/datasource/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      184 2023-02-06 07:11:36.000000 bluemist-0.1.2/bluemist/datasource/__init__.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2043 2023-02-26 07:03:38.000000 bluemist-0.1.2/bluemist/datasource/aws.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      146 2023-02-18 07:23:39.000000 bluemist-0.1.2/bluemist/datasource/azure.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4578 2023-02-26 07:07:19.000000 bluemist-0.1.2/bluemist/datasource/database.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1710 2023-06-18 09:07:22.000000 bluemist-0.1.2/bluemist/datasource/file.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      153 2023-02-18 07:24:04.000000 bluemist-0.1.2/bluemist/datasource/gcp.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.002639 bluemist-0.1.2/bluemist/eda/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)       83 2023-02-13 08:49:20.000000 bluemist-0.1.2/bluemist/eda/__init__.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     3188 2023-02-25 05:49:59.000000 bluemist-0.1.2/bluemist/eda/analyze_data.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     6724 2023-06-22 09:27:08.000000 bluemist-0.1.2/bluemist/environment.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      482 2023-02-19 23:48:31.000000 bluemist-0.1.2/bluemist/logging.config
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4492 2023-06-23 08:54:24.000000 bluemist-0.1.2/bluemist/main.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4492 2023-06-23 08:54:24.000000 bluemist-0.1.2/bluemist/main_predict.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.002639 bluemist-0.1.2/bluemist/pipeline/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      207 2023-02-18 07:24:27.000000 bluemist-0.1.2/bluemist/pipeline/__init__.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1798 2023-02-18 07:24:21.000000 bluemist-0.1.2/bluemist/pipeline/bluemist_pipeline.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.006639 bluemist-0.1.2/bluemist/preprocessing/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      214 2023-02-18 07:24:35.000000 bluemist-0.1.2/bluemist/preprocessing/__init__.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2270 2023-06-04 07:35:21.000000 bluemist-0.1.2/bluemist/preprocessing/categorical_transformer.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2128 2023-06-19 08:13:43.000000 bluemist-0.1.2/bluemist/preprocessing/numeric_transformer.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    11119 2023-06-11 07:40:08.000000 bluemist-0.1.2/bluemist/preprocessing/preprocessor.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.006639 bluemist-0.1.2/bluemist/regression/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      382 2023-06-04 07:35:21.000000 bluemist-0.1.2/bluemist/regression/__init__.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      455 2023-02-18 07:25:06.000000 bluemist-0.1.2/bluemist/regression/constant.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    21315 2023-06-23 08:51:29.000000 bluemist-0.1.2/bluemist/regression/regressor.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.010639 bluemist-0.1.2/bluemist/regression/tuning/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      199 2023-06-04 07:35:21.000000 bluemist-0.1.2/bluemist/regression/tuning/__init__.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     4899 2023-06-18 09:08:57.000000 bluemist-0.1.2/bluemist/regression/tuning/cuml.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)    10311 2023-06-18 09:08:58.000000 bluemist-0.1.2/bluemist/regression/tuning/sklearn.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.010639 bluemist-0.1.2/bluemist/tests/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-04 21:21:02.000000 bluemist-0.1.2/bluemist/tests/__init__.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:25.010639 bluemist-0.1.2/bluemist/utils/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-02-04 04:35:53.000000 bluemist-0.1.2/bluemist/utils/__init__.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      334 2023-06-20 06:42:29.000000 bluemist-0.1.2/bluemist/utils/constants.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     2642 2023-06-19 07:47:08.000000 bluemist-0.1.2/bluemist/utils/generate_api.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     3545 2023-06-19 06:56:00.000000 bluemist-0.1.2/bluemist/utils/metrics.py
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      495 2023-06-11 10:54:47.000000 bluemist-0.1.2/bluemist/utils/scaler.py
+drwxrwxr-x   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        0 2023-06-23 10:58:24.990639 bluemist-0.1.2/bluemist.egg-info/
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     8205 2023-06-23 10:58:24.000000 bluemist-0.1.2/bluemist.egg-info/PKG-INFO
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)     1573 2023-06-23 10:58:24.000000 bluemist-0.1.2/bluemist.egg-info/SOURCES.txt
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        1 2023-06-23 10:58:24.000000 bluemist-0.1.2/bluemist.egg-info/dependency_links.txt
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      418 2023-06-23 10:58:24.000000 bluemist-0.1.2/bluemist.egg-info/requires.txt
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)        9 2023-06-23 10:58:24.000000 bluemist-0.1.2/bluemist.egg-info/top_level.txt
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)       95 2023-06-23 10:39:49.000000 bluemist-0.1.2/requirements-optional.txt
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      311 2023-06-23 10:39:55.000000 bluemist-0.1.2/requirements.txt
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      500 2023-06-23 10:58:25.014639 bluemist-0.1.2/setup.cfg
+-rw-rw-r--   0 shashank-agrawal  (1000) shashank-agrawal  (1000)      399 2023-02-25 05:51:28.000000 bluemist-0.1.2/setup.py
```

### Comparing `bluemist-0.1.1/LICENSE` & `bluemist-0.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Bluemist AI
+Copyright (c) 2022-2023 Bluemist AI
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.csv` & `bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.csv`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.data` & `bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.data-original` & `bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.data-original`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/datasets/auto-mpg/auto-mpg.names` & `bluemist-0.1.2/bluemist/datasets/auto-mpg/auto-mpg.names`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/datasource/aws.py` & `bluemist-0.1.2/bluemist/datasource/aws.py`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/datasource/database.py` & `bluemist-0.1.2/bluemist/datasource/database.py`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/datasource/file.py` & `bluemist-0.1.2/bluemist/datasource/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
-__author__ = "Shashank Agrawal"
-__license__ = "MIT"
-__version__ = "0.1.1"
-__email__ = "dew@bluemist-ai.one"
+# Author: Shashank Agrawal
+# License: MIT
+# Version: 0.1.2
+# Email: dew@bluemist-ai.one
+# Created:  Jun 22, 2022
+# Last modified: June 17, 2023
 
 
 import logging
 import os
 from logging import config
 import pandas as pd
 
@@ -41,16 +43,16 @@
     """
 
     logger.info('Pulling data from {}'.format(file_path))
 
     if file_type == 'delimited':
         data = pd.read_csv(filepath_or_buffer=file_path, sep=delimiter)
         logger.info('Data pull completed !!')
-        data.columns = data.columns.str.replace('\W', '_')  # TODO: Revisit this code
+        data.columns = data.columns.str.replace('\W', '_', regex=True)  # TODO: Revisit this code
         return data
     elif file_type == 'excel':
         data = pd.read_excel(io=file_path, sheet_name=sheet_name)
         logger.info('Data pull completed !!')
-        data.columns = data.columns.str.replace('\W', '_')  # TODO: Revisit this code
+        data.columns = data.columns.str.replace('\W', '_', regex=True)  # TODO: Revisit this code
         return data
```

### Comparing `bluemist-0.1.1/bluemist/eda/analyze_data.py` & `bluemist-0.1.2/bluemist/eda/analyze_data.py`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/main.py` & `bluemist-0.1.2/bluemist/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import logging
 import os
 import sys
 from logging import config
 
 import sklearn
+import cpuinfo
+import sklearnex
+#import cuml
+from sklearnex import patch_sklearn, sklearn_is_patched
+
+#patch_sklearn()
+
 from sklearn import datasets
 
-from bluemist.environment import initialize
+from bluemist.environment import initialize, check_gpu_brand
 # from bluemist.datasource.aws import get_data_from_s3
 from bluemist.datasource import get_data_from_filesystem
 # from bluemist.pipeline import get_model_pipeline
 from bluemist.preprocessing import preprocess_data
 from bluemist.regression import train_test_evaluate, deploy_model, get_estimators
+
 # from bluemist.eda import perform_eda
 # from bluemist.datasource.database import get_data_from_database
 
 HOME_PATH = os.environ["BLUEMIST_PATH"]
 config.fileConfig(HOME_PATH + '/' + 'logging.config')
 logger = logging.getLogger("root")
 
-
 def main():
     # query = 'SELECT * FROM public.auto_mpg'
     # data = get_data_from_database(db_type='postgres', host='postgres.cxh6nuaszc34.us-east-1.rds.amazonaws.com:5432',
     #                        username='postgres', password='adminadmin', database='postgres', query=query, chunk_size=100)
     #
     # query = 'SELECT * FROM public.auto_mpg'
     # data = get_data_from_database(db_type='aurora-postgres', host='aurora-postgres-instance-1.cxh6nuaszc34.us-east-1.rds.amazonaws.com:5432',
@@ -47,33 +54,38 @@
     #
     #  query = 'SELECT * FROM AUTO_MPG'
     # data = get_data_from_database(db_type='oracle', host='oracle.cxh6nuaszc34.us-east-1.rds.amazonaws.com',
     #                               username='admin', password='adminadmin', service='DATABASE',
     #                               oracle_instant_client_path='/home/shashank-agrawal/Desktop/instantclient_21_6',
     #                               query=query, chunk_size=100)
 
-    #print('get_estimators', get_estimators())
-    initialize()
+    initialize(enable_acceleration_extensions=True)
+    # print('get_estimators', get_estimators())
+    info = cpuinfo.get_cpu_info()
+    print(info)
+    print(sklearn_is_patched())
+
+
     # data = datasets.load_diabetes(as_frame=True)
     # data = get_data_from_filesystem('datasets/auto-mpg/auto-mpg.csv')
 
-    # data = get_data_from_filesystem(
-    #     'https://raw.githubusercontent.com/plotly/datasets/3aa08e58607d1f36159efc4cca9d0d073bbf57bb/auto-mpg.csv')
+    data = get_data_from_filesystem(
+        'https://raw.githubusercontent.com/plotly/datasets/3aa08e58607d1f36159efc4cca9d0d073bbf57bb/auto-mpg.csv')
 
-    #perform_eda(data.frame, target_variable='target', provider='autoviz')
+    # perform_eda(data.frame, target_variable='target', provider='autoviz')
 
-    # X_train, X_test, y_train, y_test = preprocess_data(data,
-    #                                                    target_variable='mpg',
-    #                                                    test_size=0.25,
-    #                                                    data_scaling_strategy='StandardScaler',
-    #                                                    categorical_features=['model_year'],
-    #                                                    categorical_encoder='OneHotEncoder',
-    #                                                    drop_categories_one_hot_encoder='first')
-    # train_test_evaluate(X_train, X_test, y_train, y_test)
-    # deploy_model(estimator_name='RadiusNeighborsRegressor')
+    X_train, X_test, y_train, y_test = preprocess_data(data,
+                                                       target_variable='mpg',
+                                                       test_size=0.25,
+                                                       data_scaling_strategy='StandardScaler',
+                                                       categorical_features=['model_year'],
+                                                       categorical_encoder='OneHotEncoder',
+                                                       drop_categories_one_hot_encoder='first')
+    train_test_evaluate(X_train, X_test, y_train, y_test)
+    deploy_model(estimator_name='LinearSVR')
     # # # pipeline = get_model_pipeline('LarsCV')
     # # print(pipeline.get_params)
     # deploy_model(estimator_name='LarsCV', host='localhost', port=8000)
 
 
 # Press the green button in the gutter to run the script.
 if __name__ == '__main__':
```

### Comparing `bluemist-0.1.1/bluemist/pipeline/bluemist_pipeline.py` & `bluemist-0.1.2/bluemist/pipeline/bluemist_pipeline.py`

 * *Files identical despite different names*

### Comparing `bluemist-0.1.1/bluemist/preprocessing/categorical_transformer.py` & `bluemist-0.1.2/bluemist/preprocessing/categorical_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+# Author: Shashank Agrawal
+# License: MIT
+# Version: 0.1.2
+# Email: dew@bluemist-ai.one
+# Created: Sep 6, 2022
+# Last modified: May 29, 2023
 
-__author__ = "Shashank Agrawal"
-__license__ = "MIT"
-__version__ = "0.1.1"
-__email__ = "dew@bluemist-ai.one"
-
-
+import sklearn
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
-from sklearn.preprocessing import LabelEncoder, OneHotEncoder, OrdinalEncoder
+from sklearn.preprocessing import LabelEncoder, OrdinalEncoder, OneHotEncoder
+
+from bluemist import environment
 
 
 def build_categorical_transformer_pipeline(**kwargs):
     transformer_steps = []
 
     imputer_strategy = kwargs.get('categorical_imputer_strategy')
     categorical_constant_value = kwargs.get('categorical_constant_value')
@@ -22,31 +25,31 @@
     if imputer_strategy is not None and imputer_strategy in ['most_frequent', 'constant']:
         if imputer_strategy == 'constant':
             imputer_step = ('imputer', SimpleImputer(strategy=imputer_strategy, fill_value=categorical_constant_value))
         else:
             imputer_step = ('imputer', SimpleImputer(strategy=imputer_strategy))
         transformer_steps.append(imputer_step)
     else:
-        raise ValueError('Invalid imputer_strategy value passed : ', imputer_strategy)
+        raise ValueError('Invalid imputer_strategy value passed: {}'.format(imputer_strategy))
 
     if categorical_encoder is not None and categorical_encoder in ['OneHotEncoder', 'OrdinalEncoder']:
         encoder_step = tuple()
         if categorical_encoder == 'LabelEncoder':
             encoder_step = ('label_encoder', LabelEncoder())
         elif categorical_encoder == 'OrdinalEncoder':
             encoder_step = ('ordinal_encoder', OrdinalEncoder())
         elif categorical_encoder == 'OneHotEncoder':
-            if drop_categories is not None and handle_unknown is not None:
-                encoder_step = ('one_hot_encoder', OneHotEncoder(drop=drop_categories, handle_unknown=handle_unknown))
-            elif drop_categories is not None:
-                encoder_step = ('one_hot_encoder', OneHotEncoder(drop=drop_categories))
-            elif handle_unknown is not None:
-                encoder_step = ('one_hot_encoder', OneHotEncoder(handle_unknown=handle_unknown))
-            else:
-                encoder_step = ('one_hot_encoder', OneHotEncoder())
+            encoder_class = OneHotEncoder
+            kwargs = {}
+            if drop_categories is not None:
+                kwargs['drop'] = drop_categories
+            if handle_unknown is not None:
+                kwargs['handle_unknown'] = handle_unknown
+
+            encoder_step = ('one_hot_encoder', encoder_class(**kwargs))
 
         transformer_steps.append(encoder_step)
     else:
         raise ValueError('Invalid categorical_encoder value passed : ', categorical_encoder)
 
     categorical_transformer = Pipeline(steps=transformer_steps)
     return categorical_transformer
```

### Comparing `bluemist-0.1.1/bluemist/preprocessing/numeric_transformer.py` & `bluemist-0.1.2/bluemist/preprocessing/numeric_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-
-__author__ = "Shashank Agrawal"
-__license__ = "MIT"
-__version__ = "0.1.1"
-__email__ = "dew@bluemist-ai.one"
+# Author: Shashank Agrawal
+# License: MIT
+# Version: 0.1.2
+# Email: dew@bluemist-ai.one
+# Created: Sep 6, 2022
+# Last modified: June 19, 2023
 
 
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PowerTransformer
 
-from bluemist.utils.scaler import getScaler, available_scalers
+from bluemist.utils.scaler import get_scaler, available_scalers
 
 
 def build_numeric_transformer_pipeline(**kwargs):
     preprocessing_steps = []
 
     imputer_strategy = kwargs.get('numeric_imputer_strategy')
     scaler = kwargs.get('data_scaling_strategy')
@@ -28,21 +29,22 @@
             imputer_step = ('imputer', SimpleImputer(strategy=imputer_strategy))
         preprocessing_steps.append(imputer_step)
     elif imputer_strategy is not None:
         raise ValueError('Invalid imputer_strategy value passed : ', imputer_strategy)
 
     # data scaling
     if scaler is not None and scaler in available_scalers:
-        scaler_step = ('scaler', getScaler(scaler))
+        scaler_step = ('scaler', get_scaler(scaler))
         preprocessing_steps.append(scaler_step)
     elif scaler is not None:
         raise ValueError('Invalid scaler value passed : ', scaler)
 
     # data transformation
     if data_tranformation_strategy is not None and data_tranformation_strategy in ['auto', 'yeo-johnson', 'box-cox']:
+        transformer_step = tuple()
         if data_tranformation_strategy == 'yeo-johnson':
             transformer_step = ('transformer', PowerTransformer(method='yeo-johnson'))
         elif data_tranformation_strategy == 'box-cox':
             transformer_step = ('transformer', PowerTransformer(method='box-cox'))
         preprocessing_steps.append(transformer_step)
 
     numeric_transformer = Pipeline(steps=preprocessing_steps)
```

### Comparing `bluemist-0.1.1/bluemist/preprocessing/preprocessor.py` & `bluemist-0.1.2/bluemist/preprocessing/preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Performs data pre-processing
 """
 
-__author__ = "Shashank Agrawal"
-__license__ = "MIT"
-__version__ = "0.1.1"
-__email__ = "dew@bluemist-ai.one"
+# Author: Shashank Agrawal
+# License: MIT
+# Version: 0.1.2
+# Email: dew@bluemist-ai.one
+# Created: Jun 22, 2022
+# Last modified: June 11, 2023
 
 
 import logging
 import os
 from logging import config
 import numpy as np
 import pandas as pd
+import sklearn
 from sklearn.compose import ColumnTransformer
-from sklearn.model_selection import train_test_split
+
 from bluemist.pipeline.bluemist_pipeline import save_preprocessor
 from bluemist.preprocessing import categorical_transformer, numeric_transformer
 
 BLUEMIST_PATH = os.environ["BLUEMIST_PATH"]
 
 config.fileConfig(BLUEMIST_PATH + '/' + 'logging.config')
 logger = logging.getLogger("bluemist")
@@ -113,14 +116,17 @@
 
         .. raw:: html
            :file: ../../code_samples/quickstarts/preprocessor/preprocessor_categorical.html
 
     """
 
     global target_for_deployment
+    global initial_column_metadata_for_deployment
+    global encoded_columns_for_deployment
+
     target_for_deployment = target_variable
 
     logger.info('Shape of the dataset :: {}'.format(data.shape))
     logger.info('Columns in the dataset :: \n{}'.format(data.columns))
 
     # drop features from the dataset
     if drop_features is not None:
@@ -130,16 +136,20 @@
             data.drop(drop_features, axis=1, inplace=True)
 
     # auto compute numerical and categorical features
     auto_computed_numerical_features = data.select_dtypes(include='number').columns.tolist()
     auto_computed_categorical_features = data.select_dtypes(include='object').columns.tolist()
 
     final_numerical_features = auto_computed_numerical_features.copy()
-    final_numerical_features.remove(target_variable)
+    if target_variable in final_numerical_features:
+        final_numerical_features.remove(target_variable)
+
     final_categorical_features = auto_computed_categorical_features.copy()
+    if target_variable in final_categorical_features:
+        final_categorical_features.remove(target_variable)
 
     # finalize the list of numerical features
     if auto_computed_numerical_features is not None:
         if numerical_features is not None:
             for numerical_feature in numerical_features:
                 if numerical_feature not in auto_computed_numerical_features:
                     final_numerical_features.append(numerical_feature)
@@ -176,21 +186,22 @@
             numeric_conversion_strategy = 'coerce'
         else:
             numeric_conversion_strategy = 'raise'
 
     logger.debug('data.dtypes before preprocessing  :: \n{}'.format(data.dtypes))
 
     if numerical_features is not None:
-        data[final_numerical_features] = data[final_numerical_features].apply(pd.to_numeric, errors=numeric_conversion_strategy, axis=1)
+        data[final_numerical_features] = data[final_numerical_features].apply(pd.to_numeric,
+                                                                              errors=numeric_conversion_strategy,
+                                                                              axis=1)
 
     data[final_categorical_features] = data[final_categorical_features].astype(str)
     logger.debug('data.dtypes after dtype conversion  :: \n{}'.format(data.dtypes))
 
     # Creating list of column name and datatype which will be used in generate_api.py
-    global initial_column_metadata_for_deployment
     for col_name, col_type in data.drop(target_variable, axis=1).dtypes.items():
         initial_column_metadata_for_deployment.append((col_name, col_type))
 
     # create transformers for preprocessing pipeline
     num_transformer = numeric_transformer.build_numeric_transformer_pipeline(**locals())
     cat_transformer = categorical_transformer.build_categorical_transformer_pipeline(**locals())
 
@@ -201,21 +212,22 @@
             ("categorical_transformer", cat_transformer, final_categorical_features)
         ], verbose_feature_names_out=False
     )
 
     X = data.drop([target_variable], axis=1)
     y = data[[target_variable]]
     logger.debug('Splitting dataset into X_train, X_test, y_train, y_test...')
-    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=data_randomizer)
+
+    X_train, X_test, y_train, y_test = sklearn.model_selection.train_test_split(X, y, test_size=test_size,
+                                                                                random_state=data_randomizer)
 
     logger.debug('X_train.dtypes before ColumnTransformer :: \n{}'.format(X_train.dtypes))
     X_train = pd.DataFrame(preprocessor.fit_transform(X_train), columns=preprocessor.get_feature_names_out())
     X_test = pd.DataFrame(preprocessor.transform(X_test), columns=preprocessor.get_feature_names_out())
 
-    global encoded_columns_for_deployment
     encoded_columns_for_deployment = preprocessor.get_feature_names_out()
 
     logger.debug('X_train Columns after ColumnTransformer :: {}'.format(preprocessor.get_feature_names_out()))
     logger.debug('X_train.dtypes after ColumnTransformer :: \n{}'.format(X_train.dtypes))
 
     y_train = np.ravel(y_train)
     y_test = np.ravel(y_test)
```

### Comparing `bluemist-0.1.1/bluemist/regression/regressor.py` & `bluemist-0.1.2/bluemist/regression/regressor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,102 @@
 """
 Performs model training, testing, evaluations and deployment
 """
 
-__author__ = "Shashank Agrawal"
-__license__ = "MIT"
-__version__ = "0.1.1"
-__email__ = "dew@bluemist-ai.one"
+# Author: Shashank Agrawal
+# License: MIT
+# Version: 0.1.2
+# Email: dew@bluemist-ai.one
+# Created:  Jun 22, 2022
+# Last modified: June 19, 2023
 
 import importlib
 import logging
 import os
+import time
 from logging import config
-
 import pandas as pd
 
-import mlflow
-import mlflow.sklearn
-from mlflow.tracking import MlflowClient
 from pandas.core.dtypes.common import is_numeric_dtype
 from sklearn.compose import TransformedTargetRegressor
 from sklearn.model_selection import RandomizedSearchCV
 from sklearn.pipeline import Pipeline
 from tqdm import tqdm
 
 import bluemist
+from bluemist import environment
 from bluemist.pipeline.bluemist_pipeline import add_pipeline_step, save_model_pipeline, clear_all_model_pipelines
 from bluemist.preprocessing import preprocessor
 from bluemist.regression.constant import multi_output_regressors, multi_task_regressors, unsupported_regressors, \
     base_estimator_regressors
+from bluemist.utils.constants import GPU_BRAND_INTEL, GPU_BRAND_NVIDIA, GPU_ACCELERATION_NVIDIA, CPU_ACCELERATION_INTEL, \
+    CPU_BRAND_INTEL
 
-from bluemist.regression.tuning.constant import default_hyperparameters
-from bluemist.utils.metrics import scoringStrategy
+from bluemist.utils.metrics import metric_scorer
 from sklearn.utils import all_estimators
 
-from bluemist.utils.scaler import getScaler
+from bluemist.utils.scaler import get_scaler
 from bluemist.utils import generate_api as generate_api
 from bluemist.artifacts.api import predict
 
 from IPython.display import display, HTML
 
 BLUEMIST_PATH = os.environ["BLUEMIST_PATH"]
 
 config.fileConfig(BLUEMIST_PATH + '/' + 'logging.config')
 logger = logging.getLogger("bluemist")
 
 
+def import_mlflow():
+    import mlflow
+    return mlflow
+
+
+def measure_execution_time(start_time):
+    # Calculate the elapsed time
+    elapsed_time = time.time() - start_time
+
+    # Convert elapsed time to seconds, minutes, milliseconds, and hours
+    milliseconds = int(elapsed_time * 1000) % 1000
+    seconds = elapsed_time % 60
+    minutes = (elapsed_time // 60) % 60
+    hours = (elapsed_time // 3600)
+
+    execution_time = "{:02d}:{:02d}:{:02d},{:03d}".format(int(hours), int(minutes), int(seconds), int(milliseconds))
+    return execution_time
+
+
 def initialize_mlflow(mlflow_experiment_name):
+    mlflow = import_mlflow()
+
     logger.info('Initializing MLFlow...')
     if mlflow_experiment_name is not None:
         experiment = mlflow.get_experiment_by_name(mlflow_experiment_name)
         if not experiment:
             mlflow.create_experiment(name=mlflow_experiment_name,
                                      artifact_location=BLUEMIST_PATH + '/' + 'artifacts/experiments/mlflow')
 
         if experiment is not None and experiment.lifecycle_stage == 'deleted':
             logger.info('Restoring MLFlow experiment :: {}'.format(mlflow_experiment_name))
-            client = MlflowClient()
+            client = mlflow.tracking.MlflowClient()
             client.restore_experiment(experiment.experiment_id)
 
         mlflow.set_experiment(mlflow_experiment_name)
 
 
 def get_estimators(multi_output=False, multi_task=False, names_only=True):
     """
         **Returns the list of available regression estimators**
 
         multi_output : bool, default=False
             Future use
         multi_task : bool, default=False
             Future use
         names_only : bool, default=True
-            Rerturn only the estimator name without metadata
-
+            Returns only the estimator name without metadata
     """
 
     estimators = all_estimators(type_filter='regressor')
     logger.debug('All available estimators :: {}'.format(estimators))
 
     estimators_to_remove = []
     for estimator in estimators:
@@ -98,22 +119,20 @@
 
     logger.info('Estimators available for modelling :: {}'.format(estimators))
     return estimators
 
 
 def deploy_model(estimator_name, host='localhost', port=8000):
     """
-
-        estimator_name : str,
-            Estimator name to be delpoyed
+        estimator_name : str
+            Name of the estimator to be deployed
         host : {str, IPv4 or IPv6}, default='localhost'
-            Hostname or ip address of the machine where API to be deployed
+            Hostname or IP address of the machine where the API will be deployed
         port : int, default=8000
             API listening port
-
     """
 
     logger.info('Generating API code to deploy the model :: {}'.format(estimator_name))
     generate_api.generate_api_code(estimator_name=estimator_name,
                                    initial_column_metadata=preprocessor.initial_column_metadata_for_deployment,
                                    encoded_column_metadata=preprocessor.encoded_columns_for_deployment,
                                    target_variable=preprocessor.target_for_deployment)
@@ -177,183 +196,235 @@
 
         .. raw:: html
             :file: ../../code_samples/quickstarts/regression/regression_hyperparameter_tuning.html
 
     """
 
     tune_all_models = False
-    tune_model_list = []
+    models_to_tune = []
     target_scaler = None
-    capture_stats = False
+    sklearnex_algorithms = None
 
     if target_scaling_strategy is not None:
-        target_scaler = getScaler(target_scaling_strategy)
+        target_scaler = get_scaler(target_scaling_strategy)
 
     if isinstance(tune_models, str) and tune_models == 'all':
         tune_all_models = True
     elif isinstance(tune_models, list):
-        tune_model_list = tune_models
+        models_to_tune = tune_models
 
     if experiment_name is not None:
-        capture_stats = True
         initialize_mlflow(experiment_name)
 
+    # Get patch names from sklearnex
+    if environment.available_cpu == CPU_BRAND_INTEL:
+        from sklearnex import sklearn_is_patched, get_patch_names
+        sklearnex_algorithms = get_patch_names()
+
     df = pd.DataFrame()
 
     estimators = get_estimators(multi_output, multi_task, names_only=False)
-
     clear_all_model_pipelines()
 
-    i = 0
+    counter = 0
+
     # If hyperparameter tuning is requested for specific models, limit the overall training to those models to save time
-    if tune_models is not None and not tune_all_models and tune_model_list:
+    if tune_models is not None and not tune_all_models and models_to_tune:
         estimators_to_skip = []
         for estimator in estimators:
-            if estimator[0] not in tune_model_list:
+            if estimator[0] not in models_to_tune:
                 estimators_to_skip.append(estimator)
 
         for estimator_to_skip in estimators_to_skip:
             estimators.remove(estimator_to_skip)
 
     for estimator_name, estimator_class in (pbar := tqdm(estimators, colour='blue')):
+        start_time = time.time()
         pbar.set_description(f"Training {estimator_name}")
-        i = i + 1
 
-        if tune_models is None or tune_all_models or estimator_name in tune_model_list:
-            try:
-                logger.info(
-                    '###################  Regressor in progress :: {} ###################'.format(estimator_name))
+        counter = counter + 1
+        estimator_execution_device = 'CPU'
+
+        # No tuning OR Tune All OR Tune Few
+        if tune_models is None or tune_all_models or estimator_name in models_to_tune:
+            logger.info('############  Regressor in progress :: {} ############'.format(estimator_name))
+            regressor = None
 
-                regressor = estimator_class()
+            try:
+                if environment.available_gpu == GPU_BRAND_NVIDIA:
+                    import cuml
+                    cuml.set_global_output_type('array')  # cuML will return predictions of type cupy.ndarray
+                    if hasattr(cuml, estimator_name):
+                        regressor = getattr(cuml, estimator_name)()
+                        estimator_execution_device = GPU_ACCELERATION_NVIDIA
+                        logger.info('Regressor class from cuML :: {}'.format(regressor.__class__.__module__ + '.' + regressor.__class__.__name__))
+
+                if regressor is None and environment.available_cpu == CPU_BRAND_INTEL:
+                    for sklearnex_algorithm in sklearnex_algorithms:
+                        if (estimator_name == 'LinearRegression' and sklearnex_algorithm == 'linear') or estimator_name.lower() == sklearnex_algorithm:
+                            logger.info('\nSklearn Algorithm :: {}, Sklearn Intel(R) Ex Algorithm :: {}'.format(estimator_name, sklearnex_algorithm))
+                            if sklearn_is_patched(name=sklearnex_algorithm):
+                                regressor = estimator_class()
+                                estimator_execution_device = CPU_ACCELERATION_INTEL
+                            break
+
+                # Normal CPU processing if acceleration extensions are not applied
+                if regressor is None:
+                    regressor = estimator_class()
 
+                # TODO: Revisit this code. sklearn throws error without n_components=1
                 if estimator_name in ['CCA', 'PLSCanonical']:
                     regressor.set_params(n_components=1)
 
                 # Hyperparameter tuning is requested
-                if tune_all_models or estimator_name in tune_model_list:
-                    estimator_parameters = regressor.get_params()
-                    logger.info('Available hyperparameters to be tuned :: {}'.format(estimator_parameters))
-                    logger.debug('Python type() for hyperparameters :: {}'.format(type(estimator_parameters)))
-
-                    model_hyperparameters_for_tuning = getattr(bluemist.regression.tuning.constant, estimator_name,
-                                                               None)
-
-                    deprecated_hyperparameters = []
-                    for hyperparameter, default_hyperparameter_value in estimator_parameters.items():
-                        if default_hyperparameter_value == 'deprecated':
-                            deprecated_hyperparameters.append(hyperparameter)
+                if tune_all_models or estimator_name in models_to_tune:
+                    estimator_params = regressor.get_params()
+
+                    logger.info('Available hyperparameters to be tuned :: {}'.format(estimator_params))
+                    logger.debug('Python type() for hyperparameters :: {}'.format(type(estimator_params)))
+
+                    if estimator_execution_device == GPU_ACCELERATION_NVIDIA:
+                        default_hyperparameters_module = bluemist.regression.tuning.cuml
+                    else:
+                        default_hyperparameters_module = bluemist.regression.tuning.sklearn
+
+                    default_hyperparameters = getattr(default_hyperparameters_module, 'default_params', None)
+                    model_params_for_tuning = getattr(default_hyperparameters_module, estimator_name, None)
+                    remove_params = model_params_for_tuning.get('remove_params')
+
+                    hyperparameters_to_remove = []
+                    for hyperparameter, default_value in estimator_params.items():
+                        if str(default_value) == 'deprecated':
+                            hyperparameters_to_remove.append(hyperparameter)
                             logger.debug('Deprecated hyperparameter identified :: {}'.format(hyperparameter))
-                        elif model_hyperparameters_for_tuning is not None \
-                                and hyperparameter in model_hyperparameters_for_tuning:
-                            estimator_parameters[hyperparameter] = model_hyperparameters_for_tuning[hyperparameter]
-                            logger.debug('Hyperparameter in model configuration :: {} :: {}'.format(hyperparameter,
-                                                                                                    estimator_parameters[
-                                                                                                        hyperparameter]))
+                        elif model_params_for_tuning is not None and hyperparameter in model_params_for_tuning:
+                            estimator_params[hyperparameter] = model_params_for_tuning[hyperparameter]
+                            logger.debug('Hyperparameter in model configuration :: {} :: {}'.format(hyperparameter, estimator_params[hyperparameter]))
                         elif hyperparameter in default_hyperparameters:
-                            estimator_parameters[hyperparameter] = default_hyperparameters[hyperparameter]
-                            logger.debug('Hyperparameter in default configuration :: {} :: {}'.format(hyperparameter,
-                                                                                                      estimator_parameters[
-                                                                                                          hyperparameter]))
+                            estimator_params[hyperparameter] = default_hyperparameters[hyperparameter]
+                            logger.debug('Hyperparameter in default configuration :: {} :: {}'.format(hyperparameter, estimator_params[hyperparameter]))
 
-                    for deprecated_hyperparameter in deprecated_hyperparameters:
-                        estimator_parameters.pop(deprecated_hyperparameter, None)
+                        if remove_params is not None:
+                            if hyperparameter in remove_params and hyperparameter not in hyperparameters_to_remove:
+                                hyperparameters_to_remove.append(hyperparameter)
+                                logger.debug('Unsupported hyperparameter identified :: {}'.format(hyperparameter))
 
-                    # Creating new dictionary of hyperparameters to add step name as required by the pipeline
-                    hyperparameters = {}
+                    for hyperparameter_to_remove in hyperparameters_to_remove:
+                        estimator_params.pop(hyperparameter_to_remove, None)
 
-                    for hyperparameter in estimator_parameters:
+                    # Creating new dictionary of hyperparameters to add step name as required by the sklearn pipeline
+                    hyperparameters = {}
+                    for hyperparameter in estimator_params:
                         old_key = hyperparameter
 
                         if target_scaling_strategy is not None:
                             new_key = estimator_name + '__regressor__' + hyperparameter
                         else:
                             new_key = estimator_name + '__' + hyperparameter
-                        hyperparameters[new_key] = estimator_parameters[old_key]
+                        hyperparameters[new_key] = estimator_params[old_key]
 
                     logger.info('Hyperparameters to be used for model tuning :: {}'.format(hyperparameters))
 
                     if target_scaling_strategy is not None:
-                        transformed_target_regressor = TransformedTargetRegressor(regressor=regressor,
-                                                                                  transformer=target_scaler)
-                        step_estimator = (estimator_name, transformed_target_regressor)
+                        # TODO: Remove the usage of TransformedTargetRegressor so speical handling is not required for cuML
+                        transformed_target_regressor = TransformedTargetRegressor(regressor=regressor, transformer=target_scaler)
+
+                        if environment.available_gpu == 'NVIDIA':
+                            step_estimator = (estimator_name, regressor)
+                        else:
+                            step_estimator = (estimator_name, transformed_target_regressor)
                         steps = add_pipeline_step(estimator_name, step_estimator)
                     else:
                         step_estimator = (estimator_name, regressor)
                         steps = add_pipeline_step(estimator_name, step_estimator)
 
                     if steps is not None:
                         model_pipeline = Pipeline(steps=steps)
-                        search = RandomizedSearchCV(model_pipeline, param_distributions=hyperparameters, n_iter=100)
-                        fitted_estimator_with_all_parameters = search.fit(X_train, y_train)
-                        pipeline_with_best_estimator = fitted_estimator_with_all_parameters.best_estimator_
+                        randomized_search = RandomizedSearchCV(model_pipeline, param_distributions=hyperparameters, n_iter=100, error_score='raise')
+                        optimized_estimator = randomized_search.fit(X_train, y_train)
+                        best_estimator_pipeline = optimized_estimator.best_estimator_
+
                         logger.debug('Model pipeline parameters :: {}'.format(model_pipeline.get_params().keys()))
-                        logger.info(
-                            'Fitted estimator with all parameters :: {}'.format(fitted_estimator_with_all_parameters))
+                        logger.info('Fitted estimator with all parameters :: {}'.format(optimized_estimator))
                         logger.debug('Model pipeline :: {}'.format(model_pipeline))
-                        logger.info('Model pipeline with best estimator :: {}'.format(pipeline_with_best_estimator))
+                        logger.info('Model pipeline with best estimator :: {}'.format(best_estimator_pipeline))
+
                         if save_pipeline_to_disk:
                             logger.info('Saving model pipeline to disk')
-                            save_model_pipeline(estimator_name, pipeline_with_best_estimator)
+                            save_model_pipeline(estimator_name, best_estimator_pipeline)
                 else:
                     if target_scaling_strategy is not None:
-                        transformed_target_regressor = TransformedTargetRegressor(regressor=regressor,
-                                                                                  transformer=target_scaler)
-                        step_estimator = (estimator_name, transformed_target_regressor)
+                        # TODO: Remove the usage of TransformedTargetRegressor so speical handling is not required for cuML
+                        transformed_target_regressor = TransformedTargetRegressor(regressor=regressor, transformer=target_scaler)
+
+                        if environment.available_gpu == 'NVIDIA':
+                            step_estimator = (estimator_name, regressor)
+                        else:
+                            step_estimator = (estimator_name, transformed_target_regressor)
                         steps = add_pipeline_step(estimator_name, step_estimator)
                     else:
                         step_estimator = (estimator_name, regressor)
                         steps = add_pipeline_step(estimator_name, step_estimator)
 
                     model_pipeline = Pipeline(steps=steps)
-                    pipeline_with_best_estimator = model_pipeline.fit(X_train, y_train)
+                    best_estimator_pipeline = model_pipeline.fit(X_train, y_train)
 
                     if save_pipeline_to_disk:
-                        save_model_pipeline(estimator_name, pipeline_with_best_estimator)
+                        save_model_pipeline(estimator_name, best_estimator_pipeline)
 
-                    logger.info('Model pipeline with best estimator (no hyperparameter tuning) :: {}'.format(
-                        pipeline_with_best_estimator))
+                    logger.info('Model pipeline with best estimator (no hyperparameter tuning) :: {}'.format(best_estimator_pipeline))
                     logger.debug('Model pipeline (no hyperparameter tuning) :: {}'.format(model_pipeline))
 
-                if tune_all_models or estimator_name in tune_model_list:
-                    logger.info('Best score :: {}'.format(fitted_estimator_with_all_parameters.best_score_))
-                    logger.info('Best hyperparameters :: {}'.format(fitted_estimator_with_all_parameters.best_params_))
-
-                y_pred = pipeline_with_best_estimator.predict(X_test)
+                if tune_all_models or estimator_name in models_to_tune:
+                    logger.info('Best score :: {}'.format(optimized_estimator.best_score_))
+                    logger.info('Best hyperparameters :: {}'.format(optimized_estimator.best_params_))
+
+                y_pred = best_estimator_pipeline.predict(X_test)
+
+                # Convert cupy.ndarray to numpy.ndarray as sklearn returns numpy.ndarray but cuML will return cupy.ndarray
+                y_pred_class_name = y_pred.__class__.__module__ + '.' + y_pred.__class__.__name__
+                logger.info('y_pred_class_name :: {}'.format(y_pred_class_name))
+                if y_pred_class_name == 'cupy.ndarray':
+                    import cupy as cp
+                    y_pred = cp.asnumpy(y_pred)
 
-                scorer = scoringStrategy(y_test, y_pred, metrics)
-                estimator_stats_df = scorer.getStats()
+                scorer = metric_scorer(y_test, y_pred, metrics)
+                estimator_stats_df = scorer.calculate_metrics()
 
                 final_stats_df = estimator_stats_df.copy()
+                execution_time = measure_execution_time(start_time)
 
-                # Insert Estimator name as the first column in the dataframe
-                final_stats_df.insert(0, 'Estimator', estimator_name)
+                final_stats_df.insert(0, 'Estimator', estimator_name)  # Insert Estimator name as the first column in the dataframe
+                final_stats_df.insert(1, 'Execution Device', estimator_execution_device)  # Insert Execution Device as the second column in the dataframe
+                final_stats_df.insert(2, 'Execution Time', execution_time) # Insert Execution Time as the third column in the dataframe
 
                 logger.info('Current estimator Stats :: \n{}'.format(final_stats_df.to_string()))
-                logger.debug(
-                    'Current estimator stats as dictionary :: {}'.format(final_stats_df.to_dict('records')))
+                logger.debug('Current estimator stats as dictionary :: {}'.format(final_stats_df.to_dict('records')))
 
                 df = pd.concat([df, final_stats_df], ignore_index=True)
                 logger.debug('Estimator stats so far :: \n{}'.format(df.to_string()))
 
-                if capture_stats:
+                if experiment_name is not None:
+                    mlflow = import_mlflow()
                     with mlflow.start_run(run_name=run_name):
                         logger.info('Capturing stats in MLFlow...')
                         mlflow.log_param('model', estimator_name)
                         mlflow.log_metrics(estimator_stats_df.to_dict('records')[0])
-                        mlflow.sklearn.log_model(pipeline_with_best_estimator, 'model_' + estimator_name)
+                        mlflow.sklearn.log_model(best_estimator_pipeline, 'model_' + estimator_name)
                         run_id = mlflow.active_run().info.run_id
                         logger.info('Model saved in run :: {}'.format(run_id))
             except Exception as e:
                 exception = {'Estimator': [estimator_name], 'Exception': str(e)}
                 exception_df = pd.DataFrame(exception)
                 logger.info('Exception occurred :: \n{}'.format(exception_df))
                 df = pd.concat([df, exception_df])
                 logger.error('Exception occurred while training the model :: {}'.format(str(e)), exc_info=True)
 
     df.set_index('Estimator', inplace=True)
+    #print(df)
     display(HTML(df.style
                  .highlight_max(
         subset=[col for col in df.columns if col.endswith('score') and is_numeric_dtype(df[col])], color='green')
                  .highlight_min(
         subset=[col for col in df.columns if col.endswith('score') and is_numeric_dtype(df[col])], color='yellow')
                  .highlight_max(
         subset=[col for col in df.columns if not col.endswith('score') and is_numeric_dtype(df[col])], color='yellow')
```

### Comparing `bluemist-0.1.1/bluemist/regression/tuning/constant.py` & `bluemist-0.1.2/bluemist/regression/tuning/sklearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-
-__author__ = "Shashank Agrawal"
-__license__ = "MIT"
-__version__ = "0.1.1"
-__email__ = "dew@bluemist-ai.one"
-
+# Author: Shashank Agrawal
+# License: MIT
+# Version: 0.1.2
+# Email: dew@bluemist-ai.one
+# Created: Jun 22, 2022
+# Last modified: May 29, 2023
 
 import numpy as np
 
-default_hyperparameters = {
+default_params = {
     'algorithm': ['auto', 'ball_tree', 'kd_tree', 'brute'],
     'alphas': [None],
     'alpha': [1.0, 1.5, 2.0, 2.5, 3, 3.5, 4, 4.5, 5],
     'alpha_1': [1e-06, 1e-05, 0.0001, 0.001, 0.01, 0.1],
     'alpha_2': [1e-06, 1e-05, 0.0001, 0.001, 0.01, 0.1],
     'alpha_init': [None, 1e-06, 1e-05, 0.0001, 0.001, 0.01, 0.1],  # TODO: Review this parameter
     'bootstrap': [True, False],
@@ -251,15 +251,16 @@
     'leaf_size': np.arange(2, 50 + 1, 1).tolist(),
     'p': [1, 2],
     'metric': ['euclidean', 'minkowski'],
     'metric_params': [None]
 }
 
 RandomForestRegressor = {
-    'max_features': [None, 'sqrt', 'log2', 0.7, 0.8, 0.9, 1]
+    'max_features': [None, 'sqrt', 'log2', 0.7, 0.8, 0.9, 1],
+    'maxBins': [256]
 }
 
 Ridge = {
     'solver': ['auto', 'svd', 'cholesky', 'lsqr', 'sparse_cg', 'sag', 'saga', 'lbfgs']
 }
 
 RidgeCV = {
```

### Comparing `bluemist-0.1.1/bluemist/utils/generate_api.py` & `bluemist-0.1.2/bluemist/utils/generate_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+# Author: Shashank Agrawal
+# License: MIT
+# Version: 0.1.2
+# Email: dew@bluemist-ai.one
+# Created:  Feb 19, 2023
+# Last modified: June 19, 2023
+
 import os
 from jinja2 import Template
 
 BLUEMIST_PATH = os.environ["BLUEMIST_PATH"]
 
 class_template = """import nest_asyncio
 import pandas as pd
 import joblib
 import uvicorn
 from pydantic import BaseModel
 from fastapi import FastAPI
 from pyngrok import ngrok
 import os
-import numpy as np
 
 
 class request_body(BaseModel):
     {%+ for column, data_type in initial_column_metadata -%}
         {{ column }}: np.{{ data_type.name }}
     {%+ endfor -%}
 
@@ -23,15 +29,15 @@
 
 func_template = """
 
 app = FastAPI(debug=True)
 
 BLUEMIST_PATH = os.environ["BLUEMIST_PATH"]
 preprocessor = joblib.load(BLUEMIST_PATH + '/' + 'artifacts/preprocessor/preprocessor.joblib')
-pipeline = joblib.load(BLUEMIST_PATH + '/' + 'artifacts/models/LarsCV.joblib')
+pipeline = joblib.load(BLUEMIST_PATH + '/' + 'artifacts/models/{{ estimator_name }}.joblib')
 
 
 @app.post('/predict')
 def predict(data: request_body):
     # Making the data in a form suitable for prediction
     input_data = [[
         {%+ for column, _ in initial_column_metadata -%}
```

### Comparing `bluemist-0.1.1/bluemist.egg-info/SOURCES.txt` & `bluemist-0.1.2/bluemist.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 requirements.txt
 setup.cfg
 setup.py
 bluemist/__init__.py
 bluemist/environment.py
 bluemist/logging.config
 bluemist/main.py
+bluemist/main_predict.py
 bluemist.egg-info/PKG-INFO
 bluemist.egg-info/SOURCES.txt
 bluemist.egg-info/dependency_links.txt
 bluemist.egg-info/requires.txt
 bluemist.egg-info/top_level.txt
 bluemist/artifacts/api/predict.py
 bluemist/artifacts/api/__pycache__/predict.cpython-39.pyc
 bluemist/artifacts/logs/bluemist.log
-bluemist/artifacts/logs/bluemist.log.1
-bluemist/artifacts/logs/bluemist.log.2
 bluemist/classification/__init__.py
 bluemist/datasets/auto-mpg/Index
 bluemist/datasets/auto-mpg/auto-mpg.csv
 bluemist/datasets/auto-mpg/auto-mpg.data
 bluemist/datasets/auto-mpg/auto-mpg.data-original
 bluemist/datasets/auto-mpg/auto-mpg.names
 bluemist/datasource/__init__.py
@@ -39,13 +38,15 @@
 bluemist/preprocessing/categorical_transformer.py
 bluemist/preprocessing/numeric_transformer.py
 bluemist/preprocessing/preprocessor.py
 bluemist/regression/__init__.py
 bluemist/regression/constant.py
 bluemist/regression/regressor.py
 bluemist/regression/tuning/__init__.py
-bluemist/regression/tuning/constant.py
+bluemist/regression/tuning/cuml.py
+bluemist/regression/tuning/sklearn.py
 bluemist/tests/__init__.py
 bluemist/utils/__init__.py
+bluemist/utils/constants.py
 bluemist/utils/generate_api.py
 bluemist/utils/metrics.py
 bluemist/utils/scaler.py
```

