# Comparing `tmp/xenosite-fragment-0a7.tar.gz` & `tmp/xenosite-fragment-0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenosite-fragment-0a7.tar", last modified: Sat Jun 17 22:07:51 2023, max compression
+gzip compressed data, was "xenosite-fragment-0a8.tar", last modified: Fri Jun 23 15:58:53 2023, max compression
```

## Comparing `xenosite-fragment-0a7.tar` & `xenosite-fragment-0a8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3735 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/README.md
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1808 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/test/
--rw-r--r--   0 root         (0) root         (0)     2294 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_fragment.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_morgan.py
--rw-r--r--   0 root         (0) root         (0)     7779 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_netx.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_remap.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/test/test_tanimoto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite/fragment/
--rw-r--r--   0 root         (0) root         (0)     3976 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9026 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/__main__.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite/fragment/_static_version.py
--rw-r--r--   0 root         (0) root         (0)     5773 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/_version.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/chem.py
--rw-r--r--   0 root         (0) root         (0)     6224 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/feature.py
--rw-r--r--   0 root         (0) root         (0)     5887 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/graph.py
--rw-r--r--   0 root         (0) root         (0)     1236 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/keras_backend.py
--rw-r--r--   0 root         (0) root         (0)     3063 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/morgan.py
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/netx.py
--rw-r--r--   0 root         (0) root         (0)     3180 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/remap.py
--rw-r--r--   0 root         (0) root         (0)     5640 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/serialize.py
--rw-r--r--   0 root         (0) root         (0)     3650 2023-06-17 22:07:50.000000 xenosite-fragment-0a7/xenosite/fragment/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 22:07:51.207681 xenosite-fragment-0a7/xenosite_fragment.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      765 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-17 22:07:51.000000 xenosite-fragment-0a7/xenosite_fragment.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/README.md
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.654178 xenosite-fragment-0a8/test/
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_fragment.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_morgan.py
+-rw-r--r--   0 root         (0) root         (0)     7779 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_netx.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_remap.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_tanimoto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.654178 xenosite-fragment-0a8/xenosite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/xenosite/fragment/
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9026 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/xenosite/fragment/_static_version.py
+-rw-r--r--   0 root         (0) root         (0)     5773 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/_version.py
+-rw-r--r--   0 root         (0) root         (0)    14809 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/chem.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/feature.py
+-rw-r--r--   0 root         (0) root         (0)     7165 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/keras_backend.py
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/netx.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/ops.py
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/remap.py
+-rw-r--r--   0 root         (0) root         (0)     5640 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/xenosite_fragment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      762 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/top_level.txt
```

### Comparing `xenosite-fragment-0a7/PKG-INFO` & `xenosite-fragment-0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a7
+Version: 0a8
 Summary: Library for molecule fragment operations.
 Home-page: UNKNOWN
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Education
```

### Comparing `xenosite-fragment-0a7/README.md` & `xenosite-fragment-0a8/README.md`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/setup.py` & `xenosite-fragment-0a8/setup.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/test/test_fragment.py` & `xenosite-fragment-0a8/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/test/test_morgan.py` & `xenosite-fragment-0a8/test/test_morgan.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xenosite.fragment import morgan as mg
+from xenosite.fragment import ops as mg
 from hypothesis import strategies as st, given
 from pytest import approx
 import pytest
 import numpy as np
 
 
 @pytest.mark.parametrize(
```

### Comparing `xenosite-fragment-0a7/test/test_netx.py` & `xenosite-fragment-0a8/test/test_netx.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/test/test_remap.py` & `xenosite-fragment-0a8/test/test_remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/test/test_tanimoto.py` & `xenosite-fragment-0a8/test/test_tanimoto.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/__init__.py` & `xenosite-fragment-0a8/xenosite/fragment/__init__.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/__main__.py` & `xenosite-fragment-0a8/xenosite/fragment/__main__.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/_version.py` & `xenosite-fragment-0a8/xenosite/fragment/_version.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/chem.py` & `xenosite-fragment-0a8/xenosite/fragment/chem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from rdkit import Chem
 from .graph import Graph
 from .serialize import Serialized
 from typing import Callable, Optional, Union, Generator, Sequence, NamedTuple
-from .morgan import to_range 
+from .ops import to_range 
 import networkx as nx
+import numpy as np
 
 Mol = Chem.rdchem.Mol
 Atom = Chem.rdchem.Atom
 Bond = Chem.rdchem.Bond
 
 
 class FragmentEquivalence(NamedTuple):
@@ -168,17 +169,16 @@
         """
         Determine which atoms in a fragment are topologically equivalent.
 
         :return: Tuple of numpy array with group assignment, and the integer number of distinct topological groups.
         :rtype: FragmentEquivalence
         """        
 
-        m = self.graph.morgan()
-        i,ni = to_range(m)
-        return FragmentEquivalence(i, ni) #type: ignore
+        o = self.graph._nauty_orbits()
+        return FragmentEquivalence(o, np.max(o)) #type: ignore
 
     def canonical(self, remap=False) -> Serialized:
         """
         Canonical representation of Fragment, with reordering from input molecule.
 
         :return: Cannonical string representation of fragment.
         :rtype: Serialized
@@ -293,14 +293,60 @@
     
     if min(A,B) / max(A,B) < cutoff: return 0.0
     AnB = _maximum_common_subgraph(m1, m2, allow_disconnected)
 
     return AnB / (A + B - AnB) 
 
 
+#TODO: implment a version/option of this function uses the edge count instead of just the atoms.
+#TODO: add convenience conversion from Fragment or str to rdkit.Mol
+def smarts_edit_distance(m1 : Chem.Mol, m2 : Chem.Mol, cutoff : float = 10, allow_disconnected : bool = True) -> float: #type: ignore
+    """Vertex edit distance between two SMARTS rdkit mols. Overlap is not mesured using a fingerprint, but 
+    by computing the max-common-structure overlap (in atoms) of the two, so this can be slow.
+
+    For example, these two molecules/SMARTS overlap in 3 out of 4 molecules, yielding an edit of 1. 
+
+    >>> from rdkit import Chem
+    >>> m1 = Chem.MolFromSmarts("CCC")
+    >>> m2 = Chem.MolFromSmarts("CCCC")
+    >>> smarts_edit_distance(m1, m2)
+    1
+
+    These two molecules yield the same edit distance because the SMARTS string allows for either
+    a C or an N in the third position.
+
+    >>> m1 = Chem.MolFromSmarts("CCN")
+    >>> m2 = Chem.MolFromSmarts("CC[C,N]C")
+    >>> smarts_edit_distance(m1, m2)
+    1
+
+    Cutoff is the maximum edit-distance we care about, which can speed computation by avoiding the MCS
+    computation in some cases. When this threshold can't be met, the edit is reported as the cutoff value.
+
+    >>> smarts_edit_distance(m1, m2, cutoff=0.5)
+    0.5
+
+    Note that the function will still report edit distance, if it exists and even if it is above cutoff, when
+    the MSC step is run. In the following case, 3 out of 5 atoms match, but based on size of the framents 
+    alone 4 out of 4 atoms could have matched. So the MCS was run, and the 2 edit distance was reported even
+    though it was above the cutoff.
+
+    >>> m1 = Chem.MolFromSmarts("OCCN")
+    >>> m2 = Chem.MolFromSmarts("CC[C,N]C")
+    >>> smarts_edit_distance(m1, m2, cutoff=0.5)
+    2
+
+    """
+    A = m1.GetNumAtoms()
+    B = m2.GetNumAtoms()
+    
+    if max(A,B) - min(A,B) > cutoff: return cutoff
+    AnB = _maximum_common_subgraph(m1, m2, allow_disconnected)
+
+    return A + B - 2 * AnB
 
 def _modular_product_graph(m1 : Chem.Mol, m2: Chem.Mol) -> nx.Graph: #type: ignore
     """This function converts two molecules into a modular product graph.
     Cliques in a modular product graph correspond to the maximum-common substructure.
     Uses rdkit mols to make use of SMARTS matching logic.
     
     https://en.wikipedia.org/wiki/Modular_product_of_graphs
```

### Comparing `xenosite-fragment-0a7/xenosite/fragment/feature.py` & `xenosite-fragment-0a8/xenosite/fragment/feature.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/graph.py` & `xenosite-fragment-0a8/xenosite/fragment/graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import NamedTuple, Optional, Sequence, Union, Any
-from numba import jit, njit
+from numba import njit
+from collections import defaultdict
 import numpy as np
+import pynauty
 
 from . import serialize
-from .morgan import morgan
+from .ops import morgan, to_range, segment_min
 
 
 class BaseGraph:
     def __init__(
         self,
         n: int,
         edge: tuple[Sequence[np.uint32], Sequence[np.uint32]],
@@ -81,14 +83,25 @@
 
         eid = np.arange(ne, dtype=np.int64) + self.n
 
         e1 = np.concatenate([e1.ravel(), e2.ravel()])
         e2 = np.concatenate([eid, eid])
 
         return Graph(n=self.n + ne, edge=(e1, e2), nlabel=nlabel)  # type: ignore
+    
+    def neighbors(self) -> list[list[int]]:
+        N = [[] for _ in range(self.n)]
+
+        for i, j in zip(self.edge[0], self.edge[1]):
+            N[i].append(j)
+            N[j].append(i)
+
+        return N
+    
+
 
     def morgan(self) -> np.ndarray[np.int64]:
         try:
             _ = self._morgan
         except:
 
           if self.elabel:
@@ -98,37 +111,76 @@
               e1 = self.edge[0]
               e2 = self.edge[1]
 
               self._morgan = morgan(self.nlabel, e1, e2)  # type: ignore
     
         return self._morgan
 
+    
     def _to_nauty(self, colors=True):
-        import pynauty
-        g = pynauty.Graph(self.n)
-        for i,j in zip(*self.edge): g.connect_vertex(i,j)
+
+        adj = defaultdict(list)
+        for i in range(len(self.edge[0])):
+            adj[self.edge[0][i]].append(self.edge[1][i])
+
+        # # equiv loop:
+        # for i, j in zip(*self.edge):
+        #     adj[i].append(j)
 
         if colors and self.nlabel:
-            c = self.nlabel
-            c = _to_nauty_colors(c)
-            g.set_vertex_coloring(c)         
+            c = _to_nauty_colors(self.nlabel)   
+        else:
+            c = []
+
+        g = pynauty.Graph(self.n)
+
+        # setting adj and color, bypassing all checks
+        g._adjacency_dict = adj
+        g._vertex_coloring = c
         return g
     
     def _nauty_order(self):
         import pynauty
         if self.elabel:
             return self.edge_to_node()._nauty_order()[:self.n]
         
         g = self._to_nauty()
 
         c = pynauty.canon_label(g)
         c = np.asarray(c) #type:  ignore
         c = _invert_mapping(c)
         return c
 
+    def _nauty_orbits(self):
+        import pynauty
+        if self.elabel:
+            o = self.edge_to_node()._nauty_orbits()[:self.n]
+            o = to_range(o)[0]
+            return o
+        
+        g = self._to_nauty()
+
+        o = pynauty.autgrp(g)[3] # orbits of each vertex (equivalent groups) with non canonical colors
+
+        # Canonize using cannoical ordering
+        c = pynauty.canon_label(g)
+        c = np.asarray(c) #type:  ignore
+        c = _invert_mapping(c)
+
+        # canonical color for each orbit
+        o = to_range(o)[0]
+        can_o = segment_min(c, o)
+        can_o = to_range(can_o)[0]
+
+        # canonical orbit for each vertex
+        o = np.take(can_o, o)
+
+        return o
+
+
     def serialize(self, canonize=True) -> serialize.Serialized:
         return serialize.serialize(self, canonize)
 
     @classmethod
     def from_molecule(cls, molecule, smiles=False) -> "Graph":
         from . import chem  # lazy import to prevent load of rdkit unless needed
 
@@ -207,15 +259,16 @@
             N[n] = sorted(N[n], key=lambda x: M[x])
     else:
         for n in N:
             N[n] = sorted(N[n])
 
     return _dfs(start, N)
 
-
-def neighbors(G: Graph) -> dict[int, list[int]]:
-    N = {n: [] for n in range(G.n)}
+def neighbors(G: Graph) -> dict[int,list[int]]:
+    N = [[] for _ in range(G.n)]
 
     for i, j in zip(G.edge[0], G.edge[1]):
         N[i].append(j)
         N[j].append(i)
+
+    N = {i: N[i] for i in range(G.n)}
     return N
```

### Comparing `xenosite-fragment-0a7/xenosite/fragment/keras_backend.py` & `xenosite-fragment-0a8/xenosite/fragment/keras_backend.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/remap.py` & `xenosite-fragment-0a8/xenosite/fragment/remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/serialize.py` & `xenosite-fragment-0a8/xenosite/fragment/serialize.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a7/xenosite/fragment/stats.py` & `xenosite-fragment-0a8/xenosite/fragment/stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 from collections import defaultdict
 from .graph import Graph
 import numpy as np
 from functools import reduce
 from scipy.stats import hypergeom
 import pandas as pd
 from typing import Optional
-
+from .ops import segment_max
+from . import Fragment
 
 class FragmentStatistics:
+    # the statistics that are static, not accumulated, in updates
+    static_stats = {"size", "equivalence_group", "frag"}
+
     def __init__(self):
         self._stats: dict = defaultdict(list)
         self._lookup: dict[str, int] = {}
 
     def add(
         self, frag: str, ids: list[list[int]], marked: set[int], mol_atoms: int
     ) -> None:
         assert frag not in self._lookup
         assert self._stats is not None
 
         S = dict()
 
+        F = Fragment(frag)
+        eq = F.equivalence()[0]
+
         amarked = np.array(list(marked))[None, None, :]
 
         # normalized count of marked ids by position in fragment
         marked_ids = (np.array(ids)[:, :, None] == amarked).sum(axis=0).sum(axis=1)
         marked_ids = np.where(marked_ids > 0, 1, 0)  # type: ignore
 
+        # deal with fragment symmetries
+        marked_groups = segment_max(marked_ids, eq)
+        marked_ids = marked_groups[eq]
+
         set_ids = [set(i) for i in ids]
 
         size = len(set_ids[0])
 
         covered = reduce(lambda x, y: x | y, set_ids)
 
         marked_count = (
@@ -39,29 +50,32 @@
                     [i for i in set_ids if marked & i],
                     set(),
                 )
             )
             / size
         )
 
-        # exp = probability of fragment overlapping with at least one marked atom
-        # given: size of molecule, number of atoms matching fragment, number of marked atoms
-        exp = 1 - hypergeom.cdf(0, mol_atoms, int(len(covered)), len(marked))
-        obs = 1 if marked_count else 0
+        # # exp = probability of fragment overlapping with at least one marked atom
+        # # given: size of molecule, number of atoms matching fragment, number of marked atoms
+        # exp = 1 - hypergeom.cdf(0, mol_atoms, int(len(covered)), len(marked))
+        # obs = 1 if marked_count else 0
+        # S["exp"] = exp
+        # S["obs"] = obs
 
         S["count"] = len(covered) / size
         S["marked_count"] = marked_count
         S["n_mol"] = 1
         S["n_atom"] = mol_atoms
         S["n_mark"] = len(marked)
         S["n_cover"] = len(covered)
         S["n_mark_cover"] = len(covered & marked)
-        S["exp"] = exp
-        S["obs"] = obs
+        S["marked_groups"] = marked_groups
+        S["equivalence_group"] = eq
         S["marked_ids"] = marked_ids
+        S["size"] = len(eq)
 
         self.append_one(frag, **S)
 
     def copy_from(self, other : "FragmentStatistics") -> "FragmentStatistics":
       k1 = set(self._stats['frag'])
       k2 = set(other._stats['frag'])
 
@@ -90,15 +104,16 @@
         if self._stats:
           assert set(kwargs) | {"frag"} == set(self._stats), \
             "must always call FragmentStatistics.update_one with the same arguments."
 
         if frag in self._lookup:
             n = self._lookup[frag]
             for k in kwargs:
-                self._stats[k][n] = self._stats[k][n] + kwargs[k]
+                if k not in self.static_stats:
+                    self._stats[k][n] = self._stats[k][n] + kwargs[k]
         else:
             self.append_one(frag, **kwargs)
 
     def to_pandas(self) -> pd.DataFrame:
         return pd.DataFrame(self._stats).set_index("frag")
 
     def update(self, other: "FragmentStatistics"):
```

### Comparing `xenosite-fragment-0a7/xenosite_fragment.egg-info/PKG-INFO` & `xenosite-fragment-0a8/xenosite_fragment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a7
+Version: 0a8
 Summary: Library for molecule fragment operations.
 Home-page: UNKNOWN
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Education
```

### Comparing `xenosite-fragment-0a7/xenosite_fragment.egg-info/SOURCES.txt` & `xenosite-fragment-0a8/xenosite_fragment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 xenosite/fragment/__main__.py
 xenosite/fragment/_static_version.py
 xenosite/fragment/_version.py
 xenosite/fragment/chem.py
 xenosite/fragment/feature.py
 xenosite/fragment/graph.py
 xenosite/fragment/keras_backend.py
-xenosite/fragment/morgan.py
 xenosite/fragment/netx.py
+xenosite/fragment/ops.py
 xenosite/fragment/remap.py
 xenosite/fragment/serialize.py
 xenosite/fragment/stats.py
 xenosite_fragment.egg-info/PKG-INFO
 xenosite_fragment.egg-info/SOURCES.txt
 xenosite_fragment.egg-info/dependency_links.txt
 xenosite_fragment.egg-info/entry_points.txt
```

