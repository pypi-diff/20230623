# Comparing `tmp/atlaspy-0.0.2.tar.gz` & `tmp/atlaspy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlaspy-0.0.2.tar", last modified: Thu Jun 22 23:44:21 2023, max compression
+gzip compressed data, was "atlaspy-0.0.3.tar", last modified: Thu Jun 22 23:51:49 2023, max compression
```

## Comparing `atlaspy-0.0.2.tar` & `atlaspy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:44:21.409287 atlaspy-0.0.2/
--rw-r--r--   0 allucas    (501) staff       (20)       40 2023-06-22 23:38:45.000000 atlaspy-0.0.2/MANIFEST.in
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:44:21.409164 atlaspy-0.0.2/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.2/README.md
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:44:21.408419 atlaspy-0.0.2/atlaspy/
--rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.2/atlaspy/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)    10553 2023-06-22 23:26:17.000000 atlaspy-0.0.2/atlaspy/core.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:44:21.409011 atlaspy-0.0.2/atlaspy.egg-info/
--rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      220 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/SOURCES.txt
--rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/dependency_links.txt
--rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/requires.txt
--rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-22 23:44:21.000000 atlaspy-0.0.2/atlaspy.egg-info/top_level.txt
--rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-22 23:44:21.409327 atlaspy-0.0.2/setup.cfg
--rw-r--r--   0 allucas    (501) staff       (20)      537 2023-06-22 23:43:11.000000 atlaspy-0.0.2/setup.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:51:49.916887 atlaspy-0.0.3/
+-rw-r--r--   0 allucas    (501) staff       (20)       40 2023-06-22 23:38:45.000000 atlaspy-0.0.3/MANIFEST.in
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:51:49.916764 atlaspy-0.0.3/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      112 2023-06-22 23:24:24.000000 atlaspy-0.0.3/README.md
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:51:49.916010 atlaspy-0.0.3/atlaspy/
+-rw-r--r--   0 allucas    (501) staff       (20)        0 2023-06-22 23:18:46.000000 atlaspy-0.0.3/atlaspy/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)    10553 2023-06-22 23:26:17.000000 atlaspy-0.0.3/atlaspy/core.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-06-22 23:51:49.916600 atlaspy-0.0.3/atlaspy.egg-info/
+-rw-r--r--   0 allucas    (501) staff       (20)      308 2023-06-22 23:51:49.000000 atlaspy-0.0.3/atlaspy.egg-info/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      220 2023-06-22 23:51:49.000000 atlaspy-0.0.3/atlaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        1 2023-06-22 23:51:49.000000 atlaspy-0.0.3/atlaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       42 2023-06-22 23:51:49.000000 atlaspy-0.0.3/atlaspy.egg-info/requires.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        8 2023-06-22 23:51:49.000000 atlaspy-0.0.3/atlaspy.egg-info/top_level.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       38 2023-06-22 23:51:49.916929 atlaspy-0.0.3/setup.cfg
+-rw-r--r--   0 allucas    (501) staff       (20)      555 2023-06-22 23:51:45.000000 atlaspy-0.0.3/setup.py
```

### Comparing `atlaspy-0.0.2/atlaspy/core.py` & `atlaspy-0.0.3/atlaspy/core.py`

 * *Files identical despite different names*

