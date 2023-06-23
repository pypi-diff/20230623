# Comparing `tmp/bob.bio.vein-5.0.0.tar.gz` & `tmp/bob.bio.vein-5.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.bio.vein-5.0.0.tar", last modified: Thu Jun 22 22:24:37 2023, max compression
+gzip compressed data, was "bob.bio.vein-5.0.1b0.tar", last modified: Fri Jun 23 19:45:16 2023, max compression
```

## Comparing `bob.bio.vein-5.0.0.tar` & `bob.bio.vein-5.0.1b0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.608967 bob.bio.vein-5.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-22 22:24:37.608967 bob.bio.vein-5.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.596967 bob.bio.vein-5.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/api.rst
--rw-rw-rw-   0 root         (0) root         (0)    11026 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/baselines.rst
--rw-rw-rw-   0 root         (0) root         (0)     7267 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2673 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/references.rst
--rw-rw-rw-   0 root         (0) root         (0)     1733 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/doc/resources.rst
--rw-rw-rw-   0 root         (0) root         (0)     3948 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 22:24:37.608967 bob.bio.vein-5.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.592967 bob.bio.vein-5.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.596967 bob.bio.vein-5.0.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.600967 bob.bio.vein-5.0.0/src/bob/bio/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.600967 bob.bio.vein-5.0.0/src/bob/bio/vein/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.600967 bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/
--rw-rw-rw-   0 root         (0) root         (0)     2331 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/Correlate.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/HammingDistance.py
--rw-rw-rw-   0 root         (0) root         (0)     4993 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/MiuraMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.600967 bob.bio.vein-5.0.0/src/bob/bio/vein/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:24:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.604967 bob.bio.vein-5.0.0/src/bob/bio/vein/config/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:24:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/database/utfvp_1vsall.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/database/utfvp_full.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/database/utfvp_nom.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/database/verafinger_contactless_nom.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/maximum_curvature.py
--rw-rw-rw-   0 root         (0) root         (0)     1748 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/principal_curvature.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/repeated_line_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/config/wide_line_detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.604967 bob.bio.vein-5.0.0/src/bob/bio/vein/database/
--rw-rw-rw-   0 root         (0) root         (0)      736 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/database/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/database/roi_annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     7298 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/database/utfvp.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/database/verafinger_contactless.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.604967 bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/
--rw-rw-rw-   0 root         (0) root         (0)    19120 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/MaximumCurvature.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/NormalisedCrossCorrelation.py
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/PrincipalCurvature.py
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/RepeatedLineTracking.py
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/WideLineDetector.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.608967 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3456 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/crop.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/filters.py
--rw-rw-rw-   0 root         (0) root         (0)    15126 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/normalize.py
--rw-rw-rw-   0 root         (0) root         (0)     3099 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/preprocessor.py
--rw-rw-rw-   0 root         (0) root         (0)    10532 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.608967 bob.bio.vein-5.0.0/src/bob/bio/vein/script/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 22:24:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4100 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/script/blame.py
--rw-rw-rw-   0 root         (0) root         (0)     6035 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/script/compare_rois.py
--rw-rw-rw-   0 root         (0) root         (0)     2832 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/script/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     7520 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/src/bob/bio/vein/script/view_sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.600967 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-22 22:24:37.000000 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2187 2023-06-22 22:24:37.000000 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 22:24:37.000000 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      915 2023-06-22 22:24:37.000000 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 22:24:37.000000 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      384 2023-06-22 22:24:37.000000 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-22 22:24:37.000000 bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 22:24:37.608967 bob.bio.vein-5.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7590 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/tests/test_databases.py
--rw-rw-rw-   0 root         (0) root         (0)    22670 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.0/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.295301 bob.bio.vein-5.0.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2366 2023-06-23 19:45:16.295301 bob.bio.vein-5.0.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-23 19:39:17.000000 bob.bio.vein-5.0.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.283301 bob.bio.vein-5.0.1b0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11026 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/baselines.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/references.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/doc/resources.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2023-06-23 19:39:17.000000 bob.bio.vein-5.0.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:45:16.295301 bob.bio.vein-5.0.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.279302 bob.bio.vein-5.0.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.283301 bob.bio.vein-5.0.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.283301 bob.bio.vein-5.0.1b0/src/bob/bio/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.283301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.287301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/Correlate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/HammingDistance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4993 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/MiuraMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.287301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:44:49.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.287301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:44:49.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/database/utfvp_1vsall.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/database/utfvp_full.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/database/utfvp_nom.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/database/verafinger_contactless_nom.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/maximum_curvature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/principal_curvature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/repeated_line_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/wide_line_detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.287301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/roi_annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7298 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/utfvp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/verafinger_contactless.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.291301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/
+-rw-rw-rw-   0 root         (0) root         (0)    19120 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/MaximumCurvature.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/NormalisedCrossCorrelation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/PrincipalCurvature.py
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/RepeatedLineTracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/WideLineDetector.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.291301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3456 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/crop.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    15126 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/normalize.py
+-rw-rw-rw-   0 root         (0) root         (0)     3099 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/preprocessor.py
+-rw-rw-rw-   0 root         (0) root         (0)    10532 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.291301 bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:44:49.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4100 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/blame.py
+-rw-rw-rw-   0 root         (0) root         (0)     6035 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/compare_rois.py
+-rw-rw-rw-   0 root         (0) root         (0)     2832 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7520 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/view_sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.283301 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2366 2023-06-23 19:45:16.000000 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-06-23 19:45:16.000000 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:45:16.000000 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      915 2023-06-23 19:45:16.000000 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:45:15.000000 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-23 19:45:16.000000 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 19:45:16.000000 bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:45:16.295301 bob.bio.vein-5.0.1b0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7590 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/tests/test_databases.py
+-rw-rw-rw-   0 root         (0) root         (0)    22670 2023-06-22 22:19:13.000000 bob.bio.vein-5.0.1b0/tests/test_tools.py
```

### Comparing `bob.bio.vein-5.0.0/COPYING` & `bob.bio.vein-5.0.1b0/COPYING`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/PKG-INFO` & `bob.bio.vein-5.0.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.bio.vein
-Version: 5.0.0
+Version: 5.0.1b0
 Summary: Vein Recognition Library
 Author-email: Andre Anjos <andre.anjos@idiap.ch>, Pedro Tome <pedro.tome@idiap.ch>
 License: GPLv3 License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.bio.vein/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.bio.vein
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.bio.vein/-/releases
 Keywords: bob,biometric recognition,evaluation,vein
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,17 +21,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v5.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/v5.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein/commits/v5.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/v5.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein)
 
 # Vein Recognition Library
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains resources for finger,
 palm and wrist vein recognition as
```

### Comparing `bob.bio.vein-5.0.0/README.md` & `bob.bio.vein-5.0.1b0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![badge doc](https://img.shields.io/badge/docs-v5.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/v5.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein/commits/v5.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/v5.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein)
 
 # Vein Recognition Library
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains resources for finger,
 palm and wrist vein recognition as
```

### Comparing `bob.bio.vein-5.0.0/doc/api.rst` & `bob.bio.vein-5.0.1b0/doc/api.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/doc/baselines.rst` & `bob.bio.vein-5.0.1b0/doc/baselines.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/doc/conf.py` & `bob.bio.vein-5.0.1b0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/doc/index.rst` & `bob.bio.vein-5.0.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/doc/installation.rst` & `bob.bio.vein-5.0.1b0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/doc/links.rst` & `bob.bio.vein-5.0.1b0/doc/links.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/doc/references.rst` & `bob.bio.vein-5.0.1b0/doc/references.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/doc/resources.rst` & `bob.bio.vein-5.0.1b0/doc/resources.rst`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/pyproject.toml` & `bob.bio.vein-5.0.1b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "bob.bio.vein"
-    version = "5.0.0"
+    version = "5.0.1b0"
     requires-python = ">=3.9"
     description = "Vein Recognition Library"
     dynamic = ["readme"]
     license = {text = "GPLv3 License"}
     authors = [
     {name = "Andre Anjos", email = "andre.anjos@idiap.ch"},
     {name = "Pedro Tome", email = "pedro.tome@idiap.ch"},
@@ -23,46 +23,46 @@
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "bob.io.base==5.1.0",
-        "bob.bio.base==8.0.0",
-        "clapper==1.0.1",
-        "docopt==0.6.2",
-        "matplotlib==3.6.2",
-        "numpy==1.23.5",
-        "pillow==9.4.0",
-        "schema==0.7.5",
-        "scikit-image==0.19.3",
-        "scipy==1.10.0",
+        "bob",
+        "bob.io.base",
+        "bob.bio.base",
+        "clapper",
+        "docopt",
+        "matplotlib",
+        "numpy",
+        "pillow",
+        "schema",
+        "scikit-image",
+        "scipy",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/sphinx/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/sphinx/"
     homepage = "https://pypi.org/project/bob.bio.vein/"
     repository = "https://gitlab.idiap.ch/bob/bob.bio.vein"
     changelog = "https://gitlab.idiap.ch/bob/bob.bio.vein/-/releases"
 
 [project.optional-dependencies]
     qa = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "auto-intersphinx==1.0.2",
-        "sphinxcontrib-programoutput==0.17",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
+        "auto-intersphinx",
+        "sphinxcontrib-programoutput",
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
@@ -115,11 +115,7 @@
     addopts = [
         "--import-mode=append",
         "--cov-report=term-missing",
         "--cov=bob.bio.vein",
     ]
     junit_logging = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/Correlate.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/Correlate.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/HammingDistance.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/HammingDistance.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/MiuraMatch.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/MiuraMatch.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/algorithm/__init__.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/config/maximum_curvature.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/maximum_curvature.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/config/principal_curvature.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/principal_curvature.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/config/repeated_line_tracking.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/repeated_line_tracking.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/config/wide_line_detector.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/config/wide_line_detector.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/database/__init__.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/database/database.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/database.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/database/roi_annotation.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/roi_annotation.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/database/utfvp.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/utfvp.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/database/verafinger_contactless.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/database/verafinger_contactless.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/MaximumCurvature.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/MaximumCurvature.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/NormalisedCrossCorrelation.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/NormalisedCrossCorrelation.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/PrincipalCurvature.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/PrincipalCurvature.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/RepeatedLineTracking.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/RepeatedLineTracking.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/extractor/WideLineDetector.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/extractor/WideLineDetector.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/__init__.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/crop.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/crop.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/filters.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/filters.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/mask.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/mask.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/normalize.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/normalize.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/preprocessor.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/preprocessor.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/preprocessor/utils.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/script/blame.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/blame.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/script/compare_rois.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/compare_rois.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/script/validate.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/validate.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob/bio/vein/script/view_sample.py` & `bob.bio.vein-5.0.1b0/src/bob/bio/vein/script/view_sample.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/PKG-INFO` & `bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.bio.vein
-Version: 5.0.0
+Version: 5.0.1b0
 Summary: Vein Recognition Library
 Author-email: Andre Anjos <andre.anjos@idiap.ch>, Pedro Tome <pedro.tome@idiap.ch>
 License: GPLv3 License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.bio.vein/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.bio.vein
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.bio.vein/-/releases
 Keywords: bob,biometric recognition,evaluation,vein
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,17 +21,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: COPYING
 
-[![badge doc](https://img.shields.io/badge/docs-v5.0.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/v5.0.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein/commits/v5.0.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/v5.0.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/v5.0.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.bio.vein/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.bio.vein/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.bio.vein)
 
 # Vein Recognition Library
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains resources for finger,
 palm and wrist vein recognition as
```

### Comparing `bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/SOURCES.txt` & `bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/src/bob.bio.vein.egg-info/entry_points.txt` & `bob.bio.vein-5.0.1b0/src/bob.bio.vein.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/tests/test_databases.py` & `bob.bio.vein-5.0.1b0/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `bob.bio.vein-5.0.0/tests/test_tools.py` & `bob.bio.vein-5.0.1b0/tests/test_tools.py`

 * *Files identical despite different names*

