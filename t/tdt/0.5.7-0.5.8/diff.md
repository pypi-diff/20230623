# Comparing `tmp/tdt-0.5.7.tar.gz` & `tmp/tdt-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tdt-0.5.7.tar", last modified: Wed Feb 22 15:07:03 2023, max compression
+gzip compressed data, was "dist\tdt-0.5.8.tar", last modified: Fri Jun 23 20:38:53 2023, max compression
```

## Comparing `tdt-0.5.7.tar` & `tdt-0.5.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 15:07:03.000000 tdt-0.5.7/
--rw-rw-rw-   0        0        0     1265 2023-02-22 15:07:03.000000 tdt-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-02-22 15:06:46.000000 tdt-0.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-02-22 15:07:03.000000 tdt-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-02-22 15:06:45.000000 tdt-0.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-22 15:07:03.000000 tdt-0.5.7/tdt/
--rw-rw-rw-   0        0        0     9386 2023-02-22 15:06:46.000000 tdt-0.5.7/tdt/BH32.py
--rw-rw-rw-   0        0        0     3202 2023-02-22 15:06:45.000000 tdt-0.5.7/tdt/PynapseUDP.py
--rw-rw-rw-   0        0        0    31632 2023-02-22 15:06:45.000000 tdt-0.5.7/tdt/SynapseAPI.py
--rw-rw-rw-   0        0        0     4989 2023-02-22 15:06:46.000000 tdt-0.5.7/tdt/TDTUDP.py
--rw-rw-rw-   0        0        0   111291 2023-02-22 15:06:46.000000 tdt-0.5.7/tdt/TDTbin2py.py
--rw-rw-rw-   0        0        0    18957 2023-02-22 15:06:46.000000 tdt-0.5.7/tdt/TDTfilter.py
--rw-rw-rw-   0        0        0     4445 2023-02-22 15:06:46.000000 tdt-0.5.7/tdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 15:07:03.000000 tdt-0.5.7/tdt.egg-info/
--rw-rw-rw-   0        0        0     1265 2023-02-22 15:06:57.000000 tdt-0.5.7/tdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-02-22 15:06:57.000000 tdt-0.5.7/tdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 15:06:57.000000 tdt-0.5.7/tdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-22 15:06:57.000000 tdt-0.5.7/tdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-02-22 15:06:57.000000 tdt-0.5.7/tdt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 20:38:53.000000 tdt-0.5.8/
+-rw-rw-rw-   0        0        0     1265 2023-06-23 20:38:53.000000 tdt-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-06-23 20:38:23.000000 tdt-0.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:38:53.000000 tdt-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-06-23 20:38:22.000000 tdt-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:38:53.000000 tdt-0.5.8/tdt/
+-rw-rw-rw-   0        0        0     9386 2023-06-23 20:38:22.000000 tdt-0.5.8/tdt/BH32.py
+-rw-rw-rw-   0        0        0     3202 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/PynapseUDP.py
+-rw-rw-rw-   0        0        0    31632 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/SynapseAPI.py
+-rw-rw-rw-   0        0        0     4989 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/TDTUDP.py
+-rw-rw-rw-   0        0        0   111293 2023-06-23 20:38:22.000000 tdt-0.5.8/tdt/TDTbin2py.py
+-rw-rw-rw-   0        0        0    18957 2023-06-23 20:38:23.000000 tdt-0.5.8/tdt/TDTfilter.py
+-rw-rw-rw-   0        0        0     4445 2023-06-23 20:38:22.000000 tdt-0.5.8/tdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:38:53.000000 tdt-0.5.8/tdt.egg-info/
+-rw-rw-rw-   0        0        0     1265 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-23 20:38:47.000000 tdt-0.5.8/tdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-23 20:38:46.000000 tdt-0.5.8/tdt.egg-info/top_level.txt
```

### Comparing `tdt-0.5.7/PKG-INFO` & `tdt-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdt
-Version: 0.5.7
+Version: 0.5.8
 Summary: Tucker-Davis Technologies (TDT) Python APIs for reading data and interacting with Synapse software
 Home-page: UNKNOWN
 Author: Mark Hanus
 Author-email: mhanus@tdt.com
 License: UNKNOWN
 Description: # tdt
```

### Comparing `tdt-0.5.7/README.md` & `tdt-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tdt-0.5.7/setup.py` & `tdt-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.7/tdt/BH32.py` & `tdt-0.5.8/tdt/BH32.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.7/tdt/PynapseUDP.py` & `tdt-0.5.8/tdt/PynapseUDP.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.7/tdt/SynapseAPI.py` & `tdt-0.5.8/tdt/SynapseAPI.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.7/tdt/TDTUDP.py` & `tdt-0.5.8/tdt/TDTUDP.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.7/tdt/TDTbin2py.py` & `tdt-0.5.8/tdt/TDTbin2py.py`

 * *Files 0% similar despite different names*

```diff
@@ -1292,16 +1292,16 @@
                                                                  code=store_code['code'],
                                                                  size=store_code['size'],
                                                                  type=store_code['type'],
                                                                  type_str=store_code['type_str'])
                         if header.stores[var_name].type_str == 'streams':
                             header.stores[var_name].ucf = store_code['ucf']
                         if header.stores[var_name].type_str != 'scalars':
-                            header.stores[var_name].fs = \
-                                np.double(np.array([store_code['temp'][9]]).view(np.float32))
+                            header.stores[var_name].fs = np.double(np.array([store_code['temp'][9]]).view(np.float32)[0])
+                            
                         header.stores[var_name].dform = store_code['dform']
                 
                 valid_ind = np.where(codes == store_code['code'])[0]
                 
                 # look for notes in 'freqs' field for epoch or scalar events
                 if len(note_str) > 0 and store_code['type_str'] in ['scalars', 'epocs']:
                     
@@ -2069,19 +2069,19 @@
                         # index 1 is at header.stores.(current_name).start_time
                         # round timestamps to the nearest sample
                         
                         # actual time the segment starts on
                         td_time = time2sample(data[current_type_str][current_name].start_time[jj], current_freq, to_time=True)
                         tdSample = time2sample(td_time, current_freq, t1=1)
                         ltSample = time2sample(valid_time_range[0,jj], current_freq, t1=1)
-                        etSample = time2sample(valid_time_range[1,jj], current_freq, t1=1)
                         minSample = ltSample - tdSample
                         if np.isinf(valid_time_range[1,jj]):
                             maxSample = MAX_UINT64
                         else:
+                            etSample = time2sample(valid_time_range[1,jj], current_freq, t1=1)
                             maxSample = etSample - tdSample - 1
                         data[current_type_str][current_name].data[jj] = data[current_type_str][current_name].data[jj][:,minSample:int(maxSample+1)]
                         data[current_type_str][current_name].start_time[jj] = ltSample / current_freq
                 
                 data[current_type_str][current_name].channel = channels
                 delattr(data[current_type_str][current_name], 'filtered_chan')
                 delattr(data[current_type_str][current_name], 'filtered_data')
```

### Comparing `tdt-0.5.7/tdt/TDTfilter.py` & `tdt-0.5.8/tdt/TDTfilter.py`

 * *Files identical despite different names*

### Comparing `tdt-0.5.7/tdt/__init__.py` & `tdt-0.5.8/tdt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 
 import os
 import re
 
 import numpy as np
 
 # Tank event types (tsqEventHeader.type)
```

### Comparing `tdt-0.5.7/tdt.egg-info/PKG-INFO` & `tdt-0.5.8/tdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdt
-Version: 0.5.7
+Version: 0.5.8
 Summary: Tucker-Davis Technologies (TDT) Python APIs for reading data and interacting with Synapse software
 Home-page: UNKNOWN
 Author: Mark Hanus
 Author-email: mhanus@tdt.com
 License: UNKNOWN
 Description: # tdt
```

