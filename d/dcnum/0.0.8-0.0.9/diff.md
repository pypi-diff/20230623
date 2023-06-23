# Comparing `tmp/dcnum-0.0.8.tar.gz` & `tmp/dcnum-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.8.tar", last modified: Wed Jun 21 21:09:59 2023, max compression
+gzip compressed data, was "dcnum-0.0.9.tar", last modified: Fri Jun 23 09:35:12 2023, max compression
```

## Comparing `dcnum-0.0.8.tar` & `dcnum-0.0.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.576246 dcnum-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.564245 dcnum-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 21:09:46.000000 dcnum-0.0.8/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 21:09:46.000000 dcnum-0.0.8/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-21 21:09:46.000000 dcnum-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 21:09:46.000000 dcnum-0.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-21 21:09:46.000000 dcnum-0.0.8/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-21 21:09:46.000000 dcnum-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 21:09:59.576246 dcnum-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 21:09:46.000000 dcnum-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-21 21:09:46.000000 dcnum-0.0.8/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.568245 dcnum-0.0.8/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 21:09:59.000000 dcnum-0.0.8/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.572245 dcnum-0.0.8/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 21:09:46.000000 dcnum-0.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 21:09:46.000000 dcnum-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:09:59.576246 dcnum-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.576246 dcnum-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:09:59.576246 dcnum-0.0.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-21 21:09:46.000000 dcnum-0.0.8/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.006134 dcnum-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.994125 dcnum-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.994125 dcnum-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-23 09:34:54.000000 dcnum-0.0.9/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-23 09:34:54.000000 dcnum-0.0.9/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-23 09:34:54.000000 dcnum-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-23 09:34:54.000000 dcnum-0.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-23 09:34:54.000000 dcnum-0.0.9/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 09:34:54.000000 dcnum-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 09:35:12.006134 dcnum-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-23 09:34:54.000000 dcnum-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.994125 dcnum-0.0.9/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-23 09:34:54.000000 dcnum-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:35:12.006134 dcnum-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.006134 dcnum-0.0.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_write_writer.py
```

### Comparing `dcnum-0.0.8/.github/workflows/check.yml` & `dcnum-0.0.9/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/.github/workflows/deploy_pypi.yml` & `dcnum-0.0.9/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/.gitignore` & `dcnum-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/CHANGELOG` & `dcnum-0.0.9/CHANGELOG`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.0.9
+ - fix: properly propagate event extraction keyword arguments
+ - fix: QueueCollectorThread used uint16 for enumerating indices
+ - fix: handle case where number of events is not multiple of chunk_size
+ - enh: reduce thread waiting times
+ - enh: add bounds check for image cache
 0.0.8
  - feat: introduce QueueCollectorThread
  - feat: introduce SegmenterManagerThread
  - feat: instroduce EventExtractorManagerThread and corresponding workers
  - enh: minor improvements for HDF5ImageCache and ImageCorrCache
  - enh: use data size as cache size if smaller than requested chunk size
  - enh: return dictionary for brightness feature computation
```

### Comparing `dcnum-0.0.8/LICENSE` & `dcnum-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/PKG-INFO` & `dcnum-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.8
+Version: 0.0.9
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.8/README.rst` & `dcnum-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.0.9/dcnum/feat/event_extractor_manager_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,34 +94,34 @@
                     break
                 else:
                     unavailable_slots += 1
                     cur_slot = (cur_slot + 1) % num_slots
                 if unavailable_slots >= num_slots:
                     # There is nothing to do, try to avoid 100% CPU
                     unavailable_slots = 0
-                    time.sleep(.1)
+                    time.sleep(.01)
 
             # We have a chunk, process it!
             chunk = self.slot_chunks[cur_slot]
             # Populate the labeling array for the workers
             new_labels = self.labels_list[cur_slot]
             if len(new_labels) == self.label_array.shape[0]:
                 self.label_array[:] = new_labels
             elif len(new_labels) < self.label_array.shape[0]:
                 self.label_array[:len(new_labels)] = new_labels
                 self.label_array[len(new_labels):] = 0
             else:
                 raise ValueError("labels_list contains bad size data!")
             # Let the workers know there is work
-            for ii in range(self.data.image.chunk_size):
+            for ii in range(self.data.image.get_chunk_size(chunk)):
                 self.raw_queue.put((chunk, ii))
 
             # Make sure the entire chunk has been processed.
             while self.raw_queue.qsize():
-                time.sleep(.1)
+                time.sleep(.01)
 
             # We are done here. The segmenter may continue its deed.
             self.slot_states[cur_slot] = "w"
 
             self.logger.debug(f"Extracted one chunk: {chunk}")
 
             chunks_processed += 1
```

### Comparing `dcnum-0.0.8/dcnum/feat/feat_background/base.py` & `dcnum-0.0.9/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.0.9/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
                 # prepend output size to arguments
                 args = (output_size, job_slice)
                 self.queue.put(args)
                 num_jobs += 1
 
             # block until workers are done
             while True:
-                time.sleep(.01)
+                time.sleep(.03)
                 if self.worker_counter.value == num_jobs:
                     break
 
             # Write output data to HDF5 file
             # TODO:
             #  Do this in a different thread so workers can keep going
             #  and use a lock somewhere in case the disk is too slow.
```

### Comparing `dcnum-0.0.8/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.0.9/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.0.9/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.0.9/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.0.9/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/feat/gate.py` & `dcnum-0.0.9/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/feat/queue_event_extractor.py` & `dcnum-0.0.9/dcnum/feat/queue_event_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,16 @@
         if self.preselect:
             # TODO: Do this before segmentation already?
             ptp = np.ptp(self.data.image_corr[index])
             if ptp < 0.1 * self.ptp_median:
                 return None
         masks = self.get_masks_from_label(label)
         if masks.size:
-            events = self.get_events_from_masks(masks=masks, data_index=index)
+            events = self.get_events_from_masks(
+                masks=masks, data_index=index, **self.extract_kwargs)
         else:
             events = None
         return events
 
     def run(self):
         """Main loop of worker process"""
         # Don't wait for queues when joining workers
```

### Comparing `dcnum-0.0.8/dcnum/meta/ppid.py` & `dcnum-0.0.9/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/read/cache.py` & `dcnum-0.0.9/dcnum/read/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,41 +36,55 @@
         self.image_shape = self.shape[1:]
         self.chunk_shape = (chunk_size,) + self.shape[1:]
         self._len = self.shape[0]
         self.num_chunks = int(np.ceil(self._len / self.chunk_size))
 
     def _get_chunk_index_for_index(self, index):
         if index < 0:
-            index = len(self.h5ds) + index
+            index = self._len + index
+        elif index >= self._len:
+            raise IndexError(
+                f"Index {index} out of bounds for HDF5ImageCache "
+                f"of size {self._len}")
         chunk_index = index // self.chunk_size
         sub_index = index % self.chunk_size
         return chunk_index, sub_index
 
     def __getitem__(self, index):
         chunk_index, sub_index = self._get_chunk_index_for_index(index)
         return self.get_chunk(chunk_index)[sub_index]
 
     def __len__(self):
         return self._len
 
     def get_chunk(self, chunk_index):
-        """Get one chunk of images"""
+        """Return one chunk of images"""
         if chunk_index not in self.cache:
             fslice = slice(self.chunk_size * chunk_index,
                            self.chunk_size * (chunk_index + 1)
                            )
             data = self.h5ds[fslice]
             if self.boolean:
                 data = np.array(data, dtype=bool)
             self.cache[chunk_index] = data
             if len(self.cache) > self.cache_size:
                 # Remove the first item
                 self.cache.popitem(last=False)
         return self.cache[chunk_index]
 
+    def get_chunk_size(self, chunk_index):
+        """Return the number of images in this chunk"""
+        if chunk_index < self.num_chunks - 1:
+            return self.chunk_size
+        else:
+            chunk_size = self._len - chunk_index*self.chunk_size
+            if chunk_size < 0:
+                raise IndexError(f"{self} only has {self.num_chunks} chunks!")
+            return chunk_size
+
     def iter_chunks(self):
         size = self.h5ds.shape[0]
         index = 0
         chunk = 0
         while True:
             yield chunk
             chunk += 1
```

### Comparing `dcnum-0.0.8/dcnum/read/hdf5_data.py` & `dcnum-0.0.9/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/segm/segm_thresh.py` & `dcnum-0.0.9/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/segm/segmenter.py` & `dcnum-0.0.9/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum/segm/segmenter_cpu.py` & `dcnum-0.0.9/dcnum/segm/segmenter_cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 import multiprocessing as mp
-import os
+# import os
 import time
 import threading
 
 import numpy as np
 
 from .segmenter import Segmenter
 
@@ -185,15 +185,15 @@
         self.mp_batch_index.value += 1
 
         # Tell workers to get going
         self.mp_batch_worker.value = 0
 
         # Wait for all workers to complete
         while self.mp_batch_worker.value != num_workers:
-            time.sleep(.1)
+            time.sleep(.01)
 
         return self._mp_labels_np
 
 
 class CPUSegmenterWorker:
     def __init__(self,
                  segmenter,
@@ -229,15 +229,15 @@
         self.labels_data_raw = segmenter.mp_labels_raw
         # The shape of one image
         self.image_shape = segmenter.image_shape
         self.sl_start = sl_start
         self.sl_stop = sl_stop
 
     def run(self):
-        print(f"Running {self} in PID {os.getpid()}")
+        # print(f"Running {self} in PID {os.getpid()}")
         # We have to create the numpy-versions of the mp.RawArrays here,
         # otherwise we only get some kind of copy in the new process
         # when we use "spawn" instead of "fork".
         labels_data = np.ctypeslib.as_array(self.labels_data_raw).reshape(
             -1, self.image_shape[0], self.image_shape[1])
         image_data = np.ctypeslib.as_array(self.image_data_raw).reshape(
             -1, self.image_shape[0], self.image_shape[1])
@@ -257,15 +257,15 @@
                     labels_data[idx, :, :] = self.segmenter.segment_frame(
                         image_data[idx])
                     idx += 1
             elif self.shutdown.value:
                 break
             else:
                 # Wait for more data to arrive
-                time.sleep(.03)
+                time.sleep(.01)
 
 
 class CPUSegmenterWorkerProcess(CPUSegmenterWorker, mp.Process):
     def __init__(self, *args, **kwargs):
         super(CPUSegmenterWorkerProcess, self).__init__(*args, **kwargs)
```

### Comparing `dcnum-0.0.8/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.0.9/dcnum/segm/segmenter_manager_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                     break
                 else:
                     empty_slots += 1
                     cur_slot = (cur_slot + 1) % num_slots
                 if empty_slots >= num_slots:
                     # There is nothing to do, try to avoid 100% CPU
                     empty_slots = 0
-                    time.sleep(.1)
+                    time.sleep(.01)
 
             # We have a free slot to compute the segmentation
             labels = self.segmenter.segment_chunk(
                 image_data=self.image_data,
                 chunk=chunk,
                 debug=self.debug)
```

### Comparing `dcnum-0.0.8/dcnum/write/deque_writer_thread.py` & `dcnum-0.0.9/dcnum/write/deque_writer_thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,9 +44,9 @@
             elif len(self.dq):
                 feat, data = self.dq.popleft()
                 self.writer.store_feature_chunk(feat=feat, data=data)
             elif self.may_stop_loop:
                 break
             else:
                 # wait for the next item to arrive
-                time.sleep(.5)
+                time.sleep(.1)
         self.writer.close()
```

### Comparing `dcnum-0.0.8/dcnum/write/queue_collector_thread.py` & `dcnum-0.0.9/dcnum/write/queue_collector_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.size = int(np.sum(feat_nevents))
         #: Number of frames in this stash
         self.num_frames = len(feat_nevents)
         #: Global offset compared to the original data instance.
         self.index_offset = index_offset
         #: Array containing the indices in the original data instance
         #: that correspond to the events in `events`.
-        self.indices_for_data = np.zeros(self.size, dtype=np.uint16)
+        self.indices_for_data = np.zeros(self.size, dtype=np.uint32)
         # Private array that tracks the progress.
         self._tracker = np.zeros(self.num_frames, dtype=bool)
 
     def is_complete(self):
         """Determine whether the event stash is complete (all events added)"""
         return np.all(self._tracker)
 
@@ -175,15 +175,15 @@
         while True:
             # Slice of the shared nevents array. If it contains -1 values,
             # this means that some of the frames have not yet been processed.
             cur_nevents = self.feat_nevents[
                           cur_frame:cur_frame + self.write_threshold]
             if np.any(np.array(cur_nevents) < 0):
                 # We are not yet ready to write any new data to the queue.
-                time.sleep(.1)
+                time.sleep(.01)
                 continue
 
             if len(cur_nevents) == 0:
                 self.logger.warning("Encountered empty nevents array!")
                 break
 
             # We have reached the writer threshold. This means the extractor
@@ -252,14 +252,13 @@
             self.writer_dq.append(("image_bg", bgdat))
 
             # Write the number of events.
             self.writer_dq.append(("nevents",
                                    np.array(stash.feat_nevents)[
                                        indices - stash.index_offset]
                                    ))
-
             # Update events/frames written (used for monitoring)
             self.written_events += stash.size
             self.written_frames += stash.num_frames
 
             # Increment current frame index.
             cur_frame += self.write_threshold
```

### Comparing `dcnum-0.0.8/dcnum/write/writer.py` & `dcnum-0.0.9/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/dcnum.egg-info/PKG-INFO` & `dcnum-0.0.9/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.8
+Version: 0.0.9
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.8/dcnum.egg-info/SOURCES.txt` & `dcnum-0.0.9/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/docs/conf.py` & `dcnum-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/docs/extensions/github_changelog.py` & `dcnum-0.0.9/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/pyproject.toml` & `dcnum-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/helper_methods.py` & `dcnum-0.0.9/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.0.9/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_feat_brightness.py` & `dcnum-0.0.9/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_feat_haralick.py` & `dcnum-0.0.9/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_feat_moments_based.py` & `dcnum-0.0.9/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_ppid.py` & `dcnum-0.0.9/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_read_concat_hdf5.py` & `dcnum-0.0.9/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_read_hdf5.py` & `dcnum-0.0.9/tests/test_read_hdf5.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,14 +44,49 @@
         assert np.allclose(hic[140], h5["events/image"][140])
         assert len(hic.cache) == 2  # limited to two
         assert 0 not in hic.cache  # first item gets removed
         assert 1 in hic.cache
         assert 2 in hic.cache
 
 
+def test_image_cache_index_out_of_range(tmp_path):
+    path = tmp_path / "test.hdf5"
+    size = 20
+    chunk_size = 8
+    with h5py.File(path, "w") as hw:
+        hw["events/image"] = np.random.rand(size, 80, 180)
+    with h5py.File(path, "r") as h5:
+        hic = read.HDF5ImageCache(h5["events/image"],
+                                  chunk_size=chunk_size,
+                                  cache_size=2)
+        # Get something from first chunk. This should just work
+        hic.__getitem__(10)
+        # Now test out-of-bounds error
+        with pytest.raises(IndexError, match="of bounds for HDF5ImageCache"):
+            hic.__getitem__(20)
+
+
+def test_image_chache_get_chunk_size(tmp_path):
+    path = tmp_path / "test.hdf5"
+    size = 20
+    chunk_size = 8
+    with h5py.File(path, "w") as hw:
+        hw["events/image"] = np.random.rand(size, 80, 180)
+    with h5py.File(path, "r") as h5:
+        hic = read.HDF5ImageCache(h5["events/image"],
+                                  chunk_size=chunk_size,
+                                  cache_size=2)
+        # Get something from first chunk. This should just work
+        assert hic.get_chunk_size(0) == 8
+        assert hic.get_chunk_size(1) == 8
+        assert hic.get_chunk_size(2) == 4
+        with pytest.raises(IndexError, match="only has 3 chunks"):
+            hic.get_chunk_size(3)
+
+
 @pytest.mark.parametrize("size, chunks", [(209, 21),
                                           (210, 21),
                                           (211, 22)])
 def test_image_cache_iter_chunks(size, chunks, tmp_path):
     path = tmp_path / "test.hdf5"
     with h5py.File(path, "w") as hw:
         hw["events/image"] = np.random.rand(size, 80, 180)
```

### Comparing `dcnum-0.0.8/tests/test_segm_thresh.py` & `dcnum-0.0.9/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_write_deque_writer_thread.py` & `dcnum-0.0.9/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.8/tests/test_write_writer.py` & `dcnum-0.0.9/tests/test_write_writer.py`

 * *Files identical despite different names*

