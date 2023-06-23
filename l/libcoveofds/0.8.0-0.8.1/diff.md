# Comparing `tmp/libcoveofds-0.8.0.tar.gz` & `tmp/libcoveofds-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcoveofds-0.8.0.tar", last modified: Thu Jun 15 12:07:14 2023, max compression
+gzip compressed data, was "libcoveofds-0.8.1.tar", last modified: Fri Jun 23 15:27:59 2023, max compression
```

## Comparing `libcoveofds-0.8.0.tar` & `libcoveofds-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.544264 libcoveofds-0.8.0/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       31 2023-06-07 07:23:52.000000 libcoveofds-0.8.0/MANIFEST.in
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-15 12:07:14.544264 libcoveofds-0.8.0/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      837 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/README.rst
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.536264 libcoveofds-0.8.0/libcove2/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-07 07:24:06.000000 libcoveofds-0.8.0/libcove2/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3742 2023-06-07 07:24:06.000000 libcoveofds-0.8.0/libcove2/common.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.540264 libcoveofds-0.8.0/libcoveofds/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/libcoveofds/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      561 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/libcoveofds/additionalfields.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5520 2023-06-13 07:34:18.000000 libcoveofds-0.8.0/libcoveofds/cli.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.540264 libcoveofds-0.8.0/libcoveofds/data/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)   215804 2023-06-15 10:03:03.000000 libcoveofds-0.8.0/libcoveofds/data/schema-0-3-0.json
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    21467 2023-06-13 07:34:18.000000 libcoveofds-0.8.0/libcoveofds/geojson.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2159 2023-05-04 15:08:13.000000 libcoveofds-0.8.0/libcoveofds/jsonschemavalidate.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    35356 2023-02-09 08:10:34.000000 libcoveofds-0.8.0/libcoveofds/python_validate.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1595 2023-06-15 10:03:03.000000 libcoveofds-0.8.0/libcoveofds/schema.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-15 12:07:14.540264 libcoveofds-0.8.0/libcoveofds.egg-info/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      513 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/SOURCES.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/dependency_links.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       52 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/entry_points.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       89 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/requires.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       21 2023-06-15 12:07:14.000000 libcoveofds-0.8.0/libcoveofds.egg-info/top_level.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       61 2023-06-15 12:07:14.544264 libcoveofds-0.8.0/setup.cfg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1075 2023-06-15 12:06:39.000000 libcoveofds-0.8.0/setup.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       31 2023-06-07 07:23:52.000000 libcoveofds-0.8.1/MANIFEST.in
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      837 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/README.rst
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.390739 libcoveofds-0.8.1/libcove2/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-07 07:24:06.000000 libcoveofds-0.8.1/libcove2/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3742 2023-06-07 07:24:06.000000 libcoveofds-0.8.1/libcove2/common.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/libcoveofds/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/libcoveofds/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      561 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/libcoveofds/additionalfields.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5520 2023-06-13 07:34:18.000000 libcoveofds-0.8.1/libcoveofds/cli.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/libcoveofds/data/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)   215464 2023-06-23 15:26:41.000000 libcoveofds-0.8.1/libcoveofds/data/schema-0-3-0.json
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    21467 2023-06-13 07:34:18.000000 libcoveofds-0.8.1/libcoveofds/geojson.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2159 2023-05-04 15:08:13.000000 libcoveofds-0.8.1/libcoveofds/jsonschemavalidate.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    35356 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/libcoveofds/python_validate.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1595 2023-06-15 10:03:03.000000 libcoveofds-0.8.1/libcoveofds/schema.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/libcoveofds.egg-info/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      513 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/SOURCES.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/dependency_links.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       52 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/entry_points.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       89 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/requires.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       21 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/top_level.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       61 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/setup.cfg
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1075 2023-06-23 15:26:41.000000 libcoveofds-0.8.1/setup.py
```

### Comparing `libcoveofds-0.8.0/PKG-INFO` & `libcoveofds-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcoveofds
-Version: 0.8.0
+Version: 0.8.1
 Summary: A data review library
 Home-page: https://github.com/Open-Telecoms-Data/lib-cove-ofds
 Author: Open Data Services
 Author-email: code@opendataservices.coop
 License: UNKNOWN
 Project-URL: Documentation, https://libcoveofds.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues
```

### Comparing `libcoveofds-0.8.0/README.rst` & `libcoveofds-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcove2/common.py` & `libcoveofds-0.8.1/libcove2/common.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcoveofds/additionalfields.py` & `libcoveofds-0.8.1/libcoveofds/additionalfields.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcoveofds/cli.py` & `libcoveofds-0.8.1/libcoveofds/cli.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcoveofds/data/schema-0-3-0.json` & `libcoveofds-0.8.1/libcoveofds/data/schema-0-3-0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993582907316%*

 * *Differences: {"'properties'": "{'networks': {'items': {'properties': {'nodes': {'items': {'properties': "*

 * *                 "{'location': {'additionalProperties': False, delete: ['propertyNames']}}}}, "*

 * *                 "'spans': {'items': {'properties': {'route': {'additionalProperties': False, "*

 * *                 "delete: ['propertyNames']}}}}}, '$defs': {'Node': {'properties': {'location': "*

 * *                 "{'additionalProperties': False, delete: ['propertyNames']}}}, 'Span': "*

 * *                 "{'properties': {'rout […]*

```diff
@@ -870,14 +870,15 @@
                                 "type": "string"
                             }
                         },
                         "title": "Fibre type details",
                         "type": "object"
                     },
                     "Geometry": {
+                        "additionalProperties": false,
                         "description": "A [GeoJSON Geometry object](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1).",
                         "minProperties": 1,
                         "properties": {
                             "coordinates": {
                                 "description": "One or more [GeoJSON positions](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). For geometries of type 'Point', the coordinates member must be a single position. For geometries of type 'LineString' the coordinates member must be an array of positions.\n\nEach position is an array of numbers with two or more elements.  The first two elements are longitude and latitude, or easting and northing, precisely in that order. Longitude and latitude must be expressed using the World Geodetic System 1984 [WGS 84](https://datatracker.ietf.org/doc/html/rfc7946#ref-WGS84) datum in units of decimal degrees. Altitude or elevation may be included as an optional third element and must be expressed as the height in meters above or below the WGS 84 reference ellipsoid\n\nTherefore, geometries of type 'Point' must be a single array, e.g. [longitude, latitude], and geometries of type 'LineString' must be an array of arrays, e.g. [[longitude, latitude], [longitude, latitude]].",
                                 "items": {
                                     "minItems": 1,
@@ -898,17 +899,14 @@
                                     "Point"
                                 ],
                                 "openCodelist": false,
                                 "title": "Type",
                                 "type": "string"
                             }
                         },
-                        "propertyNames": {
-                            "pattern": "^(?!(properties$|^features$))"
-                        },
                         "required": [
                             "type",
                             "coordinates"
                         ],
                         "title": "Geometry",
                         "type": "object"
                     },
@@ -1576,14 +1574,15 @@
                                 },
                                 "minItems": 1,
                                 "title": "International connections",
                                 "type": "array",
                                 "uniqueItems": true
                             },
                             "location": {
+                                "additionalProperties": false,
                                 "description": "A [GeoJSON Geometry object](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1).",
                                 "minProperties": 1,
                                 "properties": {
                                     "coordinates": {
                                         "description": "One or more [GeoJSON positions](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). For geometries of type 'Point', the coordinates member must be a single position. For geometries of type 'LineString' the coordinates member must be an array of positions.\n\nEach position is an array of numbers with two or more elements.  The first two elements are longitude and latitude, or easting and northing, precisely in that order. Longitude and latitude must be expressed using the World Geodetic System 1984 [WGS 84](https://datatracker.ietf.org/doc/html/rfc7946#ref-WGS84) datum in units of decimal degrees. Altitude or elevation may be included as an optional third element and must be expressed as the height in meters above or below the WGS 84 reference ellipsoid\n\nTherefore, geometries of type 'Point' must be a single array, e.g. [longitude, latitude], and geometries of type 'LineString' must be an array of arrays, e.g. [[longitude, latitude], [longitude, latitude]].",
                                         "items": {
                                             "minItems": 1,
@@ -1604,17 +1603,14 @@
                                             "Point"
                                         ],
                                         "openCodelist": false,
                                         "title": "Type",
                                         "type": "string"
                                     }
                                 },
-                                "propertyNames": {
-                                    "pattern": "^(?!(properties$|^features$))"
-                                },
                                 "required": [
                                     "type",
                                     "coordinates"
                                 ],
                                 "title": "Geometry",
                                 "type": "object"
                             },
@@ -2699,14 +2695,15 @@
                                 "$comment": "",
                                 "description": "The date this span was ready to carry traffic. For spans with multiple network providers, the earliest of the dates at which each provider's network was ready to carry traffic on this span.",
                                 "format": "date",
                                 "title": "Ready for service date",
                                 "type": "string"
                             },
                             "route": {
+                                "additionalProperties": false,
                                 "description": "A [GeoJSON Geometry object](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1).",
                                 "minProperties": 1,
                                 "properties": {
                                     "coordinates": {
                                         "description": "One or more [GeoJSON positions](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). For geometries of type 'Point', the coordinates member must be a single position. For geometries of type 'LineString' the coordinates member must be an array of positions.\n\nEach position is an array of numbers with two or more elements.  The first two elements are longitude and latitude, or easting and northing, precisely in that order. Longitude and latitude must be expressed using the World Geodetic System 1984 [WGS 84](https://datatracker.ietf.org/doc/html/rfc7946#ref-WGS84) datum in units of decimal degrees. Altitude or elevation may be included as an optional third element and must be expressed as the height in meters above or below the WGS 84 reference ellipsoid\n\nTherefore, geometries of type 'Point' must be a single array, e.g. [longitude, latitude], and geometries of type 'LineString' must be an array of arrays, e.g. [[longitude, latitude], [longitude, latitude]].",
                                         "items": {
                                             "minItems": 1,
@@ -2727,17 +2724,14 @@
                                             "Point"
                                         ],
                                         "openCodelist": false,
                                         "title": "Type",
                                         "type": "string"
                                     }
                                 },
-                                "propertyNames": {
-                                    "pattern": "^(?!(properties$|^features$))"
-                                },
                                 "required": [
                                     "type",
                                     "coordinates"
                                 ],
                                 "title": "Geometry",
                                 "type": "object"
                             },
@@ -4330,14 +4324,15 @@
                                     },
                                     "minItems": 1,
                                     "title": "International connections",
                                     "type": "array",
                                     "uniqueItems": true
                                 },
                                 "location": {
+                                    "additionalProperties": false,
                                     "description": "In the [JSON publication format](https://open-fibre-data-standard.readthedocs.io/en/latest/reference/publication_formats/json.html), a GeoJSON [Point](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.4) geometry describing the physical location of this node. In the [CSV publication format](https://open-fibre-data-standard.readthedocs.io/en/latest/reference/publication_formats/csv.html), a [well-known text](https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry) POINT geometry.",
                                     "minProperties": 1,
                                     "properties": {
                                         "coordinates": {
                                             "description": "One or more [GeoJSON positions](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). For geometries of type 'Point', the coordinates member must be a single position. For geometries of type 'LineString' the coordinates member must be an array of positions.\n\nEach position is an array of numbers with two or more elements.  The first two elements are longitude and latitude, or easting and northing, precisely in that order. Longitude and latitude must be expressed using the World Geodetic System 1984 [WGS 84](https://datatracker.ietf.org/doc/html/rfc7946#ref-WGS84) datum in units of decimal degrees. Altitude or elevation may be included as an optional third element and must be expressed as the height in meters above or below the WGS 84 reference ellipsoid\n\nTherefore, geometries of type 'Point' must be a single array, e.g. [longitude, latitude], and geometries of type 'LineString' must be an array of arrays, e.g. [[longitude, latitude], [longitude, latitude]].",
                                             "items": {
                                                 "minItems": 1,
@@ -4358,17 +4353,14 @@
                                                 "Point"
                                             ],
                                             "openCodelist": false,
                                             "title": "Type",
                                             "type": "string"
                                         }
                                     },
-                                    "propertyNames": {
-                                        "pattern": "^(?!(properties$|^features$))"
-                                    },
                                     "required": [
                                         "type",
                                         "coordinates"
                                     ],
                                     "title": "Node location",
                                     "type": "object"
                                 },
@@ -5740,14 +5732,15 @@
                                     "$comment": "",
                                     "description": "The date this span was ready to carry traffic. For spans with multiple network providers, the earliest of the dates at which each provider's network was ready to carry traffic on this span.",
                                     "format": "date",
                                     "title": "Ready for service date",
                                     "type": "string"
                                 },
                                 "route": {
+                                    "additionalProperties": false,
                                     "description": "In the [JSON publication format](https://open-fibre-data-standard.readthedocs.io/en/latest/reference/publication_formats/json.html), a GeoJSON [LineString](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.4) geometry describing the route of this span. In the [CSV publication format](https://open-fibre-data-standard.readthedocs.io/en/latest/reference/publication_formats/csv.html), a [well-known text](https://en.wikipedia.org/wiki/Well-known_text_representation_of_geometry) LINESTRING geometry.",
                                     "minProperties": 1,
                                     "properties": {
                                         "coordinates": {
                                             "description": "One or more [GeoJSON positions](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). For geometries of type 'Point', the coordinates member must be a single position. For geometries of type 'LineString' the coordinates member must be an array of positions.\n\nEach position is an array of numbers with two or more elements.  The first two elements are longitude and latitude, or easting and northing, precisely in that order. Longitude and latitude must be expressed using the World Geodetic System 1984 [WGS 84](https://datatracker.ietf.org/doc/html/rfc7946#ref-WGS84) datum in units of decimal degrees. Altitude or elevation may be included as an optional third element and must be expressed as the height in meters above or below the WGS 84 reference ellipsoid\n\nTherefore, geometries of type 'Point' must be a single array, e.g. [longitude, latitude], and geometries of type 'LineString' must be an array of arrays, e.g. [[longitude, latitude], [longitude, latitude]].",
                                             "items": {
                                                 "minItems": 1,
@@ -5768,17 +5761,14 @@
                                                 "Point"
                                             ],
                                             "openCodelist": false,
                                             "title": "Type",
                                             "type": "string"
                                         }
                                     },
-                                    "propertyNames": {
-                                        "pattern": "^(?!(properties$|^features$))"
-                                    },
                                     "required": [
                                         "type",
                                         "coordinates"
                                     ],
                                     "title": "Span route",
                                     "type": "object"
                                 },
```

### Comparing `libcoveofds-0.8.0/libcoveofds/geojson.py` & `libcoveofds-0.8.1/libcoveofds/geojson.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcoveofds/jsonschemavalidate.py` & `libcoveofds-0.8.1/libcoveofds/jsonschemavalidate.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcoveofds/python_validate.py` & `libcoveofds-0.8.1/libcoveofds/python_validate.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcoveofds/schema.py` & `libcoveofds-0.8.1/libcoveofds/schema.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/libcoveofds.egg-info/PKG-INFO` & `libcoveofds-0.8.1/libcoveofds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcoveofds
-Version: 0.8.0
+Version: 0.8.1
 Summary: A data review library
 Home-page: https://github.com/Open-Telecoms-Data/lib-cove-ofds
 Author: Open Data Services
 Author-email: code@opendataservices.coop
 License: UNKNOWN
 Project-URL: Documentation, https://libcoveofds.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues
```

### Comparing `libcoveofds-0.8.0/libcoveofds.egg-info/SOURCES.txt` & `libcoveofds-0.8.1/libcoveofds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.0/setup.py` & `libcoveofds-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="libcoveofds",
-    version="0.8.0",
+    version="0.8.1",
     author="Open Data Services",
     author_email="code@opendataservices.coop",
     url="https://github.com/Open-Telecoms-Data/lib-cove-ofds",
     project_urls={
         "Documentation": "https://libcoveofds.readthedocs.io/en/latest/",
         "Issues": "https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues",
         "Source": "https://github.com/Open-Telecoms-Data/lib-cove-ofds",
```

