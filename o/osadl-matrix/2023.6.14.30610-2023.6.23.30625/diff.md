# Comparing `tmp/osadl-matrix-2023.6.14.30610.tar.gz` & `tmp/osadl-matrix-2023.6.23.30625.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osadl-matrix-2023.6.14.30610.tar", last modified: Wed Jun 14 03:19:16 2023, max compression
+gzip compressed data, was "osadl-matrix-2023.6.23.30625.tar", last modified: Fri Jun 23 03:46:30 2023, max compression
```

## Comparing `osadl-matrix-2023.6.14.30610.tar` & `osadl-matrix-2023.6.23.30625.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/
--rw-r--r--   0 runner    (1001) docker     (123)    18956 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/DATALOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/LICENSE.Unlicensed
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/LICENSE.ccby40
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 03:19:10.000000 osadl-matrix-2023.6.14.30610/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:19:16.811147 osadl-matrix-2023.6.14.30610/osadl_matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/osadl_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38552 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.csv
--rw-r--r--   0 runner    (1001) docker     (123)   213361 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 03:19:16.000000 osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-14 03:19:16.815147 osadl-matrix-2023.6.14.30610/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-14 03:18:41.000000 osadl-matrix-2023.6.14.30610/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:30.570012 osadl-matrix-2023.6.23.30625/
+-rw-r--r--   0 runner    (1001) docker     (123)    18956 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/DATALOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/LICENSE.Unlicensed
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/LICENSE.ccby40
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-23 03:46:30.570012 osadl-matrix-2023.6.23.30625/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 03:46:25.000000 osadl-matrix-2023.6.23.30625/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:30.570012 osadl-matrix-2023.6.23.30625/osadl_matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/osadl_matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38552 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/osadl_matrix/osadl-matrix.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   213361 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/osadl_matrix/osadl-matrix.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:46:30.570012 osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-23 03:46:30.000000 osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-23 03:46:30.000000 osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 03:46:30.000000 osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-23 03:46:30.000000 osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 03:46:30.000000 osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-23 03:46:30.574012 osadl-matrix-2023.6.23.30625/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-23 03:45:56.000000 osadl-matrix-2023.6.23.30625/setup.py
```

### Comparing `osadl-matrix-2023.6.14.30610/DATALOG.md` & `osadl-matrix-2023.6.23.30625/DATALOG.md`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.30610/LICENSE.Unlicensed` & `osadl-matrix-2023.6.23.30625/LICENSE.Unlicensed`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.30610/LICENSE.ccby40` & `osadl-matrix-2023.6.23.30625/LICENSE.ccby40`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.30610/PKG-INFO` & `osadl-matrix-2023.6.23.30625/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2023.6.14.30610
+Version: 2023.6.23.30625
 Summary: OSADL license compatibility matrix
 Home-page: UNKNOWN
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `osadl-matrix-2023.6.14.30610/README.md` & `osadl-matrix-2023.6.23.30625/README.md`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.30610/osadl_matrix/__init__.py` & `osadl-matrix-2023.6.23.30625/osadl_matrix/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-FileCopyrightText: 2021 Konrad Weihmann
 # SPDX-FileCopyrightText: 2023 Henrik Sandklef
 # SPDX-License-Identifier: Unlicensed
 
+import csv
 import json
 import os
 from enum import Enum, unique
 
 OSADL_MATRIX = os.path.join(os.path.dirname(__file__), 'osadl-matrix.csv')
 OSADL_MATRIX_JSON = os.path.join(os.path.dirname(__file__), 'osadl-matrix.json')
 __osadl_db = {}
@@ -39,16 +40,30 @@
 
 
 def __read_db(customdb=None):
     """reads (first call only) matrix file
     """
     global __osadl_db
     if not __osadl_db:
-        with open(customdb or OSADL_MATRIX_JSON) as i:
-            __osadl_db = json.load(i)
+        try:
+            with open(customdb or OSADL_MATRIX_JSON) as i:
+                __osadl_db = json.load(i)
+        except json.JSONDecodeError:
+            if customdb:  # pragma: no cover
+                with open(customdb) as i:
+                    _reader = csv.DictReader(i, delimiter=',', quotechar='"')
+                    for row in _reader:
+                        key = row['Compatibility*']
+                        for k, v in row.items():
+                            if k == 'Compatibility*':
+                                continue
+                            if key not in __osadl_db:
+                                __osadl_db[key] = {}
+                            __osadl_db[key][k] = v
+
 
 def is_compatible(outbound, inbound, customdb=None):
     """checks if the 'outbound' license is compatible with the 'inbound'
    license. If the licenses can be found in the matrix and the
    licenses are compatible, True is returned. In all other cases False
    is returned.
```

### Comparing `osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.csv` & `osadl-matrix-2023.6.23.30625/osadl_matrix/osadl-matrix.csv`

 * *Files identical despite different names*

### Comparing `osadl-matrix-2023.6.14.30610/osadl_matrix/osadl-matrix.json` & `osadl-matrix-2023.6.23.30625/osadl_matrix/osadl-matrix.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946808510638298%*

 * *Differences: {"'timestamp'": "'2023-06-20T02:10:00+00:00'"}*

```diff
@@ -8550,15 +8550,15 @@
         "bzip2-1.0.5": "Yes",
         "bzip2-1.0.6": "Yes",
         "curl": "Yes",
         "libtiff": "Same",
         "zlib-acknowledgement": "Yes"
     },
     "timeformat": "%Y-%m-%dT%H:%M:%S%z",
-    "timestamp": "2023-06-13T02:08:00+00:00",
+    "timestamp": "2023-06-20T02:10:00+00:00",
     "zlib-acknowledgement": {
         "0BSD": "Yes",
         "AFL-2.0": "Yes",
         "AFL-2.1": "Yes",
         "AFL-3.0": "Yes",
         "AGPL-3.0-only": "No",
         "AGPL-3.0-or-later": "No",
```

### Comparing `osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/PKG-INFO` & `osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2023.6.14.30610
+Version: 2023.6.23.30625
 Summary: OSADL license compatibility matrix
 Home-page: UNKNOWN
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `osadl-matrix-2023.6.14.30610/osadl_matrix.egg-info/requires.txt` & `osadl-matrix-2023.6.23.30625/osadl_matrix.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 flake8-2020==1.8.1
 flake8-bandit==4.1.1
 flake8-broken-line==1.0.0
 flake8-bugbear==23.3.12
 flake8-builtins==2.1.0
 flake8-coding==1.3.2
 flake8-commas==2.1.0
-flake8-comprehensions==3.12.0
+flake8-comprehensions==3.13.0
 flake8-debugger==4.1.2
 flake8-docstrings==1.7.0
 flake8-eradicate==1.5.0
 flake8-executable==2.1.3
 flake8-fixme==1.1.1
 flake8-functions==0.0.8
 flake8-isort==6.0.0
```

### Comparing `osadl-matrix-2023.6.14.30610/requirements-dev.txt` & `osadl-matrix-2023.6.23.30625/requirements-dev.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 flake8-2020 == 1.8.1
 flake8-bandit == 4.1.1
 flake8-broken-line == 1.0.0
 flake8-bugbear == 23.3.12
 flake8-builtins == 2.1.0
 flake8-coding == 1.3.2
 flake8-commas == 2.1.0
-flake8-comprehensions == 3.12.0
+flake8-comprehensions == 3.13.0
 flake8-debugger == 4.1.2
 flake8-docstrings == 1.7.0
 flake8-eradicate == 1.5.0
 flake8-executable == 2.1.3
 flake8-fixme == 1.1.1
 flake8-functions == 0.0.8
 flake8-isort == 6.0.0
```

### Comparing `osadl-matrix-2023.6.14.30610/setup.py` & `osadl-matrix-2023.6.23.30625/setup.py`

 * *Files identical despite different names*

