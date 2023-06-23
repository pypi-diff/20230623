# Comparing `tmp/pyfairsim-0.0.2.tar.gz` & `tmp/pyfairsim-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfairsim-0.0.2.tar", last modified: Fri Jun 16 12:24:53 2023, max compression
+gzip compressed data, was "pyfairsim-0.0.3.tar", last modified: Fri Jun 23 07:50:54 2023, max compression
```

## Comparing `pyfairsim-0.0.2.tar` & `pyfairsim-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.653102 pyfairsim-0.0.2/
--rw-rw-rw-   0        0        0    18431 2022-01-11 07:39:57.000000 pyfairsim-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1865 2023-06-16 12:24:53.653102 pyfairsim-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1402 2023-06-16 12:21:43.000000 pyfairsim-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.632098 pyfairsim-0.0.2/pyfairsim/
--rw-rw-rw-   0        0        0        0 2023-02-13 08:11:50.000000 pyfairsim-0.0.2/pyfairsim/__init__.py
--rw-rw-rw-   0        0        0     3659 2023-02-13 08:26:15.000000 pyfairsim-0.0.2/pyfairsim/batch_reconstruction.py
--rw-rw-rw-   0        0        0      360 2023-02-13 08:30:03.000000 pyfairsim-0.0.2/pyfairsim/create_example_settings.py
--rw-rw-rw-   0        0        0     2551 2023-02-13 08:30:11.000000 pyfairsim-0.0.2/pyfairsim/parameter_estimation.py
--rw-rw-rw-   0        0        0     2909 2023-02-13 08:30:19.000000 pyfairsim-0.0.2/pyfairsim/phase_estimation.py
--rw-rw-rw-   0        0        0     2333 2023-02-13 08:26:30.000000 pyfairsim-0.0.2/pyfairsim/reconstruction.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.646101 pyfairsim-0.0.2/pyfairsim/sim_algorithm/
--rw-rw-rw-   0        0        0     5136 2023-02-08 12:58:21.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/Direction.py
--rw-rw-rw-   0        0        0     4511 2023-02-13 08:28:59.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/OTF_Provider.py
--rw-rw-rw-   0        0        0    12225 2023-03-03 06:42:44.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Parameters.py
--rw-rw-rw-   0        0        0    37047 2023-06-16 11:51:15.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Utils.py
--rw-rw-rw-   0        0        0     3844 2023-02-13 08:27:43.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/Wiener_Filter.py
--rw-rw-rw-   0        0        0        0 2022-11-29 07:44:10.000000 pyfairsim-0.0.2/pyfairsim/sim_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.650101 pyfairsim-0.0.2/pyfairsim/utils/
--rw-rw-rw-   0        0        0        0 2023-02-08 12:58:35.000000 pyfairsim-0.0.2/pyfairsim/utils/__init__.py
--rw-rw-rw-   0        0        0     3079 2023-02-08 12:58:36.000000 pyfairsim-0.0.2/pyfairsim/utils/argparse.py
--rw-rw-rw-   0        0        0     2698 2023-03-03 05:29:05.000000 pyfairsim-0.0.2/pyfairsim/utils/load_settings.py
--rw-rw-rw-   0        0        0     1869 2023-02-08 12:58:40.000000 pyfairsim-0.0.2/pyfairsim/utils/physics.py
--rw-rw-rw-   0        0        0     5314 2023-03-03 06:49:19.000000 pyfairsim-0.0.2/pyfairsim/utils/tif.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.640100 pyfairsim-0.0.2/pyfairsim.egg-info/
--rw-rw-rw-   0        0        0     1865 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      788 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 12:24:53.000000 pyfairsim-0.0.2/pyfairsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 12:24:53.653102 pyfairsim-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      977 2023-06-16 11:51:16.000000 pyfairsim-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:24:53.652102 pyfairsim-0.0.2/tests/
--rw-rw-rw-   0        0        0     1511 2023-06-16 11:52:04.000000 pyfairsim-0.0.2/tests/test_locate_peak.py
--rw-rw-rw-   0        0        0      121 2023-02-08 12:58:33.000000 pyfairsim-0.0.2/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:50:54.405107 pyfairsim-0.0.3/
+-rw-rw-rw-   0        0        0    18431 2022-01-11 07:39:57.000000 pyfairsim-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2382 2023-06-23 07:50:54.405107 pyfairsim-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2023-06-23 07:49:57.000000 pyfairsim-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 07:50:54.387772 pyfairsim-0.0.3/pyfairsim/
+-rw-rw-rw-   0        0        0        0 2023-02-13 08:11:50.000000 pyfairsim-0.0.3/pyfairsim/__init__.py
+-rw-rw-rw-   0        0        0     3659 2023-02-13 08:26:15.000000 pyfairsim-0.0.3/pyfairsim/batch_reconstruction.py
+-rw-rw-rw-   0        0        0      360 2023-02-13 08:30:03.000000 pyfairsim-0.0.3/pyfairsim/create_example_settings.py
+-rw-rw-rw-   0        0        0     2551 2023-02-13 08:30:11.000000 pyfairsim-0.0.3/pyfairsim/parameter_estimation.py
+-rw-rw-rw-   0        0        0     2909 2023-02-13 08:30:19.000000 pyfairsim-0.0.3/pyfairsim/phase_estimation.py
+-rw-rw-rw-   0        0        0     2333 2023-02-13 08:26:30.000000 pyfairsim-0.0.3/pyfairsim/reconstruction.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:50:54.398105 pyfairsim-0.0.3/pyfairsim/sim_algorithm/
+-rw-rw-rw-   0        0        0     5136 2023-02-08 12:58:21.000000 pyfairsim-0.0.3/pyfairsim/sim_algorithm/Direction.py
+-rw-rw-rw-   0        0        0     4511 2023-02-13 08:28:59.000000 pyfairsim-0.0.3/pyfairsim/sim_algorithm/OTF_Provider.py
+-rw-rw-rw-   0        0        0    12646 2023-06-20 07:18:16.000000 pyfairsim-0.0.3/pyfairsim/sim_algorithm/SIM_Parameters.py
+-rw-rw-rw-   0        0        0    37047 2023-06-16 11:51:15.000000 pyfairsim-0.0.3/pyfairsim/sim_algorithm/SIM_Utils.py
+-rw-rw-rw-   0        0        0     3844 2023-02-13 08:27:43.000000 pyfairsim-0.0.3/pyfairsim/sim_algorithm/Wiener_Filter.py
+-rw-rw-rw-   0        0        0        0 2022-11-29 07:44:10.000000 pyfairsim-0.0.3/pyfairsim/sim_algorithm/__init__.py
+-rw-rw-rw-   0        0        0     5298 2023-06-23 07:39:07.000000 pyfairsim-0.0.3/pyfairsim/tiled_reconstruction.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:50:54.402106 pyfairsim-0.0.3/pyfairsim/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-08 12:58:35.000000 pyfairsim-0.0.3/pyfairsim/utils/__init__.py
+-rw-rw-rw-   0        0        0     3079 2023-02-08 12:58:36.000000 pyfairsim-0.0.3/pyfairsim/utils/argparse.py
+-rw-rw-rw-   0        0        0     2698 2023-03-03 05:29:05.000000 pyfairsim-0.0.3/pyfairsim/utils/load_settings.py
+-rw-rw-rw-   0        0        0     1869 2023-02-08 12:58:40.000000 pyfairsim-0.0.3/pyfairsim/utils/physics.py
+-rw-rw-rw-   0        0        0     8251 2023-06-23 07:37:24.000000 pyfairsim-0.0.3/pyfairsim/utils/tif.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:50:54.392774 pyfairsim-0.0.3/pyfairsim.egg-info/
+-rw-rw-rw-   0        0        0     2382 2023-06-23 07:50:54.000000 pyfairsim-0.0.3/pyfairsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2023-06-23 07:50:54.000000 pyfairsim-0.0.3/pyfairsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:50:54.000000 pyfairsim-0.0.3/pyfairsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-23 07:50:54.000000 pyfairsim-0.0.3/pyfairsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 07:50:54.000000 pyfairsim-0.0.3/pyfairsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:50:54.405107 pyfairsim-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      977 2023-06-23 07:44:28.000000 pyfairsim-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:50:54.404108 pyfairsim-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1511 2023-06-16 11:52:04.000000 pyfairsim-0.0.3/tests/test_locate_peak.py
+-rw-rw-rw-   0        0        0      121 2023-02-08 12:58:33.000000 pyfairsim-0.0.3/tests/tests.py
```

### Comparing `pyfairsim-0.0.2/LICENSE` & `pyfairsim-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/PKG-INFO` & `pyfairsim-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfairsim
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to run sim reconstructions including parameter estimation.
 Home-page: 
 Author: Jakob Wessendorf
 Keywords: sim,reconstruction,parameter estimation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -49,8 +49,14 @@
 
 `python -m pyfairsim.batch_reconstruction`
 
 # run absolute phase estimation
 
 Runs a non-iterative phase estimation based on auto-correlation by Wicker et al. For it to work parameter estimation needs to be executed first.
 
-`python -m pyfairsim.phase_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`  
+`python -m pyfairsim.phase_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`
+
+# run tiled reconstruction
+
+ATTENTION still in development!!! Tile size should be an even number, only supports square images with sizes divisible by the tile size. Overlap of the tiles for now is hard coded to be half of the tile size. Before running this a parameter estimation and phase estimation needs to be run. Tiled reconstruction will use absolute phase estimation for the tiles.
+
+`python -m pyfairsim.tiled_reconstruction -f <path-to-image> -s <path-to-settings> -o <path-to-save-reconstructed-image>`
```

### Comparing `pyfairsim-0.0.2/README.md` & `pyfairsim-0.0.3/pyfairsim.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: pyfairsim
+Version: 0.0.3
+Summary: A package to run sim reconstructions including parameter estimation.
+Home-page: 
+Author: Jakob Wessendorf
+Keywords: sim,reconstruction,parameter estimation
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyFairSIM
 
 python version of the fast sim project
 
 # install
 run:
 
@@ -35,8 +49,14 @@
 
 `python -m pyfairsim.batch_reconstruction`
 
 # run absolute phase estimation
 
 Runs a non-iterative phase estimation based on auto-correlation by Wicker et al. For it to work parameter estimation needs to be executed first.
 
-`python -m pyfairsim.phase_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`  
+`python -m pyfairsim.phase_estimation -f <path-to-image> -s <path-to-settings> -o <path-to-save-settings>`
+
+# run tiled reconstruction
+
+ATTENTION still in development!!! Tile size should be an even number, only supports square images with sizes divisible by the tile size. Overlap of the tiles for now is hard coded to be half of the tile size. Before running this a parameter estimation and phase estimation needs to be run. Tiled reconstruction will use absolute phase estimation for the tiles.
+
+`python -m pyfairsim.tiled_reconstruction -f <path-to-image> -s <path-to-settings> -o <path-to-save-reconstructed-image>`
```

### Comparing `pyfairsim-0.0.2/pyfairsim/batch_reconstruction.py` & `pyfairsim-0.0.3/pyfairsim/batch_reconstruction.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/parameter_estimation.py` & `pyfairsim-0.0.3/pyfairsim/parameter_estimation.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/phase_estimation.py` & `pyfairsim-0.0.3/pyfairsim/phase_estimation.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/reconstruction.py` & `pyfairsim-0.0.3/pyfairsim/reconstruction.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/sim_algorithm/Direction.py` & `pyfairsim-0.0.3/pyfairsim/sim_algorithm/Direction.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/sim_algorithm/OTF_Provider.py` & `pyfairsim-0.0.3/pyfairsim/sim_algorithm/OTF_Provider.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Parameters.py` & `pyfairsim-0.0.3/pyfairsim/sim_algorithm/SIM_Parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,26 +175,29 @@
 class Image_Parameters:
     def __init__(
         self,
         image_shape: Tuple[int, int],
         ordering: str,
         z_slice: int,
         background: float,
+        tile_size: int,
     ):
         self.image_shape = image_shape
         self.ordering = ordering
         self.z_slice = z_slice
         self.background = background
+        self.tile_size = tile_size
 
     def as_dict(self) -> dict:
         out_dict = {}
         out_dict["image_shape"] = self.image_shape
         out_dict["ordering"] = self.ordering
         out_dict["z_slice"] = self.z_slice
         out_dict["background"] = self.background
+        out_dict["tile_size"] = self.tile_size
 
         return out_dict
 
     @classmethod
     def as_descriptive_dict(cls) -> dict:
         out_dict = {}
         out_dict[
@@ -205,24 +208,30 @@
         ] = "the ordering of the images: p for phase, z for z, a for angel."
         out_dict[
             "z_slice"
         ] = "which z slice should be reconstructed. Starts to count from 0"
         out_dict[
             "background"
         ] = "Background value that should be subtracted from the raw data before further processing"
-
+        out_dict["tile_size"] = "the size of separate tiles in a tiled reconstruction"
         return out_dict
 
     @classmethod
     def from_dict(cls, data_dict: dict) -> "Image_Parameters":
         image_shape = data_dict["image_shape"]
         ordering = data_dict["ordering"]
         z_slice = data_dict["z_slice"]
         background = data_dict["background"]
-        return Image_Parameters(image_shape, ordering, z_slice, background)
+        if "tile_size" in data_dict.keys():
+            tile_size = data_dict["tile_size"]
+        else:
+            tile_size = 32
+            logger.warning(f"no tile_size set, using default: {tile_size}")
+
+        return Image_Parameters(image_shape, ordering, z_slice, background, tile_size)
 
 
 class Parameters:
     def __init__(
         self,
         directions: List[Direction],
         microscope_parameters: Microscope_Parameters,
```

### Comparing `pyfairsim-0.0.2/pyfairsim/sim_algorithm/SIM_Utils.py` & `pyfairsim-0.0.3/pyfairsim/sim_algorithm/SIM_Utils.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/sim_algorithm/Wiener_Filter.py` & `pyfairsim-0.0.3/pyfairsim/sim_algorithm/Wiener_Filter.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/utils/argparse.py` & `pyfairsim-0.0.3/pyfairsim/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/utils/load_settings.py` & `pyfairsim-0.0.3/pyfairsim/utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim/utils/physics.py` & `pyfairsim-0.0.3/pyfairsim/utils/physics.py`

 * *Files identical despite different names*

### Comparing `pyfairsim-0.0.2/pyfairsim.egg-info/SOURCES.txt` & `pyfairsim-0.0.3/pyfairsim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 pyfairsim/__init__.py
 pyfairsim/batch_reconstruction.py
 pyfairsim/create_example_settings.py
 pyfairsim/parameter_estimation.py
 pyfairsim/phase_estimation.py
 pyfairsim/reconstruction.py
+pyfairsim/tiled_reconstruction.py
 pyfairsim.egg-info/PKG-INFO
 pyfairsim.egg-info/SOURCES.txt
 pyfairsim.egg-info/dependency_links.txt
 pyfairsim.egg-info/requires.txt
 pyfairsim.egg-info/top_level.txt
 pyfairsim/sim_algorithm/Direction.py
 pyfairsim/sim_algorithm/OTF_Provider.py
```

### Comparing `pyfairsim-0.0.2/setup.py` & `pyfairsim-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "A package to run sim reconstructions including parameter estimation."
 AUTHOR = "Jakob Wessendorf"
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 def get_packages():
```

### Comparing `pyfairsim-0.0.2/tests/test_locate_peak.py` & `pyfairsim-0.0.3/tests/test_locate_peak.py`

 * *Files identical despite different names*

