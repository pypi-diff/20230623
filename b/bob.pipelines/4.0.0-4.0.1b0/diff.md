# Comparing `tmp/bob.pipelines-4.0.0.tar.gz` & `tmp/bob.pipelines-4.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.pipelines-4.0.0.tar", last modified: Fri Jun 16 12:22:58 2023, max compression
+gzip compressed data, was "bob.pipelines-4.0.1b0.tar", last modified: Fri Jun 23 19:16:50 2023, max compression
```

## Comparing `bob.pipelines-4.0.0.tar` & `bob.pipelines-4.0.1b0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.010799 bob.pipelines-4.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1556 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-16 12:22:58.010799 bob.pipelines-4.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-16 12:18:53.000000 bob.pipelines-4.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:57.998799 bob.pipelines-4.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     8204 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/checkpoint.rst
--rw-rw-rw-   0 root         (0) root         (0)     6980 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/dask.rst
--rw-rw-rw-   0 root         (0) root         (0)     5994 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/datasets.rst
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/extra-intersphinx.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:57.998799 bob.pipelines-4.0.0/doc/img/
--rw-rw-rw-   0 root         (0) root         (0)     6547 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/img/bob-128x128.png
--rw-rw-rw-   0 root         (0) root         (0)     4286 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/img/bob-favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     6266 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/img/bob-logo.png
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/nitpick-exceptions.txt
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/py_api.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:57.998799 bob.pipelines-4.0.0/doc/python/
--rw-rw-rw-   0 root         (0) root         (0)   158363 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/python/dask_graph.png
--rw-rw-rw-   0 root         (0) root         (0)     7009 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/sample.rst
--rw-rw-rw-   0 root         (0) root         (0)    17817 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/doc/xarray.rst
--rw-rw-rw-   0 root         (0) root         (0)     3630 2023-06-16 12:18:53.000000 bob.pipelines-4.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:22:58.010799 bob.pipelines-4.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:57.994799 bob.pipelines-4.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:57.998799 bob.pipelines-4.0.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.002799 bob.pipelines-4.0.0/src/bob/pipelines/
--rw-rw-rw-   0 root         (0) root         (0)     1788 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.002799 bob.pipelines-4.0.0/src/bob/pipelines/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 12:22:35.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.006799 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 12:22:35.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/dask_it_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/local_p16.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/local_p32.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/local_p4.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/local_p8.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/local_parallel.py
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/local_single_thread.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_default.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_demanding.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_gpu.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_io_big.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_io_big_non_adaptive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.006799 bob.pipelines-4.0.0/src/bob/pipelines/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10356 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/dataset/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.006799 bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6485 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/archive.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/hashing.py
--rw-rw-rw-   0 root         (0) root         (0)    14922 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/retrieve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.006799 bob.pipelines-4.0.0/src/bob/pipelines/distributed/
--rw-rw-rw-   0 root         (0) root         (0)     3588 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/distributed/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17088 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/distributed/sge.py
--rw-rw-rw-   0 root         (0) root         (0)     4109 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/distributed/sge_queues.py
--rw-rw-rw-   0 root         (0) root         (0)    10578 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.006799 bob.pipelines-4.0.0/src/bob/pipelines/transformers/
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/transformers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/transformers/str_to_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6659 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    41078 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/wrappers.py
--rw-rw-rw-   0 root         (0) root         (0)    18570 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/src/bob/pipelines/xarray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.002799 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-16 12:22:57.000000 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-16 12:22:57.000000 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:22:57.000000 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      720 2023-06-16 12:22:57.000000 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:22:57.000000 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-16 12:22:57.000000 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-16 12:22:57.000000 bob.pipelines-4.0.0/src/bob.pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:22:58.006799 bob.pipelines-4.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4519 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/tests/test_database.py
--rw-rw-rw-   0 root         (0) root         (0)     5145 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/tests/test_samples.py
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/tests/test_transformers.py
--rw-rw-rw-   0 root         (0) root         (0)     7394 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    28384 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/tests/test_wrappers.py
--rw-rw-rw-   0 root         (0) root         (0)     8231 2023-06-12 19:12:09.000000 bob.pipelines-4.0.0/tests/test_xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.723103 bob.pipelines-4.0.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-06-23 19:16:50.723103 bob.pipelines-4.0.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.711103 bob.pipelines-4.0.1b0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     8204 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/checkpoint.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6980 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/dask.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/datasets.rst
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/extra-intersphinx.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.711103 bob.pipelines-4.0.1b0/doc/img/
+-rw-rw-rw-   0 root         (0) root         (0)     6547 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/img/bob-128x128.png
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/img/bob-favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/img/bob-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/nitpick-exceptions.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/py_api.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.711103 bob.pipelines-4.0.1b0/doc/python/
+-rw-rw-rw-   0 root         (0) root         (0)   158363 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/python/dask_graph.png
+-rw-rw-rw-   0 root         (0) root         (0)     7009 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/sample.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17817 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/doc/xarray.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:16:50.723103 bob.pipelines-4.0.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.707103 bob.pipelines-4.0.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.711103 bob.pipelines-4.0.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.715103 bob.pipelines-4.0.1b0/src/bob/pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.715103 bob.pipelines-4.0.1b0/src/bob/pipelines/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:16:22.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.719103 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:16:22.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/dask_it_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/local_p16.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/local_p32.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/local_p4.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/local_p8.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/local_parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/local_single_thread.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_default.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_demanding.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_gpu.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_io_big.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_io_big_non_adaptive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.719103 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10356 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.719103 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6485 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)    14922 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/retrieve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.719103 bob.pipelines-4.0.1b0/src/bob/pipelines/distributed/
+-rw-rw-rw-   0 root         (0) root         (0)     3588 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/distributed/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17088 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/distributed/sge.py
+-rw-rw-rw-   0 root         (0) root         (0)     4109 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/distributed/sge_queues.py
+-rw-rw-rw-   0 root         (0) root         (0)    10578 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.719103 bob.pipelines-4.0.1b0/src/bob/pipelines/transformers/
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/transformers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/transformers/str_to_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6659 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    41078 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/wrappers.py
+-rw-rw-rw-   0 root         (0) root         (0)    18570 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/src/bob/pipelines/xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.715103 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-06-23 19:16:50.000000 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-23 19:16:50.000000 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:16:50.000000 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-23 19:16:50.000000 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:16:50.000000 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-23 19:16:50.000000 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 19:16:50.000000 bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:50.723103 bob.pipelines-4.0.1b0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/tests/test_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5145 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/tests/test_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/tests/test_transformers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7394 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    28384 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/tests/test_wrappers.py
+-rw-rw-rw-   0 root         (0) root         (0)     8231 2023-06-23 19:11:47.000000 bob.pipelines-4.0.1b0/tests/test_xarray.py
```

### Comparing `bob.pipelines-4.0.0/LICENSE` & `bob.pipelines-4.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/PKG-INFO` & `bob.pipelines-4.0.1b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.pipelines
-Version: 4.0.0
+Version: 4.0.1b0
 Summary: Tools to build robust and extensible pipelines
 Author-email: Tiago de Freitas Pereira <tiago.pereira@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.pipelines/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.pipelines
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.pipelines/-/releases
 Keywords: bob,pipelines
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,17 +21,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![badge doc](https://img.shields.io/badge/docs-v4.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pipelines/badges/v4.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pipelines/commits/v4.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.pipelines/badges/v4.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pipelines/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pipelines/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.pipelines/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.pipelines)
 
 # Tools to build robust and extensible pipelines
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
```

### Comparing `bob.pipelines-4.0.0/README.md` & `bob.pipelines-4.0.1b0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![badge doc](https://img.shields.io/badge/docs-v4.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pipelines/badges/v4.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pipelines/commits/v4.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.pipelines/badges/v4.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pipelines/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pipelines/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.pipelines/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.pipelines)
 
 # Tools to build robust and extensible pipelines
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
```

### Comparing `bob.pipelines-4.0.0/doc/checkpoint.rst` & `bob.pipelines-4.0.1b0/doc/checkpoint.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/dask.rst` & `bob.pipelines-4.0.1b0/doc/dask.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/datasets.rst` & `bob.pipelines-4.0.1b0/doc/datasets.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/img/bob-128x128.png` & `bob.pipelines-4.0.1b0/doc/img/bob-128x128.png`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/img/bob-favicon.ico` & `bob.pipelines-4.0.1b0/doc/img/bob-favicon.ico`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/img/bob-logo.png` & `bob.pipelines-4.0.1b0/doc/img/bob-logo.png`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/index.rst` & `bob.pipelines-4.0.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/links.rst` & `bob.pipelines-4.0.1b0/doc/links.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/nitpick-exceptions.txt` & `bob.pipelines-4.0.1b0/doc/nitpick-exceptions.txt`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/py_api.rst` & `bob.pipelines-4.0.1b0/doc/py_api.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/python/dask_graph.png` & `bob.pipelines-4.0.1b0/doc/python/dask_graph.png`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/sample.rst` & `bob.pipelines-4.0.1b0/doc/sample.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/doc/xarray.rst` & `bob.pipelines-4.0.1b0/doc/xarray.rst`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/pyproject.toml` & `bob.pipelines-4.0.1b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "bob.pipelines"
-    version = "4.0.0"
+    version = "4.0.1b0"
     requires-python = ">=3.9"
     description = "Tools to build robust and extensible pipelines"
     dynamic = ["readme"]
     license = {text = "BSD 3-Clause License"}
     authors = [
     {name = "Tiago de Freitas Pereira", email = "tiago.pereira@idiap.ch"},
     ]
@@ -22,49 +22,49 @@
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "bob.io.base==5.1.0",
-        "clapper==1.0.1",
-        "dask==2023.1.0",
-        "dask-jobqueue==0.8.1",
-        "distributed==2023.1.0",
-        "h5py==3.7.0",
-        "numpy==1.23.5",
-        "requests==2.28.2",
-        "scikit-learn==1.1.2",
-        "xarray==2022.12.0",
+        "bob",
+        "bob.io.base",
+        "clapper",
+        "dask",
+        "dask-jobqueue",
+        "distributed",
+        "h5py",
+        "numpy",
+        "requests",
+        "scikit-learn",
+        "xarray",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/sphinx/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/sphinx/"
     homepage = "https://pypi.org/project/bob.pipelines/"
     repository = "https://gitlab.idiap.ch/bob/bob.pipelines"
     changelog = "https://gitlab.idiap.ch/bob/bob.pipelines/-/releases"
 
 [project.optional-dependencies]
     qa = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "auto-intersphinx==1.0.2",
-        "sphinxcontrib-programoutput==0.17",
-        "matplotlib==3.6.2",
-        "dask-ml==2022.5.27",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
+        "auto-intersphinx",
+        "sphinxcontrib-programoutput",
+        "matplotlib",
+        "dask-ml",
         ]
     test = [
-        "pytest==7.2.1",
-        "pytest-cov==4.0.0",
-        "coverage==7.0.5",
-        "dask-ml==2022.5.27",
+        "pytest",
+        "pytest-cov",
+        "coverage",
+        "dask-ml",
         ]
 
 [tool.setuptools]
     zip-safe = false
     package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
@@ -101,11 +101,7 @@
     addopts = [
         "--import-mode=append",
         "--cov-report=term-missing",
         "--cov=bob.pipelines",
     ]
     junit_logging = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/__init__.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_default.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_default.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_demanding.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_demanding.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_gpu.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_gpu.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/config/distributed/sge_io_big.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/config/distributed/sge_io_big.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/dataset/__init__.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/dataset/database.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/database.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/archive.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/archive.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/hashing.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/hashing.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/dataset/protocols/retrieve.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/dataset/protocols/retrieve.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/distributed/__init__.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/distributed/sge.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/distributed/sge.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/distributed/sge_queues.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/distributed/sge_queues.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/sample.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/sample.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/transformers/__init__.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/transformers/str_to_types.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/transformers/str_to_types.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/utils.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/wrappers.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/wrappers.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob/pipelines/xarray.py` & `bob.pipelines-4.0.1b0/src/bob/pipelines/xarray.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob.pipelines.egg-info/PKG-INFO` & `bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.pipelines
-Version: 4.0.0
+Version: 4.0.1b0
 Summary: Tools to build robust and extensible pipelines
 Author-email: Tiago de Freitas Pereira <tiago.pereira@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.pipelines/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.pipelines
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.pipelines/-/releases
 Keywords: bob,pipelines
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,17 +21,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![badge doc](https://img.shields.io/badge/docs-v4.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pipelines/badges/v4.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pipelines/commits/v4.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.pipelines/badges/v4.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/v4.0.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.pipelines/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.pipelines/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.pipelines/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.pipelines/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.pipelines)
 
 # Tools to build robust and extensible pipelines
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob).
```

### Comparing `bob.pipelines-4.0.0/src/bob.pipelines.egg-info/SOURCES.txt` & `bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/src/bob.pipelines.egg-info/entry_points.txt` & `bob.pipelines-4.0.1b0/src/bob.pipelines.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/tests/test_database.py` & `bob.pipelines-4.0.1b0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/tests/test_samples.py` & `bob.pipelines-4.0.1b0/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/tests/test_utils.py` & `bob.pipelines-4.0.1b0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/tests/test_wrappers.py` & `bob.pipelines-4.0.1b0/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `bob.pipelines-4.0.0/tests/test_xarray.py` & `bob.pipelines-4.0.1b0/tests/test_xarray.py`

 * *Files identical despite different names*

