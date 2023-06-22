# Comparing `tmp/cfr-graphem-0.2.8.tar.gz` & `tmp/cfr-graphem-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-graphem-0.2.8.tar", last modified: Thu Mar 23 02:48:07 2023, max compression
+gzip compressed data, was "cfr-graphem-0.2.9.tar", last modified: Mon May 29 00:41:24 2023, max compression
```

## Comparing `cfr-graphem-0.2.8.tar` & `cfr-graphem-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-03-23 02:48:07.555648 cfr-graphem-0.2.8/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2023-02-11 11:26:13.000000 cfr-graphem-0.2.8/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-03-23 02:48:07.555528 cfr-graphem-0.2.8/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      215 2023-02-11 11:26:13.000000 cfr-graphem-0.2.8/README.rst
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-03-23 02:48:07.554415 cfr-graphem-0.2.8/cfr_graphem.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-03-23 02:48:07.000000 cfr-graphem-0.2.8/cfr_graphem.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      370 2023-03-23 02:48:07.000000 cfr-graphem-0.2.8/cfr_graphem.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-03-23 02:48:07.000000 cfr-graphem-0.2.8/cfr_graphem.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-02-11 12:40:30.000000 cfr-graphem-0.2.8/cfr_graphem.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-03-23 02:48:07.000000 cfr-graphem-0.2.8/cfr_graphem.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       16 2023-03-23 02:48:07.000000 cfr-graphem-0.2.8/cfr_graphem.egg-info/top_level.txt
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-03-23 02:48:07.555288 cfr-graphem-0.2.8/graphem/
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     9935 2023-03-23 01:06:59.000000 cfr-graphem-0.2.8/graphem/GraphEstimation.py
--rwxr-xr-x   0 fengzhu    (502) staff       (20)    15228 2023-02-11 11:26:13.000000 cfr-graphem-0.2.8/graphem/QUIC.cpp
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     1709 2023-02-11 11:26:13.000000 cfr-graphem-0.2.8/graphem/QUIC.py
--rw-r--r--   0 fengzhu    (502) staff       (20)       52 2023-02-11 11:26:13.000000 cfr-graphem-0.2.8/graphem/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    13086 2023-02-11 11:26:13.000000 cfr-graphem-0.2.8/graphem/graph.py
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     5846 2023-02-11 11:26:13.000000 cfr-graphem-0.2.8/graphem/iridge.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    28851 2023-03-23 01:27:20.000000 cfr-graphem-0.2.8/graphem/solver.py
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-03-23 02:48:07.555705 cfr-graphem-0.2.8/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1452 2023-03-23 02:47:40.000000 cfr-graphem-0.2.8/setup.py
+drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2023-05-29 00:41:24.201918 cfr-graphem-0.2.9/
+-rw-r--r--   0 fzhu       (501) staff       (20)     1516 2023-02-11 11:26:13.000000 cfr-graphem-0.2.9/LICENSE
+-rw-r--r--   0 fzhu       (501) staff       (20)      725 2023-05-29 00:41:24.201780 cfr-graphem-0.2.9/PKG-INFO
+-rw-r--r--   0 fzhu       (501) staff       (20)      215 2023-02-11 11:26:13.000000 cfr-graphem-0.2.9/README.rst
+drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2023-05-29 00:41:24.199849 cfr-graphem-0.2.9/cfr_graphem.egg-info/
+-rw-r--r--   0 fzhu       (501) staff       (20)      725 2023-05-29 00:41:23.000000 cfr-graphem-0.2.9/cfr_graphem.egg-info/PKG-INFO
+-rw-r--r--   0 fzhu       (501) staff       (20)      370 2023-05-29 00:41:24.000000 cfr-graphem-0.2.9/cfr_graphem.egg-info/SOURCES.txt
+-rw-r--r--   0 fzhu       (501) staff       (20)        1 2023-05-29 00:41:23.000000 cfr-graphem-0.2.9/cfr_graphem.egg-info/dependency_links.txt
+-rw-r--r--   0 fzhu       (501) staff       (20)        1 2023-02-11 12:40:30.000000 cfr-graphem-0.2.9/cfr_graphem.egg-info/not-zip-safe
+-rw-r--r--   0 fzhu       (501) staff       (20)        4 2023-05-29 00:41:24.000000 cfr-graphem-0.2.9/cfr_graphem.egg-info/requires.txt
+-rw-r--r--   0 fzhu       (501) staff       (20)       16 2023-05-29 00:41:24.000000 cfr-graphem-0.2.9/cfr_graphem.egg-info/top_level.txt
+drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2023-05-29 00:41:24.201254 cfr-graphem-0.2.9/graphem/
+-rwxr-xr-x   0 fzhu       (501) staff       (20)     9932 2023-05-29 00:40:16.000000 cfr-graphem-0.2.9/graphem/GraphEstimation.py
+-rwxr-xr-x   0 fzhu       (501) staff       (20)    15228 2023-02-11 11:26:13.000000 cfr-graphem-0.2.9/graphem/QUIC.cpp
+-rwxr-xr-x   0 fzhu       (501) staff       (20)     1709 2023-02-11 11:26:13.000000 cfr-graphem-0.2.9/graphem/QUIC.py
+-rw-r--r--   0 fzhu       (501) staff       (20)       52 2023-02-11 11:26:13.000000 cfr-graphem-0.2.9/graphem/__init__.py
+-rw-r--r--   0 fzhu       (501) staff       (20)    13086 2023-02-11 11:26:13.000000 cfr-graphem-0.2.9/graphem/graph.py
+-rwxr-xr-x   0 fzhu       (501) staff       (20)     5846 2023-02-11 11:26:13.000000 cfr-graphem-0.2.9/graphem/iridge.py
+-rw-r--r--   0 fzhu       (501) staff       (20)    28851 2023-03-23 22:06:36.000000 cfr-graphem-0.2.9/graphem/solver.py
+-rw-r--r--   0 fzhu       (501) staff       (20)       38 2023-05-29 00:41:24.201964 cfr-graphem-0.2.9/setup.cfg
+-rw-r--r--   0 fzhu       (501) staff       (20)     1452 2023-05-29 00:41:06.000000 cfr-graphem-0.2.9/setup.py
```

### Comparing `cfr-graphem-0.2.8/LICENSE` & `cfr-graphem-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.2.8/PKG-INFO` & `cfr-graphem-0.2.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: cfr-graphem
-Version: 0.2.8
+Version: 0.2.9
 Summary: The GraphEM component for CFR
 Home-page: https://github.com/fzhu2e/cfr-graphem
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
+Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ***********************************************************
 cfr-graphem: the GraphEM component for CFR
 ***********************************************************
 
 For more details, see: https://fzhu2e.github.io/cfr
+
```

### Comparing `cfr-graphem-0.2.8/cfr_graphem.egg-info/PKG-INFO` & `cfr-graphem-0.2.9/cfr_graphem.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: cfr-graphem
-Version: 0.2.8
+Version: 0.2.9
 Summary: The GraphEM component for CFR
 Home-page: https://github.com/fzhu2e/cfr-graphem
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
+Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ***********************************************************
 cfr-graphem: the GraphEM component for CFR
 ***********************************************************
 
 For more details, see: https://fzhu2e.github.io/cfr
+
```

### Comparing `cfr-graphem-0.2.8/graphem/GraphEstimation.py` & `cfr-graphem-0.2.9/graphem/GraphEstimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         Adjacency matrix of the neighborhood graph
     sparsity: float
         Sparsity level of the adjacency matrix
     '''
     print("Estimating graph using neighborhood method")
 
     D = dMat(lonlat)
-    adj = (D <= cutoff_radius).astype(np.int)           # replace 0s or 1s
+    adj = (D <= cutoff_radius).astype(int)           # replace 0s or 1s
     adj[np.ix_(ind_P, ind_P)] = np.eye(len(ind_P)) # set pp to 1s
     sparsity = graph_sparsity(adj, ind_F, ind_P)
 
     return [adj, sparsity]
 
 
 def great_circle_distance(lon1, lat1, lon2, lat2):
```

### Comparing `cfr-graphem-0.2.8/graphem/QUIC.cpp` & `cfr-graphem-0.2.9/graphem/QUIC.cpp`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.2.8/graphem/QUIC.py` & `cfr-graphem-0.2.9/graphem/QUIC.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.2.8/graphem/graph.py` & `cfr-graphem-0.2.9/graphem/graph.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.2.8/graphem/iridge.py` & `cfr-graphem-0.2.9/graphem/iridge.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.2.8/graphem/solver.py` & `cfr-graphem-0.2.9/graphem/solver.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.2.8/setup.py` & `cfr-graphem-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         filename = super().get_ext_filename(ext_name)
         suffix = sysconfig.get_config_var('EXT_SUFFIX')
         ext = os.path.splitext(filename)[1]
         return os.path.join('./graphem', filename.replace(suffix, "")+ext)
 
 setup(
     name='cfr-graphem',
-    version='0.2.8',
+    version='0.2.9',
     description='The GraphEM component for CFR',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr-graphem',
     packages=find_packages(),
```

