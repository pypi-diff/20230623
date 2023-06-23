# Comparing `tmp/mlpype-sklearn-0.4.2.tar.gz` & `tmp/mlpype-sklearn-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-sklearn-0.4.2.tar", last modified: Tue Jun 20 17:15:44 2023, max compression
+gzip compressed data, was "mlpype-sklearn-0.4.3.tar", last modified: Fri Jun 23 07:14:30 2023, max compression
```

## Comparing `mlpype-sklearn-0.4.2.tar` & `mlpype-sklearn-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:44.471739 mlpype-sklearn-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 17:15:44.471739 mlpype-sklearn-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:44.467739 mlpype-sklearn-0.4.2/mlpype_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 17:15:44.000000 mlpype-sklearn-0.4.2/mlpype_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 17:15:44.000000 mlpype-sklearn-0.4.2/mlpype_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:44.000000 mlpype-sklearn-0.4.2/mlpype_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 17:15:44.000000 mlpype-sklearn-0.4.2/mlpype_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:44.000000 mlpype-sklearn-0.4.2/mlpype_sklearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:15:44.471739 mlpype-sklearn-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-20 17:11:28.000000 mlpype-sklearn-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:30.000000 mlpype-sklearn-0.4.3/mlpype_sklearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:30.273767 mlpype-sklearn-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 07:11:18.000000 mlpype-sklearn-0.4.3/setup.py
```

### Comparing `mlpype-sklearn-0.4.2/setup.py` & `mlpype-sklearn-0.4.3/setup.py`

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

