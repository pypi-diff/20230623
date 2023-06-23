# Comparing `tmp/seqdata-0.1.0.tar.gz` & `tmp/seqdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqdata-0.1.0.tar", max compression
+gzip compressed data, was "seqdata-0.1.1.tar", max compression
```

## Comparing `seqdata-0.1.0.tar` & `seqdata-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      844 2023-06-23 19:00:15.000000 seqdata-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1355 2023-06-23 18:57:24.000000 seqdata-0.1.0/seqdata/__init__.py
--rw-r--r--   0        0        0     2412 2023-06-21 21:41:12.000000 seqdata-0.1.0/seqdata/_dataload/_SequenceDataset.py
--rw-r--r--   0        0        0      981 2023-06-21 21:41:12.000000 seqdata-0.1.0/seqdata/_deprecated.py
--rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.1.0/seqdata/_io/__init__.py
--rw-r--r--   0        0        0    10816 2023-06-21 17:40:21.000000 seqdata-0.1.0/seqdata/_io/bed_ops.py
--rw-r--r--   0        0        0     4943 2023-06-21 17:40:21.000000 seqdata-0.1.0/seqdata/_io/read.py
--rw-r--r--   0        0        0      206 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/__init__.py
--rw-r--r--   0        0        0    11173 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/bam.py
--rw-r--r--   0        0        0    10022 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/fasta.py
--rw-r--r--   0        0        0     6152 2023-06-21 17:40:21.000000 seqdata-0.1.0/seqdata/_io/readers/table.py
--rw-r--r--   0        0        0    13505 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/vcf.py
--rw-r--r--   0        0        0     9706 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/readers/wig.py
--rw-r--r--   0        0        0     2705 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/_io/utils.py
--rw-r--r--   0        0        0     9375 2023-06-21 22:49:16.000000 seqdata-0.1.0/seqdata/torch.py
--rw-r--r--   0        0        0     2281 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/types.py
--rw-r--r--   0        0        0    12620 2023-06-21 21:41:12.000000 seqdata-0.1.0/seqdata/xarray/seqdata.py
--rw-r--r--   0        0        0      901 2023-06-14 18:50:23.000000 seqdata-0.1.0/seqdata/xarray/utils.py
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 seqdata-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      861 2023-06-23 20:14:19.000000 seqdata-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1355 2023-06-23 18:57:24.000000 seqdata-0.1.1/seqdata/__init__.py
+-rw-r--r--   0        0        0     2412 2023-06-21 21:41:12.000000 seqdata-0.1.1/seqdata/_dataload/_SequenceDataset.py
+-rw-r--r--   0        0        0      981 2023-06-21 21:41:12.000000 seqdata-0.1.1/seqdata/_deprecated.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:18:07.000000 seqdata-0.1.1/seqdata/_io/__init__.py
+-rw-r--r--   0        0        0    10816 2023-06-21 17:40:21.000000 seqdata-0.1.1/seqdata/_io/bed_ops.py
+-rw-r--r--   0        0        0     4943 2023-06-21 17:40:21.000000 seqdata-0.1.1/seqdata/_io/read.py
+-rw-r--r--   0        0        0      206 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/__init__.py
+-rw-r--r--   0        0        0    11173 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/bam.py
+-rw-r--r--   0        0        0    10022 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/fasta.py
+-rw-r--r--   0        0        0     6152 2023-06-21 17:40:21.000000 seqdata-0.1.1/seqdata/_io/readers/table.py
+-rw-r--r--   0        0        0    13505 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/vcf.py
+-rw-r--r--   0        0        0     9706 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/readers/wig.py
+-rw-r--r--   0        0        0     2705 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/_io/utils.py
+-rw-r--r--   0        0        0     9375 2023-06-21 22:49:16.000000 seqdata-0.1.1/seqdata/torch.py
+-rw-r--r--   0        0        0     2281 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/types.py
+-rw-r--r--   0        0        0    12620 2023-06-21 21:41:12.000000 seqdata-0.1.1/seqdata/xarray/seqdata.py
+-rw-r--r--   0        0        0      901 2023-06-14 18:50:23.000000 seqdata-0.1.1/seqdata/xarray/utils.py
+-rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 seqdata-0.1.1/PKG-INFO
```

### Comparing `seqdata-0.1.0/pyproject.toml` & `seqdata-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqdata"
-version = "0.1.0"
+version = "0.1.1"
 description = "Annotated sequence data"
 authors = ["adamklie <aklie@ucsd.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyranges = "^0.0.120"
 xarray = "2023.4.0"
@@ -20,14 +20,15 @@
 joblib = "^1.1.0"
 natsort = "^8.3.1"
 numpy = "~1.23.5"
 pandas = "^1.5.2"
 numcodecs = "^0.11.0"
 typing-extensions = "^4.5.0"
 tqdm = "^4.65.0"
+seqpro = "0.1.1"
 torch = {version = "^1.12.0", extras = ["torch"]}
 
 [tool.poetry.extras]
 torch = ["torch"]
 
 [tool.poetry.dev-dependencies]
```

### Comparing `seqdata-0.1.0/seqdata/__init__.py` & `seqdata-0.1.1/seqdata/__init__.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_dataload/_SequenceDataset.py` & `seqdata-0.1.1/seqdata/_dataload/_SequenceDataset.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_deprecated.py` & `seqdata-0.1.1/seqdata/_deprecated.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/bed_ops.py` & `seqdata-0.1.1/seqdata/_io/bed_ops.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/read.py` & `seqdata-0.1.1/seqdata/_io/read.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/readers/bam.py` & `seqdata-0.1.1/seqdata/_io/readers/bam.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/readers/fasta.py` & `seqdata-0.1.1/seqdata/_io/readers/fasta.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/readers/table.py` & `seqdata-0.1.1/seqdata/_io/readers/table.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/readers/vcf.py` & `seqdata-0.1.1/seqdata/_io/readers/vcf.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/readers/wig.py` & `seqdata-0.1.1/seqdata/_io/readers/wig.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/_io/utils.py` & `seqdata-0.1.1/seqdata/_io/utils.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/torch.py` & `seqdata-0.1.1/seqdata/torch.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/types.py` & `seqdata-0.1.1/seqdata/types.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/xarray/seqdata.py` & `seqdata-0.1.1/seqdata/xarray/seqdata.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/seqdata/xarray/utils.py` & `seqdata-0.1.1/seqdata/xarray/utils.py`

 * *Files identical despite different names*

### Comparing `seqdata-0.1.0/PKG-INFO` & `seqdata-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Annotated sequence data
 Author: adamklie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,12 +20,13 @@
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pandera (>=0.14.5,<0.15.0)
 Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: pyBigWig (>=0.3.22,<0.4.0)
 Requires-Dist: pybedtools (>=0.9.0,<0.10.0)
 Requires-Dist: pyranges (>=0.0.120,<0.0.121)
 Requires-Dist: pysam (>=0.21.0,<0.22.0)
+Requires-Dist: seqpro (==0.1.1)
 Requires-Dist: torch[torch] (>=1.12.0,<2.0.0) ; extra == "torch"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: xarray (==2023.4.0)
 Requires-Dist: zarr (>=2.14.2,<3.0.0)
```

