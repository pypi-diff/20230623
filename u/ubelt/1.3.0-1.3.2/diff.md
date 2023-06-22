# Comparing `tmp/ubelt-1.3.0.tar.gz` & `tmp/ubelt-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubelt-1.3.0.tar", last modified: Thu Jun 15 02:32:50 2023, max compression
+gzip compressed data, was "ubelt-1.3.2.tar", last modified: Thu Jun 22 22:39:39 2023, max compression
```

## Comparing `ubelt-1.3.0.tar` & `ubelt-1.3.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:50.173372 ubelt-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-15 02:32:40.000000 ubelt-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-15 02:32:50.173372 ubelt-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    58336 2023-06-15 02:32:40.000000 ubelt-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 02:32:40.000000 ubelt-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:32:50.173372 ubelt-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7952 2023-06-15 02:32:40.000000 ubelt-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:50.173372 ubelt-1.3.0/ubelt/
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/_win32_links.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/_win32_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/orderedset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36626 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/progiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/progiter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_arg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    52100 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    31964 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_cmd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_const.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_const.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_deprecate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    74794 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_download_manager.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_func.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_futures.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_hash.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38221 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_import.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_indexable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_indexable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_io.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_links.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    32834 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_memoize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_mixins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59178 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_platform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42633 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_repr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_str.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22494 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_time.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-15 02:32:40.000000 ubelt-1.3.0/ubelt/util_zip.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:32:50.173372 ubelt-1.3.0/ubelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 02:32:50.000000 ubelt-1.3.0/ubelt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:39.954758 ubelt-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 22:39:34.000000 ubelt-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-22 22:39:39.954758 ubelt-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    58336 2023-06-22 22:39:34.000000 ubelt-1.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-22 22:39:34.000000 ubelt-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:39:39.954758 ubelt-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7952 2023-06-22 22:39:34.000000 ubelt-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:39.954758 ubelt-1.3.2/ubelt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/_win32_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/_win32_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/orderedset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36626 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/progiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/progiter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_arg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    52100 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    32162 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_cmd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_const.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_deprecate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    74794 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_download_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_func.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_futures.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    50076 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_hash.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_import.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_indexable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_indexable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_io.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_links.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    32834 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_memoize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59662 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_platform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42633 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_repr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_str.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22732 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_time.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-22 22:39:34.000000 ubelt-1.3.2/ubelt/util_zip.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:39.954758 ubelt-1.3.2/ubelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    59674 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 22:39:39.000000 ubelt-1.3.2/ubelt.egg-info/top_level.txt
```

### Comparing `ubelt-1.3.0/LICENSE` & `ubelt-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/PKG-INFO` & `ubelt-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubelt
-Version: 1.3.0
+Version: 1.3.2
 Summary: A Python utility belt containing simple tools, a stdlib like feel, and extra batteries.
 Home-page: https://github.com/Erotemic/ubelt
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ubelt-1.3.0/README.rst` & `ubelt-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/pyproject.toml` & `ubelt-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/setup.py` & `ubelt-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/__init__.py` & `ubelt-1.3.2/ubelt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     mkinit ubelt -w  # todo: get sphinx to ignore this
     # TODO: Lazy imports with mkinit (requires python 3.7)
 
 Testing:
     xdoctest ubelt
 """
 
-__version__ = '1.3.0'
+__version__ = '1.3.2'
 
 # Deprecated functions
 from ubelt.util_platform import (
     ensure_app_cache_dir, ensure_app_config_dir,
     ensure_app_data_dir, get_app_cache_dir, get_app_config_dir,
     get_app_data_dir,
 )
```

### Comparing `ubelt-1.3.0/ubelt/_win32_links.py` & `ubelt-1.3.2/ubelt/_win32_links.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/orderedset.py` & `ubelt-1.3.2/ubelt/orderedset.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/orderedset.pyi` & `ubelt-1.3.2/ubelt/orderedset.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/progiter.py` & `ubelt-1.3.2/ubelt/progiter.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/progiter.pyi` & `ubelt-1.3.2/ubelt/progiter.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_arg.py` & `ubelt-1.3.2/ubelt/util_arg.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_cache.py` & `ubelt-1.3.2/ubelt/util_cache.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_cache.pyi` & `ubelt-1.3.2/ubelt/util_cache.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_cmd.py` & `ubelt-1.3.2/ubelt/util_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,59 +152,60 @@
     (4) ability to detach, return the process object and allow the process to
     run in the background (eventually we may return a Future object instead).
 
     Args:
         command (str | List[str]):
             command string, tuple of executable and args, or shell command.
 
-        shell (bool, default=False):
-            if True, process is run in shell.
+        shell (bool):
+            if True, process is run in shell. Defaults to False.
 
-        detach (bool, default=False):
-            if True, process is detached and run in background.
+        detach (bool):
+            if True, process is detached and run in background. Defaults to False.
 
-        verbose (int, default=0):
-            verbosity mode. Can be 0, 1, 2, or 3.
+        verbose (int):
+            verbosity mode. Can be 0, 1, 2, or 3. Defaults to 0.
 
         tee (bool | None):
             if True, simultaneously writes to stdout while capturing output
             from the command. If not specified, defaults to True if verbose >
             0.  If detach is True, then this argument is ignored.
 
         cwd (str | PathLike | None):
             Path to run command. Defaults to current working directory if
             unspecified.
 
         env (Dict[str, str] | None):
             environment passed to Popen
 
-        tee_backend (str, default='auto'): backend for tee output.
+        tee_backend (str): backend for tee output.
             Valid choices are: "auto", "select" (POSIX only), and "thread".
+            Defaults to "auto".
 
-        check (bool, default=False):
+        check (bool):
             if True, check that the return code was zero before returning,
             otherwise raise a :class:`subprocess.CalledProcessError`.
-            Does nothing if detach is True.
+            Does nothing if detach is True.  Defaults to False.
 
-        system (bool, default=False):
+        system (bool):
             if True, most other considerations are dropped, and
             :func:`os.system` is used to execute the command in a platform
             dependant way. Other arguments such as env, tee, timeout, and shell
-            are all ignored.  (new in version 1.1.0)
+            are all ignored. Defaults to False. (New in version 1.1.0)
 
         timeout (float | None):
             If the process does not complete in ``timeout`` seconds, raise a
-            :class:`subprocess.TimeoutExpired`. (new in version 1.1.0).
+            :class:`subprocess.TimeoutExpired`. (New in version 1.1.0).
 
         capture (bool):
             if True, the stdout/stderr are captured and returned in the
             information dictionary. Ignored if detatch or system is True.
 
     Returns:
-        dict:
+        dict | CmdOutput:
             info - information about command status.
             if detach is False ``info`` contains captured standard out,
             standard error, and the return code
             if detach is True ``info`` contains a reference to the process.
 
     Raises:
         ValueError - on an invalid configuration
@@ -212,23 +213,24 @@
         subprocess.CalledProcessError - if check and the return value is non zero
 
     Note:
         When using the tee output, the stdout and stderr may be shuffled from
         what they would be on the command line.
 
     Related Work:
-        https://github.com/pycontribs/subprocess-tee
-        https://github.com/mortoray/shelljob
-        https://github.com/netinvent/command_runner
-        https://www.pyinvoke.org/prior-art.html
+        Similar to other libraries: [SubprocTee]_, [ShellJob]_, [CmdRunner]_, [PyInvoke]_.
 
     References:
         .. [SO_11495783] https://stackoverflow.com/questions/11495783/redirect-subprocess-stderr-to-stdout
         .. [SO_7729336] https://stackoverflow.com/questions/7729336/how-can-i-print-and-display-subprocess-stdout-and-stderr-output-without-distorti
         .. [SO_33560364] https://stackoverflow.com/questions/33560364/python-windows-parsing-command-lines-with-shlex
+        .. [SubprocTee] https://github.com/pycontribs/subprocess-tee
+        .. [ShellJob] https://github.com/mortoray/shelljob
+        .. [CmdRunner] https://github.com/netinvent/command_runner
+        .. [PyInvoke] https://www.pyinvoke.org/prior-art.html
 
     CommandLine:
         xdoctest -m ubelt.util_cmd cmd:6
         python -c "import ubelt as ub; ub.cmd('ping localhost -c 2', verbose=2)"
         pytest "$(python -c 'import ubelt; print(ubelt.util_cmd.__file__)')" -sv --xdoctest-verbose 2
 
     Example:
```

### Comparing `ubelt-1.3.0/ubelt/util_cmd.pyi` & `ubelt-1.3.2/ubelt/util_cmd.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,38 @@
 from _typeshed import Incomplete
 
 __pitch__: str
 POSIX: Incomplete
 WIN32: Incomplete
 
 
+class CmdOutput(dict):
+
+    @property
+    def stdout(self):
+        ...
+
+    @property
+    def stderr(self):
+        ...
+
+    @property
+    def returncode(self):
+        ...
+
+    def check_returncode(self) -> None:
+        ...
+
+
 def cmd(command: str | List[str],
         shell: bool = False,
         detach: bool = False,
         verbose: int = 0,
         tee: bool | None = None,
         cwd: str | PathLike | None = None,
         env: Dict[str, str] | None = None,
         tee_backend: str = 'auto',
         check: bool = False,
         system: bool = False,
-        timeout: float | None = None) -> dict:
+        timeout: float | None = None,
+        capture: bool = True) -> dict | CmdOutput:
     ...
```

### Comparing `ubelt-1.3.0/ubelt/util_colors.py` & `ubelt-1.3.2/ubelt/util_colors.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_const.py` & `ubelt-1.3.2/ubelt/util_const.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_deprecate.py` & `ubelt-1.3.2/ubelt/util_deprecate.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_dict.py` & `ubelt-1.3.2/ubelt/util_dict.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_dict.pyi` & `ubelt-1.3.2/ubelt/util_dict.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_download.py` & `ubelt-1.3.2/ubelt/util_download.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_download.pyi` & `ubelt-1.3.2/ubelt/util_download.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_download_manager.py` & `ubelt-1.3.2/ubelt/util_download_manager.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_download_manager.pyi` & `ubelt-1.3.2/ubelt/util_download_manager.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_format.py` & `ubelt-1.3.2/ubelt/util_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,17 @@
         ...     'nest_dict2': {'k': [1, 2, {3: {4, 5}}]},
         ...     'nested_tuples': [tuple([1]), tuple([2, 3]), frozenset([4, 5, 6])],
         ...     'one_tup': tuple([1]),
         ...     'simple_dict': {'spam': 'eggs', 'ham': 'jam'},
         ...     'simple_list': [1, 2, 'red', 'blue'],
         ...     'odict': ub.odict([(2, '1'), (1, '2')]),
         ... }
-        >>> result = ub.repr2(dict_, nl=1, precision=2)
+        >>> import pytest
+        >>> with pytest.warns(DeprecationWarning):
+        >>>     result = ub.repr2(dict_, nl=1, precision=2)
         >>> print(result)
         {
             'custom_types': [slice(0, 1, None), 0.33],
             'nest_dict': {'k1': [1, 2, {3: {4, 5}}], 'key2': [1, 2, {3: {4, 5}}], 'key3': [1, 2, {3: {4, 5}}]},
             'nest_dict2': {'k': [1, 2, {3: {4, 5}}]},
             'nested_tuples': [(1,), (2, 3), {4, 5, 6}],
             'odict': {2: '1', 1: '2'},
```

### Comparing `ubelt-1.3.0/ubelt/util_func.py` & `ubelt-1.3.2/ubelt/util_func.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_func.pyi` & `ubelt-1.3.2/ubelt/util_func.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_futures.py` & `ubelt-1.3.2/ubelt/util_futures.py`

 * *Files 11% similar despite different names*

```diff
@@ -142,14 +142,23 @@
         >>>         assert i + 1 == f.result()
     """
     def __enter__(self):
         self.max_workers = 0
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         return False
 
     def submit(self, func, *args, **kw):
         """
         Submit a job to be executed later
 
         Returns:
@@ -295,14 +304,23 @@
         self.backend = backend
 
     def __enter__(self):
         self.backend.__enter__()
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         # Note: the following call will block
         return self.backend.__exit__(ex_type, ex_value, ex_traceback)
 
     def submit(self, func, *args, **kw):
         """
         Calls the submit function of the underlying backend.
 
@@ -419,14 +437,23 @@
         return self.executor.shutdown()
 
     def __enter__(self):
         self.executor.__enter__()
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         return self.executor.__exit__(ex_type, ex_value, ex_traceback)
 
     def _clear_completed(self):
         active_jobs = [job for job in self.jobs if job.running()]
         self.jobs = active_jobs
 
     def as_completed(self, timeout=None, desc=None, progkw=None):
@@ -526,14 +553,18 @@
         """
         An alternative to as completed.
 
         NOTE:
             The order of iteration may be changed in the future to be the
             submission order instead.
 
+        Yields:
+            concurrent.futures.Future:
+                The completed future object containing the results of a job.
+
         Example:
             >>> import ubelt as ub
             >>> pool = ub.JobPool('serial')
             >>> assert len(list(iter(pool))) == 0
             >>> pool.submit(print, 'hi')
             >>> assert len(list(iter(pool))) == 1
         """
```

### Comparing `ubelt-1.3.0/ubelt/util_futures.pyi` & `ubelt-1.3.2/ubelt/util_indexable.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,56 @@
-import concurrent
-import concurrent.futures
-from typing import Callable
-from typing import Any
+from typing import Tuple
 from typing import List
-import concurrent.futures
+from typing import Any
+from typing import Dict
 from _typeshed import Incomplete
 from collections.abc import Generator
 from typing import Any
 
 
-class SerialFuture(concurrent.futures.Future):
-    func: Incomplete
-    args: Incomplete
-    kw: Incomplete
-
-    def __init__(self, func, *args, **kw) -> None:
-        ...
-
-    def set_result(self, result) -> None:
-        ...
-
-
-class SerialExecutor:
-    max_workers: int
-
-    def __enter__(self):
-        ...
-
-    def __exit__(self, ex_type, ex_value, tb) -> None:
-        ...
-
-    def submit(self, func, *args, **kw) -> concurrent.futures.Future:
-        ...
-
-    def shutdown(self) -> None:
-        ...
-
-    def map(self, fn: Callable[..., Any], *iterables,
-            **kwargs) -> Generator[Any, None, None]:
-        ...
-
-
-class Executor:
-    backend: Incomplete
-
-    def __init__(self, mode: str = 'thread', max_workers: int = 0) -> None:
-        ...
-
-    def __enter__(self):
-        ...
-
-    def __exit__(self, ex_type, ex_value, tb):
-        ...
-
-    def submit(self, func, *args, **kw) -> concurrent.futures.Future:
-        ...
+class IndexableWalker(Generator):
+    data: dict | list | tuple
+    dict_cls: Tuple[type]
+    list_cls: Tuple[type]
+    indexable_cls: Incomplete
 
-    def shutdown(self):
+    def __init__(self, data, dict_cls=..., list_cls=...) -> None:
         ...
 
-    def map(self, fn, *iterables, **kwargs):
+    def __iter__(self) -> Generator[Tuple[List, Any], Any, Any]:
         ...
 
-
-class JobPool:
-    executor: Incomplete
-    transient: Incomplete
-    jobs: Incomplete
-
-    def __init__(self,
-                 mode: str = ...,
-                 max_workers: int = ...,
-                 transient: bool = ...) -> None:
+    def __next__(self) -> Any:
         ...
 
-    def __len__(self):
+    def send(self, arg) -> None:
         ...
 
-    def submit(self, func: Callable[..., Any], *args,
-               **kwargs) -> concurrent.futures.Future:
+    def throw(self,
+              type: Incomplete | None = ...,
+              value: Incomplete | None = ...,
+              traceback: Incomplete | None = ...) -> None:
         ...
 
-    def shutdown(self):
+    def __setitem__(self, path: List, value: Any) -> None:
         ...
 
-    def __enter__(self):
+    def __getitem__(self, path: List) -> Any:
         ...
 
-    def __exit__(self, a, b, c) -> None:
+    def __delitem__(self, path: List) -> None:
         ...
 
-    def as_completed(
-        self,
-        timeout: float | None = None,
-        desc: str | None = None,
-        progkw: dict | None = None
-    ) -> Generator[concurrent.futures.Future, None, None]:
+    def allclose(self,
+                 other: IndexableWalker | List | Dict,
+                 rel_tol: float = 1e-09,
+                 abs_tol: float = 0.0,
+                 return_info: bool = False) -> bool | Tuple[bool, Dict]:
         ...
 
-    def join(self, **kwargs) -> List[Any]:
-        ...
 
-    def __iter__(self):
-        ...
+def indexable_allclose(items1: dict | list | tuple,
+                       items2: dict | list | tuple,
+                       rel_tol: float = 1e-09,
+                       abs_tol: float = 0.0,
+                       return_info: bool = False) -> bool | Tuple[bool, Dict]:
+    ...
```

### Comparing `ubelt-1.3.0/ubelt/util_hash.py` & `ubelt-1.3.2/ubelt/util_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,16 @@
         return list(self.algos.keys())
 
     def _evaluate_registration_queue(self):
         for func in self._lazy_queue:
             try:
                 func()
             except ImportError:  # nocover
-                pass
-        self._lazy_queue = []
+                ...
+        self._lazy_queue.clear()
 
     def __contains__(self, key):
         if self._lazy_queue:  # nocover
             self._evaluate_registration_queue()
         return key in self.algos or key in self.aliases
 
     def _register_xxhash(self):  # nocover
@@ -334,14 +334,19 @@
         # New singledispatch registry implementation
         from functools import singledispatch
         def _hash_dispatch(data):
             raise NotImplementedError
         _hash_dispatch.__is_base__ = True
         self._hash_dispatch = singledispatch(_hash_dispatch)
 
+    def _evaluate_lazy_queue(self):
+        for func in self._lazy_queue:
+            func()
+        self._lazy_queue.clear()
+
     def register(self, hash_types):
         """
         Registers a function to generate a hash for data of the appropriate
         types. This can be used to register custom classes. Internally this is
         used to define how to hash non-builtin objects like ndarrays and uuids.
 
         The registered function should return a tuple of bytes. First a small
@@ -485,18 +490,19 @@
             >>> f2 = self.lookup(data)
             >>> print(f2(data))
             >>> data = np.uint8(3)
             >>> f3 = self.lookup(data)
             >>> print(f3(data))
         """
         # Evaluate the lazy queue if anything is in it
-        if self._lazy_queue:
-            for func in self._lazy_queue:
-                func()
-            self._lazy_queue = []
+        if self._lazy_queue:  # nocover
+            # Added nocover, because a bugfix prevents this from running and it
+            # is unclear how to build a test in for this.
+            self._evaluate_lazy_queue()
+
         query_hash_type = data.__class__
         # TODO: recognize some special dunder method instead
         # of strictly using this registry.
         hash_func = self._hash_dispatch.dispatch(query_hash_type)
         if getattr(hash_func, '__is_base__', False):
             raise TypeError(
                 'No registered hash func for hashable type={!r}'.format(
@@ -617,15 +623,15 @@
             >>>     'b': 2,
             >>>     'c': [1, 2, 3],
             >>> }
             >>> datas['odict_data2'] = ub.dict_subset(datas['odict_data1'], ['a', '4', 'c', 'b'])
             >>> datas['udict_data2'] = ub.dict_isect(datas['udict_data1'], ['a', '4', 'c', 'b'])
             >>> datas['odict_data3'] = ub.dict_subset(datas['odict_data1'], ['c', 'b', 'a', '4'])
             >>> datas['udict_data3'] = ub.dict_isect(datas['udict_data1'], ['c', 'b', 'a', '4'])
-            >>> # print('datas = {}'.format(ub.repr2(datas, nl=-1)))
+            >>> # print('datas = {}'.format(ub.urepr(datas, nl=-1)))
             >>> for key, val in sorted(datas.items()):
             >>>     hashstr = ub.hash_data(val, base='abc', hasher='sha512', types=True)[0:8]
             >>>     print('{} = {}'.format(key, hashstr))
             odict_data1 = omnqalbe
             odict_data2 = tjrlsoel
             odict_data3 = cycowefz
             udict_data1 = bvshfmzm
@@ -904,14 +910,19 @@
         >>> _update_hasher(hasher, data)
         >>> print(hasher.hexdigest()[0:8])
         e2c67675
     """
     if extensions is None:
         extensions = _HASHABLE_EXTENSIONS
 
+    # bugfix: ensure the lazy registration queue is evaluated before running
+    # the iterable checks.
+    if extensions._lazy_queue:
+        extensions._evaluate_lazy_queue()
+
     # Determine if the data should be hashed directly or iterated through
     if isinstance(data, (tuple, list, zip)):
         needs_iteration = True
     else:
         needs_iteration = any(check(data) for check in
                               extensions.iterable_checks)
```

### Comparing `ubelt-1.3.0/ubelt/util_hash.pyi` & `ubelt-1.3.2/ubelt/util_hash.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_import.py` & `ubelt-1.3.2/ubelt/util_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,24 @@
         self.index = index
 
     def __enter__(self):
         if self.index < 0:
             self.index = len(sys.path) + self.index + 1
         sys.path.insert(self.index, self.dpath)
 
-    def __exit__(self, type, value, trace):
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         need_recover = False
         if len(sys.path) <= self.index:  # nocover
             msg_parts = [
                 'sys.path changed while in PythonPathContext.',
                 'len(sys.path) = {!r} but index is {!r}'.format(
                     len(sys.path), self.index),
             ]
```

### Comparing `ubelt-1.3.0/ubelt/util_import.pyi` & `ubelt-1.3.2/ubelt/util_import.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Type
+from types import TracebackType
 from os import PathLike
 from types import ModuleType
 from typing import List
 from typing import Tuple
 from _typeshed import Incomplete
 
 
@@ -11,15 +13,17 @@
 
     def __init__(self, dpath, index: int = ...) -> None:
         ...
 
     def __enter__(self) -> None:
         ...
 
-    def __exit__(self, type, value, trace) -> None:
+    def __exit__(self, ex_type: Type[BaseException] | None,
+                 ex_value: BaseException | None,
+                 ex_traceback: TracebackType | None) -> bool | None:
         ...
 
 
 def import_module_from_path(modpath: str | PathLike,
                             index: int = ...) -> ModuleType:
     ...
```

### Comparing `ubelt-1.3.0/ubelt/util_indexable.py` & `ubelt-1.3.2/ubelt/util_indexable.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_io.py` & `ubelt-1.3.2/ubelt/util_io.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_io.pyi` & `ubelt-1.3.2/ubelt/util_io.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_links.py` & `ubelt-1.3.2/ubelt/util_links.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_list.py` & `ubelt-1.3.2/ubelt/util_list.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_list.pyi` & `ubelt-1.3.2/ubelt/util_list.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_memoize.py` & `ubelt-1.3.2/ubelt/util_memoize.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_mixins.py` & `ubelt-1.3.2/ubelt/util_mixins.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_path.py` & `ubelt-1.3.2/ubelt/util_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,15 +381,24 @@
 
     def __enter__(self):
         if self.context_dpath is not None:
             self.orig_dpath = os.getcwd()
             os.chdir(self.context_dpath)
         return self
 
-    def __exit__(self, a, b, c):
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         if self.context_dpath is not None:
             os.chdir(self.orig_dpath)
 
 
 class TempDir:
     """
     Context for creating and cleaning up temporary directories.
@@ -447,15 +456,24 @@
     def start(self):
         self.ensure()
         return self
 
     def __enter__(self):
         return self.start()
 
-    def __exit__(self, type_, value, trace):
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         self.cleanup()
 
 
 _PathBase = pathlib.WindowsPath if os.name == 'nt' else pathlib.PosixPath
 
 
 class Path(_PathBase):
```

### Comparing `ubelt-1.3.0/ubelt/util_path.pyi` & `ubelt-1.3.2/ubelt/util_path.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from os import PathLike
 from typing import Tuple
+from typing import Type
+from types import TracebackType
 from typing import List
 from typing import Callable
 from _typeshed import Incomplete
 from collections.abc import Generator
 
 
 def augpath(path: str | PathLike,
@@ -43,15 +45,17 @@
 
     def __init__(self, dpath) -> None:
         ...
 
     def __enter__(self):
         ...
 
-    def __exit__(self, a, b, c) -> None:
+    def __exit__(self, ex_type: Type[BaseException] | None,
+                 ex_value: BaseException | None,
+                 ex_traceback: TracebackType | None) -> bool | None:
         ...
 
 
 class TempDir:
     dpath: Incomplete
 
     def __init__(self) -> None:
@@ -68,15 +72,17 @@
 
     def start(self):
         ...
 
     def __enter__(self):
         ...
 
-    def __exit__(self, type_, value, trace) -> None:
+    def __exit__(self, ex_type: Type[BaseException] | None,
+                 ex_value: BaseException | None,
+                 ex_traceback: TracebackType | None) -> bool | None:
         ...
 
 
 class Path:
 
     @classmethod
     def appdir(cls,
```

### Comparing `ubelt-1.3.0/ubelt/util_platform.py` & `ubelt-1.3.2/ubelt/util_platform.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_platform.pyi` & `ubelt-1.3.2/ubelt/util_platform.pyi`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_repr.py` & `ubelt-1.3.2/ubelt/util_repr.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_str.py` & `ubelt-1.3.2/ubelt/util_str.py`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt/util_stream.py` & `ubelt-1.3.2/ubelt/util_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,17 +207,24 @@
         if self.cap_stdout is not None:
             self.close()
 
     def close(self):
         self.cap_stdout.close()
         self.cap_stdout = None
 
-    def __exit__(self, type_, value, trace):
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         if self.enabled:
             try:
                 self.log_part()
-            except Exception:  # nocover
-                raise
             finally:
                 self.stop()
-        if trace is not None:
+        if ex_traceback is not None:
             return False  # return a falsey value on error
```

### Comparing `ubelt-1.3.0/ubelt/util_time.py` & `ubelt-1.3.2/ubelt/util_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -569,17 +569,26 @@
             self.flush()
         return elapsed
 
     def __enter__(self):
         self.tic()
         return self
 
-    def __exit__(self, ex_type, ex_value, trace):
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         self.elapsed = self.toc()
-        if trace is not None:
+        if ex_traceback is not None:
             return False
 
 
 # class Time:
 #     """
 #     Stub for potential future time object
 #     """
```

### Comparing `ubelt-1.3.0/ubelt/util_time.pyi` & `ubelt-1.3.2/ubelt/util_time.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import datetime
+from typing import Type
+from types import TracebackType
 from _typeshed import Incomplete
 
 
 def timestamp(datetime: datetime.datetime | datetime.date | None = None,
               precision: int = 0,
               default_timezone: str | datetime.timezone = 'local',
               allow_dateutil: bool = True) -> str:
@@ -37,9 +39,11 @@
 
     def toc(self):
         ...
 
     def __enter__(self):
         ...
 
-    def __exit__(self, ex_type, ex_value, trace):
+    def __exit__(self, ex_type: Type[BaseException] | None,
+                 ex_value: BaseException | None,
+                 ex_traceback: TracebackType | None) -> bool | None:
         ...
```

### Comparing `ubelt-1.3.0/ubelt/util_zip.py` & `ubelt-1.3.2/ubelt/util_zip.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,24 @@
         if _handle is None:
             raise IOError('file {!r} does not exist'.format(fpath))
         self._handle = _handle
 
     def __enter__(self):
         return self
 
-    def __exit__(self, *args):
+    def __exit__(self, ex_type, ex_value, ex_traceback):
+        """
+        Args:
+            ex_type (Type[BaseException] | None):
+            ex_value (BaseException | None):
+            ex_traceback (TracebackType | None):
+
+        Returns:
+            bool | None
+        """
         self.close()
 
     # TODO: Allow for navigating inside of the zipfile
 
     # TODO: opening a member should not force disk decompression unless we
     # really need to do real seeks. If we are just streaming the first few
     # bytes, then a standard handle will work fine.
```

### Comparing `ubelt-1.3.0/ubelt/util_zip.pyi` & `ubelt-1.3.2/ubelt/util_zip.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Type
+from types import TracebackType
 from _typeshed import Incomplete
 from ubelt.util_mixins import NiceRepr
 
 
 def split_archive(fpath, ext: str = ...):
     ...
 
@@ -37,9 +39,11 @@
 
     def __del__(self) -> None:
         ...
 
     def __enter__(self):
         ...
 
-    def __exit__(self, *args) -> None:
+    def __exit__(self, ex_type: Type[BaseException] | None,
+                 ex_value: BaseException | None,
+                 ex_traceback: TracebackType | None) -> bool | None:
         ...
```

### Comparing `ubelt-1.3.0/ubelt.egg-info/PKG-INFO` & `ubelt-1.3.2/ubelt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubelt
-Version: 1.3.0
+Version: 1.3.2
 Summary: A Python utility belt containing simple tools, a stdlib like feel, and extra batteries.
 Home-page: https://github.com/Erotemic/ubelt
 Author: Jon Crall
 Author-email: erotemic@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ubelt-1.3.0/ubelt.egg-info/SOURCES.txt` & `ubelt-1.3.2/ubelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ubelt-1.3.0/ubelt.egg-info/requires.txt` & `ubelt-1.3.2/ubelt.egg-info/requires.txt`

 * *Files identical despite different names*

