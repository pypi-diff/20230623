# Comparing `tmp/mlpype-tensorflow-0.4.2.tar.gz` & `tmp/mlpype-tensorflow-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-tensorflow-0.4.2.tar", last modified: Tue Jun 20 17:16:03 2023, max compression
+gzip compressed data, was "mlpype-tensorflow-0.4.3.tar", last modified: Fri Jun 23 07:14:44 2023, max compression
```

## Comparing `mlpype-tensorflow-0.4.2.tar` & `mlpype-tensorflow-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:16:03.011848 mlpype-tensorflow-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 17:16:03.011848 mlpype-tensorflow-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:16:03.011848 mlpype-tensorflow-0.4.2/mlpype_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 17:16:03.000000 mlpype-tensorflow-0.4.2/mlpype_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 17:16:03.000000 mlpype-tensorflow-0.4.2/mlpype_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:16:03.000000 mlpype-tensorflow-0.4.2/mlpype_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 17:16:03.000000 mlpype-tensorflow-0.4.2/mlpype_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:16:03.000000 mlpype-tensorflow-0.4.2/mlpype_tensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:16:03.011848 mlpype-tensorflow-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-20 17:11:28.000000 mlpype-tensorflow-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:44.085962 mlpype-tensorflow-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 07:14:44.085962 mlpype-tensorflow-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:44.085962 mlpype-tensorflow-0.4.3/mlpype_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 07:14:44.000000 mlpype-tensorflow-0.4.3/mlpype_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-23 07:14:44.000000 mlpype-tensorflow-0.4.3/mlpype_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:44.000000 mlpype-tensorflow-0.4.3/mlpype_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 07:14:44.000000 mlpype-tensorflow-0.4.3/mlpype_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:44.000000 mlpype-tensorflow-0.4.3/mlpype_tensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:44.085962 mlpype-tensorflow-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 07:11:18.000000 mlpype-tensorflow-0.4.3/setup.py
```

### Comparing `mlpype-tensorflow-0.4.2/setup.py` & `mlpype-tensorflow-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
 
     deps = [
         f"mlpype-base=={version}",
         # on mac, it is recommended to use conda/mamba or source to install tensorflow
         "tensorflow>=2.12",
         "numpy>=1.23.0",
         "protobuf>=3.20.3",
```
