# Comparing `tmp/gemlog-1.7.0.tar.gz` & `tmp/gemlog-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemlog-1.7.0.tar", last modified: Wed Mar 29 04:39:20 2023, max compression
+gzip compressed data, was "gemlog-1.7.1.tar", last modified: Fri Jun 23 18:55:10 2023, max compression
```

## Comparing `gemlog-1.7.0.tar` & `gemlog-1.7.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.573524 gemlog-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-29 04:39:10.000000 gemlog-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-29 04:39:10.000000 gemlog-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-29 04:39:20.569524 gemlog-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-29 04:39:10.000000 gemlog-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.569524 gemlog-1.7.0/gemlog/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66266 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.565524 gemlog-1.7.0/gemlog/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.569524 gemlog-1.7.0/gemlog/data/noise/
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/noise/Gem_v0.98_Noise_spec.txt
--rw-r--r--   0 runner    (1001) docker     (123)   118800 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.565524 gemlog-1.7.0/gemlog/data/response/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.569524 gemlog-1.7.0/gemlog/data/response/datalogger/
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.569524 gemlog-1.7.0/gemlog/data/response/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/gem_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    32202 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/gem_network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7020 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/gemconvert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/gemconvert_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/gemlog_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)    47418 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/huddle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/parsers.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23693 2023-03-29 04:39:12.000000 gemlog-1.7.0/gemlog/xcorr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:39:20.569524 gemlog-1.7.0/gemlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-29 04:39:20.000000 gemlog-1.7.0/gemlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-29 04:39:20.000000 gemlog-1.7.0/gemlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 04:39:20.000000 gemlog-1.7.0/gemlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-29 04:39:20.000000 gemlog-1.7.0/gemlog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 04:39:20.000000 gemlog-1.7.0/gemlog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-29 04:39:20.000000 gemlog-1.7.0/gemlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-29 04:39:20.000000 gemlog-1.7.0/gemlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 04:39:20.573524 gemlog-1.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4343 2023-03-29 04:39:12.000000 gemlog-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.177071 gemlog-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 18:55:03.000000 gemlog-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 18:55:03.000000 gemlog-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-23 18:55:10.177071 gemlog-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-23 18:55:03.000000 gemlog-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66266 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/data/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/noise/Gem_v0.98_Noise_spec.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   118800 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog/data/response/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.177071 gemlog-1.7.1/gemlog/data/response/datalogger/
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.177071 gemlog-1.7.1/gemlog/data/response/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gem_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gem_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7020 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gemconvert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gemconvert_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/gemlog_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/huddle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/parsers.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-06-23 18:55:06.000000 gemlog-1.7.1/gemlog/xcorr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:55:10.173071 gemlog-1.7.1/gemlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 18:55:10.000000 gemlog-1.7.1/gemlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:55:10.177071 gemlog-1.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4343 2023-06-23 18:55:06.000000 gemlog-1.7.1/setup.py
```

### Comparing `gemlog-1.7.0/LICENSE` & `gemlog-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/PKG-INFO` & `gemlog-1.7.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemlog
-Version: 1.7.0
+Version: 1.7.1
 Summary: A set of functions for processing Gem datalogger files.
 Home-page: https://github.com/ajakef/gemlog
 Author: Jake Anderson
 Maintainer-email: ajakef@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gemlog-1.7.0/README.md` & `gemlog-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/__init__.py` & `gemlog-1.7.1/gemlog/__init__.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/core.py` & `gemlog-1.7.1/gemlog/core.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/noise/Gem_v0.98_Noise_spec.txt` & `gemlog-1.7.1/gemlog/data/noise/Gem_v0.98_Noise_spec.txt`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt` & `gemlog-1.7.1/gemlog/data/noise/IMSNOISE_MIN_MED_MAX.txt`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100` & `gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM000..HHZ.GEMINFRAV0.0.100`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100` & `gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM001..HHZ.GEMINFRAV1.1.100`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100` & `gemlog-1.7.1/gemlog/data/response/datalogger/RESP.XX.GM002..HHZ.GEMINFRAV1.0.100`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005` & `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0005`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016` & `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0016`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023` & `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS000..BDF.GEMV0.26.0_0023`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022` & `gemlog-1.7.1/gemlog/data/response/sensor/RESP.XX.IS025..BDF.GEMV1.26.0_0022`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/gem_cat.py` & `gemlog-1.7.1/gemlog/gem_cat.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/gem_network.py` & `gemlog-1.7.1/gemlog/gem_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-import glob, obspy, os, warnings, gemlog, sys, argparse
+import glob, obspy, os, warnings, gemlog, sys, argparse, pathlib
 #from obspy.clients.nrl import NRL
 #from contextlib import contextmanager,redirect_stderr,redirect_stdout
 #from os import devnull
 #nrl = NRL()
 
 #response = nrl.get_response(sensor_keys = ['Gem', 'Gem Infrasound Sensor v1.0'], datalogger_keys = ['Gem', 'Gem Infrasound Logger v1.0', '0 - 128000 counts/V'])
 
@@ -415,15 +415,19 @@
     else:
         raise Exception('invalid gps_dir_pattern type; must be list or str')
     gpsTable = pd.DataFrame(columns=['year', 'date', 'lat', 'lon', 't'])
     for gpsDir in gpsDirList:
         if os.path.isdir(gpsDir):
             fnList = sorted(glob.glob(gpsDir + '/' + SN + '*'))
         else:
-            fnList = [gpsDir] # in case the user provides the gps filename directly
+            # in case the user provides the gps filename directly. requires that the filename start with SN.
+            if pathlib.Path(gpsDir).name[:3] == SN:
+                fnList = [gpsDir]
+            else:
+                fnList = []
         if len(fnList) > 0: # if any gps files matching SN are found, read and append the last
             gpsTable = pd.concat([gpsTable,
                                   pd.read_csv(fnList[-1])], ignore_index=True)
     return gpsTable
 ReadLoggerGPS = read_gps # alias; v1.0.0
 
 def summarize_gps(gps_dir_pattern, station_info = None, output_file = None, t1 = None, t2 = None, include_SN = None, exclude_SN = None):
@@ -496,15 +500,15 @@
         for fn in gps_dir_pattern:
             if os.path.isdir(fn):
                 gpsFileList += glob.glob(fn + '/*gps*txt')
             else:
                 gpsFileList.append(fn)
     else:
         raise Exception(f'invalid type for gpsDirList {gpsDirList}; must be str or list')
-
+    
     gpsFileList = sorted(gpsFileList)
     snList = []
     for gpsFile in gpsFileList:
         current_SN = gpsFile.split('/')[-1].split('gps')[0]
         if ((include_SN is None) or (current_SN in include_SN)) and \
            ((exclude_SN is None) or (current_SN not in exclude_SN)):
             snList.append(current_SN)
@@ -624,15 +628,15 @@
         exclude_SNs = args.exclude_SNs.split(',')
     else:
         exclude_SNs = None
 
     gps_folder = args.gps_folder
     station_info_file = args.station_info_file
     output_file = args.output_file
-    
+
     coords = summarize_gps(gps_folder, station_info = station_info_file,
                            output_file = output_file + '.csv', t1 = args.t1, t2 = args.t2,
                            include_SN = args.include_SNs, exclude_SN = args.exclude_SNs)
     response = gemlog.get_gem_response(gain = 'high')
     if 'station' not in coords.keys():
         coords['station'] = coords['SN']
     if 'elevation' not in coords.keys():
```

### Comparing `gemlog-1.7.0/gemlog/gemconvert.py` & `gemlog-1.7.1/gemlog/gemconvert.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/gemconvert_single.py` & `gemlog-1.7.1/gemlog/gemconvert_single.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/gemlog_aux.py` & `gemlog-1.7.1/gemlog/gemlog_aux.py`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/huddle_test.py` & `gemlog-1.7.1/gemlog/huddle_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,16 +506,16 @@
         gps_ax[SN_index].errorbar(gps_proportion, y_scale, yerr= y_scale, ecolor = 'r')
         gps_ax[SN_index].set_ylabel('#' + SN_list[SN_index])
         gps_ax[SN_index].axes.xaxis.set_ticklabels([])
         gps_ax[SN_index].xaxis.set_major_locator(plt.MultipleLocator(20))
         gps_ax[SN_index].xaxis.set_minor_locator(plt.MultipleLocator(10))
         if SN == SN_list[-1]:    
             gps_ax[SN_index].set_xlabel('seconds')
-            #gps_ax[SN_index].axes.xaxis.set_ticklabels([0,20,40,60,80,100,120,140,160,'>180']) ## replaced with set_xticks because this creates a warning
-            gps_ax[SN_index].set_xticks(np.arange(0, 10) * 20, [0,20,40,60,80,100,120,140,160,'>180']) ## 2022-06-14 JFA; seems to work
+            gps_ax[SN_index].set_xticks(ticks = np.arange(0, 10) * 20) ## 2022-06-14 JFA; seems to work
+            gps_ax[SN_index].axes.xaxis.set_ticklabels([0,20,40,60,80,100,120,140,160,'>180']) ## replaced with set_xticks because this creates a warning
             gps_ax[SN_index].annotate('GPS on-time ratio', (gps_proportion, 10), xytext = (gps_proportion + 10 , 15), color = 'r',
                                   arrowprops = dict(arrowstyle = '->', connectionstyle = "angle, angleA = 90, angleB = 0, rad = 10", color = 'r'))
         
            
         gps = pd.read_csv(path +'/gps/' + SN + 'gps_000.txt', sep = ',')
         gps.t = gps.t.apply(obspy.UTCDateTime)
         gps_dict[SN] = gps
```

### Comparing `gemlog-1.7.0/gemlog/parsers.pyx` & `gemlog-1.7.1/gemlog/parsers.pyx`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/gemlog/version.py` & `gemlog-1.7.1/gemlog/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-__version__ = '1.7.0' # new command-line tool to make sensor network info, including a stationXML file 
+__version__ = '1.7.1' # fixed verify_huddle_test bug with Axes.set_ticks 
+#__version__ = '1.7.0' # new command-line tool to make sensor network info, including a stationXML file 
 #__version__ = '1.6.9' # added command-line tools to cross-correlate data and invert time lags for slowness and backazimuth, fixed for pypi 
 #__version__ = '1.6.8' # added command-line tools to cross-correlate data and invert time lags for slowness and backazimuth 
 #__version__ = '1.6.7' # bug fix in verify_huddle_test 
 #__version__ = '1.6.6' # version described by JOSS paper 
 #__version__ = '1.6.5' # bug fixes and other minor improvements 
 #__version__ = '1.6.4' # upgrades dependencies due to moderate security issue in numpy: https://github.com/advisories/GHSA-fpfv-jqm9-f5jm 
 #__version__ = '1.6.3' # minor improvements/bug fixes for verify_huddle_test 
@@ -58,8 +59,8 @@
 #__version__  = '0.3.2' # added demo with inventory functions
 #__version__  = '0.3.1' #  more helpful logging output
 #__version__  = '0.3.0' # 2020-09-04, cython added
 #__version__  = '0.2.3' # improving testing, including empty/bad files
 #__version__  = '0.2.2' # automated github tests, setup.py improvements, and modelst speed-up
 #__version__  = '0.2.1' # 
 #__version__ = '0.0.5' # added new functions to make network map from gps data and rename mseeds from serial_number.channel to network.station.location.channel codes
-## List of old versions is not comprehensive#######################################################
+## List of old versions is not comprehensive########################################################
```

### Comparing `gemlog-1.7.0/gemlog/xcorr.py` & `gemlog-1.7.1/gemlog/xcorr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from obspy.signal.cross_correlation import correlate, xcorr_max
 import obspy
 import numpy as np
 import pandas as pd
 import glob, os, traceback, sys, getopt, argparse, re
 from gemlog.gem_network import _unique
+import gemlog
 import scipy.interpolate
 
 def xcorr_all_terminal(input = sys.argv[1:]):
-    examples_text = '''
+    examples_text = f'''
     Examples: (replace '/' with '\' if using Windows)\n
     # process all data in mseed_data between 2022-09-01 00:00:00 UTC and 05:00:00 UTC from stations 121, 122, and 123
     waveform_calc_lags -1 2022-09-01 -2 2022-09-01_05:00:00 -i 121,122,123 -o output_file.csv mseed_data/* 
 
     # process all data in mseed_data except stations 100 and 110, first filtering between 10-20 Hz instead of default frequencies
     waveform_calc_lags -x 100,110 -L 10 -H 20 -o 10-20Hz_output_file.csv mseed_data/* 
 
     # process all data in mseed_data, upsampling by 4x to improve precision, and using a 30-second window length
-    waveform_calc_lags -u 4 -w 30 -o upsampled_30sec_output_file.csv mseed_data/*'''
+    waveform_calc_lags -u 4 -w 30 -o upsampled_30sec_output_file.csv mseed_data/*    
+
+    gemlog version {gemlog.__version__}'''
     parser = argparse.ArgumentParser(description='Use cross-correlation to find delays between waveform files, and calculate backazimuth and horizontal slowness.',
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                      epilog = examples_text)
     parser.add_argument('files', nargs='+', help='List of data files to process (wildcards are allowed)')
     
     parser.add_argument('-o', '--output_file', nargs = 1, default=None, help='Output file to write')
     parser.add_argument('-i', '--include_IDs', help='Station IDs to include in processing (default: all)')
@@ -70,15 +73,16 @@
                          win_length_sec = args.window_length_seconds, overlap = args.overlap,
                          upsample_ratio = args.upsample_ratio, quiet = args.quiet)
     xcorr_df.to_csv(args.output_file[0], sep = ',', index = False)
 
     
 
 def calculate_direction_terminal(input = sys.argv[1:]):
-    parser = argparse.ArgumentParser(description='Invert time lags found by cross-correlation to find backazimuth and horizontal slowness.', formatter_class=argparse.HelpFormatter)
+    epilog = f'gemlog version {gemlog.__version__}'
+    parser = argparse.ArgumentParser(description='Invert time lags found by cross-correlation to find backazimuth and horizontal slowness.', formatter_class=argparse.HelpFormatter, epilog = epilog)
     parser.add_argument('-i', '--input_file', nargs = 1, help='File with time lags created by waveform_xc')
     parser.add_argument('-l', '--location_file', nargs = 1, help='stationXML file containing station locations')
     parser.add_argument('-o', '--output_file', nargs = 1, help='Output file to write, including azimuth and horizontal slowness results')
     args = parser.parse_args(input)
 
     print(args)
     
@@ -250,18 +254,19 @@
             if filename not in files_read:
                 st += obspy.read(filename)
                 files_read.append(filename)
 
         st.merge()
         ## throw out data before the start of this day, and any unused traces
         st.trim(day_start, t2)
-        for i, tr in enumerate(st):
-            if tr.id not in IDs:
-                st.pop(i) 
-
+        #for i, tr in enumerate(st):
+        #    if tr.id not in IDs:
+        #        st.pop(i) 
+        st = obspy.Stream([tr for tr in st if tr.id in IDs])
+        
         ## finally, apply whatever function you have to the data.
         ## 'function' must accept two inputs: an obspy.Stream with data,
         ## and a dictionary with function-specific arguments.
         ## the function will return a pd.DataFrame. append to a list, then merge at the end
         try:
             day_output = function(st.slice(day_start, day_end), args)
             output_list.append(day_output)
```

### Comparing `gemlog-1.7.0/gemlog.egg-info/PKG-INFO` & `gemlog-1.7.1/gemlog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemlog
-Version: 1.7.0
+Version: 1.7.1
 Summary: A set of functions for processing Gem datalogger files.
 Home-page: https://github.com/ajakef/gemlog
 Author: Jake Anderson
 Maintainer-email: ajakef@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gemlog-1.7.0/gemlog.egg-info/SOURCES.txt` & `gemlog-1.7.1/gemlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemlog-1.7.0/setup.py` & `gemlog-1.7.1/setup.py`

 * *Files identical despite different names*

