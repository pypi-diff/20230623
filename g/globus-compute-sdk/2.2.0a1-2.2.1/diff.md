# Comparing `tmp/globus-compute-sdk-2.2.0a1.tar.gz` & `tmp/globus-compute-sdk-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.2.0a1.tar", last modified: Wed Jun 21 18:53:16 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.2.1.tar", last modified: Fri Jun 23 01:03:43 2023, max compression
```

## Comparing `globus-compute-sdk-2.2.0a1.tar` & `globus-compute-sdk-2.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.908536 globus-compute-sdk-2.2.0a1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.0a1/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1821 2023-06-21 18:53:16.908593 globus-compute-sdk-2.2.0a1/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.0a1/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.901444 globus-compute-sdk-2.2.0a1/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.902574 globus-compute-sdk-2.2.0a1/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.904476 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1276 2023-06-21 18:50:27.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.905124 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)    11458 2023-04-24 21:22:25.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    27030 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    46344 2023-06-05 19:33:47.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.907175 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7287 2023-06-12 17:16:14.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     3012 2023-05-05 16:40:44.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.907467 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)     8443 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.908300 globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      603 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1412 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     7869 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     4848 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-05-08 21:56:13.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/utils.py
--rw-r--r--   0 lei        (501) staff       (20)      834 2023-06-21 18:51:48.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-21 18:53:16.902063 globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1821 2023-06-21 18:53:16.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1577 2023-06-21 18:53:16.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-21 18:53:16.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      397 2023-06-21 18:53:16.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-06-21 18:53:16.000000 globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-21 18:53:16.908839 globus-compute-sdk-2.2.0a1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3161 2023-06-21 18:50:25.000000 globus-compute-sdk-2.2.0a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.700949 globus-compute-sdk-2.2.1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.1/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1819 2023-06-23 01:03:43.701006 globus-compute-sdk-2.2.1/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.1/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.693707 globus-compute-sdk-2.2.1/globus_compute_sdk/
+-rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.694735 globus-compute-sdk-2.2.1/globus_compute_sdk/errors/
+-rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.696785 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1276 2023-06-21 18:50:27.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.697351 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 lei        (501) staff       (20)    11458 2023-04-24 21:22:25.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 lei        (501) staff       (20)    27030 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 lei        (501) staff       (20)    46344 2023-06-05 19:33:47.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.699432 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 lei        (501) staff       (20)     7287 2023-06-12 17:16:14.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 lei        (501) staff       (20)     3012 2023-05-05 16:40:44.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.699716 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 lei        (501) staff       (20)     8443 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.700708 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      603 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1412 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     7869 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 lei        (501) staff       (20)     4848 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-05-08 21:56:13.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)      832 2023-06-23 00:58:49.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.694321 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1819 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1577 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      397 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       19 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-23 01:03:43.701241 globus-compute-sdk-2.2.1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3161 2023-06-21 18:50:25.000000 globus-compute-sdk-2.2.1/setup.py
```

### Comparing `globus-compute-sdk-2.2.0a1/LICENSE` & `globus-compute-sdk-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/PKG-INFO` & `globus-compute-sdk-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.0a1/PyPI.md` & `globus-compute-sdk-2.2.1/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/_environments.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/__init__.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk/version.py` & `globus-compute-sdk-2.2.1/globus_compute_sdk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.0a1"
+__version__ = "2.2.1"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.0a1/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.0a1/setup.py` & `globus-compute-sdk-2.2.1/setup.py`

 * *Files identical despite different names*

