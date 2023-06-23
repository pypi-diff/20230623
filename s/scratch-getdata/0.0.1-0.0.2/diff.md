# Comparing `tmp/scratch-getdata-0.0.1.tar.gz` & `tmp/scratch-getdata-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-0.0.1.tar", last modified: Fri Jun 23 16:46:27 2023, max compression
+gzip compressed data, was "scratch-getdata-0.0.2.tar", last modified: Fri Jun 23 16:56:43 2023, max compression
```

## Comparing `scratch-getdata-0.0.1.tar` & `scratch-getdata-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 16:46:27.722039 scratch-getdata-0.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)      146 2023-06-23 16:46:27.718038 scratch-getdata-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1949 2023-06-23 04:47:57.000000 scratch-getdata-0.0.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 16:46:27.718038 scratch-getdata-0.0.1/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      146 2023-06-23 16:46:27.000000 scratch-getdata-0.0.1/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      212 2023-06-23 16:46:27.000000 scratch-getdata-0.0.1/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 16:46:27.000000 scratch-getdata-0.0.1/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 16:46:27.000000 scratch-getdata-0.0.1/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 16:46:27.000000 scratch-getdata-0.0.1/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 16:46:27.722039 scratch-getdata-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      271 2023-06-23 16:44:07.000000 scratch-getdata-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      146 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      146 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      202 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 16:56:43.000000 scratch-getdata-0.0.2/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 16:56:43.382311 scratch-getdata-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      306 2023-06-23 16:56:13.000000 scratch-getdata-0.0.2/setup.py
```

