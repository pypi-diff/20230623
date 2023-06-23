# Comparing `tmp/ospx-0.2.8.tar.gz` & `tmp/ospx-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospx-0.2.8.tar", last modified: Wed Jan 11 12:43:42 2023, max compression
+gzip compressed data, was "ospx-0.2.9.tar", last modified: Thu May  4 14:31:14 2023, max compression
```

## Comparing `ospx-0.2.8.tar` & `ospx-0.2.9.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.803339 ospx-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-11 12:43:19.000000 ospx-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-11 12:43:19.000000 ospx-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-01-11 12:43:42.803339 ospx-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-01-11 12:43:19.000000 ospx-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-01-11 12:43:19.000000 ospx-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-01-11 12:43:42.803339 ospx-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.791339 ospx-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.795339 ospx-0.2.8/src/ospx/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.799339 ospx-0.2.8/src/ospx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/cli/importSystemStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/cli/ospCaseBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12878 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.799339 ospx-0.2.8/src/ospx/fmi/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/fmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/fmi/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/fmi/fmu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/fmi/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/fmi/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/ospCaseBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)    29107 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/ospSimulationCase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.799339 ospx-0.2.8/src/ospx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/utils/dateTime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.803339 ospx-0.2.8/src/ospx/watch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/watch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.803339 ospx-0.2.8/src/ospx/watch/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/watch/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/watch/cli/watchCosim.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-01-11 12:43:19.000000 ospx-0.2.8/src/ospx/watch/watchCosim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:43:42.799339 ospx-0.2.8/src/ospx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-01-11 12:43:42.000000 ospx-0.2.8/src/ospx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-01-11 12:43:42.000000 ospx-0.2.8/src/ospx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 12:43:42.000000 ospx-0.2.8/src/ospx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-11 12:43:42.000000 ospx-0.2.8/src/ospx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-11 12:43:42.000000 ospx-0.2.8/src/ospx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-11 12:43:42.000000 ospx-0.2.8/src/ospx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 14:30:54.000000 ospx-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 14:30:54.000000 ospx-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-04 14:31:14.714388 ospx-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-04 14:30:54.000000 ospx-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-04 14:30:54.000000 ospx-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-04 14:31:14.714388 ospx-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.710388 ospx-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.710388 ospx-0.2.9/src/ospx/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/src/ospx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/cli/importSystemStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/cli/ospCaseBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/src/ospx/fmi/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/fmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/fmi/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/fmi/fmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/fmi/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/fmi/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/ospCaseBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29091 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/ospSimulationCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/src/ospx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/utils/dateTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/src/ospx/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/watch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/src/ospx/watch/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/watch/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/watch/cli/watchCosim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-05-04 14:30:54.000000 ospx-0.2.9/src/ospx/watch/watchCosim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/src/ospx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-04 14:31:14.000000 ospx-0.2.9/src/ospx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-04 14:31:14.000000 ospx-0.2.9/src/ospx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:31:14.000000 ospx-0.2.9/src/ospx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 14:31:14.000000 ospx-0.2.9/src/ospx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 14:31:14.000000 ospx-0.2.9/src/ospx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 14:31:14.000000 ospx-0.2.9/src/ospx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:14.714388 ospx-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-04 14:30:54.000000 ospx-0.2.9/tests/test_fmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-04 14:30:54.000000 ospx-0.2.9/tests/test_ospCaseBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-04 14:30:54.000000 ospx-0.2.9/tests/test_watchCosim.py
```

### Comparing `ospx-0.2.8/LICENSE` & `ospx-0.2.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ospx-0.2.8/PKG-INFO` & `ospx-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ospx
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension package to farn, adding support to build OSP simulation cases using FMUs
 Home-page: https://dnv-opensource.github.io/ospx/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
 Project-URL: GitHub, https://github.com/dnv-opensource/ospx
 Platform: Python3.x
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -106,15 +107,15 @@
     ~~~sh
     $ pip install -r requirements.txt
     ~~~
 
 
 ## Meta
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
```

### Comparing `ospx-0.2.8/README.md` & `ospx-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     ~~~sh
     $ pip install -r requirements.txt
     ~~~
 
 
 ## Meta
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
```

### Comparing `ospx-0.2.8/pyproject.toml` & `ospx-0.2.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -52,126 +52,174 @@
 00000330: 6e67 2073 756d 6d61 7279 2073 686f 756c  ng summary shoul
 00000340: 6420 7374 6172 7420 6174 2074 6865 2066  d start at the f
 00000350: 6972 7374 206c 696e 650d 0a20 2020 2022  irst line..    "
 00000360: 4432 3133 222c 2020 2320 4d75 6c74 692d  D213",  # Multi-
 00000370: 6c69 6e65 2064 6f63 7374 7269 6e67 2073  line docstring s
 00000380: 756d 6d61 7279 2073 686f 756c 6420 7374  ummary should st
 00000390: 6172 7420 6174 2074 6865 2073 6563 6f6e  art at the secon
-000003a0: 6420 6c69 6e65 0d0a 2020 2020 5d0d 0a6c  d line..    ]..l
-000003b0: 696e 652d 6c65 6e67 7468 203d 2031 3230  ine-length = 120
-000003c0: 0d0a 7365 6c65 6374 203d 205b 0d0a 2020  ..select = [..  
-000003d0: 2020 2245 222c 0d0a 2020 2020 2244 222c    "E",..    "D",
-000003e0: 0d0a 2020 2020 2246 222c 0d0a 2020 2020  ..    "F",..    
-000003f0: 224e 222c 0d0a 2020 2020 2257 222c 0d0a  "N",..    "W",..
-00000400: 2020 2020 2249 222c 0d0a 2020 2020 2242      "I",..    "B
-00000410: 222c 0d0a 5d0d 0a74 6172 6765 742d 7665  ",..]..target-ve
-00000420: 7273 696f 6e20 3d20 2270 7933 3922 0d0a  rsion = "py39"..
-00000430: 0d0a 5b74 6f6f 6c2e 7275 6666 2e70 6570  ..[tool.ruff.pep
-00000440: 382d 6e61 6d69 6e67 5d0d 0a69 676e 6f72  8-naming]..ignor
-00000450: 652d 6e61 6d65 7320 3d20 5b0d 0a20 2020  e-names = [..   
-00000460: 2022 7465 7374 5f2a 222c 0d0a 2020 2020   "test_*",..    
-00000470: 2273 6574 5570 222c 0d0a 2020 2020 2274  "setUp",..    "t
-00000480: 6561 7244 6f77 6e22 2c0d 0a5d 0d0a 0d0a  earDown",..]....
-00000490: 5b74 6f6f 6c2e 7275 6666 2e70 7964 6f63  [tool.ruff.pydoc
-000004a0: 7374 796c 655d 0d0a 636f 6e76 656e 7469  style]..conventi
-000004b0: 6f6e 203d 2022 6e75 6d70 7922 0d0a 0d0a  on = "numpy"....
-000004c0: 5b74 6f6f 6c2e 7275 6666 2e70 6572 2d66  [tool.ruff.per-f
-000004d0: 696c 652d 6967 6e6f 7265 735d 0d0a 225f  ile-ignores].."_
-000004e0: 5f69 6e69 745f 5f2e 7079 2220 3d20 5b22  _init__.py" = ["
-000004f0: 4930 3031 225d 0d0a 222e 2f74 6573 7473  I001"].."./tests
-00000500: 2f2a 2220 3d20 5b22 4422 5d0d 0a0d 0a5b  /*" = ["D"]....[
-00000510: 746f 6f6c 2e70 7972 6967 6874 5d0d 0a65  tool.pyright]..e
-00000520: 7863 6c75 6465 203d 205b 0d0a 2020 2020  xclude = [..    
-00000530: 222e 6769 7422 2c0d 0a20 2020 2022 2e76  ".git",..    ".v
-00000540: 656e 7622 2c0d 0a20 2020 2022 2e74 6f78  env",..    ".tox
-00000550: 222c 0d0a 2020 2020 2262 7569 6c64 222c  ",..    "build",
-00000560: 0d0a 2020 2020 2264 6973 7422 2c0d 0a20  ..    "dist",.. 
-00000570: 2020 2022 2a2a 2f5f 5f70 7963 6163 6865     "**/__pycache
-00000580: 5f5f 222c 0d0a 2020 2020 222e 2f64 6f63  __",..    "./doc
-00000590: 732f 736f 7572 6365 2f63 6f6e 662e 7079  s/source/conf.py
-000005a0: 222c 0d0a 5d0d 0a65 7874 7261 5061 7468  ",..]..extraPath
-000005b0: 7320 3d20 5b22 2e2f 7372 6322 5d0d 0a74  s = ["./src"]..t
-000005c0: 7970 6543 6865 636b 696e 674d 6f64 6520  ypeCheckingMode 
-000005d0: 3d20 2262 6173 6963 220d 0a75 7365 4c69  = "basic"..useLi
-000005e0: 6272 6172 7943 6f64 6546 6f72 5479 7065  braryCodeForType
-000005f0: 7320 3d20 7472 7565 0d0a 7265 706f 7274  s = true..report
-00000600: 4d69 7373 696e 6750 6172 616d 6574 6572  MissingParameter
-00000610: 5479 7065 203d 2022 6572 726f 7222 0d0a  Type = "error"..
-00000620: 7265 706f 7274 556e 6b6e 6f77 6e50 6172  reportUnknownPar
-00000630: 616d 6574 6572 5479 7065 203d 2022 7761  ameterType = "wa
-00000640: 726e 696e 6722 0d0a 7265 706f 7274 556e  rning"..reportUn
-00000650: 6b6e 6f77 6e4d 656d 6265 7254 7970 6520  knownMemberType 
-00000660: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-00000670: 6f72 744d 6973 7369 6e67 5479 7065 4172  ortMissingTypeAr
-00000680: 6775 6d65 6e74 203d 2022 6572 726f 7222  gument = "error"
-00000690: 0d0a 7265 706f 7274 5072 6f70 6572 7479  ..reportProperty
-000006a0: 5479 7065 4d69 736d 6174 6368 203d 2022  TypeMismatch = "
-000006b0: 6572 726f 7222 0d0a 7265 706f 7274 4675  error"..reportFu
-000006c0: 6e63 7469 6f6e 4d65 6d62 6572 4163 6365  nctionMemberAcce
-000006d0: 7373 203d 2022 7761 726e 696e 6722 0d0a  ss = "warning"..
-000006e0: 7265 706f 7274 5072 6976 6174 6555 7361  reportPrivateUsa
-000006f0: 6765 203d 2022 7761 726e 696e 6722 0d0a  ge = "warning"..
-00000700: 7265 706f 7274 5479 7065 436f 6d6d 656e  reportTypeCommen
-00000710: 7455 7361 6765 203d 2022 7761 726e 696e  tUsage = "warnin
-00000720: 6722 0d0a 7265 706f 7274 496e 636f 6d70  g"..reportIncomp
-00000730: 6174 6962 6c65 4d65 7468 6f64 4f76 6572  atibleMethodOver
-00000740: 7269 6465 203d 2022 7761 726e 696e 6722  ride = "warning"
-00000750: 0d0a 7265 706f 7274 496e 636f 6d70 6174  ..reportIncompat
-00000760: 6962 6c65 5661 7269 6162 6c65 4f76 6572  ibleVariableOver
-00000770: 7269 6465 203d 2022 6572 726f 7222 0d0a  ride = "error"..
-00000780: 7265 706f 7274 496e 636f 6e73 6973 7465  reportInconsiste
-00000790: 6e74 436f 6e73 7472 7563 746f 7220 3d20  ntConstructor = 
-000007a0: 2265 7272 6f72 220d 0a72 6570 6f72 744f  "error"..reportO
-000007b0: 7665 726c 6170 7069 6e67 4f76 6572 6c6f  verlappingOverlo
-000007c0: 6164 203d 2022 7761 726e 696e 6722 0d0a  ad = "warning"..
-000007d0: 7265 706f 7274 556e 696e 6974 6961 6c69  reportUninitiali
-000007e0: 7a65 6449 6e73 7461 6e63 6556 6172 6961  zedInstanceVaria
-000007f0: 626c 6520 3d20 2277 6172 6e69 6e67 220d  ble = "warning".
-00000800: 0a72 6570 6f72 7443 616c 6c49 6e44 6566  .reportCallInDef
-00000810: 6175 6c74 496e 6974 6961 6c69 7a65 7220  aultInitializer 
-00000820: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-00000830: 6f72 7455 6e6e 6563 6573 7361 7279 4973  ortUnnecessaryIs
-00000840: 496e 7374 616e 6365 203d 2022 696e 666f  Instance = "info
-00000850: 726d 6174 696f 6e22 0d0a 7265 706f 7274  rmation"..report
-00000860: 556e 6e65 6365 7373 6172 7943 6173 7420  UnnecessaryCast 
-00000870: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-00000880: 6f72 7455 6e6e 6563 6573 7361 7279 436f  ortUnnecessaryCo
-00000890: 6d70 6172 6973 6f6e 203d 2022 7761 726e  mparison = "warn
-000008a0: 696e 6722 0d0a 7265 706f 7274 556e 6e65  ing"..reportUnne
-000008b0: 6365 7373 6172 7943 6f6e 7461 696e 7320  cessaryContains 
-000008c0: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-000008d0: 6f72 7455 6e75 7365 6443 616c 6c52 6573  ortUnusedCallRes
-000008e0: 756c 7420 3d20 2277 6172 6e69 6e67 220d  ult = "warning".
-000008f0: 0a72 6570 6f72 7455 6e75 7365 6445 7870  .reportUnusedExp
-00000900: 7265 7373 696f 6e20 3d20 2277 6172 6e69  ression = "warni
-00000910: 6e67 220d 0a72 6570 6f72 744d 6174 6368  ng"..reportMatch
-00000920: 4e6f 7445 7868 6175 7374 6976 6520 3d20  NotExhaustive = 
-00000930: 2277 6172 6e69 6e67 220d 0a72 6570 6f72  "warning"..repor
-00000940: 7453 6861 646f 7765 6449 6d70 6f72 7473  tShadowedImports
-00000950: 203d 2022 7761 726e 696e 6722 0d0a 7265   = "warning"..re
-00000960: 706f 7274 556e 7479 7065 6446 756e 6374  portUntypedFunct
-00000970: 696f 6e44 6563 6f72 6174 6f72 203d 2022  ionDecorator = "
-00000980: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
-00000990: 556e 7479 7065 6442 6173 6543 6c61 7373  UntypedBaseClass
-000009a0: 203d 2022 6572 726f 7222 0d0a 7265 706f   = "error"..repo
-000009b0: 7274 556e 7479 7065 644e 616d 6564 5475  rtUntypedNamedTu
-000009c0: 706c 6520 3d20 2277 6172 6e69 6e67 220d  ple = "warning".
-000009d0: 0a23 2041 6374 6976 6174 6520 7468 6520  .# Activate the 
-000009e0: 666f 6c6c 6f77 696e 6720 7275 6c65 7320  following rules 
-000009f0: 6f6e 6c79 206c 6f63 616c 6c79 2061 6e64  only locally and
-00000a00: 2074 656d 706f 7261 7279 2c20 692e 652e   temporary, i.e.
-00000a10: 2066 6f72 2061 2051 4120 7365 7373 696f   for a QA sessio
-00000a20: 6e2e 0d0a 2320 2846 6f72 2073 6572 7665  n...# (For serve
-00000a30: 7220 7369 6465 2043 4920 7468 6579 2061  r side CI they a
-00000a40: 7265 2063 6f6e 7369 6465 7265 6420 746f  re considered to
-00000a50: 6f20 7374 7269 6374 2e29 0d0a 2320 7265  o strict.)..# re
-00000a60: 706f 7274 436f 6e73 7461 6e74 5265 6465  portConstantRede
-00000a70: 6669 6e69 7469 6f6e 203d 2022 7761 726e  finition = "warn
-00000a80: 696e 6722 0d0a 2320 7265 706f 7274 556e  ing"..# reportUn
-00000a90: 6e65 6365 7373 6172 7954 7970 6549 676e  necessaryTypeIgn
-00000aa0: 6f72 6543 6f6d 6d65 6e74 203d 2022 696e  oreComment = "in
-00000ab0: 666f 726d 6174 696f 6e22 0d0a 2320 7265  formation"..# re
-00000ac0: 706f 7274 496d 706f 7274 4379 636c 6573  portImportCycles
-00000ad0: 203d 2022 7761 726e 696e 6722 0d0a 2320   = "warning"..# 
-00000ae0: 7265 706f 7274 496d 706c 6963 6974 5374  reportImplicitSt
-00000af0: 7269 6e67 436f 6e63 6174 656e 6174 696f  ringConcatenatio
-00000b00: 6e20 3d20 2277 6172 6e69 6e67 220d 0a    n = "warning"..
+000003a0: 6420 6c69 6e65 0d0a 2020 2020 2320 224e  d line..    # "N
+000003b0: 3830 3222 2c20 2023 2046 756e 6374 696f  802",  # Functio
+000003c0: 6e20 6e61 6d65 2073 686f 756c 6420 6265  n name should be
+000003d0: 206c 6f77 6572 6361 7365 2020 2875 6e63   lowercase  (unc
+000003e0: 6f6d 6d65 6e74 2069 6620 796f 7520 7761  omment if you wa
+000003f0: 6e74 2074 6f20 616c 6c6f 7720 5570 7065  nt to allow Uppe
+00000400: 7263 6173 6520 6675 6e63 7469 6f6e 206e  rcase function n
+00000410: 616d 6573 290d 0a20 2020 2023 2022 4e38  ames)..    # "N8
+00000420: 3033 222c 2020 2320 4172 6775 6d65 6e74  03",  # Argument
+00000430: 206e 616d 6520 7368 6f75 6c64 2062 6520   name should be 
+00000440: 6c6f 7765 7263 6173 6520 2028 756e 636f  lowercase  (unco
+00000450: 6d6d 656e 7420 6966 2079 6f75 2077 616e  mment if you wan
+00000460: 7420 746f 2061 6c6c 6f77 2055 7070 6572  t to allow Upper
+00000470: 6361 7365 2061 7267 756d 656e 7420 6e61  case argument na
+00000480: 6d65 7329 0d0a 2020 2020 224e 3830 3622  mes)..    "N806"
+00000490: 2c20 2023 2056 6172 6961 626c 6520 696e  ,  # Variable in
+000004a0: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
+000004b0: 2062 6520 6c6f 7765 7263 6173 6520 2028   be lowercase  (
+000004c0: 756e 636f 6d6d 656e 7420 6966 2079 6f75  uncomment if you
+000004d0: 2077 616e 7420 746f 2061 6c6c 6f77 2055   want to allow U
+000004e0: 7070 6572 6361 7365 2076 6172 6961 626c  ppercase variabl
+000004f0: 6520 6e61 6d65 7320 696e 2066 756e 6374  e names in funct
+00000500: 696f 6e73 290d 0a20 2020 2023 2022 4e38  ions)..    # "N8
+00000510: 3135 222c 2020 2320 5661 7269 6162 6c65  15",  # Variable
+00000520: 2069 6e20 636c 6173 7320 7363 6f70 6520   in class scope 
+00000530: 7368 6f75 6c64 206e 6f74 2062 6520 6d69  should not be mi
+00000540: 7865 6443 6173 6520 2028 756e 636f 6d6d  xedCase  (uncomm
+00000550: 656e 7420 6966 2079 6f75 2077 616e 7420  ent if you want 
+00000560: 746f 2061 6c6c 6f77 206d 6978 6564 4361  to allow mixedCa
+00000570: 7365 2076 6172 6961 626c 6520 6e61 6d65  se variable name
+00000580: 7320 696e 2063 6c61 7373 2073 636f 7065  s in class scope
+00000590: 290d 0a20 2020 2023 2022 4e38 3136 222c  )..    # "N816",
+000005a0: 2020 2320 5661 7269 6162 6c65 2069 6e20    # Variable in 
+000005b0: 676c 6f62 616c 2073 636f 7065 2073 686f  global scope sho
+000005c0: 756c 6420 6e6f 7420 6265 206d 6978 6564  uld not be mixed
+000005d0: 4361 7365 2020 2875 6e63 6f6d 6d65 6e74  Case  (uncomment
+000005e0: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
+000005f0: 616c 6c6f 7720 6d69 7865 6443 6173 6520  allow mixedCase 
+00000600: 7661 7269 6162 6c65 206e 616d 6573 2069  variable names i
+00000610: 6e20 676c 6f62 616c 2073 636f 7065 290d  n global scope).
+00000620: 0a20 2020 2022 4e39 3939 222c 2020 2320  .    "N999",  # 
+00000630: 496e 7661 6c69 6420 6d6f 6475 6c65 206e  Invalid module n
+00000640: 616d 650d 0a20 2020 205d 0d0a 6c69 6e65  ame..    ]..line
+00000650: 2d6c 656e 6774 6820 3d20 3132 300d 0a73  -length = 120..s
+00000660: 656c 6563 7420 3d20 5b0d 0a20 2020 2022  elect = [..    "
+00000670: 4522 2c0d 0a20 2020 2022 4422 2c0d 0a20  E",..    "D",.. 
+00000680: 2020 2022 4622 2c0d 0a20 2020 2022 4e22     "F",..    "N"
+00000690: 2c0d 0a20 2020 2022 5722 2c0d 0a20 2020  ,..    "W",..   
+000006a0: 2022 4922 2c0d 0a20 2020 2022 4222 2c0d   "I",..    "B",.
+000006b0: 0a5d 0d0a 7461 7267 6574 2d76 6572 7369  .]..target-versi
+000006c0: 6f6e 203d 2022 7079 3339 220d 0a0d 0a5b  on = "py39"....[
+000006d0: 746f 6f6c 2e72 7566 662e 7065 7038 2d6e  tool.ruff.pep8-n
+000006e0: 616d 696e 675d 0d0a 6967 6e6f 7265 2d6e  aming]..ignore-n
+000006f0: 616d 6573 203d 205b 0d0a 2020 2020 2274  ames = [..    "t
+00000700: 6573 745f 2a22 2c0d 0a20 2020 2022 7365  est_*",..    "se
+00000710: 7455 7022 2c0d 0a20 2020 2022 7465 6172  tUp",..    "tear
+00000720: 446f 776e 222c 0d0a 5d0d 0a0d 0a5b 746f  Down",..]....[to
+00000730: 6f6c 2e72 7566 662e 7079 646f 6373 7479  ol.ruff.pydocsty
+00000740: 6c65 5d0d 0a63 6f6e 7665 6e74 696f 6e20  le]..convention 
+00000750: 3d20 226e 756d 7079 220d 0a0d 0a5b 746f  = "numpy"....[to
+00000760: 6f6c 2e72 7566 662e 7065 722d 6669 6c65  ol.ruff.per-file
+00000770: 2d69 676e 6f72 6573 5d0d 0a22 5f5f 696e  -ignores].."__in
+00000780: 6974 5f5f 2e70 7922 203d 205b 2249 3030  it__.py" = ["I00
+00000790: 3122 5d0d 0a22 2e2f 7465 7374 732f 2a22  1"].."./tests/*"
+000007a0: 203d 205b 2244 225d 0d0a 0d0a 5b74 6f6f   = ["D"]....[too
+000007b0: 6c2e 7079 7269 6768 745d 0d0a 6578 636c  l.pyright]..excl
+000007c0: 7564 6520 3d20 5b0d 0a20 2020 2022 2e67  ude = [..    ".g
+000007d0: 6974 222c 0d0a 2020 2020 222e 7665 6e76  it",..    ".venv
+000007e0: 222c 0d0a 2020 2020 222e 746f 7822 2c0d  ",..    ".tox",.
+000007f0: 0a20 2020 2022 6275 696c 6422 2c0d 0a20  .    "build",.. 
+00000800: 2020 2022 6469 7374 222c 0d0a 2020 2020     "dist",..    
+00000810: 222a 2a2f 5f5f 7079 6361 6368 655f 5f22  "**/__pycache__"
+00000820: 2c0d 0a20 2020 2022 2e2f 646f 6373 2f73  ,..    "./docs/s
+00000830: 6f75 7263 652f 636f 6e66 2e70 7922 2c0d  ource/conf.py",.
+00000840: 0a5d 0d0a 6578 7472 6150 6174 6873 203d  .]..extraPaths =
+00000850: 205b 222e 2f73 7263 225d 0d0a 7479 7065   ["./src"]..type
+00000860: 4368 6563 6b69 6e67 4d6f 6465 203d 2022  CheckingMode = "
+00000870: 6261 7369 6322 0d0a 7573 654c 6962 7261  basic"..useLibra
+00000880: 7279 436f 6465 466f 7254 7970 6573 203d  ryCodeForTypes =
+00000890: 2074 7275 650d 0a72 6570 6f72 744d 6973   true..reportMis
+000008a0: 7369 6e67 5061 7261 6d65 7465 7254 7970  singParameterTyp
+000008b0: 6520 3d20 2265 7272 6f72 220d 0a72 6570  e = "error"..rep
+000008c0: 6f72 7455 6e6b 6e6f 776e 5061 7261 6d65  ortUnknownParame
+000008d0: 7465 7254 7970 6520 3d20 2277 6172 6e69  terType = "warni
+000008e0: 6e67 220d 0a72 6570 6f72 7455 6e6b 6e6f  ng"..reportUnkno
+000008f0: 776e 4d65 6d62 6572 5479 7065 203d 2022  wnMemberType = "
+00000900: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000910: 4d69 7373 696e 6754 7970 6541 7267 756d  MissingTypeArgum
+00000920: 656e 7420 3d20 2265 7272 6f72 220d 0a72  ent = "error"..r
+00000930: 6570 6f72 7450 726f 7065 7274 7954 7970  eportPropertyTyp
+00000940: 654d 6973 6d61 7463 6820 3d20 2265 7272  eMismatch = "err
+00000950: 6f72 220d 0a72 6570 6f72 7446 756e 6374  or"..reportFunct
+00000960: 696f 6e4d 656d 6265 7241 6363 6573 7320  ionMemberAccess 
+00000970: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+00000980: 6f72 7450 7269 7661 7465 5573 6167 6520  ortPrivateUsage 
+00000990: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+000009a0: 6f72 7454 7970 6543 6f6d 6d65 6e74 5573  ortTypeCommentUs
+000009b0: 6167 6520 3d20 2277 6172 6e69 6e67 220d  age = "warning".
+000009c0: 0a72 6570 6f72 7449 6e63 6f6d 7061 7469  .reportIncompati
+000009d0: 626c 654d 6574 686f 644f 7665 7272 6964  bleMethodOverrid
+000009e0: 6520 3d20 2277 6172 6e69 6e67 220d 0a72  e = "warning"..r
+000009f0: 6570 6f72 7449 6e63 6f6d 7061 7469 626c  eportIncompatibl
+00000a00: 6556 6172 6961 626c 654f 7665 7272 6964  eVariableOverrid
+00000a10: 6520 3d20 2265 7272 6f72 220d 0a72 6570  e = "error"..rep
+00000a20: 6f72 7449 6e63 6f6e 7369 7374 656e 7443  ortInconsistentC
+00000a30: 6f6e 7374 7275 6374 6f72 203d 2022 6572  onstructor = "er
+00000a40: 726f 7222 0d0a 7265 706f 7274 4f76 6572  ror"..reportOver
+00000a50: 6c61 7070 696e 674f 7665 726c 6f61 6420  lappingOverload 
+00000a60: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+00000a70: 6f72 7455 6e69 6e69 7469 616c 697a 6564  ortUninitialized
+00000a80: 496e 7374 616e 6365 5661 7269 6162 6c65  InstanceVariable
+00000a90: 203d 2022 7761 726e 696e 6722 0d0a 7265   = "warning"..re
+00000aa0: 706f 7274 4361 6c6c 496e 4465 6661 756c  portCallInDefaul
+00000ab0: 7449 6e69 7469 616c 697a 6572 203d 2022  tInitializer = "
+00000ac0: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000ad0: 556e 6e65 6365 7373 6172 7949 7349 6e73  UnnecessaryIsIns
+00000ae0: 7461 6e63 6520 3d20 2269 6e66 6f72 6d61  tance = "informa
+00000af0: 7469 6f6e 220d 0a72 6570 6f72 7455 6e6e  tion"..reportUnn
+00000b00: 6563 6573 7361 7279 4361 7374 203d 2022  ecessaryCast = "
+00000b10: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000b20: 556e 6e65 6365 7373 6172 7943 6f6d 7061  UnnecessaryCompa
+00000b30: 7269 736f 6e20 3d20 2277 6172 6e69 6e67  rison = "warning
+00000b40: 220d 0a72 6570 6f72 7455 6e6e 6563 6573  "..reportUnneces
+00000b50: 7361 7279 436f 6e74 6169 6e73 203d 2022  saryContains = "
+00000b60: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00000b70: 556e 7573 6564 4361 6c6c 5265 7375 6c74  UnusedCallResult
+00000b80: 203d 2022 7761 726e 696e 6722 0d0a 7265   = "warning"..re
+00000b90: 706f 7274 556e 7573 6564 4578 7072 6573  portUnusedExpres
+00000ba0: 7369 6f6e 203d 2022 7761 726e 696e 6722  sion = "warning"
+00000bb0: 0d0a 7265 706f 7274 4d61 7463 684e 6f74  ..reportMatchNot
+00000bc0: 4578 6861 7573 7469 7665 203d 2022 7761  Exhaustive = "wa
+00000bd0: 726e 696e 6722 0d0a 7265 706f 7274 5368  rning"..reportSh
+00000be0: 6164 6f77 6564 496d 706f 7274 7320 3d20  adowedImports = 
+00000bf0: 2277 6172 6e69 6e67 220d 0a72 6570 6f72  "warning"..repor
+00000c00: 7455 6e74 7970 6564 4675 6e63 7469 6f6e  tUntypedFunction
+00000c10: 4465 636f 7261 746f 7220 3d20 2277 6172  Decorator = "war
+00000c20: 6e69 6e67 220d 0a72 6570 6f72 7455 6e74  ning"..reportUnt
+00000c30: 7970 6564 4261 7365 436c 6173 7320 3d20  ypedBaseClass = 
+00000c40: 2265 7272 6f72 220d 0a72 6570 6f72 7455  "error"..reportU
+00000c50: 6e74 7970 6564 4e61 6d65 6454 7570 6c65  ntypedNamedTuple
+00000c60: 203d 2022 7761 726e 696e 6722 0d0a 2320   = "warning"..# 
+00000c70: 4163 7469 7661 7465 2074 6865 2066 6f6c  Activate the fol
+00000c80: 6c6f 7769 6e67 2072 756c 6573 206f 6e6c  lowing rules onl
+00000c90: 7920 6c6f 6361 6c6c 7920 616e 6420 7465  y locally and te
+00000ca0: 6d70 6f72 6172 792c 2069 2e65 2e20 666f  mporary, i.e. fo
+00000cb0: 7220 6120 5141 2073 6573 7369 6f6e 2e0d  r a QA session..
+00000cc0: 0a23 2028 466f 7220 7365 7276 6572 2073  .# (For server s
+00000cd0: 6964 6520 4349 2074 6865 7920 6172 6520  ide CI they are 
+00000ce0: 636f 6e73 6964 6572 6564 2074 6f6f 2073  considered too s
+00000cf0: 7472 6963 742e 290d 0a23 2072 6570 6f72  trict.)..# repor
+00000d00: 7443 6f6e 7374 616e 7452 6564 6566 696e  tConstantRedefin
+00000d10: 6974 696f 6e20 3d20 2277 6172 6e69 6e67  ition = "warning
+00000d20: 220d 0a23 2072 6570 6f72 7455 6e6e 6563  "..# reportUnnec
+00000d30: 6573 7361 7279 5479 7065 4967 6e6f 7265  essaryTypeIgnore
+00000d40: 436f 6d6d 656e 7420 3d20 2269 6e66 6f72  Comment = "infor
+00000d50: 6d61 7469 6f6e 220d 0a23 2072 6570 6f72  mation"..# repor
+00000d60: 7449 6d70 6f72 7443 7963 6c65 7320 3d20  tImportCycles = 
+00000d70: 2277 6172 6e69 6e67 220d 0a23 2072 6570  "warning"..# rep
+00000d80: 6f72 7449 6d70 6c69 6369 7453 7472 696e  ortImplicitStrin
+00000d90: 6743 6f6e 6361 7465 6e61 7469 6f6e 203d  gConcatenation =
+00000da0: 2022 7761 726e 696e 6722 0d0a 0d0a 5b74   "warning"....[t
+00000db0: 6f6f 6c2e 7079 7465 7374 2e69 6e69 5f6f  ool.pytest.ini_o
+00000dc0: 7074 696f 6e73 5d0d 0a74 6573 7470 6174  ptions]..testpat
+00000dd0: 6873 203d 2022 7465 7374 7322 0d0a 6164  hs = "tests"..ad
+00000de0: 646f 7074 7320 3d20 222d 2d73 7472 6963  dopts = "--stric
+00000df0: 742d 6d61 726b 6572 7322 0d0a 7866 6169  t-markers"..xfai
+00000e00: 6c5f 7374 7269 6374 203d 2074 7275 65    l_strict = true
```

### Comparing `ospx-0.2.8/setup.cfg` & `ospx-0.2.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = ospx
-version = 0.2.8
+version = 0.2.9
 summary = Extension package to farn, adding support to build OSP simulation cases using FMUs
 description = Extension package to farn <https://pypi.org/project/farn>, adding support to build OSP <https://open-simulation-platform.github.io> (co-)simulation cases using functional mockup units (FMUs).
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://dnv-opensource.github.io/ospx/README.html
 project_urls = 
 	GitHub = https://github.com/dnv-opensource/ospx
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
@@ -35,18 +36,18 @@
 	=src
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	lxml>=4.9
 	numpy>=1.23
-	pandas>=1.5
-	matplotlib>=3.6
+	pandas>=2.0
+	matplotlib>=3.7
 	graphviz>=0.20
-	dictIO>=0.2.6
+	dictIO>=0.2.7
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [options.entry_points]
@@ -76,15 +77,15 @@
 
 [tox:tox]
 isolated_build = True
 envlist = py{39,310,311}-{linux,macos,windows}
 
 [testenv]
 deps = 
-	pytest>=7.2
+	pytest>=7.3
 	pytest-cov>=4.0
 	pytest-randomly>=3.12
 commands = 
 	pytest --cov --cov-config setup.cfg {posargs}
 
 [egg_info]
 tag_build =
```

### Comparing `ospx-0.2.8/src/ospx/__init__.py` & `ospx-0.2.9/src/ospx/__init__.py`

 * *Files identical despite different names*

### Comparing `ospx-0.2.8/src/ospx/cli/importSystemStructure.py` & `ospx-0.2.9/src/ospx/cli/importSystemStructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from ospx import OspSystemStructureImporter
 from ospx.utils.logging import configure_logging
 
 logger = logging.getLogger(__name__)
 
 
 def _argparser() -> argparse.ArgumentParser:
-
     parser = ArgumentParser(
         prog="importSystemStructure",
         usage="%(prog)s systemStructureFile [options [args]]",
         epilog="_________________importSystemStructure___________________",
         prefix_chars="-",
         add_help=True,
         description=("Imports an existing OspSystemStructure.xml and translates it into a caseDict."),
@@ -106,9 +105,8 @@
     # Invoke API
     OspSystemStructureImporter.import_system_structure(system_structure_file)
 
     return
 
 
 if __name__ == "__main__":
-
     main()
```

### Comparing `ospx-0.2.8/src/ospx/cli/ospCaseBuilder.py` & `ospx-0.2.9/src/ospx/cli/ospCaseBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ospx import OspCaseBuilder
 from ospx.utils.logging import configure_logging
 
 logger = logging.getLogger(__name__)
 
 
 def _argparser() -> argparse.ArgumentParser:
-
     parser = argparse.ArgumentParser(
         prog="ospCaseBuilder",
         usage="%(prog)s caseDict [options [args]]",
         epilog="_________________ospCaseBuilder___________________",
         prefix_chars="-",
         add_help=True,
         description="Builds the OSP-specific configuration files needed to run an OSP (co-)simulation case.",
```

### Comparing `ospx-0.2.8/src/ospx/component.py` & `ospx-0.2.9/src/ospx/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     Equivalent terms to 'component' are: \n
     \t 'Simulator' in OSP. See https://open-simulation-platform.github.io/libcosim/configuration#simulator \n
     \t 'Simulation model' in FMI for co-simulation. See https://github.com/modelica/fmi-standard/releases/download/v2.0.3/FMI-Specification-2.0.3.pdf \n
     \t 'Component' in SSP. See https://ssp-standard.org/publications/SSP10/SystemStructureAndParameterization10.pdf
     """
 
     def __init__(self, name: str, properties: MutableMapping[Any, Any]):
-
         self.name: str = name
         self.generate_proxy = False
         self.fmu: FMU
         self.step_size: Union[float, None] = None
         self._initial_values: dict[str, ScalarVariable] = {}
         self._connectors: dict[str, Connector] = {}
         self.generate_proxy: bool = False
@@ -192,15 +191,15 @@
         -------
         dict[str, Connector]
             dict with all connectors
         """
         return self._connectors
 
     def write_osp_model_description_xml(self):  # sourcery skip: merge-dict-assign
-        """Writes the <component.name>_OspModelDescription.xml file in the current working directory."""
+        """Write the <component.name>_OspModelDescription.xml file in the current working directory."""
         osp_model_description_file = self.fmu.file.parent.absolute() / f"{self.name}_OspModelDescription.xml"
         self._clean(osp_model_description_file)
 
         osp_model_description = {}
 
         # Unit Definitions
         unit_definitions = {}
```

### Comparing `ospx-0.2.8/src/ospx/connection.py` & `ospx-0.2.9/src/ospx/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         Union[Connector, None]
             the connector, if defined. Otherwise None.
         """
         return self._connector
 
     @connector.setter
     def connector(self, connector: Connector):
-        """Sets the connector this endpoint shall refer to.
+        """Set the connector this endpoint shall refer to.
 
         Parameters
         ----------
         connector : Connector
             the connector
         """
         if self._variable:
@@ -71,15 +71,15 @@
         Union[ScalarVariable, None]
             the scalar variable, if defined. Otherwise None.
         """
         return self._variable
 
     @variable.setter
     def variable(self, variable: ScalarVariable):
-        """Sets the scalar variable this endpoint shall refer to.
+        """Set the scalar variable this endpoint shall refer to.
 
         Parameters
         ----------
         variable : ScalarVariable
             the scalar variable
         """
         if self._connector:
```

### Comparing `ospx-0.2.8/src/ospx/connector.py` & `ospx-0.2.9/src/ospx/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         Union[str, None]
             the scalar variable, if connector is a group connector. Otherwise None.
         """
         return self._variable
 
     @variable.setter
     def variable(self, variable: str):
-        """Sets the scalar variable this connector shall be defined for.
+        """Set the scalar variable this connector shall be defined for.
 
         Parameters
         ----------
         variable : str
             the scalar variable
         """
         if self._variable_group:
@@ -71,15 +71,15 @@
         Union[str, None]
             the variable group, if connector is a group connector. Otherwise None.
         """
         return self._variable_group
 
     @variable_group.setter
     def variable_group(self, variable_group: str):
-        """Sets the variable group this connector shall be defined for.
+        """Set the variable group this connector shall be defined for.
 
         Parameters
         ----------
         variable_group : str
             the variable group
         """
         if self._variable:
@@ -95,15 +95,15 @@
     @property
     def type(self) -> Union[str, None]:
         """Returns the type of the connector."""
         return self._type
 
     @type.setter
     def type(self, type: str):
-        """Sets the type of the connector.
+        """Set the type of the connector.
 
         Valid values are:
             "input"
             "output"
         """
         valid_types: list[str] = [
             "input",
```

### Comparing `ospx-0.2.8/src/ospx/fmi/experiment.py` & `ospx-0.2.9/src/ospx/fmi/experiment.py`

 * *Files identical despite different names*

### Comparing `ospx-0.2.8/src/ospx/fmi/fmu.py` & `ospx-0.2.9/src/ospx/fmi/fmu.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             if "tolerance" in default_experiment_attributes:
                 default_experiment.tolerance = default_experiment_attributes["tolerance"]
             if "stepSize" in default_experiment_attributes:
                 default_experiment.step_size = default_experiment_attributes["stepSize"]
         return default_experiment
 
     def copy(self, new_name: str):
-        """Saves a copy of the FMU with a new name.
+        """Save a copy of the FMU with a new name.
 
         Parameters
         ----------
         new_name : str
             Intended name of the copy. The new name must be different from the existing name.
 
         Returns
@@ -268,15 +268,15 @@
         # Write updated modelDescription.xml into new FMU
         new_fmu = FMU(new_file)
         new_fmu._write_model_description(new_model_description)
 
         return new_fmu
 
     def proxify(self, host: str, port: int):
-        """Creates a proxy version of the FMU.
+        """Create a proxy version of the FMU.
 
         For details see https://github.com/NTNU-IHB/FMU-proxy
 
         Parameters
         ----------
         host : str
             Remote host
@@ -298,28 +298,27 @@
         except subprocess.TimeoutExpired:
             logger.exception(f"Timeout occured when calling {command}.")
             return self
         proxy_fmu_file = self.file.parent.absolute() / f"{self.file.stem}-proxy.fmu"
         return FMU(proxy_fmu_file)
 
     def _modify_start_values(self, variables_with_start_values: dict[str, ScalarVariable]):
-        """Modifies the start values of variables inside the FMUs modelDescription.xml."""
+        """Modify the start values of variables inside the FMUs modelDescription.xml."""
 
         logger.info(f"{self.file.name}: update start values of variables in modelDescription.xml")  # 2
 
         model_variables: MutableMapping[Any, Any] = self.model_description[
             find_key(self.model_description, "ModelVariables$")
         ]
 
         names_of_variables_with_start_values: list[str] = [
             variable.name for _, variable in variables_with_start_values.items()
         ]
 
         for model_variable_key, model_variable_properties in model_variables.items():
-
             model_variable_name: str = model_variable_properties["_attributes"]["name"]
 
             if model_variable_name in names_of_variables_with_start_values:
                 variable_with_start_values = variables_with_start_values[model_variable_name]
                 type_identifier = find_type_identifier_in_keys(model_variable_properties)
                 type_key = find_key(model_variable_properties, f"{type_identifier}$")
 
@@ -335,15 +334,14 @@
                 model_variables[model_variable_key]["_attributes"][
                     "variability"
                 ] = variable_with_start_values.variability
 
         self._log_update_in_model_description()
 
     def _log_update_in_model_description(self, model_description: Union[CppDict, None] = None):
-
         model_description = model_description or self.model_description
 
         logger.info(f"{self.file.name}: update <fmiModelDescription description>")  # 2
         # Author
         old_author = model_description["_xmlOpts"]["_rootAttributes"]["author"]
         if platform.system() == "Linux":
             new_author = os.environ["USER"]
```

### Comparing `ospx-0.2.8/src/ospx/fmi/unit.py` & `ospx-0.2.9/src/ospx/fmi/unit.py`

 * *Files identical despite different names*

### Comparing `ospx-0.2.8/src/ospx/fmi/variable.py` & `ospx-0.2.9/src/ospx/fmi/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from collections.abc import Iterable
 from typing import Any, List, Sequence, Union
 
 from dictIO import Formatter, Parser
 
 __ALL__ = ["ScalarVariable", "get_fmi_data_type"]
 
 logger = logging.getLogger(__name__)
@@ -57,15 +58,15 @@
     @property
     def data_type(self) -> Union[str, None]:
         """Returns the FMI data type of the scalar Variable."""
         return self._data_type
 
     @data_type.setter
     def data_type(self, type: str):
-        """Sets the FMI data type of the scalar Variable.
+        """Set the FMI data type of the scalar Variable.
 
         Valid values are:
             "Real"
             "Integer"
             "Boolean"
             "String"
             "Enumeration"
@@ -86,15 +87,15 @@
     @property
     def causality(self) -> str:
         """Returns the causality of the scalar Variable."""
         return self._causality
 
     @causality.setter
     def causality(self, value: str):
-        """Sets the causality of the scalar Variable.
+        """Set the causality of the scalar Variable.
 
         Valid values are:
             "parameter"
             "calculatedParameter"
             "input"
             "output"
             "local"
@@ -119,15 +120,15 @@
     @property
     def variability(self) -> Union[str, None]:
         """Returns the variability of the scalar Variable."""
         return self._variability
 
     @variability.setter
     def variability(self, value: str):
-        """Sets the variability of the scalar Variable.
+        """Set the variability of the scalar Variable.
 
         Valid values are:
             "constant"
             "fixed"
             "tunable"
             "discrete"
             "continuous"
@@ -148,15 +149,15 @@
     @property
     def start(self) -> Union[int, float, bool, str, None]:
         """Returns the start value (initial value) of the scalar Variable."""
         return self._start
 
     @start.setter
     def start(self, value: Union[int, float, bool, str, None]):
-        """Sets the start value (initial value) of the scalar Variable."""
+        """Set the start value (initial value) of the scalar Variable."""
         if value is None:
             logger.error(f"variable {self.name}: start value shall be set to 'None', but 'None' is invalid for start.")
             return
         if self.data_type:
             # make sure the data type of the new value does either match or gets casted to the data_type defined for the variable
             new_value_data_type = get_fmi_data_type(value)
             if new_value_data_type == self.data_type:
@@ -177,15 +178,15 @@
                     return
         else:
             self._start = value
             self.data_type = get_fmi_data_type(self.start)
 
 
 def get_fmi_data_type(arg: Any) -> str:
-    r"""Returns the fmi 2.0 data type corresponding to Python type of the passed in argument.
+    r"""Return the fmi 2.0 data type corresponding to Python type of the passed in argument.
 
     See https://github.com/modelica/fmi-standard/blob/v2.0.x/schema/fmi2Type.xsd
 
     Parameters
     ----------
     arg : Any
         The argument for which the fmi 2.0 data type shall be determined
@@ -246,10 +247,10 @@
         else:
             return bool(parsed_value)
     elif fmi_data_type == "String":
         # format as string
         return Formatter().format_dict(arg) if isinstance(arg, Sequence) else Formatter().format_type(arg)
     elif fmi_data_type == "Enumeration":
         # cast to list
-        return list(arg) if isinstance(arg, Sequence) else [arg]
+        return list(arg) if isinstance(arg, Iterable) else [arg]
     else:
         return None
```

### Comparing `ospx-0.2.8/src/ospx/graph.py` & `ospx-0.2.9/src/ospx/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class Graph:
     """Class providing methods to generate a visual dependency graph
     of a system's components and its connections.
     """
 
     @staticmethod
     def generate_dependency_graph(case: OspSimulationCase):
-        """Generates a dependency graph of the system structure as pdf, for documentation.
+        """Generate a dependency graph of the system structure as pdf, for documentation.
 
         Note: This requires graphviz to be installed on the local machine
         """
         graphiz_not_found_error_mesage: str = (
             "OspSimulationCase.generate_dependency_graph(): failed to run graphviz. \n"
             "To generate the system structure dependency graph, graphviz needs to be installed on the local machine. \n"
             "Kindly check your local installation of graphviz."
@@ -81,15 +81,14 @@
             callgraph = _apply_styles(callgraph, styles)
         except Exception:
             logger.exception(graphiz_not_found_error_mesage)
             return
 
         # Components
         for component in case.system_structure.components.values():
-
             label_key, label = _get_node_label(component)
             # var_keys = find_key(case.models[key]['InitialValues'], 'InitialValue')
             # variables = {}
             label = _create_table(
                 label_key,
                 {
                     "source:": component.fmu.file.name,
@@ -123,15 +122,14 @@
                 style=style,
                 fillcolor=fillcolor,
             )
 
         # Connections
 
         for _, connection in case.system_structure.connections.items():
-
             if not (connection.source_endpoint and connection.target_endpoint):
                 return
             if not (connection.source_endpoint.component and connection.target_endpoint.component):
                 return
             from_key: str = connection.source_endpoint.component.name
             to_key: str = connection.target_endpoint.component.name
 
@@ -142,23 +140,21 @@
                 style = "dashed"
                 color = "#003399"
                 fontcolor = "#003399"
                 penwidth = ("%i" % 1,)
                 weight = "%i" % 1
 
             elif re.search(basic_op_names, from_key, re.I):
-
                 style = "filled"
                 color = "#995566"
                 fontcolor = "#663344"
                 penwidth = ("%i" % 3,)
                 weight = ("%.2f" % 0.66,)
 
             else:
-
                 style = "bold"
                 color = "black"
                 fontcolor = "black"
                 penwidth = ("%i" % int(round((2) ** 1.5, 0)),)
                 weight = ("%i" % int(round((2) ** 1.5, 0)),)
 
             callgraph.edge(
@@ -207,15 +203,14 @@
         f"{connection.source_endpoint.variable_name}-->{connection.target_endpoint.variable_name}"
         if connection.is_valid
         else ""
     )
 
 
 def _create_table(name: str, child: Union[Dict[str, Any], None] = None) -> str:
-
     _child: Dict[str, Any] = child or {" ": " "}
     n_child = len(_child)
     string: str = f'<\n<TABLE BORDER="1" CELLBORDER="1" CELLSPACING="0">\n<TR>\n<TD COLSPAN="{2 * n_child:d}">{name}</TD>\n</TR>\n'
     for key, item in _child.items():
         string += f"<TR><TD>{key}</TD><TD>{item}</TD></TR>\n"
     string += "</TABLE>\n>"
```

### Comparing `ospx-0.2.8/src/ospx/importer.py` & `ospx-0.2.9/src/ospx/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
 
     @staticmethod
     def import_system_structure(
         system_structure_file: Union[str, os.PathLike[str]],
         enter_lib_source_as_relative_path: bool = False,
     ):
-        """Imports an OspSystemStructure.xml file and saves it as an ospx caseDict file.
+        """Import an OspSystemStructure.xml file and save it as an ospx caseDict file.
 
         Parameters
         ----------
         system_structure_file : Union[str, os.PathLike[str]]
             the OspSystemStructure.xml file to be imported
         enter_lib_source_as_relative_path : bool, optional
             whether lib_source shall be entered as relative path in the caseDict, by default False
```

### Comparing `ospx-0.2.8/src/ospx/ospCaseBuilder.py` & `ospx-0.2.9/src/ospx/ospCaseBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @staticmethod
     def build(
         case_dict_file: Union[str, os.PathLike[str]],
         inspect: bool = False,
         graph: bool = False,
         clean: bool = False,
     ):
-        """Builds the OSP-specific configuration files needed to run an OSP (co-)simulation case.
+        """Build the OSP-specific configuration files needed to run an OSP (co-)simulation case.
 
         Builds following files:
             - OspSystemStructure.xml
             - SystemStructure.ssd
             - Plot.json
             - statisticsDict
             - watchDict
@@ -91,15 +91,15 @@
 
         case.write_watch_dict()
 
         return
 
 
 def _clean_case_folder(case_folder: Path):
-    """Cleans up the case folder and deletes any existing ospx files, e.g. modelDescription.xml .fmu .csv etc."""
+    """Clean up the case folder and deletes any existing ospx files, e.g. modelDescription.xml .fmu .csv etc."""
     import re
     from shutil import rmtree
 
     # specify all files to be deleted (or comment-in / comment-out as needed)
     case_builder_result_files = [
         "*.csv",
         "*.out",
```

### Comparing `ospx-0.2.8/src/ospx/ospSimulationCase.py` & `ospx-0.2.9/src/ospx/ospSimulationCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 class OspSimulationCase:
     """OSP Simulation Case."""
 
     def __init__(
         self,
         case_dict: CppDict,
     ):
-
         self.counter = BorgCounter()
         self.case_dict: CppDict = case_dict
         self.case_folder: Path = case_dict.source_file.resolve().parent if case_dict.source_file else Path.cwd()
         self.system_structure: System
 
         # Global settings
         self.simulation: Simulation  # general properties of the simulation case
@@ -37,15 +36,15 @@
             self.name = self.simulation.name
 
         # Library source path
         self.lib_source: Path
         self._resolve_lib_source_folder()
 
     def setup(self):
-        """Sets up the OSP simulation case folder.
+        """Set up the OSP simulation case folder.
 
         Raises
         ------
         ValueError
             If an expected element in caseDict is missing
         FileNotFoundError
             If an FMU file referenced in caseDict does not exist
@@ -68,26 +67,26 @@
             raise ValueError(msg)
         self.system_structure = System(self.case_dict["systemStructure"])
 
         # Make sure all components have a step size defined
         self._check_components_step_size()
 
     def _write_osp_model_description_xmls(self):
-        """Writes the <component.name>_OspModelDescription.xml files for all components defined in the system structure."""
+        """Write the <component.name>_OspModelDescription.xml files for all components defined in the system structure."""
         logger.info(
             f"Write OspModelDescription.xml files for OSP simulation case '{self.name}' in case folder: {self.case_folder}"
         )
         if not self.system_structure or not self.system_structure.components:
             return
         for component in self.system_structure.components.values():
             component.write_osp_model_description_xml()
         return
 
     def write_osp_system_structure_xml(self):
-        """Writes the OspSystemStructure.xml file."""
+        """Write the OspSystemStructure.xml file."""
         # sourcery skip: class-extract-method, merge-dict-assign
 
         osp_system_structure_file = self.case_folder / "OspSystemStructure.xml"
         self._clean(osp_system_structure_file)
 
         logger.info(
             f"Write OspSystemStructure.xml file for OSP simulation case '{self.name}' in case folder: {self.case_folder}"
@@ -200,15 +199,15 @@
             "<OspSystemStructure.*>?",
             """<OspSystemStructure xmlns="http://opensimulationplatform.com/MSMI/OSPSystemStructure" version="0.1">""",
         )
 
         return
 
     def write_system_structure_ssd(self):
-        """Writes the SystemStructure.ssd file."""
+        """Write the SystemStructure.ssd file."""
 
         system_structure_ssd_file = self.case_folder / "SystemStructure.ssd"
         self._clean(system_structure_ssd_file)
 
         # sourcery skip: merge-dict-assign
         logger.info(
             f"Write SystemStructure.ssd file for OSP simulation case '{self.name}' in case folder: {self.case_folder}"
@@ -292,15 +291,15 @@
         # Write SystemStructure.ssd
         formatter = XmlFormatter(omit_prefix=False)
         DictWriter.write(system_structure_ssd, system_structure_ssd_file, formatter=formatter)
 
         return
 
     def write_statistics_dict(self):
-        """Writes selected properties of the system structure into a statistics dict.
+        """Write selected properties of the system structure into a statistics dict.
 
         I.e. for documentation or further statistical analysis.
         """
         statistics_dict_file = self.case_folder / "statisticsDict"
         # self._clean(statistics_dict_file)
 
         # sourcery skip: merge-dict-assign, simplify-dictionary-update
@@ -347,15 +346,15 @@
             "count": len(self.system_structure.variables.keys()),
             "names": list(self.system_structure.variables.keys()),
         }
 
         DictWriter.write(statistics_dict, statistics_dict_file, mode="w")
 
     def write_watch_dict(self):
-        """Writes a case-specific watch dict file.
+        """Write a case-specific watch dict file.
 
         The watch dict file can be used with watchCosim for
             - convergence control
             - convergence plotting
             - extracting the results
         """
         watch_dict_file = self.case_folder / "watchDict"
@@ -381,15 +380,15 @@
             watch_dict["datasources"].update({component_name: {"columns": columns}})
 
         DictWriter.write(watch_dict, watch_dict_file, mode="w")
 
         return
 
     def _read_simulation(self):
-        """Reads general simulation properties from case dict."""
+        """Read general simulation properties from case dict."""
         logger.info("reading simulation properties")  # 0
 
         if "run" not in self.case_dict:
             return
         if "simulation" not in self.case_dict["run"]:
             return
         simulation = Simulation()
@@ -403,15 +402,15 @@
         if "baseStepSize" in simulation_properties:
             simulation.base_step_size = simulation_properties["baseStepSize"]
         if "algorithm" in simulation_properties:
             simulation.algorithm = simulation_properties["algorithm"]
         self.simulation = simulation
 
     def _resolve_lib_source_folder(self):
-        """Resolves the library source folder."""
+        """Resolve the library source folder."""
         self.lib_source = Path.cwd()  # initialize conservatively (with fallback path)
         if "_environment" in self.case_dict:
             if "libSource" in self.case_dict["_environment"]:
                 self.lib_source = Path(self.case_dict["_environment"]["libSource"])
             else:
                 logger.warning(
                     f"no 'libSource' element found in {self.case_dict.name}['_environment']. Path to libSource will be set to current working directory."
@@ -427,15 +426,15 @@
         if fmu_file.is_absolute():
             fmu_file = fmu_file.resolve()
         else:
             fmu_file = (self.lib_source / fmu_file).resolve()
         return fmu_file
 
     def _check_all_fmus_exist(self):
-        """Checks whether all referenced FMUs actually exist."""
+        """Check whether all referenced FMUs actually exist."""
         logger.debug("Check whether all referenced FMUs exist.")
         components = self.case_dict["systemStructure"]["components"]
 
         for component_name, component_properties in components.items():
             if "fmu" not in component_properties:
                 msg = f"component {component_name}: 'fmu' element missing in case dict."
                 logger.exception(msg)
@@ -443,15 +442,15 @@
             fmu_file = self._resolve_fmu_file(component_properties["fmu"])
             if not fmu_file.exists():
                 msg = f"component {component_name}: referenced FMU file {fmu_file} not found."
                 logger.exception(msg)
                 raise FileNotFoundError(fmu_file)
 
     def _resolve_all_fmus(self):
-        """Resolves all referenced FMUs and ensures they are accessible from the case folder via a relative path.
+        """Resolve all referenced FMUs and ensures they are accessible from the case folder via a relative path.
 
         This is necessary because OspSystemStructure.xml allows only relative paths
         as 'source' attribute in a <Simulator> element.
         If an FMU is not accessible via a relative path, the FMU will be copied into the case folder.
         Note: If multiple components reference the same FMU, these get copied only once.
         """
 
@@ -462,15 +461,15 @@
             try:
                 _ = relative_path(self.case_folder, fmu_file)
             except ValueError:
                 fmu_file = self._copy_fmu_to_case_folder(fmu_file)
             component_properties["fmu"] = fmu_file
 
     def _copy_fmu_to_case_folder(self, fmu_file: Path) -> Path:
-        """Copies the passed in FMU file into the case folder.
+        """Copy the passed in FMU file into the case folder.
 
         If also an accompanying <fmu_name>_OspModelDescription.xml file exists in the same folder as the FMU file,
         then also that OspModelDescription.xml file will be copied into the case folder.
 
         Parameters
         ----------
         fmu_file : Path
@@ -504,15 +503,15 @@
             return
         for component in self.system_structure.components.values():
             if not component.step_size:
                 component.step_size = self.simulation.base_step_size
         return
 
     def _set_components_step_size(self, step_size: float):
-        """Overwrites the step size of all components with the passed in value."""
+        """Overwrite the step size of all components with the passed in value."""
         if not self.system_structure or not self.system_structure.components:
             return
         for component in self.system_structure.components.values():
             component.step_size = step_size
         return
 
     def _inspect(self):
@@ -586,15 +585,15 @@
                 )
                 log_string += connector_definitions
         logger.info(log_string + "\n")
 
         logger.info("Inspect mode: Finished.")
 
     def _write_plot_config_json(self):
-        """Writes the PlotConfig.json file, containing postprocessing information."""
+        """Write the PlotConfig.json file, containing postprocessing information."""
 
         plot_config_file = self.case_folder / "PlotConfig.json"
         self._clean(plot_config_file)
 
         if "plots" in self.case_dict["postProcessing"].keys():
             temp_dict: Dict[str, List[Dict[str, Any]]] = {"plots": []}
             for plot in self.case_dict["postproc"]["plots"].values():
```

### Comparing `ospx-0.2.8/src/ospx/simulation.py` & `ospx-0.2.9/src/ospx/simulation.py`

 * *Files identical despite different names*

### Comparing `ospx-0.2.8/src/ospx/system.py` & `ospx-0.2.9/src/ospx/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,25 +102,25 @@
         variables: dict[str, ScalarVariable] = {}
         for component in self.components.values():
             if component.variables:
                 variables |= component.variables
         return variables
 
     def _read_components(self, properties: MutableMapping[Any, Any]):
-        """Reads components from (case dict) properties."""
+        """Read components from (case dict) properties."""
         logger.info("read components from case dict")
         self._components.clear()
         if "components" not in properties:
             return
         for component_name, component_properties in properties["components"].items():
             component = Component(component_name, component_properties)
             self._components[component.name] = component
 
     def _read_connections(self, properties: MutableMapping[Any, Any]):
-        """Reads connections from (case dict) properties."""
+        """Read connections from (case dict) properties."""
         logger.info("read connections from case dict")
         self._connections.clear()
         if "connections" not in properties:
             return
         for connection_name, connection_properties in properties["connections"].items():
             source_endpoint: Union[Endpoint, None] = None
             target_endpoint: Union[Endpoint, None] = None
```

### Comparing `ospx-0.2.8/src/ospx/utils/dateTime.py` & `ospx-0.2.9/src/ospx/utils/dateTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime as datetime
 from typing import Tuple
 
 __all__ = ["calc_time"]
 
 
 def calc_time(time0: datetime, time1: datetime) -> Tuple[int, int, int, int, int]:
-    """Calculates the time delta between time0 and time1.
+    """Calculate the time delta between time0 and time1.
 
     Calculates the time delta between time0 and time1 and
     returns the result as a tuple of integers representing the number of
     months, days, hours, minutes and seconds
     the time delta constitutes.
 
     Parameters
```

### Comparing `ospx-0.2.8/src/ospx/utils/dict.py` & `ospx-0.2.9/src/ospx/utils/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import re
 from collections import OrderedDict
 from typing import Any, List, MutableMapping, Set, Union
 
 
 def find_key(dict: MutableMapping[Any, Any], pattern: str) -> Union[str, None]:
-    """Finds the first key in dict that matches the given pattern."""
+    """Find the first key in dict that matches the given pattern."""
     try:
         return [k for k in dict.keys() if re.search(pattern, k)][0]
     except Exception:
         return None
 
 
 def find_keys(dict: MutableMapping[Any, Any], pattern: str) -> Union[List[str], None]:
-    """Finds all keys in dict that match the given pattern."""
+    """Find all keys in dict that match the given pattern."""
     try:
         return [k for k in dict.keys() if re.search(pattern, k)]
     except Exception:
         return None
 
 
 def find_type_identifier_in_keys(dict: MutableMapping[Any, Any]) -> Union[str, None]:
-    """Finds the first key name in dict that contains one of the following type identifier strings:
+    """Find the first key name in dict that contains one of the following type identifier strings:
     [Integer|Real|Boolean|Enumeration|String|Unknown].
     """
     key_list: List[str] = ["Integer", "Real", "Boolean", "Enumeration", "String", "Unkown"]
     type_identifier: List[str] = []
     for key in dict:
         key_without_index = re.sub(r"^\d{6}_", "", key)
 
         if key_without_index in key_list:
             type_identifier.append(key_without_index)
 
     return type_identifier[0] if type_identifier else None
 
 
 def shrink_dict(dict: MutableMapping[Any, Any], unique_key: Union[List[str], None] = None) -> MutableMapping[Any, Any]:
-    """Identifies doubled entries in the passed in dict and returns a new dict with doubled entries removed."""
+    """Identify doubled entries in the passed in dict and return a new dict with doubled entries removed."""
     _unique_key: List[str] = unique_key or []
     unique_keys_string: str = "['" + "']['".join(_unique_key) + "']"
     # sort an ordered dict for attribute (child) where the dict is to make unique for
     eval_string: str = f"sorted(dict.items(), key=lambda x: str(x[1]{unique_keys_string}))"
 
     # Identify doublettes and collect them for subsequent removal
     seen: Set[Any] = set([])
```

### Comparing `ospx-0.2.8/src/ospx/utils/logging.py` & `ospx-0.2.9/src/ospx/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ospx-0.2.8/src/ospx/utils/plotting.py` & `ospx-0.2.9/src/ospx/utils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 
 logger = logging.getLogger(__name__)
 
 
 def create_meta_dict(title: str) -> Dict[str, str]:
-    """Creates a default of meta dict which can be passed to save_figure().
+    """Create a default of meta dict which can be passed to save_figure().
 
     Parameters
     ----------
     title : str
         the title of the figure
 
     Returns
```

### Comparing `ospx-0.2.8/src/ospx/utils/zip.py` & `ospx-0.2.9/src/ospx/utils/zip.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
     file_handle, temp_name = mkstemp(dir=zip_file.parent)
     updated_zip_file = None
     try:
         with ZipFile(zip_file, "r") as zip_read:
             with ZipFile(temp_name, "w") as zip_write:
                 zip_write.comment = zip_read.comment  # preserve the comment
                 for item in zip_read.infolist():
-
                     if not re.search(file_name_pattern, item.filename):
                         zip_write.writestr(item, zip_read.read(item.filename))
                     else:
                         temp = zip_read.read(item.filename)
                         source = (re.findall(subst[0], str(temp)))[0]
                         if not str(source):
                             logger.warning(f'substitution source is empty:\'{" ".join(source)}\'')
```

### Comparing `ospx-0.2.8/src/ospx/watch/cli/watchCosim.py` & `ospx-0.2.9/src/ospx/watch/cli/watchCosim.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from ospx.utils.logging import configure_logging
 from ospx.watch.watchCosim import CosimWatcher
 
 logger = logging.getLogger(__name__)
 
 
 def _argparser() -> argparse.ArgumentParser:
-
     parser = ArgumentParser(
         prog="watchCosim",
         usage="%(prog)s watchDict [options [args]]",
         epilog="_________________watchCosim___________________",
         prefix_chars="-",
         add_help=True,
         description="Continuously watches the progress of cosim, and finally saves results as a pandas dataframe.",
```

### Comparing `ospx-0.2.8/src/ospx/watch/watchCosim.py` & `ospx-0.2.9/src/ospx/watch/watchCosim.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,17 @@
         self.scale_factor: float = scale_factor
         self.figure: Figure
         self.terminate: bool = False
         self.max_row: int = 0
         return
 
     def read_watch_dict(self, watch_dict_file: Union[str, os.PathLike[str]]):
-        """Reads watchDict file. The watchDict file contains the parameters to be plotted.
+        """Read watchDict file.
+
+        The watchDict file contains the parameters to be plotted.
 
         Parameters
         ----------
         watch_dict_file : Union[str, os.PathLike[str]]
             watchDict file. Contains the parameters to be plotted.
 
         Raises
@@ -89,15 +91,15 @@
         if "simulation" in self.watch_dict:
             self.title = f"{self.watch_dict_file.name}-{self.watch_dict['simulation']['name']}"
 
         self._define_data_source_properties_for_plotting()
         return
 
     def plot(self, converge: bool = False):
-        """Plotting.
+        """Plot trends.
 
         Plotting + convergence checker (future task)
 
         Parameters
         ----------
         converge : bool, optional
             if True, convergence is checked, by default False
@@ -111,15 +113,14 @@
         else:
             terminate_loops = 10
             max_no_change_loops = 0
 
         df_row_size = 0
 
         while True:  # do as long as not interrupted
-
             df = self._read_csv_files_into_dataframe()
 
             # cumulate counter for termination if no changes
             if df_row_size == len(df):
                 terminate_loops += 1
             else:
                 terminate_loops = 0
@@ -127,15 +128,14 @@
             df_col_size = len(list(df)) - 1  # reduced by one because 1st col is to remove from list
 
             # axs = [None for x in range(df_col_size)]
             axs: MutableSequence[Axes] = []
             plot: Axes
             # for index in range(self.nSubplots):
             for index in range(df_col_size):
-
                 current_key = list(df)[index + 1]  # 0 is Time, StepCount was removed for simplification
 
                 plot = self.figure.add_subplot(self.max_row, self.number_of_columns, index + 1)
 
                 try:
                     _ = plot.plot(
                         "Time",
@@ -145,17 +145,17 @@
                         data=df[["Time", current_key]],
                     )
                 except (TypeError, ValueError):
                     pass
                 except Exception as e:
                     logger.exception(e)
                 # subplot.set_title(currentKey,  fontsize=10)
-                plot.grid(color="#66aa88", linestyle="--")
-                plot.xaxis.set_tick_params(labelsize=8)
-                plot.yaxis.set_tick_params(labelsize=8)
+                _ = plot.grid(color="#66aa88", linestyle="--")
+                _ = plot.xaxis.set_tick_params(labelsize=8)
+                _ = plot.yaxis.set_tick_params(labelsize=8)
                 _ = plot.legend(fontsize=8)
                 axs.append(plot)
                 # if isinstance(plot, Axes):
                 #     axs.append(plot)
                 # else:
                 #     raise TypeError(
                 #         f"CosimWatcher.plot(): plot is of type {type(plot)}. Expected type was matplotlib.axes.Axes ."
@@ -287,15 +287,15 @@
                     data_source_properties.update({"displayColNames": _display_column_names})
 
                     data_source_properties.update({"xColumn": columns[0]})
                     data_source_properties.update({"yColumns": columns[1:]})
         return
 
     def _initialize_plot(self):
-        """Initializes the plot.
+        """Initialize the plot.
 
         Collects data and sets plot header line
         """
         self.figure = plt.figure(figsize=(16 * self.scale_factor, 9 * self.scale_factor), dpi=150)
         # self.fig.tight_layout()  # constraint_layout()
         _ = self.figure.subplots_adjust(
             left=0.1,
@@ -311,15 +311,15 @@
 
         self.number_of_subplots = len(list(df)) - 1  # one of the columns is the abscissa
         self.number_of_columns = int(sqrt(self.number_of_subplots - 1)) + 1
         self.max_row = int(self.number_of_subplots / self.number_of_columns - 0.1) + 1
         return
 
     def _read_csv_files_into_dataframe(self) -> DataFrame:
-        """Reads all csv files into one joint Pandas dataframe.
+        """Read all csv files into one joint Pandas dataframe.
 
         Read all csv files (=all data sources, one csv file per data source) into one joint Pandas dataframe.
         The returned dataframe hence contains the data of all datas ources.
         This dataframe can then be used for plotting and to dump a pickle.
 
         Returns
         -------
@@ -401,14 +401,14 @@
             start = 0
 
         # if skip latest n steps is to be implemented, no changes to start, but an additional command option is required
         length: int = df_all_data_sources.shape[0]
         return df_all_data_sources.iloc[start:length, :]
 
     def _determine_optimum_screen_size(self):
-        """Determines the optimum screen size."""
+        """Determine the optimum screen size."""
         # Opening and closing of window may be deprecated when a better solution is found
         mgr = plt.get_current_fig_manager()
         mgr.full_screen_toggle()
         self.screenSize = (mgr.canvas.width(), mgr.canvas.height())  # type: ignore
         mgr.window.close()  # type: ignore
         return
```

### Comparing `ospx-0.2.8/src/ospx.egg-info/PKG-INFO` & `ospx-0.2.9/src/ospx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ospx
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension package to farn, adding support to build OSP simulation cases using FMUs
 Home-page: https://dnv-opensource.github.io/ospx/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
 Project-URL: GitHub, https://github.com/dnv-opensource/ospx
 Platform: Python3.x
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -106,15 +107,15 @@
     ~~~sh
     $ pip install -r requirements.txt
     ~~~
 
 
 ## Meta
 
-Copyright (c) 2022 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2023 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
```

### Comparing `ospx-0.2.8/src/ospx.egg-info/SOURCES.txt` & `ospx-0.2.9/src/ospx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,11 @@
 src/ospx/utils/dict.py
 src/ospx/utils/logging.py
 src/ospx/utils/plotting.py
 src/ospx/utils/zip.py
 src/ospx/watch/__init__.py
 src/ospx/watch/watchCosim.py
 src/ospx/watch/cli/__init__.py
-src/ospx/watch/cli/watchCosim.py
+src/ospx/watch/cli/watchCosim.py
+tests/test_fmu.py
+tests/test_ospCaseBuilder.py
+tests/test_watchCosim.py
```

