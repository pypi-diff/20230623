# Comparing `tmp/easymaker-1.0.8-py3-none-any.whl.zip` & `tmp/easymaker-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 21565 bytes, number of entries: 30
+Zip file size: 21563 bytes, number of entries: 30
 -rw-r--r--  2.0 unx      850 b- defN 22-Dec-01 05:31 easymaker/__init__.py
 -rw-r--r--  2.0 unx      341 b- defN 22-Oct-20 00:49 easymaker/__main__.py
 -rw-r--r--  2.0 unx     2033 b- defN 22-Nov-04 02:59 easymaker/initializer.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-20 00:49 easymaker/api/__init__.py
 -rw-r--r--  2.0 unx    14081 b- defN 22-Dec-07 00:18 easymaker/api/api_sender.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-20 00:49 easymaker/cli/__init__.py
 -rw-r--r--  2.0 unx     3114 b- defN 22-Nov-04 02:59 easymaker/cli/cli.py
@@ -21,12 +21,12 @@
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-20 00:49 easymaker/log/__init__.py
 -rw-r--r--  2.0 unx     2051 b- defN 22-Nov-18 01:00 easymaker/log/logger.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-20 00:49 easymaker/storage/__init__.py
 -rw-r--r--  2.0 unx    10185 b- defN 22-Nov-18 01:00 easymaker/storage/objectstorage.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-20 00:49 easymaker/training/__init__.py
 -rw-r--r--  2.0 unx     2291 b- defN 22-Dec-01 05:31 easymaker/training/model.py
 -rw-r--r--  2.0 unx     4102 b- defN 22-Dec-23 01:02 easymaker/training/training.py
--rw-r--r--  2.0 unx     6359 b- defN 22-Dec-27 09:23 easymaker-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-27 09:23 easymaker-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Dec-27 09:23 easymaker-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2510 b- defN 22-Dec-27 09:23 easymaker-1.0.8.dist-info/RECORD
-30 files, 72393 bytes uncompressed, 17487 bytes compressed:  75.8%
+-rw-r--r--  2.0 unx     6382 b- defN 22-Dec-27 09:25 easymaker-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Dec-27 09:25 easymaker-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 22-Dec-27 09:25 easymaker-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2510 b- defN 22-Dec-27 09:25 easymaker-1.0.9.dist-info/RECORD
+30 files, 72416 bytes uncompressed, 17485 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: easymaker/training/model.py
 Comment: 
 
 Filename: easymaker/training/training.py
 Comment: 
 
-Filename: easymaker-1.0.8.dist-info/METADATA
+Filename: easymaker-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: easymaker-1.0.8.dist-info/WHEEL
+Filename: easymaker-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: easymaker-1.0.8.dist-info/top_level.txt
+Filename: easymaker-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: easymaker-1.0.8.dist-info/RECORD
+Filename: easymaker-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `easymaker-1.0.8.dist-info/METADATA` & `easymaker-1.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymaker
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI EasyMaker SDK for Python.
 Home-page: https://www.toast.com
 Author: NHN Cloud AI EasyMaker Services
 License: Apache License 2.0
 Keywords: NHN Cloud AI EasyMaker
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -30,15 +30,15 @@
 )
 
 # NHN Cloud ObjectStorage upload/download
 easymaker.download(
     easymaker_obs_uri='obs://api-storage.cloud.toast.com/v1/AUTH_{tenant_id}/{container_name}/{source_dir}',
     download_dir_path='./source_dir',
     username='username@nhn.com',
-    password='password'
+    password='nhn_object_storage_api_password'
 )
 easymaker.upload(
     easymaker_obs_uri='obs://api-storage.cloud.toast.com/v1/AUTH_{tenant_id}/{container_name}/{upload_path}',
     src_dir_path='./local_dir',
     username='username@nhn.com',
     password='nhn_object_storage_api_password'
 )
```

## Comparing `easymaker-1.0.8.dist-info/RECORD` & `easymaker-1.0.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 easymaker/log/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 easymaker/log/logger.py,sha256=oJjXODpVS41YJ4GRAJdIg3-aEpnD1Gki2d6iNL-O-us,2051
 easymaker/storage/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 easymaker/storage/objectstorage.py,sha256=o8y2oxVsawaJxJlVbHf66bCBCH3qTAkXYz24weqxxfQ,10185
 easymaker/training/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 easymaker/training/model.py,sha256=sB2PKorcqpxMtwWHb64Z2syh973KyLsfu8gcfckFDYw,2291
 easymaker/training/training.py,sha256=2st5tvDKPqSm2SbHjfd2qnp0i9tM7wAxwZ3P192STrA,4102
-easymaker-1.0.8.dist-info/METADATA,sha256=_Csf1slTwUlJ6bE0YzRj2hq2Jfer915TcdCxPdI9FQ0,6359
-easymaker-1.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-easymaker-1.0.8.dist-info/top_level.txt,sha256=SthDJDO4Mt-3-LR6xAI6s52ozV_O3Rmt0s0uTEos3cA,10
-easymaker-1.0.8.dist-info/RECORD,,
+easymaker-1.0.9.dist-info/METADATA,sha256=7O_E6nPp6gHGbj7ntdMaPJwXStoY8ijSpr_Q6jJLN4s,6382
+easymaker-1.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+easymaker-1.0.9.dist-info/top_level.txt,sha256=SthDJDO4Mt-3-LR6xAI6s52ozV_O3Rmt0s0uTEos3cA,10
+easymaker-1.0.9.dist-info/RECORD,,
```

