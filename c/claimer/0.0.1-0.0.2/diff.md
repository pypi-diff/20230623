# Comparing `tmp/claimer-0.0.1.tar.gz` & `tmp/claimer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claimer-0.0.1.tar", last modified: Fri Jun 23 12:58:41 2023, max compression
+gzip compressed data, was "claimer-0.0.2.tar", last modified: Fri Jun 23 14:57:52 2023, max compression
```

## Comparing `claimer-0.0.1.tar` & `claimer-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 12:58:41.977094 claimer-0.0.1/
--rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-23 12:01:13.000000 claimer-0.0.1/LICENSE
--rw-r--r--   0 cbadenes   (501) staff       (20)     4325 2023-06-23 12:58:41.976984 claimer-0.0.1/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)     3621 2023-06-23 12:55:07.000000 claimer-0.0.1/README.md
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 12:58:41.976111 claimer-0.0.1/claimer/
--rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-23 10:12:52.000000 claimer-0.0.1/claimer/__init__.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1797 2023-06-23 12:44:59.000000 claimer-0.0.1/claimer/paragraph.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     2463 2023-06-23 12:42:52.000000 claimer-0.0.1/claimer/parser.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 12:58:41.976806 claimer-0.0.1/claimer.egg-info/
--rw-r--r--   0 cbadenes   (501) staff       (20)     4325 2023-06-23 12:58:41.000000 claimer-0.0.1/claimer.egg-info/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      245 2023-06-23 12:58:41.000000 claimer-0.0.1/claimer.egg-info/SOURCES.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-23 12:58:41.000000 claimer-0.0.1/claimer.egg-info/dependency_links.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       36 2023-06-23 12:58:41.000000 claimer-0.0.1/claimer.egg-info/requires.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        8 2023-06-23 12:58:41.000000 claimer-0.0.1/claimer.egg-info/top_level.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)      902 2023-06-23 10:56:31.000000 claimer-0.0.1/pyproject.toml
--rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-23 12:58:41.977133 claimer-0.0.1/setup.cfg
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 14:57:52.850060 claimer-0.0.2/
+-rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-23 12:01:13.000000 claimer-0.0.2/LICENSE
+-rw-r--r--   0 cbadenes   (501) staff       (20)     4319 2023-06-23 14:57:52.849942 claimer-0.0.2/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3615 2023-06-23 13:21:30.000000 claimer-0.0.2/README.md
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 14:57:52.849255 claimer-0.0.2/claimer/
+-rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-23 10:12:52.000000 claimer-0.0.2/claimer/__init__.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2630 2023-06-23 14:51:40.000000 claimer-0.0.2/claimer/paragraph.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2495 2023-06-23 14:39:16.000000 claimer-0.0.2/claimer/parser.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 14:57:52.849780 claimer-0.0.2/claimer.egg-info/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     4319 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      245 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/SOURCES.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/dependency_links.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       36 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/requires.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        8 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/top_level.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)      902 2023-06-23 14:56:54.000000 claimer-0.0.2/pyproject.toml
+-rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-23 14:57:52.850097 claimer-0.0.2/setup.cfg
```

### Comparing `claimer-0.0.1/LICENSE` & `claimer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `claimer-0.0.1/PKG-INFO` & `claimer-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claimer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Breaks down a textual paragraph into verifiable claims.
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/claimer
 Project-URL: Bug Tracker, https://github.com/librairy/claimer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -66,8 +66,8 @@
 # 6) Make sure you wear face coverings in all public indoor spaces and whenever you can't keep a 2m distance from others.
 # 7) Use a face covering is simple and easy way we can all stop the spread of COVID-19
 
 ```
 
 ## Note
 
-The Entity Linker at the current state is still experimental and should not be used in production mode.
+The Claimer at the current state is still experimental and should not be used in production mode.
```

### Comparing `claimer-0.0.1/README.md` & `claimer-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 # 6) Make sure you wear face coverings in all public indoor spaces and whenever you can't keep a 2m distance from others.
 # 7) Use a face covering is simple and easy way we can all stop the spread of COVID-19
 
 ```
 
 ## Note
 
-The Entity Linker at the current state is still experimental and should not be used in production mode.
+The Claimer at the current state is still experimental and should not be used in production mode.
```

### Comparing `claimer-0.0.1/claimer/paragraph.py` & `claimer-0.0.2/claimer/paragraph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 from claimer import parser
 
 def get_claims(text):
     
-    (clusters, cluster_names) = parser.get_corefs(text)
-    #print(cluster_names)
     tokens = parser.get_tokens(text)
+    print("Num Tokens:",len(tokens))
+
+    clusters = []
+    cluster_names = []
+    partial_content = []
+    current_sentence = None
+    for i in tokens:
+        t = tokens[i]
+        if (len(partial_content)>250):
+            if (current_sentence != t['sentence']):
+                partial_text = "".join(partial_content)
+                (partial_clusters, partial_cluster_names) = parser.get_corefs(partial_text)
+                clusters.extend(partial_clusters)
+                cluster_names.extend(partial_cluster_names)
+                current_sentence = t['sentence']
+                partial_content = [t['text_with_ws']]
+            else:
+                partial_content.append(t['text_with_ws'])                
+        else:
+            partial_content.append(t['text_with_ws'])
+            current_sentence = t['sentence']
+
+    #(clusters, cluster_names) = parser.get_corefs(text)
+    print(cluster_names)
 
     cluster_labels = {}
     for idx, cluster in enumerate(clusters):
         position = 0
         candidates = []
         for (i,j) in cluster:
             level = 99999
```

### Comparing `claimer-0.0.1/claimer/parser.py` & `claimer-0.0.2/claimer/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     tokens = {}
     for id, t in enumerate(doc):
         token = {
             'text' : t.text,
             'text_with_ws' : t.text_with_ws,
             'pos'  : t.pos_,
             'tag'  : t.tag_,
+            'sentence': t.sent,
             'level' : 99999
         }
         if (id in entities):
             entity = entities[id]
             token['level'] = entity['level']        
             token['label'] = entity['label']
         tokens[t.idx] = token
```

### Comparing `claimer-0.0.1/claimer.egg-info/PKG-INFO` & `claimer-0.0.2/claimer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claimer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Breaks down a textual paragraph into verifiable claims.
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/claimer
 Project-URL: Bug Tracker, https://github.com/librairy/claimer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -66,8 +66,8 @@
 # 6) Make sure you wear face coverings in all public indoor spaces and whenever you can't keep a 2m distance from others.
 # 7) Use a face covering is simple and easy way we can all stop the spread of COVID-19
 
 ```
 
 ## Note
 
-The Entity Linker at the current state is still experimental and should not be used in production mode.
+The Claimer at the current state is still experimental and should not be used in production mode.
```

### Comparing `claimer-0.0.1/pyproject.toml` & `claimer-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "spacy",
     "spacy-entity-linker"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "claimer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Carlos Badenes-Olmedo", email="carlos.badenes@upm.es" },
 ]
 description = "Breaks down a textual paragraph into verifiable claims."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

