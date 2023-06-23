# Comparing `tmp/mlpype-spark-0.4.3.tar.gz` & `tmp/mlpype-spark-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-spark-0.4.3.tar", last modified: Fri Jun 23 07:14:37 2023, max compression
+gzip compressed data, was "mlpype-spark-0.4.4.tar", last modified: Fri Jun 23 09:48:14 2023, max compression
```

## Comparing `mlpype-spark-0.4.3.tar` & `mlpype-spark-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:37.185861 mlpype-spark-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 07:14:37.185861 mlpype-spark-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:37.181861 mlpype-spark-0.4.3/mlpype_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:37.185861 mlpype-spark-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-23 07:11:18.000000 mlpype-spark-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:14.096099 mlpype-spark-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 09:48:14.096099 mlpype-spark-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:14.096099 mlpype-spark-0.4.4/mlpype_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 09:48:14.000000 mlpype-spark-0.4.4/mlpype_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-23 09:48:14.000000 mlpype-spark-0.4.4/mlpype_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:14.000000 mlpype-spark-0.4.4/mlpype_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 09:48:14.000000 mlpype-spark-0.4.4/mlpype_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:14.000000 mlpype-spark-0.4.4/mlpype_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:48:14.096099 mlpype-spark-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-23 09:44:01.000000 mlpype-spark-0.4.4/setup.py
```

### Comparing `mlpype-spark-0.4.3/setup.py` & `mlpype-spark-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.3"
+    version = "0.4.4"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```

