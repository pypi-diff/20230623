# Comparing `tmp/scratch-getdata-0.0.7.tar.gz` & `tmp/scratch-getdata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-0.0.7.tar", last modified: Fri Jun 23 18:14:02 2023, max compression
+gzip compressed data, was "scratch-getdata-0.0.8.tar", last modified: Fri Jun 23 18:23:38 2023, max compression
```

## Comparing `scratch-getdata-0.0.7.tar` & `scratch-getdata-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:14:02.029959 scratch-getdata-0.0.7/
--rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-23 18:14:02.029959 scratch-getdata-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2100 2023-06-23 17:42:16.000000 scratch-getdata-0.0.7/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      633 2023-06-23 18:13:57.000000 scratch-getdata-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:14:02.029959 scratch-getdata-0.0.7/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-23 18:14:01.000000 scratch-getdata-0.0.7/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      227 2023-06-23 18:14:01.000000 scratch-getdata-0.0.7/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 18:14:01.000000 scratch-getdata-0.0.7/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 18:14:01.000000 scratch-getdata-0.0.7/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 18:14:01.000000 scratch-getdata-0.0.7/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 18:14:02.029959 scratch-getdata-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:56:58.000000 scratch-getdata-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:23:38.689966 scratch-getdata-0.0.8/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-23 18:23:38.689966 scratch-getdata-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2100 2023-06-23 17:42:16.000000 scratch-getdata-0.0.8/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      633 2023-06-23 18:21:36.000000 scratch-getdata-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:23:38.689966 scratch-getdata-0.0.8/scratch_getdata/
+-rw-r--r--   0 runner    (1000) runner    (1000)      525 2023-06-23 18:21:11.000000 scratch-getdata-0.0.8/scratch_getdata/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2670 2023-06-23 18:21:14.000000 scratch-getdata-0.0.8/scratch_getdata/api_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:23:38.689966 scratch-getdata-0.0.8/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-23 18:23:38.000000 scratch-getdata-0.0.8/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-06-23 18:23:38.000000 scratch-getdata-0.0.8/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 18:23:38.000000 scratch-getdata-0.0.8/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 18:23:38.000000 scratch-getdata-0.0.8/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-23 18:23:38.000000 scratch-getdata-0.0.8/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 18:23:38.689966 scratch-getdata-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:56:58.000000 scratch-getdata-0.0.8/setup.py
```

### Comparing `scratch-getdata-0.0.7/PKG-INFO` & `scratch-getdata-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <none@none.com>
 Project-URL: Homepage, https://github.com/kokofixcomputers/Scratch-getdata
 Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scratch-getdata-0.0.7/README.md` & `scratch-getdata-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scratch-getdata-0.0.7/pyproject.toml` & `scratch-getdata-0.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scratch-getdata"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="kokofixcomputers", email="none@none.com" },
 ]
 description = "A Module to fetch scratch things from ScratchGetData"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scratch-getdata-0.0.7/scratch_getdata.egg-info/PKG-INFO` & `scratch-getdata-0.0.8/scratch_getdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <none@none.com>
 Project-URL: Homepage, https://github.com/kokofixcomputers/Scratch-getdata
 Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

