# Comparing `tmp/xnattagger-0.4.4-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.4.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6420 bytes, number of entries: 10
+Zip file size: 6435 bytes, number of entries: 10
 -rw-r--r--  2.0 unx    12743 b- defN 23-Jun-23 16:31 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 16:54 xnattagger/__version__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 17:24 xnattagger/__version__.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 16:36 xnattagger/config/__init__.py
 -rw-r--r--  2.0 unx     1449 b- defN 23-Jun-23 16:35 xnattagger/config/tagger.yaml
--rwxr-xr-x  2.0 unx     2287 b- defN 23-Jun-23 16:55 xnattagger-0.4.4.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 16:55 xnattagger-0.4.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 16:55 xnattagger-0.4.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 16:55 xnattagger-0.4.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 16:55 xnattagger-0.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 16:55 xnattagger-0.4.4.dist-info/RECORD
-10 files, 19665 bytes uncompressed, 4992 bytes compressed:  74.6%
+-rwxr-xr-x  2.0 unx     2334 b- defN 23-Jun-23 17:25 xnattagger-0.4.5.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 17:25 xnattagger-0.4.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 17:25 xnattagger-0.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 17:25 xnattagger-0.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 17:25 xnattagger-0.4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 17:25 xnattagger-0.4.5.dist-info/RECORD
+10 files, 19712 bytes uncompressed, 5007 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: xnattagger/config/__init__.py
 Comment: 
 
 Filename: xnattagger/config/tagger.yaml
 Comment: 
 
-Filename: xnattagger-0.4.4.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.4.5.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.4.4.dist-info/LICENSE
+Filename: xnattagger-0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.4.4.dist-info/METADATA
+Filename: xnattagger-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.4.4.dist-info/WHEEL
+Filename: xnattagger-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.4.4.dist-info/top_level.txt
+Filename: xnattagger-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.4.4.dist-info/RECORD
+Filename: xnattagger-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.4.4'
+__version__ = '0.4.5'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.4.4.data/scripts/xnat_tagger.py` & `xnattagger-0.4.5.data/scripts/xnat_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 import xnattagger.config as config 
 
 logger = logging.getLogger(os.path.basename(__file__))
 logging.basicConfig(level=logging.INFO)
 
 yaml.add_representer(collections.defaultdict, Representer.represent_dict)
 
+conf_file = config.default()
+print(conf_file)
+
 def main():
     # Parse command line arguments
     parser = ap.ArgumentParser()
     parser.add_argument('-a', '--alias', required=True,
         help='XNAT alias')  # Set default value and provide help text for alias argument
     parser.add_argument('--project',
         help='XNAT project')  # Provide help text for project argument
@@ -35,15 +38,15 @@
         help='Output summary of updates')  # Provide help text for output-file argument
     parser.add_argument('--dry-run', action='store_true',
         help='Do not execute updates')  # Provide help text for dry-run argument
     parser.add_argument('--confirm', action='store_true',
         help='Prompt user to confirm every update')  # Provide help text for confirm argument
     parser.add_argument('--filters', default=config.default(),
         help='Filters configuration file') 
-    parser.add_argument('--target', choices=['t1', 't2', 'dwi', 'bold', 'all'], nargs="+" ,required=True, type=str.lower) # Require --target argument
+    parser.add_argument('--target', choices=['t1', 't2', 'dwi', 'bold', 'all'], nargs="+", required=True, type=str.lower) # Require --target argument
     parser.add_argument('--label', required=True,
         help='Label of XNAT MR Session')  # Require label argument
     args = parser.parse_args()
 
     with open(args.filters) as fo:
         filters = yaml.load(fo, Loader=yaml.SafeLoader)
```

## Comparing `xnattagger-0.4.4.dist-info/LICENSE` & `xnattagger-0.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.4.4.dist-info/RECORD` & `xnattagger-0.4.5.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xnattagger/__init__.py,sha256=Sxh2X6lBgvqEcJZx2BVuwW75k-EmXwxYv998zGyVHmA,12743
-xnattagger/__version__.py,sha256=sj9D8sbrDLbsjEJ65VttTvNGLYbGexscgbLwusEHuew,220
+xnattagger/__version__.py,sha256=0d8XWtPCH-ie84eABUhZ5Ez4jNPHT6VGFkv9Wg6oLow,220
 xnattagger/config/__init__.py,sha256=9NvVYPkoanrrNVRCljmYCAjjJZGq5kvF_oatEgVQDQo,160
 xnattagger/config/tagger.yaml,sha256=pg1jkPEr0wcv0Dz9SzwqCHuC8E_vztjM-OUkd4tt-Mo,1449
-xnattagger-0.4.4.data/scripts/xnat_tagger.py,sha256=-6XsxLGRNNsY7GGUGhkQ44RoKtzLhSAwssgZ-73nmF8,2287
-xnattagger-0.4.4.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.4.4.dist-info/METADATA,sha256=BalgU18qddBgyGcPmMLx2J7P_eAPvWsyf49fPKwiHl0,310
-xnattagger-0.4.4.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-xnattagger-0.4.4.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.4.4.dist-info/RECORD,,
+xnattagger-0.4.5.data/scripts/xnat_tagger.py,sha256=zg20b0ziDxQwQeC9a9Xqz_cDF-_vHMsHR-SyXFWcodY,2334
+xnattagger-0.4.5.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.4.5.dist-info/METADATA,sha256=YAcDvjqv6GHwCxmJEGVXi3VQVFsRlo5ARmde_KASeBI,310
+xnattagger-0.4.5.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+xnattagger-0.4.5.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.4.5.dist-info/RECORD,,
```

