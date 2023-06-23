# Comparing `tmp/mlpype-spark-0.4.2.tar.gz` & `tmp/mlpype-spark-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-spark-0.4.2.tar", last modified: Tue Jun 20 17:15:53 2023, max compression
+gzip compressed data, was "mlpype-spark-0.4.3.tar", last modified: Fri Jun 23 07:14:37 2023, max compression
```

## Comparing `mlpype-spark-0.4.2.tar` & `mlpype-spark-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:53.723804 mlpype-spark-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 17:15:53.723804 mlpype-spark-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:53.723804 mlpype-spark-0.4.2/mlpype_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 17:15:53.000000 mlpype-spark-0.4.2/mlpype_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-20 17:15:53.000000 mlpype-spark-0.4.2/mlpype_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:53.000000 mlpype-spark-0.4.2/mlpype_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 17:15:53.000000 mlpype-spark-0.4.2/mlpype_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:53.000000 mlpype-spark-0.4.2/mlpype_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:15:53.723804 mlpype-spark-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 17:11:28.000000 mlpype-spark-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:37.185861 mlpype-spark-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 07:14:37.185861 mlpype-spark-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:37.181861 mlpype-spark-0.4.3/mlpype_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:37.000000 mlpype-spark-0.4.3/mlpype_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:37.185861 mlpype-spark-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-23 07:11:18.000000 mlpype-spark-0.4.3/setup.py
```

### Comparing `mlpype-spark-0.4.2/setup.py` & `mlpype-spark-0.4.3/setup.py`

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

