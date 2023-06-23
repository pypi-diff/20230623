# Comparing `tmp/KMLPlus-3.0.0b4.tar.gz` & `tmp/KMLPlus-3.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMLPlus-3.0.0b4.tar", last modified: Thu Jun 22 14:35:11 2023, max compression
+gzip compressed data, was "KMLPlus-3.0.0b5.tar", last modified: Fri Jun 23 15:42:47 2023, max compression
```

## Comparing `KMLPlus-3.0.0b4.tar` & `KMLPlus-3.0.0b5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/KMLPlus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/kmlplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22594 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/KMLPlus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-23 15:42:46.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 15:42:47.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:42:46.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 15:42:46.000000 KMLPlus-3.0.0b5/KMLPlus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/kmlplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23578 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21935 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/kmlplus/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:47.060622 KMLPlus-3.0.0b5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-23 15:42:36.000000 KMLPlus-3.0.0b5/test/test_util.py
```

### Comparing `KMLPlus-3.0.0b4/KMLPlus.egg-info/PKG-INFO` & `KMLPlus-3.0.0b5/KMLPlus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,15 +58,15 @@
 Installing
 ----------
 
 ### Pip
 
 ```
 pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus==3.0.0b3 <--- Current v3.0.0-beta.3
+pip install kmlplus==3.0.0b5 <--- Current v3.0.0-beta.5
 ```
 
 ### Clone
 
 ```
 git clone https://github.com/MHenderson1988/kmlplus.git
 
@@ -155,51 +155,56 @@
 linestring(coordinate_list, **kwargs)
 
 The linestring function updates the kml file with a KML linestring feature.
 
 ```
 from kmlplus.kml import KmlPlus
 
-"""
+        """
 
         Args:
             coordinate_list (list): A list containing a single coordinate
         Keyword Args:
+            uom: The unit of measurement for the Z value. Default is metres (M).
+            z (int): The Z value for the point. Default is 0.
             fol (str): A string to name the folder in which the point is stored.
             linestring_name (str): String to name the LineString object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             width(int): Line width
             altitude_mode(str): Accepts simplekml Altitude mode options
 
 
         Returns:
             None
 
-  """
+        """
 
 kml_file = KmlPlus('Point Styling.kml')
 kml_file.linestring(coordinates_list)
 ```
 
 polyhedron(coordinate_list, **kwargs)
 
 Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
 
 ```
-"""
+        """
 
         Args:
-            coordinate_list (list): A list of coordinates
+            lower_coordinate_list: List of coordinates for the lower polygon
+            upper_coordinate_list: List of coordinates for the upper polygon
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
-            lower_layer (float): Height in FT of the lower layer
-            upper_layer (float): Height in FT of the upper layer
             lower_polygon_name (str): Lower polygon object name
             upper_polygon_name (str): Upper polygon object name
+            lower_layer (str): Lower layer z value, default is 0
+            upper_layer (str): Upper layer z value, default is 0
+            lower_layer_uom (str): Lower layer unit of measure, default is M
+            upper_layer_uom (str): Upper layer unit of measure, default is M
             colour_hex (str): String representing a colour hex
             fill (str): 1 or 0, whether or not to fill the polygon
             outline (str): 1 or 0, whether to include outline of polygon
             extrude (str): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
@@ -217,18 +222,21 @@
 ```
 """
 
         Args:
             coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
             radius (float): The radius of the circle
         Keyword Args:
+            z (float): The Z value for the circle. Default is 0.
             fol (str): Name of the folder in which the KML objects are stored.
             name (str): What to name the Circle object
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-               Defaults to 'NM'
+            uom (str): The unit of measurement of z. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
+            radius_uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
             None
 
@@ -240,54 +248,57 @@
 
 cylinder(coordinate_list, radius, **kwargs)
 
 Creates a Cylinder from a single set of coordinates within a list.
 
 ```
 """
+    Args:
+        coordinate_list: A list containing a single set of coordinates representing the centre of the circle
+        radius: The radius of the circle
+    Keyword Args:
+        lower_layer (float): Height/Altitude of the lower layer
+        upper_layer (float): Height/Altitude of the upper layer
+        sample (int): How many points to use when creating the circles which make up the cylinder
+        lower_circle_name (str): Lower circle object name
+        upper_circle_name (str): Upper circle object name
+        radius_uom (str): Radius unit of measure.
+        fol (str): Name of the folder in which the KML objects are stored.
+        uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+          Defaults to 'NM'
+        colour_hex (str): String representing a colour hex
+        fill (str): 1 or 0, whether or not to fill the polygon
+        outline (str): 1 or 0, whether to include outline of polygon
+        altitude_mode (str): Accepts simplekml Altitude mode options
 
-        Args:
-            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
-            radius: The radius of the circle
-        Keyword Args:
-            lower_layer (float): Height/Altitude of the lower layer
-            upper_layer (float): Height/Altitude of the upper layer
-            sample (int): How many points to use when creating the circles which make up the cylinder
-            lower_circle_name (str): Lower circle object name
-            upper_circle_name (str): Upper circle object name
-            fol (str): Name of the folder in which the KML objects are stored.
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-              Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
+    Returns:
+        None
+"""
 
 kml_file = KmlPlus('Point Styling.kml')
 kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
 
 ```
 
 point(coordinate_list, **kwargs)
 
 Creates a single point from a single set of coordinates stored in a list in x, y, z format.
 
 ```
 
-"""
+        """
 
         Args:
-            coordinate_list (list): A list containing a single coordinate
+            coordinate_list (list): A list containing a single coordinate. Z values are to be given
+            in metres (M).
 
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
+            z (float): The Z value for the point. Default is 0.
+            uom (str): The unit of measurement for the Z value. Default is metres (M).
             point_name (str): String to name the point object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
 
         Returns:
```

### Comparing `KMLPlus-3.0.0b4/LICENSE` & `KMLPlus-3.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b4/PKG-INFO` & `KMLPlus-3.0.0b5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,15 +58,15 @@
 Installing
 ----------
 
 ### Pip
 
 ```
 pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus==3.0.0b3 <--- Current v3.0.0-beta.3
+pip install kmlplus==3.0.0b5 <--- Current v3.0.0-beta.5
 ```
 
 ### Clone
 
 ```
 git clone https://github.com/MHenderson1988/kmlplus.git
 
@@ -155,51 +155,56 @@
 linestring(coordinate_list, **kwargs)
 
 The linestring function updates the kml file with a KML linestring feature.
 
 ```
 from kmlplus.kml import KmlPlus
 
-"""
+        """
 
         Args:
             coordinate_list (list): A list containing a single coordinate
         Keyword Args:
+            uom: The unit of measurement for the Z value. Default is metres (M).
+            z (int): The Z value for the point. Default is 0.
             fol (str): A string to name the folder in which the point is stored.
             linestring_name (str): String to name the LineString object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             width(int): Line width
             altitude_mode(str): Accepts simplekml Altitude mode options
 
 
         Returns:
             None
 
-  """
+        """
 
 kml_file = KmlPlus('Point Styling.kml')
 kml_file.linestring(coordinates_list)
 ```
 
 polyhedron(coordinate_list, **kwargs)
 
 Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
 
 ```
-"""
+        """
 
         Args:
-            coordinate_list (list): A list of coordinates
+            lower_coordinate_list: List of coordinates for the lower polygon
+            upper_coordinate_list: List of coordinates for the upper polygon
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
-            lower_layer (float): Height in FT of the lower layer
-            upper_layer (float): Height in FT of the upper layer
             lower_polygon_name (str): Lower polygon object name
             upper_polygon_name (str): Upper polygon object name
+            lower_layer (str): Lower layer z value, default is 0
+            upper_layer (str): Upper layer z value, default is 0
+            lower_layer_uom (str): Lower layer unit of measure, default is M
+            upper_layer_uom (str): Upper layer unit of measure, default is M
             colour_hex (str): String representing a colour hex
             fill (str): 1 or 0, whether or not to fill the polygon
             outline (str): 1 or 0, whether to include outline of polygon
             extrude (str): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
@@ -217,18 +222,21 @@
 ```
 """
 
         Args:
             coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
             radius (float): The radius of the circle
         Keyword Args:
+            z (float): The Z value for the circle. Default is 0.
             fol (str): Name of the folder in which the KML objects are stored.
             name (str): What to name the Circle object
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-               Defaults to 'NM'
+            uom (str): The unit of measurement of z. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
+            radius_uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
             None
 
@@ -240,54 +248,57 @@
 
 cylinder(coordinate_list, radius, **kwargs)
 
 Creates a Cylinder from a single set of coordinates within a list.
 
 ```
 """
+    Args:
+        coordinate_list: A list containing a single set of coordinates representing the centre of the circle
+        radius: The radius of the circle
+    Keyword Args:
+        lower_layer (float): Height/Altitude of the lower layer
+        upper_layer (float): Height/Altitude of the upper layer
+        sample (int): How many points to use when creating the circles which make up the cylinder
+        lower_circle_name (str): Lower circle object name
+        upper_circle_name (str): Upper circle object name
+        radius_uom (str): Radius unit of measure.
+        fol (str): Name of the folder in which the KML objects are stored.
+        uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+          Defaults to 'NM'
+        colour_hex (str): String representing a colour hex
+        fill (str): 1 or 0, whether or not to fill the polygon
+        outline (str): 1 or 0, whether to include outline of polygon
+        altitude_mode (str): Accepts simplekml Altitude mode options
 
-        Args:
-            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
-            radius: The radius of the circle
-        Keyword Args:
-            lower_layer (float): Height/Altitude of the lower layer
-            upper_layer (float): Height/Altitude of the upper layer
-            sample (int): How many points to use when creating the circles which make up the cylinder
-            lower_circle_name (str): Lower circle object name
-            upper_circle_name (str): Upper circle object name
-            fol (str): Name of the folder in which the KML objects are stored.
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-              Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
+    Returns:
+        None
+"""
 
 kml_file = KmlPlus('Point Styling.kml')
 kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
 
 ```
 
 point(coordinate_list, **kwargs)
 
 Creates a single point from a single set of coordinates stored in a list in x, y, z format.
 
 ```
 
-"""
+        """
 
         Args:
-            coordinate_list (list): A list containing a single coordinate
+            coordinate_list (list): A list containing a single coordinate. Z values are to be given
+            in metres (M).
 
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
+            z (float): The Z value for the point. Default is 0.
+            uom (str): The unit of measurement for the Z value. Default is metres (M).
             point_name (str): String to name the point object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
 
         Returns:
```

### Comparing `KMLPlus-3.0.0b4/README.md` & `KMLPlus-3.0.0b5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Installing
 ----------
 
 ### Pip
 
 ```
 pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus==3.0.0b3 <--- Current v3.0.0-beta.3
+pip install kmlplus==3.0.0b5 <--- Current v3.0.0-beta.5
 ```
 
 ### Clone
 
 ```
 git clone https://github.com/MHenderson1988/kmlplus.git
 
@@ -141,51 +141,56 @@
 linestring(coordinate_list, **kwargs)
 
 The linestring function updates the kml file with a KML linestring feature.
 
 ```
 from kmlplus.kml import KmlPlus
 
-"""
+        """
 
         Args:
             coordinate_list (list): A list containing a single coordinate
         Keyword Args:
+            uom: The unit of measurement for the Z value. Default is metres (M).
+            z (int): The Z value for the point. Default is 0.
             fol (str): A string to name the folder in which the point is stored.
             linestring_name (str): String to name the LineString object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             width(int): Line width
             altitude_mode(str): Accepts simplekml Altitude mode options
 
 
         Returns:
             None
 
-  """
+        """
 
 kml_file = KmlPlus('Point Styling.kml')
 kml_file.linestring(coordinates_list)
 ```
 
 polyhedron(coordinate_list, **kwargs)
 
 Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
 
 ```
-"""
+        """
 
         Args:
-            coordinate_list (list): A list of coordinates
+            lower_coordinate_list: List of coordinates for the lower polygon
+            upper_coordinate_list: List of coordinates for the upper polygon
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
-            lower_layer (float): Height in FT of the lower layer
-            upper_layer (float): Height in FT of the upper layer
             lower_polygon_name (str): Lower polygon object name
             upper_polygon_name (str): Upper polygon object name
+            lower_layer (str): Lower layer z value, default is 0
+            upper_layer (str): Upper layer z value, default is 0
+            lower_layer_uom (str): Lower layer unit of measure, default is M
+            upper_layer_uom (str): Upper layer unit of measure, default is M
             colour_hex (str): String representing a colour hex
             fill (str): 1 or 0, whether or not to fill the polygon
             outline (str): 1 or 0, whether to include outline of polygon
             extrude (str): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
@@ -203,18 +208,21 @@
 ```
 """
 
         Args:
             coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
             radius (float): The radius of the circle
         Keyword Args:
+            z (float): The Z value for the circle. Default is 0.
             fol (str): Name of the folder in which the KML objects are stored.
             name (str): What to name the Circle object
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-               Defaults to 'NM'
+            uom (str): The unit of measurement of z. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
+            radius_uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
             None
 
@@ -226,54 +234,57 @@
 
 cylinder(coordinate_list, radius, **kwargs)
 
 Creates a Cylinder from a single set of coordinates within a list.
 
 ```
 """
+    Args:
+        coordinate_list: A list containing a single set of coordinates representing the centre of the circle
+        radius: The radius of the circle
+    Keyword Args:
+        lower_layer (float): Height/Altitude of the lower layer
+        upper_layer (float): Height/Altitude of the upper layer
+        sample (int): How many points to use when creating the circles which make up the cylinder
+        lower_circle_name (str): Lower circle object name
+        upper_circle_name (str): Upper circle object name
+        radius_uom (str): Radius unit of measure.
+        fol (str): Name of the folder in which the KML objects are stored.
+        uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+          Defaults to 'NM'
+        colour_hex (str): String representing a colour hex
+        fill (str): 1 or 0, whether or not to fill the polygon
+        outline (str): 1 or 0, whether to include outline of polygon
+        altitude_mode (str): Accepts simplekml Altitude mode options
 
-        Args:
-            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
-            radius: The radius of the circle
-        Keyword Args:
-            lower_layer (float): Height/Altitude of the lower layer
-            upper_layer (float): Height/Altitude of the upper layer
-            sample (int): How many points to use when creating the circles which make up the cylinder
-            lower_circle_name (str): Lower circle object name
-            upper_circle_name (str): Upper circle object name
-            fol (str): Name of the folder in which the KML objects are stored.
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-              Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
+    Returns:
+        None
+"""
 
 kml_file = KmlPlus('Point Styling.kml')
 kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
 
 ```
 
 point(coordinate_list, **kwargs)
 
 Creates a single point from a single set of coordinates stored in a list in x, y, z format.
 
 ```
 
-"""
+        """
 
         Args:
-            coordinate_list (list): A list containing a single coordinate
+            coordinate_list (list): A list containing a single coordinate. Z values are to be given
+            in metres (M).
 
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
+            z (float): The Z value for the point. Default is 0.
+            uom (str): The unit of measurement for the Z value. Default is metres (M).
             point_name (str): String to name the point object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
 
         Returns:
```

### Comparing `KMLPlus-3.0.0b4/kmlplus/geo.py` & `KMLPlus-3.0.0b5/kmlplus/geo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from typing import Union
 
 from pyproj import Geod
 
+import util
 from kmlplus.interface import ILocation, ILocationFactory, ICurvedSegmentFactory, ICurvedSegment
 from kmlplus.util import dms_to_decimal, detect_coordinate_type, split_segment_string
 
 
 class Point(ILocation):
     """
     A class for representing a coordinate using y, x, z representation.
 
     Attributes:
         y (str): Latitude
         x (str): Longitude
 
     Keyword Args:
         z (float): Elevation
+        uom (str): Unit of measure for elevation. Defaults to Metres
     """
-    __slots__ = ('_y', '_x', '_z')
+    __slots__ = ('_y', '_x', '_z', 'uom')
 
     def __init__(self, y: Union[str, float], x: Union[str, float], **kwargs: Union[str, int, float]):
+        self.uom = kwargs.get('uom', 'M')
         self.y: Union[str, float] = y
         self.x: Union[str, float] = x
         self.z: Union[str, float] = kwargs.get('z', 0.0)
 
     def __str__(self) -> str:
         return f'{self.y} {self.x} {self.z}'
 
@@ -65,15 +68,15 @@
             z (float)
         """
         return self._z
 
     @z.setter
     def z(self, value) -> None:
         if isinstance(value, float):
-            self._z = value
+            self._z = util.convert_to_metres(value, self.uom)
         else:
             if value is None:
                 self._z = 0.0
             else:
                 self.z = float(value)
 
     @classmethod
@@ -85,34 +88,35 @@
 
         Keyword Args:
             z (int | float):
 
         Returns:
             An ILocation object
         """
-        return cls(y, x, z=kwargs.get('z', 0))
+        return cls(y, x, z=kwargs.get('z', 0), uom=kwargs.get('uom', 'M'))
 
     @classmethod
     def from_dms(cls, y: Union[str, float], x: Union[str, float], **kwargs: Union[float, int, str]) -> ILocation:
         """
         Creates a Point object from coordinates in Degrees Minutes Seconds format.
 
         Args:
             y (str, float): Latitude value
             x (str, float): Longitude value
 
         Keyword Args:
             z (str, float): Elevation value
+            uom (str): Unit of measurement for elevation.
 
         Returns:
             An ILocation object
         """
         y = dms_to_decimal(y)
         x = dms_to_decimal(x)
-        return cls(y, x, z=kwargs.pop('z', 0))
+        return cls(y, x, z=kwargs.pop('z', 0.0), uom=kwargs.get('uom', 'M'))
 
     @classmethod
     def find_midpoint(cls, point_1: ILocation, point_2: ILocation, **kwargs: Union[int, float, str]) -> ILocation:
         """
         Args:
             point_1 (Point):
             point_2 (Point):
@@ -126,15 +130,15 @@
         """
         x1, x2 = float(point_1.x), float(point_2.x)
         y1, y2 = float(point_1.y), float(point_2.y)
 
         x = (x1 + x2) / 2
         y = (y1 + y2) / 2
 
-        return cls(y, x, z=kwargs.pop('z', 0))
+        return cls(y, x, z=kwargs.pop('z', 0), uom=kwargs.get('uom', 'M'))
 
     @classmethod
     def from_point_bearing_and_distance(cls, point: ILocation, bearing: float, distance: float, **kwargs) -> ILocation:
         """
         Calculates a new Point based upon the bearing and distance from an existing one.
 
         Args:
@@ -147,15 +151,15 @@
 
         Returns:
             A Point object at the declared bearing and distance from another Point object.
         """
         g = Geod(ellps='WGS84')
         p = g.fwd(point.x, point.y, az=bearing, dist=distance)
 
-        return cls(p[1], p[0], z=kwargs.get('z', 0))
+        return cls(p[1], p[0], z=kwargs.get('z', 0), uom=kwargs.get('uom', 'M'))
 
     def get_distance(self, another_point: ILocation, **kwargs: str) -> float:
         """
         Calculates the distance between two points.
         Args:
             another_point (Point): A Point object.
 
@@ -216,19 +220,20 @@
     Args:
         coordinate_list (list): A list of strings containing coordinates in DMS or DD
 
     Keyword Args:
         z_override: A value with which to override all z values given in the string
     """
 
-    __slots__ = ('_coordinate_list', 'z_override')
+    __slots__ = ('_coordinate_list', 'z_override', 'uom')
 
     def __init__(self, coordinate_list: list, **kwargs):
         self.z_override = kwargs.get('z', None)
         self.coordinate_list = coordinate_list
+        self.uom = kwargs.get('uom', 'M')
 
     @property
     def coordinate_list(self) -> list[str]:
         return self._coordinate_list
 
     @coordinate_list.setter
     def coordinate_list(self, coordinate_list: list[str]) -> None:
@@ -268,15 +273,15 @@
                 point_list += self.create_curved_segment(i)
             else:
                 point_list.append(self.create_new_point(i))
 
         return point_list
 
     def create_curved_segment(self, i: str) -> list[ILocation]:
-        curved_segment_points = CurvedSegmentFactory(i, z_override=self.z_override). \
+        curved_segment_points = CurvedSegmentFactory(i, z_override=self.z_override, uom=self.uom). \
             generate_segment()
 
         return curved_segment_points
 
     def create_new_point(self, i: str) -> ILocation:
         point_obj = self.process_string(i)
         return point_obj
@@ -316,55 +321,56 @@
             split (list[str]): A list containing the split coordinate string
             func (callable): The function to call to process the string
 
         Returns:
             point (ILocation): An ILocation object created from the string.
         """
         if self.z_override is not None:
-            point = func(split[0], split[1], z=self.z_override)
+            point = func(split[0], split[1], z=self.z_override, uom=self.uom)
         else:
-            point = func(split[0], split[1])
+            point = func(split[0], split[1], uom=self.uom)
         return point
 
     def process_x_y_z(self, split: list[str], func: callable) -> ILocation:
         """
         Processes coordinate strings which supply latitude, longitude and elevation values.
         Args:
             split (list[str]): A list containing the split coordinate string
             func (callable): The function to call to process the string
 
         Returns:
             point (ILocation): An ILocation object created from the string.
         """
         if self.z_override is not None:
-            point = func(split[0], split[1], z=self.z_override)
+            point = func(split[0], split[1], z=self.z_override, uom=self.uom)
         else:
             if split[2]:
-                point = func(split[0], split[1], z=split[2])
+                point = func(split[0], split[1], z=split[2], uom=self.uom)
             else:
-                point = func(split[0], split[1], z=0.0)
+                point = func(split[0], split[1], z=0.0, uom=self.uom)
         return point
 
 
 class CurvedSegmentFactory(ICurvedSegmentFactory):
     """
     A factory for creating clockwise and anticlockwise curved segments.
 
     Args:
         coordinate_string (str): A string representing the curved segment
 
     Keyword Args:
         z_override (float|None): Overrides all z values passed within the string.
     """
 
-    __slots__ = ('coordinate_string', 'z_override')
+    __slots__ = ('coordinate_string', 'z_override', 'uom')
 
     def __init__(self, coordinate_string: str, **kwargs: str):
         self.coordinate_string = coordinate_string
         self.z_override = kwargs.get('z_override', None)
+        self.uom = kwargs.get('uom', 'M')
 
     def process_segment(self) -> ICurvedSegment:
         """
         Populates all ILocation values within the segment string.
 
         Returns:
             segment (ICurvedSegment)
@@ -391,55 +397,59 @@
             string_dict (dict): A dict containing start, end and other optional data for the curved segment.
 
         Returns:
             point_list (list[ILocation])
         """
         if string_dict.get('centre') is not None:
             point_list = PointFactory([f"{string_dict['start']}", f"{string_dict['end']}",
-                                       f"{string_dict.get('centre')}"], z=self.z_override).process_coordinates()
+                                       f"{string_dict.get('centre')}"], z=self.z_override,
+                                      uom=self.uom).process_coordinates()
         else:
             point_list = PointFactory([f"{string_dict['start']}", f"{string_dict['end']}"],
-                                      z=self.z_override).process_coordinates()
+                                      z=self.z_override, uom=self.uom).process_coordinates()
         return point_list
 
     def create_clockwise_segment(self, point_list: list, string_dict: dict) -> ICurvedSegment:
         if string_dict.get('centre') is not None:
             segment = ClockwiseCurvedSegment(point_list[0], point_list[1], centre=point_list[2],
-                                             sample=string_dict.get('sample', 100), z=self.z_override)
+                                             sample=string_dict.get('sample', 100), z=self.z_override,
+                                             uom=self.uom)
         else:
             segment = ClockwiseCurvedSegment(point_list[0], point_list[1], sample=string_dict.get('sample', 100),
-                                             z=self.z_override)
+                                             z=self.z_override, uom=self.uom)
         return segment
 
     def create_anticlockwise_segment(self, point_list: list, string_dict: dict) -> ICurvedSegment:
         if string_dict.get('centre') is not None:
             segment = AnticlockwiseCurvedSegment(point_list[0], point_list[1], centre=point_list[2],
-                                                 sample=string_dict.get('sample', 100), z=self.z_override)
+                                                 sample=string_dict.get('sample', 100), z=self.z_override,
+                                                 uom=self.uom)
         else:
             segment = AnticlockwiseCurvedSegment(point_list[0], point_list[1], sample=string_dict.get('sample', 100),
-                                                 z=self.z_override)
+                                                 z=self.z_override, uom=self.uom)
         return segment
 
     def generate_segment(self) -> list[ILocation]:
         segment = self.process_segment()
         segment_points = segment.get_points()
 
         return segment_points
 
 
 class ClockwiseCurvedSegment(ICurvedSegment):
     """
     A class for creating curved segments in a clockwise direction.
     """
-    __slots__ = ('z', '_start', '_end', '_centre', '_sample', 'start_bearing', 'end_bearing')
+    __slots__ = ('z', '_start', '_end', '_centre', '_sample', 'start_bearing', 'end_bearing', 'uom')
 
     def __init__(self, start: ILocation, end: ILocation, **kwargs):
         self.z = kwargs.get('z', None)
         self.start = start
         self.end = end
+        self.uom = kwargs.get('uom', 'M')
         self.centre = kwargs.get('centre', self.find_midpoint())
         self.sample = kwargs.get('sample', 100)
         self.start_bearing = self.find_start_bearing()
         self.end_bearing = self.find_end_bearing()
 
     @property
     def start(self) -> ILocation:
@@ -541,15 +551,16 @@
         distance = self.centre.get_distance(self.start)
         point_list = []
 
         for n in range(0, self.sample + 1):
             if self.z is None:
                 self.z = self.start.z
 
-            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, z=self.z)
+            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, z=self.z,
+                                                              uom=self.uom)
             point_list.append(arc_point)
             start_bearing += bearing_inc
             self.z += height_inc
 
         point_list.append(self.end)
 
         return point_list
@@ -581,20 +592,21 @@
         return difference
 
 
 class AnticlockwiseCurvedSegment(ICurvedSegment):
     """
     Creates an AnticlockwiseCurvedSegment. For documentation, see ClockwiseCurvedSegment.
     """
-    __slots__ = ('z', '_start', '_end', '_centre', '_sample', 'start_bearing', 'end_bearing')
+    __slots__ = ('z', '_start', '_end', '_centre', '_sample', 'start_bearing', 'end_bearing', 'uom')
 
     def __init__(self, start: ILocation, end: ILocation, **kwargs):
         self.start = start
         self.end = end
         self.z = kwargs.pop('z', None)
+        self.uom = kwargs.get('uom', 'M')
         self.centre = kwargs.pop('centre', self.find_midpoint())
         self.sample = kwargs.pop('sample', 100)
         self.start_bearing = self.find_start_bearing()
         self.end_bearing = self.find_end_bearing()
 
     @property
     def start(self) -> ILocation:
@@ -664,15 +676,16 @@
 
         point_list = []
 
         for n in range(0, self.sample + 1):
             if self.z is None:
                 self.z = self.start.z
 
-            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, z=self.z)
+            arc_point = Point.from_point_bearing_and_distance(self.centre, start_bearing, distance, z=self.z,
+                                                              uom=self.uom)
             point_list.append(arc_point)
             start_bearing -= bearing_inc
             self.z += height_inc
 
         point_list.append(self.end)
 
         return point_list
```

### Comparing `KMLPlus-3.0.0b4/kmlplus/interface.py` & `KMLPlus-3.0.0b5/kmlplus/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
     @property
     @abstractmethod
     def sides(self):
         pass
 
     @abstractmethod
-    def create_layer(self, coordinate_list, layer_height):
+    def create_layer(self, coordinate_list, layer_height, layer_uom):
         pass
 
     @abstractmethod
     def generate_sides(self):
         pass
 
     @abstractmethod
```

### Comparing `KMLPlus-3.0.0b4/kmlplus/kml.py` & `KMLPlus-3.0.0b5/kmlplus/kml.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,88 +32,119 @@
 
         Args:
             coordinate_list (list): A list containing a single coordinate. Z values are to be given
             in metres (M).
 
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
+            z (float): The Z value for the point. Default is 0.
+            uom (str): The unit of measurement for the Z value. Default is metres (M).
             point_name (str): String to name the point object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
 
         Returns:
             None
 
         """
-        point = PointFactory(coordinate_list).process_coordinates()
+        if kwargs.get('altitude_mode') == 'relativetoground':
+            altitude_mode = simplekml.AltitudeMode.relativetoground
+        else:
+            altitude_mode = simplekml.AltitudeMode.absolute
+
+        point = PointFactory(coordinate_list, z=kwargs.get('z', 0.0),
+                             uom=kwargs.get('uom', 'M')).process_coordinates()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
 
         pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
         pnt.coords = [(point[0].x, point[0].y, point[0].z)]
         pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
         pnt.extrude = kwargs.get('extrude', 0)
-        pnt.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
+        pnt.altitudemode = altitude_mode
 
         self.kml.save(self.save_name)
 
     def linestring(self, coordinate_list: list, **kwargs: str) -> None:
         """
 
         Args:
             coordinate_list (list): A list containing a single coordinate
         Keyword Args:
+            uom: The unit of measurement for the Z value. Default is metres (M).
+            z (int): The Z value for the point. Default is 0.
             fol (str): A string to name the folder in which the point is stored.
             linestring_name (str): String to name the LineString object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             width(int): Line width
             altitude_mode(str): Accepts simplekml Altitude mode options
 
 
         Returns:
             None
 
         """
-
         fol = self.kml.newfolder(name=kwargs.get('name', 'KmlPlus LineString'))
 
         linestring = LineString(coordinate_list)
 
+        if kwargs.get('altitude_mode') == 'relativetoground':
+            altitude_mode = simplekml.AltitudeMode.relativetoground
+        else:
+            altitude_mode = simplekml.AltitudeMode.absolute
+
         s = fol.newlinestring(name=kwargs.get('linestring_name', 'KmlPlus Linestring'))
         s.coords = [(p.x, p.y, p.z) for p in linestring]
         s.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
         s.extrude = kwargs.get('extrude', 0)
         s.style.linestyle.width = kwargs.get('width', 1)
-        s.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
+        s.altitudemode = altitude_mode
 
         self.kml.save(self.save_name)
 
-    def polyhedron(self, coordinate_list: list, **kwargs: Union[float, str]) -> None:
+    def polyhedron(
+            self,
+            lower_coordinate_list: list,
+            upper_coordinate_list: list,
+            **kwargs: Union[float, str]
+    ) -> None:
         """
 
         Args:
-            coordinate_list (list): A list of coordinates
+            lower_coordinate_list: List of coordinates for the lower polygon
+            upper_coordinate_list: List of coordinates for the upper polygon
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
             lower_polygon_name (str): Lower polygon object name
             upper_polygon_name (str): Upper polygon object name
+            lower_layer (str): Lower layer z value
+            upper_layer (str): Upper layer z value
+            lower_layer_uom (str): Lower layer unit of measure
+            upper_layer_uom (str): Upper layer unit of measure
             colour_hex (str): String representing a colour hex
             fill (str): 1 or 0, whether or not to fill the polygon
             outline (str): 1 or 0, whether to include outline of polygon
             extrude (str): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
             None
         """
-        poly = Polyhedron(coordinate_list, coordinate_list, lower_layer=kwargs.get('lower_layer', None),
-                          upper_layer=kwargs.get('upper_layer', None))
+        poly = Polyhedron(
+            lower_coordinate_list,
+            upper_coordinate_list,
+            lower_layer=kwargs.get('lower_layer', None),
+            upper_layer=kwargs.get('upper_layer', None),
+            lower_layer_uom=kwargs.get('lower_layer_uom', 'FT'),
+            upper_layer_uom=kwargs.get('upper_layer_uom', 'FT')
+        )
+
         lower, upper, sides = poly.to_kml()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Polyhedron'))
 
         if kwargs.get('altitude_mode') == 'relativetoground':
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
@@ -148,18 +179,21 @@
     def circle(self, coordinate_list: list, radius: float, **kwargs: str) -> None:
         """
 
         Args:
             coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
             radius (float): The radius of the circle
         Keyword Args:
+            z (float): The Z value for the circle. Default is 0.
             fol (str): Name of the folder in which the KML objects are stored.
             name (str): What to name the Circle object
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-               Defaults to 'NM'
+            uom (str): The unit of measurement of z. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
+            radius_uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to metres
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
 
         Returns:
             None
 
@@ -187,14 +221,16 @@
 
         Args:
             coordinate_list: A list containing a single set of coordinates representing the centre of the circle
             radius: The radius of the circle
         Keyword Args:
             lower_layer (float): Height/Altitude of the lower layer
             upper_layer (float): Height/Altitude of the upper layer
+            lower_layer_uom (str): The unit of measurement of the lower layer z. Defaults to metres
+            upper_layer_uom (str): The unit of measurement of the upper layer z. Defaults to metres
             sample (int): How many points to use when creating the circles which make up the cylinder
             lower_circle_name (str): Lower circle object name
             upper_circle_name (str): Upper circle object name
             radius_uom (str): Radius unit of measure.
             fol (str): Name of the folder in which the KML objects are stored.
             uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
               Defaults to 'NM'
@@ -207,18 +243,30 @@
             None
         """
         if kwargs.get('altitude_mode') == 'relativetoground':
             altitude_mode = simplekml.AltitudeMode.relativetoground
         else:
             altitude_mode = simplekml.AltitudeMode.absolute
 
-        cylinder = Cylinder((coordinate_list, radius), (coordinate_list, radius),
-                            lower_layer=kwargs.get('lower_layer', None), upper_layer=kwargs.get('upper_layer', None),
-                            sample=kwargs.get('sample', 100), uom=kwargs.get('uom', 'FT'),
-                            radius_uom=kwargs.get('radius_uom', 'M'))
+        cylinder = Cylinder(
+            (
+                coordinate_list,
+                radius
+            ),
+            (
+                coordinate_list,
+                radius
+            ),
+            lower_layer=kwargs.get('lower_layer', None),
+            upper_layer=kwargs.get('upper_layer', None),
+            lower_layer_uom=kwargs.get('lower_layer_uom', 'FT'),
+            upper_layer_uom=kwargs.get('upper_layer_uom', 'FT'),
+            sample=kwargs.get('sample', 100), uom=kwargs.get('uom', 'FT'),
+            radius_uom=kwargs.get('radius_uom', 'M')
+        )
         lower, upper, sides = cylinder.to_kml()
 
         fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Cylinder'))
 
         lower_pol = fol.newpolygon(name=kwargs.get('lower_circle_name', 'KmlPlus Circle'))
         lower_pol.outerboundaryis = lower
         lower_pol.polystyle.color = kwargs.get('colour_hex', '7Fc0c0c0')
```

### Comparing `KMLPlus-3.0.0b4/kmlplus/shapes.py` & `KMLPlus-3.0.0b5/kmlplus/shapes.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
          kilometres ('KM') and nautical miles ('NM')
         uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
     """
     __slots__ = ('_centre', '_radius', 'uom', '_z', '_sample', 'point_list')
 
     def __init__(self, centre: list, radius: float, **kwargs):
-        self.uom: str = kwargs.get('uom', 'FT')
-        self.z: float = convert_to_metres(kwargs.get('z', None), self.uom)
+        self.uom: str = kwargs.get('uom', 'M')
+        self.z: float = kwargs.get('z', None)
         self.sample: int = kwargs.get('sample', 100)
         self.centre: ILocation = self.plot_centre(centre)
         self.radius: float = convert_to_metres(radius, kwargs.get('radius_uom', 'M'))
         self.point_list: list[ILocation] = self.process_points()
 
     def __eq__(self, another_circle: ICircle) -> bool:
         if self.centre and self.radius == another_circle.centre and another_circle.radius:
@@ -116,15 +116,15 @@
 
         Args:
             central_location (list): List with a single string representing x, y, z coordinate
 
         Returns:
             coordinates(ILocation): ILocation object representing the focus of the circle.
         """
-        coordinates = PointFactory(central_location).process_coordinates()[0]
+        coordinates = PointFactory(central_location, uom=self.uom).process_coordinates()[0]
         return coordinates
 
     def process_points(self) -> list[ILocation]:
         """
         Plots and creates each ILocation point of the circle.
 
         Returns:
@@ -136,16 +136,20 @@
         bearing_increment = 360 / self.sample
 
         for n in range(0, self.sample + 1):
             if self.z:
                 z = self.z
             else:
                 z = self.centre.z
+                # Change uom to metres as centre has already been converted. Failure to do so will have further
+                # calculations performed
+                self.uom = 'M'
 
-            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=z)
+            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=z,
+                                                          uom=self.uom)
             point_list.append(point)
             start_bearing -= bearing_increment
 
         return point_list
 
     def to_kml(self) -> list[tuple]:
         """
@@ -156,15 +160,16 @@
         """
         point_list = []
 
         start_bearing = 0
         bearing_increment = 360 / self.sample
 
         for n in range(0, self.sample + 1):
-            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=self.z)
+            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=self.z,
+                                                          uom=self.uom)
             point_list.append(point)
             start_bearing -= bearing_increment
 
         # kml tuples
         circle = [(p.x, p.y, p.z) for p in point_list]
 
         return circle
@@ -180,32 +185,37 @@
 
     Keyword Args:
         radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
          kilometres ('KM') and nautical miles ('NM')
         uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
         lower_radius (float): Overrides any radius in the string for the lower circle.
         upper_radius (float): Overrides any radius in the string for the upper circle.
+        lower_layer (float): Overrides any elevation in the string for the lower circle.
+        upper_layer (float): Overrides any elevation in the string for the upper circle.
+        lower_layer_uom (str): Unit of measure for elevation. Defaults to feet ('FT')
+        upper_layer_uom (str): Unit of measure for elevation. Defaults to feet ('FT')
 
     """
     __slots__ = (
-    'uom', 'sample', 'radius_uom', '_lower_radius', '_upper_radius', '_upper_layer', '_lower_layer', '_sides')
+        'uom', 'sample', 'radius_uom', '_lower_radius', '_upper_radius', '_upper_layer', '_lower_layer', '_sides')
 
     def __init__(self, lower_coordinates: list, upper_coordinates: list, **kwargs):
-        self.uom = kwargs.get('uom', 'FT')
         self.sample = kwargs.get('sample', 100)
         self.radius_uom = kwargs.get('radius_uom', 'M')
         self.lower_radius = lower_coordinates[1]
         self.upper_radius = upper_coordinates[1]
         self.lower_layer = self.create_layer(
             (lower_coordinates[0], self.lower_radius),
-            kwargs.get('lower_layer', None)
+            kwargs.get('lower_layer', None),
+            kwargs.get('lower_layer_uom', 'FT')
         )
         self._upper_layer = self.create_layer(
             (upper_coordinates[0], self.upper_radius),
-            kwargs.get('upper_layer', None)
+            kwargs.get('upper_layer', None),
+            kwargs.get('upper_layer_uom', 'FT')
         )
         self._sides = self.generate_sides()
 
     @property
     def lower_radius(self) -> float:
         return self._lower_radius
 
@@ -283,29 +293,25 @@
             holding_list = []
             for point_list in polygon:
                 holding_list.append((point_list.x, point_list.y, point_list.z))
             sides.append(holding_list)
 
         return lower, upper, sides
 
-    def create_layer(self, coordinate_list: tuple[list[str, float, int]], layer_height) -> ICircle:
+    def create_layer(self, coordinate_list: tuple[list[str, float, int]], layer_height, layer_uom) -> ICircle:
         """
         Creates a 2D circle to act as the top or bottom layer of the cylinder
         Args:
             coordinate_list (tuple[list[str, float, int]]): Contains string information for coordinate and radius
             layer_height: The z value of the layer
 
         Returns:
             circle (ICircle): A circle object
         """
-        if layer_height:
-            circle = Circle(coordinate_list[0], coordinate_list[1], z=layer_height, uom=self.uom,
-                            radius_uom=self.radius_uom)
-        else:
-            circle = Circle(coordinate_list[0], coordinate_list[1], uom=self.uom, radius_uom=self.radius_uom)
+        circle = Circle(coordinate_list[0], coordinate_list[1], z=layer_height, uom=layer_uom)
         return circle
 
     def generate_sides(self) -> list[ICircle]:
         """
         Creates the sides of the cylinder. Requires both layers to contain the same amount of points.
 
         Returns:
@@ -321,15 +327,15 @@
             side_coordinates = []
             i = 0
             while i < len(self.lower_layer) - 1:
                 polygon_coordinate_list = [self.lower_layer.point_list[i].__str__(), self.lower_layer[i + 1].__str__(),
                                            self.upper_layer[i + 1].__str__(), self.upper_layer[i].__str__(),
                                            self.lower_layer[i].__str__()]
 
-                side_coordinates.append(Polygon(polygon_coordinate_list, uom=self.uom))
+                side_coordinates.append(Polygon(polygon_coordinate_list))
 
                 i += 1
 
             return side_coordinates
 
 
 class Polygon(IPolygon, I2DObject):
@@ -342,16 +348,16 @@
     Keyword Args:
         uom (str): Unit of measure for elevation, FT or M
         z (float): Override all string elevation values with a single blanket value.
     """
     __slots__ = ('uom', '_z', '_point_list', 'centroid')
 
     def __init__(self, coordinate_list: list, **kwargs: str):
-        self.uom = kwargs.get('uom', 'FT')
-        self.z = convert_to_metres(kwargs.get('z', None), self.uom)
+        self.uom = kwargs.get('uom', 'M')
+        self.z = kwargs.get('z', None)
         self.point_list = self.process_points(coordinate_list)
         self.centroid = self.calculate_centroid()
 
     def __len__(self) -> int:
         return len(self.point_list)
 
     def __iter__(self):
@@ -415,15 +421,15 @@
         latitude_total, longitude_total = 0, 0
         for coordinate_instance in self.point_list:
             latitude_total += coordinate_instance.y
             longitude_total += coordinate_instance.x
         latitude_average, longitude_average = latitude_total / len(self.point_list), \
                                               longitude_total / len(self.point_list)
 
-        point = Point(latitude_average, longitude_average)
+        point = Point(latitude_average, longitude_average, uom=self.uom, z=self.z)
         return point
 
     def calculate_bearing_from_centroid(self, point: ILocation) -> ILocation:
         """
         Calculates the bearing to the point from the centre of the polygon (Centroid)
 
         Args:
@@ -443,15 +449,16 @@
             point_list (list[str]): A list of coordinate information in string format
 
         Returns:
             points (list[ILocation]): A list of ILocation objects representing the vertices of the polygon
         """
         points = PointFactory(
             point_list,
-            z=self._z
+            z=self._z,
+            uom=self.uom
         ).process_coordinates()
 
         return points
 
 
 class Polyhedron(I3DObject):
     """
@@ -459,22 +466,34 @@
 
     Args:
         lower_coordinates (list[str]): A list of str representation of coordinates.
         upper_coordinates (list[str]): A list of str representation of coordinates.
 
     Keyword Args:
         uom = Unit of measure for elevation, FT or M
+        lower_layer (float): The elevation of the lower layer
+        lower_layer_uom (str): Unit of measure for elevation
+        upper_layer (float): The elevation of the upper layer
+        upper_layer_uom (str): Unit of measure for elevation
+
     """
 
     __slots__ = ('uom', '_lower_layer', '_upper_layer', '_sides')
 
     def __init__(self, lower_coordinates: list[str], upper_coordinates: list[str], **kwargs: str):
-        self.uom = kwargs.get('uom', 'FT')
-        self.lower_layer = self.create_layer(lower_coordinates, kwargs.get('lower_layer', None))
-        self.upper_layer = self.create_layer(upper_coordinates, kwargs.get('upper_layer', None))
+        self.lower_layer = self.create_layer(
+            lower_coordinates,
+            kwargs.get('lower_layer', 0.0),
+            kwargs.get('lower_layer_uom', 'M')
+        )
+        self.upper_layer = self.create_layer(
+            upper_coordinates,
+            kwargs.get('upper_layer', 0.0),
+            kwargs.get('upper_layer_uom', 'M'),
+        )
         self.sides = self.generate_sides()
 
     @property
     def lower_layer(self) -> I2DObject:
         return self._lower_layer
 
     @lower_layer.setter
@@ -499,14 +518,30 @@
     @sides.setter
     def sides(self, sides: list):
         if isinstance(sides, list):
             self._sides = sides
         else:
             raise TypeError('Sides can only be passed in a list')
 
+    def create_layer(self, coordinate_list: list[str], layer_height: str, layer_uom) -> IPolygon:
+        """
+        Creates a layer for the polygon
+        Args:
+            coordinate_list (list): List containing a string of coordinate information
+            layer_height (str): The elevation value of the layer
+
+        Returns:
+
+        """
+        if layer_height:
+            poly = Polygon(coordinate_list, z=layer_height, uom=layer_uom)
+        else:
+            poly = Polygon(coordinate_list)
+        return poly
+
     def to_kml(self) -> tuple:
         """
         Processes the upper, lower layers and sides. Converts their data to a KML friendly format.
 
         Returns:
             lower, upper, sides (tuple):
         """
@@ -518,30 +553,14 @@
             holding_list = []
             for point_list in polygon:
                 holding_list.append((point_list.x, point_list.y, point_list.z))
             sides.append(holding_list)
 
         return lower, upper, sides
 
-    def create_layer(self, coordinate_list: list[str], layer_height: str) -> IPolygon:
-        """
-        Creates a layer for the polygon
-        Args:
-            coordinate_list (list): List containing a string of coordinate information
-            layer_height (str): The elevation value of the layer
-
-        Returns:
-
-        """
-        if layer_height:
-            poly = Polygon(coordinate_list, z=layer_height, uom=self.uom)
-        else:
-            poly = Polygon(coordinate_list)
-        return poly
-
     def generate_sides(self) -> list[IPolygon]:
         """
         Creates the side polygons to connect the upper and lower layers. Requires upper and lower layers to have
         matching amount of vertices
 
         Returns:
             side_coordinates (list[IPolygon]): List of polygons which make up the sides of the polyhedron.
@@ -553,15 +572,15 @@
             side_coordinates = []
             i = 0
             while i < len(self.lower_layer) - 1:
                 polygon_coordinate_list = [self.lower_layer[i].__str__(), self.lower_layer[i + 1].__str__(),
                                            self.upper_layer[i + 1].__str__(), self.upper_layer[i].__str__(),
                                            self.lower_layer[i].__str__()]
 
-                side_polygon = Polygon(polygon_coordinate_list, uom=self.uom)
+                side_polygon = Polygon(polygon_coordinate_list)
 
                 side_coordinates.append(side_polygon)
 
                 i += 1
 
             return side_coordinates
 
@@ -576,16 +595,16 @@
     Keyword Args:
         uom (str): Unit of measure for elevation, FT or M.
     """
 
     __slots__ = ('uom', '_z', 'point_list')
 
     def __init__(self, coordinate_list, **kwargs):
-        self.uom = kwargs.get('uom', 'FT')
-        self.z = convert_to_metres(kwargs.get('z', None), self.uom)
+        self.uom = kwargs.get('uom', 'M')
+        self.z = kwargs.get('z', None)
         self.point_list = self.create(coordinate_list)
 
     def __len__(self):
         return len(self.point_list)
 
     def __iter__(self):
         self.n = 0
@@ -616,9 +635,9 @@
     def z(self, value):
         if value:
             self._z = float(value)
         else:
             self._z = None
 
     def create(self, coordinate_list: list[str]) -> list[ILocation]:
-        point_list = PointFactory(coordinate_list, z=self.z).process_coordinates()
+        point_list = PointFactory(coordinate_list, z=self.z, uom=self.uom).process_coordinates()
         return point_list
```

### Comparing `KMLPlus-3.0.0b4/kmlplus/util.py` & `KMLPlus-3.0.0b5/kmlplus/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,36 +45,33 @@
     calculated_dms_dict = {'degrees': degrees, 'minutes': minutes, 'seconds': seconds,
                            'hemisphere': dms_sliced_dict['hemisphere']}
 
     return calculated_dms_dict
 
 
 def convert_to_metres(a_value, a_uom):
-    if not a_value:
-        return None
+    conversion_dict = {
+        'KM': 1000,
+        'MI': 1609.344,
+        'NM': 1852,
+        'M': 1,
+        'FT': 0.3048
+    }
+
+    regex = '^' + a_uom
+    modifier = None
+    for key, value in conversion_dict.items():
+        if re.match(regex, key, flags=re.IGNORECASE):
+            modifier = value
+
+    if modifier is None:
+        raise TypeError(f'{a_uom} is not an accepted unit of measure. Accepted units of measure are M, MI, KM, FT'
+                        f' and NM')
     else:
-        conversion_dict = {
-            'KM': 1000,
-            'MI': 1609.34,
-            'NM': 1852,
-            'M': 1,
-            'FT': 0.3048
-        }
-
-        regex = '^' + a_uom
-        modifier = None
-        for key, value in conversion_dict.items():
-            if re.match(regex, key, flags=re.IGNORECASE):
-                modifier = value
-
-        if modifier is None:
-            raise TypeError(f'{a_uom} is not an accepted unit of measure. Accepted units of measure are M, MI, KM, FT'
-                            f' and NM')
-        else:
-            return a_value * modifier
+        return round((a_value * modifier), 3)
 
 
 def get_earth_radius(**kwargs) -> float:
     uom_dict = {'km': 6378.14, 'mi': 3963.19, 'nm': 3443.92, 'm': 6378140.00}
     return uom_dict[kwargs.pop('uom', 'km')]
```

### Comparing `KMLPlus-3.0.0b4/setup.py` & `KMLPlus-3.0.0b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="KMLPlus",  # Replace with your own username
-    version="3.0.0-beta.4",
+    version="3.0.0-beta.5",
     author="Mark Henderson",
     author_email="mark.henderson1988@gmail.com",
     description="A Python library for creating 3d floating polygons and circles in .kml for Google Earth.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MHenderson1988/kmlplus",
     packages=setuptools.find_packages(),
```

### Comparing `KMLPlus-3.0.0b4/test/test_geo.py` & `KMLPlus-3.0.0b5/test/test_geo.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,32 @@
 
 
 class TestPoint(TestCase):
     def setUp(self):
         self.test_point_1 = Point.from_dms('551206.00N', '0045206.234W')
         self.test_point_2 = Point.from_dms('501206.00N', '0045206.234W')
         self.test_midpoint = Point.find_midpoint(self.test_point_1, self.test_point_2)
+        self.test_uom_m = Point.from_dms('551206.00N', '0045206.234W', z='383', uom='M')
+        self.test_uom_ft = Point.from_dms('551206.00N', '0045206.234W', z='383', uom='FT')
+        self.test_uom_km = Point.from_dms('551206.00N', '0045206.234W', z='383', uom='KM')
+        self.test_uom_nm = Point.from_dms('551206.00N', '0045206.234W', z='383', uom='NM')
+        self.test_uom_mi = Point.from_dms('551206.00N', '0045206.234W', z='383', uom='MI')
+
+    def test_conversion(self):
+        self.assertEqual(self.test_uom_m.z, 383.0)
+        self.assertEqual(self.test_uom_ft.z, 116.738)
+        self.assertEqual(self.test_uom_km.z, 383000)
+        self.assertEqual(self.test_uom_nm.z, 709316)
+        self.assertEqual(self.test_uom_mi.z, 616378.752)
 
     def test_from_dms(self):
         test_obj = Point.from_dms('551206.00N', '0045206.234W')
         self.assertEqual(test_obj.y, 55.20166666666667)
         self.assertEqual(test_obj.x, -4.868398333333333)
-        self.assertEqual(test_obj.z, 0)
+        self.assertEqual(test_obj.z, 0.0)
 
         test_obj = Point.from_dms('501206.00N', '0045206.234W', z=383, distance_uom='m')
         self.assertEqual(test_obj.y, 50.20166666666667)
         self.assertEqual(test_obj.x, -4.868398333333333)
         self.assertAlmostEqual(test_obj.z, 383.0, delta=5)
 
         test_obj = Point.from_dms('501206.00N', '0045206.234W', z=383, uom='M', distance_uom='m')
@@ -28,20 +40,30 @@
 
     def test_find_midpoint(self):
         mp = Point.find_midpoint(self.test_point_1, self.test_point_2)
         self.assertAlmostEqual(52.701666666667, mp.y, delta=0.0000001)
         self.assertAlmostEqual(-4.8683983333333, mp.x, delta=0.0000001)
 
     def test_from_point_bearing_and_distance(self):
-        test_obj = Point.from_dms('551206.00N', '0045206.23W')
-        test_result = Point.from_point_bearing_and_distance(test_obj, 180.00, 383.00)
+        test_obj_m = Point.from_dms('551206.00N', '0045206.23W', z=383, uom='M')
+        test_obj_km = Point.from_dms('551206.00N', '0045206.23W', z=383, uom='KM')
+        test_obj_ft = Point.from_dms('551206.00N', '0045206.23W', z=383, uom='FT')
+        test_obj_mi = Point.from_dms('551206.00N', '0045206.23W', z=383, uom='MI')
+        test_obj_nm = Point.from_dms('551206.00N', '0045206.23W', z=383, uom='NM')
+        test_result = Point.from_point_bearing_and_distance(test_obj_m, 180.00, 383.00)
 
         self.assertAlmostEqual(55.198333, test_result.y, delta=0.01)
         self.assertAlmostEqual(-4.868333, test_result.x, delta=0.01)
 
+        self.assertEqual(test_obj_m.z, 383)
+        self.assertEqual(test_obj_km.z, 383000)
+        self.assertEqual(test_obj_ft.z, 116.738)
+        self.assertEqual(test_obj_mi.z, 616378.752)
+        self.assertEqual(test_obj_nm.z, 709316)
+
     def test_get_distance(self):
         # test km
         test_obj = Point.from_dms('551206.00N', '0045206.234W')
         distance = test_obj.get_distance(Point.from_dms('501206.00N', '0045206.234W'))
         self.assertEqual(556402.304538113, distance)
 
         # test miles
@@ -74,85 +96,121 @@
 
         inverse_bearing = self.test_midpoint.get_inverse_bearing(self.test_point_1)
         self.assertEqual(180, inverse_bearing)
 
 
 class TestPointFactory(TestCase):
     def setUp(self):
-        self.pf = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'])
+        self.pf_m = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'],
+                                 z=100, uom='M')
+        self.pf_km = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'],
+                                  z=100, uom='KM')
+        self.pf_ft = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'],
+                                  z=100, uom='FT')
+        self.pf_mi = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'],
+                                  z=100, uom='MI')
+        self.pf_nm = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'],
+                                  z=100, uom='NM')
 
     def test_process_coordinates(self):
         # Test that decimal degrees coordinates are correctly returned as decimal degrees.
 
-        test_dd = self.pf.process_coordinates()
+        test_dd = self.pf_m.process_coordinates()
         for i in range(len(test_dd)):
             self.assertTrue(isinstance(test_dd[i], Point))
 
         self.assertEqual(3, len(test_dd))
         self.assertEqual(test_dd[0].y, 22.323232)
         self.assertTrue(isinstance(test_dd[0].y, float))
 
         # Test that dms coordinates are correctly returned as decimal degrees.
-        test_dms = self.pf.process_coordinates()
+        test_dms = self.pf_m.process_coordinates()
         type_result = util.detect_coordinate_type(f'{test_dms[0].y} {test_dms[0].x}')
         self.assertEqual(type_result, 'dd')
 
+        # Test that point lists are returning with correct uom corrections
+        test_m = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'], z=100,
+                              uom='M').process_coordinates()
+        test_km = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'], z=100,
+                               uom='KM').process_coordinates()
+        test_ft = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'], z=100,
+                               uom='FT').process_coordinates()
+        test_mi = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'], z=100,
+                               uom='MI').process_coordinates()
+        test_nm = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'], z=100,
+                               uom='NM').process_coordinates()
+
+        for i in test_m:
+            self.assertEqual(i.z, 100)
+
+        for i in test_km:
+            self.assertEqual(i.z, 100000)
+
+        for i in test_ft:
+            self.assertEqual(i.z, 30.48)
+
+        for i in test_mi:
+            self.assertEqual(i.z, 160934.4)
+
+        for i in test_nm:
+            self.assertEqual(i.z, 185200)
+
     def test_populate_point_list(self):
-        test_point_list = self.pf.populate_point_list()
+        test_point_list = self.pf_m.populate_point_list()
         self.assertNotEqual(test_point_list, None)
         self.assertAlmostEqual(test_point_list[0].y, 22.323232, delta=0.0000001)
         self.assertTrue(isinstance(test_point_list, list))
         self.assertEqual(3, len(test_point_list))
 
     def test_create_curved_segment(self):
-        test_segment = self.pf.create_curved_segment('start=553322N 0043322W, centre=502211N 0043222W, end=510000N '
-                                                     '0040010W, direction=clockwise')
+        test_segment = self.pf_m.create_curved_segment('start=553322N 0043322W, centre=502211N 0043222W, end=510000N '
+                                                       '0040010W, direction=clockwise')
 
         self.assertTrue(isinstance(test_segment, list))
         self.assertEqual(102, len(test_segment))
         for i in test_segment:
             self.assertTrue(isinstance(i, Point))
-            self.assertEqual(0, i.z)
+            self.assertEqual(100, i.z)
 
     def test_process_string(self):
         no_height = '22.323232 -4.287282'
         with_height = '22.323232 -4.287282 8'
 
         dms_test = '521244N 0056555W'
 
-        no_height_obj = self.pf.process_string(no_height)
-        with_height_obj = self.pf.process_string(with_height)
-        dms_obj = self.pf.process_string(dms_test)
+        no_height_obj = self.pf_m.process_string(no_height)
+        with_height_obj = self.pf_m.process_string(with_height)
+        dms_obj = self.pf_m.process_string(dms_test)
 
         self.assertTrue(isinstance(no_height_obj, Point))
         self.assertTrue(isinstance(with_height_obj, Point))
         self.assertTrue(isinstance(dms_obj, Point))
 
-        self.assertEqual(no_height_obj.z, 0.0)
-        self.assertEqual(with_height_obj.z, 8.0)
+        self.assertEqual(no_height_obj.z, 100.0)
+        self.assertEqual(with_height_obj.z, 100.0)
         self.assertEqual(dms_obj.y, 52.21222222222222)
 
     def test_process_x_y(self):
         dd_xy = '22.323232 -4.287282'
         dms_xy = '521244N 0056555W 50'
 
-        dd_xy_obj = self.pf.process_x_y(dd_xy.split(' '), getattr(Point, 'from_decimal_degrees'))
-        dms_xy_obj = self.pf.process_x_y(dms_xy.split(' '), getattr(Point, 'from_dms'))
+        dd_xy_obj = self.pf_m.process_x_y(dd_xy.split(' '), getattr(Point, 'from_decimal_degrees'))
+        dms_xy_obj = self.pf_m.process_x_y(dms_xy.split(' '), getattr(Point, 'from_dms'))
 
         self.assertTrue(isinstance(dd_xy_obj, Point))
         self.assertTrue(isinstance(dms_xy_obj, Point))
-        self.assertEqual(0, dd_xy_obj.z)
-        self.assertEqual(0, dms_xy_obj.z)
+        self.assertEqual(100, dd_xy_obj.z)
+        self.assertEqual(100, dms_xy_obj.z)
 
     def test_process_x_y_z(self):
         with_height = '22.323232 -4.287282 8'
-        dms_xyz_obj = self.pf.process_x_y_z(with_height.split(' '), getattr(Point, 'from_decimal_degrees'))
+        dms_xyz_obj = self.pf_m.process_x_y_z(with_height.split(' '), getattr(Point, 'from_decimal_degrees'))
 
         self.assertTrue(isinstance(dms_xyz_obj, Point))
-        self.assertEqual(8.0, dms_xyz_obj.z)
+        self.assertEqual(100, dms_xyz_obj.z)
 
 
 class TestCurvedSegmentFactory(TestCase):
     def test_process_segment(self):
         c_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=clockwise,' \
                                     ' centre=502211N 0043212W, sample=50').process_segment()
         ac_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=anticlockwise,' \
```

### Comparing `KMLPlus-3.0.0b4/test/test_util.py` & `KMLPlus-3.0.0b5/test/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,23 +101,23 @@
         result = convert_to_metres(1, 'KM')
         self.assertEqual(1000, result)
 
         result = convert_to_metres(1, 'km')
         self.assertEqual(1000, result)
 
         result = convert_to_metres(1, 'mi')
-        self.assertEqual(1609.34, result)
+        self.assertEqual(1609.344, result)
 
         result = convert_to_metres(1, 'nm')
         self.assertEqual(1852, result)
 
         result = convert_to_metres(1, 'm')
         self.assertEqual(1, result)
 
         result = convert_to_metres(1, 'Ft')
-        self.assertEqual(0.3048, result)
+        self.assertEqual(0.305, result)
 
         result = convert_to_metres(1, 'ft')
-        self.assertEqual(0.3048, result)
+        self.assertEqual(0.305, result)
 
         with self.assertRaises(TypeError):
             convert_to_metres(20, 'fdskl;jfdasjkl;adf')
```

