# Comparing `tmp/frameml-0.1.2.tar.gz` & `tmp/frameml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frameml-0.1.2.tar", last modified: Fri Jun 23 17:37:01 2023, max compression
+gzip compressed data, was "frameml-0.1.3.tar", last modified: Fri Jun 23 18:02:39 2023, max compression
```

## Comparing `frameml-0.1.2.tar` & `frameml-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-23 17:37:01.274263 frameml-0.1.2/
-drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-23 17:37:01.273879 frameml-0.1.2/FrameML.egg-info/
--rw-r--r--   0 jwd2488    (501) staff       (20)     2224 2023-06-23 17:37:01.000000 frameml-0.1.2/FrameML.egg-info/PKG-INFO
--rw-r--r--   0 jwd2488    (501) staff       (20)      280 2023-06-23 17:37:01.000000 frameml-0.1.2/FrameML.egg-info/SOURCES.txt
--rw-r--r--   0 jwd2488    (501) staff       (20)        1 2023-06-23 17:37:01.000000 frameml-0.1.2/FrameML.egg-info/dependency_links.txt
--rw-r--r--   0 jwd2488    (501) staff       (20)        1 2023-06-23 17:37:01.000000 frameml-0.1.2/FrameML.egg-info/top_level.txt
--rw-r--r--   0 jwd2488    (501) staff       (20)     1063 2023-06-23 17:28:53.000000 frameml-0.1.2/LICENSE
--rw-r--r--   0 jwd2488    (501) staff       (20)     2224 2023-06-23 17:37:01.274165 frameml-0.1.2/PKG-INFO
--rw-r--r--   0 jwd2488    (501) staff       (20)     1842 2023-06-23 17:28:53.000000 frameml-0.1.2/README.md
--rw-r--r--   0 jwd2488    (501) staff       (20)      459 2023-06-23 17:36:06.000000 frameml-0.1.2/pyproject.toml
--rw-r--r--   0 jwd2488    (501) staff       (20)       38 2023-06-23 17:37:01.274300 frameml-0.1.2/setup.cfg
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-23 18:02:39.219958 frameml-0.1.3/
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-23 18:02:39.219070 frameml-0.1.3/FrameML.egg-info/
+-rw-r--r--   0 jwd2488    (501) staff       (20)     2224 2023-06-23 18:02:39.000000 frameml-0.1.3/FrameML.egg-info/PKG-INFO
+-rw-r--r--   0 jwd2488    (501) staff       (20)      319 2023-06-23 18:02:39.000000 frameml-0.1.3/FrameML.egg-info/SOURCES.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)        1 2023-06-23 18:02:39.000000 frameml-0.1.3/FrameML.egg-info/dependency_links.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)        8 2023-06-23 18:02:39.000000 frameml-0.1.3/FrameML.egg-info/top_level.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)     1063 2023-06-23 17:28:53.000000 frameml-0.1.3/LICENSE
+-rw-r--r--   0 jwd2488    (501) staff       (20)     2224 2023-06-23 18:02:39.219836 frameml-0.1.3/PKG-INFO
+-rw-r--r--   0 jwd2488    (501) staff       (20)     1842 2023-06-23 17:28:53.000000 frameml-0.1.3/README.md
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-23 18:02:39.219296 frameml-0.1.3/frameml/
+-rw-r--r--   0 jwd2488    (501) staff       (20)        0 2023-06-23 18:00:03.000000 frameml-0.1.3/frameml/__init__.py
+-rw-r--r--   0 jwd2488    (501) staff       (20)     7691 2023-06-23 17:59:33.000000 frameml-0.1.3/frameml/frameml.py
+-rw-r--r--   0 jwd2488    (501) staff       (20)      459 2023-06-23 18:01:48.000000 frameml-0.1.3/pyproject.toml
+-rw-r--r--   0 jwd2488    (501) staff       (20)       38 2023-06-23 18:02:39.220000 frameml-0.1.3/setup.cfg
```

### Comparing `frameml-0.1.2/FrameML.egg-info/PKG-INFO` & `frameml-0.1.3/FrameML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frameml
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight markup language for interacting with machine learning models
 Author: Jake Downie, Ronan Maharaj
 Project-URL: homepage, https://github.com/ranger-labs/FrameML
 Project-URL: repository, https://github.com/ranger-labs/FrameML
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `frameml-0.1.2/LICENSE` & `frameml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `frameml-0.1.2/PKG-INFO` & `frameml-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frameml
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight markup language for interacting with machine learning models
 Author: Jake Downie, Ronan Maharaj
 Project-URL: homepage, https://github.com/ranger-labs/FrameML
 Project-URL: repository, https://github.com/ranger-labs/FrameML
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `frameml-0.1.2/README.md` & `frameml-0.1.3/README.md`

 * *Files identical despite different names*

