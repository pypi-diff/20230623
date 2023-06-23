# Comparing `tmp/xnattagger-0.3.0-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 5630 bytes, number of entries: 8
--rw-r--r--  2.0 unx    12743 b- defN 23-Apr-20 16:35 xnattagger/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-20 16:36 xnattagger/__version__.py
--rwxr-xr-x  2.0 unx     2178 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.data/scripts/xnat_tagger.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      289 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      663 b- defN 23-Apr-20 16:36 xnattagger-0.3.0.dist-info/RECORD
-8 files, 17755 bytes uncompressed, 4470 bytes compressed:  74.8%
+Zip file size: 6413 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    12743 b- defN 23-Jun-23 16:31 xnattagger/__init__.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-23 16:40 xnattagger/__version__.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 16:36 xnattagger/config/__init__.py
+-rw-r--r--  2.0 unx     1449 b- defN 23-Jun-23 16:35 xnattagger/config/tagger.yaml
+-rwxr-xr-x  2.0 unx     2296 b- defN 23-Jun-23 16:40 xnattagger-0.4.0.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-23 16:40 xnattagger-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      310 b- defN 23-Jun-23 16:40 xnattagger-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-23 16:40 xnattagger-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 16:40 xnattagger-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      834 b- defN 23-Jun-23 16:40 xnattagger-0.4.0.dist-info/RECORD
+10 files, 19674 bytes uncompressed, 4985 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: xnattagger/__init__.py
 Comment: 
 
 Filename: xnattagger/__version__.py
 Comment: 
 
-Filename: xnattagger-0.3.0.data/scripts/xnat_tagger.py
+Filename: xnattagger/config/__init__.py
 Comment: 
 
-Filename: xnattagger-0.3.0.dist-info/LICENSE
+Filename: xnattagger/config/tagger.yaml
 Comment: 
 
-Filename: xnattagger-0.3.0.dist-info/METADATA
+Filename: xnattagger-0.4.0.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.3.0.dist-info/WHEEL
+Filename: xnattagger-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.3.0.dist-info/top_level.txt
+Filename: xnattagger-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.3.0.dist-info/RECORD
+Filename: xnattagger-0.4.0.dist-info/WHEEL
+Comment: 
+
+Filename: xnattagger-0.4.0.dist-info/top_level.txt
+Comment: 
+
+Filename: xnattagger-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.3.0.data/scripts/xnat_tagger.py` & `xnattagger-0.4.0.data/scripts/xnat_tagger.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import requests
 import collections
 import argparse as ap
 from io import StringIO
 from yaml.representer import Representer
 from yaxil.exceptions import NoExperimentsError
 from xnattagger import Tagger
+import xnattagger.config as config 
 
 logger = logging.getLogger(os.path.basename(__file__))
 logging.basicConfig(level=logging.INFO)
 
 yaml.add_representer(collections.defaultdict, Representer.represent_dict)
 
 def main():
@@ -32,18 +33,19 @@
         help='Speed up development by caching yaxil.scans output')  # Provide help text for cache argument
     parser.add_argument('-o', '--output-file',
         help='Output summary of updates')  # Provide help text for output-file argument
     parser.add_argument('--dry-run', action='store_true',
         help='Do not execute updates')  # Provide help text for dry-run argument
     parser.add_argument('--confirm', action='store_true',
         help='Prompt user to confirm every update')  # Provide help text for confirm argument
-    parser.add_argument('--filters', required=True,
+    parser.add_argument('--filters', default=config.default(), required=True,
         help='Filters configuration file') 
     parser.add_argument('--target', choices=['t1', 't2', 'dwi', 'bold', 'all'], required=True, type=str.lower) # Require --target argument
-    parser.add_argument('session')  # Require session argument
+    parser.add_argument('--label', required=True,
+        help='Label of XNAT MR Session')  # Require session argument
     args = parser.parse_args()
 
     with open(args.filters) as fo:
         filters = yaml.load(fo, Loader=yaml.SafeLoader)
 
     tagger = Tagger(args.alias, filters, args.target, args.session)
     tagger.generate_updates()
```

## Comparing `xnattagger-0.3.0.dist-info/LICENSE` & `xnattagger-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.3.0.dist-info/RECORD` & `xnattagger-0.4.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 xnattagger/__init__.py,sha256=Sxh2X6lBgvqEcJZx2BVuwW75k-EmXwxYv998zGyVHmA,12743
-xnattagger/__version__.py,sha256=C94hqL0zL9ep3vaWTYO4GT2X6huqZOWgiAQ-xM9WRn4,220
-xnattagger-0.3.0.data/scripts/xnat_tagger.py,sha256=s_2_DR2BPYOXMIdsDYX25W2UaNAS0Nr6u3RD9p-aJi8,2178
-xnattagger-0.3.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.3.0.dist-info/METADATA,sha256=z1qXeLOF4FG0s1t8l6NLtnhNAaVVlaARkxnpqDXaU24,289
-xnattagger-0.3.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-xnattagger-0.3.0.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.3.0.dist-info/RECORD,,
+xnattagger/__version__.py,sha256=XFhH-AwtiKz0HtTjwfOxKok8zcEzCa5W9QeJeCkv4vQ,220
+xnattagger/config/__init__.py,sha256=9NvVYPkoanrrNVRCljmYCAjjJZGq5kvF_oatEgVQDQo,160
+xnattagger/config/tagger.yaml,sha256=pg1jkPEr0wcv0Dz9SzwqCHuC8E_vztjM-OUkd4tt-Mo,1449
+xnattagger-0.4.0.data/scripts/xnat_tagger.py,sha256=oZjjM-eVhyWU_9lydTTOoSEvB6tE4fJUKMlC8TnOyzo,2296
+xnattagger-0.4.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.4.0.dist-info/METADATA,sha256=IkO0rsf0nUvS7MkrtidBuVmEGZqNH5UF8Q8b-cnEWek,310
+xnattagger-0.4.0.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+xnattagger-0.4.0.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.4.0.dist-info/RECORD,,
```

