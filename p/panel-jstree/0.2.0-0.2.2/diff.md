# Comparing `tmp/panel-jstree-0.2.0.tar.gz` & `tmp/panel-jstree-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panel-jstree-0.2.0.tar", last modified: Thu Jun 22 23:45:54 2023, max compression
+gzip compressed data, was "panel-jstree-0.2.2.tar", last modified: Fri Jun 23 00:21:36 2023, max compression
```

## Comparing `panel-jstree-0.2.0.tar` & `panel-jstree-0.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.523424 panel-jstree-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-22 23:45:54.523424 panel-jstree-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:45:54.523424 panel-jstree-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.511423 panel-jstree-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.515423 panel-jstree-0.2.0/src/panel_jstree/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/bokeh.ext.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.519423 panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/jstree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/jstree.ts
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/layout.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.519423 panel-jstree-0.2.0/src/panel_jstree/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.519423 panel-jstree-0.2.0/src/panel_jstree/dist/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.523424 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/index.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-22 23:45:44.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-22 23:45:44.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-22 23:45:44.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/lib/index.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.js
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    48834 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.json
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-22 23:45:45.000000 panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-22 23:45:42.000000 panel-jstree-0.2.0/src/panel_jstree/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.523424 panel-jstree-0.2.0/src/panel_jstree/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/src/panel_jstree/widgets/jstree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.515423 panel-jstree-0.2.0/src/panel_jstree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-22 23:45:54.000000 panel-jstree-0.2.0/src/panel_jstree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-22 23:45:54.000000 panel-jstree-0.2.0/src/panel_jstree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:45:54.000000 panel-jstree-0.2.0/src/panel_jstree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 23:45:54.000000 panel-jstree-0.2.0/src/panel_jstree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 23:45:54.000000 panel-jstree-0.2.0/src/panel_jstree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:54.523424 panel-jstree-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/tests/test_file_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/tests/test_hello.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:07.000000 panel-jstree-0.2.0/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.491421 panel-jstree-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh.ext.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.ts
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/layout.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/dist/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    48834 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-23 00:21:26.000000 panel-jstree-0.2.2/src/panel_jstree/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/src/panel_jstree/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/widgets/jstree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/tests/test_file_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/tests/test_hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/tests/test_tree.py
```

### Comparing `panel-jstree-0.2.0/LICENSE` & `panel-jstree-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/PKG-INFO` & `panel-jstree-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panel-jstree
-Version: 0.2.0
+Version: 0.2.2
 Summary: panel-jstree is a wrapper python wrapper around the javascript library jstree for use in panel. This allows for JSON-like representations of tree data. One very useful implementation provided is a server-side file browser.
 Author: madeline-scyphers
 License: MIT License
         
         Copyright (c) 2023 Madeline Scyphers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,15 +67,15 @@
 ```python
 import panel as pn
 from panel_jstree import FileTree
 
 pn.Column(FileTree())
 ```
 
-![Project Intro](https://github.com/madeline-scyphers/panel-jstree/blob/c0c182e09f028fe0fdb963d82ab2cdaad5128a1b/assets/videos/project-intro.gif)
+![Project Intro](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/project-intro.gif)
 
 ## 🚀 Get started in under a minute
 
 ```bash
 pip install  panel-jstree
 ```
 
@@ -83,19 +83,19 @@
 
 ```bash
 panel serve examples/*.py --show
 ```
 
 Here are some of the examples. You can see a small FileTree app with a text field and controls to directly input a file path, and turn off and on some of the controls.
 
-![FileTree App Example](https://github.com/madeline-scyphers/panel-jstree/blob/777b299badf308746ff2ea0843755a12fe6158b4/assets/videos/file-tree.gif)
+![FileTree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/file-tree.gif)
 
 You can also see a generic Tree app with a custom callback to generate random nodes.
 
-![Randomw Tree App Example](https://github.com/madeline-scyphers/panel-jstree/blob/777b299badf308746ff2ea0843755a12fe6158b4/assets/videos/random-tree.gif)
+![Randomw Tree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/random-tree.gif)
 
 
 ## ⭐ Support
 
 Please support [Panel](https://panel.holoviz.org) and
 [panel-jstree](https://github.com/madeline-scyphers/panel-jstree) by giving the projects a star on Github.
```

### Comparing `panel-jstree-0.2.0/README.md` & `panel-jstree-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```python
 import panel as pn
 from panel_jstree import FileTree
 
 pn.Column(FileTree())
 ```
 
-![Project Intro](https://github.com/madeline-scyphers/panel-jstree/blob/c0c182e09f028fe0fdb963d82ab2cdaad5128a1b/assets/videos/project-intro.gif)
+![Project Intro](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/project-intro.gif)
 
 ## 🚀 Get started in under a minute
 
 ```bash
 pip install  panel-jstree
 ```
 
@@ -27,19 +27,19 @@
 
 ```bash
 panel serve examples/*.py --show
 ```
 
 Here are some of the examples. You can see a small FileTree app with a text field and controls to directly input a file path, and turn off and on some of the controls.
 
-![FileTree App Example](https://github.com/madeline-scyphers/panel-jstree/blob/777b299badf308746ff2ea0843755a12fe6158b4/assets/videos/file-tree.gif)
+![FileTree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/file-tree.gif)
 
 You can also see a generic Tree app with a custom callback to generate random nodes.
 
-![Randomw Tree App Example](https://github.com/madeline-scyphers/panel-jstree/blob/777b299badf308746ff2ea0843755a12fe6158b4/assets/videos/random-tree.gif)
+![Randomw Tree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/random-tree.gif)
 
 
 ## ⭐ Support
 
 Please support [Panel](https://panel.holoviz.org) and
 [panel-jstree](https://github.com/madeline-scyphers/panel-jstree) by giving the projects a star on Github.
```

### Comparing `panel-jstree-0.2.0/pyproject.toml` & `panel-jstree-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/jstree.py` & `panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.py`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/jstree.ts` & `panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/bokeh_extensions/layout.ts` & `panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/layout.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts` & `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js` & `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map` & `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts` & `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js` & `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map` & `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.js` & `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.js.map` & `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js.map`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.json` & `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.json`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/dist/panel_jstree.min.js` & `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.min.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/package-lock.json` & `panel-jstree-0.2.2/src/panel_jstree/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9161931818181818%*

 * *Differences: {"'packages'": "{'': {'version': '0.2.2'}}", "'version'": "'0.2.2'"}*

```diff
@@ -68,15 +68,15 @@
         "": {
             "dependencies": {
                 "@bokeh/bokehjs": "^3.1",
                 "@holoviz/panel": "^1"
             },
             "license": "MIT",
             "name": "panel_jstree",
-            "version": "0.2.0"
+            "version": "0.2.2"
         },
         "node_modules/@bokeh/bokehjs": {
             "engines": {
                 "node": ">=16.0",
                 "npm": ">=8.0"
             },
             "integrity": "sha512-+S3hqhIaOS17Xp0Oy7fB+hhOPe+v3jeIew40sWaH4/DEEMuUmhDZZMFowWhicuwTN9J6Bay9bp/62YJc5Na1Qg==",
@@ -141,9 +141,9 @@
             },
             "integrity": "sha512-4oh2sf208mKAdL5AQtzXxE387iSGNWMX/YjwMjH6m/XROILKAmx5Pbs2FsXrW7ixoVGGjpfYSBB833vOwYxNxw==",
             "resolved": "https://registry.npmjs.org/preact/-/preact-10.14.0.tgz",
             "version": "10.14.0"
         }
     },
     "requires": true,
-    "version": "0.2.0"
+    "version": "0.2.2"
 }
```

### Comparing `panel-jstree-0.2.0/src/panel_jstree/tsconfig.json` & `panel-jstree-0.2.2/src/panel_jstree/tsconfig.json`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree/widgets/jstree.py` & `panel-jstree-0.2.2/src/panel_jstree/widgets/jstree.py`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.0/src/panel_jstree.egg-info/PKG-INFO` & `panel-jstree-0.2.2/src/panel_jstree.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panel-jstree
-Version: 0.2.0
+Version: 0.2.2
 Summary: panel-jstree is a wrapper python wrapper around the javascript library jstree for use in panel. This allows for JSON-like representations of tree data. One very useful implementation provided is a server-side file browser.
 Author: madeline-scyphers
 License: MIT License
         
         Copyright (c) 2023 Madeline Scyphers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,15 +67,15 @@
 ```python
 import panel as pn
 from panel_jstree import FileTree
 
 pn.Column(FileTree())
 ```
 
-![Project Intro](https://github.com/madeline-scyphers/panel-jstree/blob/c0c182e09f028fe0fdb963d82ab2cdaad5128a1b/assets/videos/project-intro.gif)
+![Project Intro](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/project-intro.gif)
 
 ## 🚀 Get started in under a minute
 
 ```bash
 pip install  panel-jstree
 ```
 
@@ -83,19 +83,19 @@
 
 ```bash
 panel serve examples/*.py --show
 ```
 
 Here are some of the examples. You can see a small FileTree app with a text field and controls to directly input a file path, and turn off and on some of the controls.
 
-![FileTree App Example](https://github.com/madeline-scyphers/panel-jstree/blob/777b299badf308746ff2ea0843755a12fe6158b4/assets/videos/file-tree.gif)
+![FileTree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/file-tree.gif)
 
 You can also see a generic Tree app with a custom callback to generate random nodes.
 
-![Randomw Tree App Example](https://github.com/madeline-scyphers/panel-jstree/blob/777b299badf308746ff2ea0843755a12fe6158b4/assets/videos/random-tree.gif)
+![Randomw Tree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/random-tree.gif)
 
 
 ## ⭐ Support
 
 Please support [Panel](https://panel.holoviz.org) and
 [panel-jstree](https://github.com/madeline-scyphers/panel-jstree) by giving the projects a star on Github.
```

### Comparing `panel-jstree-0.2.0/src/panel_jstree.egg-info/SOURCES.txt` & `panel-jstree-0.2.2/src/panel_jstree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

