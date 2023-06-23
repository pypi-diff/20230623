# Comparing `tmp/xnattagger-0.4.1-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.4.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6410 bytes, number of entries: 10
+Zip file size: 6411 bytes, number of entries: 10
 -rw-r--r--  2.0 unx    12743 b- defN 23-Jun-23 16:31 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 16:43 xnattagger/__version__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 16:45 xnattagger/__version__.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 16:36 xnattagger/config/__init__.py
 -rw-r--r--  2.0 unx     1449 b- defN 23-Jun-23 16:35 xnattagger/config/tagger.yaml
--rwxr-xr-x  2.0 unx     2281 b- defN 23-Jun-23 16:44 xnattagger-0.4.1.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 16:44 xnattagger-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 16:44 xnattagger-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 16:44 xnattagger-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 16:44 xnattagger-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 16:44 xnattagger-0.4.1.dist-info/RECORD
-10 files, 19659 bytes uncompressed, 4982 bytes compressed:  74.7%
+-rwxr-xr-x  2.0 unx     2277 b- defN 23-Jun-23 16:46 xnattagger-0.4.2.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 16:46 xnattagger-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 16:46 xnattagger-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 16:46 xnattagger-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 16:46 xnattagger-0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 16:46 xnattagger-0.4.2.dist-info/RECORD
+10 files, 19655 bytes uncompressed, 4983 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: xnattagger/config/__init__.py
 Comment: 
 
 Filename: xnattagger/config/tagger.yaml
 Comment: 
 
-Filename: xnattagger-0.4.1.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.4.2.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.4.1.dist-info/LICENSE
+Filename: xnattagger-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.4.1.dist-info/METADATA
+Filename: xnattagger-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.4.1.dist-info/WHEEL
+Filename: xnattagger-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.4.1.dist-info/top_level.txt
+Filename: xnattagger-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.4.1.dist-info/RECORD
+Filename: xnattagger-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.4.1.data/scripts/xnat_tagger.py` & `xnattagger-0.4.2.data/scripts/xnat_tagger.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,21 +37,21 @@
         help='Do not execute updates')  # Provide help text for dry-run argument
     parser.add_argument('--confirm', action='store_true',
         help='Prompt user to confirm every update')  # Provide help text for confirm argument
     parser.add_argument('--filters', default=config.default(),
         help='Filters configuration file') 
     parser.add_argument('--target', choices=['t1', 't2', 'dwi', 'bold', 'all'], required=True, type=str.lower) # Require --target argument
     parser.add_argument('--label', required=True,
-        help='Label of XNAT MR Session')  # Require session argument
+        help='Label of XNAT MR Session')  # Require label argument
     args = parser.parse_args()
 
     with open(args.filters) as fo:
         filters = yaml.load(fo, Loader=yaml.SafeLoader)
 
-    tagger = Tagger(args.alias, filters, args.target, args.session)
+    tagger = Tagger(args.alias, filters, args.target, args.label)
     tagger.generate_updates()
 
     if args.output_file:
         with open(args.output_file, 'w') as fo:
             js = json.dumps(tagger.updates, indent=2)
             fo.write(js)
     if not args.dry_run:
```

## Comparing `xnattagger-0.4.1.dist-info/LICENSE` & `xnattagger-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.4.1.dist-info/RECORD` & `xnattagger-0.4.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xnattagger/__init__.py,sha256=Sxh2X6lBgvqEcJZx2BVuwW75k-EmXwxYv998zGyVHmA,12743
-xnattagger/__version__.py,sha256=btTe84BPzb4N9qGyzfznRHXW6Z4m079TvgJSw1hxwCY,220
+xnattagger/__version__.py,sha256=DBPm2v3X5DyoYgcUtVQtOjodXDm29qJUChrtU5lAjfA,220
 xnattagger/config/__init__.py,sha256=9NvVYPkoanrrNVRCljmYCAjjJZGq5kvF_oatEgVQDQo,160
 xnattagger/config/tagger.yaml,sha256=pg1jkPEr0wcv0Dz9SzwqCHuC8E_vztjM-OUkd4tt-Mo,1449
-xnattagger-0.4.1.data/scripts/xnat_tagger.py,sha256=SN2NI-aUui1uvpZVaLbBeX_myG_K2NVn3fAiNTk62zw,2281
-xnattagger-0.4.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.4.1.dist-info/METADATA,sha256=COX8QQ1HcO0veIKlaQOv_ECj_ilkokGLORr11QvEE-4,310
-xnattagger-0.4.1.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-xnattagger-0.4.1.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.4.1.dist-info/RECORD,,
+xnattagger-0.4.2.data/scripts/xnat_tagger.py,sha256=SafnhdZfmH-IxBqRQdLjbYZgyNLDg1nEI8SzVPfTuI4,2277
+xnattagger-0.4.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.4.2.dist-info/METADATA,sha256=8zgIFPcZUn0Qe4ldQihJdczRd_h-on4-xUWcZscB8T4,310
+xnattagger-0.4.2.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+xnattagger-0.4.2.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.4.2.dist-info/RECORD,,
```

