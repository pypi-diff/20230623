# Comparing `tmp/panel-jstree-0.2.2.tar.gz` & `tmp/panel-jstree-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panel-jstree-0.2.2.tar", last modified: Fri Jun 23 00:21:36 2023, max compression
+gzip compressed data, was "panel-jstree-0.3.0.tar", last modified: Fri Jun 23 21:37:42 2023, max compression
```

## Comparing `panel-jstree-0.2.2.tar` & `panel-jstree-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.491421 panel-jstree-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh.ext.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.ts
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/layout.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree/dist/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/index.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/lib/index.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    48834 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.json
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-23 00:21:28.000000 panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-23 00:21:26.000000 panel-jstree-0.2.2/src/panel_jstree/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/src/panel_jstree/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/src/panel_jstree/widgets/jstree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.495422 panel-jstree-0.2.2/src/panel_jstree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 00:21:36.000000 panel-jstree-0.2.2/src/panel_jstree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:21:36.499422 panel-jstree-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/tests/test_file_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/tests/test_hello.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:20:55.000000 panel-jstree-0.2.2/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.895057 panel-jstree-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-23 21:37:42.895057 panel-jstree-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:37:42.895057 panel-jstree-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.887056 panel-jstree-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.891057 panel-jstree-0.3.0/src/panel_jstree/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/bokeh.ext.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.891057 panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/jstree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/jstree.ts
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/layout.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.891057 panel-jstree-0.3.0/src/panel_jstree/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.891057 panel-jstree-0.3.0/src/panel_jstree/dist/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.895057 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 21:37:35.000000 panel-jstree-0.3.0/src/panel_jstree/dist/lib/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-06-23 21:37:36.000000 panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-06-23 21:37:36.000000 panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50271 2023-06-23 21:37:36.000000 panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-06-23 21:37:36.000000 panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-23 21:37:34.000000 panel-jstree-0.3.0/src/panel_jstree/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.895057 panel-jstree-0.3.0/src/panel_jstree/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/src/panel_jstree/widgets/jstree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.891057 panel-jstree-0.3.0/src/panel_jstree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-23 21:37:42.000000 panel-jstree-0.3.0/src/panel_jstree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-23 21:37:42.000000 panel-jstree-0.3.0/src/panel_jstree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:37:42.000000 panel-jstree-0.3.0/src/panel_jstree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 21:37:42.000000 panel-jstree-0.3.0/src/panel_jstree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 21:37:42.000000 panel-jstree-0.3.0/src/panel_jstree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:42.895057 panel-jstree-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/tests/test_file_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/tests/test_hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/tests/test_random_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-23 21:37:05.000000 panel-jstree-0.3.0/tests/test_tree.py
```

### Comparing `panel-jstree-0.2.2/LICENSE` & `panel-jstree-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.2/PKG-INFO` & `panel-jstree-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panel-jstree
-Version: 0.2.2
+Version: 0.3.0
 Summary: panel-jstree is a wrapper python wrapper around the javascript library jstree for use in panel. This allows for JSON-like representations of tree data. One very useful implementation provided is a server-side file browser.
 Author: madeline-scyphers
 License: MIT License
         
         Copyright (c) 2023 Madeline Scyphers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,14 +28,15 @@
 Keywords: python,holoviz,panel,dataviz,dataapp,dashboard,datascience,analytics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
@@ -57,42 +58,57 @@
 # ✨ panel-jstree
 
 panel-jstree is a wrapper python wrapper around the javascript library [jstree](https://www.jstree.com) for use in [panel](https://panel.holoviz.org/). This allows for JSON-like representations of tree data. One very useful implementation provided is a server-side file browser.
 
 You can install and use the package as simple as.
 
 ```bash
+conda install -c conda-forge panel-jstree
+```
+
+or with pip
+
+```bash
 pip install panel-jstree
 ```
 
+Add this into a python file to play with the FileTree
+
 ```python
-import panel as pn
 from panel_jstree import FileTree
 
-pn.Column(FileTree())
+FileTree().servable()
 ```
 
+run it with `panel serve name_of_app.py`
+
+It should run exploring the directory of the file.
+
 ![Project Intro](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/project-intro.gif)
 
 ## 🚀 Get started in under a minute
 
 ```bash
 pip install  panel-jstree
 ```
 
 Run the examples
 
 ```bash
-panel serve examples/*.py --show
+panel serve tests/*tree.py --show
 ```
 
 Here are some of the examples. You can see a small FileTree app with a text field and controls to directly input a file path, and turn off and on some of the controls.
 
 ![FileTree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/file-tree.gif)
 
+You can make a simple tree where you swap out the data.
+
+![Randomw Tree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/simple-tree.gif)
+
 You can also see a generic Tree app with a custom callback to generate random nodes.
 
 ![Randomw Tree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/random-tree.gif)
 
 
 ## ⭐ Support
 
@@ -105,11 +121,14 @@
 
 If you are looking to contribute to this project you can find ideas in the [issue tracker](https://github.com/madeline-scyphers/panel-jstree/issues). To get started check out the [DEVELOPER_GUIDE](DEVELOPER_GUIDE.md).
 
 I would love to support and receive your contributions. Thanks.
 
 ## Monitor
 
-[![PyPI version](https://badge.fury.io/py/panel-jstree.svg)](https://pypi.org/project/panel-jstree/)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
-[![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIT)
-
+|                 |                                                                                                                                                                         |
+|-----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Conda Install   | [![Conda Version](https://anaconda.org/conda-forge/panel-jstree/badges/version.svg)](https://anaconda.org/conda-forge/panel-jstree)                                     |
+| PyPI Install    | [![PyPI version](https://badge.fury.io/py/panel-jstree.svg)](https://badge.fury.io/py/panel-jstree)                                                                     |
+| Github release  | [![Github tag](https://img.shields.io/github/v/tag/madeline-scyphers/panel-jstree.svg?label=tag&colorB=11ccbb)](https://github.com/madeline-scyphers/panel-jstree/tags) |
+| Python Versions | ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)                                                                               |
+| License         | [![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIT)                                                              |
```

### Comparing `panel-jstree-0.2.2/pyproject.toml` & `panel-jstree-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Legal Industry",
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.py` & `panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/jstree.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
     __javascript__ = [
         "https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js",
         "https://cdnjs.cloudflare.com/ajax/libs/jstree/3.3.12/jstree.min.js",
     ]
 
     plugins = List(Any)
+    checkbox = Bool(default=True)
     multiple = Bool(default=True)
     show_icons = Bool(default=True)
     show_dots = Bool(default=True)
     _last_opened = Dict(String, Any)
     _new_nodes = List(Any)
     _flat_tree = List(Any)
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/jstree.ts` & `panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/jstree.ts`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     connect_signals(): void {
         console.log("connect")
         super.connect_signals()
         this.connect(this.model.properties._data.change, () => this._update_tree_from_data())
         this.connect(this.model.properties.value.change, () => this._update_selection_from_value())
         this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes())
+        this.connect(this.model.properties.checkbox.change, () => this.setCheckboxes())
         this.connect(this.model.properties.show_icons.change, () => this._setShowIcons())
         this.connect(this.model.properties.show_dots.change, () => this._setShowDots())
         this.connect(this.model.properties.multiple.change, () => this._setMultiple())
         console.log(this.model.show_dots)
         console.log(this.model.show_icons)
     }
 
@@ -45,17 +46,22 @@
         this._id = ID()
         console.log(this._id)
         this._container = div({id: this._id, style: "overflow: auto; minHeight: 200px; minWidth: 200px;"},)
         set_size(this._container, this.model)
         this.shadow_el.appendChild(this._container);
         console.log(this._container)
 
+        if (this.model.checkbox) {
+            this.model.plugins.push("checkbox")
+        }
+
         let kw = {"checkbox": {
             "three_state": false,
-            "cascade": "undetermined"}}
+            "cascade": "undetermined"
+        }}
 
         this._jstree = jQuery(this._container).jstree(
             { "core":
                 {"data": this.model._data, "check_callback": true,
                  "multiple": this.model.multiple,
                  "themes": {
                     "dots": this.model.show_dots,
@@ -66,27 +72,27 @@
                 ...kw
             }
             );
         this.init_callbacks()
     }
     init_callbacks(): void {
         // Initialization
-        this._jstree.on('ready.jstree', ({}, {}) => this.onjsTreeInit());
 
         // Rendering callbacks
         // TODO: do I need both of these?
         this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());
 
         // Sync state with model
+        this._jstree.on('model.jstree', ({}, {}) => this.onNewData());
         this._jstree.on('activate_node.jstree', ({}, data: any) => this.selectNodeFromEditor({}, data));
         this._jstree.on('before_open.jstree', (e: any, data: any) => this._listen_for_node_open(e, data));
 
     }
 
-    onjsTreeInit(): void {
+    onNewData(): void {
         this.model._flat_tree = this._jstree.jstree(true).get_json(null, {"flat": true})
         console.log("flat tree: ", this.model._flat_tree)
     }
 
     selectNodeFromEditor({}, data: any): void {
         console.log("select pre", this.model.value)
         this.model.value = data.instance.get_selected();
@@ -102,21 +108,14 @@
         if (this.model.value != this._last_selected) {
             let deselected = this._last_selected.filter(x => !this.model.value.includes(x));
             this._jstree.jstree(true).deselect_node(deselected)
         }
         // We choose get_selected
         this._last_selected = this.model.value;
 
-
-        if (this.model.show_icons) {
-            this._jstree.jstree(true).show_icons ( );
-        }
-        else {
-            this._jstree.jstree(true).hide_icons ( );
-        }
     }
 
     _update_tree_from_new_nodes(): void {
         console.log("new nodes: ", this.model._new_nodes)
         for (let node of this.model._new_nodes){
             this._jstree.jstree(true).create_node(node["parent"], node, "first")
         }
@@ -125,29 +124,31 @@
         // this._update_selection_from_value()
     }
 
     _update_tree_from_data(): void {
         console.log("updating data")
         this._jstree.jstree(true).settings.core.data = this.model._data;
         console.log("data: ", this._jstree.jstree(true).settings.core.data)
-        this.model._flat_tree = this._jstree.jstree(true).get_json(null, {"flat": true})
-        console.log("flat tree: ", this.model._flat_tree)
         console.log("value after data", this.model.value)
         // This will redraw the tree if we swap out the data with new data
         // we set forget_state to true, so the current state is not reapplied
-        // letting whatever state is set in the new data (open or closed, selected, etc)
+        // letting whatever state is set in the new data (open or closed, etc)
         // be the new state
         this._jstree.jstree(true).refresh(
             {"skip_loading": false,
             "forget_state": true});
 
+        // selected state is not preserved correctly right now, so we then
+        // deselect everything because that is better than getting it wrong
+        this._jstree.jstree(true).deselect_all({"supress_event": true})
+
         console.log("value after refresh", this.model.value)
+        console.log("data after refresh", this._jstree.jstree(true).settings.core.data)
     }
 
-
     _setShowIcons(): void {
         console.log("setShowIcons")
         if (this.model.show_icons) {
             this._jstree.jstree(true).show_icons ( );
         }
         else {
             this._jstree.jstree(true).hide_icons ( );
@@ -159,20 +160,30 @@
             this._jstree.jstree(true).show_dots ( );
         }
         else {
             this._jstree.jstree(true).hide_dots ( );
         }
     }
 
+    setCheckboxes(): void {
+        console.log("setCheckBoxes")
+        if (this.model.checkbox) {
+            this._jstree.jstree(true).show_checkboxes();
+        }
+        else {
+            this._jstree.jstree(true).hide_checkboxes();
+        }
+    }
+
     _setMultiple(): void {
         console.log("setMultiple")
         this._jstree.jstree(true).settings.core.multiple = this.model.multiple
     }
 
-    _update_tree_theme_from_model(): void {
+    _update_tree_theme_from_model(): void {  // TODO can we remove this?
         this._jstree.jstree(true).refresh(false, true);
     }
 
     _listen_for_node_open({}, data: any): void {
         console.log("listen for node open")
         data.node = this.add_node_children(data.node)
         this.model._last_opened = data.node
@@ -190,14 +201,15 @@
 }
 
 export namespace jsTreePlot {
   export type Attrs = p.AttrsOf<Props>
   export type Props = HTMLBox.Props & {
     _data: p.Property<any>
     plugins: p.Property<any>
+    checkbox: p.Property<boolean>
     multiple: p.Property<boolean>
     show_icons: p.Property<boolean>
     show_dots: p.Property<boolean>
     value: p.Property<any>
     _last_opened: p.Property<any>
     _new_nodes: p.Property<any>
     _flat_tree: p.Property<any>
@@ -218,14 +230,15 @@
     static {
       this.prototype.default_view = jsTreePlotView
 
       this.define<jsTreePlot.Props>(({Array, Any, Boolean}) => ({
         value:          [ Array(Any), []     ],
         _data:          [ Array(Any), []     ],
         plugins:       [ Array(Any), []     ],
+        checkbox:      [ Boolean, true ],
         multiple:      [ Boolean, true ],
         show_icons:    [ Boolean, true ],
         show_dots:     [ Boolean, true ],
         _last_opened: [ Any, {} ],
         _new_nodes: [ Array(Any), [] ],
         _flat_tree: [ Array(Any), []     ],
       }))
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/bokeh_extensions/layout.ts` & `panel-jstree-0.3.0/src/panel_jstree/bokeh_extensions/layout.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts` & `panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts`

 * *Files 11% similar despite different names*

```diff
@@ -9,31 +9,33 @@
     protected _id: any;
     protected _jstree: any;
     protected _last_selected: string[];
     initialize(): void;
     connect_signals(): void;
     render(): void;
     init_callbacks(): void;
-    onjsTreeInit(): void;
+    onNewData(): void;
     selectNodeFromEditor({}: {}, data: any): void;
     _update_selection_from_value(): void;
     _update_tree_from_new_nodes(): void;
     _update_tree_from_data(): void;
     _setShowIcons(): void;
     _setShowDots(): void;
+    setCheckboxes(): void;
     _setMultiple(): void;
     _update_tree_theme_from_model(): void;
     _listen_for_node_open({}: {}, data: any): void;
     add_node_children(node: Node): Node;
 }
 export declare namespace jsTreePlot {
     type Attrs = p.AttrsOf<Props>;
     type Props = HTMLBox.Props & {
         _data: p.Property<any>;
         plugins: p.Property<any>;
+        checkbox: p.Property<boolean>;
         multiple: p.Property<boolean>;
         show_icons: p.Property<boolean>;
         show_dots: p.Property<boolean>;
         value: p.Property<any>;
         _last_opened: p.Property<any>;
         _new_nodes: p.Property<any>;
         _flat_tree: p.Property<any>;
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js` & `panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -21,14 +21,15 @@
     }
     connect_signals() {
         console.log("connect");
         super.connect_signals();
         this.connect(this.model.properties._data.change, () => this._update_tree_from_data());
         this.connect(this.model.properties.value.change, () => this._update_selection_from_value());
         this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());
+        this.connect(this.model.properties.checkbox.change, () => this.setCheckboxes());
         this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());
         this.connect(this.model.properties.show_dots.change, () => this._setShowDots());
         this.connect(this.model.properties.multiple.change, () => this._setMultiple());
         console.log(this.model.show_dots);
         console.log(this.model.show_icons);
     }
     render() {
@@ -38,14 +39,17 @@
         this._container = div({
             id: this._id,
             style: "overflow: auto; minHeight: 200px; minWidth: 200px;"
         });
         set_size(this._container, this.model);
         this.shadow_el.appendChild(this._container);
         console.log(this._container);
+        if (this.model.checkbox) {
+            this.model.plugins.push("checkbox");
+        }
         let kw = {
             "checkbox": {
                 "three_state": false,
                 "cascade": "undetermined"
             }
         };
         this._jstree = jQuery(this._container).jstree({
@@ -61,23 +65,23 @@
             "plugins": this.model.plugins,
             ...kw
         });
         this.init_callbacks();
     }
     init_callbacks() {
         // Initialization
-        this._jstree.on('ready.jstree', ({}, {}) => this.onjsTreeInit());
         // Rendering callbacks
         // TODO: do I need both of these?
         this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());
         // Sync state with model
+        this._jstree.on('model.jstree', ({}, {}) => this.onNewData());
         this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));
         this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));
     }
-    onjsTreeInit() {
+    onNewData() {
         this.model._flat_tree = this._jstree.jstree(true).get_json(null, {
             "flat": true
         });
         console.log("flat tree: ", this.model._flat_tree);
     }
     selectNodeFromEditor({}, data) {
         console.log("select pre", this.model.value);
@@ -92,19 +96,14 @@
         // by comparing to last_selected
         if (this.model.value != this._last_selected) {
             let deselected = this._last_selected.filter(x => !this.model.value.includes(x));
             this._jstree.jstree(true).deselect_node(deselected);
         }
         // We choose get_selected
         this._last_selected = this.model.value;
-        if (this.model.show_icons) {
-            this._jstree.jstree(true).show_icons();
-        } else {
-            this._jstree.jstree(true).hide_icons();
-        }
     }
     _update_tree_from_new_nodes() {
         console.log("new nodes: ", this.model._new_nodes);
         for (let node of this.model._new_nodes) {
             this._jstree.jstree(true).create_node(node["parent"], node, "first");
         }
         this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, {
@@ -115,28 +114,30 @@
         this.model._data = this._jstree.jstree(true).settings.core.data;
         // this._update_selection_from_value()
     }
     _update_tree_from_data() {
         console.log("updating data");
         this._jstree.jstree(true).settings.core.data = this.model._data;
         console.log("data: ", this._jstree.jstree(true).settings.core.data);
-        this.model._flat_tree = this._jstree.jstree(true).get_json(null, {
-            "flat": true
-        });
-        console.log("flat tree: ", this.model._flat_tree);
         console.log("value after data", this.model.value);
         // This will redraw the tree if we swap out the data with new data
         // we set forget_state to true, so the current state is not reapplied
-        // letting whatever state is set in the new data (open or closed, selected, etc)
+        // letting whatever state is set in the new data (open or closed, etc)
         // be the new state
         this._jstree.jstree(true).refresh({
             "skip_loading": false,
             "forget_state": true
         });
+        // selected state is not preserved correctly right now, so we then
+        // deselect everything because that is better than getting it wrong
+        this._jstree.jstree(true).deselect_all({
+            "supress_event": true
+        });
         console.log("value after refresh", this.model.value);
+        console.log("data after refresh", this._jstree.jstree(true).settings.core.data);
     }
     _setShowIcons() {
         console.log("setShowIcons");
         if (this.model.show_icons) {
             this._jstree.jstree(true).show_icons();
         } else {
             this._jstree.jstree(true).hide_icons();
@@ -146,14 +147,22 @@
         console.log("setShowDots");
         if (this.model.show_dots) {
             this._jstree.jstree(true).show_dots();
         } else {
             this._jstree.jstree(true).hide_dots();
         }
     }
+    setCheckboxes() {
+        console.log("setCheckBoxes");
+        if (this.model.checkbox) {
+            this._jstree.jstree(true).show_checkboxes();
+        } else {
+            this._jstree.jstree(true).hide_checkboxes();
+        }
+    }
     _setMultiple() {
         console.log("setMultiple");
         this._jstree.jstree(true).settings.core.multiple = this.model.multiple;
     }
     _update_tree_theme_from_model() {
         this._jstree.jstree(true).refresh(false, true);
     }
@@ -186,14 +195,15 @@
         Array,
         Any,
         Boolean
     }) => ({
         value: [Array(Any), []],
         _data: [Array(Any), []],
         plugins: [Array(Any), []],
+        checkbox: [Boolean, true],
         multiple: [Boolean, true],
         show_icons: [Boolean, true],
         show_dots: [Boolean, true],
         _last_opened: [Any, {}],
         _new_nodes: [Array(Any), []],
         _flat_tree: [Array(Any), []],
     }));
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map` & `panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "';AACA,OAAO,EAAE,GAAG,EAAE,MAAM,mBAAmB,CAAA;AACvC,OAAO,EAAC,OAAO,EAAE,WAAW,EAAE,QAAQ,EAAC,MAAM,UAAU,CAAA;AAQvD,SAAS,EAAE;IACP,iEAAiE;IACjE,6EAA6E;IAC7E,qBAAqB;IACrB,OAAO,GAAG,GAAG,IAAI,CAAC,MAAM,EAAE,CAAC,QAAQ,CAAC,EAAE,CAAC,CAAC,SAAS,CAAC,CAAC,EAAE,EAAE,CAAC,CAAC;AAC7D,CAAC;AAED,MAAM,OAAO,cAAe,SAAQ,WAAW;IAO3C,UAAU;QACR,KAAK,CAAC,UAAU,EAAE,CAAA;QAChB,IAAI,CAAC,cAAc,GAAG,EAAE,CAAA;IAC5B,CAAC;IAED,eAAe;QACX,OAAO,CAAC,GAAG,CAAC,SAAS,CAAC,CAAA;QACtB,KAAK,CAAC,eAAe,EAAE,CAAA;QACvB,IAAI,CAAC,OAAO, […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "jstree.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../../../bokeh_extensions/jstree.ts"
     ],
     "version": 3
 }
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts` & `panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js` & `panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map` & `panel-jstree-0.3.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js` & `panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -51,20 +51,20 @@
                 exports.PaneljsTree = PaneljsTree;
                 const base_1 = require("@bokehjs/base");
                 (0, base_1.register_models)(PaneljsTree);
             },
             "ef403b5ad2": /* bokeh_extensions/index.js */ function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const tslib_1 = require("tslib");
-                const jsTree = tslib_1.__importStar(require("c52315dab1") /* ./jstree */ );
+                const jsTree = tslib_1.__importStar(require("79591b3bf4") /* ./jstree */ );
                 exports.jsTree = jsTree;
                 const base_1 = require("@bokehjs/base");
                 (0, base_1.register_models)(jsTree);
             },
-            "c52315dab1": /* bokeh_extensions/jstree.js */ function _(require, module, exports, __esModule, __esExport) {
+            "79591b3bf4": /* bokeh_extensions/jstree.js */ function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 var _a;
                 const dom_1 = require("@bokehjs/core/dom");
                 const layout_1 = require("bfe8e8c0eb") /* ./layout */ ;
 
                 function ID() {
                     // Math.random should be unique because of its seeding algorithm.
@@ -79,14 +79,15 @@
                     }
                     connect_signals() {
                         console.log("connect");
                         super.connect_signals();
                         this.connect(this.model.properties._data.change, () => this._update_tree_from_data());
                         this.connect(this.model.properties.value.change, () => this._update_selection_from_value());
                         this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());
+                        this.connect(this.model.properties.checkbox.change, () => this.setCheckboxes());
                         this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());
                         this.connect(this.model.properties.show_dots.change, () => this._setShowDots());
                         this.connect(this.model.properties.multiple.change, () => this._setMultiple());
                         console.log(this.model.show_dots);
                         console.log(this.model.show_icons);
                     }
                     render() {
@@ -96,14 +97,17 @@
                         this._container = (0, dom_1.div)({
                             id: this._id,
                             style: "overflow: auto; minHeight: 200px; minWidth: 200px;"
                         });
                         (0, layout_1.set_size)(this._container, this.model);
                         this.shadow_el.appendChild(this._container);
                         console.log(this._container);
+                        if (this.model.checkbox) {
+                            this.model.plugins.push("checkbox");
+                        }
                         let kw = {
                             "checkbox": {
                                 "three_state": false,
                                 "cascade": "undetermined"
                             }
                         };
                         this._jstree = jQuery(this._container).jstree(Object.assign({
@@ -118,23 +122,23 @@
                             },
                             "plugins": this.model.plugins
                         }, kw));
                         this.init_callbacks();
                     }
                     init_callbacks() {
                         // Initialization
-                        this._jstree.on('ready.jstree', ({}, {}) => this.onjsTreeInit());
                         // Rendering callbacks
                         // TODO: do I need both of these?
                         this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());
                         // Sync state with model
+                        this._jstree.on('model.jstree', ({}, {}) => this.onNewData());
                         this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));
                         this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));
                     }
-                    onjsTreeInit() {
+                    onNewData() {
                         this.model._flat_tree = this._jstree.jstree(true).get_json(null, {
                             "flat": true
                         });
                         console.log("flat tree: ", this.model._flat_tree);
                     }
                     selectNodeFromEditor({}, data) {
                         console.log("select pre", this.model.value);
@@ -149,19 +153,14 @@
                         // by comparing to last_selected
                         if (this.model.value != this._last_selected) {
                             let deselected = this._last_selected.filter(x => !this.model.value.includes(x));
                             this._jstree.jstree(true).deselect_node(deselected);
                         }
                         // We choose get_selected
                         this._last_selected = this.model.value;
-                        if (this.model.show_icons) {
-                            this._jstree.jstree(true).show_icons();
-                        } else {
-                            this._jstree.jstree(true).hide_icons();
-                        }
                     }
                     _update_tree_from_new_nodes() {
                         console.log("new nodes: ", this.model._new_nodes);
                         for (let node of this.model._new_nodes) {
                             this._jstree.jstree(true).create_node(node["parent"], node, "first");
                         }
                         this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, {
@@ -172,28 +171,30 @@
                         this.model._data = this._jstree.jstree(true).settings.core.data;
                         // this._update_selection_from_value()
                     }
                     _update_tree_from_data() {
                         console.log("updating data");
                         this._jstree.jstree(true).settings.core.data = this.model._data;
                         console.log("data: ", this._jstree.jstree(true).settings.core.data);
-                        this.model._flat_tree = this._jstree.jstree(true).get_json(null, {
-                            "flat": true
-                        });
-                        console.log("flat tree: ", this.model._flat_tree);
                         console.log("value after data", this.model.value);
                         // This will redraw the tree if we swap out the data with new data
                         // we set forget_state to true, so the current state is not reapplied
-                        // letting whatever state is set in the new data (open or closed, selected, etc)
+                        // letting whatever state is set in the new data (open or closed, etc)
                         // be the new state
                         this._jstree.jstree(true).refresh({
                             "skip_loading": false,
                             "forget_state": true
                         });
+                        // selected state is not preserved correctly right now, so we then
+                        // deselect everything because that is better than getting it wrong
+                        this._jstree.jstree(true).deselect_all({
+                            "supress_event": true
+                        });
                         console.log("value after refresh", this.model.value);
+                        console.log("data after refresh", this._jstree.jstree(true).settings.core.data);
                     }
                     _setShowIcons() {
                         console.log("setShowIcons");
                         if (this.model.show_icons) {
                             this._jstree.jstree(true).show_icons();
                         } else {
                             this._jstree.jstree(true).hide_icons();
@@ -203,14 +204,22 @@
                         console.log("setShowDots");
                         if (this.model.show_dots) {
                             this._jstree.jstree(true).show_dots();
                         } else {
                             this._jstree.jstree(true).hide_dots();
                         }
                     }
+                    setCheckboxes() {
+                        console.log("setCheckBoxes");
+                        if (this.model.checkbox) {
+                            this._jstree.jstree(true).show_checkboxes();
+                        } else {
+                            this._jstree.jstree(true).hide_checkboxes();
+                        }
+                    }
                     _setMultiple() {
                         console.log("setMultiple");
                         this._jstree.jstree(true).settings.core.multiple = this.model.multiple;
                     }
                     _update_tree_theme_from_model() {
                         this._jstree.jstree(true).refresh(false, true);
                     }
@@ -245,14 +254,15 @@
                         Array,
                         Any,
                         Boolean
                     }) => ({
                         value: [Array(Any), []],
                         _data: [Array(Any), []],
                         plugins: [Array(Any), []],
+                        checkbox: [Boolean, true],
                         multiple: [Boolean, true],
                         show_icons: [Boolean, true],
                         show_dots: [Boolean, true],
                         _last_opened: [Any, {}],
                         _new_nodes: [Array(Any), []],
                         _flat_tree: [Array(Any), []],
                     }));
@@ -397,12 +407,12 @@
                 }
                 exports.HTMLBox = HTMLBox;
                 HTMLBox.__name__ = "HTMLBox";
             },
         }, "ecf49f9c64", {
             "index": "ecf49f9c64",
             "bokeh_extensions/index": "ef403b5ad2",
-            "bokeh_extensions/jstree": "c52315dab1",
+            "bokeh_extensions/jstree": "79591b3bf4",
             "bokeh_extensions/layout": "bfe8e8c0eb"
         }, {});
 });
 //# sourceMappingURL=panel_jstree.js.map
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.js.map` & `panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.js.map`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.880952380952381%*

 * *Differences: {"'mappings'": "';;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAAA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,ACXA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,ACRA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AA […]*

```diff
@@ -1,19 +1,19 @@
 {
     "file": "generated.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAAA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,ACXA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,ACRA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,AChLA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA",
+    "mappings": ";;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AAAA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,ACXA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,ACRA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,AC1LA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "@@/src/panel_jstree/dist/lib/index.js",
         "@@/src/panel_jstree/dist/lib/bokeh_extensions/index.js",
         "@@/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js",
         "@@/src/panel_jstree/dist/lib/bokeh_extensions/layout.js"
     ],
     "sourcesContent": [
         "/* index.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const tslib_1 = require(\"tslib\");\n    // export {jsTreePlot} from \"./models/jstree\"\n    // import {register_models} from \"@bokehjs/base\"\n    // register_models(jsTreePlot as any)\n    const PaneljsTree = tslib_1.__importStar(require(\"ef403b5ad2\") /* ./bokeh_extensions/ */);\n    exports.PaneljsTree = PaneljsTree;\n    const base_1 = require(\"@bokehjs/base\");\n    (0, base_1.register_models)(PaneljsTree);\n}\n",
-        "/* bokeh_extensions/index.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const tslib_1 = require(\"tslib\");\n    const jsTree = tslib_1.__importStar(require(\"c52315dab1\") /* ./jstree */);\n    exports.jsTree = jsTree;\n    const base_1 = require(\"@bokehjs/base\");\n    (0, base_1.register_models)(jsTree);\n}\n",
-        "/* bokeh_extensions/jstree.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    var _a;\n    const dom_1 = require(\"@bokehjs/core/dom\");\n    const layout_1 = require(\"bfe8e8c0eb\") /* ./layout */;\n    function ID() {\n        // Math.random should be unique because of its seeding algorithm.\n        // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n        // after the decimal.\n        return '_' + Math.random().toString(36).substring(2, 11);\n    }\n    class jsTreePlotView extends layout_1.HTMLBoxView {\n        initialize() {\n            super.initialize();\n            this._last_selected = [];\n        }\n        connect_signals() {\n            console.log(\"connect\");\n            super.connect_signals();\n            this.connect(this.model.properties._data.change, () => this._update_tree_from_data());\n            this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n            this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n            this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n            this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n            this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n            console.log(this.model.show_dots);\n            console.log(this.model.show_icons);\n        }\n        render() {\n            super.render();\n            this._id = ID();\n            console.log(this._id);\n            this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n            (0, layout_1.set_size)(this._container, this.model);\n            this.shadow_el.appendChild(this._container);\n            console.log(this._container);\n            let kw = { \"checkbox\": {\n                    \"three_state\": false,\n                    \"cascade\": \"undetermined\"\n                } };\n            this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model._data, \"check_callback\": true,\n                    \"multiple\": this.model.multiple,\n                    \"themes\": {\n                        \"dots\": this.model.show_dots,\n                        \"icons\": this.model.show_icons\n                    }\n                }, \"plugins\": this.model.plugins }, kw));\n            this.init_callbacks();\n        }\n        init_callbacks() {\n            // Initialization\n            this._jstree.on('ready.jstree', ({}, {}) => this.onjsTreeInit());\n            // Rendering callbacks\n            // TODO: do I need both of these?\n            this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n            // Sync state with model\n            this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));\n            this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n        }\n        onjsTreeInit() {\n            this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n            console.log(\"flat tree: \", this.model._flat_tree);\n        }\n        selectNodeFromEditor({}, data) {\n            console.log(\"select pre\", this.model.value);\n            this.model.value = data.instance.get_selected();\n            console.log(\"select post\", this.model.value);\n        }\n        _update_selection_from_value() {\n            console.log(\"update selection from value\");\n            this._jstree.jstree(true).select_node(this.model.value);\n            // We sometimes have to fire this function more than once per value change because of\n            // calling jstree.refresh, so we check to see if model.value has really changed\n            // by comparing to last_selected\n            if (this.model.value != this._last_selected) {\n                let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n                this._jstree.jstree(true).deselect_node(deselected);\n            }\n            // We choose get_selected\n            this._last_selected = this.model.value;\n            if (this.model.show_icons) {\n                this._jstree.jstree(true).show_icons();\n            }\n            else {\n                this._jstree.jstree(true).hide_icons();\n            }\n        }\n        _update_tree_from_new_nodes() {\n            console.log(\"new nodes: \", this.model._new_nodes);\n            for (let node of this.model._new_nodes) {\n                this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n            }\n            this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n            this.model._data = this._jstree.jstree(true).settings.core.data;\n            // this._update_selection_from_value()\n        }\n        _update_tree_from_data() {\n            console.log(\"updating data\");\n            this._jstree.jstree(true).settings.core.data = this.model._data;\n            console.log(\"data: \", this._jstree.jstree(true).settings.core.data);\n            this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n            console.log(\"flat tree: \", this.model._flat_tree);\n            console.log(\"value after data\", this.model.value);\n            // This will redraw the tree if we swap out the data with new data\n            // we set forget_state to true, so the current state is not reapplied\n            // letting whatever state is set in the new data (open or closed, selected, etc)\n            // be the new state\n            this._jstree.jstree(true).refresh({ \"skip_loading\": false,\n                \"forget_state\": true });\n            console.log(\"value after refresh\", this.model.value);\n        }\n        _setShowIcons() {\n            console.log(\"setShowIcons\");\n            if (this.model.show_icons) {\n                this._jstree.jstree(true).show_icons();\n            }\n            else {\n                this._jstree.jstree(true).hide_icons();\n            }\n        }\n        _setShowDots() {\n            console.log(\"setShowDots\");\n            if (this.model.show_dots) {\n                this._jstree.jstree(true).show_dots();\n            }\n            else {\n                this._jstree.jstree(true).hide_dots();\n            }\n        }\n        _setMultiple() {\n            console.log(\"setMultiple\");\n            this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n        }\n        _update_tree_theme_from_model() {\n            this._jstree.jstree(true).refresh(false, true);\n        }\n        _listen_for_node_open({}, data) {\n            console.log(\"listen for node open\");\n            data.node = this.add_node_children(data.node);\n            this.model._last_opened = data.node;\n        }\n        add_node_children(node) {\n            console.log(\"add node children\");\n            node[\"children_nodes\"] = [];\n            for (let child of node.children) {\n                node.children_nodes.push(this._jstree.jstree(true).get_node(child));\n            }\n            return node;\n        }\n    }\n    exports.jsTreePlotView = jsTreePlotView;\n    jsTreePlotView.__name__ = \"jsTreePlotView\";\n    class jsTreePlot extends layout_1.HTMLBox {\n        constructor(attrs) {\n            super(attrs);\n        }\n    }\n    exports.jsTreePlot = jsTreePlot;\n    _a = jsTreePlot;\n    jsTreePlot.__name__ = \"jsTreePlot\";\n    jsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n    (() => {\n        _a.prototype.default_view = jsTreePlotView;\n        _a.define(({ Array, Any, Boolean }) => ({\n            value: [Array(Any), []],\n            _data: [Array(Any), []],\n            plugins: [Array(Any), []],\n            multiple: [Boolean, true],\n            show_icons: [Boolean, true],\n            show_dots: [Boolean, true],\n            _last_opened: [Any, {}],\n            _new_nodes: [Array(Any), []],\n            _flat_tree: [Array(Any), []],\n        }));\n    })();\n}\n",
+        "/* bokeh_extensions/index.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const tslib_1 = require(\"tslib\");\n    const jsTree = tslib_1.__importStar(require(\"79591b3bf4\") /* ./jstree */);\n    exports.jsTree = jsTree;\n    const base_1 = require(\"@bokehjs/base\");\n    (0, base_1.register_models)(jsTree);\n}\n",
+        "/* bokeh_extensions/jstree.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    var _a;\n    const dom_1 = require(\"@bokehjs/core/dom\");\n    const layout_1 = require(\"bfe8e8c0eb\") /* ./layout */;\n    function ID() {\n        // Math.random should be unique because of its seeding algorithm.\n        // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n        // after the decimal.\n        return '_' + Math.random().toString(36).substring(2, 11);\n    }\n    class jsTreePlotView extends layout_1.HTMLBoxView {\n        initialize() {\n            super.initialize();\n            this._last_selected = [];\n        }\n        connect_signals() {\n            console.log(\"connect\");\n            super.connect_signals();\n            this.connect(this.model.properties._data.change, () => this._update_tree_from_data());\n            this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n            this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n            this.connect(this.model.properties.checkbox.change, () => this.setCheckboxes());\n            this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n            this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n            this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n            console.log(this.model.show_dots);\n            console.log(this.model.show_icons);\n        }\n        render() {\n            super.render();\n            this._id = ID();\n            console.log(this._id);\n            this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n            (0, layout_1.set_size)(this._container, this.model);\n            this.shadow_el.appendChild(this._container);\n            console.log(this._container);\n            if (this.model.checkbox) {\n                this.model.plugins.push(\"checkbox\");\n            }\n            let kw = { \"checkbox\": {\n                    \"three_state\": false,\n                    \"cascade\": \"undetermined\"\n                } };\n            this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model._data, \"check_callback\": true,\n                    \"multiple\": this.model.multiple,\n                    \"themes\": {\n                        \"dots\": this.model.show_dots,\n                        \"icons\": this.model.show_icons\n                    }\n                }, \"plugins\": this.model.plugins }, kw));\n            this.init_callbacks();\n        }\n        init_callbacks() {\n            // Initialization\n            // Rendering callbacks\n            // TODO: do I need both of these?\n            this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n            // Sync state with model\n            this._jstree.on('model.jstree', ({}, {}) => this.onNewData());\n            this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));\n            this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n        }\n        onNewData() {\n            this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n            console.log(\"flat tree: \", this.model._flat_tree);\n        }\n        selectNodeFromEditor({}, data) {\n            console.log(\"select pre\", this.model.value);\n            this.model.value = data.instance.get_selected();\n            console.log(\"select post\", this.model.value);\n        }\n        _update_selection_from_value() {\n            console.log(\"update selection from value\");\n            this._jstree.jstree(true).select_node(this.model.value);\n            // We sometimes have to fire this function more than once per value change because of\n            // calling jstree.refresh, so we check to see if model.value has really changed\n            // by comparing to last_selected\n            if (this.model.value != this._last_selected) {\n                let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n                this._jstree.jstree(true).deselect_node(deselected);\n            }\n            // We choose get_selected\n            this._last_selected = this.model.value;\n        }\n        _update_tree_from_new_nodes() {\n            console.log(\"new nodes: \", this.model._new_nodes);\n            for (let node of this.model._new_nodes) {\n                this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n            }\n            this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n            this.model._data = this._jstree.jstree(true).settings.core.data;\n            // this._update_selection_from_value()\n        }\n        _update_tree_from_data() {\n            console.log(\"updating data\");\n            this._jstree.jstree(true).settings.core.data = this.model._data;\n            console.log(\"data: \", this._jstree.jstree(true).settings.core.data);\n            console.log(\"value after data\", this.model.value);\n            // This will redraw the tree if we swap out the data with new data\n            // we set forget_state to true, so the current state is not reapplied\n            // letting whatever state is set in the new data (open or closed, etc)\n            // be the new state\n            this._jstree.jstree(true).refresh({ \"skip_loading\": false,\n                \"forget_state\": true });\n            // selected state is not preserved correctly right now, so we then\n            // deselect everything because that is better than getting it wrong\n            this._jstree.jstree(true).deselect_all({ \"supress_event\": true });\n            console.log(\"value after refresh\", this.model.value);\n            console.log(\"data after refresh\", this._jstree.jstree(true).settings.core.data);\n        }\n        _setShowIcons() {\n            console.log(\"setShowIcons\");\n            if (this.model.show_icons) {\n                this._jstree.jstree(true).show_icons();\n            }\n            else {\n                this._jstree.jstree(true).hide_icons();\n            }\n        }\n        _setShowDots() {\n            console.log(\"setShowDots\");\n            if (this.model.show_dots) {\n                this._jstree.jstree(true).show_dots();\n            }\n            else {\n                this._jstree.jstree(true).hide_dots();\n            }\n        }\n        setCheckboxes() {\n            console.log(\"setCheckBoxes\");\n            if (this.model.checkbox) {\n                this._jstree.jstree(true).show_checkboxes();\n            }\n            else {\n                this._jstree.jstree(true).hide_checkboxes();\n            }\n        }\n        _setMultiple() {\n            console.log(\"setMultiple\");\n            this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n        }\n        _update_tree_theme_from_model() {\n            this._jstree.jstree(true).refresh(false, true);\n        }\n        _listen_for_node_open({}, data) {\n            console.log(\"listen for node open\");\n            data.node = this.add_node_children(data.node);\n            this.model._last_opened = data.node;\n        }\n        add_node_children(node) {\n            console.log(\"add node children\");\n            node[\"children_nodes\"] = [];\n            for (let child of node.children) {\n                node.children_nodes.push(this._jstree.jstree(true).get_node(child));\n            }\n            return node;\n        }\n    }\n    exports.jsTreePlotView = jsTreePlotView;\n    jsTreePlotView.__name__ = \"jsTreePlotView\";\n    class jsTreePlot extends layout_1.HTMLBox {\n        constructor(attrs) {\n            super(attrs);\n        }\n    }\n    exports.jsTreePlot = jsTreePlot;\n    _a = jsTreePlot;\n    jsTreePlot.__name__ = \"jsTreePlot\";\n    jsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n    (() => {\n        _a.prototype.default_view = jsTreePlotView;\n        _a.define(({ Array, Any, Boolean }) => ({\n            value: [Array(Any), []],\n            _data: [Array(Any), []],\n            plugins: [Array(Any), []],\n            checkbox: [Boolean, true],\n            multiple: [Boolean, true],\n            show_icons: [Boolean, true],\n            show_dots: [Boolean, true],\n            _last_opened: [Any, {}],\n            _new_nodes: [Array(Any), []],\n            _flat_tree: [Array(Any), []],\n        }));\n    })();\n}\n",
         "/* bokeh_extensions/layout.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const dom_1 = require(\"@bokehjs/core/dom\");\n    const types_1 = require(\"@bokehjs/core/util/types\");\n    const widget_1 = require(\"@bokehjs/models/widgets/widget\");\n    const layout_dom_1 = require(\"@bokehjs/models/layouts/layout_dom\");\n    class PanelMarkupView extends widget_1.WidgetView {\n        async lazy_initialize() {\n            await super.lazy_initialize();\n            if (this.provider.status == \"not_started\" || this.provider.status == \"loading\")\n                this.provider.ready.connect(() => {\n                    if (this.contains_tex_string(this.model.text))\n                        this.render();\n                });\n        }\n        connect_signals() {\n            super.connect_signals();\n            this.connect(this.model.change, () => {\n                this.render();\n            });\n        }\n        has_math_disabled() {\n            return this.model.disable_math || !this.contains_tex_string(this.model.text);\n        }\n        render() {\n            super.render();\n            set_size(this.el, this.model);\n            this.container = (0, dom_1.div)();\n            set_size(this.container, this.model, false);\n            this.shadow_el.appendChild(this.container);\n            if (this.provider.status == \"failed\" || this.provider.status == \"loaded\")\n                this._has_finished = true;\n        }\n    }\n    exports.PanelMarkupView = PanelMarkupView;\n    PanelMarkupView.__name__ = \"PanelMarkupView\";\n    function set_size(el, model, adjustMargin = true) {\n        let width_policy = model.width != null ? \"fixed\" : \"fit\";\n        let height_policy = model.height != null ? \"fixed\" : \"fit\";\n        const { sizing_mode, margin } = model;\n        if (sizing_mode != null) {\n            if (sizing_mode == \"fixed\")\n                width_policy = height_policy = \"fixed\";\n            else if (sizing_mode == \"stretch_both\")\n                width_policy = height_policy = \"max\";\n            else if (sizing_mode == \"stretch_width\")\n                width_policy = \"max\";\n            else if (sizing_mode == \"stretch_height\")\n                height_policy = \"max\";\n            else {\n                switch (sizing_mode) {\n                    case \"scale_width\":\n                        width_policy = \"max\";\n                        height_policy = \"min\";\n                        break;\n                    case \"scale_height\":\n                        width_policy = \"min\";\n                        height_policy = \"max\";\n                        break;\n                    case \"scale_both\":\n                        width_policy = \"max\";\n                        height_policy = \"max\";\n                        break;\n                    default:\n                        throw new Error(\"unreachable\");\n                }\n            }\n        }\n        let wm, hm;\n        if (!adjustMargin) {\n            hm = wm = 0;\n        }\n        else if ((0, types_1.isArray)(margin)) {\n            if (margin.length === 4) {\n                hm = margin[0] + margin[2];\n                wm = margin[1] + margin[3];\n            }\n            else {\n                hm = margin[0] * 2;\n                wm = margin[1] * 2;\n            }\n        }\n        else if (margin == null) {\n            hm = wm = 0;\n        }\n        else {\n            wm = hm = margin * 2;\n        }\n        if (width_policy == \"fixed\" && model.width)\n            el.style.width = model.width + \"px\";\n        else if (width_policy == \"max\")\n            el.style.width = wm ? `calc(100% - ${wm}px)` : \"100%\";\n        if (model.min_width != null)\n            el.style.minWidth = model.min_width + \"px\";\n        if (model.max_width != null)\n            el.style.maxWidth = model.max_width + \"px\";\n        if (height_policy == \"fixed\" && model.height)\n            el.style.height = model.height + \"px\";\n        else if (height_policy == \"max\")\n            el.style.height = hm ? `calc(100% - ${hm}px)` : \"100%\";\n        if (model.min_height != null)\n            el.style.minHeight = model.min_height + \"px\";\n        if (model.max_width != null)\n            el.style.maxHeight = model.max_height + \"px\";\n    }\n    exports.set_size = set_size;\n    class HTMLBoxView extends layout_dom_1.LayoutDOMView {\n        render() {\n            super.render();\n            set_size(this.el, this.model);\n        }\n        watch_stylesheets() {\n            this._initialized_stylesheets = {};\n            for (const sts of this._applied_stylesheets) {\n                const style_el = sts.el;\n                if (style_el instanceof HTMLLinkElement) {\n                    this._initialized_stylesheets[style_el.href] = false;\n                    style_el.addEventListener(\"load\", () => {\n                        this._initialized_stylesheets[style_el.href] = true;\n                        if (Object.values(this._initialized_stylesheets).every(Boolean))\n                            this.style_redraw();\n                    });\n                }\n            }\n        }\n        style_redraw() {\n        }\n        get child_models() {\n            return [];\n        }\n    }\n    exports.HTMLBoxView = HTMLBoxView;\n    HTMLBoxView.__name__ = \"HTMLBoxView\";\n    class HTMLBox extends layout_dom_1.LayoutDOM {\n        constructor(attrs) {\n            super(attrs);\n        }\n    }\n    exports.HTMLBox = HTMLBox;\n    HTMLBox.__name__ = \"HTMLBox\";\n}\n"
     ],
     "version": 3
 }
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.json` & `panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9853050595238095%*

 * *Differences: {"'artifacts'": "{1: {'code': {'source': '/* bokeh_extensions/index.js */ function _(require, "*

 * *                'module, exports, __esModule, __esExport) {\\n    __esModule();\\n    const '*

 * *                'tslib_1 = require("tslib");\\n    const jsTree = '*

 * *                'tslib_1.__importStar(require("79591b3bf4") /* ./jstree */);\\n    exports.jsTree '*

 * *                '= jsTree;\\n    const base_1 = require("@bokehjs/base");\\n    (0, '*

 * *                "base_1.register_models)(jsTree);\\n}\\n', 'min_sour […]*

```diff
@@ -27,16 +27,16 @@
                 "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.PaneljsTree = void 0;\nconst tslib_1 = require(\"tslib\");\n// export {jsTreePlot} from \"./models/jstree\"\n// import {register_models} from \"@bokehjs/base\"\n// register_models(jsTreePlot as any)\nconst PaneljsTree = tslib_1.__importStar(require(\"./bokeh_extensions/\"));\nexports.PaneljsTree = PaneljsTree;\nconst base_1 = require(\"@bokehjs/base\");\n(0, base_1.register_models)(PaneljsTree);\n//# sourceMappingURL=index.js.map\n",
                 "type": "js"
             }
         },
         {
             "code": {
                 "min_map": "{\"version\":3,\"file\":\"index.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"jsTree\",\"__importStar\",\"register_models\"],\"sources\":[\"0\"],\"mappings\":\"AAAgC,SAASA,EAAEC,EAASC,EAAQC,EAASC,EAAYC,GAC7ED,IACA,MACME,EADUL,EAAQ,SACDM,aAAaN,EAAQ,eAC5CE,EAAQG,OAASA,GAEjB,EADeL,EAAQ,iBACZO,iBAAiBF,EAChC\"}",
-                "min_source": "function _(e,s,t,o,r){o();const b=e(\"tslib\").__importStar(e(\"c52315dab1\"));t.jsTree=b;(0,e(\"@bokehjs/base\").register_models)(b)}\n//# sourceMappingURL=index.min.js.map",
-                "source": "/* bokeh_extensions/index.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const tslib_1 = require(\"tslib\");\n    const jsTree = tslib_1.__importStar(require(\"c52315dab1\") /* ./jstree */);\n    exports.jsTree = jsTree;\n    const base_1 = require(\"@bokehjs/base\");\n    (0, base_1.register_models)(jsTree);\n}\n"
+                "min_source": "function _(e,s,t,b,o){b();const r=e(\"tslib\").__importStar(e(\"79591b3bf4\"));t.jsTree=r;(0,e(\"@bokehjs/base\").register_models)(r)}\n//# sourceMappingURL=index.min.js.map",
+                "source": "/* bokeh_extensions/index.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const tslib_1 = require(\"tslib\");\n    const jsTree = tslib_1.__importStar(require(\"79591b3bf4\") /* ./jstree */);\n    exports.jsTree = jsTree;\n    const base_1 = require(\"@bokehjs/base\");\n    (0, base_1.register_models)(jsTree);\n}\n"
             },
             "module": {
                 "base": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib",
                 "base_path": "bokeh_extensions/index.js",
                 "canonical": "bokeh_extensions/index",
                 "dependency_map": [],
                 "dependency_paths": [
@@ -54,17 +54,17 @@
                 "shims": [],
                 "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.jsTree = void 0;\nconst tslib_1 = require(\"tslib\");\nconst jsTree = tslib_1.__importStar(require(\"./jstree\"));\nexports.jsTree = jsTree;\nconst base_1 = require(\"@bokehjs/base\");\n(0, base_1.register_models)(jsTree);\n//# sourceMappingURL=index.js.map\n",
                 "type": "js"
             }
         },
         {
             "code": {
-                "min_map": "{\"version\":3,\"file\":\"jstree.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"_a\",\"dom_1\",\"layout_1\",\"jsTreePlotView\",\"HTMLBoxView\",\"initialize\",\"super\",\"this\",\"_last_selected\",\"connect_signals\",\"console\",\"log\",\"connect\",\"model\",\"properties\",\"_data\",\"change\",\"_update_tree_from_data\",\"value\",\"_update_selection_from_value\",\"_new_nodes\",\"_update_tree_from_new_nodes\",\"show_icons\",\"_setShowIcons\",\"show_dots\",\"_setShowDots\",\"multiple\",\"_setMultiple\",\"render\",\"_id\",\"Math\",\"random\",\"toString\",\"substring\",\"_container\",\"div\",\"id\",\"style\",\"set_size\",\"shadow_el\",\"appendChild\",\"_jstree\",\"jQuery\",\"jstree\",\"Object\",\"assign\",\"core\",\"data\",\"check_callback\",\"themes\",\"dots\",\"icons\",\"plugins\",\"checkbox\",\"three_state\",\"cascade\",\"init_callbacks\",\"on\",\"onjsTreeInit\",\"selectNodeFromEditor\",\"e\",\"_listen_for_node_open\",\"_flat_tree\",\"get_json\",\"flat\",\"instance\",\"get_selected\",\"select_node\",\"deselected\",\"filter\",\"x\",\"includes\",\"deselect_node\",\"hide_icons\",\"node\",\"create_node\",\"settings\",\"no_li_attr\",\"no_a_attr\",\"no_data\",\"refresh\",\"skip_loading\",\"forget_state\",\"hide_dots\",\"_update_tree_theme_from_model\",\"add_node_children\",\"_last_opened\",\"child\",\"children\",\"children_nodes\",\"push\",\"get_node\",\"__name__\",\"jsTreePlot\",\"HTMLBox\",\"constructor\",\"attrs\",\"__module__\",\"prototype\",\"default_view\",\"define\",\"Array\",\"Any\",\"Boolean\"],\"sources\":[\"0\"],\"mappings\":\"AAAiC,SAASA,EAAEC,EAASC,EAAQC,EAASC,EAAYC,GAE9E,IAAIC,EADJF,IAEA,MAAMG,EAAQN,EAAQ,qBAChBO,EAAWP,EAAQ,cAOzB,MAAMQ,UAAuBD,EAASE,YAClCC,aACIC,MAAMD,aACNE,KAAKC,eAAiB,EAC1B,CACAC,kBACIC,QAAQC,IAAI,WACZL,MAAMG,kBACNF,KAAKK,QAAQL,KAAKM,MAAMC,WAAWC,MAAMC,QAAQ,IAAMT,KAAKU,2BAC5DV,KAAKK,QAAQL,KAAKM,MAAMC,WAAWI,MAAMF,QAAQ,IAAMT,KAAKY,iCAC5DZ,KAAKK,QAAQL,KAAKM,MAAMC,WAAWM,WAAWJ,QAAQ,IAAMT,KAAKc,gCACjEd,KAAKK,QAAQL,KAAKM,MAAMC,WAAWQ,WAAWN,QAAQ,IAAMT,KAAKgB,kBACjEhB,KAAKK,QAAQL,KAAKM,MAAMC,WAAWU,UAAUR,QAAQ,IAAMT,KAAKkB,iBAChElB,KAAKK,QAAQL,KAAKM,MAAMC,WAAWY,SAASV,QAAQ,IAAMT,KAAKoB,iBAC/DjB,QAAQC,IAAIJ,KAAKM,MAAMW,WACvBd,QAAQC,IAAIJ,KAAKM,MAAMS,WAC3B,CACAM,SACItB,MAAMsB,SACNrB,KAAKsB,IArBF,IAAMC,KAAKC,SAASC,SAAS,IAAIC,UAAU,EAAG,IAsBjDvB,QAAQC,IAAIJ,KAAKsB,KACjBtB,KAAK2B,YAAa,EAAIjC,EAAMkC,KAAK,CAAEC,GAAI7B,KAAKsB,IAAKQ,MAAO,wDACxD,EAAInC,EAASoC,UAAU/B,KAAK2B,WAAY3B,KAAKM,OAC7CN,KAAKgC,UAAUC,YAAYjC,KAAK2B,YAChCxB,QAAQC,IAAIJ,KAAK2B,YAKjB3B,KAAKkC,QAAUC,OAAOnC,KAAK2B,YAAYS,OAAOC,OAAOC,OAAO,CAAEC,KAAQ,CAAEC,KAAQxC,KAAKM,MAAME,MAAOiC,gBAAkB,EAC5GtB,SAAYnB,KAAKM,MAAMa,SACvBuB,OAAU,CACNC,KAAQ3C,KAAKM,MAAMW,UACnB2B,MAAS5C,KAAKM,MAAMS,aAEzB8B,QAAW7C,KAAKM,MAAMuC,SAVpB,CAAEC,SAAY,CACfC,aAAe,EACfC,QAAW,mBASnBhD,KAAKiD,gBACT,CACAA,iBAEIjD,KAAKkC,QAAQgB,GAAG,gBAAgB,SAAYlD,KAAKmD,iBAGjDnD,KAAKkC,QAAQgB,GAAG,kBAAkB,SAAYlD,KAAKY,iCAEnDZ,KAAKkC,QAAQgB,GAAG,wBAAwB,IAAKV,IAASxC,KAAKoD,qBAAqB,CAAC,EAAGZ,KACpFxC,KAAKkC,QAAQgB,GAAG,sBAAsB,CAACG,EAAGb,IAASxC,KAAKsD,sBAAsBD,EAAGb,IACrF,CACAW,eACInD,KAAKM,MAAMiD,WAAavD,KAAKkC,QAAQE,QAAO,GAAMoB,SAAS,KAAM,CAAEC,MAAQ,IAC3EtD,QAAQC,IAAI,cAAeJ,KAAKM,MAAMiD,WAC1C,CACAH,wBAAyBZ,GACrBrC,QAAQC,IAAI,aAAcJ,KAAKM,MAAMK,OACrCX,KAAKM,MAAMK,MAAQ6B,EAAKkB,SAASC,eACjCxD,QAAQC,IAAI,cAAeJ,KAAKM,MAAMK,MAC1C,CACAC,+BAMI,GALAT,QAAQC,IAAI,+BACZJ,KAAKkC,QAAQE,QAAO,GAAMwB,YAAY5D,KAAKM,MAAMK,OAI7CX,KAAKM,MAAMK,OAASX,KAAKC,eAAgB,CACzC,IAAI4D,EAAa7D,KAAKC,eAAe6D,QAAOC,IAAM/D,KAAKM,MAAMK,MAAMqD,SAASD,KAC5E/D,KAAKkC,QAAQE,QAAO,GAAM6B,cAAcJ,EAC5C,CAEA7D,KAAKC,eAAiBD,KAAKM,MAAMK,MAC7BX,KAAKM,MAAMS,WACXf,KAAKkC,QAAQE,QAAO,GAAMrB,aAG1Bf,KAAKkC,QAAQE,QAAO,GAAM8B,YAElC,CACApD,8BACIX,QAAQC,IAAI,cAAeJ,KAAKM,MAAMO,YACtC,IAAK,IAAIsD,KAAQnE,KAAKM,MAAMO,WACxBb,KAAKkC,QAAQE,QAAO,GAAMgC,YAAYD,EAAa,OAAGA,EAAM,SAEhEnE,KAAKkC,QAAQE,QAAO,GAAMiC,SAAS9B,KAAKC,KAAOxC,KAAKkC,QAAQE,QAAO,GAAMoB,SAAS,KAAM,CAAEc,YAAY,EAAMC,WAAW,EAAMC,SAAS,IACtIxE,KAAKM,MAAME,MAAQR,KAAKkC,QAAQE,QAAO,GAAMiC,SAAS9B,KAAKC,IAE/D,CACA9B,yBACIP,QAAQC,IAAI,iBACZJ,KAAKkC,QAAQE,QAAO,GAAMiC,SAAS9B,KAAKC,KAAOxC,KAAKM,MAAME,MAC1DL,QAAQC,IAAI,SAAUJ,KAAKkC,QAAQE,QAAO,GAAMiC,SAAS9B,KAAKC,MAC9DxC,KAAKM,MAAMiD,WAAavD,KAAKkC,QAAQE,QAAO,GAAMoB,SAAS,KAAM,CAAEC,MAAQ,IAC3EtD,QAAQC,IAAI,cAAeJ,KAAKM,MAAMiD,YACtCpD,QAAQC,IAAI,mBAAoBJ,KAAKM,MAAMK,OAK3CX,KAAKkC,QAAQE,QAAO,GAAMqC,QAAQ,CAAEC,cAAgB,EAChDC,cAAgB,IACpBxE,QAAQC,IAAI,sBAAuBJ,KAAKM,MAAMK,MAClD,CACAK,gBACIb,QAAQC,IAAI,gBACRJ,KAAKM,MAAMS,WACXf,KAAKkC,QAAQE,QAAO,GAAMrB,aAG1Bf,KAAKkC,QAAQE,QAAO,GAAM8B,YAElC,CACAhD,eACIf,QAAQC,IAAI,eACRJ,KAAKM,MAAMW,UACXjB,KAAKkC,QAAQE,QAAO,GAAMnB,YAG1BjB,KAAKkC,QAAQE,QAAO,GAAMwC,WAElC,CACAxD,eACIjB,QAAQC,IAAI,eACZJ,KAAKkC,QAAQE,QAAO,GAAMiC,SAAS9B,KAAKpB,SAAWnB,KAAKM,MAAMa,QAClE,CACA0D,gCACI7E,KAAKkC,QAAQE,QAAO,GAAMqC,SAAQ,GAAO,EAC7C,CACAnB,yBAA0Bd,GACtBrC,QAAQC,IAAI,wBACZoC,EAAK2B,KAAOnE,KAAK8E,kBAAkBtC,EAAK2B,MACxCnE,KAAKM,MAAMyE,aAAevC,EAAK2B,IACnC,CACAW,kBAAkBX,GACdhE,QAAQC,IAAI,qBACZ+D,EAAqB,eAAI,GACzB,IAAK,IAAIa,KAASb,EAAKc,SACnBd,EAAKe,eAAeC,KAAKnF,KAAKkC,QAAQE,QAAO,GAAMgD,SAASJ,IAEhE,OAAOb,CACX,EAEJ7E,EAAQM,eAAiBA,EACzBA,EAAeyF,SAAW,iBAC1B,MAAMC,UAAmB3F,EAAS4F,QAC9BC,YAAYC,GACR1F,MAAM0F,EACV,EAEJnG,EAAQgG,WAAaA,EACrB7F,EAAK6F,EACLA,EAAWD,SAAW,aACtBC,EAAWI,WAAa,uCAEpBjG,EAAGkG,UAAUC,aAAehG,EAC5BH,EAAGoG,QAAO,EAAGC,QAAOC,MAAKC,cAAc,CACnCrF,MAAO,CAACmF,EAAMC,GAAM,IACpBvF,MAAO,CAACsF,EAAMC,GAAM,IACpBlD,QAAS,CAACiD,EAAMC,GAAM,IACtB5E,SAAU,CAAC6E,GAAS,GACpBjF,WAAY,CAACiF,GAAS,GACtB/E,UAAW,CAAC+E,GAAS,GACrBjB,aAAc,CAACgB,EAAK,CAAC,GACrBlF,WAAY,CAACiF,EAAMC,GAAM,IACzBxC,WAAY,CAACuC,EAAMC,GAAM,OAGrC\"}",
-                "min_source": "function _(e,t,s,o,i){var l;o();const _=e(\"@bokehjs/core/dom\"),n=e(\"bfe8e8c0eb\");class r extends n.HTMLBoxView{initialize(){super.initialize(),this._last_selected=[]}connect_signals(){console.log(\"connect\"),super.connect_signals(),this.connect(this.model.properties._data.change,(()=>this._update_tree_from_data())),this.connect(this.model.properties.value.change,(()=>this._update_selection_from_value())),this.connect(this.model.properties._new_nodes.change,(()=>this._update_tree_from_new_nodes())),this.connect(this.model.properties.show_icons.change,(()=>this._setShowIcons())),this.connect(this.model.properties.show_dots.change,(()=>this._setShowDots())),this.connect(this.model.properties.multiple.change,(()=>this._setMultiple())),console.log(this.model.show_dots),console.log(this.model.show_icons)}render(){super.render(),this._id=\"_\"+Math.random().toString(36).substring(2,11),console.log(this._id),this._container=(0,_.div)({id:this._id,style:\"overflow: auto; minHeight: 200px; minWidth: 200px;\"}),(0,n.set_size)(this._container,this.model),this.shadow_el.appendChild(this._container),console.log(this._container);this._jstree=jQuery(this._container).jstree(Object.assign({core:{data:this.model._data,check_callback:!0,multiple:this.model.multiple,themes:{dots:this.model.show_dots,icons:this.model.show_icons}},plugins:this.model.plugins},{checkbox:{three_state:!1,cascade:\"undetermined\"}})),this.init_callbacks()}init_callbacks(){this._jstree.on(\"ready.jstree\",(({},{})=>this.onjsTreeInit())),this._jstree.on(\"refresh.jstree\",(({},{})=>this._update_selection_from_value())),this._jstree.on(\"activate_node.jstree\",(({},e)=>this.selectNodeFromEditor({},e))),this._jstree.on(\"before_open.jstree\",((e,t)=>this._listen_for_node_open(e,t)))}onjsTreeInit(){this.model._flat_tree=this._jstree.jstree(!0).get_json(null,{flat:!0}),console.log(\"flat tree: \",this.model._flat_tree)}selectNodeFromEditor({},e){console.log(\"select pre\",this.model.value),this.model.value=e.instance.get_selected(),console.log(\"select post\",this.model.value)}_update_selection_from_value(){if(console.log(\"update selection from value\"),this._jstree.jstree(!0).select_node(this.model.value),this.model.value!=this._last_selected){let e=this._last_selected.filter((e=>!this.model.value.includes(e)));this._jstree.jstree(!0).deselect_node(e)}this._last_selected=this.model.value,this.model.show_icons?this._jstree.jstree(!0).show_icons():this._jstree.jstree(!0).hide_icons()}_update_tree_from_new_nodes(){console.log(\"new nodes: \",this.model._new_nodes);for(let e of this.model._new_nodes)this._jstree.jstree(!0).create_node(e.parent,e,\"first\");this._jstree.jstree(!0).settings.core.data=this._jstree.jstree(!0).get_json(null,{no_li_attr:!0,no_a_attr:!0,no_data:!0}),this.model._data=this._jstree.jstree(!0).settings.core.data}_update_tree_from_data(){console.log(\"updating data\"),this._jstree.jstree(!0).settings.core.data=this.model._data,console.log(\"data: \",this._jstree.jstree(!0).settings.core.data),this.model._flat_tree=this._jstree.jstree(!0).get_json(null,{flat:!0}),console.log(\"flat tree: \",this.model._flat_tree),console.log(\"value after data\",this.model.value),this._jstree.jstree(!0).refresh({skip_loading:!1,forget_state:!0}),console.log(\"value after refresh\",this.model.value)}_setShowIcons(){console.log(\"setShowIcons\"),this.model.show_icons?this._jstree.jstree(!0).show_icons():this._jstree.jstree(!0).hide_icons()}_setShowDots(){console.log(\"setShowDots\"),this.model.show_dots?this._jstree.jstree(!0).show_dots():this._jstree.jstree(!0).hide_dots()}_setMultiple(){console.log(\"setMultiple\"),this._jstree.jstree(!0).settings.core.multiple=this.model.multiple}_update_tree_theme_from_model(){this._jstree.jstree(!0).refresh(!1,!0)}_listen_for_node_open({},e){console.log(\"listen for node open\"),e.node=this.add_node_children(e.node),this.model._last_opened=e.node}add_node_children(e){console.log(\"add node children\"),e.children_nodes=[];for(let t of e.children)e.children_nodes.push(this._jstree.jstree(!0).get_node(t));return e}}s.jsTreePlotView=r,r.__name__=\"jsTreePlotView\";class d extends n.HTMLBox{constructor(e){super(e)}}s.jsTreePlot=d,l=d,d.__name__=\"jsTreePlot\",d.__module__=\"panel_jstree.bokeh_extensions.jstree\",l.prototype.default_view=r,l.define((({Array:e,Any:t,Boolean:s})=>({value:[e(t),[]],_data:[e(t),[]],plugins:[e(t),[]],multiple:[s,!0],show_icons:[s,!0],show_dots:[s,!0],_last_opened:[t,{}],_new_nodes:[e(t),[]],_flat_tree:[e(t),[]]})))}\n//# sourceMappingURL=jstree.min.js.map",
-                "source": "/* bokeh_extensions/jstree.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    var _a;\n    const dom_1 = require(\"@bokehjs/core/dom\");\n    const layout_1 = require(\"bfe8e8c0eb\") /* ./layout */;\n    function ID() {\n        // Math.random should be unique because of its seeding algorithm.\n        // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n        // after the decimal.\n        return '_' + Math.random().toString(36).substring(2, 11);\n    }\n    class jsTreePlotView extends layout_1.HTMLBoxView {\n        initialize() {\n            super.initialize();\n            this._last_selected = [];\n        }\n        connect_signals() {\n            console.log(\"connect\");\n            super.connect_signals();\n            this.connect(this.model.properties._data.change, () => this._update_tree_from_data());\n            this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n            this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n            this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n            this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n            this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n            console.log(this.model.show_dots);\n            console.log(this.model.show_icons);\n        }\n        render() {\n            super.render();\n            this._id = ID();\n            console.log(this._id);\n            this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n            (0, layout_1.set_size)(this._container, this.model);\n            this.shadow_el.appendChild(this._container);\n            console.log(this._container);\n            let kw = { \"checkbox\": {\n                    \"three_state\": false,\n                    \"cascade\": \"undetermined\"\n                } };\n            this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model._data, \"check_callback\": true,\n                    \"multiple\": this.model.multiple,\n                    \"themes\": {\n                        \"dots\": this.model.show_dots,\n                        \"icons\": this.model.show_icons\n                    }\n                }, \"plugins\": this.model.plugins }, kw));\n            this.init_callbacks();\n        }\n        init_callbacks() {\n            // Initialization\n            this._jstree.on('ready.jstree', ({}, {}) => this.onjsTreeInit());\n            // Rendering callbacks\n            // TODO: do I need both of these?\n            this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n            // Sync state with model\n            this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));\n            this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n        }\n        onjsTreeInit() {\n            this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n            console.log(\"flat tree: \", this.model._flat_tree);\n        }\n        selectNodeFromEditor({}, data) {\n            console.log(\"select pre\", this.model.value);\n            this.model.value = data.instance.get_selected();\n            console.log(\"select post\", this.model.value);\n        }\n        _update_selection_from_value() {\n            console.log(\"update selection from value\");\n            this._jstree.jstree(true).select_node(this.model.value);\n            // We sometimes have to fire this function more than once per value change because of\n            // calling jstree.refresh, so we check to see if model.value has really changed\n            // by comparing to last_selected\n            if (this.model.value != this._last_selected) {\n                let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n                this._jstree.jstree(true).deselect_node(deselected);\n            }\n            // We choose get_selected\n            this._last_selected = this.model.value;\n            if (this.model.show_icons) {\n                this._jstree.jstree(true).show_icons();\n            }\n            else {\n                this._jstree.jstree(true).hide_icons();\n            }\n        }\n        _update_tree_from_new_nodes() {\n            console.log(\"new nodes: \", this.model._new_nodes);\n            for (let node of this.model._new_nodes) {\n                this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n            }\n            this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n            this.model._data = this._jstree.jstree(true).settings.core.data;\n            // this._update_selection_from_value()\n        }\n        _update_tree_from_data() {\n            console.log(\"updating data\");\n            this._jstree.jstree(true).settings.core.data = this.model._data;\n            console.log(\"data: \", this._jstree.jstree(true).settings.core.data);\n            this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n            console.log(\"flat tree: \", this.model._flat_tree);\n            console.log(\"value after data\", this.model.value);\n            // This will redraw the tree if we swap out the data with new data\n            // we set forget_state to true, so the current state is not reapplied\n            // letting whatever state is set in the new data (open or closed, selected, etc)\n            // be the new state\n            this._jstree.jstree(true).refresh({ \"skip_loading\": false,\n                \"forget_state\": true });\n            console.log(\"value after refresh\", this.model.value);\n        }\n        _setShowIcons() {\n            console.log(\"setShowIcons\");\n            if (this.model.show_icons) {\n                this._jstree.jstree(true).show_icons();\n            }\n            else {\n                this._jstree.jstree(true).hide_icons();\n            }\n        }\n        _setShowDots() {\n            console.log(\"setShowDots\");\n            if (this.model.show_dots) {\n                this._jstree.jstree(true).show_dots();\n            }\n            else {\n                this._jstree.jstree(true).hide_dots();\n            }\n        }\n        _setMultiple() {\n            console.log(\"setMultiple\");\n            this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n        }\n        _update_tree_theme_from_model() {\n            this._jstree.jstree(true).refresh(false, true);\n        }\n        _listen_for_node_open({}, data) {\n            console.log(\"listen for node open\");\n            data.node = this.add_node_children(data.node);\n            this.model._last_opened = data.node;\n        }\n        add_node_children(node) {\n            console.log(\"add node children\");\n            node[\"children_nodes\"] = [];\n            for (let child of node.children) {\n                node.children_nodes.push(this._jstree.jstree(true).get_node(child));\n            }\n            return node;\n        }\n    }\n    exports.jsTreePlotView = jsTreePlotView;\n    jsTreePlotView.__name__ = \"jsTreePlotView\";\n    class jsTreePlot extends layout_1.HTMLBox {\n        constructor(attrs) {\n            super(attrs);\n        }\n    }\n    exports.jsTreePlot = jsTreePlot;\n    _a = jsTreePlot;\n    jsTreePlot.__name__ = \"jsTreePlot\";\n    jsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n    (() => {\n        _a.prototype.default_view = jsTreePlotView;\n        _a.define(({ Array, Any, Boolean }) => ({\n            value: [Array(Any), []],\n            _data: [Array(Any), []],\n            plugins: [Array(Any), []],\n            multiple: [Boolean, true],\n            show_icons: [Boolean, true],\n            show_dots: [Boolean, true],\n            _last_opened: [Any, {}],\n            _new_nodes: [Array(Any), []],\n            _flat_tree: [Array(Any), []],\n        }));\n    })();\n}\n"
+                "min_map": "{\"version\":3,\"file\":\"jstree.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"_a\",\"dom_1\",\"layout_1\",\"jsTreePlotView\",\"HTMLBoxView\",\"initialize\",\"super\",\"this\",\"_last_selected\",\"connect_signals\",\"console\",\"log\",\"connect\",\"model\",\"properties\",\"_data\",\"change\",\"_update_tree_from_data\",\"value\",\"_update_selection_from_value\",\"_new_nodes\",\"_update_tree_from_new_nodes\",\"checkbox\",\"setCheckboxes\",\"show_icons\",\"_setShowIcons\",\"show_dots\",\"_setShowDots\",\"multiple\",\"_setMultiple\",\"render\",\"_id\",\"Math\",\"random\",\"toString\",\"substring\",\"_container\",\"div\",\"id\",\"style\",\"set_size\",\"shadow_el\",\"appendChild\",\"plugins\",\"push\",\"_jstree\",\"jQuery\",\"jstree\",\"Object\",\"assign\",\"core\",\"data\",\"check_callback\",\"themes\",\"dots\",\"icons\",\"three_state\",\"cascade\",\"init_callbacks\",\"on\",\"onNewData\",\"selectNodeFromEditor\",\"e\",\"_listen_for_node_open\",\"_flat_tree\",\"get_json\",\"flat\",\"instance\",\"get_selected\",\"select_node\",\"deselected\",\"filter\",\"x\",\"includes\",\"deselect_node\",\"node\",\"create_node\",\"settings\",\"no_li_attr\",\"no_a_attr\",\"no_data\",\"refresh\",\"skip_loading\",\"forget_state\",\"deselect_all\",\"supress_event\",\"hide_icons\",\"hide_dots\",\"show_checkboxes\",\"hide_checkboxes\",\"_update_tree_theme_from_model\",\"add_node_children\",\"_last_opened\",\"child\",\"children\",\"children_nodes\",\"get_node\",\"__name__\",\"jsTreePlot\",\"HTMLBox\",\"constructor\",\"attrs\",\"__module__\",\"prototype\",\"default_view\",\"define\",\"Array\",\"Any\",\"Boolean\"],\"sources\":[\"0\"],\"mappings\":\"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\"}",
+                "min_source": "function _(e,t,s,o,i){var l;o();const n=e(\"@bokehjs/core/dom\"),_=e(\"bfe8e8c0eb\");class r extends _.HTMLBoxView{initialize(){super.initialize(),this._last_selected=[]}connect_signals(){console.log(\"connect\"),super.connect_signals(),this.connect(this.model.properties._data.change,(()=>this._update_tree_from_data())),this.connect(this.model.properties.value.change,(()=>this._update_selection_from_value())),this.connect(this.model.properties._new_nodes.change,(()=>this._update_tree_from_new_nodes())),this.connect(this.model.properties.checkbox.change,(()=>this.setCheckboxes())),this.connect(this.model.properties.show_icons.change,(()=>this._setShowIcons())),this.connect(this.model.properties.show_dots.change,(()=>this._setShowDots())),this.connect(this.model.properties.multiple.change,(()=>this._setMultiple())),console.log(this.model.show_dots),console.log(this.model.show_icons)}render(){super.render(),this._id=\"_\"+Math.random().toString(36).substring(2,11),console.log(this._id),this._container=(0,n.div)({id:this._id,style:\"overflow: auto; minHeight: 200px; minWidth: 200px;\"}),(0,_.set_size)(this._container,this.model),this.shadow_el.appendChild(this._container),console.log(this._container),this.model.checkbox&&this.model.plugins.push(\"checkbox\");this._jstree=jQuery(this._container).jstree(Object.assign({core:{data:this.model._data,check_callback:!0,multiple:this.model.multiple,themes:{dots:this.model.show_dots,icons:this.model.show_icons}},plugins:this.model.plugins},{checkbox:{three_state:!1,cascade:\"undetermined\"}})),this.init_callbacks()}init_callbacks(){this._jstree.on(\"refresh.jstree\",(({},{})=>this._update_selection_from_value())),this._jstree.on(\"model.jstree\",(({},{})=>this.onNewData())),this._jstree.on(\"activate_node.jstree\",(({},e)=>this.selectNodeFromEditor({},e))),this._jstree.on(\"before_open.jstree\",((e,t)=>this._listen_for_node_open(e,t)))}onNewData(){this.model._flat_tree=this._jstree.jstree(!0).get_json(null,{flat:!0}),console.log(\"flat tree: \",this.model._flat_tree)}selectNodeFromEditor({},e){console.log(\"select pre\",this.model.value),this.model.value=e.instance.get_selected(),console.log(\"select post\",this.model.value)}_update_selection_from_value(){if(console.log(\"update selection from value\"),this._jstree.jstree(!0).select_node(this.model.value),this.model.value!=this._last_selected){let e=this._last_selected.filter((e=>!this.model.value.includes(e)));this._jstree.jstree(!0).deselect_node(e)}this._last_selected=this.model.value}_update_tree_from_new_nodes(){console.log(\"new nodes: \",this.model._new_nodes);for(let e of this.model._new_nodes)this._jstree.jstree(!0).create_node(e.parent,e,\"first\");this._jstree.jstree(!0).settings.core.data=this._jstree.jstree(!0).get_json(null,{no_li_attr:!0,no_a_attr:!0,no_data:!0}),this.model._data=this._jstree.jstree(!0).settings.core.data}_update_tree_from_data(){console.log(\"updating data\"),this._jstree.jstree(!0).settings.core.data=this.model._data,console.log(\"data: \",this._jstree.jstree(!0).settings.core.data),console.log(\"value after data\",this.model.value),this._jstree.jstree(!0).refresh({skip_loading:!1,forget_state:!0}),this._jstree.jstree(!0).deselect_all({supress_event:!0}),console.log(\"value after refresh\",this.model.value),console.log(\"data after refresh\",this._jstree.jstree(!0).settings.core.data)}_setShowIcons(){console.log(\"setShowIcons\"),this.model.show_icons?this._jstree.jstree(!0).show_icons():this._jstree.jstree(!0).hide_icons()}_setShowDots(){console.log(\"setShowDots\"),this.model.show_dots?this._jstree.jstree(!0).show_dots():this._jstree.jstree(!0).hide_dots()}setCheckboxes(){console.log(\"setCheckBoxes\"),this.model.checkbox?this._jstree.jstree(!0).show_checkboxes():this._jstree.jstree(!0).hide_checkboxes()}_setMultiple(){console.log(\"setMultiple\"),this._jstree.jstree(!0).settings.core.multiple=this.model.multiple}_update_tree_theme_from_model(){this._jstree.jstree(!0).refresh(!1,!0)}_listen_for_node_open({},e){console.log(\"listen for node open\"),e.node=this.add_node_children(e.node),this.model._last_opened=e.node}add_node_children(e){console.log(\"add node children\"),e.children_nodes=[];for(let t of e.children)e.children_nodes.push(this._jstree.jstree(!0).get_node(t));return e}}s.jsTreePlotView=r,r.__name__=\"jsTreePlotView\";class h extends _.HTMLBox{constructor(e){super(e)}}s.jsTreePlot=h,l=h,h.__name__=\"jsTreePlot\",h.__module__=\"panel_jstree.bokeh_extensions.jstree\",l.prototype.default_view=r,l.define((({Array:e,Any:t,Boolean:s})=>({value:[e(t),[]],_data:[e(t),[]],plugins:[e(t),[]],checkbox:[s,!0],multiple:[s,!0],show_icons:[s,!0],show_dots:[s,!0],_last_opened:[t,{}],_new_nodes:[e(t),[]],_flat_tree:[e(t),[]]})))}\n//# sourceMappingURL=jstree.min.js.map",
+                "source": "/* bokeh_extensions/jstree.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    var _a;\n    const dom_1 = require(\"@bokehjs/core/dom\");\n    const layout_1 = require(\"bfe8e8c0eb\") /* ./layout */;\n    function ID() {\n        // Math.random should be unique because of its seeding algorithm.\n        // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n        // after the decimal.\n        return '_' + Math.random().toString(36).substring(2, 11);\n    }\n    class jsTreePlotView extends layout_1.HTMLBoxView {\n        initialize() {\n            super.initialize();\n            this._last_selected = [];\n        }\n        connect_signals() {\n            console.log(\"connect\");\n            super.connect_signals();\n            this.connect(this.model.properties._data.change, () => this._update_tree_from_data());\n            this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n            this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n            this.connect(this.model.properties.checkbox.change, () => this.setCheckboxes());\n            this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n            this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n            this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n            console.log(this.model.show_dots);\n            console.log(this.model.show_icons);\n        }\n        render() {\n            super.render();\n            this._id = ID();\n            console.log(this._id);\n            this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n            (0, layout_1.set_size)(this._container, this.model);\n            this.shadow_el.appendChild(this._container);\n            console.log(this._container);\n            if (this.model.checkbox) {\n                this.model.plugins.push(\"checkbox\");\n            }\n            let kw = { \"checkbox\": {\n                    \"three_state\": false,\n                    \"cascade\": \"undetermined\"\n                } };\n            this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model._data, \"check_callback\": true,\n                    \"multiple\": this.model.multiple,\n                    \"themes\": {\n                        \"dots\": this.model.show_dots,\n                        \"icons\": this.model.show_icons\n                    }\n                }, \"plugins\": this.model.plugins }, kw));\n            this.init_callbacks();\n        }\n        init_callbacks() {\n            // Initialization\n            // Rendering callbacks\n            // TODO: do I need both of these?\n            this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n            // Sync state with model\n            this._jstree.on('model.jstree', ({}, {}) => this.onNewData());\n            this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));\n            this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n        }\n        onNewData() {\n            this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n            console.log(\"flat tree: \", this.model._flat_tree);\n        }\n        selectNodeFromEditor({}, data) {\n            console.log(\"select pre\", this.model.value);\n            this.model.value = data.instance.get_selected();\n            console.log(\"select post\", this.model.value);\n        }\n        _update_selection_from_value() {\n            console.log(\"update selection from value\");\n            this._jstree.jstree(true).select_node(this.model.value);\n            // We sometimes have to fire this function more than once per value change because of\n            // calling jstree.refresh, so we check to see if model.value has really changed\n            // by comparing to last_selected\n            if (this.model.value != this._last_selected) {\n                let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n                this._jstree.jstree(true).deselect_node(deselected);\n            }\n            // We choose get_selected\n            this._last_selected = this.model.value;\n        }\n        _update_tree_from_new_nodes() {\n            console.log(\"new nodes: \", this.model._new_nodes);\n            for (let node of this.model._new_nodes) {\n                this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n            }\n            this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n            this.model._data = this._jstree.jstree(true).settings.core.data;\n            // this._update_selection_from_value()\n        }\n        _update_tree_from_data() {\n            console.log(\"updating data\");\n            this._jstree.jstree(true).settings.core.data = this.model._data;\n            console.log(\"data: \", this._jstree.jstree(true).settings.core.data);\n            console.log(\"value after data\", this.model.value);\n            // This will redraw the tree if we swap out the data with new data\n            // we set forget_state to true, so the current state is not reapplied\n            // letting whatever state is set in the new data (open or closed, etc)\n            // be the new state\n            this._jstree.jstree(true).refresh({ \"skip_loading\": false,\n                \"forget_state\": true });\n            // selected state is not preserved correctly right now, so we then\n            // deselect everything because that is better than getting it wrong\n            this._jstree.jstree(true).deselect_all({ \"supress_event\": true });\n            console.log(\"value after refresh\", this.model.value);\n            console.log(\"data after refresh\", this._jstree.jstree(true).settings.core.data);\n        }\n        _setShowIcons() {\n            console.log(\"setShowIcons\");\n            if (this.model.show_icons) {\n                this._jstree.jstree(true).show_icons();\n            }\n            else {\n                this._jstree.jstree(true).hide_icons();\n            }\n        }\n        _setShowDots() {\n            console.log(\"setShowDots\");\n            if (this.model.show_dots) {\n                this._jstree.jstree(true).show_dots();\n            }\n            else {\n                this._jstree.jstree(true).hide_dots();\n            }\n        }\n        setCheckboxes() {\n            console.log(\"setCheckBoxes\");\n            if (this.model.checkbox) {\n                this._jstree.jstree(true).show_checkboxes();\n            }\n            else {\n                this._jstree.jstree(true).hide_checkboxes();\n            }\n        }\n        _setMultiple() {\n            console.log(\"setMultiple\");\n            this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n        }\n        _update_tree_theme_from_model() {\n            this._jstree.jstree(true).refresh(false, true);\n        }\n        _listen_for_node_open({}, data) {\n            console.log(\"listen for node open\");\n            data.node = this.add_node_children(data.node);\n            this.model._last_opened = data.node;\n        }\n        add_node_children(node) {\n            console.log(\"add node children\");\n            node[\"children_nodes\"] = [];\n            for (let child of node.children) {\n                node.children_nodes.push(this._jstree.jstree(true).get_node(child));\n            }\n            return node;\n        }\n    }\n    exports.jsTreePlotView = jsTreePlotView;\n    jsTreePlotView.__name__ = \"jsTreePlotView\";\n    class jsTreePlot extends layout_1.HTMLBox {\n        constructor(attrs) {\n            super(attrs);\n        }\n    }\n    exports.jsTreePlot = jsTreePlot;\n    _a = jsTreePlot;\n    jsTreePlot.__name__ = \"jsTreePlot\";\n    jsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n    (() => {\n        _a.prototype.default_view = jsTreePlotView;\n        _a.define(({ Array, Any, Boolean }) => ({\n            value: [Array(Any), []],\n            _data: [Array(Any), []],\n            plugins: [Array(Any), []],\n            checkbox: [Boolean, true],\n            multiple: [Boolean, true],\n            show_icons: [Boolean, true],\n            show_dots: [Boolean, true],\n            _last_opened: [Any, {}],\n            _new_nodes: [Array(Any), []],\n            _flat_tree: [Array(Any), []],\n        }));\n    })();\n}\n"
             },
             "module": {
                 "base": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib",
                 "base_path": "bokeh_extensions/jstree.js",
                 "canonical": "bokeh_extensions/jstree",
                 "dependency_map": [],
                 "dependency_paths": [
@@ -81,19 +81,19 @@
                     {
                         "name": "jsTreePlot",
                         "type": "named"
                     }
                 ],
                 "externals": [],
                 "file": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js",
-                "hash": "c52315dab1f322533fa9817c8a365780552ed380d328b8809aec08ea11594a0a",
-                "id": "c52315dab1",
+                "hash": "79591b3bf4bcba7298a6323f4ca42098dff07ba66ee9f3a0db8738e72e7ce6e8",
+                "id": "79591b3bf4",
                 "resolution": "ESM",
                 "shims": [],
-                "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.jsTreePlot = exports.jsTreePlotView = void 0;\nvar _a;\nconst dom_1 = require(\"@bokehjs/core/dom\");\nconst layout_1 = require(\"./layout\");\nfunction ID() {\n    // Math.random should be unique because of its seeding algorithm.\n    // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n    // after the decimal.\n    return '_' + Math.random().toString(36).substring(2, 11);\n}\nclass jsTreePlotView extends layout_1.HTMLBoxView {\n    initialize() {\n        super.initialize();\n        this._last_selected = [];\n    }\n    connect_signals() {\n        console.log(\"connect\");\n        super.connect_signals();\n        this.connect(this.model.properties._data.change, () => this._update_tree_from_data());\n        this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n        this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n        this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n        this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n        this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n        console.log(this.model.show_dots);\n        console.log(this.model.show_icons);\n    }\n    render() {\n        super.render();\n        this._id = ID();\n        console.log(this._id);\n        this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n        (0, layout_1.set_size)(this._container, this.model);\n        this.shadow_el.appendChild(this._container);\n        console.log(this._container);\n        let kw = { \"checkbox\": {\n                \"three_state\": false,\n                \"cascade\": \"undetermined\"\n            } };\n        this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model._data, \"check_callback\": true,\n                \"multiple\": this.model.multiple,\n                \"themes\": {\n                    \"dots\": this.model.show_dots,\n                    \"icons\": this.model.show_icons\n                }\n            }, \"plugins\": this.model.plugins }, kw));\n        this.init_callbacks();\n    }\n    init_callbacks() {\n        // Initialization\n        this._jstree.on('ready.jstree', ({}, {}) => this.onjsTreeInit());\n        // Rendering callbacks\n        // TODO: do I need both of these?\n        this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n        // Sync state with model\n        this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));\n        this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n    }\n    onjsTreeInit() {\n        this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n        console.log(\"flat tree: \", this.model._flat_tree);\n    }\n    selectNodeFromEditor({}, data) {\n        console.log(\"select pre\", this.model.value);\n        this.model.value = data.instance.get_selected();\n        console.log(\"select post\", this.model.value);\n    }\n    _update_selection_from_value() {\n        console.log(\"update selection from value\");\n        this._jstree.jstree(true).select_node(this.model.value);\n        // We sometimes have to fire this function more than once per value change because of\n        // calling jstree.refresh, so we check to see if model.value has really changed\n        // by comparing to last_selected\n        if (this.model.value != this._last_selected) {\n            let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n            this._jstree.jstree(true).deselect_node(deselected);\n        }\n        // We choose get_selected\n        this._last_selected = this.model.value;\n        if (this.model.show_icons) {\n            this._jstree.jstree(true).show_icons();\n        }\n        else {\n            this._jstree.jstree(true).hide_icons();\n        }\n    }\n    _update_tree_from_new_nodes() {\n        console.log(\"new nodes: \", this.model._new_nodes);\n        for (let node of this.model._new_nodes) {\n            this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n        }\n        this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n        this.model._data = this._jstree.jstree(true).settings.core.data;\n        // this._update_selection_from_value()\n    }\n    _update_tree_from_data() {\n        console.log(\"updating data\");\n        this._jstree.jstree(true).settings.core.data = this.model._data;\n        console.log(\"data: \", this._jstree.jstree(true).settings.core.data);\n        this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n        console.log(\"flat tree: \", this.model._flat_tree);\n        console.log(\"value after data\", this.model.value);\n        // This will redraw the tree if we swap out the data with new data\n        // we set forget_state to true, so the current state is not reapplied\n        // letting whatever state is set in the new data (open or closed, selected, etc)\n        // be the new state\n        this._jstree.jstree(true).refresh({ \"skip_loading\": false,\n            \"forget_state\": true });\n        console.log(\"value after refresh\", this.model.value);\n    }\n    _setShowIcons() {\n        console.log(\"setShowIcons\");\n        if (this.model.show_icons) {\n            this._jstree.jstree(true).show_icons();\n        }\n        else {\n            this._jstree.jstree(true).hide_icons();\n        }\n    }\n    _setShowDots() {\n        console.log(\"setShowDots\");\n        if (this.model.show_dots) {\n            this._jstree.jstree(true).show_dots();\n        }\n        else {\n            this._jstree.jstree(true).hide_dots();\n        }\n    }\n    _setMultiple() {\n        console.log(\"setMultiple\");\n        this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n    }\n    _update_tree_theme_from_model() {\n        this._jstree.jstree(true).refresh(false, true);\n    }\n    _listen_for_node_open({}, data) {\n        console.log(\"listen for node open\");\n        data.node = this.add_node_children(data.node);\n        this.model._last_opened = data.node;\n    }\n    add_node_children(node) {\n        console.log(\"add node children\");\n        node[\"children_nodes\"] = [];\n        for (let child of node.children) {\n            node.children_nodes.push(this._jstree.jstree(true).get_node(child));\n        }\n        return node;\n    }\n}\nexports.jsTreePlotView = jsTreePlotView;\njsTreePlotView.__name__ = \"jsTreePlotView\";\nclass jsTreePlot extends layout_1.HTMLBox {\n    constructor(attrs) {\n        super(attrs);\n    }\n}\nexports.jsTreePlot = jsTreePlot;\n_a = jsTreePlot;\njsTreePlot.__name__ = \"jsTreePlot\";\njsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n(() => {\n    _a.prototype.default_view = jsTreePlotView;\n    _a.define(({ Array, Any, Boolean }) => ({\n        value: [Array(Any), []],\n        _data: [Array(Any), []],\n        plugins: [Array(Any), []],\n        multiple: [Boolean, true],\n        show_icons: [Boolean, true],\n        show_dots: [Boolean, true],\n        _last_opened: [Any, {}],\n        _new_nodes: [Array(Any), []],\n        _flat_tree: [Array(Any), []],\n    }));\n})();\n//# sourceMappingURL=jstree.js.map\n",
+                "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.jsTreePlot = exports.jsTreePlotView = void 0;\nvar _a;\nconst dom_1 = require(\"@bokehjs/core/dom\");\nconst layout_1 = require(\"./layout\");\nfunction ID() {\n    // Math.random should be unique because of its seeding algorithm.\n    // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n    // after the decimal.\n    return '_' + Math.random().toString(36).substring(2, 11);\n}\nclass jsTreePlotView extends layout_1.HTMLBoxView {\n    initialize() {\n        super.initialize();\n        this._last_selected = [];\n    }\n    connect_signals() {\n        console.log(\"connect\");\n        super.connect_signals();\n        this.connect(this.model.properties._data.change, () => this._update_tree_from_data());\n        this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n        this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n        this.connect(this.model.properties.checkbox.change, () => this.setCheckboxes());\n        this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n        this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n        this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n        console.log(this.model.show_dots);\n        console.log(this.model.show_icons);\n    }\n    render() {\n        super.render();\n        this._id = ID();\n        console.log(this._id);\n        this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n        (0, layout_1.set_size)(this._container, this.model);\n        this.shadow_el.appendChild(this._container);\n        console.log(this._container);\n        if (this.model.checkbox) {\n            this.model.plugins.push(\"checkbox\");\n        }\n        let kw = { \"checkbox\": {\n                \"three_state\": false,\n                \"cascade\": \"undetermined\"\n            } };\n        this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model._data, \"check_callback\": true,\n                \"multiple\": this.model.multiple,\n                \"themes\": {\n                    \"dots\": this.model.show_dots,\n                    \"icons\": this.model.show_icons\n                }\n            }, \"plugins\": this.model.plugins }, kw));\n        this.init_callbacks();\n    }\n    init_callbacks() {\n        // Initialization\n        // Rendering callbacks\n        // TODO: do I need both of these?\n        this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n        // Sync state with model\n        this._jstree.on('model.jstree', ({}, {}) => this.onNewData());\n        this._jstree.on('activate_node.jstree', ({}, data) => this.selectNodeFromEditor({}, data));\n        this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n    }\n    onNewData() {\n        this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n        console.log(\"flat tree: \", this.model._flat_tree);\n    }\n    selectNodeFromEditor({}, data) {\n        console.log(\"select pre\", this.model.value);\n        this.model.value = data.instance.get_selected();\n        console.log(\"select post\", this.model.value);\n    }\n    _update_selection_from_value() {\n        console.log(\"update selection from value\");\n        this._jstree.jstree(true).select_node(this.model.value);\n        // We sometimes have to fire this function more than once per value change because of\n        // calling jstree.refresh, so we check to see if model.value has really changed\n        // by comparing to last_selected\n        if (this.model.value != this._last_selected) {\n            let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n            this._jstree.jstree(true).deselect_node(deselected);\n        }\n        // We choose get_selected\n        this._last_selected = this.model.value;\n    }\n    _update_tree_from_new_nodes() {\n        console.log(\"new nodes: \", this.model._new_nodes);\n        for (let node of this.model._new_nodes) {\n            this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n        }\n        this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n        this.model._data = this._jstree.jstree(true).settings.core.data;\n        // this._update_selection_from_value()\n    }\n    _update_tree_from_data() {\n        console.log(\"updating data\");\n        this._jstree.jstree(true).settings.core.data = this.model._data;\n        console.log(\"data: \", this._jstree.jstree(true).settings.core.data);\n        console.log(\"value after data\", this.model.value);\n        // This will redraw the tree if we swap out the data with new data\n        // we set forget_state to true, so the current state is not reapplied\n        // letting whatever state is set in the new data (open or closed, etc)\n        // be the new state\n        this._jstree.jstree(true).refresh({ \"skip_loading\": false,\n            \"forget_state\": true });\n        // selected state is not preserved correctly right now, so we then\n        // deselect everything because that is better than getting it wrong\n        this._jstree.jstree(true).deselect_all({ \"supress_event\": true });\n        console.log(\"value after refresh\", this.model.value);\n        console.log(\"data after refresh\", this._jstree.jstree(true).settings.core.data);\n    }\n    _setShowIcons() {\n        console.log(\"setShowIcons\");\n        if (this.model.show_icons) {\n            this._jstree.jstree(true).show_icons();\n        }\n        else {\n            this._jstree.jstree(true).hide_icons();\n        }\n    }\n    _setShowDots() {\n        console.log(\"setShowDots\");\n        if (this.model.show_dots) {\n            this._jstree.jstree(true).show_dots();\n        }\n        else {\n            this._jstree.jstree(true).hide_dots();\n        }\n    }\n    setCheckboxes() {\n        console.log(\"setCheckBoxes\");\n        if (this.model.checkbox) {\n            this._jstree.jstree(true).show_checkboxes();\n        }\n        else {\n            this._jstree.jstree(true).hide_checkboxes();\n        }\n    }\n    _setMultiple() {\n        console.log(\"setMultiple\");\n        this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n    }\n    _update_tree_theme_from_model() {\n        this._jstree.jstree(true).refresh(false, true);\n    }\n    _listen_for_node_open({}, data) {\n        console.log(\"listen for node open\");\n        data.node = this.add_node_children(data.node);\n        this.model._last_opened = data.node;\n    }\n    add_node_children(node) {\n        console.log(\"add node children\");\n        node[\"children_nodes\"] = [];\n        for (let child of node.children) {\n            node.children_nodes.push(this._jstree.jstree(true).get_node(child));\n        }\n        return node;\n    }\n}\nexports.jsTreePlotView = jsTreePlotView;\njsTreePlotView.__name__ = \"jsTreePlotView\";\nclass jsTreePlot extends layout_1.HTMLBox {\n    constructor(attrs) {\n        super(attrs);\n    }\n}\nexports.jsTreePlot = jsTreePlot;\n_a = jsTreePlot;\njsTreePlot.__name__ = \"jsTreePlot\";\njsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n(() => {\n    _a.prototype.default_view = jsTreePlotView;\n    _a.define(({ Array, Any, Boolean }) => ({\n        value: [Array(Any), []],\n        _data: [Array(Any), []],\n        plugins: [Array(Any), []],\n        checkbox: [Boolean, true],\n        multiple: [Boolean, true],\n        show_icons: [Boolean, true],\n        show_dots: [Boolean, true],\n        _last_opened: [Any, {}],\n        _new_nodes: [Array(Any), []],\n        _flat_tree: [Array(Any), []],\n    }));\n})();\n//# sourceMappingURL=jstree.js.map\n",
                 "type": "js"
             }
         },
         {
             "code": {
                 "min_map": "{\"version\":3,\"file\":\"layout.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"dom_1\",\"types_1\",\"widget_1\",\"layout_dom_1\",\"PanelMarkupView\",\"WidgetView\",\"async\",\"super\",\"lazy_initialize\",\"this\",\"provider\",\"status\",\"ready\",\"connect\",\"contains_tex_string\",\"model\",\"text\",\"render\",\"connect_signals\",\"change\",\"has_math_disabled\",\"disable_math\",\"set_size\",\"el\",\"container\",\"div\",\"shadow_el\",\"appendChild\",\"_has_finished\",\"adjustMargin\",\"width_policy\",\"width\",\"height_policy\",\"height\",\"sizing_mode\",\"margin\",\"Error\",\"wm\",\"hm\",\"isArray\",\"length\",\"style\",\"min_width\",\"minWidth\",\"max_width\",\"maxWidth\",\"min_height\",\"minHeight\",\"maxHeight\",\"max_height\",\"__name__\",\"HTMLBoxView\",\"LayoutDOMView\",\"watch_stylesheets\",\"_initialized_stylesheets\",\"sts\",\"_applied_stylesheets\",\"style_el\",\"HTMLLinkElement\",\"href\",\"addEventListener\",\"Object\",\"values\",\"every\",\"Boolean\",\"style_redraw\",\"child_models\",\"HTMLBox\",\"LayoutDOM\",\"constructor\",\"attrs\"],\"sources\":[\"0\"],\"mappings\":\"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\"}",
                 "min_source": "function _(e,t,i,s,h){s();const a=e(\"@bokehjs/core/dom\"),l=e(\"@bokehjs/core/util/types\"),n=e(\"@bokehjs/models/widgets/widget\"),d=e(\"@bokehjs/models/layouts/layout_dom\");class r extends n.WidgetView{async lazy_initialize(){await super.lazy_initialize(),\"not_started\"!=this.provider.status&&\"loading\"!=this.provider.status||this.provider.ready.connect((()=>{this.contains_tex_string(this.model.text)&&this.render()}))}connect_signals(){super.connect_signals(),this.connect(this.model.change,(()=>{this.render()}))}has_math_disabled(){return this.model.disable_math||!this.contains_tex_string(this.model.text)}render(){super.render(),o(this.el,this.model),this.container=(0,a.div)(),o(this.container,this.model,!1),this.shadow_el.appendChild(this.container),\"failed\"!=this.provider.status&&\"loaded\"!=this.provider.status||(this._has_finished=!0)}}function o(e,t,i=!0){let s=null!=t.width?\"fixed\":\"fit\",h=null!=t.height?\"fixed\":\"fit\";const{sizing_mode:a,margin:n}=t;if(null!=a)if(\"fixed\"==a)s=h=\"fixed\";else if(\"stretch_both\"==a)s=h=\"max\";else if(\"stretch_width\"==a)s=\"max\";else if(\"stretch_height\"==a)h=\"max\";else switch(a){case\"scale_width\":s=\"max\",h=\"min\";break;case\"scale_height\":s=\"min\",h=\"max\";break;case\"scale_both\":s=\"max\",h=\"max\";break;default:throw new Error(\"unreachable\")}let d,r;i?(0,l.isArray)(n)?4===n.length?(r=n[0]+n[2],d=n[1]+n[3]):(r=2*n[0],d=2*n[1]):null==n?r=d=0:d=r=2*n:r=d=0,\"fixed\"==s&&t.width?e.style.width=t.width+\"px\":\"max\"==s&&(e.style.width=d?`calc(100% - ${d}px)`:\"100%\"),null!=t.min_width&&(e.style.minWidth=t.min_width+\"px\"),null!=t.max_width&&(e.style.maxWidth=t.max_width+\"px\"),\"fixed\"==h&&t.height?e.style.height=t.height+\"px\":\"max\"==h&&(e.style.height=r?`calc(100% - ${r}px)`:\"100%\"),null!=t.min_height&&(e.style.minHeight=t.min_height+\"px\"),null!=t.max_width&&(e.style.maxHeight=t.max_height+\"px\")}i.PanelMarkupView=r,r.__name__=\"PanelMarkupView\",i.set_size=o;class _ extends d.LayoutDOMView{render(){super.render(),o(this.el,this.model)}watch_stylesheets(){this._initialized_stylesheets={};for(const e of this._applied_stylesheets){const t=e.el;t instanceof HTMLLinkElement&&(this._initialized_stylesheets[t.href]=!1,t.addEventListener(\"load\",(()=>{this._initialized_stylesheets[t.href]=!0,Object.values(this._initialized_stylesheets).every(Boolean)&&this.style_redraw()})))}}style_redraw(){}get child_models(){return[]}}i.HTMLBoxView=_,_.__name__=\"HTMLBoxView\";class c extends d.LayoutDOM{constructor(e){super(e)}}i.HTMLBox=c,c.__name__=\"HTMLBox\"}\n//# sourceMappingURL=layout.min.js.map",
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/dist/panel_jstree.min.js` & `panel-jstree-0.3.0/src/panel_jstree/dist/panel_jstree.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -43,37 +43,37 @@
         ({
             "ecf49f9c64": function _(e, s, t, o, r) {
                 o();
                 const a = e("tslib").__importStar(e("ef403b5ad2"));
                 t.PaneljsTree = a;
                 (0, e("@bokehjs/base").register_models)(a)
             },
-            "ef403b5ad2": function _(e, s, t, o, r) {
-                o();
-                const b = e("tslib").__importStar(e("c52315dab1"));
-                t.jsTree = b;
-                (0, e("@bokehjs/base").register_models)(b)
+            "ef403b5ad2": function _(e, s, t, b, o) {
+                b();
+                const r = e("tslib").__importStar(e("79591b3bf4"));
+                t.jsTree = r;
+                (0, e("@bokehjs/base").register_models)(r)
             },
-            "c52315dab1": function _(e, t, s, o, i) {
+            "79591b3bf4": function _(e, t, s, o, i) {
                 var l;
                 o();
-                const _ = e("@bokehjs/core/dom"),
-                    n = e("bfe8e8c0eb");
-                class r extends n.HTMLBoxView {
+                const n = e("@bokehjs/core/dom"),
+                    _ = e("bfe8e8c0eb");
+                class r extends _.HTMLBoxView {
                     initialize() {
                         super.initialize(), this._last_selected = []
                     }
                     connect_signals() {
-                        console.log("connect"), super.connect_signals(), this.connect(this.model.properties._data.change, (() => this._update_tree_from_data())), this.connect(this.model.properties.value.change, (() => this._update_selection_from_value())), this.connect(this.model.properties._new_nodes.change, (() => this._update_tree_from_new_nodes())), this.connect(this.model.properties.show_icons.change, (() => this._setShowIcons())), this.connect(this.model.properties.show_dots.change, (() => this._setShowDots())), this.connect(this.model.properties.multiple.change, (() => this._setMultiple())), console.log(this.model.show_dots), console.log(this.model.show_icons)
+                        console.log("connect"), super.connect_signals(), this.connect(this.model.properties._data.change, (() => this._update_tree_from_data())), this.connect(this.model.properties.value.change, (() => this._update_selection_from_value())), this.connect(this.model.properties._new_nodes.change, (() => this._update_tree_from_new_nodes())), this.connect(this.model.properties.checkbox.change, (() => this.setCheckboxes())), this.connect(this.model.properties.show_icons.change, (() => this._setShowIcons())), this.connect(this.model.properties.show_dots.change, (() => this._setShowDots())), this.connect(this.model.properties.multiple.change, (() => this._setMultiple())), console.log(this.model.show_dots), console.log(this.model.show_icons)
                     }
                     render() {
-                        super.render(), this._id = "_" + Math.random().toString(36).substring(2, 11), console.log(this._id), this._container = (0, _.div)({
+                        super.render(), this._id = "_" + Math.random().toString(36).substring(2, 11), console.log(this._id), this._container = (0, n.div)({
                             id: this._id,
                             style: "overflow: auto; minHeight: 200px; minWidth: 200px;"
-                        }), (0, n.set_size)(this._container, this.model), this.shadow_el.appendChild(this._container), console.log(this._container);
+                        }), (0, _.set_size)(this._container, this.model), this.shadow_el.appendChild(this._container), console.log(this._container), this.model.checkbox && this.model.plugins.push("checkbox");
                         this._jstree = jQuery(this._container).jstree(Object.assign({
                             core: {
                                 data: this.model._data,
                                 check_callback: !0,
                                 multiple: this.model.multiple,
                                 themes: {
                                     dots: this.model.show_dots,
@@ -85,54 +85,57 @@
                             checkbox: {
                                 three_state: !1,
                                 cascade: "undetermined"
                             }
                         })), this.init_callbacks()
                     }
                     init_callbacks() {
-                        this._jstree.on("ready.jstree", (({}, {}) => this.onjsTreeInit())), this._jstree.on("refresh.jstree", (({}, {}) => this._update_selection_from_value())), this._jstree.on("activate_node.jstree", (({}, e) => this.selectNodeFromEditor({}, e))), this._jstree.on("before_open.jstree", ((e, t) => this._listen_for_node_open(e, t)))
+                        this._jstree.on("refresh.jstree", (({}, {}) => this._update_selection_from_value())), this._jstree.on("model.jstree", (({}, {}) => this.onNewData())), this._jstree.on("activate_node.jstree", (({}, e) => this.selectNodeFromEditor({}, e))), this._jstree.on("before_open.jstree", ((e, t) => this._listen_for_node_open(e, t)))
                     }
-                    onjsTreeInit() {
+                    onNewData() {
                         this.model._flat_tree = this._jstree.jstree(!0).get_json(null, {
                             flat: !0
                         }), console.log("flat tree: ", this.model._flat_tree)
                     }
                     selectNodeFromEditor({}, e) {
                         console.log("select pre", this.model.value), this.model.value = e.instance.get_selected(), console.log("select post", this.model.value)
                     }
                     _update_selection_from_value() {
                         if (console.log("update selection from value"), this._jstree.jstree(!0).select_node(this.model.value), this.model.value != this._last_selected) {
                             let e = this._last_selected.filter((e => !this.model.value.includes(e)));
                             this._jstree.jstree(!0).deselect_node(e)
                         }
-                        this._last_selected = this.model.value, this.model.show_icons ? this._jstree.jstree(!0).show_icons() : this._jstree.jstree(!0).hide_icons()
+                        this._last_selected = this.model.value
                     }
                     _update_tree_from_new_nodes() {
                         console.log("new nodes: ", this.model._new_nodes);
                         for (let e of this.model._new_nodes) this._jstree.jstree(!0).create_node(e.parent, e, "first");
                         this._jstree.jstree(!0).settings.core.data = this._jstree.jstree(!0).get_json(null, {
                             no_li_attr: !0,
                             no_a_attr: !0,
                             no_data: !0
                         }), this.model._data = this._jstree.jstree(!0).settings.core.data
                     }
                     _update_tree_from_data() {
-                        console.log("updating data"), this._jstree.jstree(!0).settings.core.data = this.model._data, console.log("data: ", this._jstree.jstree(!0).settings.core.data), this.model._flat_tree = this._jstree.jstree(!0).get_json(null, {
-                            flat: !0
-                        }), console.log("flat tree: ", this.model._flat_tree), console.log("value after data", this.model.value), this._jstree.jstree(!0).refresh({
+                        console.log("updating data"), this._jstree.jstree(!0).settings.core.data = this.model._data, console.log("data: ", this._jstree.jstree(!0).settings.core.data), console.log("value after data", this.model.value), this._jstree.jstree(!0).refresh({
                             skip_loading: !1,
                             forget_state: !0
-                        }), console.log("value after refresh", this.model.value)
+                        }), this._jstree.jstree(!0).deselect_all({
+                            supress_event: !0
+                        }), console.log("value after refresh", this.model.value), console.log("data after refresh", this._jstree.jstree(!0).settings.core.data)
                     }
                     _setShowIcons() {
                         console.log("setShowIcons"), this.model.show_icons ? this._jstree.jstree(!0).show_icons() : this._jstree.jstree(!0).hide_icons()
                     }
                     _setShowDots() {
                         console.log("setShowDots"), this.model.show_dots ? this._jstree.jstree(!0).show_dots() : this._jstree.jstree(!0).hide_dots()
                     }
+                    setCheckboxes() {
+                        console.log("setCheckBoxes"), this.model.checkbox ? this._jstree.jstree(!0).show_checkboxes() : this._jstree.jstree(!0).hide_checkboxes()
+                    }
                     _setMultiple() {
                         console.log("setMultiple"), this._jstree.jstree(!0).settings.core.multiple = this.model.multiple
                     }
                     _update_tree_theme_from_model() {
                         this._jstree.jstree(!0).refresh(!1, !0)
                     }
                     _listen_for_node_open({}, e) {
@@ -141,27 +144,28 @@
                     add_node_children(e) {
                         console.log("add node children"), e.children_nodes = [];
                         for (let t of e.children) e.children_nodes.push(this._jstree.jstree(!0).get_node(t));
                         return e
                     }
                 }
                 s.jsTreePlotView = r, r.__name__ = "jsTreePlotView";
-                class d extends n.HTMLBox {
+                class h extends _.HTMLBox {
                     constructor(e) {
                         super(e)
                     }
                 }
-                s.jsTreePlot = d, l = d, d.__name__ = "jsTreePlot", d.__module__ = "panel_jstree.bokeh_extensions.jstree", l.prototype.default_view = r, l.define((({
+                s.jsTreePlot = h, l = h, h.__name__ = "jsTreePlot", h.__module__ = "panel_jstree.bokeh_extensions.jstree", l.prototype.default_view = r, l.define((({
                     Array: e,
                     Any: t,
                     Boolean: s
                 }) => ({
                     value: [e(t), []],
                     _data: [e(t), []],
                     plugins: [e(t), []],
+                    checkbox: [s, !0],
                     multiple: [s, !0],
                     show_icons: [s, !0],
                     show_dots: [s, !0],
                     _last_opened: [t, {}],
                     _new_nodes: [e(t), []],
                     _flat_tree: [e(t), []]
                 })))
@@ -245,11 +249,11 @@
                     }
                 }
                 i.HTMLBox = c, c.__name__ = "HTMLBox"
             },
         }, "ecf49f9c64", {
             "index": "ecf49f9c64",
             "bokeh_extensions/index": "ef403b5ad2",
-            "bokeh_extensions/jstree": "c52315dab1",
+            "bokeh_extensions/jstree": "79591b3bf4",
             "bokeh_extensions/layout": "bfe8e8c0eb"
         }, {});
 });
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/package-lock.json` & `panel-jstree-0.3.0/src/panel_jstree/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9161931818181818%*

 * *Differences: {"'packages'": "{'': {'version': '0.3.0'}}", "'version'": "'0.3.0'"}*

```diff
@@ -68,15 +68,15 @@
         "": {
             "dependencies": {
                 "@bokeh/bokehjs": "^3.1",
                 "@holoviz/panel": "^1"
             },
             "license": "MIT",
             "name": "panel_jstree",
-            "version": "0.2.2"
+            "version": "0.3.0"
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
-    "version": "0.2.2"
+    "version": "0.3.0"
 }
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree/tsconfig.json` & `panel-jstree-0.3.0/src/panel_jstree/tsconfig.json`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.2.2/src/panel_jstree/widgets/jstree.py` & `panel-jstree-0.3.0/src/panel_jstree/widgets/jstree.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,17 +111,14 @@
         if not properties.get("height") and (
             self.sizing_mode is None or "width" in self.sizing_mode
         ):
             properties["height"] = 400
         if properties.get("height") and properties["height"] < 100:
             properties["height"] = 100
 
-        if properties.pop("checkbox", None):
-            properties.get("plugins", []).append("checkbox")
-
         properties["value"] = self._values
         return properties
 
     def add_children_on_new_values(self, *event):
         def transverse(d: list, value):
             parents = self._get_parents_cb(value)
             for node in d:
@@ -201,14 +198,17 @@
     def __init__(self, data, **params):
         if "get_children_cb" in params:
             params["_get_children_cb"] = params.pop("get_children_cb")
         super().__init__(_data=data, **params)
 
     @property
     def data(self):
+        """When swapping out data, you are not able to input selections data on nodes.
+        All nodes will start out deselected.
+        """
         return self._data
 
     @data.setter
     def data(self, value):
         self._data = value
 
     @property
@@ -227,15 +227,25 @@
         default=str(Path.cwd()),
         doc="""
         The directory to explore.""",
     )
 
     @property
     def _values(self):
-        return [os.path.expanduser(os.path.normpath(p)) for p in self.value]
+        # normpath removes any ending slashes that mess up jstree
+        # expand user lets people use things like ~ for home
+        values = [os.path.expanduser(os.path.normpath(p)) for p in self.value]
+
+        # This lets people use paths relative to self.directory
+        for i, value in enumerate(values):
+            value = Path(value)
+            if not value.is_absolute():
+                values[i] = str(Path(self.directory).parent / value)
+
+        return values
 
     def _process_param_change(self, msg: dict[str, Any]) -> dict[str, Any]:
         """
         Transform parameter changes into bokeh model property updates.
         Should be overridden to provide appropriate mapping between
         parameter value and bokeh model change. By default uses the
         _rename class level attribute to map between parameter and
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree.egg-info/PKG-INFO` & `panel-jstree-0.3.0/src/panel_jstree.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panel-jstree
-Version: 0.2.2
+Version: 0.3.0
 Summary: panel-jstree is a wrapper python wrapper around the javascript library jstree for use in panel. This allows for JSON-like representations of tree data. One very useful implementation provided is a server-side file browser.
 Author: madeline-scyphers
 License: MIT License
         
         Copyright (c) 2023 Madeline Scyphers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,14 +28,15 @@
 Keywords: python,holoviz,panel,dataviz,dataapp,dashboard,datascience,analytics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Legal Industry
@@ -57,42 +58,57 @@
 # ✨ panel-jstree
 
 panel-jstree is a wrapper python wrapper around the javascript library [jstree](https://www.jstree.com) for use in [panel](https://panel.holoviz.org/). This allows for JSON-like representations of tree data. One very useful implementation provided is a server-side file browser.
 
 You can install and use the package as simple as.
 
 ```bash
+conda install -c conda-forge panel-jstree
+```
+
+or with pip
+
+```bash
 pip install panel-jstree
 ```
 
+Add this into a python file to play with the FileTree
+
 ```python
-import panel as pn
 from panel_jstree import FileTree
 
-pn.Column(FileTree())
+FileTree().servable()
 ```
 
+run it with `panel serve name_of_app.py`
+
+It should run exploring the directory of the file.
+
 ![Project Intro](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/project-intro.gif)
 
 ## 🚀 Get started in under a minute
 
 ```bash
 pip install  panel-jstree
 ```
 
 Run the examples
 
 ```bash
-panel serve examples/*.py --show
+panel serve tests/*tree.py --show
 ```
 
 Here are some of the examples. You can see a small FileTree app with a text field and controls to directly input a file path, and turn off and on some of the controls.
 
 ![FileTree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/file-tree.gif)
 
+You can make a simple tree where you swap out the data.
+
+![Randomw Tree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/simple-tree.gif)
+
 You can also see a generic Tree app with a custom callback to generate random nodes.
 
 ![Randomw Tree App Example](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/random-tree.gif)
 
 
 ## ⭐ Support
 
@@ -105,11 +121,14 @@
 
 If you are looking to contribute to this project you can find ideas in the [issue tracker](https://github.com/madeline-scyphers/panel-jstree/issues). To get started check out the [DEVELOPER_GUIDE](DEVELOPER_GUIDE.md).
 
 I would love to support and receive your contributions. Thanks.
 
 ## Monitor
 
-[![PyPI version](https://badge.fury.io/py/panel-jstree.svg)](https://pypi.org/project/panel-jstree/)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
-[![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIT)
-
+|                 |                                                                                                                                                                         |
+|-----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Conda Install   | [![Conda Version](https://anaconda.org/conda-forge/panel-jstree/badges/version.svg)](https://anaconda.org/conda-forge/panel-jstree)                                     |
+| PyPI Install    | [![PyPI version](https://badge.fury.io/py/panel-jstree.svg)](https://badge.fury.io/py/panel-jstree)                                                                     |
+| Github release  | [![Github tag](https://img.shields.io/github/v/tag/madeline-scyphers/panel-jstree.svg?label=tag&colorB=11ccbb)](https://github.com/madeline-scyphers/panel-jstree/tags) |
+| Python Versions | ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)                                                                               |
+| License         | [![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIT)                                                              |
```

### Comparing `panel-jstree-0.2.2/src/panel_jstree.egg-info/SOURCES.txt` & `panel-jstree-0.3.0/src/panel_jstree.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts
 src/panel_jstree/dist/lib/bokeh_extensions/layout.js
 src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map
 src/panel_jstree/widgets/__init__.py
 src/panel_jstree/widgets/jstree.py
 tests/test_file_tree.py
 tests/test_hello.py
+tests/test_random_tree.py
 tests/test_tree.py
```

