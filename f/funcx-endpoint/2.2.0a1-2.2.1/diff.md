# Comparing `tmp/funcx-endpoint-2.2.0a1.tar.gz` & `tmp/funcx-endpoint-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-endpoint-2.2.0a1.tar", last modified: Wed Jun 21 18:54:06 2023, max compression
+gzip compressed data, was "funcx-endpoint-2.2.1.tar", last modified: Fri Jun 23 01:08:11 2023, max compression
```

## Comparing `funcx-endpoint-2.2.0a1.tar` & `funcx-endpoint-2.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:54:06.746999 funcx-endpoint-2.2.0a1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.0a1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 funcx-endpoint-2.2.0a1/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     2042 2023-06-21 18:54:06.747064 funcx-endpoint-2.2.0a1/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1115 2023-04-20 03:21:56.000000 funcx-endpoint-2.2.0a1/PyPI.md
--rw-r--r--   0 lei        (501) staff       (20)      430 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.0a1/README.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:54:06.744898 funcx-endpoint-2.2.0a1/funcx_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      122 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:54:06.745689 funcx-endpoint-2.2.0a1/funcx_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:54:06.745886 funcx-endpoint-2.2.0a1/funcx_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)       73 2023-06-13 18:28:48.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:54:06.746141 funcx-endpoint-2.2.0a1/funcx_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      107 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:54:06.746839 funcx-endpoint-2.2.0a1/funcx_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      101 2023-04-20 03:22:06.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/executors/high_throughput/funcx_manager.py
--rw-r--r--   0 lei        (501) staff       (20)      114 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/executors/high_throughput/funcx_worker.py
--rw-r--r--   0 lei        (501) staff       (20)      245 2023-06-21 18:52:15.000000 funcx-endpoint-2.2.0a1/funcx_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:54:06.745579 funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     2042 2023-06-21 18:54:06.000000 funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      662 2023-06-21 18:54:06.000000 funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-21 18:54:06.000000 funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      329 2023-06-21 18:54:06.000000 funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)       33 2023-06-21 18:54:06.000000 funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       15 2023-06-21 18:54:06.000000 funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-06-21 18:54:06.747321 funcx-endpoint-2.2.0a1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     2032 2023-06-21 18:52:09.000000 funcx-endpoint-2.2.0a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:08:11.782297 funcx-endpoint-2.2.1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 funcx-endpoint-2.2.1/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     2040 2023-06-23 01:08:11.782367 funcx-endpoint-2.2.1/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1115 2023-04-20 03:21:56.000000 funcx-endpoint-2.2.1/PyPI.md
+-rw-r--r--   0 lei        (501) staff       (20)      430 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.1/README.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:08:11.779962 funcx-endpoint-2.2.1/funcx_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      122 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.1/funcx_endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:08:11.780870 funcx-endpoint-2.2.1/funcx_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.2.1/funcx_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:08:11.781100 funcx-endpoint-2.2.1/funcx_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.2.1/funcx_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)       73 2023-06-13 18:28:48.000000 funcx-endpoint-2.2.1/funcx_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:08:11.781379 funcx-endpoint-2.2.1/funcx_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      107 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.1/funcx_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:08:11.782123 funcx-endpoint-2.2.1/funcx_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.2.1/funcx_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      101 2023-04-20 03:22:06.000000 funcx-endpoint-2.2.1/funcx_endpoint/executors/high_throughput/funcx_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      114 2023-04-10 19:02:41.000000 funcx-endpoint-2.2.1/funcx_endpoint/executors/high_throughput/funcx_worker.py
+-rw-r--r--   0 lei        (501) staff       (20)      243 2023-06-23 01:07:20.000000 funcx-endpoint-2.2.1/funcx_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:08:11.780734 funcx-endpoint-2.2.1/funcx_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     2040 2023-06-23 01:08:11.000000 funcx-endpoint-2.2.1/funcx_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      662 2023-06-23 01:08:11.000000 funcx-endpoint-2.2.1/funcx_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-23 01:08:11.000000 funcx-endpoint-2.2.1/funcx_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      329 2023-06-23 01:08:11.000000 funcx-endpoint-2.2.1/funcx_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)       31 2023-06-23 01:08:11.000000 funcx-endpoint-2.2.1/funcx_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       15 2023-06-23 01:08:11.000000 funcx-endpoint-2.2.1/funcx_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      305 2023-06-23 01:08:11.782644 funcx-endpoint-2.2.1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     2030 2023-06-23 01:07:20.000000 funcx-endpoint-2.2.1/setup.py
```

### Comparing `funcx-endpoint-2.2.0a1/LICENSE` & `funcx-endpoint-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.2.0a1/PKG-INFO` & `funcx-endpoint-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.2.0a1/PyPI.md` & `funcx-endpoint-2.2.1/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/PKG-INFO` & `funcx-endpoint-2.2.1/funcx_endpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.2.0a1/funcx_endpoint.egg-info/SOURCES.txt` & `funcx-endpoint-2.2.1/funcx_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.2.0a1/setup.py` & `funcx-endpoint-2.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-endpoint==2.2.0a1",
+    "globus-compute-endpoint==2.2.1",
 ]
 
 version_ns = {}
 with open(os.path.join("funcx_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
```

