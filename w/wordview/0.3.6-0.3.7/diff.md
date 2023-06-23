# Comparing `tmp/wordview-0.3.6.tar.gz` & `tmp/wordview-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.3.6.tar", max compression
+gzip compressed data, was "wordview-0.3.7.tar", max compression
```

## Comparing `wordview-0.3.6.tar` & `wordview-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1558 2023-06-23 09:38:44.102337 wordview-0.3.6/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-06-23 09:38:44.106337 wordview-0.3.6/LICENSE
--rw-r--r--   0        0        0     4638 2023-06-23 09:38:44.106337 wordview-0.3.6/README.rst
--rw-r--r--   0        0        0      873 2023-06-23 09:38:44.186338 wordview-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/am.py
--rw-r--r--   0        0        0     8698 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11805 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8399 2023-06-23 09:38:44.186338 wordview-0.3.6/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1662 2023-06-23 09:52:21.149500 wordview-0.3.7/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-06-23 09:52:21.149500 wordview-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4638 2023-06-23 09:52:21.149500 wordview-0.3.7/README.rst
+-rw-r--r--   0        0        0      873 2023-06-23 09:52:21.249501 wordview-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/am.py
+-rw-r--r--   0        0        0     8698 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-06-23 09:52:21.253501 wordview-0.3.7/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11805 2023-06-23 09:52:21.253501 wordview-0.3.7/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8399 2023-06-23 09:52:21.253501 wordview-0.3.7/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.7/PKG-INFO
```

### Comparing `wordview-0.3.6/CHANGES.rst` & `wordview-0.3.7/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Version 0.3.7
+-------------
+- Change newline encoding.
+- To support multiline in GitHub release body.
+
+
 Version 0.3.6
 -------------
 - Test description.
 - Test description2.
 - Test description3.
 - Test description4.
```

### Comparing `wordview-0.3.6/LICENSE` & `wordview-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/README.rst` & `wordview-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/pyproject.toml` & `wordview-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "0.3.6"
+version = "0.3.7"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
```

### Comparing `wordview-0.3.6/wordview/anomaly/gaussianize.py` & `wordview-0.3.7/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/anomaly/normaldist.py` & `wordview-0.3.7/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/clustering/cluster.py` & `wordview-0.3.7/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/mwes/am.py` & `wordview-0.3.7/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/mwes/mwe.py` & `wordview-0.3.7/wordview/mwes/mwe.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/mwes/mwe_utils.py` & `wordview-0.3.7/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/preprocessing/cleaning.py` & `wordview-0.3.7/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/text_analysis/core.py` & `wordview-0.3.7/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/wordview/text_analysis/wrapper.py` & `wordview-0.3.7/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.6/PKG-INFO` & `wordview-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.3.6
+Version: 0.3.7
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

