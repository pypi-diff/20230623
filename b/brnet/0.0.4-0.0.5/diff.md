# Comparing `tmp/brnet-0.0.4.tar.gz` & `tmp/brnet-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brnet-0.0.4.tar", last modified: Wed Jun 21 22:46:05 2023, max compression
+gzip compressed data, was "brnet-0.0.5.tar", last modified: Thu Jun 22 23:46:29 2023, max compression
```

## Comparing `brnet-0.0.4.tar` & `brnet-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 22:45:51.000000 brnet-0.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 22:45:51.000000 brnet-0.0.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-21 22:45:51.000000 brnet-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 22:45:51.000000 brnet-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 22:45:51.000000 brnet-0.0.4/01-phys-to-bridge
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 22:45:51.000000 brnet-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 22:45:51.000000 brnet-0.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 22:46:05.930070 brnet-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-21 22:45:51.000000 brnet-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-21 22:45:51.000000 brnet-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:46:05.930070 brnet-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/sh/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/brnet
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/pidp11.sh.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/wait_for_if
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.926070 brnet-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/src/brnet/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/bridger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/external.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/src/brnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:45:51.000000 brnet-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 22:45:51.000000 brnet-0.0.4/tests/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 22:45:51.000000 brnet-0.0.4/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-21 22:45:51.000000 brnet-0.0.4/wrapper.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.163032 brnet-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-22 23:46:14.000000 brnet-0.0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-22 23:46:14.000000 brnet-0.0.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-22 23:46:14.000000 brnet-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-22 23:46:14.000000 brnet-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 23:46:14.000000 brnet-0.0.5/01-phys-to-bridge
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-22 23:46:14.000000 brnet-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-22 23:46:14.000000 brnet-0.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-22 23:46:29.163032 brnet-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-22 23:46:14.000000 brnet-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-22 23:46:14.000000 brnet-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:46:29.163032 brnet-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/sh/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/brnet
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/pidp11.sh.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/wait_for_if
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/src/brnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 23:46:14.000000 brnet-0.0.5/src/brnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-22 23:46:14.000000 brnet-0.0.5/src/brnet/brnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/src/brnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/object_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.163032 brnet-0.0.5/tests/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/support/ip
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/support/start_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/support/stop_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-22 23:46:14.000000 brnet-0.0.5/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 23:46:14.000000 brnet-0.0.5/wrapper.sh
```

### Comparing `brnet-0.0.4/.github/workflows/ci.yaml` & `brnet-0.0.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/.gitignore` & `brnet-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/LICENSE` & `brnet-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/Makefile` & `brnet-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/PKG-INFO` & `brnet-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.4/README.md` & `brnet-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/pyproject.toml` & `brnet-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]
 requires-python = ">=3.9"
 # Use requirements/main.in for runtime dependencies instead.
 dependencies = []
 dynamic = ["version"]
 
 [project.scripts]
-brnet = "brnet.cli:main"
+brnet = "brnet.brnet:main"
 
 [project.urls]
 Source = "https://github.com/athornton/brnet"
 
 [build-system]
 requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
```

### Comparing `brnet-0.0.4/requirements/dev.txt` & `brnet-0.0.5/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/sh/README.md` & `brnet-0.0.5/sh/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/sh/brnet` & `brnet-0.0.5/sh/brnet`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/src/brnet.egg-info/PKG-INFO` & `brnet-0.0.5/src/brnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.4/tox.ini` & `brnet-0.0.5/tox.ini`

 * *Files identical despite different names*

### Comparing `brnet-0.0.4/wrapper.sh` & `brnet-0.0.5/wrapper.sh`

 * *Files identical despite different names*

