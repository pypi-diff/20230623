# Comparing `tmp/autogluon-0.8.1b20230621.tar.gz` & `tmp/autogluon-0.8.1b20230622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.1b20230621.tar", last modified: Wed Jun 21 09:04:33 2023, max compression
+gzip compressed data, was "autogluon-0.8.1b20230622.tar", last modified: Thu Jun 22 09:04:16 2023, max compression
```

## Comparing `autogluon-0.8.1b20230621.tar` & `autogluon-0.8.1b20230622.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:33.396947 autogluon-0.8.1b20230621/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-21 09:04:33.396947 autogluon-0.8.1b20230621/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:04:33.396947 autogluon-0.8.1b20230621/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-21 09:03:46.000000 autogluon-0.8.1b20230621/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:33.396947 autogluon-0.8.1b20230621/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:33.396947 autogluon-0.8.1b20230621/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:33.396947 autogluon-0.8.1b20230621/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:03:46.000000 autogluon-0.8.1b20230621/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:33.396947 autogluon-0.8.1b20230621/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-21 09:04:33.000000 autogluon-0.8.1b20230621/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-21 09:04:33.000000 autogluon-0.8.1b20230621/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:04:33.000000 autogluon-0.8.1b20230621/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 09:04:33.000000 autogluon-0.8.1b20230621/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 09:04:33.000000 autogluon-0.8.1b20230621/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 09:04:33.000000 autogluon-0.8.1b20230621/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:04:33.000000 autogluon-0.8.1b20230621/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:16.368095 autogluon-0.8.1b20230622/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-22 09:04:16.368095 autogluon-0.8.1b20230622/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:04:16.368095 autogluon-0.8.1b20230622/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-22 09:03:32.000000 autogluon-0.8.1b20230622/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:16.368095 autogluon-0.8.1b20230622/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:16.368095 autogluon-0.8.1b20230622/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:16.368095 autogluon-0.8.1b20230622/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:03:32.000000 autogluon-0.8.1b20230622/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:04:16.368095 autogluon-0.8.1b20230622/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-22 09:04:16.000000 autogluon-0.8.1b20230622/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 09:04:16.000000 autogluon-0.8.1b20230622/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:04:16.000000 autogluon-0.8.1b20230622/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:04:16.000000 autogluon-0.8.1b20230622/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 09:04:16.000000 autogluon-0.8.1b20230622/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:04:16.000000 autogluon-0.8.1b20230622/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:04:16.000000 autogluon-0.8.1b20230622/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.1b20230621/PKG-INFO` & `autogluon-0.8.1b20230622/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230621
+Version: 0.8.1b20230622
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.1b20230621/setup.py` & `autogluon-0.8.1b20230622/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.1b20230621/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.1b20230622/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230621
+Version: 0.8.1b20230622
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

