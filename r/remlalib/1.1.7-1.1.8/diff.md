# Comparing `tmp/remlalib-1.1.7.tar.gz` & `tmp/remlalib-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remlalib-1.1.7.tar", last modified: Fri Jun 23 13:59:38 2023, max compression
+gzip compressed data, was "remlalib-1.1.8.tar", last modified: Fri Jun 23 15:51:36 2023, max compression
```

## Comparing `remlalib-1.1.7.tar` & `remlalib-1.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:59:38.563759 remlalib-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-23 13:59:28.000000 remlalib-1.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 13:59:38.563759 remlalib-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 13:59:28.000000 remlalib-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:59:38.563759 remlalib-1.1.7/remlalib/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-23 13:59:28.000000 remlalib-1.1.7/remlalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 13:59:29.000000 remlalib-1.1.7/remlalib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-23 13:59:28.000000 remlalib-1.1.7/remlalib/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 13:59:28.000000 remlalib-1.1.7/remlalib/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:59:38.563759 remlalib-1.1.7/remlalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 13:59:38.000000 remlalib-1.1.7/remlalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 13:59:38.000000 remlalib-1.1.7/remlalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:59:38.000000 remlalib-1.1.7/remlalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 13:59:38.000000 remlalib-1.1.7/remlalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 13:59:38.000000 remlalib-1.1.7/remlalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 13:59:38.563759 remlalib-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-23 13:59:28.000000 remlalib-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:36.115727 remlalib-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-23 15:51:27.000000 remlalib-1.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 15:51:36.115727 remlalib-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 15:51:27.000000 remlalib-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:36.115727 remlalib-1.1.8/remlalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-23 15:51:27.000000 remlalib-1.1.8/remlalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 15:51:27.000000 remlalib-1.1.8/remlalib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-23 15:51:27.000000 remlalib-1.1.8/remlalib/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 15:51:27.000000 remlalib-1.1.8/remlalib/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:51:36.115727 remlalib-1.1.8/remlalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 15:51:36.000000 remlalib-1.1.8/remlalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 15:51:36.000000 remlalib-1.1.8/remlalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:51:36.000000 remlalib-1.1.8/remlalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 15:51:36.000000 remlalib-1.1.8/remlalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 15:51:36.000000 remlalib-1.1.8/remlalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 15:51:36.115727 remlalib-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-23 15:51:27.000000 remlalib-1.1.8/setup.py
```

### Comparing `remlalib-1.1.7/LICENSE.txt` & `remlalib-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remlalib-1.1.7/PKG-INFO` & `remlalib-1.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.1.7
+Version: 1.1.8
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.1.7/remlalib/preprocess.py` & `remlalib-1.1.8/remlalib/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
         self.count_vectorizer = None
 
     def load_from_url(self, url) -> None:
         """Load a preprocessor from a url"""
         with urlopen(url) as file:
             self.count_vectorizer = load(file)
 
-    def load_dataset(data_path) -> pd.DataFrame:
+    def load_dataset(self, data_path) -> pd.DataFrame:
         """Load dataset from data_path"""
         return pd.read_csv(data_path, delimiter='\t', quoting=3)
 
-    def _get_stopwords() -> list:
+    def _get_stopwords(self) -> list:
         """Obtain the list of stopwords"""
         nltk.download('stopwords')
 
         all_stopwords = stopwords.words('english')
         all_stopwords.remove('not')
 
         return all_stopwords
```

### Comparing `remlalib-1.1.7/remlalib.egg-info/PKG-INFO` & `remlalib-1.1.8/remlalib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.1.7
+Version: 1.1.8
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.1.7/setup.py` & `remlalib-1.1.8/setup.py`

 * *Files identical despite different names*

