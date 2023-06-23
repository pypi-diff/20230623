# Comparing `tmp/FrameML-0.1.0.tar.gz` & `tmp/FrameML-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrameML-0.1.0.tar", last modified: Fri Jun 23 15:57:39 2023, max compression
+gzip compressed data, was "FrameML-0.1.1.tar", last modified: Fri Jun 23 17:32:46 2023, max compression
```

## Comparing `FrameML-0.1.0.tar` & `FrameML-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 erika     (1000) wheel      (998)        0 2023-06-23 15:57:39.698335 FrameML-0.1.0/
-drwxr-xr-x   0 erika     (1000) wheel      (998)        0 2023-06-23 15:57:39.698335 FrameML-0.1.0/FrameML.egg-info/
--rw-r--r--   0 erika     (1000) wheel      (998)     2224 2023-06-23 15:57:39.000000 FrameML-0.1.0/FrameML.egg-info/PKG-INFO
--rw-r--r--   0 erika     (1000) wheel      (998)      156 2023-06-23 15:57:39.000000 FrameML-0.1.0/FrameML.egg-info/SOURCES.txt
--rw-r--r--   0 erika     (1000) wheel      (998)        1 2023-06-23 15:57:39.000000 FrameML-0.1.0/FrameML.egg-info/dependency_links.txt
--rw-r--r--   0 erika     (1000) wheel      (998)        1 2023-06-23 15:57:39.000000 FrameML-0.1.0/FrameML.egg-info/top_level.txt
--rw-r--r--   0 erika     (1000) wheel      (998)     1063 2023-06-23 14:56:12.000000 FrameML-0.1.0/LICENSE
--rw-r--r--   0 erika     (1000) wheel      (998)     2224 2023-06-23 15:57:39.698335 FrameML-0.1.0/PKG-INFO
--rw-r--r--   0 erika     (1000) wheel      (998)     1842 2023-06-23 15:27:56.000000 FrameML-0.1.0/README.md
--rw-r--r--   0 erika     (1000) wheel      (998)      459 2023-06-23 15:56:14.000000 FrameML-0.1.0/pyproject.toml
--rw-r--r--   0 erika     (1000) wheel      (998)       38 2023-06-23 15:57:39.698335 FrameML-0.1.0/setup.cfg
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-23 17:32:46.553702 FrameML-0.1.1/
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-23 17:32:46.553434 FrameML-0.1.1/FrameML.egg-info/
+-rw-r--r--   0 jwd2488    (501) staff       (20)     2224 2023-06-23 17:32:46.000000 FrameML-0.1.1/FrameML.egg-info/PKG-INFO
+-rw-r--r--   0 jwd2488    (501) staff       (20)      156 2023-06-23 17:32:46.000000 FrameML-0.1.1/FrameML.egg-info/SOURCES.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)        1 2023-06-23 17:32:46.000000 FrameML-0.1.1/FrameML.egg-info/dependency_links.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)        1 2023-06-23 17:32:46.000000 FrameML-0.1.1/FrameML.egg-info/top_level.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)     1063 2023-06-23 17:28:53.000000 FrameML-0.1.1/LICENSE
+-rw-r--r--   0 jwd2488    (501) staff       (20)     2224 2023-06-23 17:32:46.553587 FrameML-0.1.1/PKG-INFO
+-rw-r--r--   0 jwd2488    (501) staff       (20)     1842 2023-06-23 17:28:53.000000 FrameML-0.1.1/README.md
+-rw-r--r--   0 jwd2488    (501) staff       (20)      459 2023-06-23 17:31:54.000000 FrameML-0.1.1/pyproject.toml
+-rw-r--r--   0 jwd2488    (501) staff       (20)       38 2023-06-23 17:32:46.553742 FrameML-0.1.1/setup.cfg
```

### Comparing `FrameML-0.1.0/FrameML.egg-info/PKG-INFO` & `FrameML-0.1.1/FrameML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrameML
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight markup language for interacting with machine learning models
 Author: Jake Downie, Ronan Maharaj
 Project-URL: homepage, https://github.com/ranger-labs/FrameML
 Project-URL: repository, https://github.com/ranger-labs/FrameML
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FrameML-0.1.0/LICENSE` & `FrameML-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FrameML-0.1.0/PKG-INFO` & `FrameML-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrameML
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight markup language for interacting with machine learning models
 Author: Jake Downie, Ronan Maharaj
 Project-URL: homepage, https://github.com/ranger-labs/FrameML
 Project-URL: repository, https://github.com/ranger-labs/FrameML
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FrameML-0.1.0/README.md` & `FrameML-0.1.1/README.md`

 * *Files identical despite different names*

