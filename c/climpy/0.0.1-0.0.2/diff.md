# Comparing `tmp/climpy-0.0.1-py3-none-any.whl.zip` & `tmp/climpy-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 10219 bytes, number of entries: 17
+Zip file size: 10220 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 climpy/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 climpy/metric/__init__.py
 -rw-r--r--  2.0 unx     1650 b- defN 20-Feb-02 00:00 climpy/metric/metric.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 climpy/ml_data/__init__.py
 -rw-r--r--  2.0 unx      220 b- defN 20-Feb-02 00:00 climpy/ml_data/data.py
 -rw-r--r--  2.0 unx     2888 b- defN 20-Feb-02 00:00 climpy/transform/condition.py
 -rw-r--r--  2.0 unx      915 b- defN 20-Feb-02 00:00 climpy/transform/criterion.py
 -rw-r--r--  2.0 unx     3543 b- defN 20-Feb-02 00:00 climpy/transform/event.py
 -rw-r--r--  2.0 unx     2329 b- defN 20-Feb-02 00:00 climpy/transform/hazard.py
 -rw-r--r--  2.0 unx     1354 b- defN 20-Feb-02 00:00 climpy/transform/link.py
 -rw-r--r--  2.0 unx     2881 b- defN 20-Feb-02 00:00 climpy/transform/select.py
 -rw-r--r--  2.0 unx      879 b- defN 20-Feb-02 00:00 climpy/transform/utils.py
 -rw-r--r--  2.0 unx      622 b- defN 20-Feb-02 00:00 climpy/transform/specialized/flood_criterion.py
-?rw-r--r--  2.0 unx     2316 b- defN 20-Feb-02 00:00 climpy-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 climpy-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1498 b- defN 20-Feb-02 00:00 climpy-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1372 b- defN 20-Feb-02 00:00 climpy-0.0.1.dist-info/RECORD
-17 files, 22554 bytes uncompressed, 7961 bytes compressed:  64.7%
+?rw-r--r--  2.0 unx     2316 b- defN 20-Feb-02 00:00 climpy-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 climpy-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1498 b- defN 20-Feb-02 00:00 climpy-0.0.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1372 b- defN 20-Feb-02 00:00 climpy-0.0.2.dist-info/RECORD
+17 files, 22554 bytes uncompressed, 7962 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: climpy/transform/utils.py
 Comment: 
 
 Filename: climpy/transform/specialized/flood_criterion.py
 Comment: 
 
-Filename: climpy-0.0.1.dist-info/METADATA
+Filename: climpy-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: climpy-0.0.1.dist-info/WHEEL
+Filename: climpy-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: climpy-0.0.1.dist-info/licenses/LICENSE
+Filename: climpy-0.0.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: climpy-0.0.1.dist-info/RECORD
+Filename: climpy-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `climpy-0.0.1.dist-info/METADATA` & `climpy-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Climate Data related tools in Python
 Project-URL: Homepage, https://github.com/ClimAI/climpy
 Project-URL: Bug Tracker, https://github.com/ClimAI/climpy/issues
 Author-email: Mohit Anand <mohit@climai.earth>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `climpy-0.0.1.dist-info/licenses/LICENSE` & `climpy-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `climpy-0.0.1.dist-info/RECORD` & `climpy-0.0.2.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 climpy/transform/criterion.py,sha256=dkuscEAU0ZDnqb6ihnynqw5HLnALFJcSQcH32GnatPA,915
 climpy/transform/event.py,sha256=J7EzPJKMpKYmKm6SWQacyN_bDDvssXd2SyGfPTMRvDQ,3543
 climpy/transform/hazard.py,sha256=3oZHJDzpLbD07rb4vGn1H3lFXx4NGEq1cP7DAUQx5rU,2329
 climpy/transform/link.py,sha256=hmrO7xX0cdQ4INePEAiLJIcQP71rjslwIHEbfKQGY40,1354
 climpy/transform/select.py,sha256=cfrcpt2THR_pwSyFdnEyktakh3pdHEmc5HYF0pNdhIc,2881
 climpy/transform/utils.py,sha256=m2eJq2Tph6tSeLHj2A2ECgigJfl2Ph082C-7ibAMoJ0,879
 climpy/transform/specialized/flood_criterion.py,sha256=wXVW6P18ig4_txyJl3Z-4wFCUnnuO4nmNJx1IpXBw40,622
-climpy-0.0.1.dist-info/METADATA,sha256=e3-_YpFe4G7D9nqtSGTOFbZjX4eIn9uePurqDkUv1UM,2316
-climpy-0.0.1.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-climpy-0.0.1.dist-info/licenses/LICENSE,sha256=DgR2QRFXJud27dSfcdMBfyXNdWoaTvdB9s4teXXnl84,1498
-climpy-0.0.1.dist-info/RECORD,,
+climpy-0.0.2.dist-info/METADATA,sha256=oEpN2pk4oJdBmBPP-jh0Do6NsQ2XH8XAlUaI_OrKcDU,2316
+climpy-0.0.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+climpy-0.0.2.dist-info/licenses/LICENSE,sha256=DgR2QRFXJud27dSfcdMBfyXNdWoaTvdB9s4teXXnl84,1498
+climpy-0.0.2.dist-info/RECORD,,
```

