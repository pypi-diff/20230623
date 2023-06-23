# Comparing `tmp/HiPart-0.4.1.tar.gz` & `tmp/HiPart-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiPart-0.4.1.tar", last modified: Tue May 23 12:53:46 2023, max compression
+gzip compressed data, was "HiPart-0.4.2.tar", last modified: Fri Jun 23 14:53:22 2023, max compression
```

## Comparing `HiPart-0.4.1.tar` & `HiPart-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.335885 HiPart-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 12:53:24.000000 HiPart-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 12:53:24.000000 HiPart-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-23 12:53:46.331885 HiPart-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-23 12:53:24.000000 HiPart-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 12:53:24.000000 HiPart-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:53:46.335885 HiPart-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-23 12:53:24.000000 HiPart-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/HiPart/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31954 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/__utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/HiPart/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/assets/int_viz.css
--rw-r--r--   0 runner    (1001) docker     (123)    88495 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/interactive_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-23 12:53:24.000000 HiPart-0.4.1/src/HiPart/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/src/HiPart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 12:53:46.000000 HiPart-0.4.1/src/HiPart.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:53:46.331885 HiPart-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-05-23 12:53:24.000000 HiPart-0.4.1/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:22.640783 HiPart-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-23 14:53:11.000000 HiPart-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 14:53:11.000000 HiPart-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-23 14:53:22.640783 HiPart-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-23 14:53:11.000000 HiPart-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 14:53:12.000000 HiPart-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:53:22.640783 HiPart-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-23 14:53:12.000000 HiPart-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:22.636783 HiPart-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:22.636783 HiPart-0.4.2/src/HiPart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-23 14:53:12.000000 HiPart-0.4.2/src/HiPart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-06-23 14:53:12.000000 HiPart-0.4.2/src/HiPart/__utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:22.640783 HiPart-0.4.2/src/HiPart/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-06-23 14:53:12.000000 HiPart-0.4.2/src/HiPart/assets/int_viz.css
+-rw-r--r--   0 runner    (1001) docker     (123)    92433 2023-06-23 14:53:12.000000 HiPart-0.4.2/src/HiPart/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42704 2023-06-23 14:53:12.000000 HiPart-0.4.2/src/HiPart/interactive_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-06-23 14:53:12.000000 HiPart-0.4.2/src/HiPart/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:22.640783 HiPart-0.4.2/src/HiPart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-23 14:53:22.000000 HiPart-0.4.2/src/HiPart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-23 14:53:22.000000 HiPart-0.4.2/src/HiPart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:53:22.000000 HiPart-0.4.2/src/HiPart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 14:53:22.000000 HiPart-0.4.2/src/HiPart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 14:53:22.000000 HiPart-0.4.2/src/HiPart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:53:22.640783 HiPart-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23291 2023-06-23 14:53:12.000000 HiPart-0.4.2/tests/test_package.py
```

### Comparing `HiPart-0.4.1/LICENSE` & `HiPart-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HiPart-0.4.1/PKG-INFO` & `HiPart-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.4.1
+Version: 0.4.2
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
 Project-URL: Documentation, https://hipart.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/panagiotisanagnostou/HiPart/
```

### Comparing `HiPart-0.4.1/README.md` & `HiPart-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `HiPart-0.4.1/setup.py` & `HiPart-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 setuptools.setup(
     name="HiPart",
     version=__version__,
     url="https://github.com/panagiotisanagnostou/HiPart",
     author="Panagiotis Anagnostou",
     author_email="panagno@uth.gr",
```

### Comparing `HiPart-0.4.1/src/HiPart/__init__.py` & `HiPart-0.4.2/src/HiPart/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,13 +33,13 @@
 
 """
 
 from KDEpy.NaiveKDE import NaiveKDE
 from KDEpy.TreeKDE import TreeKDE
 from KDEpy.FFTKDE import FFTKDE
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __author__ = "Panagiotis Anagnostou"
 
 TreeKDE = TreeKDE
 NaiveKDE = NaiveKDE
 FFTKDE = FFTKDE
```

### Comparing `HiPart-0.4.1/src/HiPart/__utility_functions.py` & `HiPart-0.4.2/src/HiPart/__utility_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,32 +65,41 @@
     Projection of the data matrix onto its first two Components with the
     utilization of the "Principal Components Analysis", "Kernel Principal
     Components Analysis" or "Independent Component Analysis" decomposition
     methods.
 
     Parameters
     ----------
-    two_dimentions
     data_matrix : numpy.ndarray
         The data matrix contains all the data for the samples.
     decomposition_method : str
         One of 'kpca', 'pca' and 'ica' the decomposition methods supported by
         this software.
+    two_dimentions : bool
+        If True the projection will be on the first two components of the 'pca'
+        and 'ica' methods. The 'kpca' and 'tsne' methods will be projected only
+        on one dimension because of the nature.
     decomposition_args : dict
         Arguments to use by each of the decomposition methods utilized by the
-        HIDIV package.
+        HiPart package.
 
     Returns
     -------
     two_dimensions : numpy.ndarray
         The projections of the samples on the first two components of the pca
         and kernel pca methods.
 
     """
     if two_dimentions:
+        if decomposition_method in ["tsne"]:
+            raise ValueError(
+                ": The decomposition method ("
+                + decomposition_method
+                + ") cannot be executed correctly for two dimentions!"
+            )
         n_of_dimentions = 2
     else:
         n_of_dimentions = 1
 
     if decomposition_method == "pca":
         pca = PCA(
             n_components=n_of_dimentions,
```

### Comparing `HiPart-0.4.1/src/HiPart/assets/int_viz.css` & `HiPart-0.4.2/src/HiPart/assets/int_viz.css`

 * *Files identical despite different names*

### Comparing `HiPart-0.4.1/src/HiPart/clustering.py` & `HiPart-0.4.2/src/HiPart/clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 @author Panagiotis Anagnostou
 @author Nicos Pavlidis
 """
 
 import HiPart.__utility_functions as util
 import numpy as np
 import statsmodels.api as sm
+import warnings
 
 from KDEpy import FFTKDE
 from scipy import stats
 from sklearn.cluster import KMeans
 from treelib import Tree
 
 
@@ -57,15 +58,17 @@
         The percentile distance from the dataset's edge in which a split can
         not occur. [0,0.5) values are allowed.
     min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
     visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
-        interactive_visualization of the package can not be created.
+        interactive_visualization of the package can not be created. For the
+        'tsne' decomposition method does not support visualization because it
+        affects the correct execution of the dePDDP algorithm.
     **decomposition_args :
         Arguments for each of the decomposition methods ("decomposition.PCA" as
         "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
         "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
         documented in the scikit-learn package, from which they are implemented.
 
     Attributes
@@ -93,15 +96,19 @@
         **decomposition_args,
     ):
         self.decomposition_method = decomposition_method
         self.max_clusters_number = max_clusters_number
         self.bandwidth_scale = bandwidth_scale
         self.percentile = percentile
         self.min_sample_split = min_sample_split
-        self.visualization_utility = visualization_utility
+        if decomposition_method in ["tsne"]:
+            self.visualization_utility = False
+            warnings.warn("DePDDP: does not support visualization for 'tsne'.")
+        else:
+            self.visualization_utility = visualization_utility
         self.decomposition_args = decomposition_args
 
     def fit(self, X):
         """
         Execute the dePDDP algorithm and return all the execution data in the
         form of a dePDDP class object.
 
@@ -427,14 +434,32 @@
         if v < 0 or (not isinstance(v, int)):
             raise ValueError(
                 "DePDDP: min_sample_split: Invalid value it should be int and > 1"
             )
         self._min_sample_split = v
 
     @property
+    def visualization_utility(self):
+        return self._visualization_utility
+
+    @visualization_utility.setter
+    def visualization_utility(self, v):
+        if v is not True and v is not False:
+            raise ValueError(
+                "DePDDP: visualization_utility: Should be True or False"
+            )
+
+        if v is True and self.decomposition_method not in ["pca", "ica", "kpca"]:
+            raise ValueError(
+                "DePDDP: visualization_utility: 'tsne' method is can't be used"
+                + " with the visualization utility."
+            )
+        self._visualization_utility = v
+
+    @property
     def tree(self):
         return self._tree
 
     @tree.setter
     def tree(self, v):
         self._tree = v
 
@@ -513,15 +538,17 @@
         The percentile distance from the dataset's edge in which a split can
         not occur. [0,0.5) values are allowed.
     min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
     visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
-        interactive_visualization of the package can not be created.
+        interactive_visualization of the package can not be created. For the
+        'tsne' decomposition method does not support visualization because it
+        affects the correct execution of the iPDDP algorithm.
     **decomposition_args :
         Arguments for each of the decomposition methods ("decomposition.PCA" as
         "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
         "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
         documented in the scikit-learn package, from which they are implemented.
 
     Attributes
@@ -547,15 +574,19 @@
         visualization_utility=True,
         **decomposition_args,
     ):
         self.decomposition_method = decomposition_method
         self.max_clusters_number = max_clusters_number
         self.percentile = percentile
         self.min_sample_split = min_sample_split
-        self.visualization_utility = visualization_utility
+        if decomposition_method in ["tsne"]:
+            self.visualization_utility = False
+            warnings.warn("IPDDP: does not support visualization for 'tsne'.")
+        else:
+            self.visualization_utility = visualization_utility
         self.decomposition_args = decomposition_args
 
     def fit(self, X):
         """
         Execute the iPDDP algorithm and return all the execution data in the
         form of a IPDDP class object.
 
@@ -865,14 +896,31 @@
         if v < 0 or (not isinstance(v, int)):
             raise ValueError(
                 "IPDDP: min_sample_split: Invalid value it should be int and > 1"
             )
         self._min_sample_split = v
 
     @property
+    def visualization_utility(self):
+        return self._visualization_utility
+
+    @visualization_utility.setter
+    def visualization_utility(self, v):
+        if v is not True and v is not False:
+            raise ValueError(
+                "IPDDP: visualization_utility: Should be True or False"
+            )
+
+        if v is True and self.decomposition_method not in ["pca", "ica", "kpca"]:
+            raise ValueError(
+                "IPDDP: visualization_utility: Should be pca when visualization_utility is True."
+            )
+        self._visualization_utility = v
+
+    @property
     def tree(self):
         return self._tree
 
     @tree.setter
     def tree(self, v):
         self._tree = v
 
@@ -948,15 +996,17 @@
     max_clusters_number : int, (optional)
         Desired maximum number of clusters for the algorithm.
     min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
     visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
-        interactive_visualization of the package can not be created.
+        interactive_visualization of the package can not be created. For the
+        'tsne' decomposition method does not support visualization because it
+        affects the correct execution of the kMeans-PDDP algorithm.
     random_seed : int, (optional)
         The random seed fed in the k-Means algorithm
     **decomposition_args :
         Arguments for each of the decomposition methods ("decomposition.PCA" as
         "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
         "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
         documented in the scikit-learn package, from which they are implemented.
@@ -983,15 +1033,19 @@
         visualization_utility=True,
         random_seed=None,
         **decomposition_args,
     ):
         self.decomposition_method = decomposition_method
         self.max_clusters_number = max_clusters_number
         self.min_sample_split = min_sample_split
-        self.visualization_utility = visualization_utility
+        if decomposition_method in ["tsne"]:
+            self.visualization_utility = False
+            warnings.warn("KMPDDP: does not support visualization for 'tsne'.")
+        else:
+            self.visualization_utility = visualization_utility
         self.random_seed = random_seed
         self.decomposition_args = decomposition_args
 
     def fit(self, X):
         """
         Execute the kM-PDDP algorithm and return all the execution data in the
         form of a kM_PDDP class object.
@@ -1301,14 +1355,31 @@
         if v is not None and (not isinstance(v, int)):
             raise ValueError(
                 "KMPDDP: min_sample_split: Invalid value it should be int and > 1"
             )
         self._random_seed = v
 
     @property
+    def visualization_utility(self):
+        return self._visualization_utility
+
+    @visualization_utility.setter
+    def visualization_utility(self, v):
+        if v is not True and v is not False:
+            raise ValueError(
+                "KMPDDP: visualization_utility: Should be True or False"
+            )
+
+        if v is True and self.decomposition_method not in ["pca", "ica", "kpca"]:
+            raise ValueError(
+                "KMPDDP: visualization_utility: Should be pca when visualization_utility is True"
+            )
+        self._visualization_utility = v
+
+    @property
     def tree(self):
         return self._tree
 
     @tree.setter
     def tree(self, v):
         self._tree = v
 
@@ -1381,15 +1452,17 @@
     max_clusters_number : int, (optional)
         Desired maximum number of clusters for the algorithm.
     min_sample_split : int, (optional)
         The minimum number of points needed in a cluster for a split to occur.
     visualization_utility : bool, (optional)
         If (True) generate the data needed by the visualization utilities of
         the package otherwise, if false the split_visualization and
-        interactive_visualization of the package can not be created.
+        interactive_visualization of the package can not be created. For the
+        'tsne' decomposition method does not support visualization because it
+        affects the correct execution of the PDDP algorithm.
     **decomposition_args :
         Arguments for each of the decomposition methods ("decomposition.PCA" as
         "pca", "decomposition.KernelPCA" as "kpca", "decomposition.FastICA" as
         "ica", "manifold.TSNE" as "tsne") utilized by the HiPart package, as
         documented in the scikit-learn package, from which they are implemented.
 
     Attributes
@@ -1413,15 +1486,19 @@
         min_sample_split=5,
         visualization_utility=True,
         **decomposition_args,
     ):
         self.decomposition_method = decomposition_method
         self.max_clusters_number = max_clusters_number
         self.min_sample_split = min_sample_split
-        self.visualization_utility = visualization_utility
+        if decomposition_method in ["tsne"]:
+            self.visualization_utility = False
+            warnings.warn("PDDP: does not support visualization for 'tsne'.")
+        else:
+            self.visualization_utility = visualization_utility
         self.decomposition_args = decomposition_args
 
     def fit(self, X):
         """
         Execute the PDDP algorithm and return all the execution data in the
         form of a PDDP class object.
 
@@ -1702,14 +1779,31 @@
         if v < 0 or (not isinstance(v, int)):
             raise ValueError(
                 "PDDP: min_sample_split: Invalid value it should be int and > 1"
             )
         self._min_sample_split = v
 
     @property
+    def visualization_utility(self):
+        return self._visualization_utility
+
+    @visualization_utility.setter
+    def visualization_utility(self, v):
+        if v is not True and v is not False:
+            raise ValueError(
+                "PDDP: visualization_utility: Should be True or False"
+            )
+
+        if v is True and self.decomposition_method not in ["pca", "ica", "kpca"]:
+            raise ValueError(
+                "PDDP: visualization_utility: Should be pca when visualization_utility is True"
+            )
+        self._visualization_utility = v
+
+    @property
     def tree(self):
         return self._tree
 
     @tree.setter
     def tree(self, v):
         self._tree = v
 
@@ -2119,27 +2213,30 @@
         # transpose the output_matrix to be extracted
         output_matrix = np.array(output_matrix).transpose()
 
         return output_matrix
 
     @output_matrix.setter
     def output_matrix(self, v):
-        self._output_matrix = v
+        raise RuntimeError(
+            "BisectingKmeans: output_matrix: can only be generated and not to be assigned!"
+        )
 
     @property
     def labels_(self):
         labels_ = np.ones(np.size(self.X, 0))
         for i in self.tree.leaves():
             labels_[i.data["indices"]] = i.identifier
-        self.labels_ = labels_
-        return self._labels_
+        return labels_
 
     @labels_.setter
     def labels_(self, v):
-        self._labels_ = v
+        raise RuntimeError(
+            "BisectingKmeans: labels_: can only be generated and not to be assigned!"
+        )
 
 
 class MDH:
     """
     Class MDH. It executes the MDH algorithm.
 
     References
@@ -2158,15 +2255,15 @@
         The multiples of the standard deviation which the existence of a
         splitting hyperplane is allowed. The default value is 2.3.
     percentile : float, optional
         The percentile distance from the dataset's edge in which a split can
         not occur. [0,0.5) values are allowed.
     min_sample_split : int, optional
         The minimum number of points needed in a cluster for a split to occur.
-    random_seed : int, optional
+    random_state : int, optional
         The random seed to be used in the algorithm's execution.
 
     Attributes
     ----------
     output_matrix : numpy.ndarray
         Model's step by step execution output.
     labels_ : numpy.ndarray
@@ -2436,15 +2533,15 @@
                     # res has the following fields that are of interest:
                     #   1. success (whether algorithm terminated successfully)
                     #   2. x (solution)
                     #   3. nfev (number of function evaluations)
                     #   4. njev (number of jacobian/ gradient evaluations)
                     results, depth = util.md_sqp(initial_v_n_b, node_data, self.k)
 
-                    # If the algorithm terminated successfully try appending the append the solution
+                    # If the algorithm terminated successfully try to append the solution
                     if results.success:
                         v = results.x[:-1] / np.linalg.norm(results.x[:-1])
                         projection = np.dot(node_data, v).reshape(-1, 1)
                         b = results.x[-1]
                         c0 = np.sum(projection > b)
                         # Solutions in the edges of the projection are not acceptable
                         if min(c0, node_size - c0) >= minC:
```

### Comparing `HiPart-0.4.1/src/HiPart/interactive_visualization.py` & `HiPart-0.4.2/src/HiPart/interactive_visualization.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.4.1/src/HiPart/visualizations.py` & `HiPart-0.4.2/src/HiPart/visualizations.py`

 * *Files identical despite different names*

### Comparing `HiPart-0.4.1/src/HiPart.egg-info/PKG-INFO` & `HiPart-0.4.2/src/HiPart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiPart
-Version: 0.4.1
+Version: 0.4.2
 Summary: A hierarchical divisive clustering toolbox
 Home-page: https://github.com/panagiotisanagnostou/HiPart
 Author: Panagiotis Anagnostou
 Author-email: panagno@uth.gr
 License: MIT License
 Project-URL: Documentation, https://hipart.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/panagiotisanagnostou/HiPart/
```

### Comparing `HiPart-0.4.1/tests/test_package.py` & `HiPart-0.4.2/tests/test_package.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,16 +105,26 @@
         DePDDP(percentile=.8)
     except Exception:
         success_score += 1
     try:
         DePDDP(min_sample_split=-5)
     except Exception:
         success_score += 1
+    try:
+        obj = DePDDP()
+        obj.output_matrix = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
+    try:
+        obj = DePDDP()
+        obj.labels_ = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
 
-    assert success_score == 11
+    assert success_score == 13
 
 
 def test_ipddp_parameter_errors(datadir):
     success_score = 0
 
     algorithm = IPDDP()
     success_score += 1 if isinstance(algorithm.decomposition_method, str) else 0
@@ -135,16 +145,26 @@
         IPDDP(percentile=.8)
     except Exception:
         success_score += 1
     try:
         IPDDP(min_sample_split=-5)
     except Exception:
         success_score += 1
+    try:
+        obj = IPDDP()
+        obj.output_matrix = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
+    try:
+        obj = IPDDP()
+        obj.labels_ = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
 
-    assert success_score == 9
+    assert success_score == 11
 
 
 def test_kmpddp_parameter_errors(datadir):
     success = 0
 
     algorithm = KMPDDP(random_seed=123)
     success += 1 if isinstance(algorithm.decomposition_method, str) else 0
@@ -165,16 +185,26 @@
         KMPDDP(random_seed=.8)
     except Exception:
         success += 1
     try:
         KMPDDP(min_sample_split=-5)
     except Exception:
         success += 1
+    try:
+        obj = KMPDDP()
+        obj.output_matrix = np.array([1, 2, 3])
+    except Exception:
+        success += 1
+    try:
+        obj = KMPDDP()
+        obj.labels_ = np.array([1, 2, 3])
+    except Exception:
+        success += 1
 
-    assert success == 9
+    assert success == 11
 
 
 def test_pddp_parameter_errors(datadir):
     success_score = 0
 
     algorithm = PDDP()
     success_score += 1 if isinstance(algorithm.decomposition_method, str) else 0
@@ -190,16 +220,26 @@
         PDDP(max_clusters_number=-5)
     except Exception:
         success_score += 1
     try:
         PDDP(min_sample_split=-5)
     except Exception:
         success_score += 1
+    try:
+        obj = PDDP()
+        obj.output_matrix = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
+    try:
+        obj = PDDP()
+        obj.labels_ = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
 
-    assert success_score == 7
+    assert success_score == 9
 
 
 def test_bicecting_kmeans_parameter_errors():
     success_score = 0
 
     algorithm = BisectingKmeans(random_seed=5)
     success_score += 1 if isinstance(algorithm.max_clusters_number, int) else 0
@@ -214,16 +254,26 @@
         BisectingKmeans(random_seed=.8)
     except Exception:
         success_score += 1
     try:
         BisectingKmeans(min_sample_split=-5)
     except Exception:
         success_score += 1
+    try:
+        obj = BisectingKmeans()
+        obj.output_matrix = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
+    try:
+        obj = BisectingKmeans()
+        obj.labels_ = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
 
-    assert success_score == 6
+    assert success_score == 8
 
 
 def test_mdh_parameter_errors():
     success_score = 0
 
     algorithm = MDH(random_state=5)
     success_score += 1 if isinstance(algorithm.max_clusters_number, int) else 0
@@ -253,16 +303,26 @@
         MDH(random_state=.8)
     except Exception:
         success_score += 1
     try:
         MDH(min_sample_split=-5)
     except Exception:
         success_score += 1
+    try:
+        obj = MDH()
+        obj.output_matrix = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
+    try:
+        obj = MDH()
+        obj.labels_ = np.array([1, 2, 3])
+    except Exception:
+        success_score += 1
 
-    assert success_score == 12
+    assert success_score == 14
 
 
 def test_depddp_labels__return_type_and_form(datadir):
     with open(datadir.join('test_data.dump'), "rb") as inf:
         data_import = pickle.load(inf)
 
     results = DePDDP(max_clusters_number=5).fit_predict(data_import["data"])
```

