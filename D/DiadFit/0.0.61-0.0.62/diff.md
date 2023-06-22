# Comparing `tmp/DiadFit-0.0.61.tar.gz` & `tmp/DiadFit-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DiadFit-0.0.61.tar", last modified: Thu Jun 22 21:15:53 2023, max compression
+gzip compressed data, was "DiadFit-0.0.62.tar", last modified: Thu Jun 22 23:18:12 2023, max compression
```

## Comparing `DiadFit-0.0.61.tar` & `DiadFit-0.0.62.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.316125 DiadFit-0.0.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 21:15:53.316125 DiadFit-0.0.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 21:15:34.000000 DiadFit-0.0.61/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:15:53.316125 DiadFit-0.0.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-22 21:15:37.000000 DiadFit-0.0.61/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.312125 DiadFit-0.0.61/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.316125 DiadFit-0.0.61/src/DiadFit/
--rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/CO2_EOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/CO2_in_bubble_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/H2O_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Highrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Lowrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Mediumrho_polyfit_data.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/Psensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/argon_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/cosmicray_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/densimeter_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/densimeters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/density_depth_crustal_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)   162634 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/diads.py
--rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/error_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35199 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/importing_data_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    63944 2023-06-22 21:15:37.000000 DiadFit-0.0.61/src/DiadFit/ne_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:15:53.316125 DiadFit-0.0.61/src/DiadFit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-22 21:15:53.000000 DiadFit-0.0.61/src/DiadFit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 21:15:52.000000 DiadFit-0.0.61/src/DiadFit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:18:12.788352 DiadFit-0.0.62/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 23:18:12.788352 DiadFit-0.0.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 23:17:58.000000 DiadFit-0.0.62/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:18:12.788352 DiadFit-0.0.62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-22 23:18:01.000000 DiadFit-0.0.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:18:12.784352 DiadFit-0.0.62/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:18:12.788352 DiadFit-0.0.62/src/DiadFit/
+-rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/CO2_EOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/CO2_in_bubble_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43406 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/H2O_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/Highrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/Lowrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/Mediumrho_polyfit_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/Psensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/argon_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/cosmicray_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/densimeter_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/densimeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/density_depth_crustal_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162634 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/diads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32657 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/error_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35199 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/importing_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63944 2023-06-22 23:18:01.000000 DiadFit-0.0.62/src/DiadFit/ne_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:18:12.788352 DiadFit-0.0.62/src/DiadFit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 23:18:12.000000 DiadFit-0.0.62/src/DiadFit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-22 23:18:12.000000 DiadFit-0.0.62/src/DiadFit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:18:12.000000 DiadFit-0.0.62/src/DiadFit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 23:18:12.000000 DiadFit-0.0.62/src/DiadFit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 23:18:12.000000 DiadFit-0.0.62/src/DiadFit.egg-info/top_level.txt
```

### Comparing `DiadFit-0.0.61/PKG-INFO` & `DiadFit-0.0.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.61
+Version: 0.0.62
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.61/README.md` & `DiadFit-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/setup.py` & `DiadFit-0.0.62/setup.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/CO2_EOS.py` & `DiadFit-0.0.62/src/DiadFit/CO2_EOS.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/CO2_in_bubble_error.py` & `DiadFit-0.0.62/src/DiadFit/CO2_in_bubble_error.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/H2O_fitting.py` & `DiadFit-0.0.62/src/DiadFit/H2O_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/Highrho_polyfit_data.pkl` & `DiadFit-0.0.62/src/DiadFit/Highrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/Lowrho_polyfit_data.pkl` & `DiadFit-0.0.62/src/DiadFit/Lowrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/Mediumrho_polyfit_data.pkl` & `DiadFit-0.0.62/src/DiadFit/Mediumrho_polyfit_data.pkl`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/Psensor.py` & `DiadFit-0.0.62/src/DiadFit/Psensor.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/__init__.py` & `DiadFit-0.0.62/src/DiadFit/__init__.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/argon_lines.py` & `DiadFit-0.0.62/src/DiadFit/argon_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/cosmicray_filter.py` & `DiadFit-0.0.62/src/DiadFit/cosmicray_filter.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/densimeter_fitting.py` & `DiadFit-0.0.62/src/DiadFit/densimeter_fitting.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/densimeters.py` & `DiadFit-0.0.62/src/DiadFit/densimeters.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from lmfit.models import GaussianModel, VoigtModel, LinearModel, ConstantModel
 from scipy.signal import find_peaks
 import os
 import re
 from os import listdir
 from os.path import isfile, join
 import pickle
+from pathlib import Path
 encode="ISO-8859-1"
 
 ## Cornell densimeters
 def calculate_density_cornell(*, temp='SupCrit', Split, split_err=None):
     """ This function converts Diad Splitting into CO$_2$ density using the densimeters of DeVitre et al. (2021)
     This should only be used for the Cornell Raman, not other Ramans at present
 
@@ -221,26 +222,28 @@
 
 
 
 
     """
 
     # #if temp is "RoomT":
+    DiadFit_dir=Path(__file__).parent
+
     LowD_RT=-38.34631 + 0.3732578*Split
     HighD_RT=-41.64784 + 0.4058777*Split- 0.1460339*(Split-104.653)**2
 
     # IF temp is 37
     pickle_str='Lowrho_polyfit_data.pkl'
-    with open(pickle_str, 'rb') as f:
+    with open(DiadFit_dir/pickle_str, 'rb') as f:
         lowrho_pickle_data = pickle.load(f)
     pickle_str='Mediumrho_polyfit_data.pkl'
-    with open(pickle_str, 'rb') as f:
+    with open(DiadFit_dir/pickle_str, 'rb') as f:
         medrho_pickle_data = pickle.load(f)
     pickle_str='Highrho_polyfit_data.pkl'
-    with open(pickle_str, 'rb') as f:
+    with open(DiadFit_dir/pickle_str, 'rb') as f:
         highrho_pickle_data = pickle.load(f)
 
     lowrho_model = lowrho_pickle_data['model']
     medrho_model = medrho_pickle_data['model']
     highrho_model = highrho_pickle_data['model']
 
     LowD_SC = pd.Series(lowrho_model(Split), index=Split.index)
```

### Comparing `DiadFit-0.0.61/src/DiadFit/density_depth_crustal_profiles.py` & `DiadFit-0.0.62/src/DiadFit/density_depth_crustal_profiles.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/diads.py` & `DiadFit-0.0.62/src/DiadFit/diads.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/error_propagation.py` & `DiadFit-0.0.62/src/DiadFit/error_propagation.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/importing_data_files.py` & `DiadFit-0.0.62/src/DiadFit/importing_data_files.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit/ne_lines.py` & `DiadFit-0.0.62/src/DiadFit/ne_lines.py`

 * *Files identical despite different names*

### Comparing `DiadFit-0.0.61/src/DiadFit.egg-info/PKG-INFO` & `DiadFit-0.0.62/src/DiadFit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiadFit
-Version: 0.0.61
+Version: 0.0.62
 Summary: DiadFit
 Home-page: https://github.com/PennyWieser/DiadFit
 Author: Penny Wieser
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/DiadFit)](https://pypi.org/project/DiadFit/)
         [![Build Status](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/DiadFit/actions/workflows/main.yml)
```

### Comparing `DiadFit-0.0.61/src/DiadFit.egg-info/SOURCES.txt` & `DiadFit-0.0.62/src/DiadFit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

