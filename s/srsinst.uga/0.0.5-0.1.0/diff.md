# Comparing `tmp/srsinst.uga-0.0.5.tar.gz` & `tmp/srsinst.uga-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument_library\uga100\dist\.tmp-h3cmqrk7\srsinst.uga-0.0.5.tar", last modified: Thu Jun 15 19:20:47 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument drivers to GIT\uga100\dist\.tmp-ry0s2_h7\srsinst.uga-0.1.0.tar", last modified: Fri Jun 23 00:06:11 2023, max compression
```

## Comparing `srsinst.uga-0.0.5.tar` & `srsinst.uga-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/
--rw-rw-rw-   0        0        0     1103 2023-05-19 19:35:50.000000 srsinst.uga-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     7323 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6408 2023-06-15 19:19:47.000000 srsinst.uga-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.410714 srsinst.uga-0.0.5/docs/
--rw-rw-rw-   0        0        0      654 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.393316 srsinst.uga-0.0.5/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.410714 srsinst.uga-0.0.5/docs/_static/image/
--rw-rw-rw-   0        0        0   174299 2023-05-16 16:03:57.000000 srsinst.uga-0.0.5/docs/_static/image/UGA100_composition_analysis_screenshot.png
--rwxrwxrwx   0        0        0       28 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/autodoc.bat
--rw-rw-rw-   0        0        0     5458 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/basic_operation.rst
--rw-rw-rw-   0        0        0       26 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/changelog.rst
--rw-rw-rw-   0        0        0     1985 2023-06-13 17:27:43.000000 srsinst.uga-0.0.5/docs/conf.py
--rw-rw-rw-   0        0        0     1168 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/connection.rst
--rw-rw-rw-   0        0        0     1541 2023-06-13 17:07:45.000000 srsinst.uga-0.0.5/docs/index.rst
--rw-rw-rw-   0        0        0     1246 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/make.bat
--rw-rw-rw-   0        0        0       32 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/requirements.txt
--rw-rw-rw-   0        0        0     1010 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/scan_operation.rst
--rw-rw-rw-   0        0        0      329 2023-06-13 17:18:39.000000 srsinst.uga-0.0.5/docs/srsinst.uga.instruments.rst
--rw-rw-rw-   0        0        0      478 2023-06-13 17:16:42.000000 srsinst.uga-0.0.5/docs/srsinst.uga.instruments.uga100.rst
--rw-rw-rw-   0        0        0      134 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/srsinst.uga.rst
--rw-rw-rw-   0        0        0      530 2023-06-13 17:33:33.000000 srsinst.uga-0.0.5/docs/srsinst.uga.tasks.rst
--rw-rw-rw-   0        0        0     1473 2023-05-19 21:28:14.000000 srsinst.uga-0.0.5/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1363 2023-06-15 19:14:32.000000 srsinst.uga-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.393316 srsinst.uga-0.0.5/srsinst/
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst/uga/
--rw-rw-rw-   0        0        0      229 2023-06-15 19:17:17.000000 srsinst.uga-0.0.5/srsinst/uga/__init__.py
--rw-rw-rw-   0        0        0      483 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/__main__.py
--rw-rw-rw-   0        0        0    10600 2023-05-19 21:22:27.000000 srsinst.uga-0.0.5/srsinst/uga/gaslib.dat
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst/uga/instruments/
--rw-rw-rw-   0        0        0       47 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-05-19 21:32:52.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/get_instruments.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/__init__.py
--rw-rw-rw-   0        0        0    10643 2023-05-31 00:34:22.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/components.py
--rw-rw-rw-   0        0        0     4643 2023-05-24 17:51:21.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/keys.py
--rw-rw-rw-   0        0        0     5544 2023-06-15 17:42:38.000000 srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/uga.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.427008 srsinst.uga-0.0.5/srsinst/uga/tasks/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/__init__.py
--rw-rw-rw-   0        0        0     4415 2023-05-24 17:26:46.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/ugamodecontroltask.py
--rw-rw-rw-   0        0        0     3881 2023-05-19 21:34:42.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/ugamultiplottask.py
--rw-rw-rw-   0        0        0     1949 2023-05-24 18:32:16.000000 srsinst.uga-0.0.5/srsinst/uga/tasks/ugastatemonitortask.py
--rw-rw-rw-   0        0        0     2339 2023-05-24 16:25:05.000000 srsinst.uga-0.0.5/srsinst/uga/uga.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-15 19:20:47.417005 srsinst.uga-0.0.5/srsinst.uga.egg-info/
--rw-rw-rw-   0        0        0     7323 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 19:20:47.000000 srsinst.uga-0.0.5/srsinst.uga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.674432 srsinst.uga-0.1.0/
+-rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsinst.uga-0.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1103 2023-05-19 19:35:50.000000 srsinst.uga-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7444 2023-06-23 00:06:11.674432 srsinst.uga-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6529 2023-06-15 22:40:27.000000 srsinst.uga-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.651659 srsinst.uga-0.1.0/docs/
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.651659 srsinst.uga-0.1.0/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.651659 srsinst.uga-0.1.0/docs/_static/image/
+-rw-rw-rw-   0        0        0   174299 2023-05-16 16:03:57.000000 srsinst.uga-0.1.0/docs/_static/image/UGA100_composition_analysis_screenshot.png
+-rw-rw-rw-   0        0        0     1363 2023-06-23 00:00:45.000000 srsinst.uga-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 00:06:11.674432 srsinst.uga-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.uga-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.651659 srsinst.uga-0.1.0/srsinst/
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.664428 srsinst.uga-0.1.0/srsinst/uga/
+-rw-rw-rw-   0        0        0      229 2023-06-23 00:04:31.000000 srsinst.uga-0.1.0/srsinst/uga/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-05-19 21:22:28.000000 srsinst.uga-0.1.0/srsinst/uga/__main__.py
+-rw-rw-rw-   0        0        0    10600 2023-05-19 21:22:27.000000 srsinst.uga-0.1.0/srsinst/uga/gaslib.dat
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.664428 srsinst.uga-0.1.0/srsinst/uga/instruments/
+-rw-rw-rw-   0        0        0       47 2023-05-19 21:22:28.000000 srsinst.uga-0.1.0/srsinst/uga/instruments/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-05-19 21:32:52.000000 srsinst.uga-0.1.0/srsinst/uga/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.674432 srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/__init__.py
+-rw-rw-rw-   0        0        0    11021 2023-06-22 00:17:16.000000 srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/components.py
+-rw-rw-rw-   0        0        0     4643 2023-05-24 17:51:21.000000 srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/keys.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 17:42:38.000000 srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/uga.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.674432 srsinst.uga-0.1.0/srsinst/uga/tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:22:28.000000 srsinst.uga-0.1.0/srsinst/uga/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4415 2023-05-24 17:26:46.000000 srsinst.uga-0.1.0/srsinst/uga/tasks/ugamodecontroltask.py
+-rw-rw-rw-   0        0        0     3881 2023-05-19 21:34:42.000000 srsinst.uga-0.1.0/srsinst/uga/tasks/ugamultiplottask.py
+-rw-rw-rw-   0        0        0     1949 2023-05-24 18:32:16.000000 srsinst.uga-0.1.0/srsinst/uga/tasks/ugastatemonitortask.py
+-rw-rw-rw-   0        0        0     2339 2023-05-24 16:25:05.000000 srsinst.uga-0.1.0/srsinst/uga/uga.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-23 00:06:11.664428 srsinst.uga-0.1.0/srsinst.uga.egg-info/
+-rw-rw-rw-   0        0        0     7444 2023-06-23 00:06:11.000000 srsinst.uga-0.1.0/srsinst.uga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-06-23 00:06:11.000000 srsinst.uga-0.1.0/srsinst.uga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 00:06:11.000000 srsinst.uga-0.1.0/srsinst.uga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-23 00:06:11.000000 srsinst.uga-0.1.0/srsinst.uga.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-06-23 00:06:11.000000 srsinst.uga-0.1.0/srsinst.uga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 00:06:11.000000 srsinst.uga-0.1.0/srsinst.uga.egg-info/top_level.txt
```

### Comparing `srsinst.uga-0.0.5/LICENSE` & `srsinst.uga-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/PKG-INFO` & `srsinst.uga-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.5
+Version: 0.1.0
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsinst.uga
 Project-URL: repository, https://github.com/thinkSRS/srsinst.uga.git
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
@@ -189,7 +189,12 @@
 
 Commands in other components can be used in a similar way. 
 
 The most important component in a UGA is the Residual Gas Analyzer, 
 which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
  for its independent usage.
 Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.  
+
+    >>> uga.rga.status.id_string
+    'SRSRGA200VER0.24SN12226'
+    >>> uga.rga.ionizer.emission_current
+    0.9976
```

### Comparing `srsinst.uga-0.0.5/README.md` & `srsinst.uga-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -167,7 +167,12 @@
 
 Commands in other components can be used in a similar way. 
 
 The most important component in a UGA is the Residual Gas Analyzer, 
 which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
  for its independent usage.
 Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.  
+
+    >>> uga.rga.status.id_string
+    'SRSRGA200VER0.24SN12226'
+    >>> uga.rga.ionizer.emission_current
+    0.9976
```

### Comparing `srsinst.uga-0.0.5/docs/_static/image/UGA100_composition_analysis_screenshot.png` & `srsinst.uga-0.1.0/docs/_static/image/UGA100_composition_analysis_screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/pyproject.toml` & `srsinst.uga-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering"
 ]
 dependencies = [
-    "numpy", "scipy", "srsgui>=0.3.3", "srsinst.rga>=0.3.3"
+    "numpy", "scipy", "srsgui>=0.4.0", "srsinst.rga>=0.3.3"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsinst.uga.__version__"}
 
 [project.optional-dependencies]
```

### Comparing `srsinst.uga-0.0.5/srsinst/uga/gaslib.dat` & `srsinst.uga-0.1.0/srsinst/uga/gaslib.dat`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst/uga/instruments/get_instruments.py` & `srsinst.uga-0.1.0/srsinst/uga/instruments/get_instruments.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/components.py` & `srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,15 +125,14 @@
     state = DictCommand('ZCRG', Mode.OffOnDict, Mode.StateDict)
 
     def __init__(self, parent):
         super().__init__()
 
         self._parent = parent
         self._parent._children.append(self)
-        self._add_parent_to_index_commands()
         self.comm = parent.comm
         self.update_components()
 
         if self.comm.is_connected():
             if self.state == Keys.On:
                 self.check_id()
    
@@ -183,16 +182,20 @@
         Keys.Elbow: 0,
         Keys.Chamber: 1,
     }
 
     state = DictCommand('ZCHT', ModeDict, Mode.StateDict)
     bake_time = IntCommand('ZPBT', 'hr.')
     bake_time_remained = IntGetCommand('ZQBR', 'min.')
-    bake_temperature = IntIndexCommand('ZPTB', 1, 0, BakeHeaterDict, '°C')
-    sample_temperature = IntIndexCommand('ZPTH', 3, 0, HeaterDict, '°C')
+
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.bake_temperature = IntIndexCommand('ZPTB', 1, 0, Heaters.BakeHeaterDict, '°C')
+        self.sample_temperature = IntIndexCommand('ZPTH', 3, 0, Heaters.HeaterDict, '°C')
+        self.add_parent_to_index_commands()
 
 
 class Temperature(Component):
     """
     Temperature component contains temperature measurements from 5 sensors.
     If the temperature value is 255, the sensor is not working properly.
     """
@@ -232,17 +235,21 @@
 
     UnitDict = {
         Keys.Torr: 0,
         Keys.Pascal: 1,
         Keys.MilliBar: 2,
         Keys.Bar: 3
     }
-    values = IntIndexGetCommand('ZQAD', 3, 0, GaugeDict)
     display_unit = DictCommand('ZPPU', UnitDict)
 
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.values = IntIndexGetCommand('ZQAD', 3, 0, Pressure.GaugeDict)
+        self.add_parent_to_index_commands()
+
 
 class Ethernet(Component):
     mac_address = GetCommand('ZQMC')
     ip_address = Command('ZPIP')
     gateway = Command('ZPGW')
     subnet_mask = Command('ZPSM')
     login = Command('ZPNM')
@@ -283,17 +290,21 @@
     baud_rate = IntCommand('ZPBA')
 
     states = IntGetCommand('ZBST')
     changed = IntGetCommand('ZBCT')
     changing = IntGetCommand('ZBTT')
     error = DictGetCommand('ZERR', Keys.ErrorMessageDict)
     error_number = IntGetCommand('ZERR')
-    error_message = IndexGetCommand('ZEDS', index_max=126)
 
-    exclude_capture = [error_number, error_message]
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.error_message = IndexGetCommand('ZEDS', index_max=126)
+        self.add_parent_to_index_commands()
+
+        self.exclude_capture = [Status.error_number, self.error_message]
 
     def get_status_text(self):
         out_buffer = ''
         error_buffer = 'Errors: '
         item_line_format = '{}: {} \n'
         
         states = self.states
```

### Comparing `srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/keys.py` & `srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/keys.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst/uga/instruments/uga100/uga.py` & `srsinst.uga-0.1.0/srsinst/uga/instruments/uga100/uga.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst/uga/tasks/ugamodecontroltask.py` & `srsinst.uga-0.1.0/srsinst/uga/tasks/ugamodecontroltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst/uga/tasks/ugamultiplottask.py` & `srsinst.uga-0.1.0/srsinst/uga/tasks/ugamultiplottask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst/uga/tasks/ugastatemonitortask.py` & `srsinst.uga-0.1.0/srsinst/uga/tasks/ugastatemonitortask.py`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst/uga/uga.taskconfig` & `srsinst.uga-0.1.0/srsinst/uga/uga.taskconfig`

 * *Files identical despite different names*

### Comparing `srsinst.uga-0.0.5/srsinst.uga.egg-info/PKG-INFO` & `srsinst.uga-0.1.0/srsinst.uga.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.uga
-Version: 0.0.5
+Version: 0.1.0
 Summary: Instrument driver package for Universal Gas Analyzers (UGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsinst.uga
 Project-URL: repository, https://github.com/thinkSRS/srsinst.uga.git
 Keywords: UGA,universal gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
@@ -189,7 +189,12 @@
 
 Commands in other components can be used in a similar way. 
 
 The most important component in a UGA is the Residual Gas Analyzer, 
 which has the separate [RGA instrument driver package](https://github.com/thinkSRS/srsinst.rga)
  for its independent usage.
 Refer to [RGA documentation](https://thinksrs.github.io/srsinst.rga/) for RGA component usage.  
+
+    >>> uga.rga.status.id_string
+    'SRSRGA200VER0.24SN12226'
+    >>> uga.rga.ionizer.emission_current
+    0.9976
```

