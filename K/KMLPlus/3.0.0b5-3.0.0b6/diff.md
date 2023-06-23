# Comparing `tmp/KMLPlus-3.0.0b5.tar.gz` & `tmp/KMLPlus-3.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMLPlus-3.0.0b5.tar", last modified: Fri Jun 23 15:42:47 2023, max compression
+gzip compressed data, was "KMLPlus-3.0.0b6.tar", last modified: Fri Jun 23 16:51:47 2023, max compression
```

## Comparing `KMLPlus-3.0.0b5.tar` & `KMLPlus-3.0.0b6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/KMLPlus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-23 15:42:46.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 15:42:47.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:42:46.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 15:42:46.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/kmlplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23578 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)    21935 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:51:47.122347 KMLPlus-3.0.0b6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:51:47.118347 KMLPlus-3.0.0b6/KMLPlus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-23 16:51:47.000000 KMLPlus-3.0.0b6/KMLPlus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 16:51:47.000000 KMLPlus-3.0.0b6/KMLPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:51:47.000000 KMLPlus-3.0.0b6/KMLPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 16:51:47.000000 KMLPlus-3.0.0b6/KMLPlus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-23 16:51:47.122347 KMLPlus-3.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:51:47.122347 KMLPlus-3.0.0b6/kmlplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/kmlplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/kmlplus/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/kmlplus/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/kmlplus/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21985 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/kmlplus/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/kmlplus/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:51:47.122347 KMLPlus-3.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:51:47.122347 KMLPlus-3.0.0b6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/test/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-23 16:51:35.000000 KMLPlus-3.0.0b6/test/test_util.py
```

### Comparing `KMLPlus-3.0.0b5/KMLPlus.egg-info/PKG-INFO` & `KMLPlus-3.0.0b6/KMLPlus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KMLPlus-3.0.0b5/LICENSE` & `KMLPlus-3.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b5/PKG-INFO` & `KMLPlus-3.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `KMLPlus-3.0.0b5/README.md` & `KMLPlus-3.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b5/kmlplus/geo.py` & `KMLPlus-3.0.0b6/kmlplus/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union
 
 from pyproj import Geod
 
-import util
 from kmlplus.interface import ILocation, ILocationFactory, ICurvedSegmentFactory, ICurvedSegment
-from kmlplus.util import dms_to_decimal, detect_coordinate_type, split_segment_string
+from kmlplus.util import dms_to_decimal, detect_coordinate_type, split_segment_string, convert_to_metres
 
 
 class Point(ILocation):
     """
     A class for representing a coordinate using y, x, z representation.
 
     Attributes:
@@ -68,15 +67,15 @@
             z (float)
         """
         return self._z
 
     @z.setter
     def z(self, value) -> None:
         if isinstance(value, float):
-            self._z = util.convert_to_metres(value, self.uom)
+            self._z = convert_to_metres(value, self.uom)
         else:
             if value is None:
                 self._z = 0.0
             else:
                 self.z = float(value)
 
     @classmethod
```

### Comparing `KMLPlus-3.0.0b5/kmlplus/interface.py` & `KMLPlus-3.0.0b6/kmlplus/interface.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b5/kmlplus/kml.py` & `KMLPlus-3.0.0b6/kmlplus/kml.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         """
         if kwargs.get('altitude_mode') == 'relativetoground':
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
             altitude_mode = simplekml.AltitudeMode.absolute
 
-        point = PointFactory(coordinate_list, z=kwargs.get('z', 0.0),
+        point = PointFactory(coordinate_list, z=kwargs.get('z', None),
                              uom=kwargs.get('uom', 'M')).process_coordinates()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
 
         pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
         pnt.coords = [(point[0].x, point[0].y, point[0].z)]
         pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
@@ -133,16 +133,16 @@
             None
         """
         poly = Polyhedron(
             lower_coordinate_list,
             upper_coordinate_list,
             lower_layer=kwargs.get('lower_layer', None),
             upper_layer=kwargs.get('upper_layer', None),
-            lower_layer_uom=kwargs.get('lower_layer_uom', 'FT'),
-            upper_layer_uom=kwargs.get('upper_layer_uom', 'FT')
+            lower_layer_uom=kwargs.get('lower_layer_uom', 'M'),
+            upper_layer_uom=kwargs.get('upper_layer_uom', 'M')
         )
 
         lower, upper, sides = poly.to_kml()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Polyhedron'))
 
         if kwargs.get('altitude_mode') == 'relativetoground':
@@ -200,15 +200,15 @@
         """
         if kwargs.get('altitude_mode') == 'relativetoground':
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
             altitude_mode = simplekml.AltitudeMode.absolute
 
         points = Circle(coordinate_list, radius, radius_uom=kwargs.get('radius_uom', 'M'),
-                        uom=('uom', 'FT')).process_points()
+                        uom=('uom', 'M')).process_points()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Circle'))
 
         pol = fol.newpolygon(name=kwargs.get('name', 'KmlPlus Circle'))
         pol.outerboundaryis = points
         pol.polystyle.colour = kwargs.get('colour_hex', '7Fc0c0c0')
         pol.extrude = kwargs.get('extrude', 0)
@@ -246,26 +246,26 @@
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
             altitude_mode = simplekml.AltitudeMode.absolute
 
         cylinder = Cylinder(
             (
                 coordinate_list,
-                radius
+                radius,
             ),
             (
                 coordinate_list,
-                radius
+                radius,
             ),
+            radius_uom=kwargs.get('radius_uom', 'M'),
             lower_layer=kwargs.get('lower_layer', None),
             upper_layer=kwargs.get('upper_layer', None),
             lower_layer_uom=kwargs.get('lower_layer_uom', 'FT'),
             upper_layer_uom=kwargs.get('upper_layer_uom', 'FT'),
-            sample=kwargs.get('sample', 100), uom=kwargs.get('uom', 'FT'),
-            radius_uom=kwargs.get('radius_uom', 'M')
+            sample=kwargs.get('sample', 100), uom=kwargs.get('uom', 'M'),
         )
         lower, upper, sides = cylinder.to_kml()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Cylinder'))
 
         lower_pol = fol.newpolygon(name=kwargs.get('lower_circle_name', 'KmlPlus Circle'))
         lower_pol.outerboundaryis = lower
```

### Comparing `KMLPlus-3.0.0b5/kmlplus/shapes.py` & `KMLPlus-3.0.0b6/kmlplus/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,20 +202,20 @@
         self.sample = kwargs.get('sample', 100)
         self.radius_uom = kwargs.get('radius_uom', 'M')
         self.lower_radius = lower_coordinates[1]
         self.upper_radius = upper_coordinates[1]
         self.lower_layer = self.create_layer(
             (lower_coordinates[0], self.lower_radius),
             kwargs.get('lower_layer', None),
-            kwargs.get('lower_layer_uom', 'FT')
+            kwargs.get('lower_layer_uom', 'M')
         )
         self._upper_layer = self.create_layer(
             (upper_coordinates[0], self.upper_radius),
             kwargs.get('upper_layer', None),
-            kwargs.get('upper_layer_uom', 'FT')
+            kwargs.get('upper_layer_uom', 'M')
         )
         self._sides = self.generate_sides()
 
     @property
     def lower_radius(self) -> float:
         return self._lower_radius
 
@@ -303,15 +303,16 @@
         Args:
             coordinate_list (tuple[list[str, float, int]]): Contains string information for coordinate and radius
             layer_height: The z value of the layer
 
         Returns:
             circle (ICircle): A circle object
         """
-        circle = Circle(coordinate_list[0], coordinate_list[1], z=layer_height, uom=layer_uom)
+        circle = Circle(coordinate_list[0], coordinate_list[1], z=layer_height,
+                        uom=layer_uom, radius_uom=self.radius_uom)
         return circle
 
     def generate_sides(self) -> list[ICircle]:
         """
         Creates the sides of the cylinder. Requires both layers to contain the same amount of points.
 
         Returns:
```

### Comparing `KMLPlus-3.0.0b5/kmlplus/util.py` & `KMLPlus-3.0.0b6/kmlplus/util.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b5/setup.py` & `KMLPlus-3.0.0b6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="KMLPlus",  # Replace with your own username
-    version="3.0.0-beta.5",
+    version="3.0.0-beta.6",
     author="Mark Henderson",
     author_email="mark.henderson1988@gmail.com",
     description="A Python library for creating 3d floating polygons and circles in .kml for Google Earth.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MHenderson1988/kmlplus",
     packages=setuptools.find_packages(),
```

### Comparing `KMLPlus-3.0.0b5/test/test_geo.py` & `KMLPlus-3.0.0b6/test/test_geo.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b5/test/test_shapes.py` & `KMLPlus-3.0.0b6/test/test_shapes.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b5/test/test_util.py` & `KMLPlus-3.0.0b6/test/test_util.py`

 * *Files identical despite different names*

