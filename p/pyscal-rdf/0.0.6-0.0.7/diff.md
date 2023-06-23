# Comparing `tmp/pyscal_rdf-0.0.6.tar.gz` & `tmp/pyscal_rdf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal_rdf-0.0.6.tar", last modified: Thu Jun 22 12:29:22 2023, max compression
+gzip compressed data, was "pyscal_rdf-0.0.7.tar", last modified: Fri Jun 23 10:59:43 2023, max compression
```

## Comparing `pyscal_rdf-0.0.6.tar` & `pyscal_rdf-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.542357 pyscal_rdf-0.0.6/pyscal_rdf/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/json_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/pyscal_rdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.542357 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/pyscal_rdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-22 12:29:22.000000 pyscal_rdf-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:29:22.546357 pyscal_rdf-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-22 12:29:15.000000 pyscal_rdf-0.0.6/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.856590 pyscal_rdf-0.0.7/pyscal_rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33695 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/pyscal_rdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.856590 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/pyscal_rdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-23 10:59:43.000000 pyscal_rdf-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:59:43.860590 pyscal_rdf-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-23 10:59:40.000000 pyscal_rdf-0.0.7/tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.0.6/LICENSE` & `pyscal_rdf-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/PKG-INFO` & `pyscal_rdf-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.0.6/README.md` & `pyscal_rdf-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf/graph.py` & `pyscal_rdf-0.0.7/pyscal_rdf/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import os
 import numpy as np
 from ase.io import write
 
 from pyscal_rdf.visualize import visualize_graph
 from pyscal_rdf.network import OntologyNetwork
 import pyscal_rdf.properties as prp
-from pyscal.core import System
-from pyscal.atoms import Atoms
-from pyscal.core import System
+from pyscal3.core import System
+from pyscal3.atoms import Atoms
+from pyscal3.core import System
 
 CMSO = Namespace("https://purls.helmholtz-metadaten.de/cmso/")
 PLDO = Namespace("https://purls.helmholtz-metadaten.de/pldo/")
 PODO = Namespace("https://purls.helmholtz-metadaten.de/podo/")
 
 defstyledict = {
     "BNode": {"color": "#ffe6ff",
```

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf/json_io.py` & `pyscal_rdf-0.0.7/pyscal_rdf/json_io.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf/network.py` & `pyscal_rdf-0.0.7/pyscal_rdf/network.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf/properties.py` & `pyscal_rdf-0.0.7/pyscal_rdf/properties.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf/queries.py` & `pyscal_rdf-0.0.7/pyscal_rdf/queries.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf/structure.py` & `pyscal_rdf-0.0.7/pyscal_rdf/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 StructureGraph is the central object in pyscal_rdf which combines all the functionality
 of :py:class:`pyscal_rdf.graph.RDFGraph` along with easy structural creation routines.
 """
 import numpy as np
-from pyscal.core import System
-from pyscal.crystal_structures import structure_creator, elements, structures
+from pyscal3.core import System
+from pyscal3.crystal_structures import structure_creator, elements, structures
 from pyscal_rdf.graph import RDFGraph
-from pyscal.grain_boundary import GrainBoundary
+from pyscal3.grain_boundary import GrainBoundary
 
 class StructureGraph(RDFGraph):
     def __init__(self, graph_file=None, 
         store="Memory", 
         store_file=None,
         identifier="default_graph"):
         super().__init__(graph_file=graph_file, store=store, store_file=store_file, identifier=identifier)
```

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf/visualize.py` & `pyscal_rdf-0.0.7/pyscal_rdf/visualize.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf.egg-info/PKG-INFO` & `pyscal_rdf-0.0.7/pyscal_rdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal-rdf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal_rdf-0.0.6/pyscal_rdf.egg-info/SOURCES.txt` & `pyscal_rdf-0.0.7/pyscal_rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/setup.py` & `pyscal_rdf-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal_rdf',
-    version='0.0.6',
+    version='0.0.7',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['pyscal_rdf', 'pyscal_rdf.*']),
     zip_safe=False,
```

### Comparing `pyscal_rdf-0.0.6/tests/test_encoder_and_write.py` & `pyscal_rdf-0.0.7/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/tests/test_graph.py` & `pyscal_rdf-0.0.7/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/tests/test_queries.py` & `pyscal_rdf-0.0.7/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.0.6/tests/test_structuregraph.py` & `pyscal_rdf-0.0.7/tests/test_structuregraph.py`

 * *Files identical despite different names*

