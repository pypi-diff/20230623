# Comparing `tmp/DielModels-0.0.2.tar.gz` & `tmp/DielModels-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DielModels-0.0.2.tar", last modified: Fri Jun 23 09:19:08 2023, max compression
+gzip compressed data, was "dist\DielModels-1.0.1.tar", last modified: Fri Jun 23 10:24:06 2023, max compression
```

## Comparing `DielModels-0.0.2.tar` & `DielModels-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:19:08.539607 DielModels-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-03-20 16:26:03.000000 DielModels-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      767 2023-06-23 09:19:08.539607 DielModels-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-23 09:17:06.000000 DielModels-0.0.2/README.md
--rw-rw-rw-   0        0        0      556 2023-03-20 16:26:03.000000 DielModels-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      919 2023-06-23 09:19:08.541336 DielModels-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-03-20 16:26:03.000000 DielModels-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:19:08.427812 DielModels-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 09:19:08.470031 DielModels-0.0.2/src/DielModels.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-23 09:19:08.000000 DielModels-0.0.2/src/DielModels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-06-23 09:19:08.000000 DielModels-0.0.2/src/DielModels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:19:08.000000 DielModels-0.0.2/src/DielModels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 09:19:08.000000 DielModels-0.0.2/src/DielModels.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      100 2023-06-23 09:19:08.000000 DielModels-0.0.2/src/DielModels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-23 09:19:08.000000 DielModels-0.0.2/src/DielModels.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 09:19:08.527750 DielModels-0.0.2/src/diel_models/
--rw-rw-rw-   0        0        0        0 2023-03-20 16:26:03.000000 DielModels-0.0.2/src/diel_models/__init__.py
--rw-rw-rw-   0        0        0     2572 2023-06-22 12:47:14.000000 DielModels-0.0.2/src/diel_models/biomass_adjuster.py
--rw-rw-rw-   0        0        0     3954 2023-06-22 12:47:14.000000 DielModels-0.0.2/src/diel_models/day_night_creator.py
--rw-rw-rw-   0        0        0     2125 2023-06-22 12:47:14.000000 DielModels-0.0.2/src/diel_models/diel_models_creator.py
--rw-rw-rw-   0        0        0     2096 2023-06-22 12:47:14.000000 DielModels-0.0.2/src/diel_models/nitrate_uptake_ratio.py
--rw-rw-rw-   0        0        0     2245 2023-06-22 12:47:14.000000 DielModels-0.0.2/src/diel_models/photon_reaction_inhibitor.py
--rw-rw-rw-   0        0        0      952 2023-06-22 12:47:14.000000 DielModels-0.0.2/src/diel_models/pipeline.py
--rw-rw-rw-   0        0        0     7077 2023-06-22 12:47:14.000000 DielModels-0.0.2/src/diel_models/storage_pool_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.326083 DielModels-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-03-20 16:26:03.000000 DielModels-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      647 2023-06-23 10:24:06.326083 DielModels-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2023-06-23 10:22:45.000000 DielModels-1.0.1/README.md
+-rw-rw-rw-   0        0        0      556 2023-03-20 16:26:03.000000 DielModels-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      919 2023-06-23 10:24:06.328302 DielModels-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-03-20 16:26:03.000000 DielModels-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.199869 DielModels-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.251439 DielModels-1.0.1/src/DielModels.egg-info/
+-rw-rw-rw-   0        0        0      647 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 09:19:08.000000 DielModels-1.0.1/src/DielModels.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-23 10:24:05.000000 DielModels-1.0.1/src/DielModels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 10:24:06.315524 DielModels-1.0.1/src/diel_models/
+-rw-rw-rw-   0        0        0        0 2023-03-20 16:26:03.000000 DielModels-1.0.1/src/diel_models/__init__.py
+-rw-rw-rw-   0        0        0     2572 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/biomass_adjuster.py
+-rw-rw-rw-   0        0        0     3954 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/day_night_creator.py
+-rw-rw-rw-   0        0        0     2125 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/diel_models_creator.py
+-rw-rw-rw-   0        0        0     2096 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/nitrate_uptake_ratio.py
+-rw-rw-rw-   0        0        0     2245 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/photon_reaction_inhibitor.py
+-rw-rw-rw-   0        0        0      952 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/pipeline.py
+-rw-rw-rw-   0        0        0     7077 2023-06-22 12:47:14.000000 DielModels-1.0.1/src/diel_models/storage_pool_generator.py
```

### Comparing `DielModels-0.0.2/LICENSE` & `DielModels-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/PKG-INFO` & `DielModels-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DielModels
-Version: 0.0.2
+Version: 1.0.1
 Summary: DielModels:
 Author: Luciana Martins and João Capela
 License: MIT
 Keywords: plants,diel models
 Platform: unix
 Platform: linux
 Platform: osx
@@ -18,18 +18,13 @@
 Provides-Extra: testing
 License-File: LICENSE
 
 # DielModels
 
 ### Package diel_models
 
-``` pip install DielModels==0.0.1 ```
+``` pip install DielModels==1.0.1 ```
 
 ``` import diel_models```
 
-For more information read __index.html__ documentation file.
-
-https://github.com/LucianaMartins26/DielModels.git
-
-
```

### Comparing `DielModels-0.0.2/pyproject.toml` & `DielModels-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/setup.cfg` & `DielModels-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 6965 6c4d 6f64 656c 730d 0a76   = DielModels..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
+00000020: 6572 7369 6f6e 203d 2031 2e30 2e31 0d0a  ersion = 1.0.1..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 4469  description = Di
 00000040: 656c 4d6f 6465 6c73 3a0d 0a6c 6f6e 675f  elModels:..long_
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000060: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6b  le: README.md..k
 00000070: 6579 776f 7264 7320 3d20 706c 616e 7473  eywords = plants
 00000080: 2c20 6469 656c 206d 6f64 656c 730d 0a61  , diel models..a
 00000090: 7574 686f 7220 3d20 4c75 6369 616e 6120  uthor = Luciana
```

### Comparing `DielModels-0.0.2/src/DielModels.egg-info/PKG-INFO` & `DielModels-1.0.1/src/DielModels.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DielModels
-Version: 0.0.2
+Version: 1.0.1
 Summary: DielModels:
 Author: Luciana Martins and João Capela
 License: MIT
 Keywords: plants,diel models
 Platform: unix
 Platform: linux
 Platform: osx
@@ -18,18 +18,13 @@
 Provides-Extra: testing
 License-File: LICENSE
 
 # DielModels
 
 ### Package diel_models
 
-``` pip install DielModels==0.0.1 ```
+``` pip install DielModels==1.0.1 ```
 
 ``` import diel_models```
 
-For more information read __index.html__ documentation file.
-
-https://github.com/LucianaMartins26/DielModels.git
-
-
```

### Comparing `DielModels-0.0.2/src/DielModels.egg-info/SOURCES.txt` & `DielModels-1.0.1/src/DielModels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/src/diel_models/biomass_adjuster.py` & `DielModels-1.0.1/src/diel_models/biomass_adjuster.py`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/src/diel_models/day_night_creator.py` & `DielModels-1.0.1/src/diel_models/day_night_creator.py`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/src/diel_models/diel_models_creator.py` & `DielModels-1.0.1/src/diel_models/diel_models_creator.py`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/src/diel_models/nitrate_uptake_ratio.py` & `DielModels-1.0.1/src/diel_models/nitrate_uptake_ratio.py`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/src/diel_models/photon_reaction_inhibitor.py` & `DielModels-1.0.1/src/diel_models/photon_reaction_inhibitor.py`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/src/diel_models/pipeline.py` & `DielModels-1.0.1/src/diel_models/pipeline.py`

 * *Files identical despite different names*

### Comparing `DielModels-0.0.2/src/diel_models/storage_pool_generator.py` & `DielModels-1.0.1/src/diel_models/storage_pool_generator.py`

 * *Files identical despite different names*

