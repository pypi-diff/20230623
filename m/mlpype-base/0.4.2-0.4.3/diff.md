# Comparing `tmp/mlpype-base-0.4.2.tar.gz` & `tmp/mlpype-base-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-base-0.4.2.tar", last modified: Tue Jun 20 17:15:06 2023, max compression
+gzip compressed data, was "mlpype-base-0.4.3.tar", last modified: Fri Jun 23 07:14:01 2023, max compression
```

## Comparing `mlpype-base-0.4.2.tar` & `mlpype-base-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:06.723435 mlpype-base-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 17:15:06.723435 mlpype-base-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:06.723435 mlpype-base-0.4.2/mlpype_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 17:15:06.000000 mlpype-base-0.4.2/mlpype_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 17:15:06.000000 mlpype-base-0.4.2/mlpype_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:06.000000 mlpype-base-0.4.2/mlpype_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-20 17:15:06.000000 mlpype-base-0.4.2/mlpype_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:06.000000 mlpype-base-0.4.2/mlpype_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:15:06.723435 mlpype-base-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 17:11:28.000000 mlpype-base-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/mlpype_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:01.000000 mlpype-base-0.4.3/mlpype_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:01.841370 mlpype-base-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-23 07:11:18.000000 mlpype-base-0.4.3/setup.py
```

### Comparing `mlpype-base-0.4.2/setup.py` & `mlpype-base-0.4.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
     deps = [
         f"mlpype=={version}",
         "docstring_parser>=0.14.1",
         "pydantic>=1.9.1",
```

