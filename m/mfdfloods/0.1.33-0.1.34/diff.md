# Comparing `tmp/mfdfloods-0.1.33.tar.gz` & `tmp/mfdfloods-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfdfloods-0.1.33.tar", last modified: Tue Feb 21 09:33:01 2023, max compression
+gzip compressed data, was "mfdfloods-0.1.34.tar", last modified: Fri Jun 23 18:58:11 2023, max compression
```

## Comparing `mfdfloods-0.1.33.tar` & `mfdfloods-0.1.34.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 orzo      (1000) orzo      (1000)        0 2023-02-21 09:33:01.184896 mfdfloods-0.1.33/
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1086 2023-02-06 13:12:26.000000 mfdfloods-0.1.33/LICENSE
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     2176 2023-02-21 09:33:01.180896 mfdfloods-0.1.33/PKG-INFO
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1436 2023-02-06 13:12:26.000000 mfdfloods-0.1.33/README.md
-drwxrwxr-x   0 orzo      (1000) orzo      (1000)        0 2023-02-21 09:33:01.180896 mfdfloods-0.1.33/mfdfloods/
--rw-rw-r--   0 orzo      (1000) orzo      (1000)       46 2023-02-21 09:32:48.000000 mfdfloods-0.1.33/mfdfloods/__init__.py
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     2455 2023-02-06 13:12:26.000000 mfdfloods-0.1.33/mfdfloods/__main__.py
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1779 2023-01-30 19:15:58.000000 mfdfloods-0.1.33/mfdfloods/debug.py
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1129 2023-02-06 13:12:26.000000 mfdfloods-0.1.33/mfdfloods/geotransform.py
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1090 2023-02-06 13:12:26.000000 mfdfloods-0.1.33/mfdfloods/gtif.py
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1532 2023-02-14 22:05:24.000000 mfdfloods-0.1.33/mfdfloods/hydrogram.py
--rw-rw-r--   0 orzo      (1000) orzo      (1000)    14265 2023-02-14 23:05:13.000000 mfdfloods-0.1.33/mfdfloods/main.py
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1612 2023-02-10 23:42:37.000000 mfdfloods-0.1.33/mfdfloods/matrix.py
-drwxrwxr-x   0 orzo      (1000) orzo      (1000)        0 2023-02-21 09:33:01.180896 mfdfloods-0.1.33/mfdfloods.egg-info/
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     2176 2023-02-21 09:33:01.000000 mfdfloods-0.1.33/mfdfloods.egg-info/PKG-INFO
--rw-rw-r--   0 orzo      (1000) orzo      (1000)      400 2023-02-21 09:33:01.000000 mfdfloods-0.1.33/mfdfloods.egg-info/SOURCES.txt
--rw-rw-r--   0 orzo      (1000) orzo      (1000)        1 2023-02-21 09:33:01.000000 mfdfloods-0.1.33/mfdfloods.egg-info/dependency_links.txt
--rw-rw-r--   0 orzo      (1000) orzo      (1000)       54 2023-02-21 09:33:01.000000 mfdfloods-0.1.33/mfdfloods.egg-info/entry_points.txt
--rw-rw-r--   0 orzo      (1000) orzo      (1000)       19 2023-02-21 09:33:01.000000 mfdfloods-0.1.33/mfdfloods.egg-info/requires.txt
--rw-rw-r--   0 orzo      (1000) orzo      (1000)       10 2023-02-21 09:33:01.000000 mfdfloods-0.1.33/mfdfloods.egg-info/top_level.txt
--rw-rw-r--   0 orzo      (1000) orzo      (1000)     1054 2023-02-21 09:32:34.000000 mfdfloods-0.1.33/pyproject.toml
--rw-rw-r--   0 orzo      (1000) orzo      (1000)       38 2023-02-21 09:33:01.184896 mfdfloods-0.1.33/setup.cfg
+drwxrwxr-x   0 orzo      (1000) orzo      (1000)        0 2023-06-23 18:58:11.955588 mfdfloods-0.1.34/
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1086 2023-04-20 10:26:13.000000 mfdfloods-0.1.34/LICENSE
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     2176 2023-06-23 18:58:11.955588 mfdfloods-0.1.34/PKG-INFO
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1436 2023-04-20 10:26:13.000000 mfdfloods-0.1.34/README.md
+drwxrwxr-x   0 orzo      (1000) orzo      (1000)        0 2023-06-23 18:58:11.951588 mfdfloods-0.1.34/mfdfloods/
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)       46 2023-06-23 18:52:59.000000 mfdfloods-0.1.34/mfdfloods/__init__.py
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     3307 2023-06-23 18:33:48.000000 mfdfloods-0.1.34/mfdfloods/__main__.py
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1779 2023-01-30 19:15:58.000000 mfdfloods-0.1.34/mfdfloods/debug.py
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1129 2023-04-20 10:26:13.000000 mfdfloods-0.1.34/mfdfloods/geotransform.py
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1090 2023-04-20 10:26:13.000000 mfdfloods-0.1.34/mfdfloods/gtif.py
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1532 2023-04-20 10:26:13.000000 mfdfloods-0.1.34/mfdfloods/hydrogram.py
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)    16740 2023-06-23 18:49:13.000000 mfdfloods-0.1.34/mfdfloods/main.py
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1612 2023-04-20 10:26:13.000000 mfdfloods-0.1.34/mfdfloods/matrix.py
+drwxrwxr-x   0 orzo      (1000) orzo      (1000)        0 2023-06-23 18:58:11.955588 mfdfloods-0.1.34/mfdfloods.egg-info/
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     2176 2023-06-23 18:58:11.000000 mfdfloods-0.1.34/mfdfloods.egg-info/PKG-INFO
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)      400 2023-06-23 18:58:11.000000 mfdfloods-0.1.34/mfdfloods.egg-info/SOURCES.txt
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)        1 2023-06-23 18:58:11.000000 mfdfloods-0.1.34/mfdfloods.egg-info/dependency_links.txt
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)       54 2023-06-23 18:58:11.000000 mfdfloods-0.1.34/mfdfloods.egg-info/entry_points.txt
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)       19 2023-06-23 18:58:11.000000 mfdfloods-0.1.34/mfdfloods.egg-info/requires.txt
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)       10 2023-06-23 18:58:11.000000 mfdfloods-0.1.34/mfdfloods.egg-info/top_level.txt
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)     1054 2023-06-23 18:52:53.000000 mfdfloods-0.1.34/pyproject.toml
+-rw-rw-r--   0 orzo      (1000) orzo      (1000)       38 2023-06-23 18:58:11.955588 mfdfloods-0.1.34/setup.cfg
```

### Comparing `mfdfloods-0.1.33/LICENSE` & `mfdfloods-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `mfdfloods-0.1.33/PKG-INFO` & `mfdfloods-0.1.34/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfdfloods
-Version: 0.1.33
+Version: 0.1.34
 Summary: Multiple flow direction floods hydrodynamic modelation
 Author-email: Orzo Cogorzo <orzocogorzo@hotmail.com>
 Project-URL: Homepage, https://github.com/orzocogorzo/mfdfloods
 Keywords: mfdfloods,mfd,flood,drainpaths,hidrology,downstreams,multiple flow direction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mfdfloods-0.1.33/README.md` & `mfdfloods-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `mfdfloods-0.1.33/mfdfloods/__main__.py` & `mfdfloods-0.1.34/mfdfloods/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,73 +7,109 @@
 from .main import MFD
 from .gtif import writef
 
 
 def main(
     dtm_path: str,
     mannings_path: str,
+    water_path: str | None,
     hydrogram: list,
     lng: float,
     lat: float,
 ) -> None:
     """
-    Runs a floods distribution modelation. 
+    Runs a floods distribution modelation.
 
     Parameters:
     area <str>: Name of the area
     lng <float>: Longitude of the brak point
     lat <float>: Latitude of the break point
     hydrogram <list[typle[float, float]]>: A list of pair values with time and flow representing the break hydrogram
 
     Returns:
     None: The script will write three raster files on the data directory
     """
 
     floods, drafts, speeds = None, None, None
     try:
-        model = MFD(dtm_path, mannings_path, radius=3000, mute=False)
+        model = MFD(dtm_path, mannings_path, water_path, radius=3000, mute=False)
         floods, drafts, speeds = model.drainpaths((lng, lat), hydrogram)
     except KeyboardInterrupt as e:
         print(e)
         print("Keyboard Interruption")
     finally:
         if not (floods is None or drafts is None or speeds is None):
             data_dir = os.path.dirname(dtm_path)
             writef(os.path.join(data_dir, "floods.tif"), floods, dtm_path)
             writef(os.path.join(data_dir, "drafts.tif"), drafts, dtm_path)
             writef(os.path.join(data_dir, "speeds.tif"), speeds, dtm_path)
 
 
 if __name__ == "__main__":
-    if len(sys.argv) < 4:
-        print("Usage: python -m mfdfloods <path:data_dir> <float:lng> <float:lat> [float:radius]")
-        exit()
+    if len(sys.argv) < 3:
+        print("Usage: python -m mfdfloods <path:data_dir> <int:pk>")
+        exit(1)
 
     kwargs = dict()
     data_dir = os.path.abspath(sys.argv[1])
-    kwargs["lng"] = float(sys.argv[2])
-    kwargs["lat"] = float(sys.argv[3])
+    try:
+        pk = sys.argv[2]
+    except Exception as e:
+        print("Invalid pk")
+        exit(1)
+
+    data = None
+    with open(os.path.join(data_dir, "pks.csv")) as f:
+        reader = csv.reader(f)
+        headers = None
+        for row in reader:
+            if data is not None:
+                break
+
+            if headers is None:
+                headers = row
+                continue
+
+            if row[headers.index("pk")] == pk:
+                data = {headers[i]: row[i] for i in range(len(headers))}
+
+    if data is None:
+        print("Pk not found")
+        exit(1)
 
     dtm_path = os.path.join(data_dir, "dtm.tif")
     if not os.path.isfile(dtm_path):
         raise FileNotFoundError(dtm_path + " does not exists")
     else:
-        kwargs["dtm_path"] = dtm_path
+        data["dtm_path"] = dtm_path
 
     mannings_path = os.path.join(data_dir, "mannings.tif")
     if not os.path.isfile(mannings_path):
         raise FileNotFoundError(mannings_path + " does not exists")
     else:
-        kwargs["mannings_path"] = mannings_path
+        data["mannings_path"] = mannings_path
+
+    water_path = os.path.join(data_dir, "water.tif")
+    if os.path.isfile(water_path):
+        data["water_path"] = water_path
+    else:
+        data["water_path"] = None
 
     hydrogram_name = os.path.join(data_dir, "hydrogram.csv")
     if not os.path.isfile(hydrogram_name):
         raise FileNotFoundError(hydrogram_name + " does not exists")
     else:
         with open(hydrogram_name) as f:
             reader = csv.reader(f, delimiter=",", quotechar='"')
-            kwargs["hydrogram"] = [row for row in reader]
+            data["hydrogram"] = [row for row in reader]
 
-    if len(sys.argv) == 5:
-        kwargs["radius"] = float(sys.argv[4])
+    if len(sys.argv) == 4:
+        data["radius"] = float(sys.argv[3])
 
-    main(**kwargs)
+    main(
+        data["dtm_path"],
+        data["mannings_path"],
+        data["water_path"],
+        data["hydrogram"],
+        float(data["lng"]),
+        float(data["lat"]),
+    )
```

### Comparing `mfdfloods-0.1.33/mfdfloods/debug.py` & `mfdfloods-0.1.34/mfdfloods/debug.py`

 * *Files identical despite different names*

### Comparing `mfdfloods-0.1.33/mfdfloods/geotransform.py` & `mfdfloods-0.1.34/mfdfloods/geotransform.py`

 * *Files identical despite different names*

### Comparing `mfdfloods-0.1.33/mfdfloods/gtif.py` & `mfdfloods-0.1.34/mfdfloods/gtif.py`

 * *Files identical despite different names*

### Comparing `mfdfloods-0.1.33/mfdfloods/hydrogram.py` & `mfdfloods-0.1.34/mfdfloods/hydrogram.py`

 * *Files identical despite different names*

### Comparing `mfdfloods-0.1.33/mfdfloods/main.py` & `mfdfloods-0.1.34/mfdfloods/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # BULTINS
 import math
 from typing import Optional
+from osgeo.gdal import Dataset
 
 # VENDOR
 import richdem as rd
 import numpy as np
 from numpy.typing import NDArray
 
 # MODULES
@@ -17,126 +18,169 @@
 
 def del_key(key, handle) -> None:
     try:
         del handle[key]
     except KeyError:
         pass
 
+
 class MFD(Matrix):
+    max_drain: float = 5e1
+    dtm_ds: Dataset
+    mannings_ds: Dataset
+    water_ds: Dataset | None = None
+    dtm_gt: tuple
+    mannings_gt: tuple
+    water_gt: tuple
+    dtm: rd.rdarray
+    mannings: GeoTransformFit
+    water: GeoTransformFit
+    cellsize: float
+    cellarea: float
+    nodata: float
+    radius: float
+    convergence_factor: float
+    speed_trawl: float
+    mute: bool
+
     def __init__(
         self,
         dtm_path: str,
         mannings_path: str,
+        water_path: str | None = None,
         nodata: float = -99,
         radius: float = 2000,
         convergence_factor: float = 1.5,
         speed_trawl: float = 1.5,
-        mute: bool = True
+        mute: bool = True,
     ) -> None:
         self.dtm_ds = openf(dtm_path)
         self.dtm_gt = self.dtm_ds.GetGeoTransform()
         self.mannings_ds = openf(mannings_path)
         self.mannings_gt = self.mannings_ds.GetGeoTransform()
+        if water_path is not None:
+            self.water_ds = openf(water_path)
+            self.water_gt = self.water_ds.GetGeoTransform()
 
         Matrix.__init__(self, as_array(self.dtm_ds))
 
-        self.cellsize = (self.dtm_gt[1] + abs(self.dtm_gt[5])) / 2.
-        self.cellarea = math.pow(self.cellsize, 2.)
+        self.cellsize = (self.dtm_gt[1] + abs(self.dtm_gt[5])) / 2.0
+        self.cellarea = math.pow(self.cellsize, 2.0)
         self.nodata = nodata
 
         self.dtm = rd.rdarray(self.dtm, no_data=nodata)
         rd.FillDepressions(self.dtm, in_place=True)
 
-        self.mannings = self.array(as_array(self.mannings_ds))
         self.mannings = GeoTransformFit(
-            self.mannings,
+            self.array(as_array(self.mannings_ds)),
             self.mannings_gt,
             self.dtm_gt,
         )
 
+        if self.water_ds is not None:
+            self.water = GeoTransformFit(
+                self.array(as_array(self.water_ds)),
+                self.water_gt,
+                self.dtm_gt,
+            )
+        else:
+            self.water = GeoTransformFit(
+                self.dtm * 0,
+                self.dtm_gt,
+                self.dtm_gt,
+            )
+
         self.radius = radius
         self.convergence_factor = convergence_factor
         self.speed_trawl = speed_trawl
-        self.max_drain = 2e+1
         self.mute = mute
 
     def __del__(self) -> None:
         try:
             del self.dtm_ds
             del self.mannings_ds
         except AttributeError:
             pass
 
     def start_point(self, rc: tuple, drafts: NDArray) -> tuple:
         slopes = self.get_slopes(rc, drafts)
         direction = slopes.argmin()
         deltas = self.get_deltas(rc)
         gateway = deltas[direction]
-        
+
         self.overcomes[rc] = True
         for delta in deltas:
             if not (delta[0] == gateway[0] and delta[1] == gateway[1]):
                 self.overcomes[tuple(delta)] = True
 
         return tuple(gateway), slopes[direction]
 
     def get_deltas(self, rc: tuple) -> NDArray:
         # Non visited deltas
-        return self.array([
-            delta for delta in rc + self.deltas
-            # if tuple(delta) not in self.overcomes
-        ])
+        return self.array([delta for delta in rc + self.deltas])
 
-    def get_slopes(self, rc: tuple, drafts: NDArray, self_draft: Optional[float] = None) -> NDArray:
+    def get_slopes(
+        self, rc: tuple, drafts: NDArray, self_draft: Optional[float] = None
+    ) -> NDArray:
         # Get peripheric alt deltas
         if self_draft is None:
             self_draft = float(drafts[rc])
 
-        return self.array([
-            (float(self.dtm[tuple(delta)]) + float(drafts[tuple(delta)])) - (self.dtm[rc] + self_draft)
-            for delta in self.get_deltas(rc)
-        ])
+        return self.array(
+            [
+                (float(self.dtm[tuple(delta)]) + float(drafts[tuple(delta)]))
+                - (self.dtm[rc] + self_draft)
+                for delta in self.get_deltas(rc)
+            ]
+        )
 
     def get_slope(self, slopes: NDArray) -> float:
         # Max cell traversal slope
         try:
-            slopes = np.append(slopes, .0)
+            slopes = np.append(slopes, 0.0)
             return slopes.min() - slopes.max()
         except Exception:
-            return .0
+            return 0.0
 
     def get_volumetries(self, slopes: NDArray) -> NDArray:
         # Volumetrie of the pyramide from the center to the edge (half of the cell)
-        return self.cellarea * .25 * slopes * (1. / 3.)
+        return self.cellarea * 0.25 * slopes * (1.0 / 3.0)
 
     def get_downslopes(self, slopes: NDArray) -> NDArray:
         # Negativa alt deltas
-        return self.where(slopes < .0, slopes * -1, .0)
+        return self.where(slopes < 0.0, slopes * -1, 0.0)
 
     def get_upslopes(self, slopes: NDArray) -> NDArray:
         # Positive alt deltas
-        return self.where(slopes >= .0, slopes, .0)
+        return self.where(slopes >= 0.0, slopes, 0.0)
 
     def get_draft(self, flood: float) -> float:
         # return (flood + self.get_volumetries(slopes * .5).sum()) / self.cellarea
         return flood / self.cellarea
 
     def get_speeds(self, slopes: NDArray, draft: float, manning) -> NDArray:
         return self.array([self.get_speed(draft, manning, slope) for slope in slopes])
 
     def get_speed(self, draft: float, manning, slope: float) -> float:
         # Manning formula
-        return max(.0, (1. / manning) * math.pow(self.cellsize + 2. * draft, 2. / 3.) * math.pow(max(.0, abs(slope)) / self.cellsize, .5))
+        return max(
+            0.0,
+            (1.0 / manning)
+            * math.pow(self.cellsize + 2.0 * draft, 2.0 / 3.0)
+            * math.pow(max(0.0, abs(slope)) / self.cellsize, 0.5),
+        )
 
-    def drainpaths(self, source: tuple, hydrogram_curve: list) -> tuple[NDArray, NDArray, NDArray]:
+    def drainpaths(
+        self, source: tuple, hydrogram_curve: list
+    ) -> tuple[NDArray, NDArray, NDArray]:
         floods = self.zeros(self.dtm.shape)
         drafts = self.zeros(self.dtm.shape)
         speeds = self.zeros(self.dtm.shape)
         drainages = self.zeros(self.dtm.shape)
-        flood_factor = .0
+        flood_factor = 0.0
         self.is_over = False
         self.overcomes = {}
 
         def _drainpaths(
             rcs: dict,
             next_step: dict,
             catchments: dict,
@@ -146,105 +190,145 @@
         ) -> tuple[dict, dict]:
             try:
                 reacheds = {}
                 if self.is_over:
                     return {}, {}
 
                 for rc in rcs:
-                    if rc in self.overcomes:
+                    if self.water[rc] == 1:
+                        self.overcomes[rc] = True
+                        del_key(rc, next_step)
+                        del_key(rc, reacheds)
+                        del_key(rc, visited)
+
+                    if self.overcomes.get(rc) is not None:
                         continue
 
                     if type(rcs[rc]) is int and rcs[rc] > 1:
                         next_step[rc] = rcs[rc] - 1
                         continue
 
                     src_deltas = self.get_deltas(rc)
-                    src_flood = max(.0, float(floods[rc]) + catchments.get(rc, .0))
+                    src_flood = max(0.0, float(floods[rc]) + catchments.get(rc, 0.0))
                     src_draft = self.get_draft(src_flood)
                     src_slopes = self.get_slopes(rc, drafts, src_draft)
                     src_slope = self.get_slope(src_slopes)
                     src_speed = self.get_speed(src_draft, self.mannings[rc], src_slope)
 
                     if src_speed / level / self.cellsize < 1:
                         if drainages[rc] <= self.max_drain:
                             next_step[rc] = True
                         else:
                             self.overcomes[rc] = True
                             del_key(rc, next_step)
+                            del_key(rc, reacheds)
+                            del_key(rc, visited)
                         continue
 
                     downslopes = self.get_downslopes(src_slopes)
                     upslopes = self.get_upslopes(src_slopes)
                     under_volume = self.get_volumetries(downslopes)
                     over_volume = self.get_volumetries(upslopes)
 
                     if downslopes.sum() == 0:
-                        over_flood = max(.0, src_flood - over_volume.min() * 8)
-                        drived_flood = .0
+                        over_flood = max(0.0, src_flood - over_volume.min() * 8)
+                        drived_flood = 0.0
                         if over_flood == 0:
                             if drainages[rc] <= self.max_drain:
                                 next_step[rc] = True
                             else:
                                 self.overcomes[rc] = True
                                 del_key(rc, next_step)
+                                del_key(rc, visited)
+                                del_key(rc, reacheds)
                             continue
                     else:
                         drived_flood = min(src_flood, under_volume.sum())
                         over_flood = src_flood - drived_flood
 
-                    over_catchments = self.where(src_flood > over_volume * 8, src_flood - over_volume * 8, 0)
-                    over_floods = over_catchments / over_catchments.sum() * over_flood if over_catchments.sum() else self.zeros((len(src_deltas),))
+                    over_catchments = self.where(
+                        src_flood > over_volume * 8, src_flood - over_volume * 8, 0
+                    )
+                    over_floods = (
+                        over_catchments / over_catchments.sum() * over_flood
+                        if over_catchments.sum()
+                        else self.zeros((len(src_deltas),))
+                    )
                     over_floods = self.where(over_floods > 1e-3, over_floods, 0)
-                    drived_floods = downslopes / downslopes.sum() * drived_flood if downslopes.sum() else self.zeros((len(src_deltas),))
+                    drived_floods = (
+                        downslopes / downslopes.sum() * drived_flood
+                        if downslopes.sum()
+                        else self.zeros((len(src_deltas),))
+                    )
                     drived_floods = self.where(drived_floods > 1e-3, drived_floods, 0)
                     src_floods = over_floods + drived_floods
-                    src_speeds = self.get_speeds(downslopes, float(drafts[rc]), self.mannings[rc])
+                    src_speeds = self.get_speeds(
+                        downslopes, float(drafts[rc]), self.mannings[rc]
+                    )
 
                     if src_floods.sum() == 0:
                         if drainages[rc] <= self.max_drain:
                             next_step[rc] = True
                         else:
                             self.overcomes[rc] = True
                             del_key(rc, next_step)
+                            del_key(rc, reacheds)
+                            del_key(rc, visited)
                         continue
-                    
+
                     src_acum_flood = src_floods.sum()
-                    powered_flood = (np.power(src_floods, self.convergence_factor)).sum()
+                    powered_flood = (
+                        np.power(src_floods, self.convergence_factor)
+                    ).sum()
                     powered_speed = (np.power(src_speeds, self.speed_trawl)).sum()
                     cell_reacheds = 0
                     for i, (flood, speed) in enumerate(zip(src_floods, src_speeds)):
                         new_rc = tuple(src_deltas[i])
                         try:
-                            if self.mannings[new_rc] == self.nodata or self.dtm[new_rc] == self.nodata:
+                            if (
+                                self.mannings[new_rc] == self.nodata
+                                or self.dtm[new_rc] == self.nodata
+                            ):
                                 raise IndexError
                         except IndexError:
                             self.is_over = True
                             return {}, {}
 
                         if flood > 0 and speed > 0:
                             speed = max(speeds[new_rc], speed)
-                            flood = ((np.power(flood, self.convergence_factor) / powered_flood + np.power(speed, self.speed_trawl) / powered_speed) / 2 * src_acum_flood) / level
+                            flood = (
+                                (
+                                    np.power(flood, self.convergence_factor)
+                                    / powered_flood
+                                    + np.power(speed, self.speed_trawl) / powered_speed
+                                )
+                                / 2
+                                * src_acum_flood
+                            ) / level
                             flood = flood * min(1, speed / level / self.cellsize)
-                            catchments[new_rc] = catchments.get(new_rc, .0) + flood
-                            catchments[rc] = catchments.get(rc, .0) - flood
+                            catchments[new_rc] = catchments.get(new_rc, 0.0) + flood
+                            catchments[rc] = catchments.get(rc, 0.0) - flood
 
-                            if new_rc in visited:
+                            if visited.get(rc) is not None:
                                 continue
 
-
-                            if (iters := speed / level / self.cellsize) < 1.:
-                                if drainages[new_rc] <= self.max_drain and not new_rc in reacheds:
+                            if (iters := speed / level / self.cellsize) < 1.0:
+                                if (
+                                    drainages[new_rc] <= self.max_drain
+                                    and reacheds.get(new_rc) is None
+                                ):
                                     next_step[new_rc] = round(1 / iters)
                                 continue
 
                             reacheds[new_rc] = True
                             cell_reacheds += 1
 
                     if cell_reacheds == 0:
                         next_step[rc] = True
+                        del_key(rc, visited)
                     else:
                         visited[rc] = True
 
                 if len(reacheds) > 0:
                     queue.append((reacheds, level + 1))
 
                 if len(queue) > 0:
@@ -253,17 +337,17 @@
                         reacheds,
                         next_step={**next_step, **reacheds},
                         catchments=catchments,
                         level=level,
                         queue=queue,
                         visited=visited,
                     )
-                elif len(visited) > 0:
-                    for rc in visited:
-                        self.overcomes[rc] = True
+
+                for rc in visited:
+                    self.overcomes[rc] = True
 
             except KeyboardInterrupt:
                 self.is_over = True
                 return {}, {}
             except Exception as e:
                 raise e
             finally:
@@ -291,15 +375,15 @@
                 progress = progress_counter("FLOOD")
             else:
                 progress = lambda i, f: f
 
             i = 0
             last_flood = break_flood
             flood = break_flood
-            distance = .0
+            distance = 0.0
             trapped = 0
             peak = 0
             next_step = {start: True}
             catchments = {}
 
             while True:
                 progress(i, flood)
@@ -314,46 +398,52 @@
                     print("\nExit condition: Hydrogram drained")
                     break
 
                 # for rc in catchments:
                 for rc in next_step:
                     catchments[rc] = catchments.get(rc)
                     if catchments[rc] is None:
-                        if rc in self.overcomes:
+                        if self.overcomes.get(rc) is not None:
                             del_key(rc, next_step)
                             continue
 
                         catchments[rc] = prev_catchments.get(rc, 0)
                     catchment = catchments[rc] * flood_factor
                     if catchment <= 0:
                         continue
 
                     floods[rc] += catchment
                     drafts[rc] = self.get_draft(catchment)
                     slope = self.get_slope(self.get_slopes(rc, drafts))
-                    speeds[rc] = self.get_speed(float(drafts[rc]), self.mannings[rc], slope)
+                    speeds[rc] = self.get_speed(
+                        float(drafts[rc]), self.mannings[rc], slope
+                    )
                     drainages[rc] += 1
 
                 prev_catchments = catchments
 
-                edge = np.sqrt(np.power(abs(self.argwhere(floods > 0) - start) * self.cellsize, 2.).sum(1)).max()
+                edge = np.sqrt(
+                    np.power(
+                        abs(self.argwhere(floods > 0) - start) * self.cellsize, 2.0
+                    ).sum(1)
+                ).max()
                 if distance == int(edge) and peak == hyd_statistics["peak"]:
                     trapped += 1
                 else:
                     trapped = 0
 
                 distance = int(edge)
                 i += 1
                 if self.is_over:
                     print("\nExit condition: Flood is over dtm boundaries")
                     break
-                elif i > 5e+3:
+                elif i > 5e3:
                     print("\nExit condition: Max recursion limit")
                     break
-                elif trapped >= 2e+2:
+                elif trapped >= 2e2:
                     print("\nExit condition: Flood's stability reached")
                     break
                 elif distance >= self.radius:
                     print("\nExit condition: Distance limit reached")
                     break
 
                 last_flood = flood
```

### Comparing `mfdfloods-0.1.33/mfdfloods/matrix.py` & `mfdfloods-0.1.34/mfdfloods/matrix.py`

 * *Files identical despite different names*

### Comparing `mfdfloods-0.1.33/mfdfloods.egg-info/PKG-INFO` & `mfdfloods-0.1.34/mfdfloods.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfdfloods
-Version: 0.1.33
+Version: 0.1.34
 Summary: Multiple flow direction floods hydrodynamic modelation
 Author-email: Orzo Cogorzo <orzocogorzo@hotmail.com>
 Project-URL: Homepage, https://github.com/orzocogorzo/mfdfloods
 Keywords: mfdfloods,mfd,flood,drainpaths,hidrology,downstreams,multiple flow direction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mfdfloods-0.1.33/pyproject.toml` & `mfdfloods-0.1.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["mfdfloods"]
 
 [project]
 name = "mfdfloods"
-version = "0.1.33"
+version = "0.1.34"
 description = "Multiple flow direction floods hydrodynamic modelation"
 readme = "README.md"
 authors = [{ name = "Orzo Cogorzo", email = "orzocogorzo@hotmail.com" }]
 license = { file = "MIT" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

