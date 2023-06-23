# Comparing `tmp/xlwings-0.9.2.tar.gz` & `tmp/xlwings-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xlwings-0.9.2.tar", last modified: Mon Aug  8 21:23:16 2016, max compression
+gzip compressed data, was "dist/xlwings-0.9.3.tar", last modified: Mon Aug 22 21:34:05 2016, max compression
```

## Comparing `xlwings-0.9.2.tar` & `xlwings-0.9.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-08 21:23:16.000000 xlwings-0.9.2/
-drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-08 21:23:16.000000 xlwings-0.9.2/docs/
--rw-r--r--   0 Felix      (501) staff       (20)     6148 2016-03-29 21:19:23.000000 xlwings-0.9.2/docs/.DS_Store
--rw-r--r--   0 Felix      (501) staff       (20)     1028 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/api.rst
--rw-r--r--   0 Felix      (501) staff       (20)     2704 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/command_line.rst
--rw-r--r--   0 Felix      (501) staff       (20)     9764 2016-08-08 21:19:59.000000 xlwings-0.9.2/docs/conf.py
--rw-r--r--   0 Felix      (501) staff       (20)     2414 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/connect_to_workbook.rst
--rw-r--r--   0 Felix      (501) staff       (20)    15829 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/converters.rst
--rw-r--r--   0 Felix      (501) staff       (20)     5975 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/datastructures.rst
--rw-r--r--   0 Felix      (501) staff       (20)     2404 2016-08-08 21:20:26.000000 xlwings-0.9.2/docs/debugging.rst
-drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-08 21:23:16.000000 xlwings-0.9.2/docs/images/
--rw-r--r--   0 Felix      (501) staff       (20)     6148 2016-02-26 10:14:31.000000 xlwings-0.9.2/docs/images/.DS_Store
--rw-r--r--   0 Felix      (501) staff       (20)     2742 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/1d_ranges.png
--rwxr-xr-x   0 Felix      (501) staff       (20)    63283 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/array_formula.png
--rw-r--r--   0 Felix      (501) staff       (20)    12604 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/chart_type.png
--rw-r--r--   0 Felix      (501) staff       (20)    10612 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/debugging_error.png
--rw-r--r--   0 Felix      (501) staff       (20)    22440 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/df_converter.png
--rw-r--r--   0 Felix      (501) staff       (20)     8622 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/dict_converter.png
--rwxr-xr-x   0 Felix      (501) staff       (20)    40711 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/double_sum.png
--rw-r--r--   0 Felix      (501) staff       (20)    36392 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/mac_error.png
--rw-r--r--   0 Felix      (501) staff       (20)   361294 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/matplotlib.png
--rw-r--r--   0 Felix      (501) staff       (20)    66535 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/mpl_basic.png
--rw-r--r--   0 Felix      (501) staff       (20)    76924 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/mpl_udf.png
--rw-r--r--   0 Felix      (501) staff       (20)     3126 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/pandas_series.png
--rw-r--r--   0 Felix      (501) staff       (20)    17807 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/series_conv.png
--rw-r--r--   0 Felix      (501) staff       (20)   168823 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/udf_debugging.png
--rw-r--r--   0 Felix      (501) staff       (20)     9818 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/images/udf_example.png
--rw-r--r--   0 Felix      (501) staff       (20)      895 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/index.rst
--rw-r--r--   0 Felix      (501) staff       (20)      286 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/index_latex.rst
--rw-r--r--   0 Felix      (501) staff       (20)     1719 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/installation.rst
--rw-r--r--   0 Felix      (501) staff       (20)     5098 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/make.bat
--rw-r--r--   0 Felix      (501) staff       (20)     5568 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/Makefile
--rw-r--r--   0 Felix      (501) staff       (20)     2695 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/matplotlib.rst
--rw-r--r--   0 Felix      (501) staff       (20)    13930 2016-08-08 21:20:26.000000 xlwings-0.9.2/docs/migrate_to_0.9.rst
--rw-r--r--   0 Felix      (501) staff       (20)     1832 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/missing_features.rst
--rw-r--r--   0 Felix      (501) staff       (20)     3526 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/quickstart.rst
--rw-r--r--   0 Felix      (501) staff       (20)     2879 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/r_and_julia.rst
--rw-r--r--   0 Felix      (501) staff       (20)       22 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/requirements.txt
--rw-r--r--   0 Felix      (501) staff       (20)     2484 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/syntax_overview.rst
--rw-r--r--   0 Felix      (501) staff       (20)     7875 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/udfs.rst
--rw-r--r--   0 Felix      (501) staff       (20)     5251 2016-08-05 13:15:32.000000 xlwings-0.9.2/docs/vba.rst
--rw-r--r--   0 Felix      (501) staff       (20)    44968 2016-08-08 21:20:26.000000 xlwings-0.9.2/docs/whatsnew.rst
--rw-r--r--   0 Felix      (501) staff       (20)    12983 2016-08-05 13:15:32.000000 xlwings-0.9.2/LICENSE.txt
--rw-r--r--   0 Felix      (501) staff       (20)      292 2016-08-05 13:15:32.000000 xlwings-0.9.2/MANIFEST.in
--rw-r--r--   0 Felix      (501) staff       (20)     1978 2016-08-08 21:23:16.000000 xlwings-0.9.2/PKG-INFO
--rw-r--r--   0 Felix      (501) staff       (20)      846 2016-08-08 21:19:59.000000 xlwings-0.9.2/README.rst
--rw-r--r--   0 Felix      (501) staff       (20)       59 2016-08-08 21:23:16.000000 xlwings-0.9.2/setup.cfg
--rw-r--r--   0 Felix      (501) staff       (20)     2867 2016-08-05 13:15:32.000000 xlwings-0.9.2/setup.py
-drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-08 21:23:16.000000 xlwings-0.9.2/xlwings/
--rw-r--r--   0 Felix      (501) staff       (20)     1618 2016-08-08 21:20:26.000000 xlwings-0.9.2/xlwings/__init__.py
--rw-r--r--   0 Felix      (501) staff       (20)    37637 2016-08-08 21:20:26.000000 xlwings-0.9.2/xlwings/_xlmac.py
--rw-r--r--   0 Felix      (501) staff       (20)    40602 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/_xlwindows.py
--rw-r--r--   0 Felix      (501) staff       (20)     9910 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/command_line.py
--rw-r--r--   0 Felix      (501) staff       (20)   128884 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/constants.py
-drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-08 21:23:16.000000 xlwings-0.9.2/xlwings/conversion/
--rw-r--r--   0 Felix      (501) staff       (20)     1220 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/conversion/__init__.py
--rw-r--r--   0 Felix      (501) staff       (20)     3750 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/conversion/framework.py
--rw-r--r--   0 Felix      (501) staff       (20)     1047 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/conversion/numpy_conv.py
--rw-r--r--   0 Felix      (501) staff       (20)     5354 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/conversion/pandas_conv.py
--rw-r--r--   0 Felix      (501) staff       (20)     7300 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/conversion/standard.py
--rw-r--r--   0 Felix      (501) staff       (20)   233416 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/mac_dict.py
--rw-r--r--   0 Felix      (501) staff       (20)    75883 2016-08-08 21:20:26.000000 xlwings-0.9.2/xlwings/main.py
--rw-r--r--   0 Felix      (501) staff       (20)    36759 2016-08-08 21:20:26.000000 xlwings-0.9.2/xlwings/quickstart.xlsm
--rw-r--r--   0 Felix      (501) staff       (20)     9160 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/server.py
-drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-08 21:23:16.000000 xlwings-0.9.2/xlwings/tests/
--rw-r--r--   0 Felix      (501) staff       (20)        0 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/__init__.py
--rw-r--r--   0 Felix      (501) staff       (20)     1007 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/common.py
--rw-r--r--   0 Felix      (501) staff       (20)    12945 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/macro book.xlsm
--rw-r--r--   0 Felix      (501) staff       (20)     3799 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/sample_picture.png
--rw-r--r--   0 Felix      (501) staff       (20)     8340 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test book.xlsx
--rw-r--r--   0 Felix      (501) staff       (20)     2321 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_active.py
--rw-r--r--   0 Felix      (501) staff       (20)     4500 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_app.py
--rw-r--r--   0 Felix      (501) staff       (20)     7656 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_book.py
--rw-r--r--   0 Felix      (501) staff       (20)    20554 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_conversion.py
--rw-r--r--   0 Felix      (501) staff       (20)     4242 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_names.py
--rw-r--r--   0 Felix      (501) staff       (20)    23848 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_range.py
--rw-r--r--   0 Felix      (501) staff       (20)     8532 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_shape.py
--rw-r--r--   0 Felix      (501) staff       (20)     4976 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/tests/test_sheet.py
--rw-r--r--   0 Felix      (501) staff       (20)    12533 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/udfs.py
--rw-r--r--   0 Felix      (501) staff       (20)     4898 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/utils.py
--rw-r--r--   0 Felix      (501) staff       (20)     1233 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/xlwings.applescript
--rw-r--r--   0 Felix      (501) staff       (20)    24052 2016-08-08 21:20:26.000000 xlwings-0.9.2/xlwings/xlwings.bas
--rwxr-xr-x   0 Felix      (501) staff       (20)    17881 2016-08-05 13:15:32.000000 xlwings-0.9.2/xlwings/xlwings.xlam
--rw-r--r--   0 Felix      (501) staff       (20)    37007 2016-08-08 21:20:26.000000 xlwings-0.9.2/xlwings/xlwings_template.xltm
-drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-08 21:23:16.000000 xlwings-0.9.2/xlwings.egg-info/
--rw-r--r--   0 Felix      (501) staff       (20)        1 2016-08-08 21:23:15.000000 xlwings-0.9.2/xlwings.egg-info/dependency_links.txt
--rw-r--r--   0 Felix      (501) staff       (20)       55 2016-08-08 21:23:15.000000 xlwings-0.9.2/xlwings.egg-info/entry_points.txt
--rw-r--r--   0 Felix      (501) staff       (20)     1978 2016-08-08 21:23:15.000000 xlwings-0.9.2/xlwings.egg-info/PKG-INFO
--rw-r--r--   0 Felix      (501) staff       (20)       35 2016-08-08 21:23:15.000000 xlwings-0.9.2/xlwings.egg-info/requires.txt
--rw-r--r--   0 Felix      (501) staff       (20)     1991 2016-08-08 21:23:15.000000 xlwings-0.9.2/xlwings.egg-info/SOURCES.txt
--rw-r--r--   0 Felix      (501) staff       (20)        8 2016-08-08 21:23:15.000000 xlwings-0.9.2/xlwings.egg-info/top_level.txt
--rwx------   0 Felix      (501) staff       (20)   276480 2016-02-23 16:51:38.000000 xlwings-0.9.2/xlwings32.dll
--rwx------   0 Felix      (501) staff       (20)   344064 2016-02-23 16:51:18.000000 xlwings-0.9.2/xlwings64.dll
+drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-22 21:34:05.000000 xlwings-0.9.3/
+drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-22 21:34:05.000000 xlwings-0.9.3/docs/
+-rw-r--r--   0 Felix      (501) staff       (20)     6148 2016-03-29 21:19:23.000000 xlwings-0.9.3/docs/.DS_Store
+-rw-r--r--   0 Felix      (501) staff       (20)     1028 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/api.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     2704 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/command_line.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     9764 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/conf.py
+-rw-r--r--   0 Felix      (501) staff       (20)     2414 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/connect_to_workbook.rst
+-rw-r--r--   0 Felix      (501) staff       (20)    15829 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/converters.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     5975 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/datastructures.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     2404 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/debugging.rst
+drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-22 21:34:05.000000 xlwings-0.9.3/docs/images/
+-rw-r--r--   0 Felix      (501) staff       (20)     6148 2016-02-26 10:14:31.000000 xlwings-0.9.3/docs/images/.DS_Store
+-rw-r--r--   0 Felix      (501) staff       (20)     2742 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/1d_ranges.png
+-rwxr-xr-x   0 Felix      (501) staff       (20)    63283 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/array_formula.png
+-rw-r--r--   0 Felix      (501) staff       (20)    12604 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/chart_type.png
+-rw-r--r--   0 Felix      (501) staff       (20)    10612 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/debugging_error.png
+-rw-r--r--   0 Felix      (501) staff       (20)    22440 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/df_converter.png
+-rw-r--r--   0 Felix      (501) staff       (20)     8622 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/dict_converter.png
+-rwxr-xr-x   0 Felix      (501) staff       (20)    40711 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/double_sum.png
+-rw-r--r--   0 Felix      (501) staff       (20)    36392 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/mac_error.png
+-rw-r--r--   0 Felix      (501) staff       (20)   361294 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/matplotlib.png
+-rw-r--r--   0 Felix      (501) staff       (20)    66535 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/mpl_basic.png
+-rw-r--r--   0 Felix      (501) staff       (20)    76924 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/mpl_udf.png
+-rw-r--r--   0 Felix      (501) staff       (20)     3126 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/pandas_series.png
+-rw-r--r--   0 Felix      (501) staff       (20)    17807 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/series_conv.png
+-rw-r--r--   0 Felix      (501) staff       (20)   168823 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/udf_debugging.png
+-rw-r--r--   0 Felix      (501) staff       (20)     9818 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/images/udf_example.png
+-rw-r--r--   0 Felix      (501) staff       (20)      895 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/index.rst
+-rw-r--r--   0 Felix      (501) staff       (20)      286 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/index_latex.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     1719 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/installation.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     5098 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/make.bat
+-rw-r--r--   0 Felix      (501) staff       (20)     5568 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/Makefile
+-rw-r--r--   0 Felix      (501) staff       (20)     2695 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/matplotlib.rst
+-rw-r--r--   0 Felix      (501) staff       (20)    13930 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/migrate_to_0.9.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     1832 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/missing_features.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     3526 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/quickstart.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     2879 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/r_and_julia.rst
+-rw-r--r--   0 Felix      (501) staff       (20)       22 2016-08-21 11:12:32.000000 xlwings-0.9.3/docs/requirements.txt
+-rw-r--r--   0 Felix      (501) staff       (20)     2484 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/syntax_overview.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     7875 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/udfs.rst
+-rw-r--r--   0 Felix      (501) staff       (20)     5251 2016-08-21 17:09:28.000000 xlwings-0.9.3/docs/vba.rst
+-rw-r--r--   0 Felix      (501) staff       (20)    45480 2016-08-22 21:30:04.000000 xlwings-0.9.3/docs/whatsnew.rst
+-rw-r--r--   0 Felix      (501) staff       (20)    12983 2016-08-21 11:12:32.000000 xlwings-0.9.3/LICENSE.txt
+-rw-r--r--   0 Felix      (501) staff       (20)      292 2016-08-21 11:12:32.000000 xlwings-0.9.3/MANIFEST.in
+-rw-r--r--   0 Felix      (501) staff       (20)     1978 2016-08-22 21:34:05.000000 xlwings-0.9.3/PKG-INFO
+-rw-r--r--   0 Felix      (501) staff       (20)      846 2016-08-21 17:09:28.000000 xlwings-0.9.3/README.rst
+-rw-r--r--   0 Felix      (501) staff       (20)       59 2016-08-22 21:34:05.000000 xlwings-0.9.3/setup.cfg
+-rw-r--r--   0 Felix      (501) staff       (20)     2867 2016-08-21 17:09:28.000000 xlwings-0.9.3/setup.py
+drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-22 21:34:05.000000 xlwings-0.9.3/xlwings/
+-rw-r--r--   0 Felix      (501) staff       (20)     1618 2016-08-22 21:30:04.000000 xlwings-0.9.3/xlwings/__init__.py
+-rw-r--r--   0 Felix      (501) staff       (20)    38036 2016-08-22 21:30:04.000000 xlwings-0.9.3/xlwings/_xlmac.py
+-rw-r--r--   0 Felix      (501) staff       (20)    40915 2016-08-22 21:30:04.000000 xlwings-0.9.3/xlwings/_xlwindows.py
+-rw-r--r--   0 Felix      (501) staff       (20)     9910 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/command_line.py
+-rw-r--r--   0 Felix      (501) staff       (20)   128884 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/constants.py
+drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-22 21:34:05.000000 xlwings-0.9.3/xlwings/conversion/
+-rw-r--r--   0 Felix      (501) staff       (20)     1220 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/conversion/__init__.py
+-rw-r--r--   0 Felix      (501) staff       (20)     3750 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/conversion/framework.py
+-rw-r--r--   0 Felix      (501) staff       (20)     1047 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/conversion/numpy_conv.py
+-rw-r--r--   0 Felix      (501) staff       (20)     5354 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/conversion/pandas_conv.py
+-rw-r--r--   0 Felix      (501) staff       (20)     7300 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/conversion/standard.py
+-rw-r--r--   0 Felix      (501) staff       (20)   233416 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/mac_dict.py
+-rw-r--r--   0 Felix      (501) staff       (20)    77230 2016-08-22 21:30:04.000000 xlwings-0.9.3/xlwings/main.py
+-rw-r--r--   0 Felix      (501) staff       (20)    36589 2016-08-22 21:30:04.000000 xlwings-0.9.3/xlwings/quickstart.xlsm
+-rw-r--r--   0 Felix      (501) staff       (20)     9160 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/server.py
+drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-22 21:34:05.000000 xlwings-0.9.3/xlwings/tests/
+-rw-r--r--   0 Felix      (501) staff       (20)        0 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/tests/__init__.py
+-rw-r--r--   0 Felix      (501) staff       (20)     1007 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/common.py
+-rw-r--r--   0 Felix      (501) staff       (20)    12945 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/tests/macro book.xlsm
+-rw-r--r--   0 Felix      (501) staff       (20)     3799 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/tests/sample_picture.png
+-rw-r--r--   0 Felix      (501) staff       (20)     8340 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test book.xlsx
+-rw-r--r--   0 Felix      (501) staff       (20)     2321 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_active.py
+-rw-r--r--   0 Felix      (501) staff       (20)     4500 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_app.py
+-rw-r--r--   0 Felix      (501) staff       (20)     7656 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_book.py
+-rw-r--r--   0 Felix      (501) staff       (20)    20554 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_conversion.py
+-rw-r--r--   0 Felix      (501) staff       (20)     4242 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_names.py
+-rw-r--r--   0 Felix      (501) staff       (20)    23848 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_range.py
+-rw-r--r--   0 Felix      (501) staff       (20)     8532 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_shape.py
+-rw-r--r--   0 Felix      (501) staff       (20)     4976 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/tests/test_sheet.py
+-rw-r--r--   0 Felix      (501) staff       (20)    12533 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/udfs.py
+-rw-r--r--   0 Felix      (501) staff       (20)     4898 2016-08-21 17:09:28.000000 xlwings-0.9.3/xlwings/utils.py
+-rw-r--r--   0 Felix      (501) staff       (20)     1233 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/xlwings.applescript
+-rw-r--r--   0 Felix      (501) staff       (20)    24192 2016-08-22 21:30:04.000000 xlwings-0.9.3/xlwings/xlwings.bas
+-rwxr-xr-x   0 Felix      (501) staff       (20)    17881 2016-08-21 11:12:32.000000 xlwings-0.9.3/xlwings/xlwings.xlam
+-rw-r--r--   0 Felix      (501) staff       (20)    37244 2016-08-22 21:30:04.000000 xlwings-0.9.3/xlwings/xlwings_template.xltm
+drwxr-xr-x   0 Felix      (501) staff       (20)        0 2016-08-22 21:34:05.000000 xlwings-0.9.3/xlwings.egg-info/
+-rw-r--r--   0 Felix      (501) staff       (20)        1 2016-08-22 21:34:04.000000 xlwings-0.9.3/xlwings.egg-info/dependency_links.txt
+-rw-r--r--   0 Felix      (501) staff       (20)       55 2016-08-22 21:34:04.000000 xlwings-0.9.3/xlwings.egg-info/entry_points.txt
+-rw-r--r--   0 Felix      (501) staff       (20)     1978 2016-08-22 21:34:04.000000 xlwings-0.9.3/xlwings.egg-info/PKG-INFO
+-rw-r--r--   0 Felix      (501) staff       (20)       35 2016-08-22 21:34:04.000000 xlwings-0.9.3/xlwings.egg-info/requires.txt
+-rw-r--r--   0 Felix      (501) staff       (20)     1991 2016-08-22 21:34:05.000000 xlwings-0.9.3/xlwings.egg-info/SOURCES.txt
+-rw-r--r--   0 Felix      (501) staff       (20)        8 2016-08-22 21:34:04.000000 xlwings-0.9.3/xlwings.egg-info/top_level.txt
+-rwx------   0 Felix      (501) staff       (20)   276480 2016-02-23 16:51:38.000000 xlwings-0.9.3/xlwings32.dll
+-rwx------   0 Felix      (501) staff       (20)   344064 2016-02-23 16:51:18.000000 xlwings-0.9.3/xlwings64.dll
```

### Comparing `xlwings-0.9.2/docs/.DS_Store` & `xlwings-0.9.3/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/api.rst` & `xlwings-0.9.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/command_line.rst` & `xlwings-0.9.3/docs/command_line.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/conf.py` & `xlwings-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/connect_to_workbook.rst` & `xlwings-0.9.3/docs/connect_to_workbook.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/converters.rst` & `xlwings-0.9.3/docs/converters.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/datastructures.rst` & `xlwings-0.9.3/docs/datastructures.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/debugging.rst` & `xlwings-0.9.3/docs/debugging.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/.DS_Store` & `xlwings-0.9.3/docs/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/1d_ranges.png` & `xlwings-0.9.3/docs/images/1d_ranges.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/array_formula.png` & `xlwings-0.9.3/docs/images/array_formula.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/chart_type.png` & `xlwings-0.9.3/docs/images/chart_type.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/debugging_error.png` & `xlwings-0.9.3/docs/images/debugging_error.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/df_converter.png` & `xlwings-0.9.3/docs/images/df_converter.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/dict_converter.png` & `xlwings-0.9.3/docs/images/dict_converter.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/double_sum.png` & `xlwings-0.9.3/docs/images/double_sum.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/mac_error.png` & `xlwings-0.9.3/docs/images/mac_error.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/matplotlib.png` & `xlwings-0.9.3/docs/images/matplotlib.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/mpl_basic.png` & `xlwings-0.9.3/docs/images/mpl_basic.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/mpl_udf.png` & `xlwings-0.9.3/docs/images/mpl_udf.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/pandas_series.png` & `xlwings-0.9.3/docs/images/pandas_series.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/series_conv.png` & `xlwings-0.9.3/docs/images/series_conv.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/udf_debugging.png` & `xlwings-0.9.3/docs/images/udf_debugging.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/images/udf_example.png` & `xlwings-0.9.3/docs/images/udf_example.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/index.rst` & `xlwings-0.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/installation.rst` & `xlwings-0.9.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/make.bat` & `xlwings-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/Makefile` & `xlwings-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/matplotlib.rst` & `xlwings-0.9.3/docs/matplotlib.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/migrate_to_0.9.rst` & `xlwings-0.9.3/docs/migrate_to_0.9.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/missing_features.rst` & `xlwings-0.9.3/docs/missing_features.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/quickstart.rst` & `xlwings-0.9.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/r_and_julia.rst` & `xlwings-0.9.3/docs/r_and_julia.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/syntax_overview.rst` & `xlwings-0.9.3/docs/syntax_overview.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/udfs.rst` & `xlwings-0.9.3/docs/udfs.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/vba.rst` & `xlwings-0.9.3/docs/vba.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/docs/whatsnew.rst` & `xlwings-0.9.3/docs/whatsnew.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 What's New
 ==========
 
+v0.9.3 (Aug 22, 2016)
+---------------------
+
+* [Win] ``App.visible`` wasn't behaving correctly (:issue:`551`).
+* [Mac] Added support for the new 64bit version of Excel 2016 on Mac (:issue:`549`).
+* Unicode book names are again supported (:issue:`546`).
+* :meth:`xlwings.Book.save()` now supports relative paths. Also, when saving an existing book under a new name
+  without specifying the full path, it'll be saved in Python's current working directory instead of in Excel's default
+  directory (:issue:`185`).
+
 v0.9.2 (Aug 8, 2016)
 --------------------
 
 Another round of bug fixes:
 
 * [Mac]: Sometimes, a column was referenced instead of a named range (:issue:`545`)
 * [Mac]: Python 2.7 was raising a ``LookupError: unknown encoding: mbcs`` (:issue:`544`)
```

### Comparing `xlwings-0.9.2/LICENSE.txt` & `xlwings-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/PKG-INFO` & `xlwings-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xlwings
-Version: 0.9.2
+Version: 0.9.3
 Summary: Make Excel fly: Interact with Excel from Python and vice versa.
 Home-page: http://xlwings.org
 Author: Zoomer Analytics LLC
 Author-email: felix.zumstein@zoomeranalytics.com
 License: BSD 3-clause
 Description: xlwings - Make Excel fly with Python!
         =====================================
```

### Comparing `xlwings-0.9.2/README.rst` & `xlwings-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/setup.py` & `xlwings-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/__init__.py` & `xlwings-0.9.3/xlwings/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import absolute_import
 import sys
 
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 # Python 2 vs 3
 PY3 = sys.version_info[0] == 3
 
 if PY3:
     string_types = str
     xrange = range
```

### Comparing `xlwings-0.9.2/xlwings/_xlmac.py` & `xlwings-0.9.3/xlwings/_xlmac.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,22 +216,27 @@
         self.xl.close(saving=kw.no)
 
     def save(self, path):
         saved_path = self.xl.properties().get(kw.path)
         if (saved_path != '') and (path is None):
             # Previously saved: Save under existing name
             self.xl.save()
+        elif (saved_path != '') and (path is not None) and (os.path.split(path)[0] == ''):
+            # Save existing book under new name in cwd if no path has been provided
+            path = os.path.join(os.getcwd(), path)
+            hfs_path = posix_to_hfs_path(os.path.realpath(path))
+            self.xl.save_workbook_as(filename=hfs_path, overwrite=True)
         elif (saved_path == '') and (path is None):
             # Previously unsaved: Save under current name in current working directory
             path = os.path.join(os.getcwd(), self.xl.name.get() + '.xlsx')
-            hfs_path = posix_to_hfs_path(path)
+            hfs_path = posix_to_hfs_path(os.path.realpath(path))
             self.xl.save_workbook_as(filename=hfs_path, overwrite=True)
         elif path:
             # Save under new name/location
-            hfs_path = posix_to_hfs_path(path)
+            hfs_path = posix_to_hfs_path(os.path.realpath(path))
             self.xl.save_workbook_as(filename=hfs_path, overwrite=True)
 
     @property
     def fullname(self):
         hfs_path = self.xl.properties().get(kw.full_name)
         # Excel 2011 returns HFS path, Excel 2016 returns POSIX path
         if hfs_path == self.xl.properties().get(kw.name) or int(self.app.version.split('.')[0]) >= 15:
```

### Comparing `xlwings-0.9.2/xlwings/_xlwindows.py` & `xlwings-0.9.3/xlwings/_xlwindows.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,26 +462,30 @@
         self.xl.Close(SaveChanges=False)
 
     def save(self, path=None):
         saved_path = self.xl.Path
         if (saved_path != '') and (path is None):
             # Previously saved: Save under existing name
             self.xl.Save()
+        elif (saved_path != '') and (path is not None) and (os.path.split(path)[0] == ''):
+            # Save existing book under new name in cwd if no path has been provided
+            path = os.path.join(os.getcwd(), path)
+            self.xl.SaveAs(os.path.realpath(path))
         elif (saved_path == '') and (path is None):
             # Previously unsaved: Save under current name in current working directory
             path = os.path.join(os.getcwd(), self.xl.Name + '.xlsx')
             alerts_state = self.xl.Application.DisplayAlerts
             self.xl.Application.DisplayAlerts = False
-            self.xl.SaveAs(path)
+            self.xl.SaveAs(os.path.realpath(path))
             self.xl.Application.DisplayAlerts = alerts_state
         elif path:
             # Save under new name/location
             alerts_state = self.xl.Application.DisplayAlerts
             self.xl.Application.DisplayAlerts = False
-            self.xl.SaveAs(path)
+            self.xl.SaveAs(os.path.realpath(path))
             self.xl.Application.DisplayAlerts = alerts_state
 
     @property
     def fullname(self):
         return self.xl.FullName
 
     @property
```

### Comparing `xlwings-0.9.2/xlwings/command_line.py` & `xlwings-0.9.3/xlwings/command_line.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/constants.py` & `xlwings-0.9.3/xlwings/constants.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/conversion/__init__.py` & `xlwings-0.9.3/xlwings/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/conversion/framework.py` & `xlwings-0.9.3/xlwings/conversion/framework.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/conversion/numpy_conv.py` & `xlwings-0.9.3/xlwings/conversion/numpy_conv.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/conversion/pandas_conv.py` & `xlwings-0.9.3/xlwings/conversion/pandas_conv.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/conversion/standard.py` & `xlwings-0.9.3/xlwings/conversion/standard.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/mac_dict.py` & `xlwings-0.9.3/xlwings/mac_dict.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/main.py` & `xlwings-0.9.3/xlwings/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,16 +176,17 @@
     >>> xw.apps[0]
     <Excel App 1668>
     >>> xw.apps.active
     <Excel App 1668>
 
     Parameters
     ----------
-    visible : bool, default True
-        Returns or sets a boolean value that determines whether the app is visible.
+    visible : bool, default None
+        Returns or sets a boolean value that determines whether the app is visible. The default
+        leaves the state unchanged or sets visible=True if the object doesn't exist yet.
 
     spec : str, default None
         Mac-only, use the full path to the Excel application,
         e.g. ``/Applications/Microsoft Office 2011/Microsoft Excel`` or ``/Applications/Microsoft Excel``
 
         On Windows, if you want to change the version of Excel that xlwings talks to, go to ``Control Panel >
         Programs and Features`` and ``Repair`` the Office version that you want as default.
@@ -194,15 +195,15 @@
     .. note::
         On Mac, while xlwings allows you to run multiple instances of Excel, it's a feature that is not officially
         supported by Excel for Mac: Unlike on Windows, Excel will not ask you to open a read-only version of a file
         if it is already open in another instance. This means that you need to watch out yourself so that the same
         file is not being overwritten from different instances.
     """
 
-    def __init__(self, visible=True, spec=None, add_book=True, impl=None):
+    def __init__(self, visible=None, spec=None, add_book=True, impl=None):
         if impl is None:
             self.impl = xlplatform.App(spec=spec, add_book=add_book)
             if visible or visible is None:
                 self.visible = True
         else:
             self.impl = impl
             if visible:
@@ -460,20 +461,14 @@
         path, it looks for the file in the current working directory.
 
     """
 
     def __init__(self, fullname=None, impl=None):
         if not impl:
             if fullname:
-                if not PY3 and isinstance(fullname, str):
-                    if sys.platform.startswith('win'):
-                        fullname = unicode(fullname, 'mbcs')
-                    elif sys.platform.startswith('darwin'):
-                        fullname = unicode(fullname, 'utf-8')
-                        # fullname = unicodedata.normalize('NFKC', fullname)  # necessary?
                 fullname = fullname.lower()
 
                 candidates = []
                 for app in apps:
                     for wb in app.books:
                         if wb.fullname.lower() == fullname or wb.name.lower() == fullname:
                             candidates.append((app, wb))
@@ -538,17 +533,26 @@
         if hasattr(Book, '_mock_caller'):
             # Use mocking Book, see Book.set_mock_caller()
             return cls(impl=Book._mock_caller.impl)
         elif len(sys.argv) > 2 and sys.argv[2] == 'from_xl':
             fullname = sys.argv[1].lower()
             if sys.platform.startswith('win'):
                 app = App(impl=xlplatform.App(xl=int(sys.argv[4])))  # hwnd
+                if not PY3 and isinstance(fullname, str):
+                    fullname = fullname.decode('mbcs')
                 return cls(impl=app.books.open(fullname).impl)
             else:
                 # On Mac, the same file open in two instances is not supported
+                if PY3 and apps.active.version < 15:
+                    fullname = fullname.encode('utf-8', 'surrogateescape').decode('mac_latin2')
+                elif not PY3 and isinstance(fullname, str):
+                    if apps.active.version < 15:
+                        fullname = fullname.decode('mac_latin2')
+                    else:
+                        fullname = fullname.decode('utf-8')
                 return cls(impl=Book(fullname).impl)
         elif xlplatform.BOOK_CALLER:
             # Called via OPTIMIZED_CONNECTION = True
             return cls(impl=xlplatform.Book(xlplatform.BOOK_CALLER))
         else:
             raise Exception('Workbook.caller() must not be called directly. Call through Excel or set a mock caller '
                             'first with Book.set_mock_caller().')
@@ -661,18 +665,41 @@
         Closes the book without saving it.
 
         .. versionadded:: 0.1.1
         """
         self.impl.close()
 
     def save(self, path=None):
+        """
+        Saves the Workbook. If a path is being provided, this works like SaveAs() in Excel. If no path is specified and
+        if the file hasn't been saved previously, it's being saved in the current working directory with the current
+        filename. Existing files are overwritten without prompting.
+
+        Arguments
+        ---------
+        path : str, default None
+            Full path to the workbook
+        Example
+        -------
+        >>> import xlwings as xw
+        >>> wb = xw.Book()
+        >>> wb.save()
+        >>> wb.save(r'C:\\path\\to\\new_file_name.xlsx')
+
+
+        .. versionadded:: 0.3.1
+        """
         return self.impl.save(path)
 
     @property
     def fullname(self):
+        """
+        Returns the name of the object, including its path on disk, as a string. Read-only String.
+
+        """
         return self.impl.fullname
 
     @property
     def names(self):
         """
         Returns a names collection that represents all the names in the specified book (including all sheet-specific names).
 
@@ -700,15 +727,18 @@
         Returns the selected cells as Range.
 
         .. versionadded:: 0.9.0
         """
         return Range(impl=self.app.selection.impl)
 
     def __repr__(self):
-        return "<Book [{0}]>".format(self.name)
+        if not PY3:
+            return u"<Book [{0}]>".format(self.name).encode('utf-8')
+        else:
+            return "<Book [{0}]>".format(self.name)
 
 
 class Sheet(object):
     """
     A sheet object is a member of the :meth:`sheets <xlwings.main.Sheets>` collection:
 
     >>> import xlwings as xw
@@ -851,15 +881,18 @@
         Deletes the Sheet.
 
         .. versionadded: 0.6.0
         """
         return self.impl.delete()
 
     def __repr__(self):
-        return "<Sheet [{1}]{0}>".format(self.name, self.book.name)
+        if not PY3:
+            return u"<Sheet [{1}]{0}>".format(self.name, self.book.name).encode('utf-8')
+        else:
+            return "<Sheet [{1}]{0}>".format(self.name, self.book.name)
 
     @property
     def charts(self):
         """
         See :meth:`Charts <xlwings.main.Charts>`
 
         .. versionadded:: 0.9.0
@@ -1584,19 +1617,18 @@
             else:
                 return self(k + 1)
 
         else:
             raise TypeError("Cell indices must be integers or slices, not %s" % type(key).__name__)
 
     def __repr__(self):
-        return "<Range [{1}]{0}!{2}>".format(
-            self.sheet.name,
-            self.sheet.book.name,
-            self.address
-        )
+        if not PY3:
+            return u"<Range [{1}]{0}!{2}>".format(self.sheet.name, self.sheet.book.name, self.address).encode('utf-8')
+        else:
+            return "<Range [{1}]{0}!{2}>".format(self.sheet.name, self.sheet.book.name, self.address)
 
     @property
     def hyperlink(self):
         """
         Returns the hyperlink address of the specified Range (single Cell only)
 
         Examples
```

### Comparing `xlwings-0.9.2/xlwings/server.py` & `xlwings-0.9.3/xlwings/server.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/common.py` & `xlwings-0.9.3/xlwings/tests/common.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/macro book.xlsm` & `xlwings-0.9.3/xlwings/tests/macro book.xlsm`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/sample_picture.png` & `xlwings-0.9.3/xlwings/tests/sample_picture.png`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test book.xlsx` & `xlwings-0.9.3/xlwings/tests/test book.xlsx`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_active.py` & `xlwings-0.9.3/xlwings/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_app.py` & `xlwings-0.9.3/xlwings/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_book.py` & `xlwings-0.9.3/xlwings/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_conversion.py` & `xlwings-0.9.3/xlwings/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_names.py` & `xlwings-0.9.3/xlwings/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_range.py` & `xlwings-0.9.3/xlwings/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_shape.py` & `xlwings-0.9.3/xlwings/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/tests/test_sheet.py` & `xlwings-0.9.3/xlwings/tests/test_sheet.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/udfs.py` & `xlwings-0.9.3/xlwings/udfs.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/utils.py` & `xlwings-0.9.3/xlwings/utils.py`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/xlwings.applescript` & `xlwings-0.9.3/xlwings/xlwings.applescript`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings/xlwings.bas` & `xlwings-0.9.3/xlwings/xlwings.bas`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Attribute VB_Name = "xlwings"
-' xlwings.org, version: 0.9.2
+' xlwings.org, version: 0.9.3
 '
 ' Copyright (C) 2014-2016, Zoomer Analytics LLC (www.zoomeranalytics.com)
 ' License: BSD 3-clause (see LICENSE.txt for details)
 Option Explicit
-#If Mac Then
-    Private Declare Function system Lib "libc.dylib" (ByVal Command As String) As Long
-#End If
 #If VBA7 Then
+    #If Mac Then
+        Private Declare PtrSafe Function system Lib "libc.dylib" (ByVal Command As String) As Long
+    #End If
     #If Win64 Then
         Const XLPyDLLName As String = "xlwings64.dll"
         Declare PtrSafe Function XLPyDLLActivateAuto Lib "xlwings64.dll" (ByRef result As Variant, Optional ByVal config As String = "") As Long
         Declare PtrSafe Function XLPyDLLNDims Lib "xlwings64.dll" (ByRef src As Variant, ByRef dims As Long, ByRef transpose As Boolean, ByRef dest As Variant) As Long
         Declare PtrSafe Function XLPyDLLVersion Lib "xlwings64.dll" (tag As String, version As Double, arch As String) As Long
     #Else
         Private Const XLPyDLLName As String = "xlwings32.dll"
         Private Declare PtrSafe Function XLPyDLLActivateAuto Lib "xlwings32.dll" (ByRef result As Variant, Optional ByVal config As String = "") As Long
         Private Declare PtrSafe Function XLPyDLLNDims Lib "xlwings32.dll" (ByRef src As Variant, ByRef dims As Long, ByRef transpose As Boolean, ByRef dest As Variant) As Long
         Private Declare PtrSafe Function XLPyDLLVersion Lib "xlwings32.dll" (tag As String, version As Double, arch As String) As Long
     #End If
     Private Declare PtrSafe Function LoadLibrary Lib "kernel32" Alias "LoadLibraryA" (ByVal lpLibFileName As String) As Long
 #Else
+    #If Mac Then
+        Private Declare Function system Lib "libc.dylib" (ByVal Command As String) As Long
+    #End If
     Private Const XLPyDLLName As String = "xlwings32.dll"
     Private Declare Function XLPyDLLActivateAuto Lib "xlwings32.dll" (ByRef result As Variant, Optional ByVal config As String = "") As Long
     Private Declare Function XLPyDLLNDims Lib "xlwings32.dll" (ByRef src As Variant, ByRef dims As Long, ByRef transpose As Boolean, ByRef dest As Variant) As Long
     Private Declare Function LoadLibrary Lib "kernel32" Alias "LoadLibraryA" (ByVal lpLibFileName As String) As Long
     Declare Function XLPyDLLVersion Lib "xlwings32.dll" (tag As String, version As Double, arch As String) As Long
 #End If
```

### Comparing `xlwings-0.9.2/xlwings/xlwings.xlam` & `xlwings-0.9.3/xlwings/xlwings.xlam`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings.egg-info/PKG-INFO` & `xlwings-0.9.3/xlwings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xlwings
-Version: 0.9.2
+Version: 0.9.3
 Summary: Make Excel fly: Interact with Excel from Python and vice versa.
 Home-page: http://xlwings.org
 Author: Zoomer Analytics LLC
 Author-email: felix.zumstein@zoomeranalytics.com
 License: BSD 3-clause
 Description: xlwings - Make Excel fly with Python!
         =====================================
```

### Comparing `xlwings-0.9.2/xlwings.egg-info/SOURCES.txt` & `xlwings-0.9.3/xlwings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings32.dll` & `xlwings-0.9.3/xlwings32.dll`

 * *Files identical despite different names*

### Comparing `xlwings-0.9.2/xlwings64.dll` & `xlwings-0.9.3/xlwings64.dll`

 * *Files identical despite different names*

