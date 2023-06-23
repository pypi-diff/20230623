# Comparing `tmp/catencfamily-0.0.80.tar.gz` & `tmp/catencfamily-0.0.81.tar.gz`

## Comparing `catencfamily-0.0.80.tar` & `catencfamily-0.0.81.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.80/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89201 2020-02-02 00:00:00.000000 catencfamily-0.0.80/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    42984 2020-02-02 00:00:00.000000 catencfamily-0.0.80/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.80/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.80/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.80/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.80/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.81/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89201 2020-02-02 00:00:00.000000 catencfamily-0.0.81/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    43737 2020-02-02 00:00:00.000000 catencfamily-0.0.81/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.81/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.81/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.81/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.81/PKG-INFO
```

### Comparing `catencfamily-0.0.80/src/catencfamily/encoders.py` & `catencfamily-0.0.81/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.80/src/catencfamily/utils.py` & `catencfamily-0.0.81/src/catencfamily/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# 19th June, 2023
+# 23th June, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
-import random
 from scipy.stats import kurtosis
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.datasets import make_classification
 from sklearn.feature_selection import  mutual_info_classif
 import networkx as nx
 import itertools
 import pickle
 import pathlib
 import string
 import matplotlib.pyplot as plt
 import seaborn as sns
 from pathlib import Path
-import time
+
 
 
 
 def xgImptFeatures(model, df_columns, filename = None, master=None):
     """
     Given an xgboost classifier model & data col
     names, the function returns two lists of cols,
@@ -521,32 +520,54 @@
 
 
 
 # Ref: https://stackoverflow.com/a/4529901/3282777
 def savePythonObject(pythonObject, filename, filePath = None ):
     
     """
+    Desc
+    ----
     Saves any python object to disk
-    File is saved to filePath. Restore it
+    File is saved to filePath. If
+    filePath does not exist, it is
+    created.
+    Restore the pythonObject
     using restorePythonObject()
+    
     Parameters
     ----------
-    filename : pickle file for dumping
+    pythonObject: Obj to be saved
+    filename : str Name of pickle file
+    filePath: str, NAme of folder
+    
     Returns
     -------
     None.
     """
+    
     # Current dir is the default filePath
     if filePath is None:
         filePath = pathlib.Path.cwd()
         path = filePath / filename
     else:
         path = pathlib.Path(filePath) / filename
+        
+    # Check if specified folder exixts:
+    # IF not create one:
+    p = pathlib.Path(filePath)
+    if not pathlib.Path.exists(p):
+        print(f"Folder '{filePath}' does not exist")
+        print("Being created..")
+        p.mkdir(parents=True, exist_ok=True)    
+    
+    # Now dump the python object    
     with open(path, 'wb') as outp:
         pickle.dump(pythonObject, outp, pickle.HIGHEST_PROTOCOL)
+        
+    # Finally print your message    
     print("Object saved to:", str(path))    
 
      
      
 
  # It restores an earlier saved python object
 def restorePythonObject(filename, filePath = None):
@@ -986,21 +1007,27 @@
     Returns
     -------
     None.
 
     """
     filepath = pathToFolder / filename
     G = nx.read_gml(filepath) 
+    if (len(G.edges())) == 0: 
+        print("This network has no edges. Moving ahead.")
+        return 
+
     
     # If network is very large, take a sanple
     # Ref: https://stackoverflow.com/a/62407941/3282777
     if takeGraphSample:
         sampled_nodes = np.random.choice(G.nodes, noSampleNodes)
         G = G.subgraph(sampled_nodes)
-    
+        if (len(G.edges())) == 0: 
+            print("This network has no edges. Moving ahead.")
+            return 
     
     colors = colorList
     pos = nx.spring_layout(G, k)
     
     if algo == nx.community.girvan_newman:
         lst_b = algo(G)
         lst_b = tuple(sorted(c) for c in next(lst_b))
```

### Comparing `catencfamily-0.0.80/LICENSE` & `catencfamily-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.80/README.md` & `catencfamily-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.80/pyproject.toml` & `catencfamily-0.0.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.80"
+version = "0.0.81"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.80/PKG-INFO` & `catencfamily-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.80
+Version: 0.0.81
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

