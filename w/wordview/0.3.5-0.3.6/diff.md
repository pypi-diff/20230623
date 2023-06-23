# Comparing `tmp/wordview-0.3.5.tar.gz` & `tmp/wordview-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.3.5.tar", max compression
+gzip compressed data, was "wordview-0.3.6.tar", max compression
```

## Comparing `wordview-0.3.5.tar` & `wordview-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1535 2023-06-23 09:25:42.584149 wordview-0.3.5/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-06-23 09:25:42.584149 wordview-0.3.5/LICENSE
--rw-r--r--   0        0        0     4638 2023-06-23 09:25:42.584149 wordview-0.3.5/README.rst
--rw-r--r--   0        0        0      873 2023-06-23 09:25:42.680149 wordview-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/mwes/am.py
--rw-r--r--   0        0        0     8698 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11805 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8399 2023-06-23 09:25:42.680149 wordview-0.3.5/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1558 2023-06-23 09:38:44.102337 wordview-0.3.6/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-06-23 09:38:44.106337 wordview-0.3.6/LICENSE
+-rw-r--r--   0        0        0     4638 2023-06-23 09:38:44.106337 wordview-0.3.6/README.rst
+-rw-r--r--   0        0        0      873 2023-06-23 09:38:44.186338 wordview-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/am.py
+-rw-r--r--   0        0        0     8698 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11805 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8399 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.6/PKG-INFO
```

### Comparing `wordview-0.3.5/CHANGES.rst` & `wordview-0.3.6/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+Version 0.3.6
+-------------
+- Test description.
+- Test description2.
+- Test description3.
+- Test description4.
+
 Version 0.3.5
 -------------
-- Sersion to support multiline description l1.
-- Support multiline description l2.
-- Sersion to support multiline description l3.
+- Test description.
+- Test description2.
 
 Version 0.3.4
 -------------
 - Update awk sed parser to correctly read release body. 
 
 Version 0.3.3
 -------------
```

### Comparing `wordview-0.3.5/LICENSE` & `wordview-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/README.rst` & `wordview-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/pyproject.toml` & `wordview-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "0.3.5"
+version = "0.3.6"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
```

### Comparing `wordview-0.3.5/wordview/anomaly/gaussianize.py` & `wordview-0.3.6/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/anomaly/normaldist.py` & `wordview-0.3.6/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/clustering/cluster.py` & `wordview-0.3.6/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/mwes/am.py` & `wordview-0.3.6/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/mwes/mwe.py` & `wordview-0.3.6/wordview/mwes/mwe.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/mwes/mwe_utils.py` & `wordview-0.3.6/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/preprocessing/cleaning.py` & `wordview-0.3.6/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/text_analysis/core.py` & `wordview-0.3.6/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/wordview/text_analysis/wrapper.py` & `wordview-0.3.6/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.5/PKG-INFO` & `wordview-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.3.5
+Version: 0.3.6
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

