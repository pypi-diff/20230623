# Comparing `tmp/scratch-getdata-0.0.3.tar.gz` & `tmp/scratch-getdata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-0.0.3.tar", last modified: Fri Jun 23 17:28:45 2023, max compression
+gzip compressed data, was "scratch-getdata-0.0.4.tar", last modified: Fri Jun 23 17:33:47 2023, max compression
```

## Comparing `scratch-getdata-0.0.3.tar` & `scratch-getdata-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     2136 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1949 2023-06-23 17:23:18.000000 scratch-getdata-0.0.3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2136 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:28:23.000000 scratch-getdata-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2196 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2009 2023-06-23 17:33:30.000000 scratch-getdata-0.0.4/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2196 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:33:46.000000 scratch-getdata-0.0.4/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 17:33:47.016156 scratch-getdata-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:30:32.000000 scratch-getdata-0.0.4/setup.py
```

### Comparing `scratch-getdata-0.0.3/PKG-INFO` & `scratch-getdata-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-Metadata-Version: 2.1
-Name: scratch-getdata
-Version: 0.0.3
-Summary: A Module to fetch scratch things from ScratchGetData
-Author: kokofixcomputers
-Description-Content-Type: text/markdown
-
 ScratchAPIClient Documentation
 =============================
 
 Introduction
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
+Github: https://github.com/kokofixcomputers/Scratch-getdata
 
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
```

### Comparing `scratch-getdata-0.0.3/scratch_getdata.egg-info/PKG-INFO` & `scratch-getdata-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Description-Content-Type: text/markdown
 
 ScratchAPIClient Documentation
 =============================
 
 Introduction
 ------------
 The ScratchAPIClient class provides a convenient interface for accessing data from the Scratch API using the "https://scratch-get-data.kokoiscool.repl.co" base URL.
+Github: https://github.com/kokofixcomputers/Scratch-getdata
 
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
```

