# Comparing `tmp/mlpype-sklearn-0.4.3.tar.gz` & `tmp/mlpype-sklearn-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-sklearn-0.4.3.tar", last modified: Fri Jun 23 07:14:30 2023, max compression
+gzip compressed data, was "mlpype-sklearn-0.4.4.tar", last modified: Fri Jun 23 09:48:05 2023, max compression
```

## Comparing `mlpype-sklearn-0.4.3.tar` & `mlpype-sklearn-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 07:11:18.000000 mlpype-sklearn-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:05.292093 mlpype-sklearn-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 09:48:05.292093 mlpype-sklearn-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:05.292093 mlpype-sklearn-0.4.4/mlpype_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 09:48:05.000000 mlpype-sklearn-0.4.4/mlpype_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 09:48:05.000000 mlpype-sklearn-0.4.4/mlpype_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:05.000000 mlpype-sklearn-0.4.4/mlpype_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 09:48:05.000000 mlpype-sklearn-0.4.4/mlpype_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:05.000000 mlpype-sklearn-0.4.4/mlpype_sklearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:48:05.292093 mlpype-sklearn-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 09:44:01.000000 mlpype-sklearn-0.4.4/setup.py
```

### Comparing `mlpype-sklearn-0.4.3/setup.py` & `mlpype-sklearn-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.3"
+    version = "0.4.4"
 
     deps = [
         f"mlpype-base=={version}",
         "numpy>=1.23.0",
         "scikit-learn>=1.1.1",
         "pandas>=1.4.3",
     ]
```

