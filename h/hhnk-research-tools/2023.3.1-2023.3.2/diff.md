# Comparing `tmp/hhnk_research_tools-2023.3.1.tar.gz` & `tmp/hhnk_research_tools-2023.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk_research_tools-2023.3.1.tar", last modified: Fri Jun 23 10:38:28 2023, max compression
+gzip compressed data, was "hhnk_research_tools-2023.3.2.tar", last modified: Fri Jun 23 10:55:36 2023, max compression
```

## Comparing `hhnk_research_tools-2023.3.1.tar` & `hhnk_research_tools-2023.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:22.803257 hhnk_research_tools-2023.3.1/
--rw-rw-rw-   0        0        0      598 2023-06-23 10:38:28.419829 hhnk_research_tools-2023.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-06-23 10:04:59.000000 hhnk_research_tools-2023.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:23.650270 hhnk_research_tools-2023.3.1/hhnk_research_tools/
--rw-rw-rw-   0        0        0     2110 2023-06-23 09:49:02.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/__init__.py
--rw-rw-rw-   0        0        0     5861 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/dataframe_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:24.947290 hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/
--rw-rw-rw-   0        0        0        0 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/__init__.py
--rw-rw-rw-   0        0        0     1561 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/file_class.py
--rw-rw-rw-   0        0        0     7014 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/folder_file_classes.py
--rw-rw-rw-   0        0        0     6168 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/sqlite_class.py
--rw-rw-rw-   0        0        0     6784 2023-06-23 09:46:46.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/threedi_schematisation.py
--rw-rw-rw-   0        0        0     3570 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/general_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:25.398296 hhnk_research_tools-2023.3.1/hhnk_research_tools/gis/
--rw-rw-rw-   0        0        0     1092 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/gis/__init__.py
--rw-rw-rw-   0        0        0    18597 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/gis/raster.py
--rw-rw-rw-   0        0        0     1427 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/gis/vector.py
--rw-rw-rw-   0        0        0     2097 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/processes.py
--rw-rw-rw-   0        0        0    18373 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/raster_functions.py
--rw-rw-rw-   0        0        0    11573 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/sql_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:26.860319 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/
--rw-rw-rw-   0        0        0      149 2022-07-04 12:41:36.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/__init__.py
--rw-rw-rw-   0        0        0     3603 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/construct_rain_scenario.py
--rw-rw-rw-   0        0        0     2260 2022-08-17 15:04:24.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py
--rw-rw-rw-   0        0        0     1997 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/geometry_functions.py
--rw-rw-rw-   0        0        0    12463 2022-07-04 14:10:34.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/grid.py
--rw-rw-rw-   0        0        0     1722 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/gridedit.py
--rw-rw-rw-   0        0        0      343 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/read_api_file.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:27.220325 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/variables/
--rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/variables/__init__.py
--rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/variables/gridadmin.py
--rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/variables/rain_dataframe.py
--rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/variables/results_mapping.py
--rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/variables/variables_container.py
--rw-rw-rw-   0        0        0     1870 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/variables.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:22.591253 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/
--rw-rw-rw-   0        0        0       80 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:28.295341 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/
--rw-rw-rw-   0        0        0        0 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/__init__.py
--rw-rw-rw-   0        0        0    70142 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg
--rw-rw-rw-   0        0        0    64399 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg
--rw-rw-rw-   0        0        0    64209 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg
--rw-rw-rw-   0        0        0    69232 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg
--rw-rw-rw-   0        0        0     5000 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/wss_calculations.py
--rw-rw-rw-   0        0        0     4088 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/wss_loading.py
--rw-rw-rw-   0        0        0     7076 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/wss_main.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:24.265279 hhnk_research_tools-2023.3.1/hhnk_research_tools.egg-info/
--rw-rw-rw-   0        0        0      598 2023-06-23 10:38:21.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2015 2023-06-23 10:38:21.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 10:38:21.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-23 10:38:21.000000 hhnk_research_tools-2023.3.1/hhnk_research_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 10:38:28.479194 hhnk_research_tools-2023.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1902 2023-06-23 08:12:53.000000 hhnk_research_tools-2023.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:31.156098 hhnk_research_tools-2023.3.2/
+-rw-rw-rw-   0        0        0      598 2023-06-23 10:55:36.438237 hhnk_research_tools-2023.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2023-06-23 10:51:35.000000 hhnk_research_tools-2023.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:31.866109 hhnk_research_tools-2023.3.2/hhnk_research_tools/
+-rw-rw-rw-   0        0        0     2110 2023-06-23 10:52:41.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/__init__.py
+-rw-rw-rw-   0        0        0     5861 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/dataframe_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:32.905125 hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/
+-rw-rw-rw-   0        0        0        0 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/__init__.py
+-rw-rw-rw-   0        0        0     1561 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/file_class.py
+-rw-rw-rw-   0        0        0     7014 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/folder_file_classes.py
+-rw-rw-rw-   0        0        0     6168 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/sqlite_class.py
+-rw-rw-rw-   0        0        0     6813 2023-06-23 10:52:14.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/threedi_schematisation.py
+-rw-rw-rw-   0        0        0     3570 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/general_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:33.304131 hhnk_research_tools-2023.3.2/hhnk_research_tools/gis/
+-rw-rw-rw-   0        0        0     1092 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/gis/__init__.py
+-rw-rw-rw-   0        0        0    18597 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/gis/raster.py
+-rw-rw-rw-   0        0        0     1427 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/gis/vector.py
+-rw-rw-rw-   0        0        0     2097 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/processes.py
+-rw-rw-rw-   0        0        0    18373 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/raster_functions.py
+-rw-rw-rw-   0        0        0    11573 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/sql_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:34.257146 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/
+-rw-rw-rw-   0        0        0      149 2022-07-04 12:41:36.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/__init__.py
+-rw-rw-rw-   0        0        0     3603 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/construct_rain_scenario.py
+-rw-rw-rw-   0        0        0     2260 2022-08-17 15:04:24.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py
+-rw-rw-rw-   0        0        0     1997 2023-05-10 15:38:56.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/geometry_functions.py
+-rw-rw-rw-   0        0        0    12463 2022-07-04 14:10:34.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/grid.py
+-rw-rw-rw-   0        0        0     1722 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/gridedit.py
+-rw-rw-rw-   0        0        0      343 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/read_api_file.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:35.114159 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/variables/
+-rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/variables/__init__.py
+-rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/variables/gridadmin.py
+-rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/variables/rain_dataframe.py
+-rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/variables/results_mapping.py
+-rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/variables/variables_container.py
+-rw-rw-rw-   0        0        0     1870 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/variables.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:35.505165 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/
+-rw-rw-rw-   0        0        0       80 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:36.245176 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/
+-rw-rw-rw-   0        0        0        0 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/__init__.py
+-rw-rw-rw-   0        0        0    70142 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg
+-rw-rw-rw-   0        0        0    64399 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg
+-rw-rw-rw-   0        0        0    64209 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg
+-rw-rw-rw-   0        0        0    69232 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg
+-rw-rw-rw-   0        0        0     5000 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/wss_calculations.py
+-rw-rw-rw-   0        0        0     4088 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/wss_loading.py
+-rw-rw-rw-   0        0        0     7076 2023-06-22 10:20:37.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/wss_main.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:55:32.324116 hhnk_research_tools-2023.3.2/hhnk_research_tools.egg-info/
+-rw-rw-rw-   0        0        0      598 2023-06-23 10:55:30.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2015 2023-06-23 10:55:30.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 10:55:30.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-23 10:55:30.000000 hhnk_research_tools-2023.3.2/hhnk_research_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 10:55:36.482597 hhnk_research_tools-2023.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1902 2023-06-23 08:12:53.000000 hhnk_research_tools-2023.3.2/setup.py
```

### Comparing `hhnk_research_tools-2023.3.1/PKG-INFO` & `hhnk_research_tools-2023.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhnk_research_tools
-Version: 2023.3.1
+Version: 2023.3.2
 Summary: General tools for analysis, data manipulation and threedi interaction for analysis of water systems
 Home-page: https://github.com/HHNK/hhnk-research-tools
 Author: Wietse van Gerwen
 Author-email: w.vangerwen@hhnk.nl
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HHNK/hhnk-research-tools/issues
 Platform: UNKNOWN
```

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/__init__.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,12 +69,12 @@
     ThreediResult,
     RevisionsDir,
 )
 
 # TODO how does this versioning work?
 # Threedigrid version number is automatic updated with zest.releaser. Geopandas uses versioneer.py.
 # the version number in setup.py is updated using the find_version()
-__version__ = '2023.3.1'
+__version__ = '2023.3.2'
 
 __doc__ = """
 General toolbox for loading, converting and saving serval datatypes.
 """
```

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/dataframe_functions.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/file_class.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/file_class.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/folder_file_classes.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/folder_file_classes.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/sqlite_class.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/sqlite_class.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/folder_file_classes/threedi_schematisation.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/folder_file_classes/threedi_schematisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,16 @@
 """
 
 
 class ThreediResult(Folder):
     """Result of threedi simulation. Base files are .nc and .h5.
     Use .grid to access GridH5ResultAdmin and .admin to access GridH5Admin"""
 
-    def __init__(self, base):
-        super().__init__(base)
+    def __init__(self, base, create=False):
+        super().__init__(base, create=create)
 
         # Files
         self.add_file("grid_path", "results_3di.nc")
         self.add_file("admin_path", "gridadmin.h5")
 
     @property
     def grid(self):
```

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/general_functions.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/general_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/gis/__init__.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/gis/__init__.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/gis/raster.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/gis/raster.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/gis/vector.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/gis/vector.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/processes.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/processes.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/raster_functions.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/raster_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/sql_functions.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/sql_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/construct_rain_scenario.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/construct_rain_scenario.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/geometry_functions.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/grid.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/grid.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/threedi/gridedit.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/threedi/gridedit.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/variables.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/variables.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_hhnk_2020.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_lizard_servicedesk.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/resources/cfg_stowa_standaard.cfg`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/wss_calculations.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/wss_calculations.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/wss_loading.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/wss_loading.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools/waterschadeschatter/wss_main.py` & `hhnk_research_tools-2023.3.2/hhnk_research_tools/waterschadeschatter/wss_main.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools.egg-info/PKG-INFO` & `hhnk_research_tools-2023.3.2/hhnk_research_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhnk-research-tools
-Version: 2023.3.1
+Version: 2023.3.2
 Summary: General tools for analysis, data manipulation and threedi interaction for analysis of water systems
 Home-page: https://github.com/HHNK/hhnk-research-tools
 Author: Wietse van Gerwen
 Author-email: w.vangerwen@hhnk.nl
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HHNK/hhnk-research-tools/issues
 Platform: UNKNOWN
```

### Comparing `hhnk_research_tools-2023.3.1/hhnk_research_tools.egg-info/SOURCES.txt` & `hhnk_research_tools-2023.3.2/hhnk_research_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-2023.3.1/setup.py` & `hhnk_research_tools-2023.3.2/setup.py`

 * *Files identical despite different names*

