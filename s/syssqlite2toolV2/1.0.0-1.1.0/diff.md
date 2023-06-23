# Comparing `tmp/syssqlite2toolV2-1.0.0.tar.gz` & `tmp/syssqlite2toolV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlite2toolV2-1.0.0.tar", last modified: Fri Jun 23 21:03:36 2023, max compression
+gzip compressed data, was "syssqlite2toolV2-1.1.0.tar", last modified: Fri Jun 23 21:05:41 2023, max compression
```

## Comparing `syssqlite2toolV2-1.0.0.tar` & `syssqlite2toolV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:03:36.129515 syssqlite2toolV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-23 21:03:36.125515 syssqlite2toolV2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 21:03:36.129515 syssqlite2toolV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2023-06-23 21:03:35.000000 syssqlite2toolV2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:03:36.125515 syssqlite2toolV2-1.0.0/syssqlite2toolV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-23 21:03:35.000000 syssqlite2toolV2-1.0.0/syssqlite2toolV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:03:36.125515 syssqlite2toolV2-1.0.0/syssqlite2toolV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-23 21:03:35.000000 syssqlite2toolV2-1.0.0/syssqlite2toolV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-23 21:03:36.000000 syssqlite2toolV2-1.0.0/syssqlite2toolV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:03:35.000000 syssqlite2toolV2-1.0.0/syssqlite2toolV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-23 21:03:35.000000 syssqlite2toolV2-1.0.0/syssqlite2toolV2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:05:41.685149 syssqlite2toolV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-23 21:05:41.685149 syssqlite2toolV2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 21:05:41.685149 syssqlite2toolV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-06-23 21:05:41.000000 syssqlite2toolV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:05:41.681149 syssqlite2toolV2-1.1.0/syssqlite2toolV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-06-23 21:05:41.000000 syssqlite2toolV2-1.1.0/syssqlite2toolV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:05:41.685149 syssqlite2toolV2-1.1.0/syssqlite2toolV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-23 21:05:41.000000 syssqlite2toolV2-1.1.0/syssqlite2toolV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-23 21:05:41.000000 syssqlite2toolV2-1.1.0/syssqlite2toolV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:05:41.000000 syssqlite2toolV2-1.1.0/syssqlite2toolV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-23 21:05:41.000000 syssqlite2toolV2-1.1.0/syssqlite2toolV2.egg-info/top_level.txt
```

### Comparing `syssqlite2toolV2-1.0.0/setup.py` & `syssqlite2toolV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syssqlite2toolV2",
     version=VERSION,
```

