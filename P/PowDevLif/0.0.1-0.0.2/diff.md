# Comparing `tmp/PowDevLif-0.0.1.tar.gz` & `tmp/PowDevLif-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDevLif-0.0.1.tar", last modified: Fri Jun 23 10:38:52 2023, max compression
+gzip compressed data, was "PowDevLif-0.0.2.tar", last modified: Fri Jun 23 10:54:43 2023, max compression
```

## Comparing `PowDevLif-0.0.1.tar` & `PowDevLif-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:38:52.270673 PowDevLif-0.0.1/
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 10:38:52.266673 PowDevLif-0.0.1/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.1/README.md
--rw-------   0 runner    (1000) runner    (1000)      451 2023-06-23 10:38:20.000000 PowDevLif-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 10:38:52.270673 PowDevLif-0.0.1/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)     1072 2023-06-23 10:38:12.000000 PowDevLif-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:38:52.262673 PowDevLif-0.0.1/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:38:52.262673 PowDevLif-0.0.1/src/PowDevLif.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 10:38:52.000000 PowDevLif-0.0.1/src/PowDevLif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-06-23 10:38:52.000000 PowDevLif-0.0.1/src/PowDevLif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 10:38:52.000000 PowDevLif-0.0.1/src/PowDevLif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-06-23 10:38:52.000000 PowDevLif-0.0.1/src/PowDevLif.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-23 10:38:52.000000 PowDevLif-0.0.1/src/PowDevLif.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:38:52.262673 PowDevLif-0.0.1/src/powdevlif/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:38:52.266673 PowDevLif-0.0.1/src/powdevlif/function/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/counters.py
--rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/cumul_endommagement.py
--rw-------   0 runner    (1000) runner    (1000)     3279 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/graphs.py
--rw-------   0 runner    (1000) runner    (1000)     3175 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/losses.py
--rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/materials.py
--rw-------   0 runner    (1000) runner    (1000)     2782 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/matrix.py
--rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/path_reader.py
--rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/poly_somme.py
--rw-------   0 runner    (1000) runner    (1000)     2077 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/temperature.py
--rw-------   0 runner    (1000) runner    (1000)     3782 2023-06-23 10:35:27.000000 PowDevLif-0.0.1/src/powdevlif/function/zth_materials.py
--rw-------   0 runner    (1000) runner    (1000)     3245 2023-06-23 10:37:14.000000 PowDevLif-0.0.1/src/powdevlif/lifetime.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.2/README.md
+-rw-------   0 runner    (1000) runner    (1000)      451 2023-06-23 10:54:33.000000 PowDevLif-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)     1072 2023-06-23 10:54:30.000000 PowDevLif-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.251475 PowDevLif-0.0.2/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.255475 PowDevLif-0.0.2/src/PowDevLif.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-06-23 10:54:42.000000 PowDevLif-0.0.2/src/PowDevLif.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/src/powdevlif/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 10:54:43.263476 PowDevLif-0.0.2/src/powdevlif/function/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/counters.py
+-rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/cumul_endommagement.py
+-rw-------   0 runner    (1000) runner    (1000)     3275 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/function/graphs.py
+-rw-------   0 runner    (1000) runner    (1000)     3175 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/losses.py
+-rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/materials.py
+-rw-------   0 runner    (1000) runner    (1000)     2782 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/matrix.py
+-rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/path_reader.py
+-rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.2/src/powdevlif/function/poly_somme.py
+-rw-------   0 runner    (1000) runner    (1000)     2073 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/function/temperature.py
+-rw-------   0 runner    (1000) runner    (1000)     3774 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/function/zth_materials.py
+-rw-------   0 runner    (1000) runner    (1000)     3221 2023-06-23 10:54:01.000000 PowDevLif-0.0.2/src/powdevlif/lifetime.py
```

### Comparing `PowDevLif-0.0.1/LICENSE` & `PowDevLif-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/PKG-INFO` & `PowDevLif-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.1
+Version: 0.0.2
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.1/README.md` & `PowDevLif-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/setup.py` & `PowDevLif-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='PowDevLif',
-    version='0.0.1',
+    version='0.0.2',
     description ='The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)',
     readme='README.md',
     license='MIT',
     author='Garnier Paul, Baudais Briac',
     author_email='paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages('src'),
```

### Comparing `PowDevLif-0.0.1/src/PowDevLif.egg-info/PKG-INFO` & `PowDevLif-0.0.2/src/PowDevLif.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.1
+Version: 0.0.2
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.1/src/PowDevLif.egg-info/SOURCES.txt` & `PowDevLif-0.0.2/src/PowDevLif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/counters.py` & `PowDevLif-0.0.2/src/powdevlif/function/counters.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/cumul_endommagement.py` & `PowDevLif-0.0.2/src/powdevlif/function/cumul_endommagement.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/graphs.py` & `PowDevLif-0.0.2/src/powdevlif/function/graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import matplotlib.pyplot as plt
 import numpy as np
-from src.powdevlif.function.matrix import show_matrix
+from powdevlif.function.matrix import show_matrix
 
 def graph(file, dic, losses, temp_IGBT, temp_diode, temp_case, counter_IGBT, counter_diode):
     """
     Generates and displays two graphs based on the given file, losses, and dictionary.
     The first graph shows Torque and Speed as a function of Time.
     The second graph shows Current and Total losses as a function of Time.
```

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/losses.py` & `PowDevLif-0.0.2/src/powdevlif/function/losses.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/matrix.py` & `PowDevLif-0.0.2/src/powdevlif/function/matrix.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/poly_somme.py` & `PowDevLif-0.0.2/src/powdevlif/function/poly_somme.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/temperature.py` & `PowDevLif-0.0.2/src/powdevlif/function/temperature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from scipy import signal
-from src.powdevlif.function.zth_materials import ZthMaterials
+from powdevlif.function.zth_materials import ZthMaterials
 
 def calculate_temperature( losses, dic, file):
     """
     Function to calculate the temperature of IGBT and Diode.
 
     Parameters:
     losses (object): Object containing the loss data.
```

### Comparing `PowDevLif-0.0.1/src/powdevlif/function/zth_materials.py` & `PowDevLif-0.0.2/src/powdevlif/function/zth_materials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from numpy import convolve
-from src.powdevlif.function.materials import Materials
-from src.powdevlif.function.poly_somme import poly_somme
+from powdevlif.function.materials import Materials
+from powdevlif.function.poly_somme import poly_somme
 
 class ZthMaterials:
   """
   Class representing the thermal impedance of materials for IGBT and diode. It uses Foster's model.
   """
 
   def __init__(self, dic):
```

### Comparing `PowDevLif-0.0.1/src/powdevlif/lifetime.py` & `PowDevLif-0.0.2/src/powdevlif/lifetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 # Importing required modules from the local directories
-from src.powdevlif.function.counters import count
-from src.powdevlif.function.cumul_endommagement import calculate_damage_cumulation
-from src.powdevlif.function.losses import Losses
-from src.powdevlif.function.temperature import calculate_temperature
-from src.powdevlif.function.graphs import graph
-from src.powdevlif.function.path_reader import import_variables
+from powdevlif.function.counters import count
+from powdevlif.function.cumul_endommagement import calculate_damage_cumulation
+from powdevlif.function.losses import Losses
+from powdevlif.function.temperature import calculate_temperature
+from powdevlif.function.graphs import graph
+from powdevlif.function.path_reader import import_variables
 
 def pdl_calculation(variables_file_path):
   """
   This function executes a sequence of calculations related to thermal 
   and electrical properties of some materials, based on data from an Excel file.
   """
   # Choice of dictionary for the analysis. This could be modified in the future for flexibility.
```

