# Comparing `tmp/hat_json-0.5.8-cp38.cp39.cp310-none-any.whl.zip` & `tmp/hat_json-0.5.9-cp38.cp39.cp310-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 15424 bytes, number of entries: 16
--rw-r--r--  2.0 unx     1670 b- defN 22-May-16 15:17 hat/json/__init__.py
+Zip file size: 16860 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     1711 b- defN 22-Sep-18 13:09 hat/json/__init__.py
 -rw-r--r--  2.0 unx     2334 b- defN 22-May-16 14:57 hat/json/data.py
 -rw-r--r--  2.0 unx     4483 b- defN 22-Mar-10 23:19 hat/json/encoder.py
--rw-r--r--  2.0 unx     2385 b- defN 22-Jul-19 18:09 hat/json/json_schema_repo.json
+-rw-r--r--  2.0 unx     2385 b- defN 22-Sep-18 13:12 hat/json/json_schema_repo.json
 -rw-r--r--  2.0 unx     1833 b- defN 22-Mar-16 19:55 hat/json/patch.py
 -rw-r--r--  2.0 unx     5436 b- defN 22-May-16 15:17 hat/json/path.py
 -rw-r--r--  2.0 unx     6455 b- defN 22-Jul-16 14:36 hat/json/repository.py
+-rw-r--r--  2.0 unx     3426 b- defN 22-Sep-18 13:08 hat/json/vt.py
 -rw-r--r--  2.0 unx      272 b- defN 22-Mar-16 19:52 hat/json/validator/__init__.py
 -rw-r--r--  2.0 unx     1172 b- defN 22-May-16 15:07 hat/json/validator/common.py
 -rw-r--r--  2.0 unx      786 b- defN 22-May-16 15:07 hat/json/validator/jsonschema.py
--rw-r--r--  2.0 unx    11358 b- defN 22-Jul-19 18:09 hat_json-0.5.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1945 b- defN 22-Jul-19 18:09 hat_json-0.5.8.dist-info/METADATA
--rw-r--r--  2.0 unx      132 b- defN 22-Jul-19 18:09 hat_json-0.5.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-Jul-19 18:09 hat_json-0.5.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Jul-19 18:09 hat_json-0.5.8.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1277 b- defN 22-Jul-19 18:09 hat_json-0.5.8.dist-info/RECORD
-16 files, 41543 bytes uncompressed, 13332 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx    11358 b- defN 22-Sep-18 13:12 hat_json-0.5.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1945 b- defN 22-Sep-18 13:12 hat_json-0.5.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      132 b- defN 22-Sep-18 13:12 hat_json-0.5.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 22-Sep-18 13:12 hat_json-0.5.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 22-Sep-18 13:12 hat_json-0.5.9.dist-info/zip-safe
+?rw-rw-r--  2.0 unx     1348 b- defN 22-Sep-18 13:12 hat_json-0.5.9.dist-info/RECORD
+17 files, 45081 bytes uncompressed, 14664 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -15,35 +15,38 @@
 
 Filename: hat/json/path.py
 Comment: 
 
 Filename: hat/json/repository.py
 Comment: 
 
+Filename: hat/json/vt.py
+Comment: 
+
 Filename: hat/json/validator/__init__.py
 Comment: 
 
 Filename: hat/json/validator/common.py
 Comment: 
 
 Filename: hat/json/validator/jsonschema.py
 Comment: 
 
-Filename: hat_json-0.5.8.dist-info/LICENSE
+Filename: hat_json-0.5.9.dist-info/LICENSE
 Comment: 
 
-Filename: hat_json-0.5.8.dist-info/METADATA
+Filename: hat_json-0.5.9.dist-info/METADATA
 Comment: 
 
-Filename: hat_json-0.5.8.dist-info/WHEEL
+Filename: hat_json-0.5.9.dist-info/WHEEL
 Comment: 
 
-Filename: hat_json-0.5.8.dist-info/top_level.txt
+Filename: hat_json-0.5.9.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_json-0.5.8.dist-info/zip-safe
+Filename: hat_json-0.5.9.dist-info/zip-safe
 Comment: 
 
-Filename: hat_json-0.5.8.dist-info/RECORD
+Filename: hat_json-0.5.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/json/__init__.py

```diff
@@ -22,14 +22,15 @@
 from hat.json.patch import (diff,
                             patch)
 from hat.json.repository import (SchemaRepository,
                                  json_schema_repo)
 from hat.json.validator import (Validator,
                                 DefaultValidator,
                                 JsonSchemaValidator)
+from hat.json import vt
 
 
 __all__ = ['Array',
            'Object',
            'Data',
            'equals',
            'clone',
@@ -49,8 +50,9 @@
            'decode_stream',
            'diff',
            'patch',
            'SchemaRepository',
            'json_schema_repo',
            'Validator',
            'DefaultValidator',
-           'JsonSchemaValidator']
+           'JsonSchemaValidator',
+           'vt']
```

## Comparing `hat_json-0.5.8.dist-info/LICENSE` & `hat_json-0.5.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_json-0.5.8.dist-info/METADATA` & `hat_json-0.5.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hat-json
-Version: 0.5.8
+Version: 0.5.9
 Summary: Hat JSON library
 Home-page: https://github.com/hat-open/hat-json
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

## Comparing `hat_json-0.5.8.dist-info/RECORD` & `hat_json-0.5.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-hat/json/__init__.py,sha256=Ev4vTMdQ8_k6ABOByedrstgAW_tH1h_p7h0KC-UUS6c,1670
+hat/json/__init__.py,sha256=8KZOIEunBRe2RqWftqbJ6YxREMqS8MG9uLOIze1ub4U,1711
 hat/json/data.py,sha256=eU8PlK3EAQ4RPL64T6K10_y5_QRYvIpk_irhkEUm8HY,2334
 hat/json/encoder.py,sha256=nvyf7zhRC61KSBafMsJ4Q_fQdpFGnb7F7qrvQ3dgyHM,4483
 hat/json/json_schema_repo.json,sha256=BTYzpstgzLPlyUgH5nNfR8NAdXeklPKq0za_MHfH9qo,2385
 hat/json/patch.py,sha256=zwZ-9-KWqb13WrCbA4TWxYMldRUlIzq2QjrvXPtEGr4,1833
 hat/json/path.py,sha256=KekjPW3609Gx_L_F6vU9q1s8HryO-NyW8NS-X-Wdyjo,5436
 hat/json/repository.py,sha256=K_eqJxwqYRvZLNcnX1eEERmO1wWARrdtXeCcYyb-il0,6455
+hat/json/vt.py,sha256=AROrOi3T1o2LTOTLpXcreygzGqmExRL2YohvgjhiMMs,3426
 hat/json/validator/__init__.py,sha256=LS_ZzbG3vwvLolO103EvA0xs3rxBvbd9tK-HHxiC6cg,272
 hat/json/validator/common.py,sha256=OrD5i2sLcH8Cg-Fs-1radB1n4ySPo7F0_rc8sWGed-E,1172
 hat/json/validator/jsonschema.py,sha256=vI0m_9_o49R6D5qfLa8MIIsjyMNO0Wgd2hmuQWbzd04,786
-hat_json-0.5.8.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_json-0.5.8.dist-info/METADATA,sha256=C3oHmF6mbWvHxm2DyxW3z23NKowPTgUsWd_cBN02iQI,1945
-hat_json-0.5.8.dist-info/WHEEL,sha256=J6o_EVcUhZ99gpCSeF2DGIW9mETC6p0M-27vXCgDo6E,132
-hat_json-0.5.8.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_json-0.5.8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-hat_json-0.5.8.dist-info/RECORD,,
+hat_json-0.5.9.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_json-0.5.9.dist-info/METADATA,sha256=r6ChfkXz3NGwGC8cv_Vap3GJH1_RXF2cTv-64xbd8U4,1945
+hat_json-0.5.9.dist-info/WHEEL,sha256=J6o_EVcUhZ99gpCSeF2DGIW9mETC6p0M-27vXCgDo6E,132
+hat_json-0.5.9.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
+hat_json-0.5.9.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+hat_json-0.5.9.dist-info/RECORD,,
```

