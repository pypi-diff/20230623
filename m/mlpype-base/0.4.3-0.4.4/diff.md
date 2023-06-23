# Comparing `tmp/mlpype-base-0.4.3.tar.gz` & `tmp/mlpype-base-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-base-0.4.3.tar", last modified: Fri Jun 23 07:14:01 2023, max compression
+gzip compressed data, was "mlpype-base-0.4.4.tar", last modified: Fri Jun 23 09:47:29 2023, max compression
```

## Comparing `mlpype-base-0.4.3.tar` & `mlpype-base-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/mlpype_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-23 07:11:18.000000 mlpype-base-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:29.891941 mlpype-base-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 09:47:29.891941 mlpype-base-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:29.891941 mlpype-base-0.4.4/mlpype_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 09:47:29.000000 mlpype-base-0.4.4/mlpype_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 09:47:29.000000 mlpype-base-0.4.4/mlpype_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:47:29.000000 mlpype-base-0.4.4/mlpype_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-23 09:47:29.000000 mlpype-base-0.4.4/mlpype_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:47:29.000000 mlpype-base-0.4.4/mlpype_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:47:29.891941 mlpype-base-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-23 09:44:01.000000 mlpype-base-0.4.4/setup.py
```

### Comparing `mlpype-base-0.4.3/setup.py` & `mlpype-base-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.3"
+    version = "0.4.4"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
     deps = [
         f"mlpype=={version}",
         "docstring_parser>=0.14.1",
         "pydantic>=1.9.1",
```

