# Comparing `tmp/scratch-getdata-0.0.2.tar.gz` & `tmp/scratch-getdata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-0.0.2.tar", last modified: Fri Jun 23 16:56:43 2023, max compression
+gzip compressed data, was "scratch-getdata-0.0.3.tar", last modified: Fri Jun 23 17:28:45 2023, max compression
```

## Comparing `scratch-getdata-0.0.2.tar` & `scratch-getdata-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)      146 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      146 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      202 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      306 2023-06-23 16:56:13.000000 scratch-getdata-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2136 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1949 2023-06-23 17:23:18.000000 scratch-getdata-0.0.3/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2136 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 17:28:45.000000 scratch-getdata-0.0.3/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 17:28:45.292944 scratch-getdata-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:28:23.000000 scratch-getdata-0.0.3/setup.py
```

