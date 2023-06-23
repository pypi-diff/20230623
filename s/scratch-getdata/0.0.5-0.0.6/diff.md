# Comparing `tmp/scratch-getdata-0.0.5.tar.gz` & `tmp/scratch_getdata-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-0.0.5.tar", last modified: Fri Jun 23 17:42:37 2023, max compression
+gzip compressed data, was "scratch_getdata-0.0.6.tar", last modified: Fri Jun 23 17:57:14 2023, max compression
```

## Comparing `scratch-getdata-0.0.5.tar` & `scratch_getdata-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     2287 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2100 2023-06-23 17:42:16.000000 scratch-getdata-0.0.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2287 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:42:32.000000 scratch-getdata-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:57:14.539096 scratch_getdata-0.0.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2287 2023-06-23 17:57:14.539096 scratch_getdata-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2100 2023-06-23 17:42:16.000000 scratch_getdata-0.0.6/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:57:14.539096 scratch_getdata-0.0.6/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2287 2023-06-23 17:57:14.000000 scratch_getdata-0.0.6/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 17:57:14.000000 scratch_getdata-0.0.6/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:57:14.000000 scratch_getdata-0.0.6/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 17:57:14.000000 scratch_getdata-0.0.6/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:57:14.000000 scratch_getdata-0.0.6/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 17:57:14.539096 scratch_getdata-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:56:58.000000 scratch_getdata-0.0.6/setup.py
```

### Comparing `scratch-getdata-0.0.5/PKG-INFO` & `scratch_getdata-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scratch-getdata
-Version: 0.0.5
+Name: scratch_getdata
+Version: 0.0.6
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 
 ScratchAPIClient Documentation
 =============================
```

### Comparing `scratch-getdata-0.0.5/README.md` & `scratch_getdata-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `scratch-getdata-0.0.5/scratch_getdata.egg-info/PKG-INFO` & `scratch_getdata-0.0.6/scratch_getdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 
 ScratchAPIClient Documentation
 =============================
```

