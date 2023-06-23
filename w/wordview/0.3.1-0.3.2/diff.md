# Comparing `tmp/wordview-0.3.1.tar.gz` & `tmp/wordview-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.3.1.tar", max compression
+gzip compressed data, was "wordview-0.3.2.tar", max compression
```

## Comparing `wordview-0.3.1.tar` & `wordview-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1109 2023-06-22 17:48:02.895774 wordview-0.3.1/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-06-22 17:48:02.895774 wordview-0.3.1/LICENSE
--rw-r--r--   0        0        0     4638 2023-06-22 17:48:02.895774 wordview-0.3.1/README.rst
--rw-r--r--   0        0        0      873 2023-06-22 17:48:02.975774 wordview-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/am.py
--rw-r--r--   0        0        0     8698 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11805 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8399 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1193 2023-06-23 08:20:14.864651 wordview-0.3.2/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-06-23 08:20:14.864651 wordview-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4638 2023-06-23 08:20:14.864651 wordview-0.3.2/README.rst
+-rw-r--r--   0        0        0      873 2023-06-23 08:20:14.944655 wordview-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/mwes/am.py
+-rw-r--r--   0        0        0     8698 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11805 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8399 2023-06-23 08:20:14.944655 wordview-0.3.2/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.2/PKG-INFO
```

### Comparing `wordview-0.3.1/CHANGES.rst` & `wordview-0.3.2/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Version 0.3.2
+-------------
+- Fix missing multiline description in GitHub release.
+
 Version 0.3.1
 -------------
 - Add action for CD.
 - Publish to PyPi and GitHub Releases on bump version.
 - Improve the CD workflow to ensure checks are passed and the merge is successful.
 - Check for release notes, otherwise do not publish.
```

### Comparing `wordview-0.3.1/LICENSE` & `wordview-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/README.rst` & `wordview-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/pyproject.toml` & `wordview-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "0.3.1"
+version = "0.3.2"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
```

### Comparing `wordview-0.3.1/wordview/anomaly/gaussianize.py` & `wordview-0.3.2/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/anomaly/normaldist.py` & `wordview-0.3.2/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/clustering/cluster.py` & `wordview-0.3.2/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/mwes/am.py` & `wordview-0.3.2/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/mwes/mwe.py` & `wordview-0.3.2/wordview/mwes/mwe.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/mwes/mwe_utils.py` & `wordview-0.3.2/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/preprocessing/cleaning.py` & `wordview-0.3.2/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/text_analysis/core.py` & `wordview-0.3.2/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/wordview/text_analysis/wrapper.py` & `wordview-0.3.2/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.1/PKG-INFO` & `wordview-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.3.1
+Version: 0.3.2
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

