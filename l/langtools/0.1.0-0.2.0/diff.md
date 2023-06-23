# Comparing `tmp/langtools-0.1.0-py3-none-any.whl.zip` & `tmp/langtools-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2539 bytes, number of entries: 6
--rw-r--r--  2.0 unx       36 b- defN 80-Jan-01 00:00 langtools/__init__.py
+Zip file size: 4779 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      100 b- defN 80-Jan-01 00:00 langtools/__init__.py
+-rw-r--r--  2.0 unx     1973 b- defN 80-Jan-01 00:00 langtools/pornhub.py
+-rw-r--r--  2.0 unx     3002 b- defN 80-Jan-01 00:00 langtools/visa.py
 -rw-r--r--  2.0 unx      630 b- defN 80-Jan-01 00:00 langtools/web_browser.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 langtools-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      586 b- defN 80-Jan-01 00:00 langtools-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 langtools-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      457 b- defN 16-Jan-01 00:00 langtools-0.1.0.dist-info/RECORD
-6 files, 2863 bytes uncompressed, 1711 bytes compressed:  40.2%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 langtools-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 langtools-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 langtools-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      609 b- defN 16-Jan-01 00:00 langtools-0.2.0.dist-info/RECORD
+8 files, 8184 bytes uncompressed, 3725 bytes compressed:  54.5%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: langtools/__init__.py
 Comment: 
 
+Filename: langtools/pornhub.py
+Comment: 
+
+Filename: langtools/visa.py
+Comment: 
+
 Filename: langtools/web_browser.py
 Comment: 
 
-Filename: langtools-0.1.0.dist-info/LICENSE
+Filename: langtools-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: langtools-0.1.0.dist-info/METADATA
+Filename: langtools-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: langtools-0.1.0.dist-info/WHEEL
+Filename: langtools-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: langtools-0.1.0.dist-info/RECORD
+Filename: langtools-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langtools/__init__.py

```diff
@@ -1 +1,3 @@
+from .pornhub import PornHubSearch
+from .visa import VISAFXRate
 from .web_browser import WebBrowser
```

## Comparing `langtools-0.1.0.dist-info/LICENSE` & `langtools-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langtools-0.1.0.dist-info/METADATA` & `langtools-0.2.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: langtools
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: なるみ
 Author-email: toucans-cutouts0f@icloud.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: cloudscraper (>=1.2.71,<2.0.0)
 Requires-Dist: langchain (>=0.0.209,<0.0.210)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pornhub-api (>=0.3.0,<0.4.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: retry (>=0.9.2,<0.10.0)
 Description-Content-Type: text/markdown
 
 # langtools
```

