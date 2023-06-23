# Comparing `tmp/ensemble_core-0.1.0.tar.gz` & `tmp/ensemble_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble_core-0.1.0.tar", last modified: Fri Jun 23 02:40:13 2023, max compression
+gzip compressed data, was "ensemble_core-0.1.2.tar", last modified: Fri Jun 23 02:46:29 2023, max compression
```

## Comparing `ensemble_core-0.1.0.tar` & `ensemble_core-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:40:13.859804 ensemble_core-0.1.0/
--rw-r--r--   0 chenweixu   (501) staff       (20)      221 2023-06-23 02:40:13.859684 ensemble_core-0.1.0/PKG-INFO
-drwxr-xr-x   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:40:13.858903 ensemble_core-0.1.0/ensemble_core/
--rw-r--r--   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:32:56.000000 ensemble_core-0.1.0/ensemble_core/__init__.py
--rw-r--r--   0 chenweixu   (501) staff       (20)     4797 2023-06-21 17:48:46.000000 ensemble_core-0.1.0/ensemble_core/login.py
-drwxr-xr-x   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:40:13.859503 ensemble_core-0.1.0/ensemble_core.egg-info/
--rw-r--r--   0 chenweixu   (501) staff       (20)      221 2023-06-23 02:40:13.000000 ensemble_core-0.1.0/ensemble_core.egg-info/PKG-INFO
--rw-r--r--   0 chenweixu   (501) staff       (20)      241 2023-06-23 02:40:13.000000 ensemble_core-0.1.0/ensemble_core.egg-info/SOURCES.txt
--rw-r--r--   0 chenweixu   (501) staff       (20)        1 2023-06-23 02:40:13.000000 ensemble_core-0.1.0/ensemble_core.egg-info/dependency_links.txt
--rw-r--r--   0 chenweixu   (501) staff       (20)       26 2023-06-23 02:40:13.000000 ensemble_core-0.1.0/ensemble_core.egg-info/requires.txt
--rw-r--r--   0 chenweixu   (501) staff       (20)       14 2023-06-23 02:40:13.000000 ensemble_core-0.1.0/ensemble_core.egg-info/top_level.txt
--rw-r--r--   0 chenweixu   (501) staff       (20)       38 2023-06-23 02:40:13.859847 ensemble_core-0.1.0/setup.cfg
--rw-r--r--   0 chenweixu   (501) staff       (20)      493 2023-06-23 02:40:11.000000 ensemble_core-0.1.0/setup.py
+drwxr-xr-x   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:46:29.507486 ensemble_core-0.1.2/
+-rw-r--r--   0 chenweixu   (501) staff       (20)      221 2023-06-23 02:46:29.507384 ensemble_core-0.1.2/PKG-INFO
+drwxr-xr-x   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:46:29.506676 ensemble_core-0.1.2/ensemble_core/
+-rw-r--r--   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:32:56.000000 ensemble_core-0.1.2/ensemble_core/__init__.py
+-rw-r--r--   0 chenweixu   (501) staff       (20)     4797 2023-06-21 17:48:46.000000 ensemble_core-0.1.2/ensemble_core/login.py
+drwxr-xr-x   0 chenweixu   (501) staff       (20)        0 2023-06-23 02:46:29.507237 ensemble_core-0.1.2/ensemble_core.egg-info/
+-rw-r--r--   0 chenweixu   (501) staff       (20)      221 2023-06-23 02:46:29.000000 ensemble_core-0.1.2/ensemble_core.egg-info/PKG-INFO
+-rw-r--r--   0 chenweixu   (501) staff       (20)      241 2023-06-23 02:46:29.000000 ensemble_core-0.1.2/ensemble_core.egg-info/SOURCES.txt
+-rw-r--r--   0 chenweixu   (501) staff       (20)        1 2023-06-23 02:46:29.000000 ensemble_core-0.1.2/ensemble_core.egg-info/dependency_links.txt
+-rw-r--r--   0 chenweixu   (501) staff       (20)       21 2023-06-23 02:46:29.000000 ensemble_core-0.1.2/ensemble_core.egg-info/requires.txt
+-rw-r--r--   0 chenweixu   (501) staff       (20)       14 2023-06-23 02:46:29.000000 ensemble_core-0.1.2/ensemble_core.egg-info/top_level.txt
+-rw-r--r--   0 chenweixu   (501) staff       (20)       38 2023-06-23 02:46:29.507525 ensemble_core-0.1.2/setup.cfg
+-rw-r--r--   0 chenweixu   (501) staff       (20)      491 2023-06-23 02:46:13.000000 ensemble_core-0.1.2/setup.py
```

### Comparing `ensemble_core-0.1.0/ensemble_core/login.py` & `ensemble_core-0.1.2/ensemble_core/login.py`

 * *Files identical despite different names*

