# Comparing `tmp/HanLabTools-0.2.2.tar.gz` & `tmp/HanLabTools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HanLabTools-0.2.2.tar", last modified: Fri Jun 16 20:34:56 2023, max compression
+gzip compressed data, was "HanLabTools-0.2.3.tar", last modified: Fri Jun 23 13:07:17 2023, max compression
```

## Comparing `HanLabTools-0.2.2.tar` & `HanLabTools-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.517973 HanLabTools-0.2.2/HanLabTools/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/HanLabTools/config/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/config/HanLab.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/HanLabTools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:34:56.517973 HanLabTools-0.2.2/HanLabTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 20:34:56.000000 HanLabTools-0.2.2/HanLabTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:34:56.521973 HanLabTools-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-16 20:34:47.000000 HanLabTools-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:07:17.667009 HanLabTools-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:07:17.663009 HanLabTools-0.2.3/HanLabTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:07:17.667009 HanLabTools-0.2.3/HanLabTools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/config/HanLab.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/HanLabTools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:07:17.667009 HanLabTools-0.2.3/HanLabTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-23 13:07:17.000000 HanLabTools-0.2.3/HanLabTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-23 13:07:17.000000 HanLabTools-0.2.3/HanLabTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:07:17.000000 HanLabTools-0.2.3/HanLabTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 13:07:17.000000 HanLabTools-0.2.3/HanLabTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 13:07:17.000000 HanLabTools-0.2.3/HanLabTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-23 13:07:17.667009 HanLabTools-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:07:17.667009 HanLabTools-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-23 13:07:08.000000 HanLabTools-0.2.3/setup.py
```

### Comparing `HanLabTools-0.2.2/HanLabTools/config/HanLab.cfg` & `HanLabTools-0.2.3/HanLabTools/config/HanLab.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -34,7 +34,11 @@
 data_format = topspin
 dim1 = B0
 
 [ODNP_CNSI]
 
 [ODNP_HanLab]
 
+[SC_Plot_Parameters]
+xaxis_scaling_factor = 2
+bar_width = 0.25
+
```

### Comparing `HanLabTools-0.2.2/HanLabTools/config/config.py` & `HanLabTools-0.2.3/HanLabTools/config/config.py`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.2/HanLabTools/io.py` & `HanLabTools-0.2.3/HanLabTools/io.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,82 +8,87 @@
 """
 
 import numpy as _np
 import dnplab as _dnp
 from .config.config import HanLab_CONFIG
 
 
-def import_data(path, data_type, start_stop=None, spacing="lin", verbose=False):
+def import_data(path, experiment_type, start_stop=None, spacing="lin", verbose=False):
     """
     Import Han Lab specific experiments
 
     Args:
         path (str, list):                   Path to data directory or list of directories
-        data_type (str):                    Data/experiment type (see list below)
+        experimnet=nt_type (str)            Experiment type (see list below)
         start_stop (tuple or vector):       Coords for new dimension
         spacing (str):                      "lin" for linear spaced axis or "log" for logarithmically spaced axis
         verbose (boolean):                  For debugging, get more specific information what the module is doing
 
     Returns:
         data (DNPData):                     Data object
 
-    Currently implemented experiments:
+    Currently implemented experiment types:
 
         **DNPProfile_F:**                   DNP enhancement versus microwave frequency. Data is recorded in TopSpin. Experiment is controlled through SpecMan
         **DNPEnhancementBuildUp:**          DNP enhancement (NMR) versus contact time t<sub>c</sub>. Data is recorded using TopSpin.
         **ELDOR:**                          EPR pump probe experiment. The data is recorded using SpecMan.
         **DNPPowerBuildUp:**                DNP enhancement at a fixed microwave frequency versus microwave power. Data is recorded in TopSpin. The experiment is controlled through SpecMan.
         **EPRT1e:**                         EPR inversion-recovery experiments. Data is recorded in SpecMan.
         **EPRT2e:**                         EPR two-pulse echo decay. Data is recorded in SpecMan.
 
     """
 
-    if data_type in dict.keys(HanLab_CONFIG):
+    if experiment_type in dict.keys(HanLab_CONFIG):
         if verbose == True:
             print("Key exists")
-            print(HanLab_CONFIG[data_type])
-            print("")
+            print(HanLab_CONFIG[experiment_type])
 
         # Create sub-dictionary for experiment configuration
-        tempKeys = dict.keys(HanLab_CONFIG[data_type])
+        temp_keys = dict.keys(HanLab_CONFIG[experiment_type])
+
+        if verbose == True:
+            print("temp_keys:", temp_keys)
 
         # Load data
-        if "data_format" in tempKeys:
-            data_format = HanLab_CONFIG[data_type].get("data_format")
+        if "data_format" in temp_keys:
+            data_format = HanLab_CONFIG[experiment_type].get("data_format")
         else:
             data_format = None
 
-        data = _dnp.load(path, data_type=data_format)
+        if verbose == True:
+            print("data_format:", data_format)
+
+        data = _dnp.load(path, data_format=data_format)
 
         if verbose == True:
-            print("Data loaded")
+            print("Done! Data loaded")
 
         # Assign axis. Could probably be more elegant, but this will do for now
-        if "dim0" in tempKeys:
-            temp = HanLab_CONFIG[data_type].get("dim0")
+        if "dim0" in temp_keys:
+            temp = HanLab_CONFIG[experiment_type].get("dim0")
             data.rename("x0", temp)
             data.coords[temp] = data.coords[temp] * 1e-9
 
-        if "dim1" in tempKeys:
-            temp = HanLab_CONFIG[data_type].get("dim1")
+        if "dim1" in temp_keys:
+            temp = HanLab_CONFIG[experiment_type].get("dim1")
             data = _dnp.update_axis(
                 data, dim=1, new_dims=temp, start_stop=start_stop, spacing=spacing
             )
 
         # if "dim2" in tempKeys:
         #     # Not yet implemented
 
         # if "dim3" in tempKeys:
         #     # Not yet implemented
 
-        if HanLab_CONFIG[data_type].get("data_format") == "specman":
+        if HanLab_CONFIG[experiment_type].get("data_format") == "specman":
             if verbose == True:
                 print("Data format is SpecMan")
 
-            if HanLab_CONFIG[data_type].get("make_complex") == "true":
+            if HanLab_CONFIG[experiment_type].get("make_complex") == "true":
                 if verbose == True:
                     print("Create complex array from dimensions [...,0] and [...,1]")
                 data = _dnp.create_complex(
                     data, data.values[..., 0], data.values[..., 1]
                 )
 
     else:
```

### Comparing `HanLabTools-0.2.2/HanLabTools.egg-info/PKG-INFO` & `HanLabTools-0.2.3/HanLabTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabTools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabTools
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `HanLabTools-0.2.2/LICENSE` & `HanLabTools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.2/PKG-INFO` & `HanLabTools-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabTools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabTools
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `HanLabTools-0.2.2/README.md` & `HanLabTools-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.2.2/setup.py` & `HanLabTools-0.2.3/setup.py`

 * *Files identical despite different names*

