# Comparing `tmp/langtools-0.2.0-py3-none-any.whl.zip` & `tmp/langtools-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 4779 bytes, number of entries: 8
--rw-r--r--  2.0 unx      100 b- defN 80-Jan-01 00:00 langtools/__init__.py
--rw-r--r--  2.0 unx     1973 b- defN 80-Jan-01 00:00 langtools/pornhub.py
--rw-r--r--  2.0 unx     3002 b- defN 80-Jan-01 00:00 langtools/visa.py
+Zip file size: 5862 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      137 b- defN 80-Jan-01 00:00 langtools/__init__.py
+-rw-r--r--  2.0 unx     2408 b- defN 80-Jan-01 00:00 langtools/mortgage.py
+-rw-r--r--  2.0 unx     1974 b- defN 80-Jan-01 00:00 langtools/pornhub.py
+-rw-r--r--  2.0 unx     3003 b- defN 80-Jan-01 00:00 langtools/visa.py
 -rw-r--r--  2.0 unx      630 b- defN 80-Jan-01 00:00 langtools/web_browser.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 langtools-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 langtools-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 langtools-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      609 b- defN 16-Jan-01 00:00 langtools-0.2.0.dist-info/RECORD
-8 files, 8184 bytes uncompressed, 3725 bytes compressed:  54.5%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 langtools-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      757 b- defN 80-Jan-01 00:00 langtools-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 langtools-0.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      687 b- defN 16-Jan-01 00:00 langtools-0.3.0.dist-info/RECORD
+9 files, 10750 bytes uncompressed, 4690 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: langtools/__init__.py
 Comment: 
 
+Filename: langtools/mortgage.py
+Comment: 
+
 Filename: langtools/pornhub.py
 Comment: 
 
 Filename: langtools/visa.py
 Comment: 
 
 Filename: langtools/web_browser.py
 Comment: 
 
-Filename: langtools-0.2.0.dist-info/LICENSE
+Filename: langtools-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: langtools-0.2.0.dist-info/METADATA
+Filename: langtools-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: langtools-0.2.0.dist-info/WHEEL
+Filename: langtools-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: langtools-0.2.0.dist-info/RECORD
+Filename: langtools-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langtools/__init__.py

```diff
@@ -1,3 +1,4 @@
+from .mortgage import LoanCalculator
 from .pornhub import PornHubSearch
 from .visa import VISAFXRate
 from .web_browser import WebBrowser
```

## langtools/pornhub.py

 * *Ordering differences only*

```diff
@@ -52,8 +52,8 @@
             return 'No videos found.'
 
         videos = videos[:self.max_videos]
         docs = [to_string(video) for video in videos]
         return '\n\n'.join(docs)[:self.max_chars]
 
     async def _arun(self, url: str) -> str:
-        raise NotImplementedError("This tool does not support async")
+        raise NotImplementedError("This tool does not support async")
```

## langtools/visa.py

 * *Ordering differences only*

```diff
@@ -95,8 +95,8 @@
         return (f'Amount: {amount}\n'
                 f'From: {from_curr}\n'
                 f'To: {to_curr}\n'
                 f'Converted Amount: {r.convertedAmount}\n'
                 f'FX Rate: {r.fxRateWithAdditionalFee}\n')
 
     async def _arun(self, url: str) -> str:
-        raise NotImplementedError("This tool does not support async")
+        raise NotImplementedError("This tool does not support async")
```

## Comparing `langtools-0.2.0.dist-info/LICENSE` & `langtools-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langtools-0.2.0.dist-info/METADATA` & `langtools-0.3.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: langtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: なるみ
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cloudscraper (>=1.2.71,<2.0.0)
 Requires-Dist: langchain (>=0.0.209,<0.0.210)
+Requires-Dist: mortgage (>=1.0.5,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pornhub-api (>=0.3.0,<0.4.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Description-Content-Type: text/markdown
 
 # langtools
```

