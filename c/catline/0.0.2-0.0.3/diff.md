# Comparing `tmp/catline-0.0.2.tar.gz` & `tmp/catline-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catline-0.0.2.tar", last modified: Fri Jun 23 10:29:25 2023, max compression
+gzip compressed data, was "catline-0.0.3.tar", last modified: Fri Jun 23 10:40:43 2023, max compression
```

## Comparing `catline-0.0.2.tar` & `catline-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 10:29:11.000000 catline-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 10:29:11.000000 catline-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-23 10:29:25.830224 catline-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-23 10:29:11.000000 catline-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/catline/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 10:29:11.000000 catline-0.0.2/catline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 10:29:25.830224 catline-0.0.2/catline/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/catline/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:11.000000 catline-0.0.2/catline/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-23 10:29:11.000000 catline-0.0.2/catline/adapters/json_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-23 10:29:11.000000 catline-0.0.2/catline/adapters/redis_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-23 10:29:11.000000 catline-0.0.2/catline/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-23 10:29:11.000000 catline-0.0.2/catline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/catline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 10:29:11.000000 catline-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:29:11.000000 catline-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-23 10:29:25.830224 catline-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-23 10:29:11.000000 catline-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-23 10:29:11.000000 catline-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:40:43.317345 catline-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 10:40:27.000000 catline-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 10:40:27.000000 catline-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-23 10:40:43.317345 catline-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-23 10:40:27.000000 catline-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:40:43.317345 catline-0.0.3/catline/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 10:40:27.000000 catline-0.0.3/catline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 10:40:43.317345 catline-0.0.3/catline/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:40:43.317345 catline-0.0.3/catline/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 10:40:27.000000 catline-0.0.3/catline/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-23 10:40:27.000000 catline-0.0.3/catline/adapters/json_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-23 10:40:27.000000 catline-0.0.3/catline/adapters/redis_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-23 10:40:27.000000 catline-0.0.3/catline/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-23 10:40:27.000000 catline-0.0.3/catline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:40:43.317345 catline-0.0.3/catline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-23 10:40:43.000000 catline-0.0.3/catline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 10:40:43.000000 catline-0.0.3/catline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:40:43.000000 catline-0.0.3/catline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 10:40:43.000000 catline-0.0.3/catline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 10:40:43.000000 catline-0.0.3/catline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 10:40:27.000000 catline-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:40:27.000000 catline-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-23 10:40:43.317345 catline-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-23 10:40:27.000000 catline-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-23 10:40:27.000000 catline-0.0.3/versioneer.py
```

### Comparing `catline-0.0.2/LICENSE` & `catline-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `catline-0.0.2/PKG-INFO` & `catline-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catline
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple job queue
 Home-page: https://github.com/yupix/catline
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `catline-0.0.2/README.md` & `catline-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `catline-0.0.2/catline/adapters/json_adapter.py` & `catline-0.0.3/catline/adapters/json_adapter.py`

 * *Files identical despite different names*

### Comparing `catline-0.0.2/catline/adapters/redis_adapter.py` & `catline-0.0.3/catline/adapters/redis_adapter.py`

 * *Files identical despite different names*

### Comparing `catline-0.0.2/catline/queue.py` & `catline-0.0.3/catline/queue.py`

 * *Files identical despite different names*

### Comparing `catline-0.0.2/catline.egg-info/PKG-INFO` & `catline-0.0.3/catline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catline
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple job queue
 Home-page: https://github.com/yupix/catline
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `catline-0.0.2/setup.py` & `catline-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `catline-0.0.2/versioneer.py` & `catline-0.0.3/versioneer.py`

 * *Files identical despite different names*

