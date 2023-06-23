# Comparing `tmp/claimer-0.0.2.tar.gz` & `tmp/claimer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claimer-0.0.2.tar", last modified: Fri Jun 23 14:57:52 2023, max compression
+gzip compressed data, was "claimer-0.0.3.tar", last modified: Fri Jun 23 15:00:41 2023, max compression
```

## Comparing `claimer-0.0.2.tar` & `claimer-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 14:57:52.850060 claimer-0.0.2/
--rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-23 12:01:13.000000 claimer-0.0.2/LICENSE
--rw-r--r--   0 cbadenes   (501) staff       (20)     4319 2023-06-23 14:57:52.849942 claimer-0.0.2/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)     3615 2023-06-23 13:21:30.000000 claimer-0.0.2/README.md
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 14:57:52.849255 claimer-0.0.2/claimer/
--rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-23 10:12:52.000000 claimer-0.0.2/claimer/__init__.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     2630 2023-06-23 14:51:40.000000 claimer-0.0.2/claimer/paragraph.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     2495 2023-06-23 14:39:16.000000 claimer-0.0.2/claimer/parser.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 14:57:52.849780 claimer-0.0.2/claimer.egg-info/
--rw-r--r--   0 cbadenes   (501) staff       (20)     4319 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      245 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/SOURCES.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/dependency_links.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       36 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/requires.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        8 2023-06-23 14:57:52.000000 claimer-0.0.2/claimer.egg-info/top_level.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)      902 2023-06-23 14:56:54.000000 claimer-0.0.2/pyproject.toml
--rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-23 14:57:52.850097 claimer-0.0.2/setup.cfg
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 15:00:41.472278 claimer-0.0.3/
+-rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-23 12:01:13.000000 claimer-0.0.3/LICENSE
+-rw-r--r--   0 cbadenes   (501) staff       (20)     4319 2023-06-23 15:00:41.472059 claimer-0.0.3/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3615 2023-06-23 13:21:30.000000 claimer-0.0.3/README.md
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 15:00:41.471008 claimer-0.0.3/claimer/
+-rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-23 10:12:52.000000 claimer-0.0.3/claimer/__init__.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2630 2023-06-23 14:51:40.000000 claimer-0.0.3/claimer/paragraph.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2496 2023-06-23 14:59:26.000000 claimer-0.0.3/claimer/parser.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-23 15:00:41.471824 claimer-0.0.3/claimer.egg-info/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     4319 2023-06-23 15:00:41.000000 claimer-0.0.3/claimer.egg-info/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      245 2023-06-23 15:00:41.000000 claimer-0.0.3/claimer.egg-info/SOURCES.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-23 15:00:41.000000 claimer-0.0.3/claimer.egg-info/dependency_links.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       36 2023-06-23 15:00:41.000000 claimer-0.0.3/claimer.egg-info/requires.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        8 2023-06-23 15:00:41.000000 claimer-0.0.3/claimer.egg-info/top_level.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)      902 2023-06-23 14:59:44.000000 claimer-0.0.3/pyproject.toml
+-rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-23 15:00:41.472333 claimer-0.0.3/setup.cfg
```

### Comparing `claimer-0.0.2/LICENSE` & `claimer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `claimer-0.0.2/PKG-INFO` & `claimer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claimer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Breaks down a textual paragraph into verifiable claims.
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/claimer
 Project-URL: Bug Tracker, https://github.com/librairy/claimer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `claimer-0.0.2/README.md` & `claimer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `claimer-0.0.2/claimer/paragraph.py` & `claimer-0.0.3/claimer/paragraph.py`

 * *Files identical despite different names*

### Comparing `claimer-0.0.2/claimer/parser.py` & `claimer-0.0.3/claimer/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             if (i in cluster_spans) and (cluster_spans[i] == (i,j)):
                 cluster_tokens.append((i,j))
         if (len(cluster_tokens)>0):
             clusters.append(cluster_tokens)
     #print("Cluster Spans:", clusters)
 
     labels = preds[0].get_clusters()
-    print("Cluster Tokens:",labels)
+    #print("Cluster Tokens:",labels)
 
     return (clusters,labels)
 
 def get_tokens(text):
     doc = nlp(text)
 
     entities = {}
```

### Comparing `claimer-0.0.2/claimer.egg-info/PKG-INFO` & `claimer-0.0.3/claimer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claimer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Breaks down a textual paragraph into verifiable claims.
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/claimer
 Project-URL: Bug Tracker, https://github.com/librairy/claimer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `claimer-0.0.2/pyproject.toml` & `claimer-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "spacy",
     "spacy-entity-linker"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "claimer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Carlos Badenes-Olmedo", email="carlos.badenes@upm.es" },
 ]
 description = "Breaks down a textual paragraph into verifiable claims."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

