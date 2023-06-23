# Comparing `tmp/bob.fusion.base-0.1.5.tar.gz` & `tmp/bob.fusion.base-0.1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.fusion.base-0.1.5.tar", last modified: Thu Jun 22 17:01:00 2023, max compression
+gzip compressed data, was "bob.fusion.base-0.1.6b0.tar", last modified: Fri Jun 23 20:02:59 2023, max compression
```

## Comparing `bob.fusion.base-0.1.5.tar` & `bob.fusion.base-0.1.6b0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.524584 bob.fusion.base-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2380 2023-06-22 17:01:00.524584 bob.fusion.base-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.516584 bob.fusion.base-0.1.5/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7373 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2928 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/doc/guide.rst
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/doc/py_api.rst
--rw-rw-rw-   0 root         (0) root         (0)     3616 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 17:01:00.524584 bob.fusion.base-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.512584 bob.fusion.base-0.1.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.516584 bob.fusion.base-0.1.5/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.520584 bob.fusion.base-0.1.5/src/bob/fusion/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.520584 bob.fusion.base-0.1.5/src/bob/fusion/base/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.520584 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/
--rw-rw-rw-   0 root         (0) root         (0)      959 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/AND.py
--rw-rw-rw-   0 root         (0) root         (0)     4802 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/Algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/AlgorithmBob.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/Empty.py
--rw-rw-rw-   0 root         (0) root         (0)     3013 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/GMM.py
--rw-rw-rw-   0 root         (0) root         (0)      668 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/Weighted_Sum.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.520584 bob.fusion.base-0.1.5/src/bob/fusion/base/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 17:00:37.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.520584 bob.fusion.base-0.1.5/src/bob/fusion/base/config/algorithm/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 17:00:37.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/config/algorithm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/config/algorithm/gmm.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/config/algorithm/llr_skl.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/config/algorithm/mean.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/config/algorithm/plr_2.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/config/algorithm/plr_3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.520584 bob.fusion.base-0.1.5/src/bob/fusion/base/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/preprocessor/Tanh.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/preprocessor/ZNorm.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/preprocessor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.524584 bob.fusion.base-0.1.5/src/bob/fusion/base/script/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6580 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/script/boundary.py
--rw-rw-rw-   0 root         (0) root         (0)    12560 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/script/fuse.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/script/fusion.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/script/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.524584 bob.fusion.base-0.1.5/src/bob/fusion/base/tools/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4685 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/tools/common.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/src/bob/fusion/base/tools/plotting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.520584 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2380 2023-06-22 17:01:00.000000 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1612 2023-06-22 17:01:00.000000 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:01:00.000000 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      850 2023-06-22 17:01:00.000000 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:01:00.000000 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-22 17:01:00.000000 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-22 17:01:00.000000 bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:01:00.524584 bob.fusion.base-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     8061 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/tests/test_algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/tests/test_preprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)     6716 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.5/tests/test_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.117547 bob.fusion.base-0.1.6b0/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-23 20:02:59.117547 bob.fusion.base-0.1.6b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-23 14:27:21.000000 bob.fusion.base-0.1.6b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.105547 bob.fusion.base-0.1.6b0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7373 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2928 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/doc/guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/doc/py_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3362 2023-06-23 19:53:47.000000 bob.fusion.base-0.1.6b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 20:02:59.117547 bob.fusion.base-0.1.6b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.101547 bob.fusion.base-0.1.6b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.105547 bob.fusion.base-0.1.6b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.109547 bob.fusion.base-0.1.6b0/src/bob/fusion/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.109547 bob.fusion.base-0.1.6b0/src/bob/fusion/base/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.109547 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/
+-rw-rw-rw-   0 root         (0) root         (0)      959 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/AND.py
+-rw-rw-rw-   0 root         (0) root         (0)     4802 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/Algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/AlgorithmBob.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/Empty.py
+-rw-rw-rw-   0 root         (0) root         (0)     3013 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/GMM.py
+-rw-rw-rw-   0 root         (0) root         (0)      668 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/Weighted_Sum.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.113547 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 20:02:29.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.113547 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/algorithm/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 20:02:29.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/algorithm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/algorithm/gmm.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/algorithm/llr_skl.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/algorithm/mean.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/algorithm/plr_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/config/algorithm/plr_3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.113547 bob.fusion.base-0.1.6b0/src/bob/fusion/base/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/preprocessor/Tanh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/preprocessor/ZNorm.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/preprocessor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.113547 bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6580 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/boundary.py
+-rw-rw-rw-   0 root         (0) root         (0)    12560 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/fuse.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/fusion.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.117547 bob.fusion.base-0.1.6b0/src/bob/fusion/base/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4685 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/tools/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/src/bob/fusion/base/tools/plotting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.109547 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-23 20:02:59.000000 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-23 20:02:59.000000 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:02:59.000000 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      850 2023-06-23 20:02:59.000000 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 20:02:58.000000 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-23 20:02:59.000000 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 20:02:59.000000 bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 20:02:59.117547 bob.fusion.base-0.1.6b0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     8061 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/tests/test_algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/tests/test_preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-06-22 16:57:46.000000 bob.fusion.base-0.1.6b0/tests/test_scripts.py
```

### Comparing `bob.fusion.base-0.1.5/COPYING` & `bob.fusion.base-0.1.6b0/COPYING`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/PKG-INFO` & `bob.fusion.base-0.1.6b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.fusion.base
-Version: 0.1.5
+Version: 0.1.6b0
 Summary: Score fusion in biometric and pad experiments
 Author-email: Amir Mohammadi <amir.mohammadi@idiap.ch>
 License: GPLv3 License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.fusion.base/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.fusion.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.fusion.base/-/releases
 Keywords: bob,score fusion,evaluation,biometric
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,17 +19,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v0.1.5-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/v0.1.5/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base/commits/v0.1.5)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/v0.1.5/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base)
 
 # Score Fusion in Biometric Recognition and Presentation Attack Detection
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It runs score fusion in biometric and
 presentation attack detection experiments using various algorithms. It provides
```

### Comparing `bob.fusion.base-0.1.5/README.md` & `bob.fusion.base-0.1.6b0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![badge doc](https://img.shields.io/badge/docs-v0.1.5-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/v0.1.5/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base/commits/v0.1.5)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/v0.1.5/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base)
 
 # Score Fusion in Biometric Recognition and Presentation Attack Detection
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It runs score fusion in biometric and
 presentation attack detection experiments using various algorithms. It provides
```

### Comparing `bob.fusion.base-0.1.5/doc/conf.py` & `bob.fusion.base-0.1.6b0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/doc/guide.rst` & `bob.fusion.base-0.1.6b0/doc/guide.rst`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/doc/index.rst` & `bob.fusion.base-0.1.6b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/doc/py_api.rst` & `bob.fusion.base-0.1.6b0/doc/py_api.rst`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/pyproject.toml` & `bob.fusion.base-0.1.6b0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "bob.fusion.base"
-    version = "0.1.5"
+    version = "0.1.6b0"
     requires-python = ">=3.9"
     description = "Score fusion in biometric and pad experiments"
     dynamic = ["readme"]
     license = {text = "GPLv3 License"}
     authors = [
     {name = "Amir Mohammadi", email = "amir.mohammadi@idiap.ch"},
     ]
@@ -20,44 +20,44 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "bob.measure==6.1.0",
-        "bob.learn.em==3.3.0",
-        "bob.bio.base==8.0.0",
-        "clapper==1.0.1",
-        "matplotlib==3.6.2",
-        "numpy==1.23.5",
-        "scikit-learn==1.1.2",
+        "bob",
+        "bob.measure",
+        "bob.learn.em",
+        "bob.bio.base",
+        "clapper",
+        "matplotlib",
+        "numpy",
+        "scikit-learn",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/sphinx/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/sphinx/"
     homepage      = "https://pypi.org/project/bob.fusion.base/"
     repository    = "https://gitlab.idiap.ch/bob/bob.fusion.base"
     changelog     = "https://gitlab.idiap.ch/bob/bob.fusion.base/-/releases"
 
 [project.optional-dependencies]
     qa = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "auto-intersphinx==1.0.2",
-        "sphinxcontrib-programoutput==0.17",
-        "bob.pad.base==6.0.0",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
+        "auto-intersphinx",
+        "sphinxcontrib-programoutput",
+        "bob.pad.base",
         ]
     test = [
-        "pytest==7.2.1",
-        "pytest-cov==4.0.0",
-        "coverage==7.0.5",
+        "pytest",
+        "pytest-cov",
+        "coverage",
         ]
 
 [tool.setuptools]
     zip-safe = false
     package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
@@ -102,11 +102,7 @@
     addopts = [
         "--import-mode=append",
         "--cov-report=term-missing",
         "--cov=bob.fusion.base",
     ]
     junit_logging = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/AND.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/AND.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/Algorithm.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/Algorithm.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/AlgorithmBob.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/AlgorithmBob.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/GMM.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/GMM.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/Weighted_Sum.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/Weighted_Sum.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/algorithm/__init__.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/preprocessor/Tanh.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/preprocessor/Tanh.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/preprocessor/ZNorm.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/preprocessor/ZNorm.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/preprocessor/__init__.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/script/boundary.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/boundary.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/script/fuse.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/fuse.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/script/resource.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/script/resource.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/tools/common.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/tools/common.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob/fusion/base/tools/plotting.py` & `bob.fusion.base-0.1.6b0/src/bob/fusion/base/tools/plotting.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/PKG-INFO` & `bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.fusion.base
-Version: 0.1.5
+Version: 0.1.6b0
 Summary: Score fusion in biometric and pad experiments
 Author-email: Amir Mohammadi <amir.mohammadi@idiap.ch>
 License: GPLv3 License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.fusion.base/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.fusion.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.fusion.base/-/releases
 Keywords: bob,score fusion,evaluation,biometric
 Classifier: Framework :: Bob
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,17 +19,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v0.1.5-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/v0.1.5/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base/commits/v0.1.5)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/v0.1.5/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/v0.1.5/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.fusion.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.fusion.base/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.fusion.base)
 
 # Score Fusion in Biometric Recognition and Presentation Attack Detection
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It runs score fusion in biometric and
 presentation attack detection experiments using various algorithms. It provides
```

### Comparing `bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/SOURCES.txt` & `bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/src/bob.fusion.base.egg-info/entry_points.txt` & `bob.fusion.base-0.1.6b0/src/bob.fusion.base.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/tests/test_algorithm.py` & `bob.fusion.base-0.1.6b0/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/tests/test_preprocessor.py` & `bob.fusion.base-0.1.6b0/tests/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `bob.fusion.base-0.1.5/tests/test_scripts.py` & `bob.fusion.base-0.1.6b0/tests/test_scripts.py`

 * *Files identical despite different names*

