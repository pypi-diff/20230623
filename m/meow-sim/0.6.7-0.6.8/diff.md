# Comparing `tmp/meow-sim-0.6.7.tar.gz` & `tmp/meow-sim-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.6.7.tar", last modified: Thu Jun 22 19:10:35 2023, max compression
+gzip compressed data, was "meow-sim-0.6.8.tar", last modified: Fri Jun 23 19:54:30 2023, max compression
```

## Comparing `meow-sim-0.6.7.tar` & `meow-sim-0.6.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-22 19:10:31.000000 meow-sim-0.6.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-22 19:10:35.713666 meow-sim-0.6.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-22 19:10:31.000000 meow-sim-0.6.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8378 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     6615 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6063 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     4924 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/propagate.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10400 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    17355 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-06-22 19:10:31.000000 meow-sim-0.6.7/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      708 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-22 19:10:35.000000 meow-sim-0.6.7/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-22 19:10:31.000000 meow-sim-0.6.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 19:10:35.713666 meow-sim-0.6.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:10:35.713666 meow-sim-0.6.7/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-22 19:10:31.000000 meow-sim-0.6.7/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-22 19:10:31.000000 meow-sim-0.6.7/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-22 19:10:31.000000 meow-sim-0.6.7/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-23 19:54:26.000000 meow-sim-0.6.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-23 19:54:30.403039 meow-sim-0.6.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-23 19:54:26.000000 meow-sim-0.6.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8378 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     3298 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6063 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/propagate.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10442 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2023-06-23 19:54:26.000000 meow-sim-0.6.8/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 19:54:30.000000 meow-sim-0.6.8/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-23 19:54:26.000000 meow-sim-0.6.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:54:30.403039 meow-sim-0.6.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:54:30.403039 meow-sim-0.6.8/tests/
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-06-23 19:54:26.000000 meow-sim-0.6.8/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-06-23 19:54:26.000000 meow-sim-0.6.8/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-23 19:54:26.000000 meow-sim-0.6.8/tests/test_nbs.py
```

### Comparing `meow-sim-0.6.7/LICENSE` & `meow-sim-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/PKG-INFO` & `meow-sim-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.7
+Version: 0.6.8
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.7/README.md` & `meow-sim-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/__init__.py` & `meow-sim-0.6.8/meow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.6.7/meow/assets/silicon.csv` & `meow-sim-0.6.8/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/assets/silicon_oxide.csv` & `meow-sim-0.6.8/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/base_model.py` & `meow-sim-0.6.8/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/cache.py` & `meow-sim-0.6.8/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/eme/__init__.py` & `meow-sim-0.6.8/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/eme/common.py` & `meow-sim-0.6.8/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/eme/propagate.py` & `meow-sim-0.6.8/meow/eme/propagate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/eme/sax.py` & `meow-sim-0.6.8/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/environment.py` & `meow-sim-0.6.8/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/fde/lumerical.py` & `meow-sim-0.6.8/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/fde/tidy3d.py` & `meow-sim-0.6.8/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/gds_structures.py` & `meow-sim-0.6.8/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/geometries.py` & `meow-sim-0.6.8/meow/geometries.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,18 @@
     z_min: float = Field(description="the minimum z-value of the box")
     z_max: float = Field(description="the maximum z-value of the box")
 
     def _mask2d(self, X, Y, z):
         if (z < self.z_min) or (self.z_max < z):
             return np.zeros_like(X, dtype=bool)
         return (
-            (self.x_min <= X) & (X < self.x_max) & (self.y_min <= Y) & (Y < self.y_max)
+            (self.x_min <= X)
+            & (X <= self.x_max)
+            & (self.y_min <= Y)
+            & (Y <= self.y_max)
         )
 
     def _lumadd(self, sim, material_name, mesh_order, unit, xyz):
         x, y, z = xyz
         name = token_hex(4)
         kwargs = {
             f"{x}_min": float(self.x_min * unit),
@@ -154,15 +157,15 @@
         for intersection in intersections.geoms:
             intersection = np.asarray(intersection.coords)
             if not intersection.shape[0]:
                 return np.zeros_like(X, dtype=bool)
             (y_min, _), (y_max, _) = intersection
             y_min, y_max = min(y_min, y_max), max(y_min, y_max)
             x_min, x_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-            mask |= (x_min <= X) & (X < x_max) & (y_min <= Y) & (Y < y_max)
+            mask |= (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
         return mask
 
     def _mask2d_axis_y(self, X, Y, z):
         # x, y, z -> z, x, y
         poly = sg.Polygon(self.poly)
         _, x_min = self.poly.min(0)
         _, x_max = self.poly.max(0)
@@ -181,15 +184,15 @@
         for intersection in intersections.geoms:
             intersection = np.asarray(intersection.coords)
             if not intersection.shape[0]:
                 continue
             (_, x_min), (_, x_max) = intersection
             x_min, x_max = min(x_min, x_max), max(x_min, x_max)
             y_min, y_max = min(self.h_min, self.h_max), max(self.h_min, self.h_max)
-            mask |= (x_min <= X) & (X < x_max) & (y_min <= Y) & (Y < y_max)
+            mask |= (x_min <= X) & (X <= x_max) & (y_min <= Y) & (Y <= y_max)
         return mask
 
     def _mask2d_axis_z(self, X, Y, z):
         # x, y, z -> x, y, z
         poly = sg.Polygon(self.poly)
         if (z < self.h_min) or (self.h_max < z):
             return np.zeros_like(X, dtype=bool)
```

### Comparing `meow-sim-0.6.7/meow/integrate.py` & `meow-sim-0.6.8/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/materials.py` & `meow-sim-0.6.8/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/mesh.py` & `meow-sim-0.6.8/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow/mode.py` & `meow-sim-0.6.8/meow/mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,25 @@
             # little bit lighter colored than the one in cs._visualize:
             n_cmap = colors.LinearSegmentedColormap.from_list(
                 name="c_cmap", colors=["#ffffff", "#c1d9ed"]
             )
         self.cs._visualize(ax=ax, n_cmap=n_cmap, cbar=False, show=False)
 
         x, y = "x", "y"  # currently only propagation in z supported, see Mesh2d
-        c = {"Ex": "x", "Ey": "y", "Ez": "z", "Hx": "y", "Hy": "x", "Hz": "z_"}[field]
+        c = {
+            "Ex": "x",
+            "Ey": "y",
+            "Ez": "z",
+            "Hx": "y",
+            "Hy": "x",
+            "Hz": "z_",
+            "Px": "x",
+            "Py": "y",
+            "Pz": "z",
+        }[field]
         if mode_cmap is None:
             mode_cmap = "inferno"
         X = getattr(self.mesh, f"X{c}")
         Y = getattr(self.mesh, f"Y{c}")
         mode = operation(getattr(self, field))
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
```

### Comparing `meow-sim-0.6.7/meow/structures.py` & `meow-sim-0.6.8/meow/structures.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,7 +41,19 @@
     return scene.show()
 
 
 def sort_structures(structures):
     struct_info = [(s.mesh_order, -i, s) for i, s in enumerate(structures)]
     sorted_struct_info = sorted(struct_info, key=lambda I: (I[0], I[1]), reverse=True)
     return [s for _, _, s in sorted_struct_info]
+
+
+def classify_structures_by_mesh_order_and_material(structures, materials):
+    structures = sort_structures(structures)
+    structures_dict = {}
+    for structure in structures:
+        mo = structure.mesh_order
+        mat = materials[structure.material]
+        if (mo, mat) not in structures_dict:
+            structures_dict[mo, mat] = []
+        structures_dict[mo, mat].append(structure)
+    return structures_dict
```

### Comparing `meow-sim-0.6.7/meow/visualize.py` & `meow-sim-0.6.8/meow/visualize.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.6.8/meow_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.6.7
+Version: 0.6.8
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.6.7/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.6.8/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.6.7/pyproject.toml` & `meow-sim-0.6.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.6.7"
+version = "0.6.8"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.6.7/tests/test_deserialization.py` & `meow-sim-0.6.8/tests/test_deserialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "cell": {
             "structures": [
                 {
                     "material": {
                         "name": "SiO2",
                         "params": {"wl": [1.2]},
                         "n": {"real": [1.955], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -1.0,
                         "x_max": 1.0,
                         "y_min": 0.0,
                         "y_max": 3.5,
@@ -47,14 +48,15 @@
                     "mesh_order": 5,
                 },
                 {
                     "material": {
                         "name": "SiO2",
                         "params": {"wl": [1.2]},
                         "n": {"real": [1.955], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -4.0,
                         "x_max": 4.0,
                         "y_min": -2.0,
                         "y_max": 2.3,
@@ -64,14 +66,15 @@
                     "mesh_order": 5,
                 },
                 {
                     "material": {
                         "name": "Si",
                         "params": {"wl": [1.2], "T": [38.0]},
                         "n": {"real": [3.526617910662], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -0.75,
                         "x_max": 0.75,
                         "y_min": 0.0,
                         "y_max": 3.0,
@@ -81,14 +84,15 @@
                     "mesh_order": 5,
                 },
                 {
                     "material": {
                         "name": "Si",
                         "params": {"wl": [1.2], "T": [38.0]},
                         "n": {"real": [3.526617910662], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -4.0,
                         "x_max": 4.0,
                         "y_min": 0.0,
                         "y_max": 1.8,
```

### Comparing `meow-sim-0.6.7/tests/test_mode_operators.py` & `meow-sim-0.6.8/tests/test_mode_operators.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         "cell": {
             "structures": [
                 {
                     "material": {
                         "name": "SiO2",
                         "params": {"wl": [1.2]},
                         "n": {"real": [1.955], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -1.0,
                         "x_max": 1.0,
                         "y_min": 0.0,
                         "y_max": 3.5,
@@ -29,14 +30,15 @@
                     "mesh_order": 5,
                 },
                 {
                     "material": {
                         "name": "SiO2",
                         "params": {"wl": [1.2]},
                         "n": {"real": [1.955], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -4.0,
                         "x_max": 4.0,
                         "y_min": -2.0,
                         "y_max": 2.3,
@@ -46,14 +48,15 @@
                     "mesh_order": 5,
                 },
                 {
                     "material": {
                         "name": "Si",
                         "params": {"wl": [1.2], "T": [38.0]},
                         "n": {"real": [3.526617910662], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -0.75,
                         "x_max": 0.75,
                         "y_min": 0.0,
                         "y_max": 3.0,
@@ -63,14 +66,15 @@
                     "mesh_order": 5,
                 },
                 {
                     "material": {
                         "name": "Si",
                         "params": {"wl": [1.2], "T": [38.0]},
                         "n": {"real": [3.526617910662], "imag": [0.0]},
+                        "type": "SampledMaterial",
                     },
                     "geometry": {
                         "type": "Box",
                         "x_min": -4.0,
                         "x_max": 4.0,
                         "y_min": 0.0,
                         "y_max": 1.8,
```

### Comparing `meow-sim-0.6.7/tests/test_nbs.py` & `meow-sim-0.6.8/tests/test_nbs.py`

 * *Files identical despite different names*

