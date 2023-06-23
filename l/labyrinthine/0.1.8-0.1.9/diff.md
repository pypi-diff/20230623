# Comparing `tmp/labyrinthine-0.1.8.tar.gz` & `tmp/labyrinthine-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labyrinthine-0.1.8.tar", last modified: Wed Jun 21 20:09:53 2023, max compression
+gzip compressed data, was "labyrinthine-0.1.9.tar", last modified: Thu Jun 22 10:38:08 2023, max compression
```

## Comparing `labyrinthine-0.1.8.tar` & `labyrinthine-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/labyrinthine/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/labyrinthine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/labyrinthine/depth_first.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/labyrinthine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 20:09:53.000000 labyrinthine-0.1.8/labyrinthine.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-21 20:09:44.000000 labyrinthine-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 20:09:53.384826 labyrinthine-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:38:08.399934 labyrinthine-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 10:37:46.000000 labyrinthine-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-22 10:38:08.399934 labyrinthine-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-22 10:37:46.000000 labyrinthine-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:38:08.399934 labyrinthine-0.1.9/labyrinthine/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-22 10:37:46.000000 labyrinthine-0.1.9/labyrinthine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-22 10:37:46.000000 labyrinthine-0.1.9/labyrinthine/depth_first.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:38:08.399934 labyrinthine-0.1.9/labyrinthine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-22 10:38:08.000000 labyrinthine-0.1.9/labyrinthine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 10:38:08.000000 labyrinthine-0.1.9/labyrinthine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:38:08.000000 labyrinthine-0.1.9/labyrinthine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 10:38:08.000000 labyrinthine-0.1.9/labyrinthine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:38:08.000000 labyrinthine-0.1.9/labyrinthine.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-22 10:37:46.000000 labyrinthine-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-22 10:38:08.399934 labyrinthine-0.1.9/setup.cfg
```

### Comparing `labyrinthine-0.1.8/LICENSE` & `labyrinthine-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `labyrinthine-0.1.8/PKG-INFO` & `labyrinthine-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labyrinthine
-Version: 0.1.8
+Version: 0.1.9
 Summary: A no-dependency library that generates all the mazes you need.
 Author-email: Roberto Schiavone <hello@robertoschiavone.io>
 Maintainer-email: Roberto Schiavone <hello@robertoschiavone.io>
 License: MIT License
         
         Copyright (c) 2023 Roberto Schiavone
```

### Comparing `labyrinthine-0.1.8/README.md` & `labyrinthine-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `labyrinthine-0.1.8/labyrinthine/depth_first.py` & `labyrinthine-0.1.9/labyrinthine/depth_first.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 
 from types import NoneType
 from typing import List, Tuple, Union
 
 
-def compute_neighbors(matrix: List[List[int]], cell: Tuple[int, int]) -> list[int]:
+def compute_neighbors(matrix: List[List[int]], cell: Tuple[int, int]) -> List[int]:
     result = []
     x, y = cell
     max_width, max_height = len(matrix), len(matrix[0])
     if x + 2 < max_width:
         result += [(x + 2, y)]
     if x - 2 >= 0:
         result += [(x - 2, y)]
```

### Comparing `labyrinthine-0.1.8/labyrinthine.egg-info/PKG-INFO` & `labyrinthine-0.1.9/labyrinthine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labyrinthine
-Version: 0.1.8
+Version: 0.1.9
 Summary: A no-dependency library that generates all the mazes you need.
 Author-email: Roberto Schiavone <hello@robertoschiavone.io>
 Maintainer-email: Roberto Schiavone <hello@robertoschiavone.io>
 License: MIT License
         
         Copyright (c) 2023 Roberto Schiavone
```

### Comparing `labyrinthine-0.1.8/pyproject.toml` & `labyrinthine-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "labyrinthine"
-version = "0.1.8"
+version = "0.1.9"
 description = """A no-dependency library that generates all the mazes you need."""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.5"
 license = { file = "LICENSE" }
 authors = [
     { name = "Roberto Schiavone", email = "hello@robertoschiavone.io" },
 ]
```

