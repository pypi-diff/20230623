# Comparing `tmp/qps_limit-1.0.1-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4964 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jun-23 02:21 qps_limit/__init__.py
+Zip file size: 4969 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jun-23 02:46 qps_limit/__init__.py
 -rw-rw-r--  2.0 unx     4665 b- defN 23-Jun-23 02:19 qps_limit/limiter.py
 -rw-rw-r--  2.0 unx     4335 b- defN 23-Jun-23 02:19 qps_limit/run.py
--rw-rw-r--  2.0 unx     2489 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/RECORD
-8 files, 12378 bytes uncompressed, 3880 bytes compressed:  68.7%
+-rw-rw-r--  2.0 unx     2509 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jun-23 02:46 qps_limit-1.0.2.dist-info/RECORD
+8 files, 12398 bytes uncompressed, 3885 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.1.dist-info/METADATA
+Filename: qps_limit-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.1.dist-info/WHEEL
+Filename: qps_limit-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.1.dist-info/top_level.txt
+Filename: qps_limit-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.1.dist-info/zip-safe
+Filename: qps_limit-1.0.2.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.1.dist-info/RECORD
+Filename: qps_limit-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 from .run import batch_run, async_batch_run
 from .limiter import Limiter
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## Comparing `qps_limit-1.0.1.dist-info/METADATA` & `qps_limit-1.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
+Requires-Dist: tqdm
 Requires-Dist: aiolimiter
 
 ## QPS Limit
 
 Run functions under any limited rate using `multiprocessing` + `asyncio`
 
 ### Installation
```

## Comparing `qps_limit-1.0.1.dist-info/RECORD` & `qps_limit-1.0.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-qps_limit/__init__.py,sha256=A760JpJfCpJVpoXvSnAcwjR0yGBWbvMuacKJ1JpebA0,165
+qps_limit/__init__.py,sha256=TxgSqfPfDDFECLzgdUiE2F2CBDqR4ay9uyfdJbbSkaI,165
 qps_limit/limiter.py,sha256=fDvhBmLwwwIYNdIl6Alco0mkEwiOnV2h4ZnePTADpWg,4665
 qps_limit/run.py,sha256=7osK_VGsB0IVEP6J_pHeBhmAxuH9RZTMCnsmFHgyjdE,4335
-qps_limit-1.0.1.dist-info/METADATA,sha256=G3aVD32O6j_lsQ_J1MfyYUtFEPDCsjGKva9j4_E3v8k,2489
-qps_limit-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-qps_limit-1.0.1.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
-qps_limit-1.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-qps_limit-1.0.1.dist-info/RECORD,,
+qps_limit-1.0.2.dist-info/METADATA,sha256=-Cye1b-w0o-jGB0SlD2AzW1nPA_1wCEiaZ4d9VCWchM,2509
+qps_limit-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+qps_limit-1.0.2.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
+qps_limit-1.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+qps_limit-1.0.2.dist-info/RECORD,,
```

