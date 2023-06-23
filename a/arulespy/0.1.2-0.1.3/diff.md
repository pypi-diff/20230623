# Comparing `tmp/arulespy-0.1.2.tar.gz` & `tmp/arulespy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arulespy-0.1.2.tar", last modified: Wed May 31 16:19:17 2023, max compression
+gzip compressed data, was "arulespy-0.1.3.tar", last modified: Fri Jun 23 19:43:09 2023, max compression
```

## Comparing `arulespy-0.1.2.tar` & `arulespy-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-31 16:19:07.000000 arulespy-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 16:19:07.000000 arulespy-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-31 16:19:17.344966 arulespy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-05-31 16:19:07.000000 arulespy-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 16:19:07.000000 arulespy-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 16:19:17.344966 arulespy-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-31 16:19:07.000000 arulespy-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/src/arulespy/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-31 16:19:07.000000 arulespy-0.1.2/src/arulespy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-31 16:19:07.000000 arulespy-0.1.2/src/arulespy/arules.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 16:19:07.000000 arulespy-0.1.2/src/arulespy/arulesViz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/src/arulespy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-31 16:19:07.000000 arulespy-0.1.2/tests/test_arules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:43:09.467776 arulespy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-23 19:42:57.000000 arulespy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 19:42:57.000000 arulespy-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-23 19:43:09.467776 arulespy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-06-23 19:42:57.000000 arulespy-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 19:42:57.000000 arulespy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 19:43:09.467776 arulespy-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-23 19:42:57.000000 arulespy-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:43:09.467776 arulespy-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:43:09.467776 arulespy-0.1.3/src/arulespy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-23 19:42:57.000000 arulespy-0.1.3/src/arulespy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-06-23 19:42:57.000000 arulespy-0.1.3/src/arulespy/arules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-23 19:42:57.000000 arulespy-0.1.3/src/arulespy/arulesViz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:43:09.467776 arulespy-0.1.3/src/arulespy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-23 19:43:09.000000 arulespy-0.1.3/src/arulespy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 19:43:09.000000 arulespy-0.1.3/src/arulespy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:43:09.000000 arulespy-0.1.3/src/arulespy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 19:43:09.000000 arulespy-0.1.3/src/arulespy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 19:43:09.000000 arulespy-0.1.3/src/arulespy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:43:09.467776 arulespy-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-23 19:42:57.000000 arulespy-0.1.3/tests/test_arules.py
```

### Comparing `arulespy-0.1.2/LICENSE` & `arulespy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arulespy-0.1.2/PKG-INFO` & `arulespy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arulespy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface to the R package arules
 Home-page: https://github.com/mhahsler/arulespy
 Author: Michael Hahsler
 Author-email: mhahsler@lyle.smu.edu
 Project-URL: Documentation, https://github.com/mhahsler/arulespy
 Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
 Project-URL: Source Code, https://github.com/mhahsler/arulespy
```

### Comparing `arulespy-0.1.2/README.md` & `arulespy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arulespy-0.1.2/setup.py` & `arulespy-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `arulespy-0.1.2/src/arulespy/__init__.py` & `arulespy-0.1.3/src/arulespy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 import rpy2.robjects as ro
 import rpy2.robjects.packages as packages
 import os
 
 os.makedirs(ro.r('Sys.getenv("R_LIBS_USER")')[0], exist_ok=True)
 ro.r('.libPaths(c(Sys.getenv("R_LIBS_USER"), .libPaths()))')
@@ -18,9 +18,9 @@
 if not ro.packages.isinstalled('arulesViz'):
     print("Installing R package arulesViz (plus dependencies).")
     utils.install_packages('arulesViz', 
                            repos='https://cloud.r-project.org/',
                            lib = ro.r('Sys.getenv("R_LIBS_USER")[1]'))
 
               
-from .arules import parameters, Associations, ItemMatrix, Rules, Itemsets, Transactions, R, a2py, concat, apriori, eclat, discretizeDF
-from .arulesViz import plot, inspectDT
+from .arules import R_arules, arules2py, parameters, Associations, ItemMatrix, Rules, Itemsets, Transactions, concat, apriori, eclat, discretizeDF
+from .arulesViz import R_arulesViz, plot, inspectDT, ruleExplorer
```

### Comparing `arulespy-0.1.2/src/arulespy/arules.py` & `arulespy-0.1.3/src/arulespy/arules.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,42 @@
 ### activate automatic conversion of pandas dataframes to R dataframes
 #pandas2ri.activate()
 
 # install arules if necessary. Note: the system path is probably not writable for the user.
 # we try to create the directory so install.packages does not ask
 
 ### import the R arules package
-R = packages.importr('arules')
+R_arules = packages.importr('arules')
 methods = packages.importr('methods')
 base = packages.importr('base')
 
 ### Sparse matrix helper
 def ngC_to_csc_matrix(m):
     """convert a ngCMatrix to a scipy csc_matrix"""
     indices = np.array(m.slots['i'])
     indptr  = np.array(m.slots['p'])
     ## all ones for ngCMatrix
     data = np.array([1]*len(indices))
     return csc_matrix((data, indices, indptr), tuple(m.slots['Dim']))    
 
 ### Conversion functions
-def a2py(x):
+def arules2py(x):
     """convert arules S4 object to python object
     
     Conversion rules:
     - rules: Python Rules object
     - itemsets: Python Itemsets object
     - transactions: Python Transactions object
     - itemMatrix: Python ItemMatrix object
     - data.frame: pandas dataframe
     - character: string list
     - integer: int list
     - numeric: float list
-    - matrix: numpy matrix
+    - logical: bool list
+    - matrix: numpy array
     """
 
     if x.rclass[0] == "rules":
         return Rules(x)
     elif x.rclass[0] == "itemsets":
         return Itemsets(x)
     elif x.rclass[0] == "transactions":
@@ -64,71 +65,64 @@
         return list(x)
     elif x.rclass[0] == "matrix":
         return np.array(x)
 
     else:
         return x
 
-def a2py_decor(function):
+def arules2py_decor(function):
     """decorator to convert arules S4 objects to python objects"""
-
     def wrapper(*args, **kwargs):
-        return a2py(function(*args, **kwargs))
+        return arules2py(function(*args, **kwargs))
     return wrapper
 
 
 ### arules interface code 
-
 def parameters(x):
     """define parameters for apriori and eclat"""
-
     return ro.ListVector(x)
 
 
 class ItemMatrix(ro.RS4):
     """Class for arules itemMatrix object"""
     
     @staticmethod
     def from_list(items, itemLabels):
         """convert list of lists into an arules itemMatrix object"""
         items = [ro.StrVector(x) for x in items]
-        return ItemMatrix(R.encode(items, itemLabels))
+        return ItemMatrix(R_arules.encode(items, itemLabels))
 
     def as_df(self):
         """convert to pandas dataframe"""
         if type(self) != ro.vectors.DataFrame:
-            self  = R.DATAFRAME(self)
+            self  = R_arules.DATAFRAME(self)
         with (ro.default_converter + pandas2ri.converter).context():
             pd_df = ro.conversion.get_conversion().rpy2py(self)
         return pd_df
     
     def as_matrix(self):
         """convert to numpy matrix"""
-
         return np.array(ro.r('function(x) as(x, "matrix")')(self))
 
     def as_csc_matrix(self):
         """convert to scipy sparse matrix"""
-
         return ngC_to_csc_matrix(self.slots['data'])
 
     def as_dict(self):
         """convert to dictionary"""
-
         l = ro.r('function(x) as(x, "list")')(self)
         l.names = [*range(0, len(l))]
         return dict(zip(l.names, map(list,list(l))))
       
     def as_list(self):
         """convert to list"""
         return list(self.as_dict().values())  
     
     def as_int_list(self):
         """convert to int list"""
-
         l = ro.r('function(x) LIST(x, decode = FALSE)')(self)
         return [list(x) for x in l]
 
     def __getitem__(self, key):
         # prepare subset selection
         if isinstance(key, slice):
             key = list(range(key.stop)[key])  
@@ -151,63 +145,62 @@
         ret =  r_subset(self, key)
         ret.__class__ = class_type
 
         return ret
     
     def __len__(self):
         """return number of elements in the set"""
-
         return ro.r('function(x) length(x)')(self)[0]
     
     def sort(self, by = "lift", decreasing = True):
         """sort
         
         Args:
             by: the interest measure from the quality slot
             decreasing: sort decreasingly?
         """
         decreasing  = ro.vectors.BoolVector([decreasing])
-        return a2py(ro.r('function(x, by, decreasing) sort(x, by = by, decreasing = decreasing)')(self, by, decreasing))
+        return arules2py(ro.r('function(x, by, decreasing) sort(x, by = by, decreasing = decreasing)')(self, by, decreasing))
 
     def unique(self):
         """return unique elements"""
-        return a2py(ro.r('function(x) unique(x)')(self))
+        return arules2py(ro.r('function(x) unique(x)')(self))
     
     def sample(self, size = 1, replace = False):
         """sample from the set
         
         Args:
             size: number of samples
         """
         replace = ro.vectors.BoolVector([replace])
-        return a2py(ro.r('function(x, size, replace) sample(x, size = size, replace = replace)')(self, size, replace))
+        return arules2py(ro.r('function(x, size, replace) sample(x, size = size, replace = replace)')(self, size, replace))
     
     def items(self):
         """return items"""
         return ItemMatrix(ro.r('function(x) items(x)')(self))
     
     def itemFrequency(self, type = "absolute"):
         """return item frequency
         
         Args:
             type: "absolute" or "relative"
         """
-        return a2py(ro.r('function(x, type) itemFrequency(x, type)')(self, type))
+        return arules2py(ro.r('function(x, type) itemFrequency(x, type)')(self, type))
     
     def itemInfo(self):
         """return item info as dataframe"""
-        return a2py(ro.r('function(x) itemInfo(x)')(self))
+        return arules2py(ro.r('function(x) itemInfo(x)')(self))
     
     def labels(self):
         """returns a list of labels for the sets"""
-        return a2py(ro.r('function(x) labels(x)')(self))
+        return arules2py(ro.r('function(x) labels(x)')(self))
     
     def itemLabels(self):
         """returns a list of labels for the sets"""
-        return a2py(ro.r('function(x) itemLabels(x)')(self))
+        return arules2py(ro.r('function(x) itemLabels(x)')(self))
     
     def is_subset(self, x, proper = False, sparse = True):
         """check if x is a subset of self
         
         Args:
             x: the other set
             proper: proper subset?
@@ -238,47 +231,47 @@
             return np.array(m)     
 
 class Associations(ItemMatrix):
     """Superclass for arules associations (rules/itemsets)"""
 
     def quality(self):
         """return quality measures as dataframe"""
-        return a2py(ro.r('function(x) quality(x)')(self))
+        return arules2py(ro.r('function(x) quality(x)')(self))
 
     def is_closed(self):
         """return closedness as boolean vector"""
-        return a2py(ro.r('function(x) is.closed(x)')(self))
+        return arules2py(ro.r('function(x) is.closed(x)')(self))
     
     def is_maximal(self):
         """return maximality as boolean vector"""
-        return a2py(ro.r('function(x) is.maximal(x)')(self))
+        return arules2py(ro.r('function(x) is.maximal(x)')(self))
     
     def is_generator(self):
         """return generator as boolean vector"""
-        return a2py(ro.r('function(x) is.generator(x)')(self))
+        return arules2py(ro.r('function(x) is.generator(x)')(self))
     
     def is_redundant(self):
         """return redundent rules as boolean vector"""
-        return a2py(ro.r('function(x) is.redundant(x)')(self))
+        return arules2py(ro.r('function(x) is.redundant(x)')(self))
     
     def is_significant(self):
         """return significant rules as boolean vector"""
-        return a2py(ro.r('function(x) is.significant(x)')(self))
+        return arules2py(ro.r('function(x) is.significant(x)')(self))
     
     def interestMeasure(self, measure = ["support", "confidence", "lift"], 
                         transactions = None):
         """calculate additional interest measures
         
         Args:
             measure: a list of interest measures (see: https://mhahsler.github.io/arules/docs/measures)
             transactions: the transactions to use (optional)
         """
         if transactions == None:
             transactions = ro.r('NULL')
-        return a2py(ro.r('function(x, measure, transactions) interestMeasure(x, measure, transactions)')
+        return arules2py(ro.r('function(x, measure, transactions) interestMeasure(x, measure, transactions)')
                     (self, measure, transactions))
 
     def addQuality(self, df):
         """add quality measures to the associations.
         
         Args:
             df: a pandas dataframe with the same number of rows as the associations
@@ -313,17 +306,17 @@
 class Itemsets(Associations):
     """Class for arules itemsets object"""
     
     @staticmethod
     def new(items, quality = None):
 
         if quality == None:
-            return a2py(methods.new("itemsets", items))
+            return arules2py(methods.new("itemsets", items))
         else:
-            return a2py(methods.new("itemsets", items, quality))
+            return arules2py(methods.new("itemsets", items, quality))
     
     def items(self):
         """return items as an itemMatrix"""
         return ItemMatrix(ro.r('function(x) lhs(x)')(self))
 
 
 class Transactions(ItemMatrix):
@@ -337,26 +330,27 @@
     def from_df(x, itemLabels = None):
         """convert pandas dataframe into an arules transactions object"""
     
         with (ro.default_converter + ro.pandas2ri.converter).context():
             x_r = ro.conversion.get_conversion().py2rpy(x)
     
         if itemLabels == None:
-            return Transactions(R.transactions(x_r))
+            return Transactions(R_arules.transactions(x_r))
         else:
-            return Transactions(R.transactions(x_r, itemLabels))
+            return Transactions(R_arules.transactions(x_r, itemLabels))
 
 
 # package functions
-discretizeDF = a2py_decor(R.discretizeDF)
-discretizeDF.__doc__ = R.discretizeDF.__doc__   
+discretizeDF = arules2py_decor(R_arules.discretizeDF)
+discretizeDF.__doc__ = R_arules.discretizeDF.__doc__   
 
+apriori = arules2py_decor(R_arules.apriori)
+apriori.__doc__ = R_arules.apriori.__doc__
 
-apriori = a2py_decor(R.apriori)
-apriori.__doc__ = R.apriori.__doc__
-
-eclat = a2py_decor(R.eclat)
-eclat.__doc__ = R.eclat.__doc__
+eclat = arules2py_decor(R_arules.eclat)
+eclat.__doc__ = R_arules.eclat.__doc__
 
 def concat(list):
+    """Combining Association and Transaction Objects"""
+    
     conc = methods.selectMethod("c", tuple(list[0].rclass)[0])
-    return a2py(conc(*list))
+    return arules2py(conc(*list))
```

### Comparing `arulespy-0.1.2/src/arulespy.egg-info/PKG-INFO` & `arulespy-0.1.3/src/arulespy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arulespy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface to the R package arules
 Home-page: https://github.com/mhahsler/arulespy
 Author: Michael Hahsler
 Author-email: mhahsler@lyle.smu.edu
 Project-URL: Documentation, https://github.com/mhahsler/arulespy
 Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
 Project-URL: Source Code, https://github.com/mhahsler/arulespy
```

### Comparing `arulespy-0.1.2/tests/test_arules.py` & `arulespy-0.1.3/tests/test_arules.py`

 * *Files identical despite different names*

