# Comparing `tmp/syssqliteaddV2-1.0.0.tar.gz` & `tmp/syssqliteaddV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqliteaddV2-1.0.0.tar", last modified: Fri Jun 23 20:46:48 2023, max compression
+gzip compressed data, was "syssqliteaddV2-1.1.0.tar", last modified: Fri Jun 23 20:48:53 2023, max compression
```

## Comparing `syssqliteaddV2-1.0.0.tar` & `syssqliteaddV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:46:48.368439 syssqliteaddV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-23 20:46:48.368439 syssqliteaddV2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 20:46:48.368439 syssqliteaddV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-06-23 20:46:47.000000 syssqliteaddV2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:46:48.364439 syssqliteaddV2-1.0.0/syssqliteaddV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-23 20:46:47.000000 syssqliteaddV2-1.0.0/syssqliteaddV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:46:48.368439 syssqliteaddV2-1.0.0/syssqliteaddV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-23 20:46:48.000000 syssqliteaddV2-1.0.0/syssqliteaddV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-23 20:46:48.000000 syssqliteaddV2-1.0.0/syssqliteaddV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:46:48.000000 syssqliteaddV2-1.0.0/syssqliteaddV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-23 20:46:48.000000 syssqliteaddV2-1.0.0/syssqliteaddV2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:48:53.988077 syssqliteaddV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-23 20:48:53.988077 syssqliteaddV2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 20:48:53.988077 syssqliteaddV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-06-23 20:48:53.000000 syssqliteaddV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:48:53.988077 syssqliteaddV2-1.1.0/syssqliteaddV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-06-23 20:48:53.000000 syssqliteaddV2-1.1.0/syssqliteaddV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:48:53.988077 syssqliteaddV2-1.1.0/syssqliteaddV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-23 20:48:53.000000 syssqliteaddV2-1.1.0/syssqliteaddV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-23 20:48:53.000000 syssqliteaddV2-1.1.0/syssqliteaddV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:48:53.000000 syssqliteaddV2-1.1.0/syssqliteaddV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-23 20:48:53.000000 syssqliteaddV2-1.1.0/syssqliteaddV2.egg-info/top_level.txt
```

### Comparing `syssqliteaddV2-1.0.0/setup.py` & `syssqliteaddV2-1.1.0/setup.py`

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
     name="syssqliteaddV2",
     version=VERSION,
```

