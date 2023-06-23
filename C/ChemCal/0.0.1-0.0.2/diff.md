# Comparing `tmp/ChemCal-0.0.1.tar.gz` & `tmp/ChemCal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChemCal-0.0.1.tar", last modified: Wed Jun 21 23:54:27 2023, max compression
+gzip compressed data, was "ChemCal-0.0.2.tar", last modified: Fri Jun 23 09:23:34 2023, max compression
```

## Comparing `ChemCal-0.0.1.tar` & `ChemCal-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-21 23:54:27.381021 ChemCal-0.0.1/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-21 23:54:27.381021 ChemCal-0.0.1/ChemCal/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-21 23:53:50.000000 ChemCal-0.0.1/ChemCal/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2571 2023-06-21 23:53:50.000000 ChemCal-0.0.1/ChemCal/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1983 2023-06-21 23:53:50.000000 ChemCal-0.0.1/ChemCal/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-21 23:54:27.381021 ChemCal-0.0.1/ChemCal.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1116 2023-06-21 23:54:27.000000 ChemCal-0.0.1/ChemCal.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      324 2023-06-21 23:54:27.000000 ChemCal-0.0.1/ChemCal.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-21 23:54:27.000000 ChemCal-0.0.1/ChemCal.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       36 2023-06-21 23:54:27.000000 ChemCal-0.0.1/ChemCal.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-21 23:54:27.000000 ChemCal-0.0.1/ChemCal.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-21 23:54:27.000000 ChemCal-0.0.1/ChemCal.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        8 2023-06-21 23:54:27.000000 ChemCal-0.0.1/ChemCal.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-21 23:43:34.000000 ChemCal-0.0.1/LICENSE
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 ChemCal-0.0.1/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1116 2023-06-21 23:54:27.381021 ChemCal-0.0.1/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      284 2023-06-21 23:43:59.000000 ChemCal-0.0.1/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1054 2023-06-21 23:52:46.000000 ChemCal-0.0.1/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-21 23:54:27.381021 ChemCal-0.0.1/setup.cfg
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 ChemCal-0.0.1/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-23 09:23:34.314898 ChemCal-0.0.2/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-23 09:23:34.314898 ChemCal-0.0.2/ChemCal/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-23 09:23:31.000000 ChemCal-0.0.2/ChemCal/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2841 2023-06-23 09:23:31.000000 ChemCal-0.0.2/ChemCal/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3210 2023-06-23 09:23:31.000000 ChemCal-0.0.2/ChemCal/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-23 09:23:34.314898 ChemCal-0.0.2/ChemCal.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     6809 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      324 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       36 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-21 23:54:27.000000 ChemCal-0.0.2/ChemCal.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        8 2023-06-23 09:23:34.000000 ChemCal-0.0.2/ChemCal.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-21 23:43:34.000000 ChemCal-0.0.2/LICENSE
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 ChemCal-0.0.2/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     6809 2023-06-23 09:23:34.314898 ChemCal-0.0.2/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     5977 2023-06-23 09:14:10.000000 ChemCal-0.0.2/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      933 2023-06-23 09:23:31.000000 ChemCal-0.0.2/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-23 09:23:34.314898 ChemCal-0.0.2/setup.cfg
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 ChemCal-0.0.2/setup.py
```

### Comparing `ChemCal-0.0.1/ChemCal/_modidx.py` & `ChemCal-0.0.2/ChemCal/_modidx.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
                 'doc_host': 'https://Rhys-McAlister.github.io',
                 'git_url': 'https://github.com/Rhys-McAlister/ChemCal',
                 'lib_path': 'ChemCal'},
   'syms': { 'ChemCal.core': { 'ChemCal.core.CalibrationModel': ('core.html#calibrationmodel', 'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.__init__': ('core.html#calibrationmodel.__init__', 'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_fitted_values': ( 'core.html#calibrationmodel.calculate_fitted_values',
                                                                                          'ChemCal/core.py'),
+                              'ChemCal.core.CalibrationModel.calculate_hibbert_uncertainty': ( 'core.html#calibrationmodel.calculate_hibbert_uncertainty',
+                                                                                               'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_sse': ( 'core.html#calibrationmodel.calculate_sse',
                                                                                'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_sxhat': ( 'core.html#calibrationmodel.calculate_sxhat',
                                                                                  'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_syx': ( 'core.html#calibrationmodel.calculate_syx',
                                                                                'ChemCal/core.py'),
                               'ChemCal.core.CalibrationModel.calculate_uncertainty': ( 'core.html#calibrationmodel.calculate_uncertainty',
```

### Comparing `ChemCal-0.0.1/ChemCal/core.py` & `ChemCal-0.0.2/ChemCal/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,93 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['CalibrationModel']
 
-# %% ../nbs/00_core.ipynb 5
+# %% ../nbs/00_core.ipynb 3
+import pandas as pd
+import scipy as sp
+import matplotlib.pyplot as plt
+import numpy as np
+import seaborn as sns
+from dataclasses import dataclass
+import typing
+
+# %% ../nbs/00_core.ipynb 6
 class CalibrationModel:
 
     def __init__(self, x, y, test_replicates):
       
         self.x = x
         self.y = y
         self.slope = None
         self.intercept = None
         self.r_squared = None
         self.std_err = None
         self.test_replicates = test_replicates
         self.cal_line_points = self.x.shape[0]
         self.df_resid = self.cal_line_points - 2
+        self.sr = None
+        self.mean_replicate_observations = None
+        self.average_response_cal_line = None
 
     def fit_ols(self):
 
         self.slope, self.intercept, self.r_squared, self.std_err, _ = sp.stats.linregress(self.x, self.y)
     
     def calculate_fitted_values(self):
         
         self.fitted_values = self.slope * self.x + self.intercept
 
-   
-    def inverse_prediction(self, unknown):
-
-        if len(unknown) > 1:
-            y = np.mean(unknown)
-        else:
-            y = unknown[0]
-       
-        return (y - self.intercept)/self.slope
     
     def calculate_sse(self):
         self.calculate_fitted_values()
         return np.sum((self.fitted_values - self.y) **2)
     
     def calculate_syx(self):
         return np.sqrt((self.calculate_sse())/(len(self.x)-2))
 
     def get_t_value(self,alpha):
         return sp.stats.t.ppf(1 - alpha/2, self.df_resid)
 
     def calculate_uncertainty(self):
         return self.calculate_sxhat() * self.get_t_value(0.05)
     
+
+    
+    def calculate_hibbert_uncertainty(self, sr, test_repeats, y0, average_response_cal_line, sumsquares):
+        return (1/self.slope) * np.sqrt(((sr**2)/test_repeats) + ((self.calculate_syx()**2)/self.cal_line_points) + 
+                                                                   (((self.calculate_syx()**2)*((y0-average_response_cal_line)**2))/((self.slope**2)*(sumsquares))))
+
+    
     def calculate_sxhat(self):
         return (self.calculate_syx() / self.slope) * np.sqrt( 1/ self.test_replicates + 1 / self.cal_line_points) 
     
     def fit_model(self):
         self.fit_ols()
         self.calculate_uncertainty()
         self.tabulate_results()
 
+    def inverse_prediction(self, unknown):
+
+        if len(unknown) > 1:
+            y0 = np.mean(unknown)
+            sr = np.std(unknown)
+            test_repeats = len(unknown)
+            average_response_cal_line = np.mean(self.y)
+            sumsquares = np.sum((self.x - self.x.mean())**2)
+
+            pred =  (y0 - self.intercept)/self.slope
+        
+            return f"{pred} ± {self.calculate_hibbert_uncertainty(sr=sr, y0=y0, test_repeats=test_repeats, average_response_cal_line=average_response_cal_line, sumsquares=sumsquares) * self.get_t_value(0.05)}"
+        else:
+            y = unknown[0]
+            pred = (y - self.intercept)/self.slope
+            return f"{pred} ± {self.calculate_uncertainty()}"
+
     def tabulate_results(self):
         print(f"Calibration curve")
         print(f"R2 = {self.r_squared}")
         print(f"Slope = {self.slope}")
         print(f"Intercept = {self.intercept}")
         print(f"Uncertainity = {self.calculate_uncertainty()}")
         # print(f"Prediction = {self.inverse_prediction()}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ChemCal-0.0.1/LICENSE` & `ChemCal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ChemCal-0.0.1/setup.py` & `ChemCal-0.0.2/setup.py`

 * *Files identical despite different names*

