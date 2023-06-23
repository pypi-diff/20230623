# Comparing `tmp/pymchelper-2.5.0.tar.gz` & `tmp/pymchelper-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymchelper-2.5.0.tar", last modified: Sun Jun 11 21:01:23 2023, max compression
+gzip compressed data, was "pymchelper-2.5.1.tar", last modified: Fri Jun 23 13:19:40 2023, max compression
```

## Comparing `pymchelper-2.5.0.tar` & `pymchelper-2.5.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.997996 pymchelper-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-11 21:00:43.000000 pymchelper-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-11 21:01:22.997996 pymchelper-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-11 21:00:43.000000 pymchelper-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/executor/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/executor/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/flair/
--rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper/flair/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/bmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/csg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/fortran.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/common/rexx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/flair/db/
--rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/db/card.db
--rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/db/card.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/flair/db/db2ini.r
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/input_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/fluka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/readers/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/binary_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2016.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bin2010.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/shieldhit/detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/detector_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/estimator_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/fortran_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/detector/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/shieldhit/particle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/mcscripter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.993995 pymchelper-2.5.0/pymchelper/utils/radiotherapy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/radiotherapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/radiotherapy/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/utils/runmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.997996 pymchelper-2.5.0/pymchelper/writers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/fortranformatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/mcpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/shieldhit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/trip98cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/trip98ddd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-11 21:00:43.000000 pymchelper-2.5.0/pymchelper/writers/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:01:22.989995 pymchelper-2.5.0/pymchelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 21:01:22.000000 pymchelper-2.5.0/pymchelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-11 21:01:22.997996 pymchelper-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-11 21:00:43.000000 pymchelper-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 13:19:08.000000 pymchelper-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-23 13:19:40.740245 pymchelper-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-23 13:19:08.000000 pymchelper-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/executor/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/executor/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/flair/
+-rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/flair/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/bmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/csg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/rexx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/flair/db/
+-rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/db/card.db
+-rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/db/card.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/db/db2ini.r
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/fluka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/readers/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/binary_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bin2010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/shieldhit/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/detector_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/estimator_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/fortran_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/particle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/mcscripter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/utils/radiotherapy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/radiotherapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/radiotherapy/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/runmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/fortranformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/mcpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/shieldhit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/trip98cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/trip98ddd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-23 13:19:40.740245 pymchelper-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-23 13:19:09.000000 pymchelper-2.5.1/setup.py
```

### Comparing `pymchelper-2.5.0/PKG-INFO` & `pymchelper-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.5.0/README.md` & `pymchelper-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/__init__.py` & `pymchelper-2.5.1/pymchelper/__init__.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/axis.py` & `pymchelper-2.5.1/pymchelper/axis.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/estimator.py` & `pymchelper-2.5.1/pymchelper/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 from enum import IntEnum
 import logging
+from typing import Optional
 
 import numpy as np
 from pymchelper.axis import MeshAxis, AxisId
 
 logger = logging.getLogger(__name__)
 
 
@@ -77,15 +78,15 @@
         :param page:
         :return: None
         """
         new_page = copy.deepcopy(page)
         new_page.estimator = self
         self.pages += (new_page,)
 
-    def axis(self, axis_id):
+    def axis(self, axis_id : int) -> Optional[MeshAxis]:
         """
         Mesh axis selector method based on integer id's.
 
         Instead of getting mesh axis data by calling `d.x`, `d.y` or `d.z` (assuming `d` an object of `Detector`
         class) we can get that data by calling `d.axis(0)`, `d.axis(1)` or `d.axis(2)`. See for example:
         >>> d = Estimator()
         >>> d.x = MeshAxis(n=2, min_val=0.0, max_val=10.0, name="X", unit="cm", binning=MeshAxis.BinningType.linear)
```

### Comparing `pymchelper-2.5.0/pymchelper/executor/options.py` & `pymchelper-2.5.1/pymchelper/executor/options.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/executor/runner.py` & `pymchelper-2.5.1/pymchelper/executor/runner.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/Data.py` & `pymchelper-2.5.1/pymchelper/flair/Data.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/Input.py` & `pymchelper-2.5.1/pymchelper/flair/Input.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/common/bmath.py` & `pymchelper-2.5.1/pymchelper/flair/common/bmath.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/common/csg.py` & `pymchelper-2.5.1/pymchelper/flair/common/csg.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/common/fortran.py` & `pymchelper-2.5.1/pymchelper/flair/common/fortran.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/common/log.py` & `pymchelper-2.5.1/pymchelper/flair/common/log.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/common/rexx.py` & `pymchelper-2.5.1/pymchelper/flair/common/rexx.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/db/card.db` & `pymchelper-2.5.1/pymchelper/flair/db/card.db`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/db/card.ini` & `pymchelper-2.5.1/pymchelper/flair/db/card.ini`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/flair/db/db2ini.r` & `pymchelper-2.5.1/pymchelper/flair/db/db2ini.r`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/input_output.py` & `pymchelper-2.5.1/pymchelper/input_output.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 from collections import defaultdict
 from glob import glob
+from typing import Optional
 
 import numpy as np
 
 from pymchelper.estimator import ErrorEstimate, Estimator, average_with_nan
 from pymchelper.readers.fluka import FlukaReader, FlukaReaderFactory
 from pymchelper.readers.shieldhit.general import SHReaderFactory
 from pymchelper.readers.shieldhit.reader_base import SHReader
@@ -40,28 +41,29 @@
     """
     corename = FlukaReader(filename).corename
     if corename is None:
         corename = SHReader(filename).corename
     return corename
 
 
-def fromfile(filename: str):
+def fromfile(filename: str) -> Optional[Estimator]:
     """Read estimator data from a binary file ```filename```"""
 
     reader = guess_reader(filename)
     if reader is None:
         raise Exception("File format not compatible", filename)
     estimator = Estimator()
     estimator.file_counter = 1
     if not reader.read(estimator):  # some problems occurred during read
+        logger.error("Error reading file %s", filename)
         estimator = None
     return estimator
 
 
-def fromfilelist(input_file_list, error=ErrorEstimate.stderr, nan: bool = True):
+def fromfilelist(input_file_list, error: ErrorEstimate = ErrorEstimate.stderr, nan: bool = True) -> Optional[Estimator]:
     """
     Reads all files from a given list, and returns a list of averaged estimators.
 
     :param input_file_list: list of files to be read
     :param error: error estimation, see class ErrorEstimate class in pymchelper.estimator
     :param nan: if True, NaN (not a number) are excluded when averaging data.
     :return: list of estimators
@@ -89,28 +91,34 @@
             for page in result.pages:
                 page.error_raw = np.zeros_like(page.data_raw)
 
         # loop over all files with n running from 2
         for n, filename in enumerate(input_file_list[1:], start=2):
             current_estimator = fromfile(filename)  # x
 
-            # Running variance algorithm based on algorithm by B. P. Welford,
-            # presented in Donald Knuth's Art of Computer Programming, Vol 2, page 232, 3rd edition.
-            # Can be found here: http://www.johndcook.com/blog/standard_deviation/
-            # and https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Online_algorithm
-            delta = [
-                current_page.data_raw - result_page.data_raw
-                for current_page, result_page in zip(current_estimator.pages, result.pages)
-            ]  # delta = x - mean
-            for page, delta_item in zip(result.pages, delta):
-                page.data_raw += delta_item / np.float64(n)
-
-            if error != ErrorEstimate.none:
-                for page, delta_item, current_page in zip(result.pages, delta, current_estimator.pages):
-                    page.error_raw += delta_item * (current_page.data_raw - page.data_raw)  # M2 += delta * (x - mean)
+            if not current_estimator:
+                logger.warning("File %s could not be read", filename)
+                return None
+
+            for current_page, result_page in zip(current_estimator.pages, result.pages):
+                # got a page with "concatenate normalisation"
+                if getattr(current_page, 'page_normalized', 2) == 4:
+                    logger.info("Concatenating page %s", current_page.name)
+                    result_page.data_raw = np.concatenate((result_page.data_raw, current_page.data_raw))
+                else:
+                    logger.info("Averaging page %s", current_page.name)
+                    # Running variance algorithm based on algorithm by B. P. Welford,
+                    # presented in Donald Knuth's Art of Computer Programming, Vol 2, page 232, 3rd edition.
+                    # Can be found here: http://www.johndcook.com/blog/standard_deviation/
+                    # and https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Online_algorithm
+                    delta = current_page.data_raw - result_page.data_raw  # delta = x - mean
+                    result_page.data_raw += delta / np.float64(n)
+                    if error != ErrorEstimate.none:
+                        # the line below is equivalent to M2 += delta * (x - mean)
+                        result_page.error_raw += delta * (current_page.data_raw - result_page.data_raw)
 
         # unbiased sample variance is stored in `__M2 / (n - 1)`
         # unbiased sample standard deviation in classical algorithm is calculated as (sqrt(1/(n-1)sum(x-<x>)**2)
         # here it is calculated as square root of unbiased sample variance:
         if len(input_file_list) > 1 and error != ErrorEstimate.none:
             for page in result.pages:
                 page.error_raw = np.sqrt(page.error_raw / (len(input_file_list) - 1.0))
@@ -126,15 +134,15 @@
     core_names_dict = group_input_files(input_file_list)
     if len(core_names_dict) == 1:
         result.file_corename = list(core_names_dict)[0]
 
     return result
 
 
-def frompattern(pattern, error=ErrorEstimate.stderr, nan=True):
+def frompattern(pattern: str, error: ErrorEstimate = ErrorEstimate.stderr, nan: bool = True):
     """
     Reads all files matching pattern, e.g.: 'foobar_*.bdo', and returns a list of averaged estimators.
 
     :param pattern: pattern to be matched for reading.
     :param error: error estimation, see class ErrorEstimate class in pymchelper.estimator
     :param nan: if True, NaN (not a number) are excluded when averaing data.
     :return: a list of estimators, or an empty list if no files were found.
@@ -172,20 +180,15 @@
         output_path = estimator.file_corename
     else:
         output_path = os.path.join(outputdir, estimator.file_corename)
     status = tofile(estimator, output_path, converter_name, options)
     return status
 
 
-def convertfrompattern(pattern,
-                       outputdir,
-                       converter_name,
-                       options,
-                       error=ErrorEstimate.stderr,
-                       nan: bool = True):
+def convertfrompattern(pattern, outputdir, converter_name, options, error=ErrorEstimate.stderr, nan: bool = True):
     """
 
     :param pattern:
     :param outputdir:
     :param converter_name:
     :param options:
     :param error: error estimation, see class ErrorEstimate class in pymchelper.estimator
```

### Comparing `pymchelper-2.5.0/pymchelper/page.py` & `pymchelper-2.5.1/pymchelper/page.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/common.py` & `pymchelper-2.5.1/pymchelper/readers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/fluka.py` & `pymchelper-2.5.1/pymchelper/readers/fluka.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/shieldhit/binary_spec.py` & `pymchelper-2.5.1/pymchelper/readers/shieldhit/binary_spec.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/shieldhit/general.py` & `pymchelper-2.5.1/pymchelper/readers/shieldhit/general.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_base.py` & `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_base.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2016.py` & `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2016.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bdo2019.py` & `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2019.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/readers/shieldhit/reader_bin2010.py` & `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bin2010.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/run.py` & `pymchelper-2.5.1/pymchelper/run.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/shieldhit/detector/detector_type.py` & `pymchelper-2.5.1/pymchelper/shieldhit/detector/detector_type.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/shieldhit/detector/estimator.py` & `pymchelper-2.5.1/pymchelper/shieldhit/detector/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/shieldhit/detector/fortran_card.py` & `pymchelper-2.5.1/pymchelper/shieldhit/detector/fortran_card.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/shieldhit/detector/geometry.py` & `pymchelper-2.5.1/pymchelper/shieldhit/detector/geometry.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/shieldhit/particle.py` & `pymchelper-2.5.1/pymchelper/shieldhit/particle.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/utils/mcscripter.py` & `pymchelper-2.5.1/pymchelper/utils/mcscripter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/utils/radiotherapy/plan.py` & `pymchelper-2.5.1/pymchelper/utils/radiotherapy/plan.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/utils/runmc.py` & `pymchelper-2.5.1/pymchelper/utils/runmc.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/version.py` & `pymchelper-2.5.1/pymchelper/version.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/common.py` & `pymchelper-2.5.1/pymchelper/writers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/excel.py` & `pymchelper-2.5.1/pymchelper/writers/excel.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/fortranformatter.py` & `pymchelper-2.5.1/pymchelper/writers/fortranformatter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/hdf.py` & `pymchelper-2.5.1/pymchelper/writers/hdf.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/inspector.py` & `pymchelper-2.5.1/pymchelper/writers/inspector.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/json.py` & `pymchelper-2.5.1/pymchelper/writers/json.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/mcpl.py` & `pymchelper-2.5.1/pymchelper/writers/mcpl.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/plots.py` & `pymchelper-2.5.1/pymchelper/writers/plots.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/shieldhit.py` & `pymchelper-2.5.1/pymchelper/writers/shieldhit.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/sparse.py` & `pymchelper-2.5.1/pymchelper/writers/sparse.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/trip98cube.py` & `pymchelper-2.5.1/pymchelper/writers/trip98cube.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/trip98ddd.py` & `pymchelper-2.5.1/pymchelper/writers/trip98ddd.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper/writers/writer.py` & `pymchelper-2.5.1/pymchelper/writers/writer.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper.egg-info/PKG-INFO` & `pymchelper-2.5.1/pymchelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.5.0/pymchelper.egg-info/SOURCES.txt` & `pymchelper-2.5.1/pymchelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.0/pymchelper.egg-info/requires.txt` & `pymchelper-2.5.1/pymchelper.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 [dicom:python_version == "3.11"]
 pydicom>=2.3.1
 
 [excel]
 xlwt
 
 [full]
-scipy
-matplotlib
-xlwt
 h5py
+xlwt
+matplotlib
+scipy
 hipsterplot
 bashplotlib
 
 [full:python_version < "3.11"]
 pydicom
 
 [full:python_version == "3.11"]
```

### Comparing `pymchelper-2.5.0/setup.py` & `pymchelper-2.5.1/setup.py`

 * *Files identical despite different names*

