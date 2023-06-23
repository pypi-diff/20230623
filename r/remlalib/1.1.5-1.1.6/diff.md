# Comparing `tmp/remlalib-1.1.5.tar.gz` & `tmp/remlalib-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remlalib-1.1.5.tar", last modified: Thu Jun 15 22:06:09 2023, max compression
+gzip compressed data, was "remlalib-1.1.6.tar", last modified: Fri Jun 23 13:56:06 2023, max compression
```

## Comparing `remlalib-1.1.5.tar` & `remlalib-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:06:09.133761 remlalib-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-15 22:05:59.000000 remlalib-1.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 22:06:09.133761 remlalib-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 22:05:59.000000 remlalib-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:06:09.133761 remlalib-1.1.5/remlalib/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 22:05:59.000000 remlalib-1.1.5/remlalib/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:06:09.133761 remlalib-1.1.5/remlalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 22:06:09.000000 remlalib-1.1.5/remlalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 22:06:09.133761 remlalib-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-15 22:05:59.000000 remlalib-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:06.769058 remlalib-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-23 13:55:55.000000 remlalib-1.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 13:56:06.769058 remlalib-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 13:55:55.000000 remlalib-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:06.769058 remlalib-1.1.6/remlalib/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-23 13:55:55.000000 remlalib-1.1.6/remlalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 13:55:55.000000 remlalib-1.1.6/remlalib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-23 13:55:55.000000 remlalib-1.1.6/remlalib/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 13:55:55.000000 remlalib-1.1.6/remlalib/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:06.769058 remlalib-1.1.6/remlalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-23 13:56:06.000000 remlalib-1.1.6/remlalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 13:56:06.000000 remlalib-1.1.6/remlalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:56:06.000000 remlalib-1.1.6/remlalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 13:56:06.000000 remlalib-1.1.6/remlalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 13:56:06.000000 remlalib-1.1.6/remlalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 13:56:06.769058 remlalib-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-23 13:55:55.000000 remlalib-1.1.6/setup.py
```

### Comparing `remlalib-1.1.5/LICENSE.txt` & `remlalib-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remlalib-1.1.5/PKG-INFO` & `remlalib-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.1.5
+Version: 1.1.6
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.1.5/remlalib/preprocess.py` & `remlalib-1.1.6/remlalib/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 class Preprocess:
 
     # load a default preprocessor
     def __init__(self):
         self.count_vectorizer = None
 
-    def load_from_url(self, url):
+    def load_from_url(self, url) -> None:
         """Load a preprocessor from a url"""
         with urlopen(url) as file:
             self.count_vectorizer = load(file)
 
-    def load_dataset(data_path):
+    def load_dataset(data_path) -> pd.DataFrame:
         """Load dataset from data_path"""
         return pd.read_csv(data_path, delimiter='\t', quoting=3)
 
-    def _get_stopwords():
+    def _get_stopwords() -> list:
         """Obtain the list of stopwords"""
         nltk.download('stopwords')
 
         all_stopwords = stopwords.words('english')
         all_stopwords.remove('not')
 
         return all_stopwords
 
 
-    def _get_corpus(self, dataset):
+    def _get_corpus(self, dataset) -> list:
         """produce the corpus from the dataset by applying preprocessing steps"""
         all_stopwords = self.get_stopwords()
         corpus = []
 
         porter_stemmer = PorterStemmer()
 
         for i in range(0, 900):
@@ -47,19 +47,19 @@
             review = [porter_stemmer.stem(word)
                     for word in review if not word in set(all_stopwords)]
             review = ' '.join(review)
             corpus.append(review)
         return corpus
 
 
-    def preprocess_dataset(self, dataset):
+    def preprocess_dataset(self, dataset) -> tuple:
         """Preprocess the dataset and save it"""
-        corpus = self.get_corpus(dataset)
+        corpus = self._get_corpus(dataset)
         self.count_vectorizer = CountVectorizer(max_features=1420)
         X = self.count_vectorizer.fit_transform(corpus).toarray()
         y = dataset.iloc[:, -1].values
 
         return X, y
 
-    def preprocess_sample(self, review):
+    def preprocess_sample(self, review) -> list:
         """Preprocess the sample review and return it"""
         return self.count_vectorizer.transform([review]).toarray()[0]
```

### Comparing `remlalib-1.1.5/remlalib.egg-info/PKG-INFO` & `remlalib-1.1.6/remlalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remlalib
-Version: 1.1.5
+Version: 1.1.6
 Summary: REMLA23 - Team 13 - Lib
 Home-page: https://github.com/remla23-team13/lib
 Download-URL: https://github.com/remla23-team13/lib
 Author: Team 13
 Author-email: gasparsantosrocha@gmail.com
 License: MIT
 Keywords: REMLA,Versioning
```

### Comparing `remlalib-1.1.5/setup.py` & `remlalib-1.1.6/setup.py`

 * *Files identical despite different names*

