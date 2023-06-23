# Comparing `tmp/mlpype-hyperopt-0.4.3.tar.gz` & `tmp/mlpype-hyperopt-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-hyperopt-0.4.3.tar", last modified: Fri Jun 23 07:14:15 2023, max compression
+gzip compressed data, was "mlpype-hyperopt-0.4.4.tar", last modified: Fri Jun 23 09:47:47 2023, max compression
```

## Comparing `mlpype-hyperopt-0.4.3.tar` & `mlpype-hyperopt-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:15.561567 mlpype-hyperopt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 07:14:15.561567 mlpype-hyperopt-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:15.561567 mlpype-hyperopt-0.4.3/mlpype_hyperopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 07:14:15.000000 mlpype-hyperopt-0.4.3/mlpype_hyperopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 07:14:15.000000 mlpype-hyperopt-0.4.3/mlpype_hyperopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:15.000000 mlpype-hyperopt-0.4.3/mlpype_hyperopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 07:14:15.000000 mlpype-hyperopt-0.4.3/mlpype_hyperopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:15.000000 mlpype-hyperopt-0.4.3/mlpype_hyperopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:15.561567 mlpype-hyperopt-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-23 07:11:18.000000 mlpype-hyperopt-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:47.720027 mlpype-hyperopt-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 09:47:47.720027 mlpype-hyperopt-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:47.720027 mlpype-hyperopt-0.4.4/mlpype_hyperopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 09:47:47.000000 mlpype-hyperopt-0.4.4/mlpype_hyperopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 09:47:47.000000 mlpype-hyperopt-0.4.4/mlpype_hyperopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:47:47.000000 mlpype-hyperopt-0.4.4/mlpype_hyperopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 09:47:47.000000 mlpype-hyperopt-0.4.4/mlpype_hyperopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:47:47.000000 mlpype-hyperopt-0.4.4/mlpype_hyperopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:47:47.720027 mlpype-hyperopt-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-23 09:44:01.000000 mlpype-hyperopt-0.4.4/setup.py
```

