# Comparing `tmp/mlpype-xgboost-0.4.2.tar.gz` & `tmp/mlpype-xgboost-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-xgboost-0.4.2.tar", last modified: Tue Jun 20 17:16:12 2023, max compression
+gzip compressed data, was "mlpype-xgboost-0.4.3.tar", last modified: Fri Jun 23 07:14:50 2023, max compression
```

## Comparing `mlpype-xgboost-0.4.2.tar` & `mlpype-xgboost-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:16:12.231917 mlpype-xgboost-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 17:16:12.231917 mlpype-xgboost-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:16:12.231917 mlpype-xgboost-0.4.2/mlpype_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 17:16:12.000000 mlpype-xgboost-0.4.2/mlpype_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 17:16:12.000000 mlpype-xgboost-0.4.2/mlpype_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:16:12.000000 mlpype-xgboost-0.4.2/mlpype_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 17:16:12.000000 mlpype-xgboost-0.4.2/mlpype_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:16:12.000000 mlpype-xgboost-0.4.2/mlpype_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:16:12.231917 mlpype-xgboost-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 17:11:28.000000 mlpype-xgboost-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:50.970062 mlpype-xgboost-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:50.970062 mlpype-xgboost-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:50.970062 mlpype-xgboost-0.4.3/mlpype_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:50.000000 mlpype-xgboost-0.4.3/mlpype_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 07:14:50.000000 mlpype-xgboost-0.4.3/mlpype_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:50.000000 mlpype-xgboost-0.4.3/mlpype_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-23 07:14:50.000000 mlpype-xgboost-0.4.3/mlpype_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:50.000000 mlpype-xgboost-0.4.3/mlpype_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:50.970062 mlpype-xgboost-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-23 07:11:18.000000 mlpype-xgboost-0.4.3/setup.py
```

