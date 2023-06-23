# Comparing `tmp/scratch-getdata-0.0.4.tar.gz` & `tmp/scratch-getdata-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-0.0.4.tar", last modified: Fri Jun 23 17:33:47 2023, max compression
+gzip compressed data, was "scratch-getdata-0.0.5.tar", last modified: Fri Jun 23 17:42:37 2023, max compression
```

## Comparing `scratch-getdata-0.0.4.tar` & `scratch-getdata-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     2196 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2009 2023-06-23 17:33:30.000000 scratch-getdata-0.0.4/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2196 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:30:32.000000 scratch-getdata-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2287 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2100 2023-06-23 17:42:16.000000 scratch-getdata-0.0.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2287 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:42:37.000000 scratch-getdata-0.0.5/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 17:42:37.600008 scratch-getdata-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:42:32.000000 scratch-getdata-0.0.5/setup.py
```

### Comparing `scratch-getdata-0.0.4/PKG-INFO` & `scratch-getdata-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 
 ScratchAPIClient Documentation
 =============================
 
 Introduction
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
 Github: https://github.com/kokofixcomputers/Scratch-getdata
 
+Install: pip install scratch-getdata
+Import: from scratch_getdata import ScratchAPIClient
+
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
```

### Comparing `scratch-getdata-0.0.4/README.md` & `scratch-getdata-0.0.5/scratch_getdata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+Metadata-Version: 2.1
+Name: scratch-getdata
+Version: 0.0.5
+Summary: A Module to fetch scratch things from ScratchGetData
+Author: kokofixcomputers
+Description-Content-Type: text/markdown
+
 ScratchAPIClient Documentation
 =============================
 
 Introduction
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
 Github: https://github.com/kokofixcomputers/Scratch-getdata
 
+Install: pip install scratch-getdata
+Import: from scratch_getdata import ScratchAPIClient
+
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
```

### Comparing `scratch-getdata-0.0.4/scratch_getdata.egg-info/PKG-INFO` & `scratch-getdata-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-Metadata-Version: 2.1
-Name: scratch-getdata
-Version: 0.0.4
-Summary: A Module to fetch scratch things from ScratchGetData
-Author: kokofixcomputers
-Description-Content-Type: text/markdown
-
 ScratchAPIClient Documentation
 =============================
 
 Introduction
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
 Github: https://github.com/kokofixcomputers/Scratch-getdata
 
+Install: pip install scratch-getdata
+Import: from scratch_getdata import ScratchAPIClient
+
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
```

