# Comparing `tmp/mapdata-2.5.0.tar.gz` & `tmp/mapdata-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.5.0.tar", last modified: Tue Jun 20 15:30:25 2023, max compression
+gzip compressed data, was "mapdata-2.6.2.tar", last modified: Fri Jun 23 20:38:37 2023, max compression
```

## Comparing `mapdata-2.5.0.tar` & `mapdata-2.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-20 15:30:25.252635 mapdata-2.5.0/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.5.0/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.5.0/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3742 2023-06-20 15:30:25.252635 mapdata-2.5.0/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2544 2023-06-19 13:37:21.000000 mapdata-2.5.0/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-20 15:30:25.252635 mapdata-2.5.0/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   176187 2023-06-20 15:03:06.000000 mapdata-2.5.0/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-20 15:30:25.252635 mapdata-2.5.0/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3742 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-20 15:30:25.252635 mapdata-2.5.0/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-20 15:18:57.000000 mapdata-2.5.0/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-23 20:38:37.462579 mapdata-2.6.2/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.6.2/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.6.2/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-23 20:38:37.462579 mapdata-2.6.2/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2821 2023-06-23 20:29:24.000000 mapdata-2.6.2/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-23 20:38:37.462579 mapdata-2.6.2/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   328306 2023-06-23 20:04:35.000000 mapdata-2.6.2/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-23 20:38:37.462579 mapdata-2.6.2/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-23 20:38:37.462579 mapdata-2.6.2/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-23 20:19:05.000000 mapdata-2.6.2/setup.py
```

### Comparing `mapdata-2.5.0/LICENSE.txt` & `mapdata-2.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.5.0/PKG-INFO` & `mapdata-2.6.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.5.0
+Version: 2.6.2
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -35,15 +35,15 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
-![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png)
+![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png){width=50%}
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
@@ -68,14 +68,19 @@
 
 Data can also be displayed in several different types of plots: box plots, scatter
 plots, line charts, and counts of categorical and quantitative variables.  Plots
 can use either all data or only data values that are selected in the map and
 table.  Plots have a live connection to the data table, so when selections are
 changed the plots are automatically updated.
 
+SQL commands can be used when pulling a data set from a database, to create
+a temporary table, for example, instead of using a base table.  The SQL
+commands can be augmented with [execsql](https://pypi.org/project/execsql/)
+metacommands and substitution variables.
+
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
```

### Comparing `mapdata-2.5.0/README.md` & `mapdata-2.6.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
-![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png)
+![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png){width=50%}
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
@@ -34,14 +34,19 @@
 
 Data can also be displayed in several different types of plots: box plots, scatter
 plots, line charts, and counts of categorical and quantitative variables.  Plots
 can use either all data or only data values that are selected in the map and
 table.  Plots have a live connection to the data table, so when selections are
 changed the plots are automatically updated.
 
+SQL commands can be used when pulling a data set from a database, to create
+a temporary table, for example, instead of using a base table.  The SQL
+commands can be augmented with [execsql](https://pypi.org/project/execsql/)
+metacommands and substitution variables.
+
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
```

### Comparing `mapdata-2.5.0/mapdata.egg-info/PKG-INFO` & `mapdata-2.6.2/mapdata.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.5.0
+Version: 2.6.2
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -35,15 +35,15 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
-![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png)
+![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png){width=50%}
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
@@ -68,14 +68,19 @@
 
 Data can also be displayed in several different types of plots: box plots, scatter
 plots, line charts, and counts of categorical and quantitative variables.  Plots
 can use either all data or only data values that are selected in the map and
 table.  Plots have a live connection to the data table, so when selections are
 changed the plots are automatically updated.
 
+SQL commands can be used when pulling a data set from a database, to create
+a temporary table, for example, instead of using a base table.  The SQL
+commands can be augmented with [execsql](https://pypi.org/project/execsql/)
+metacommands and substitution variables.
+
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
```

### Comparing `mapdata-2.5.0/setup.py` & `mapdata-2.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.5.0',
+	version='2.6.2',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```

