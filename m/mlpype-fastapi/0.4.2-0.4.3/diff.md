# Comparing `tmp/mlpype-fastapi-0.4.2.tar.gz` & `tmp/mlpype-fastapi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-fastapi-0.4.2.tar", last modified: Tue Jun 20 17:15:15 2023, max compression
+gzip compressed data, was "mlpype-fastapi-0.4.3.tar", last modified: Fri Jun 23 07:14:08 2023, max compression
```

## Comparing `mlpype-fastapi-0.4.2.tar` & `mlpype-fastapi-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:15.983511 mlpype-fastapi-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 17:15:15.983511 mlpype-fastapi-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:15:15.983511 mlpype-fastapi-0.4.2/mlpype_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 17:15:15.000000 mlpype-fastapi-0.4.2/mlpype_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 17:15:15.000000 mlpype-fastapi-0.4.2/mlpype_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:15.000000 mlpype-fastapi-0.4.2/mlpype_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 17:15:15.000000 mlpype-fastapi-0.4.2/mlpype_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:15:15.000000 mlpype-fastapi-0.4.2/mlpype_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:15:15.983511 mlpype-fastapi-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 17:11:28.000000 mlpype-fastapi-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 07:11:18.000000 mlpype-fastapi-0.4.3/setup.py
```

### Comparing `mlpype-fastapi-0.4.2/setup.py` & `mlpype-fastapi-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.2"
+    version = "0.4.3"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

