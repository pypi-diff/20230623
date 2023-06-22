# Comparing `tmp/pymongoarrow-1.0.0.tar.gz` & `tmp/pymongoarrow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongoarrow-1.0.0.tar", last modified: Wed Jun 21 21:48:29 2023, max compression
+gzip compressed data, was "pymongoarrow-1.0.1.tar", last modified: Thu Jun 22 20:58:51 2023, max compression
```

## Comparing `pymongoarrow-1.0.0.tar` & `pymongoarrow-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:48:29.939520 pymongoarrow-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 21:48:29.939520 pymongoarrow-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:48:29.935521 pymongoarrow-1.0.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/benchmarks/benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/build-libbson.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/cibw_before_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:48:29.935521 pymongoarrow-1.0.0/pymongoarrow/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    31916 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/lib.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/libarrow.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/libbson.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/monkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/pandas_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pymongoarrow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:48:29.939520 pymongoarrow-1.0.0/pymongoarrow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 21:48:29.000000 pymongoarrow-1.0.0/pymongoarrow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-21 21:48:29.000000 pymongoarrow-1.0.0/pymongoarrow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:48:29.000000 pymongoarrow-1.0.0/pymongoarrow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:48:29.000000 pymongoarrow-1.0.0/pymongoarrow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 21:48:29.000000 pymongoarrow-1.0.0/pymongoarrow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 21:48:29.000000 pymongoarrow-1.0.0/pymongoarrow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-21 21:48:29.939520 pymongoarrow-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:48:29.939520 pymongoarrow-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:48:29.939520 pymongoarrow-1.0.0/test/pandas_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/pandas_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/pandas_types/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/pandas_types/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/pandas_types/test_decimal128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/pandas_types/test_objectid.py
--rw-r--r--   0 runner    (1001) docker     (123)    27564 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_bson.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_libbson.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_monkey.py
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_pymongoarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-06-21 21:48:02.000000 pymongoarrow-1.0.0/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:58:51.755003 pymongoarrow-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-22 20:58:51.755003 pymongoarrow-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:58:51.751002 pymongoarrow-1.0.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/benchmarks/benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/build-libbson.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/cibw_before_build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:58:51.755003 pymongoarrow-1.0.1/pymongoarrow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31916 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/lib.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/libarrow.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/libbson.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/monkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/pandas_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pymongoarrow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:58:51.755003 pymongoarrow-1.0.1/pymongoarrow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-22 20:58:51.000000 pymongoarrow-1.0.1/pymongoarrow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-22 20:58:51.000000 pymongoarrow-1.0.1/pymongoarrow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:58:51.000000 pymongoarrow-1.0.1/pymongoarrow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:58:50.000000 pymongoarrow-1.0.1/pymongoarrow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-22 20:58:51.000000 pymongoarrow-1.0.1/pymongoarrow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 20:58:51.000000 pymongoarrow-1.0.1/pymongoarrow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-22 20:58:51.759003 pymongoarrow-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:58:51.755003 pymongoarrow-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:58:51.755003 pymongoarrow-1.0.1/test/pandas_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/pandas_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/pandas_types/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/pandas_types/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/pandas_types/test_decimal128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/pandas_types/test_objectid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27564 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_bson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_libbson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_monkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_pymongoarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-06-22 20:58:25.000000 pymongoarrow-1.0.1/test/utils.py
```

### Comparing `pymongoarrow-1.0.0/LICENSE` & `pymongoarrow-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/PKG-INFO` & `pymongoarrow-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongoarrow
-Version: 1.0.0
+Version: 1.0.1
 Summary: "Tools for using NumPy, Pandas and PyArrow with MongoDB"
 Home-page: https://github.com/mongodb-labs/mongo-arrow/tree/main/bindings/python
 Author: Prashant Mital
 Maintainer: MongoDB, Inc.
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongo,arrow,bson,numpy,pandas
 Platform: Linux
```

### Comparing `pymongoarrow-1.0.0/README.rst` & `pymongoarrow-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/benchmarks/__init__.py` & `pymongoarrow-1.0.1/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/benchmarks/benchmarks.py` & `pymongoarrow-1.0.1/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/build-libbson.sh` & `pymongoarrow-1.0.1/build-libbson.sh`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/cibw_before_build.sh` & `pymongoarrow-1.0.1/cibw_before_build.sh`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/__init__.py` & `pymongoarrow-1.0.1/pymongoarrow/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/api.py` & `pymongoarrow-1.0.1/pymongoarrow/api.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/context.py` & `pymongoarrow-1.0.1/pymongoarrow/context.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/errors.py` & `pymongoarrow-1.0.1/pymongoarrow/errors.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/lib.pyx` & `pymongoarrow-1.0.1/pymongoarrow/lib.pyx`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/libarrow.pxd` & `pymongoarrow-1.0.1/pymongoarrow/libarrow.pxd`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/libbson.pxd` & `pymongoarrow-1.0.1/pymongoarrow/libbson.pxd`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/monkey.py` & `pymongoarrow-1.0.1/pymongoarrow/monkey.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/pandas_types.py` & `pymongoarrow-1.0.1/pymongoarrow/pandas_types.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/result.py` & `pymongoarrow-1.0.1/pymongoarrow/result.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/schema.py` & `pymongoarrow-1.0.1/pymongoarrow/schema.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/types.py` & `pymongoarrow-1.0.1/pymongoarrow/types.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pymongoarrow/version.py` & `pymongoarrow-1.0.1/pymongoarrow/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 _MIN_LIBBSON_VERSION = "1.21.0"
```

### Comparing `pymongoarrow-1.0.0/pymongoarrow.egg-info/PKG-INFO` & `pymongoarrow-1.0.1/pymongoarrow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongoarrow
-Version: 1.0.0
+Version: 1.0.1
 Summary: "Tools for using NumPy, Pandas and PyArrow with MongoDB"
 Home-page: https://github.com/mongodb-labs/mongo-arrow/tree/main/bindings/python
 Author: Prashant Mital
 Maintainer: MongoDB, Inc.
 License: Apache License, Version 2.0
 Keywords: mongo,mongodb,pymongo,arrow,bson,numpy,pandas
 Platform: Linux
```

### Comparing `pymongoarrow-1.0.0/pymongoarrow.egg-info/SOURCES.txt` & `pymongoarrow-1.0.1/pymongoarrow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/pyproject.toml` & `pymongoarrow-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/setup.cfg` & `pymongoarrow-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/setup.py` & `pymongoarrow-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/__init__.py` & `pymongoarrow-1.0.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/conftest.py` & `pymongoarrow-1.0.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/pandas_types/test_binary.py` & `pymongoarrow-1.0.1/test/pandas_types/test_binary.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/pandas_types/test_code.py` & `pymongoarrow-1.0.1/test/pandas_types/test_code.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/pandas_types/test_decimal128.py` & `pymongoarrow-1.0.1/test/pandas_types/test_decimal128.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/pandas_types/test_objectid.py` & `pymongoarrow-1.0.1/test/pandas_types/test_objectid.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_arrow.py` & `pymongoarrow-1.0.1/test/test_arrow.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_bson.py` & `pymongoarrow-1.0.1/test/test_bson.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_builders.py` & `pymongoarrow-1.0.1/test/test_builders.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_datetime.py` & `pymongoarrow-1.0.1/test/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_libbson.py` & `pymongoarrow-1.0.1/test/test_libbson.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_monkey.py` & `pymongoarrow-1.0.1/test/test_monkey.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_numpy.py` & `pymongoarrow-1.0.1/test/test_numpy.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_pandas.py` & `pymongoarrow-1.0.1/test/test_pandas.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_pymongoarrow.py` & `pymongoarrow-1.0.1/test/test_pymongoarrow.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/test_schema.py` & `pymongoarrow-1.0.1/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `pymongoarrow-1.0.0/test/utils.py` & `pymongoarrow-1.0.1/test/utils.py`

 * *Files identical despite different names*

