# Comparing `tmp/atlaspy-0.0.1.tar.gz` & `tmp/atlaspy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlaspy-0.0.1.tar", last modified: Thu Jun 22 23:26:56 2023, max compression
+gzip compressed data, was "atlaspy-0.0.2.tar", last modified: Thu Jun 22 23:44:21 2023, max compression
```

## Comparing `atlaspy-0.0.1.tar` & `atlaspy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:26:56.810364 atlaspy-0.0.1/
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:26:56.810239 atlaspy-0.0.1/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.1/README.md
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:26:56.809429 atlaspy-0.0.1/atlaspy/
--rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.1/atlaspy/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)    10553 2023-06-22 23:26:17.000000 atlaspy-0.0.1/atlaspy/core.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:26:56.810054 atlaspy-0.0.1/atlaspy.egg-info/
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:26:56.000000 atlaspy-0.0.1/atlaspy.egg-info/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      208 2023-06-22 23:26:56.000000 atlaspy-0.0.1/atlaspy.egg-info/SOURCES.txt
--rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-22 23:26:56.000000 atlaspy-0.0.1/atlaspy.egg-info/dependency_links.txt
--rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-22 23:26:56.000000 atlaspy-0.0.1/atlaspy.egg-info/requires.txt
--rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-22 23:26:56.000000 atlaspy-0.0.1/atlaspy.egg-info/top_level.txt
--rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-22 23:26:56.810408 atlaspy-0.0.1/setup.cfg
--rw-r--r--   0 allucas    (501) staff       (20)      635 2023-06-22 23:24:26.000000 atlaspy-0.0.1/setup.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:44:21.409287 atlaspy-0.0.2/
+-rw-r--r--   0 allucas    (501) staff       (20)       40 2023-06-22 23:38:45.000000 atlaspy-0.0.2/MANIFEST.in
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:44:21.409164 atlaspy-0.0.2/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.2/README.md
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:44:21.408419 atlaspy-0.0.2/atlaspy/
+-rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.2/atlaspy/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)    10553 2023-06-22 23:26:17.000000 atlaspy-0.0.2/atlaspy/core.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:44:21.409011 atlaspy-0.0.2/atlaspy.egg-info/
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      220 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/requires.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/top_level.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-22 23:44:21.409327 atlaspy-0.0.2/setup.cfg
+-rw-r--r--   0 allucas    (501) staff       (20)      537 2023-06-22 23:43:11.000000 atlaspy-0.0.2/setup.py
```

### Comparing `atlaspy-0.0.1/atlaspy/core.py` & `atlaspy-0.0.2/atlaspy/core.py`

 * *Files identical despite different names*

