# Comparing `tmp/mlpype-fastapi-0.4.3.tar.gz` & `tmp/mlpype-fastapi-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-fastapi-0.4.3.tar", last modified: Fri Jun 23 07:14:08 2023, max compression
+gzip compressed data, was "mlpype-fastapi-0.4.4.tar", last modified: Fri Jun 23 09:47:38 2023, max compression
```

## Comparing `mlpype-fastapi-0.4.3.tar` & `mlpype-fastapi-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:14:08.000000 mlpype-fastapi-0.4.3/mlpype_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:14:08.677471 mlpype-fastapi-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 07:11:18.000000 mlpype-fastapi-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:38.687983 mlpype-fastapi-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 09:47:38.687983 mlpype-fastapi-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:47:38.687983 mlpype-fastapi-0.4.4/mlpype_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 09:47:38.000000 mlpype-fastapi-0.4.4/mlpype_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-23 09:47:38.000000 mlpype-fastapi-0.4.4/mlpype_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:47:38.000000 mlpype-fastapi-0.4.4/mlpype_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 09:47:38.000000 mlpype-fastapi-0.4.4/mlpype_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:47:38.000000 mlpype-fastapi-0.4.4/mlpype_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:47:38.687983 mlpype-fastapi-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-23 09:44:01.000000 mlpype-fastapi-0.4.4/setup.py
```

### Comparing `mlpype-fastapi-0.4.3/setup.py` & `mlpype-fastapi-0.4.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.3"
+    version = "0.4.4"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

