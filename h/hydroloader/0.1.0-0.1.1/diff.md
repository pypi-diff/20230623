# Comparing `tmp/hydroloader-0.1.0.tar.gz` & `tmp/hydroloader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroloader-0.1.0.tar", last modified: Thu Apr 13 20:33:18 2023, max compression
+gzip compressed data, was "hydroloader-0.1.1.tar", last modified: Fri Jun 23 01:34:46 2023, max compression
```

## Comparing `hydroloader-0.1.0.tar` & `hydroloader-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-04-13 20:33:18.491246 hydroloader-0.1.0/
--rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-04-11 23:07:08.000000 hydroloader-0.1.0/LICENSE.txt
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-04-13 20:33:18.491289 hydroloader-0.1.0/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)        0 2023-04-11 23:06:14.000000 hydroloader-0.1.0/README.md
--rw-r--r--   0 klippold   (501) staff       (20)       80 2023-04-11 23:06:41.000000 hydroloader-0.1.0/pyproject.toml
--rw-r--r--   0 klippold   (501) staff       (20)      338 2023-04-13 20:33:18.491523 hydroloader-0.1.0/setup.cfg
--rw-r--r--   0 klippold   (501) staff       (20)       93 2023-04-11 23:05:02.000000 hydroloader-0.1.0/setup.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-04-13 20:33:18.489382 hydroloader-0.1.0/src/
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-04-13 20:33:18.490434 hydroloader-0.1.0/src/hydroloader/
--rw-r--r--   0 klippold   (501) staff       (20)      397 2023-04-13 19:58:23.000000 hydroloader-0.1.0/src/hydroloader/__init__.py
--rw-r--r--   0 klippold   (501) staff       (20)     1451 2023-04-13 19:06:22.000000 hydroloader-0.1.0/src/hydroloader/main.py
--rw-r--r--   0 klippold   (501) staff       (20)     1043 2023-04-13 19:06:10.000000 hydroloader-0.1.0/src/hydroloader/models.py
--rw-r--r--   0 klippold   (501) staff       (20)     1965 2023-04-13 19:05:40.000000 hydroloader-0.1.0/src/hydroloader/utils.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-04-13 20:33:18.491142 hydroloader-0.1.0/src/hydroloader.egg-info/
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-04-13 20:33:18.000000 hydroloader-0.1.0/src/hydroloader.egg-info/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)      386 2023-04-13 20:33:18.000000 hydroloader-0.1.0/src/hydroloader.egg-info/SOURCES.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-04-13 20:33:18.000000 hydroloader-0.1.0/src/hydroloader.egg-info/dependency_links.txt
--rw-r--r--   0 klippold   (501) staff       (20)       90 2023-04-13 20:33:18.000000 hydroloader-0.1.0/src/hydroloader.egg-info/requires.txt
--rw-r--r--   0 klippold   (501) staff       (20)       12 2023-04-13 20:33:18.000000 hydroloader-0.1.0/src/hydroloader.egg-info/top_level.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-04-13 20:11:58.000000 hydroloader-0.1.0/src/hydroloader.egg-info/zip-safe
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.515020 hydroloader-0.1.1/
+-rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.1/LICENSE.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-23 01:34:46.515088 hydroloader-0.1.1/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.1/README.md
+-rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.1/pyproject.toml
+-rw-r--r--   0 klippold   (501) staff       (20)      352 2023-06-23 01:34:46.515375 hydroloader-0.1.1/setup.cfg
+-rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.1/setup.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.512218 hydroloader-0.1.1/src/
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.513905 hydroloader-0.1.1/src/hydroloader/
+-rw-r--r--   0 klippold   (501) staff       (20)      337 2023-06-13 00:42:46.000000 hydroloader-0.1.1/src/hydroloader/__init__.py
+-rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.1/src/hydroloader/exceptions.py
+-rw-r--r--   0 klippold   (501) staff       (20)    15287 2023-06-23 00:32:44.000000 hydroloader-0.1.1/src/hydroloader/main.py
+-rw-r--r--   0 klippold   (501) staff       (20)     7793 2023-06-22 20:13:42.000000 hydroloader-0.1.1/src/hydroloader/models.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-23 01:34:46.514757 hydroloader-0.1.1/src/hydroloader.egg-info/
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)      391 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/SOURCES.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/dependency_links.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      101 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/requires.txt
+-rw-r--r--   0 klippold   (501) staff       (20)       12 2023-06-23 01:34:46.000000 hydroloader-0.1.1/src/hydroloader.egg-info/top_level.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.1/src/hydroloader.egg-info/zip-safe
```

### Comparing `hydroloader-0.1.0/LICENSE.txt` & `hydroloader-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

