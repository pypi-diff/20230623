# Comparing `tmp/xnattagger-0.4.6-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.4.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6417 bytes, number of entries: 10
+Zip file size: 6412 bytes, number of entries: 10
 -rw-r--r--  2.0 unx    12743 b- defN 23-Jun-23 16:31 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 17:37 xnattagger/__version__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 17:41 xnattagger/__version__.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 16:36 xnattagger/config/__init__.py
 -rw-r--r--  2.0 unx     1449 b- defN 23-Jun-23 16:35 xnattagger/config/tagger.yaml
--rwxr-xr-x  2.0 unx     2306 b- defN 23-Jun-23 17:38 xnattagger-0.4.6.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 17:38 xnattagger-0.4.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 17:38 xnattagger-0.4.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 17:38 xnattagger-0.4.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 17:38 xnattagger-0.4.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 17:38 xnattagger-0.4.6.dist-info/RECORD
-10 files, 19684 bytes uncompressed, 4989 bytes compressed:  74.7%
+-rwxr-xr-x  2.0 unx     2276 b- defN 23-Jun-23 17:42 xnattagger-0.4.7.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 17:42 xnattagger-0.4.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 17:42 xnattagger-0.4.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 17:42 xnattagger-0.4.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 17:42 xnattagger-0.4.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 17:42 xnattagger-0.4.7.dist-info/RECORD
+10 files, 19654 bytes uncompressed, 4984 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: xnattagger/config/__init__.py
 Comment: 
 
 Filename: xnattagger/config/tagger.yaml
 Comment: 
 
-Filename: xnattagger-0.4.6.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.4.7.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.4.6.dist-info/LICENSE
+Filename: xnattagger-0.4.7.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.4.6.dist-info/METADATA
+Filename: xnattagger-0.4.7.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.4.6.dist-info/WHEEL
+Filename: xnattagger-0.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.4.6.dist-info/top_level.txt
+Filename: xnattagger-0.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.4.6.dist-info/RECORD
+Filename: xnattagger-0.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.4.6'
+__version__ = '0.4.7'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.4.6.data/scripts/xnat_tagger.py` & `xnattagger-0.4.7.data/scripts/xnat_tagger.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 import xnattagger.config as config 
 
 logger = logging.getLogger(os.path.basename(__file__))
 logging.basicConfig(level=logging.INFO)
 
 yaml.add_representer(collections.defaultdict, Representer.represent_dict)
 
-conf_file = config.default()
 
 def main():
     # Parse command line arguments
     parser = ap.ArgumentParser()
-    parser.add_argument('-a', '--alias', required=True,
+    parser.add_argument('--xnat-alias', required=True,
         help='XNAT alias')  # Set default value and provide help text for alias argument
     parser.add_argument('--project',
         help='XNAT project')  # Provide help text for project argument
     parser.add_argument('-c', '--cache', action='store_true',
         help='Speed up development by caching yaxil.scans output')  # Provide help text for cache argument
     parser.add_argument('-o', '--output-file',
         help='Output summary of updates')  # Provide help text for output-file argument
```

## Comparing `xnattagger-0.4.6.dist-info/LICENSE` & `xnattagger-0.4.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.4.6.dist-info/RECORD` & `xnattagger-0.4.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xnattagger/__init__.py,sha256=Sxh2X6lBgvqEcJZx2BVuwW75k-EmXwxYv998zGyVHmA,12743
-xnattagger/__version__.py,sha256=rYDETD8kOhVyEsOHLjXfs4zs_TIHkk8dt4y9aiH0wx4,220
+xnattagger/__version__.py,sha256=XTJ8PIuBvwWUeApEthTIkS2ndofTy1J9vgEO4bLFTuM,220
 xnattagger/config/__init__.py,sha256=9NvVYPkoanrrNVRCljmYCAjjJZGq5kvF_oatEgVQDQo,160
 xnattagger/config/tagger.yaml,sha256=pg1jkPEr0wcv0Dz9SzwqCHuC8E_vztjM-OUkd4tt-Mo,1449
-xnattagger-0.4.6.data/scripts/xnat_tagger.py,sha256=N_BHaMcNUY2TqiJCjQDF3CvoLXpqCboKNnx9zusT2y4,2306
-xnattagger-0.4.6.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.4.6.dist-info/METADATA,sha256=XC6apt5fJIr_gZLFpnKgabekv7Z2yqR5rO69sd_PvYQ,310
-xnattagger-0.4.6.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-xnattagger-0.4.6.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.4.6.dist-info/RECORD,,
+xnattagger-0.4.7.data/scripts/xnat_tagger.py,sha256=j-Tow5NnJjFrD9X91EU89T3m9mKOQrBmK319FwbN5EE,2276
+xnattagger-0.4.7.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.4.7.dist-info/METADATA,sha256=ZWsDdiDHGx_G6vVBEVuC8TDj4c72HLYf7eJOTJ57Ogk,310
+xnattagger-0.4.7.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+xnattagger-0.4.7.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.4.7.dist-info/RECORD,,
```

