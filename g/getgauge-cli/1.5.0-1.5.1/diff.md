# Comparing `tmp/getgauge-cli-1.5.0.tar.gz` & `tmp/getgauge-cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/getgauge-cli-1.5.0.tar", last modified: Thu Jun 22 13:28:58 2023, max compression
+gzip compressed data, was "dist/getgauge-cli-1.5.1.tar", last modified: Fri Jun 23 15:01:08 2023, max compression
```

## Comparing `getgauge-cli-1.5.0.tar` & `getgauge-cli-1.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 13:28:47.000000 getgauge-cli-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-22 13:28:47.000000 getgauge-cli-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/getgauge_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/getgauge_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/getgauge_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/getgauge_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/getgauge_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/getgauge_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:28:58.000000 getgauge-cli-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-22 13:28:56.000000 getgauge-cli-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 15:01:00.000000 getgauge-cli-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-23 15:01:00.000000 getgauge-cli-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-23 15:01:07.000000 getgauge-cli-1.5.1/setup.py
```

### Comparing `getgauge-cli-1.5.0/PKG-INFO` & `getgauge-cli-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.5.0
+Version: 1.5.1
 Summary: UNKNOWN
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
 Description: # PIP Installer for getgauge-cli tool
```

### Comparing `getgauge-cli-1.5.0/README.md` & `getgauge-cli-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `getgauge-cli-1.5.0/getgauge_cli.egg-info/PKG-INFO` & `getgauge-cli-1.5.1/getgauge_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.5.0
+Version: 1.5.1
 Summary: UNKNOWN
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
 Description: # PIP Installer for getgauge-cli tool
```

### Comparing `getgauge-cli-1.5.0/setup.py` & `getgauge-cli-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import platform
 import zipfile
 import os
 import sys
 
 
-_version = "1.5.0"
+_version = "1.5.1"
 _latest_version = ""
 
 
 class CustomInstallCommand(install):
     """Customized setuptools install command to download and setup."""
 
     _base_url = 'https://api.github.com/repos/getgauge/gauge/releases'
```

