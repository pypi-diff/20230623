# Comparing `tmp/centerline-width-0.2.5.tar.gz` & `tmp/centerline-width-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-0.2.5.tar", last modified: Sat Jun  3 01:23:41 2023, max compression
+gzip compressed data, was "dist/centerline-width-0.3.0.tar", last modified: Fri Jun 23 06:25:52 2023, max compression
```

## Comparing `centerline-width-0.2.5.tar` & `centerline-width-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/
--rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:23:41.188273 centerline-width-0.2.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32073 2023-06-03 00:59:35.000000 centerline-width-0.2.5/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-05-25 22:01:48.000000 centerline-width-0.2.5/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    22521 2023-06-03 01:17:56.000000 centerline-width-0.2.5/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    12386 2023-05-26 06:35:11.000000 centerline-width-0.2.5/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.2.5/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)     7460 2023-06-01 21:30:40.000000 centerline-width-0.2.5/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.2.5/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     8687 2023-05-26 06:39:09.000000 centerline-width-0.2.5/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.2.5/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.2.5/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.2.5/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     3397 2023-05-19 19:58:39.000000 centerline-width-0.2.5/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     5221 2023-06-01 22:13:28.000000 centerline-width-0.2.5/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 01:23:41.188273 centerline-width-0.2.5/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    37387 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-03 01:23:41.000000 centerline-width-0.2.5/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-03 01:23:41.188273 centerline-width-0.2.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1813 2023-06-03 01:22:11.000000 centerline-width-0.2.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.216256 centerline-width-0.3.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    41251 2023-06-23 06:25:52.216256 centerline-width-0.3.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    35625 2023-06-23 06:21:40.000000 centerline-width-0.3.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.208256 centerline-width-0.3.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1632 2023-06-23 06:05:21.000000 centerline-width-0.3.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27096 2023-06-23 05:59:37.000000 centerline-width-0.3.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15761 2023-06-23 06:16:11.000000 centerline-width-0.3.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-0.3.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7691 2023-06-22 22:02:51.000000 centerline-width-0.3.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-0.3.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.216256 centerline-width-0.3.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)    14666 2023-06-23 06:16:37.000000 centerline-width-0.3.0/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-0.3.0/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10312 2023-05-26 06:26:00.000000 centerline-width-0.3.0/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-0.3.0/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4107 2023-06-23 05:49:19.000000 centerline-width-0.3.0/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6131 2023-06-23 05:40:55.000000 centerline-width-0.3.0/centerline_width/riverCenterlineClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-23 06:25:52.208256 centerline-width-0.3.0/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    41251 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      700 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      160 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-06-23 06:25:52.000000 centerline-width-0.3.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-23 06:25:52.216256 centerline-width-0.3.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1850 2023-06-23 06:24:04.000000 centerline-width-0.3.0/setup.py
```

### Comparing `centerline-width-0.2.5/PKG-INFO` & `centerline-width-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.5
+Version: 0.3.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.5.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.3.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -22,15 +22,17 @@
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
         	* saveCenterlineCSV()
+        	* saveCenterlineMAT()
         	* centerlineVoronoi
+        	* centerlineEqualDistance 
         	* centerlineEvenlySpaced
         	* centerlineSmoothed
         	* centerlineLength
         	* rightBankLength
         	* leftBankLength
         
         | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
@@ -54,24 +56,24 @@
         ```
         pip install -r requirements.txt
         ```
         Requirements will also be downloaded as part of the pip download
         
         ## Quickstart: centerline-width
         
-        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. So, if starting from Google Earth Pro, two .kml must first be translated to a single .csv file
         
         ```python
         import centerline_width
         centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
         					right_kml="right_bank.kml",
         					text_output_name="river_coordinates_output.txt")
         centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
         ```
-        Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+        Then once the .csv file is created, in order to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
         
         ```python
         river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
         ```
         
         To plot the centerline, run the `plotCenterline()` function from `river_object` created
         ```python
@@ -83,14 +85,16 @@
         
         While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
         ```python
         river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
+        For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
+        
         ## Preprocessing
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
         extractPointsToTextFile(left_kml=None,
@@ -118,15 +122,15 @@
         30.037648 -92.868546 30.119746 -92.907917
         30.037674 -92.868536 30.119721 -92.907909
         30.037702 -92.868533 30.119706 -92.907905
         ```
         
         ### Converted Text File to CSV
         
-        Convert a text file with coordinates for a left and right bank's latitude/longitude to a csv file
+        Convert a text file with coordinates for a left and right bank's latitude and longitude to a csv file with columns for the left bank latitude (llat), left bank longitude (llon), right bank latitude (rlat), right bank longitude (rlon)
         
         ```
         convertColumnsToCSV(text_file=None, flipBankDirection=False)
         ```
         * **[REQUIRED]** text_file (string): File location of the text file to convert
         * [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
@@ -162,47 +166,51 @@
         ### River Object
         First, generate a river object to contain river data and available transformations
         ```
         centerline_width.riverCenterline(csv_data=None,
         				optional_cutoff=None,
         				interpolate_data=False,
         				interpolate_n=5,
-        				interpolate_n_centerpoints=None)
+        				interpolate_n_centerpoints=None,
+        				equal_distance=10)
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
         * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
+        * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
         
         **Solutions for sparse data:**
         
-        `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be changed with the `interpolate_n` option
+        `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
         | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_75.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_200.png) |
         
         **Object (class) useful attributes:**
         
         * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+        * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
         * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
         * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
         
         **Object (class) additional atttributes:**
         
         * river_name (string): name of object, set to the csv_data string
         * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
         * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
+        * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
         * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
         * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
@@ -218,63 +226,89 @@
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longitude coordinates of the centerline based on the left and right banks
         
         **Types of Centerlines**
         
-        There are three types of centerline coordinates formed from the riverbank data. Each are built off of each other and are used to clean and smooth data
+        There are four types of centerline coordinates formed from the riverbank data
         
         - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
+        - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
         - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
         - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
         
         Centerline coordinates are formed by the Voronoi vertices
         ```
         river_object.centerlineVoronoi
         ```
         
-        Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+        Centerline coordinates are formed by Equally Distanced vertices, set by `equal_distance`
+        ```
+        river_object.centerlineEqualDistance
+        ```
+        
+        Centerline coordinates are formed by Evenly Spaced vertices, set by `interpolate_n_centerpoints`
         ```
         river_object.centerlineEvenlySpaced
         ```
         
-        Centerline coordinates are formed from Smoothed Voronoi vertices
+        Centerline coordinates are formed from Smoothed vertices
         ```
         river_object.centerlineSmoothed
         ```
         
         Example:
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
         river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
-        ### Save Centerline Coordinates to a CSV
+        ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude
         
         ```
         saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
         ```
         * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
+        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
-        
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
+        ### Save Centerline Coordinates to a .MAT File
+        Save the centerline coordinates to a .mat file with columns for latitude and longitude
+        
+        ```
+        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
+        ```
+        * **[REQUIRED]** save_to_mat (str): MAT filename, requires a .mat extension
+        * [OPTIONAL] centerline_type (str): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
+        ```
+        Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
+        
         ### Return Length of Centerline
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
@@ -460,26 +494,30 @@
         
         If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
         This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
         
         ### Invalid Smoothed Centerline
-        The smoothed centerline can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
+        The smoothed centerline (`river_object.centerlineSmoothed`) can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
         
         Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
         
         By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polyogon
         
         `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
         
         | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
         
+        For very narrow rivers, this problem can become extreme and pronounced
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_extreme.png)
+        
+        By increasing the interpolation between the centerline points, the smoothed centerlines will be forced within the polygon and reduce the amount of points outside of the polygon. By default, this warning will be thrown if more than 2 points are outside of polygon, so as long as more than 2 points lie outside the polygon, the warning will recommend doubling the amount of centerline points
         
         ### Fix Gaps and Jagged Centerlines
         Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
         Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
         ```python
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
@@ -488,16 +526,17 @@
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
         
         The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
         
         ## Developer Notes: Tech Debt and Bug Fixes
+        * option to turn off verbose (no logs printed)
+        * option to specify Geod type (defaults to pyproj.Geod(ellps='WGS84'))
         * Fix legend overlapping on graph, replace doc_examples that have an overlapping
-        * Verify that smoothing filter option does not produce a line that goes outside of the polygon
         
         ## Citations
         Based on work written in R (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
         
         [Github - CMGO](https://github.com/AntoniusGolly/cmgo)
```

### Comparing `centerline-width-0.2.5/README.md` & `centerline-width-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 	* extractPointsToTextFile()
 	* convertColumnsToCSV()
 * **Find centerline and width of river**
 	* plotCenterline()
 	* plotCenterlineWidth()
 	* riverWidthFromCenterline()
 	* saveCenterlineCSV()
+	* saveCenterlineMAT()
 	* centerlineVoronoi
+	* centerlineEqualDistance 
 	* centerlineEvenlySpaced
 	* centerlineSmoothed
 	* centerlineLength
 	* rightBankLength
 	* leftBankLength
 
 | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
@@ -46,24 +48,24 @@
 ```
 pip install -r requirements.txt
 ```
 Requirements will also be downloaded as part of the pip download
 
 ## Quickstart: centerline-width
 
-The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. So, if starting from Google Earth Pro, two .kml must first be translated to a single .csv file
 
 ```python
 import centerline_width
 centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
 					right_kml="right_bank.kml",
 					text_output_name="river_coordinates_output.txt")
 centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
 ```
-Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+Then once the .csv file is created, in order to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
 
 ```python
 river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
 ```
 
 To plot the centerline, run the `plotCenterline()` function from `river_object` created
 ```python
@@ -75,14 +77,16 @@
 
 While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
 ```python
 river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
 ```
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
 
+For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
+
 ## Preprocessing
 ### Convert KML files to Text File
 
 Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
 
 ```
 extractPointsToTextFile(left_kml=None,
@@ -110,15 +114,15 @@
 30.037648 -92.868546 30.119746 -92.907917
 30.037674 -92.868536 30.119721 -92.907909
 30.037702 -92.868533 30.119706 -92.907905
 ```
 
 ### Converted Text File to CSV
 
-Convert a text file with coordinates for a left and right bank's latitude/longitude to a csv file
+Convert a text file with coordinates for a left and right bank's latitude and longitude to a csv file with columns for the left bank latitude (llat), left bank longitude (llon), right bank latitude (rlat), right bank longitude (rlon)
 
 ```
 convertColumnsToCSV(text_file=None, flipBankDirection=False)
 ```
 * **[REQUIRED]** text_file (string): File location of the text file to convert
 * [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
@@ -154,47 +158,51 @@
 ### River Object
 First, generate a river object to contain river data and available transformations
 ```
 centerline_width.riverCenterline(csv_data=None,
 				optional_cutoff=None,
 				interpolate_data=False,
 				interpolate_n=5,
-				interpolate_n_centerpoints=None)
+				interpolate_n_centerpoints=None,
+				equal_distance=10)
 ```
 * **[REQUIRED]** csv_data (string): File location of the text file to convert
 * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
 * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
 * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
 * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
+* [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
 
 **Solutions for sparse data:**
 
-`interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be changed with the `interpolate_n` option
+`interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
 
 `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
 
 | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_75.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_200.png) |
 
 **Object (class) useful attributes:**
 
 * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+* centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
 * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
 * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
 * centerlineLength (float): Length of the centerline of the river (in km)
 * rightBankLength (float): Length of the right bank of the river (in km)
 * leftBankLength (float): Length of the left bank of the river (in km)
 
 **Object (class) additional atttributes:**
 
 * river_name (string): name of object, set to the csv_data string
 * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
 * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
 * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
+* equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
 * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
 * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
 * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
 * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
 * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
 * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
 * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
@@ -210,63 +218,89 @@
 ```
 
 ### Return Latitude/Longitude Coordinates of Centerline
 Return the latitude/longitude coordinates of the centerline based on the left and right banks
 
 **Types of Centerlines**
 
-There are three types of centerline coordinates formed from the riverbank data. Each are built off of each other and are used to clean and smooth data
+There are four types of centerline coordinates formed from the riverbank data
 
 - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
+- **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
 - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
 - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
 
 Centerline coordinates are formed by the Voronoi vertices
 ```
 river_object.centerlineVoronoi
 ```
 
-Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+Centerline coordinates are formed by Equally Distanced vertices, set by `equal_distance`
+```
+river_object.centerlineEqualDistance
+```
+
+Centerline coordinates are formed by Evenly Spaced vertices, set by `interpolate_n_centerpoints`
 ```
 river_object.centerlineEvenlySpaced
 ```
 
-Centerline coordinates are formed from Smoothed Voronoi vertices
+Centerline coordinates are formed from Smoothed vertices
 ```
 river_object.centerlineSmoothed
 ```
 
 Example:
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
 river_centerline_coordinates = river_object.centerlineVoronoi
 ```
 Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
 
-### Save Centerline Coordinates to a CSV
+### Save Centerline Coordinates to a .CSV File
 Save the centerline coordinates to a csv file with columns for latitude and longitude
 
 ```
 saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
 ```
 * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-* [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+* [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+* [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
+* [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
 ```
-
 Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
 
+### Save Centerline Coordinates to a .MAT File
+Save the centerline coordinates to a .mat file with columns for latitude and longitude
+
+```
+saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
+```
+* **[REQUIRED]** save_to_mat (str): MAT filename, requires a .mat extension
+* [OPTIONAL] centerline_type (str): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+* [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+* [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+
+```python
+import centerline_width
+river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
+```
+Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
+
 ### Return Length of Centerline
 Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
 ```
 river_object.centerlineLength
 ```
 Length returned in kilometers
 ```python
@@ -452,26 +486,30 @@
 
 If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
 
 This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
 
 ### Invalid Smoothed Centerline
-The smoothed centerline can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
+The smoothed centerline (`river_object.centerlineSmoothed`) can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
 
 Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
 
 By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polyogon
 
 `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
 
 | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
 
+For very narrow rivers, this problem can become extreme and pronounced
+![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_extreme.png)
+
+By increasing the interpolation between the centerline points, the smoothed centerlines will be forced within the polygon and reduce the amount of points outside of the polygon. By default, this warning will be thrown if more than 2 points are outside of polygon, so as long as more than 2 points lie outside the polygon, the warning will recommend doubling the amount of centerline points
 
 ### Fix Gaps and Jagged Centerlines
 Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
 ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
 Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
 ```python
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
@@ -480,16 +518,17 @@
 | ------------- | ------------- |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
 | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
 
 The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
 
 ## Developer Notes: Tech Debt and Bug Fixes
+* option to turn off verbose (no logs printed)
+* option to specify Geod type (defaults to pyproj.Geod(ellps='WGS84'))
 * Fix legend overlapping on graph, replace doc_examples that have an overlapping
-* Verify that smoothing filter option does not produce a line that goes outside of the polygon
 
 ## Citations
 Based on work written in R (Golly et al. 2017):
 
 >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
 
 [Github - CMGO](https://github.com/AntoniusGolly/cmgo)
```

### Comparing `centerline-width-0.2.5/centerline_width/__init__.py` & `centerline-width-0.3.0/centerline_width/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,28 @@
 # riverObject.py function calls
 from .riverCenterlineClass import riverCenterline
 
 # centerline.py function calls
 from .centerline import centerlinePath
 from .centerline import networkXGraphShortestPath
 from .centerline import centerlineLength
+from .centerline import equalDistanceCenterline
 from .centerline import evenlySpacedCenterline
 from .centerline import smoothedCoordinates
 from .centerline import riverWidthFromCenterlineCoordinates
 from .centerline import riverWidthFromCenterline
 from .centerline import saveCenterlineCSV
+from .centerline import saveCenterlineMAT
 
 # plotDiagrams.py function calls
 from .plotDiagrams import plotCenterline
 from .plotDiagrams import plotCenterlineWidth
 
 # error_handling.py function calls
 from .error_handling import errrorHandlingConvertColumnsToCSV
 from .error_handling import errorHandlingPlotCenterline
 from .error_handling import errorHandlingPlotCenterlineWidth
 from .error_handling import errorHandlingRiverWidthFromCenterline
 from .error_handling import errorHandlingSaveCenterlineCSV
+from .error_handling import errorHandlingSaveCenterlineMAT
 from .error_handling import errorHandlingExtractPointsToTextFile
 from .error_handling import errorHandlingRiverCenterlineClass
```

### Comparing `centerline-width-0.2.5/centerline_width/centerline.py` & `centerline-width-0.3.0/centerline_width/centerline.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import csv
 
 # External Python libraries (installed via pip install)
 from haversine import haversine
 import numpy as np
 import networkx as nx
 from scipy import interpolate
+from scipy.io import savemat
 from shapely.geometry import Point, LineString
+import pyproj
+import geopy.distance
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
@@ -52,15 +55,15 @@
 def networkXGraphShortestPath(nx_graph, starting_node, ending_node):
 	# Find the shortest path if it exists
 	if starting_node is not None:
 		try:
 			shortest_path = nx.shortest_path(nx_graph, source=starting_node, target=ending_node)
 			logger.info("[SUCCESS] Valid centerline path found")
 		except nx.NetworkXNoPath: # no direct path found
-			logger.info("[FAILED]  No direct path found from starting node to ending node")
+			logger.info("[FAILED]  No direct path found from starting node to ending node. To view gaps, plotCenterline(display_all_possible_paths=True). Recommended fix, rerun riverCenterline: set interpolate_data=True or (if interpolate_data=True) increase interpolate_n")
 			return None
 		#nx.draw(graph_connections, with_labels=True, font_size=10)
 		return shortest_path
 	else:
 		return None
 
 def centerlinePath(river_voronoi, river_polygon, top_polygon_line, bottom_polygon_line):
@@ -106,14 +109,49 @@
 		logger.critical("\nCRITICAL ERROR, Polygon too short for the Voronoi diagram generated (no starting node found), unable to plot centerline. Set displayVoronoi=True to view vertices. Can typically be fixed by adding more data to expand range.")
 		shortest_path_points = None
 	else:
 		shortest_path_points = networkXGraphShortestPath(nx_graphs, starting_node, ending_node)
 
 	return starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_points
 
+def equalDistanceCenterline(centerline_coordinates=None, equal_distance=None):
+	# Interpolate centerline to space out coordinates an equal physical distance from the next (in meters)
+	if centerline_coordinates is None:
+		return None
+
+	centerline_line = LineString(centerline_coordinates)
+	equal_distance_between_centerline_coordinates=[]
+
+	geodesic = pyproj.Geod(ellps='WGS84')
+
+	# Iterate through coordinates based on a set distance (distance_m)
+	lon_start, lat_start = centerline_coordinates[0]
+	equal_distance_between_centerline_coordinates.append((lon_start, lat_start))
+	for i, centerline_coord in enumerate(centerline_coordinates):
+		if i+1 < len(centerline_coordinates):
+			lon_end, lat_end = centerline_coordinates[i+1]
+			# move to next point when distance between points is less than the equal distance
+			move_to_next_point = False 
+			while (not move_to_next_point):
+				# forward_bearing: direction towards the next point
+				forward_bearing, reverse_bearing, distance_between_meters = geodesic.inv(lon_start, lat_start, lon_end, lat_end)
+				if distance_between_meters < equal_distance:
+					# if the distance to the next point is less than the equal distance, reorient to bearing to next latitude
+					move_to_next_point = True
+				else:
+					start_point = geopy.Point(lat_start, lon_start)
+					distance_to_move = geopy.distance.distance(kilometers=equal_distance/1000) # distance to move towards the next point
+					final_position = distance_to_move.destination(start_point, bearing=forward_bearing)
+					equal_distance_between_centerline_coordinates.append((final_position.longitude, final_position.latitude))
+					# set new starting point to current newly generated destination
+					lon_start = final_position.longitude
+					lat_start = final_position.latitude
+
+	return equal_distance_between_centerline_coordinates
+
 def evenlySpacedCenterline(centerline_coordinates=None, number_of_fixed_points=None):
 	# Interpolate to evenly space points along the centerline coordinates (effectively smoothing with fewer points)
 	if centerline_coordinates is None:
 		return None
 
 	centerline_line = LineString(centerline_coordinates)
 
@@ -381,21 +419,70 @@
 		else:
 			lon1, lon2 = previous_pair[0], xy_pair[0]
 			lat1, lat2 = previous_pair[1], xy_pair[1]
 			distance_to_add = haversine((lat1, lon1), (lat2, lon2), unit="km")
 			total_length += distance_to_add
 	return total_length
 
-def saveCenterlineCSV(river_object=None, save_to_csv=None, centerline_type="Voronoi"):
-	# Save Centerline Coordinates generated by Voronoi Diagram to CSV
-	centerline_width.errorHandlingSaveCenterlineCSV(river_object=river_object, save_to_csv=save_to_csv, centerline_type=centerline_type)
+def saveCenterlineCSV(river_object=None, save_to_csv=None, latitude_header=None, longitude_header=None, centerline_type="Voronoi"):
+	# Save Centerline Coordinates generated by Voronoi Diagram to .CSV
+	centerline_width.errorHandlingSaveCenterlineCSV(river_object=river_object,
+													save_to_csv=save_to_csv, 
+													latitude_header=latitude_header,
+													longitude_header=longitude_header,
+													centerline_type=centerline_type)
 	centerline_type = centerline_type.title()
 
 	if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
+	if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
 	if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
 	if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
 
+	if latitude_header is None:
+		latitude_header = "{0} Centerline Latitude (Deg)".format(centerline_type)
+	if longitude_header is None:
+		longitude_header = "{0} Centerline Longitude (Deg)".format(centerline_type)
+
 	with open(save_to_csv, "w") as csv_file_output:
 		writer = csv.writer(csv_file_output)
-		writer.writerow(["{0} Centerline Latitude (Deg)".format(centerline_type), "{0} Centerline Longitude (Deg)".format(centerline_type)])
+		writer.writerow([latitude_header, longitude_header])
+		if centerline_coordinates_by_type is not None:
+			for latitude_longitude in centerline_coordinates_by_type:
+				writer.writerow([latitude_longitude[1], latitude_longitude[0]])
+		else:
+			logger.warn("\nWARNING, no {0} centerline coordinates found, {1} file generated will be empty".format(centerline_type, save_to_csv))
+
+def saveCenterlineMAT(river_object=None, save_to_mat=None, latitude_header=None, longitude_header=None, centerline_type="Voronoi"):
+	# Save Centerline Coordinates generated by Voronoi Diagram to .MAT
+	centerline_width.errorHandlingSaveCenterlineMAT(river_object=river_object,
+													save_to_mat=save_to_mat, 
+													latitude_header=latitude_header,
+													longitude_header=longitude_header,
+													centerline_type=centerline_type)
+	centerline_type = centerline_type.title()
+
+	if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
+	if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
+	if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+	if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
+
+	# .mat files do not allow for spaces or special characters in the header
+	if latitude_header is None:
+		latitude_header = "{0}_Centerline_Latitude_Deg".format(centerline_type.replace(" ", "_"))
+	if longitude_header is None:
+		longitude_header = "{0}_Centerline_Longitude_Deg".format(centerline_type.replace(" ", "_"))
+
+	latitude_lst = []
+	longtiude_lst = []
+
+	if centerline_coordinates_by_type is not None:
 		for latitude_longitude in centerline_coordinates_by_type:
-			writer.writerow([latitude_longitude[1], latitude_longitude[0]])
+			longtiude_lst.append(latitude_longitude[0])
+			latitude_lst.append(latitude_longitude[1])
+	else:
+		logger.warn("\nWARNING, no {0} centerline coordinates found, {1} file generated will be empty".format(centerline_type, save_to_mat))
+	
+	# Centerline dictionary of latitude and longtiude centerline coordinates
+	centerline_dict = {latitude_header: np.asarray(latitude_lst), longitude_header: np.asarray(longtiude_lst)}
+
+	# Save to matlab format (.mat)
+	savemat(save_to_mat, mdict=centerline_dict)
```

### Comparing `centerline-width-0.2.5/centerline_width/error_handling.py` & `centerline-width-0.3.0/centerline_width/error_handling.py`

 * *Files 22% similar despite different names*

```diff
@@ -162,37 +162,92 @@
 		if type(save_to_csv) != str:
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
 			exit()
 		if not save_to_csv.lower().endswith(".csv"):
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = '{0}'".format(save_to_csv.split(".")[1]))
 			exit()
 
-def errorHandlingSaveCenterlineCSV(river_object=None, save_to_csv=None, centerline_type=None):
+def errorHandlingSaveCenterlineCSV(river_object=None, latitude_header=None, longitude_header=None, save_to_csv=None, centerline_type=None):
 	# Error Handling for saveCenterlineCSV()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
 			exit()
 
+	if latitude_header is not None and type(latitude_header) != str:
+		logger.critical("\nCRITICAL ERROR, [latitude_header]: Must be a str, current type = '{0}'".format(type(latitude_header)))
+		exit()
+
+	if longitude_header is not None and type(longitude_header) != str:
+		logger.critical("\nCRITICAL ERROR, [longitude_header]: Must be a str, current type = '{0}'".format(type(longitude_header)))
+		exit()
+
 	if save_to_csv is None:
 		logger.critical("\nCRITICAL ERROR, [save_to_csv]: Requires csv filename")
 		exit()
 	else:
 		if type(save_to_csv) != str:
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
 			exit()
 		else:
 			if not save_to_csv.lower().endswith(".csv"):
 				logger.critical("\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = '{0}'".format(save_to_csv.split(".")[1]))
 				exit()
 
-	centerline_type_options = ["Voronoi", "Evenly Spaced", "Smoothed"]
+	centerline_type_options = ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"]
+	if type(centerline_type) != str:
+		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
+		exit()
+	else:
+		if centerline_type.title() not in centerline_type_options:
+			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
+			exit()
+
+def errorHandlingSaveCenterlineMAT(river_object=None, latitude_header=None, longitude_header=None, save_to_mat=None, centerline_type=None):
+	# Error Handling for saveCenterlineMAT()
+	if river_object is None:
+		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
+		exit()
+	else:
+		if not isinstance(river_object, centerline_width.riverCenterline):
+			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
+			exit()
+
+	if latitude_header is not None:
+		if type(latitude_header) != str:
+			logger.critical("\nCRITICAL ERROR, [latitude_header]: Must be a str, current type = '{0}'".format(type(latitude_header)))
+			exit()
+		if any(not character.isalnum() for character in latitude_header):
+			logger.critical("\nCRITICAL ERROR, [latitude_header]: Column names cannot contain any whitespace or non-alphanumeric characters, currently = '{0}'".format(latitude_header))
+			exit()
+
+	if longitude_header is not None:
+		if type(longitude_header) != str:
+			logger.critical("\nCRITICAL ERROR, [longitude_header]: Must be a str, current type = '{0}'".format(type(longitude_header)))
+			exit()
+		if any(not character.isalnum() for character in longitude_header):
+			logger.critical("\nCRITICAL ERROR, [longitude_header]: Column names cannot contain any whitespace or non-alphanumeric characters, currently = '{0}'".format(longitude_header))
+			exit()
+
+	if save_to_mat is None:
+		logger.critical("\nCRITICAL ERROR, [save_to_mat]: Requires mat filename")
+		exit()
+	else:
+		if type(save_to_mat) != str:
+			logger.critical("\nCRITICAL ERROR, [save_to_mat]: Must be a str, current type = '{0}'".format(type(save_to_mat)))
+			exit()
+		else:
+			if not save_to_mat.lower().endswith(".mat"):
+				logger.critical("\nCRITICAL ERROR, [save_to_mat]: Extension must be a .mat file, current extension = '{0}'".format(save_to_mat.split(".")[1]))
+				exit()
+
+	centerline_type_options = ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"]
 	if type(centerline_type) != str:
 		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
 		exit()
 	else:
 		if centerline_type.title() not in centerline_type_options:
 			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
 			exit()
@@ -235,15 +290,16 @@
 			exit()
 
 ## Error Handling: riverCenterlineClass.py
 def errorHandlingRiverCenterlineClass(csv_data=None,
 									optional_cutoff=None,
 									interpolate_data=None,
 									interpolate_n=None,
-									interpolate_n_centerpoints=None):
+									interpolate_n_centerpoints=None,
+									equal_distance=None):
 	# Error Handling for riverCenterlineClass()
 	if csv_data is None:
 		logger.critical("\nCRITICAL ERROR, [csv_data]: Requires csv_data location")
 		exit()
 	else:
 		if type(csv_data) != str and not isinstance(csv_data, StringIO): 
 			# StringIO accounts for testing against a StringIO instead of a CSV (used in pytests)
@@ -269,7 +325,14 @@
 		if type(interpolate_n_centerpoints) != int:
 			logger.critical("\nCRITICAL ERROR, [interpolate_n_centerpoints]: Must be a int, current type = '{0}'".format(type(interpolate_n_centerpoints)))
 			exit()
 		else:
 			if interpolate_n_centerpoints < 2:
 				logger.critical("\nCRITICAL ERROR, [interpolate_n_centerpoints]: Must be a greater than 1, currently = '{0}'".format(interpolate_n_centerpoints))
 				exit()
+
+	if type(equal_distance) != int and type(equal_distance) != float:
+		logger.critical("\nCRITICAL ERROR, [equal_distance]: Must be a int or float, current type = '{0}'".format(type(equal_distance)))
+		exit()
+		if equal_distance <= 0:
+			logger.critical("WARNING, [equal_distance]: Must be a postive value, greater than 0, currently = '{0}'".format(equal_distance))
+			exit()
```

### Comparing `centerline-width-0.2.5/centerline_width/getCoordinatesKML.py` & `centerline-width-0.3.0/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.5/centerline_width/plotDiagrams.py` & `centerline-width-0.3.0/centerline_width/plotDiagrams.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,25 +67,33 @@
 	# Plot Centerline of River
 	centerline_width.errorHandlingPlotCenterline(river_object=river_object,
 												display_all_possible_paths=display_all_possible_paths,
 												plot_title=plot_title,
 												save_plot_name=save_plot_name,
 												display_voronoi=display_voronoi)
 
-	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object)
+	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, display_true_centerline=True)
 
 	# Display the Voronoi Diagram
 	if display_voronoi:
 		voronoi_plot_2d(river_object.bank_voronoi, show_points=True, point_size=1, ax=ax)
 
 	# Plot all possible paths with text for positions
 	if display_all_possible_paths:
 		for i in range(len(river_object.x_voronoi_ridge_point)):
 			plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1)
 
+	# Plot Equally Spaced Points
+	x = []
+	y = []
+	for k, v in river_object.centerlineEqualDistance:
+			x.append(k)
+			y.append(v)
+	#plt.scatter(x, y, c="darkorchid", label="Equal Distance Centerline Coordinates", s=8)
+
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Coordinates: Valid Centerline = {0}, Valid Polygon = {1}, Interpolated = {2}".format(valid_path_through, river_object.bank_polygon.is_valid, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 	plt.xlabel("Longitude (°)")
 	plt.ylabel("Latitude (°)")
@@ -109,16 +117,14 @@
 													transect_span_distance=transect_span_distance,
 													apply_smoothing=apply_smoothing,
 													flag_intersections=flag_intersections,
 													remove_intersections=remove_intersections)
 
 	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, display_true_centerline=display_true_centerline)
 
-	# Plot river
-
 	# Determine the Width of River
 	number_of_evenly_spaced_points = ""
 
 	if river_object.centerlineVoronoi is not None:
 		number_of_evenly_spaced_points = "\nCenterline made of {0} Fixed Points, width lines generated every {1} points".format(river_object.interpolate_n_centerpoints, transect_span_distance)
 		if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
 			if apply_smoothing:
```

### Comparing `centerline-width-0.2.5/centerline_width/preprocessing.py` & `centerline-width-0.3.0/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.5/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-0.3.0/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.5/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-0.3.0/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.5/centerline_width/pytests/test_preprocessing.py` & `centerline-width-0.3.0/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.5/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-0.3.0/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 						("testing_string", "<class 'str'>")]
 
 invalid_non_int_options = [("testing_string", "<class 'str'>"),
 						(3.1415, "<class 'float'>"),
 						([], "<class 'list'>"),
 						(False, "<class 'bool'>")]
 
+invalid_non_num_options = [("testing_string", "<class 'str'>"),
+						([], "<class 'list'>"),
+						(False, "<class 'bool'>")]
+
 invalid_non_str_options = [(1961, "<class 'int'>"),
 						(3.1415, "<class 'float'>"),
 						([], "<class 'list'>"),
 						(False, "<class 'bool'>")]
 
 ## class riverCenterline #####################################################
 def test_riverCenterline_csvDataRequired(caplog):
@@ -59,7 +63,15 @@
 @pytest.mark.parametrize("interpolate_n_invalid, interpolate_n_error_output", invalid_non_int_options)
 def test_riverCenterline_interpolateNInvalidTypes(caplog, interpolate_n_invalid, interpolate_n_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.riverCenterline(csv_data="csv_example.csv", interpolate_n=interpolate_n_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [interpolate_n]: Must be a int, current type = '{0}'".format(interpolate_n_error_output)
+
+@pytest.mark.parametrize("equal_distance_invalid, equal_distance_error_output", invalid_non_num_options)
+def test_riverCenterline_equalDistanceInvalidTypes(caplog, equal_distance_invalid, equal_distance_error_output):
+	with pytest.raises(SystemExit):
+		centerline_width.riverCenterline(csv_data="csv_example.csv", equal_distance=equal_distance_invalid)
+	log_record = caplog.records[0]
+	assert log_record.levelno == logging.CRITICAL
+	assert log_record.message == "\nCRITICAL ERROR, [equal_distance]: Must be a int or float, current type = '{0}'".format(equal_distance_error_output)
```

### Comparing `centerline-width-0.2.5/centerline_width/riverCenterlineClass.py` & `centerline-width-0.3.0/centerline_width/riverCenterlineClass.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,27 @@
 # External Python libraries (installed via pip install)
 import pandas as pd
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
 
 class riverCenterline:
-	def __init__(self, csv_data=None, optional_cutoff=None, interpolate_data=False, interpolate_n=5, interpolate_n_centerpoints=None):
+	def __init__(self,
+				csv_data=None,
+				optional_cutoff=None,
+				interpolate_data=False,
+				interpolate_n=5,
+				interpolate_n_centerpoints=None, 
+				equal_distance=10):
 		centerline_width.errorHandlingRiverCenterlineClass(csv_data=csv_data,
 															optional_cutoff=optional_cutoff,
 															interpolate_data=interpolate_data,
 															interpolate_n=interpolate_n,
-															interpolate_n_centerpoints=interpolate_n_centerpoints)
+															interpolate_n_centerpoints=interpolate_n_centerpoints,
+															equal_distance=equal_distance)
 
 		# Description and dataframe
 		self.river_name = csv_data
 		self.interpolate_data = interpolate_data
 		self.interpolate_n = interpolate_n
 		df = pd.read_csv(csv_data)
 		if optional_cutoff:
@@ -28,14 +35,18 @@
 		# Left and Right Coordinates from the given csv data and data cutoff
 		left_bank_coordinates, right_bank_coordinates = centerline_width.leftRightCoordinates(df)
 		if interpolate_data:
 			right_bank_coordinates, left_bank_coordinates = centerline_width.interpolateBetweenPoints(left_bank_coordinates, right_bank_coordinates, interpolate_n)
 		self.left_bank_coordinates = left_bank_coordinates
 		self.right_bank_coordinates = right_bank_coordinates
 
+		# Right/Length Bank Length
+		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates)
+		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates)
+
 		# River polygon, position of the top/bottom polygon
 		river_bank_polygon, top_bank, bottom_bank = centerline_width.generatePolygon(self.left_bank_coordinates, self.right_bank_coordinates)
 		self.bank_polygon = river_bank_polygon
 		self.top_bank = top_bank
 		self.bottom_bank = bottom_bank
 
 		# Voronoi generated by left/right bank coordinates
@@ -45,27 +56,30 @@
 		# All possible paths: starting/ending node, all possible paths (ridges), paths dictionary
 		starting_node, ending_node, x_ridge_point, y_ridge_point, shortest_path_coordinates = centerline_width.centerlinePath(self.bank_voronoi, self.bank_polygon, self.top_bank, self.bottom_bank)
 		self.starting_node = starting_node # starting position for centerline
 		self.ending_node = ending_node # ending position for centerline
 		self.x_voronoi_ridge_point = x_ridge_point # Voronoi x positions
 		self.y_voronoi_ridge_point = y_ridge_point # Voronoi y postions
 
-		# Centerline coordinates
+		# Voronoi Centerline Coordinates
 		self.centerlineVoronoi = shortest_path_coordinates
+
+		# Centerline length
+		self.centerlineLength = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates)
+		self.equal_distance = equal_distance
+
+		# The different types of Centerline coordinates
+		self.centerlineEqualDistance = centerline_width.equalDistanceCenterline(centerline_coordinates=self.centerlineVoronoi,
+																				equal_distance=self.equal_distance)
 		self.centerlineEvenlySpaced = centerline_width.evenlySpacedCenterline(centerline_coordinates=self.centerlineVoronoi,
-																						number_of_fixed_points=self.interpolate_n_centerpoints)
+																				number_of_fixed_points=self.interpolate_n_centerpoints)
 		self.centerlineSmoothed = centerline_width.smoothedCoordinates(river_object=self, centerline_coordinates=self.centerlineEvenlySpaced,
-																						interprolate_num=self.interpolate_n_centerpoints)
+																		interprolate_num=self.interpolate_n_centerpoints)
 
-		# Right/Length Bank Length
-		self.rightBankLength = centerline_width.centerlineLength(centerline_coordinates=right_bank_coordinates)
-		self.leftBankLength = centerline_width.centerlineLength(centerline_coordinates=left_bank_coordinates)
 
-		# Centerline length
-		self.centerlineLength = centerline_width.centerlineLength(centerline_coordinates=shortest_path_coordinates)
 
 	def plotCenterline(self,
 						display_all_possible_paths=False,
 						plot_title=None,
 						save_plot_name=None,
 						display_voronoi=False):
 		centerline_width.plotCenterline(river_object=self,
@@ -100,11 +114,28 @@
 		return centerline_width.riverWidthFromCenterline(river_object=self,
 														transect_span_distance=transect_span_distance,
 														apply_smoothing=apply_smoothing,
 														remove_intersections=remove_intersections,
 														units=units,
 														save_to_csv=save_to_csv)
 
-	def saveCenterlineCSV(self, save_to_csv=None, centerline_type="Voronoi"):
+	def saveCenterlineCSV(self, 
+						save_to_csv=None,
+						latitude_header=None,
+						longitude_header=None, 
+						centerline_type="Voronoi"):
 		return centerline_width.saveCenterlineCSV(river_object=self,
 												save_to_csv=save_to_csv,
+												latitude_header=latitude_header, 
+												longitude_header=longitude_header, 
+												centerline_type=centerline_type)
+
+	def saveCenterlineMAT(self,
+						save_to_mat=None, 
+						latitude_header=None,
+						longitude_header=None, 
+						centerline_type="Voronoi"):
+		return centerline_width.saveCenterlineMAT(river_object=self,
+												save_to_mat=save_to_mat,
+												latitude_header=latitude_header,
+												longitude_header=longitude_header,
 												centerline_type=centerline_type)
```

### Comparing `centerline-width-0.2.5/centerline_width.egg-info/PKG-INFO` & `centerline-width-0.3.0/centerline_width.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 0.2.5
+Version: 0.3.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.2.5.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v0.3.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -22,15 +22,17 @@
         	* extractPointsToTextFile()
         	* convertColumnsToCSV()
         * **Find centerline and width of river**
         	* plotCenterline()
         	* plotCenterlineWidth()
         	* riverWidthFromCenterline()
         	* saveCenterlineCSV()
+        	* saveCenterlineMAT()
         	* centerlineVoronoi
+        	* centerlineEqualDistance 
         	* centerlineEvenlySpaced
         	* centerlineSmoothed
         	* centerlineLength
         	* rightBankLength
         	* leftBankLength
         
         | River Outlined in Google Earth Pro | Generated Centerline for the Riverbank |
@@ -54,24 +56,24 @@
         ```
         pip install -r requirements.txt
         ```
         Requirements will also be downloaded as part of the pip download
         
         ## Quickstart: centerline-width
         
-        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. Starting with Google Earth Pro, two .kml must first be translated to a single .csv file
+        The core of centerline-width works with a .csv file of the left and right bank latitude/longitudes. So, if starting from Google Earth Pro, two .kml must first be translated to a single .csv file
         
         ```python
         import centerline_width
         centerline_width.extractPointsToTextFile(left_kml="left_bank.kml",
         					right_kml="right_bank.kml",
         					text_output_name="river_coordinates_output.txt")
         centerline_width.convertColumnsToCSV(text_file="river_coordinates_output.txt")
         ```
-        Then, to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
+        Then once the .csv file is created, in order to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
         
         ```python
         river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
         ```
         
         To plot the centerline, run the `plotCenterline()` function from `river_object` created
         ```python
@@ -83,14 +85,16 @@
         
         While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
         ```python
         river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
+        For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
+        
         ## Preprocessing
         ### Convert KML files to Text File
         
         Convert two .kml files from Google Earth Pro (for the left and right bank) and export the coordinates into a text file
         
         ```
         extractPointsToTextFile(left_kml=None,
@@ -118,15 +122,15 @@
         30.037648 -92.868546 30.119746 -92.907917
         30.037674 -92.868536 30.119721 -92.907909
         30.037702 -92.868533 30.119706 -92.907905
         ```
         
         ### Converted Text File to CSV
         
-        Convert a text file with coordinates for a left and right bank's latitude/longitude to a csv file
+        Convert a text file with coordinates for a left and right bank's latitude and longitude to a csv file with columns for the left bank latitude (llat), left bank longitude (llon), right bank latitude (rlat), right bank longitude (rlon)
         
         ```
         convertColumnsToCSV(text_file=None, flipBankDirection=False)
         ```
         * **[REQUIRED]** text_file (string): File location of the text file to convert
         * [OPTIONAL] flipBankDirection (boolean): If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
@@ -162,47 +166,51 @@
         ### River Object
         First, generate a river object to contain river data and available transformations
         ```
         centerline_width.riverCenterline(csv_data=None,
         				optional_cutoff=None,
         				interpolate_data=False,
         				interpolate_n=5,
-        				interpolate_n_centerpoints=None)
+        				interpolate_n_centerpoints=None,
+        				equal_distance=10)
         ```
         * **[REQUIRED]** csv_data (string): File location of the text file to convert
         * [OPTIONAL] optional_cutoff (int): Include only the first x number of the data to chart (useful for debugging)
         * [OPTIONAL] interpolate_data (bool): Interpolate between existing data by adding additional points
         * [OPTIONAL] interpolate_n (int): Number of additional points to add between existing data, defaults to 5 (note: larger numbers will take exponentially longer to run, recommends less than 15)
         * [OPTIONAL] interpolate_n_centerpoints (int): Number of points used to interpolate the Voronoi centerline, defaults to the the length of the data frame (df_len)
+        * [OPTIONAL] equal_distance (int): Equal distance between points (in meters) used to interpolate the Voronoi centerline, defaults 10 meters
         
         **Solutions for sparse data:**
         
-        `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be changed with the `interpolate_n` option
+        `interpolate_data` is an option that can be used to find a centerline when the existing data generates a Voronoi graph that is jagged or contains gaps due to the combination of sparse data and a narrow river (See: Debugging, Error Handling, and Edge Cases - Fix Gaps and Jagged Centerlines). By default, `interpolate_data=True` will add 5 additional points between each existing point but can be increased or decreased by modifying the `interpolate_n` option
         
         `interpolate_n_centerpoints` is an option that can be used to increase the resolution (number of points) of the centerline found by the Voronoi vertices. By default, will evenly space out to the size of the dataframe. Can artificially increase the amount of width lines generated by increasing the number of center points. When `interpolate_n_centerpoints` increases, the number of width lines generated will increase (and visa versa)
         
         | interpolate_n_centerpoints=75 | interpolate_n_centerpoints=200 |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_75.png) | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_n_centerpoints_200.png) |
         
         **Object (class) useful attributes:**
         
         * centerlineVoronoi (list of tuples): List of the latitude and longitude coordinates of the centerline generated by Voronoi diagrams
+        * centerlineEqualDistance (list of tuples): List of the latitude and longitude coordinates of the centerline generated by equal distances between coordinates from the Voronoi diagrams
         * centerlineEvenlySpaced (list of tuples): List of the latitude and longitude coordinates of the centerline generated by evenly spacing out points generated by the Voronoi diagrams
         * centerlineSmoothed (list of tuples): List of the latitude and longitude coordinates of the centerline generated by smoothing out the evenly spaced out points generated by the Voronoi diagrams
         * centerlineLength (float): Length of the centerline of the river (in km)
         * rightBankLength (float): Length of the right bank of the river (in km)
         * leftBankLength (float): Length of the left bank of the river (in km)
         
         **Object (class) additional atttributes:**
         
         * river_name (string): name of object, set to the csv_data string
         * left_bank_coordinates (list of tuples): list of coordinates of the left bank generated from the csv file (`[(x, y), (x, y)]`)
         * right_bank_coordinates (list of tuples) list of coordinates of the right bank generated from the csv file (`[(x, y), (x, y)]`)
         * df_len (int): Length of the data frame of the csv data (spliced by the optional_cutoff)
+        * equal_distance (int): Distance between points (in meters) used in centerlineEqualDistance, defaults to points every 10 meters
         * bank_polygon (Shapley Polygon): Multi-sided polygon generated to encapsulate river bank (used to define an inside and an outside of the river)
         * top_bank (Shapley Linestring): Linestring that represents the top of the river/polygon
         * bottom_bank (Shapley Linestring): Linestring that represents the bottom of the river/polygon
         * starting_node (tuple): Tuple of the starting position (latitude and longitude) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
@@ -218,63 +226,89 @@
         ```
         
         ### Return Latitude/Longitude Coordinates of Centerline
         Return the latitude/longitude coordinates of the centerline based on the left and right banks
         
         **Types of Centerlines**
         
-        There are three types of centerline coordinates formed from the riverbank data. Each are built off of each other and are used to clean and smooth data
+        There are four types of centerline coordinates formed from the riverbank data
         
         - **Voronoi centerline**: centerline generated from where Voronoi vertices intersect within the river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/voronoi_centerline.png)
+        - **Equal Distance Centerline**: centerline based on Voronoi centerline but each point is equally spaced out from the previous (in meters) and takes into account the radius of the Earth to convert degrees to meters
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/equal_distance_centerline.png)
         - **Evenly Spaced Centerline**: centerline based on Voronoi centerline but evenly spaced with a fixed number of points
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/evenly_spaced_centerline.png)
         - **Smoothed Centerline**: centerline generated from the evenly spaced centerline but smoothed by a b-spline
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/smoothed_centerline.png)
         
         Centerline coordinates are formed by the Voronoi vertices
         ```
         river_object.centerlineVoronoi
         ```
         
-        Centerline coordinates are formed by Evenly Spaced Voronoi vertices
+        Centerline coordinates are formed by Equally Distanced vertices, set by `equal_distance`
+        ```
+        river_object.centerlineEqualDistance
+        ```
+        
+        Centerline coordinates are formed by Evenly Spaced vertices, set by `interpolate_n_centerpoints`
         ```
         river_object.centerlineEvenlySpaced
         ```
         
-        Centerline coordinates are formed from Smoothed Voronoi vertices
+        Centerline coordinates are formed from Smoothed vertices
         ```
         river_object.centerlineSmoothed
         ```
         
         Example:
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", optional_cutoff=15)
         river_centerline_coordinates = river_object.centerlineVoronoi
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
-        ### Save Centerline Coordinates to a CSV
+        ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude
         
         ```
         saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi")
         ```
         * **[REQUIRED]** save_to_csv (str): CSV filename, requires a .csv extension
-        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed"], defaults to "Voronoi"
+        * [OPTIONAL] centerline_type (str): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)`
+        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)`
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
-        
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
+        ### Save Centerline Coordinates to a .MAT File
+        Save the centerline coordinates to a .mat file with columns for latitude and longitude
+        
+        ```
+        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi")
+        ```
+        * **[REQUIRED]** save_to_mat (str): MAT filename, requires a .mat extension
+        * [OPTIONAL] centerline_type (str): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
+        * [OPTIONAL] latitude_header (str): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+        * [OPTIONAL] longitude_header (str): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` (will remove spaces and special characters and replaces with underscores)
+        
+        ```python
+        import centerline_width
+        river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
+        river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
+        ```
+        Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
+        
         ### Return Length of Centerline
         Return the length of the centerline found between the left and right bank generated by the Voronoi diagram
         ```
         river_object.centerlineLength
         ```
         Length returned in kilometers
         ```python
@@ -460,26 +494,30 @@
         
         If the latitude/longitude of the banks are generated in reverse order, flip the final values so left/right bank are in order
         
         This can be fixed by using the flipBankDirection optional argument `centerline_width.convertColumnsToCSV(text_file="data_example.txt", flipBankDirection=True)`
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/flipDirection_example.png)
         
         ### Invalid Smoothed Centerline
-        The smoothed centerline can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
+        The smoothed centerline (`river_object.centerlineSmoothed`) can end up lying outside the river if the centerline data points are sparse in a narrow river. If more than two points in the smoothed centerline lie outside the river, a warning will be thrown
         
         Example Error: `WARNING: Partially invalid smoothed centerline due to sparse centerline data (6 points lie outside the polygon), fix recommendation: rerun riverCenterline to create river object with interpolate_n_centerpoints set to 62+`
         
         By default, `interpolate_n_centerpoints` is set to None and not additional points will be added between the existing points along the centerline. By adding additional points between the existing centerline, the smoothed centerline can be fixed to stay within the polygon. This fix is set by creating a river object, `centerline_width.riverCenterline`, with `interpolate_n_centerpoints=65` (with the recommended 62+) to fix for centerline coordinates that lie outside the polyogon
         
         `interpolate_n_centerpoints = None` does not interpolate data points, so the size will be set to the number of fixed points when creating the evenly spaced coordinates (equal to the size of the data frame)
         
         | interpolate_n_centerpoints = None | interpolate_n_centerpoints = 65 |
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_fixed.png) |
         
+        For very narrow rivers, this problem can become extreme and pronounced
+        ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/invalid_smoothed_centerline_extreme.png)
+        
+        By increasing the interpolation between the centerline points, the smoothed centerlines will be forced within the polygon and reduce the amount of points outside of the polygon. By default, this warning will be thrown if more than 2 points are outside of polygon, so as long as more than 2 points lie outside the polygon, the warning will recommend doubling the amount of centerline points
         
         ### Fix Gaps and Jagged Centerlines
         Gaps formed can cause part of the centerline to be skipped due to sparse data. As a result, the start and end of the centerline can skip parts at the beginning or end of a river
         ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_short_path.png)
         Set river object created by `centerline_width.riverCenterline` to `interpolate_data=True` to fix for jagged edges or gaps formed by the interaction of sparse data and narrow banks
         ```python
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv", interpolate_data=True)
@@ -488,16 +526,17 @@
         | ------------- | ------------- |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps.png) |
         | ![example+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_false_gaps_2.png) | ![river_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/interpolate_true_no_gaps_2.png) |
         
         The amount of additional points added by interpolating can be adjusted with `interpolate_n`, but defaults to add 5 additional points between values
         
         ## Developer Notes: Tech Debt and Bug Fixes
+        * option to turn off verbose (no logs printed)
+        * option to specify Geod type (defaults to pyproj.Geod(ellps='WGS84'))
         * Fix legend overlapping on graph, replace doc_examples that have an overlapping
-        * Verify that smoothing filter option does not produce a line that goes outside of the polygon
         
         ## Citations
         Based on work written in R (Golly et al. 2017):
         
         >Golly, A. and Turowski, J. M.: Deriving principal channel metrics from bank and long-profile geometry with the R package cmgo, Earth Surf. Dynam., 5, 557-570, https://doi.org/10.5194/esurf-5-557-2017, 2017.
         
         [Github - CMGO](https://github.com/AntoniusGolly/cmgo)
```

### Comparing `centerline-width-0.2.5/centerline_width.egg-info/SOURCES.txt` & `centerline-width-0.3.0/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-0.2.5/setup.py` & `centerline-width-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.2.5"
+VERSION="0.3.0"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
@@ -34,19 +34,21 @@
 		"Topic :: Scientific/Engineering :: Hydrology",
 		"Topic :: Scientific/Engineering :: Visualization"
 	],
 	packages=find_namespace_packages(include=['centerline_width',
 											'centerline_width.*']),
 	include_package_data=True,
 	install_requires=[
+		"geopy>=2.3.0",
 		"haversine>=2.8.0",
 		"matplotlib>=3.1.0",
 		"networkx>=3.0",
 		"numpy>=1.24.1",
 		"pandas>=1.3.5",
 		"pykml>=0.2.0",
+		"pyproj>=3.4.1",
 		"pytest>=7.2.2",
 		"scipy>=1.10.1",
 		"shapely>=2.0.1"
 	],
 	python_requires='>=3.9'
 )
```

