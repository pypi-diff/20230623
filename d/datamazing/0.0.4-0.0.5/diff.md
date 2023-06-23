# Comparing `tmp/datamazing-0.0.4.tar.gz` & `tmp/datamazing-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-0.0.4.tar", max compression
+gzip compressed data, was "datamazing-0.0.5.tar", max compression
```

## Comparing `datamazing-0.0.4.tar` & `datamazing-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       21 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/__init__.py
--rw-r--r--   0        0        0      185 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/datacollection/__init__.py
--rw-r--r--   0        0        0      226 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0       99 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      826 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     2222 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     1998 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0      868 2023-06-23 06:41:51.879338 datamazing-0.0.4/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      690 2023-06-23 06:41:51.879338 datamazing-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/__init__.py
+-rw-r--r--   0        0        0      258 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0       99 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      826 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     2222 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     1998 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0      868 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-06-23 09:57:51.804855 datamazing-0.0.5/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      690 2023-06-23 09:57:51.804855 datamazing-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.5/PKG-INFO
```

### Comparing `datamazing-0.0.4/datamazing/pandas/testing/assertions.py` & `datamazing-0.0.5/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.4/datamazing/pandas/testing/data.py` & `datamazing-0.0.5/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.4/datamazing/pandas/transformations/basic.py` & `datamazing-0.0.5/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.4/datamazing/pandas/transformations/grouping.py` & `datamazing-0.0.5/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.4/datamazing/pandas/transformations/resampling.py` & `datamazing-0.0.5/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.4/pyproject.toml` & `datamazing-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "0.0.4"
+version = "0.0.5"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `datamazing-0.0.4/PKG-INFO` & `datamazing-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

