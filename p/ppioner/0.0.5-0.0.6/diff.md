# Comparing `tmp/ppioner-0.0.5.tar.gz` & `tmp/ppioner-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppioner-0.0.5.tar", last modified: Fri Jun 23 09:38:51 2023, max compression
+gzip compressed data, was "ppioner-0.0.6.tar", last modified: Fri Jun 23 09:47:41 2023, max compression
```

## Comparing `ppioner-0.0.5.tar` & `ppioner-0.0.6.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.479173 ppioner-0.0.5/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:31:35.000000 ppioner-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1297 2023-06-23 09:38:51.479173 ppioner-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-06-22 09:12:07.000000 ppioner-0.0.5/README.md
--rw-rw-rw-   0        0        0     1008 2023-06-23 09:36:31.000000 ppioner-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 09:38:51.479173 ppioner-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.438174 ppioner-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.443174 ppioner-0.0.5/src/pioner/
--rw-rw-rw-   0        0        0       17 2023-06-22 07:37:28.000000 ppioner-0.0.5/src/pioner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.444172 ppioner-0.0.5/src/pioner/assets/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.5/src/pioner/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.456173 ppioner-0.0.5/src/pioner/back/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.5/src/pioner/back/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-06-22 07:25:36.000000 ppioner-0.0.5/src/pioner/back/ai_device.py
--rw-rw-rw-   0        0        0     4186 2023-06-22 07:25:36.000000 ppioner-0.0.5/src/pioner/back/ao_data_generators.py
--rw-rw-rw-   0        0        0     2845 2023-06-22 07:25:36.000000 ppioner-0.0.5/src/pioner/back/ao_device.py
--rw-rw-rw-   0        0        0     3416 2023-06-22 07:25:36.000000 ppioner-0.0.5/src/pioner/back/daq_device.py
--rw-rw-rw-   0        0        0     3031 2023-06-22 07:41:21.000000 ppioner-0.0.5/src/pioner/back/debug.py
--rw-rw-rw-   0        0        0    10394 2023-06-22 07:41:46.000000 ppioner-0.0.5/src/pioner/back/experiment_manager.py
--rw-rw-rw-   0        0        0     9782 2023-06-22 07:42:19.000000 ppioner-0.0.5/src/pioner/back/fastheat.py
--rw-rw-rw-   0        0        0     2395 2023-06-22 07:42:20.000000 ppioner-0.0.5/src/pioner/back/iso_mode.py
--rw-rw-rw-   0        0        0     6830 2023-06-22 07:42:20.000000 ppioner-0.0.5/src/pioner/back/nanocontrol_tango.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.467175 ppioner-0.0.5/src/pioner/front/
--rw-rw-rw-   0        0        0    34303 2023-06-22 07:25:36.000000 ppioner-0.0.5/src/pioner/front/SetProg_widget.py
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.5/src/pioner/front/__init__.py
--rw-rw-rw-   0        0        0    17651 2023-06-22 07:49:40.000000 ppioner-0.0.5/src/pioner/front/calibWindow.py
--rw-rw-rw-   0        0        0     5639 2023-06-22 07:49:54.000000 ppioner-0.0.5/src/pioner/front/configWindow.py
--rw-rw-rw-   0        0        0    15454 2023-06-23 09:35:26.000000 ppioner-0.0.5/src/pioner/front/mainWindow.py
--rw-rw-rw-   0        0        0    28411 2023-06-22 09:13:29.000000 ppioner-0.0.5/src/pioner/front/mainWindowUi.py
--rw-rw-rw-   0        0        0     1058 2023-04-17 10:43:41.000000 ppioner-0.0.5/src/pioner/front/messageWindows.py
--rw-rw-rw-   0        0        0    36341 2023-06-22 07:51:08.000000 ppioner-0.0.5/src/pioner/front/procFastHeatWidget.py
--rw-rw-rw-   0        0        0    16086 2023-06-22 07:51:35.000000 ppioner-0.0.5/src/pioner/front/resultsDataWidget.py
--rw-rw-rw-   0        0        0      940 2023-04-17 10:43:41.000000 ppioner-0.0.5/src/pioner/front/virtualDevice.py
--rw-rw-rw-   0        0        0      325 2023-06-22 09:20:13.000000 ppioner-0.0.5/src/pioner/runUI.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.473171 ppioner-0.0.5/src/pioner/shared/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.5/src/pioner/shared/__init__.py
--rw-rw-rw-   0        0        0     9194 2023-06-22 12:23:54.000000 ppioner-0.0.5/src/pioner/shared/calibration.py
--rw-rw-rw-   0        0        0     3819 2023-06-23 09:33:14.000000 ppioner-0.0.5/src/pioner/shared/constants.py
--rw-rw-rw-   0        0        0    14061 2023-06-23 09:06:34.000000 ppioner-0.0.5/src/pioner/shared/settings.py
--rw-rw-rw-   0        0        0     2394 2023-06-22 12:15:47.000000 ppioner-0.0.5/src/pioner/shared/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:38:51.478171 ppioner-0.0.5/src/ppioner.egg-info/
--rw-rw-rw-   0        0        0     1297 2023-06-23 09:38:51.000000 ppioner-0.0.5/src/ppioner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1117 2023-06-23 09:38:51.000000 ppioner-0.0.5/src/ppioner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:38:51.000000 ppioner-0.0.5/src/ppioner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-23 09:38:51.000000 ppioner-0.0.5/src/ppioner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      229 2023-06-23 09:38:51.000000 ppioner-0.0.5/src/ppioner.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 09:38:51.000000 ppioner-0.0.5/src/ppioner.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.431937 ppioner-0.0.6/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:31:35.000000 ppioner-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1297 2023-06-23 09:47:41.431937 ppioner-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-06-22 09:12:07.000000 ppioner-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1008 2023-06-23 09:47:09.000000 ppioner-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 09:47:41.431937 ppioner-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.385949 ppioner-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.393966 ppioner-0.0.6/src/pioner/
+-rw-rw-rw-   0        0        0       17 2023-06-22 07:37:28.000000 ppioner-0.0.6/src/pioner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.394937 ppioner-0.0.6/src/pioner/assets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.6/src/pioner/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.405937 ppioner-0.0.6/src/pioner/back/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.6/src/pioner/back/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-06-22 07:25:36.000000 ppioner-0.0.6/src/pioner/back/ai_device.py
+-rw-rw-rw-   0        0        0     4186 2023-06-22 07:25:36.000000 ppioner-0.0.6/src/pioner/back/ao_data_generators.py
+-rw-rw-rw-   0        0        0     2845 2023-06-22 07:25:36.000000 ppioner-0.0.6/src/pioner/back/ao_device.py
+-rw-rw-rw-   0        0        0     3416 2023-06-22 07:25:36.000000 ppioner-0.0.6/src/pioner/back/daq_device.py
+-rw-rw-rw-   0        0        0     3031 2023-06-22 07:41:21.000000 ppioner-0.0.6/src/pioner/back/debug.py
+-rw-rw-rw-   0        0        0    10394 2023-06-22 07:41:46.000000 ppioner-0.0.6/src/pioner/back/experiment_manager.py
+-rw-rw-rw-   0        0        0     9782 2023-06-22 07:42:19.000000 ppioner-0.0.6/src/pioner/back/fastheat.py
+-rw-rw-rw-   0        0        0     2395 2023-06-22 07:42:20.000000 ppioner-0.0.6/src/pioner/back/iso_mode.py
+-rw-rw-rw-   0        0        0     6830 2023-06-22 07:42:20.000000 ppioner-0.0.6/src/pioner/back/nanocontrol_tango.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.417940 ppioner-0.0.6/src/pioner/front/
+-rw-rw-rw-   0        0        0    34303 2023-06-22 07:25:36.000000 ppioner-0.0.6/src/pioner/front/SetProg_widget.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.6/src/pioner/front/__init__.py
+-rw-rw-rw-   0        0        0    17651 2023-06-22 07:49:40.000000 ppioner-0.0.6/src/pioner/front/calibWindow.py
+-rw-rw-rw-   0        0        0     5639 2023-06-22 07:49:54.000000 ppioner-0.0.6/src/pioner/front/configWindow.py
+-rw-rw-rw-   0        0        0    15454 2023-06-23 09:35:26.000000 ppioner-0.0.6/src/pioner/front/mainWindow.py
+-rw-rw-rw-   0        0        0    28411 2023-06-22 09:13:29.000000 ppioner-0.0.6/src/pioner/front/mainWindowUi.py
+-rw-rw-rw-   0        0        0     1058 2023-04-17 10:43:41.000000 ppioner-0.0.6/src/pioner/front/messageWindows.py
+-rw-rw-rw-   0        0        0    36341 2023-06-22 07:51:08.000000 ppioner-0.0.6/src/pioner/front/procFastHeatWidget.py
+-rw-rw-rw-   0        0        0    16086 2023-06-22 07:51:35.000000 ppioner-0.0.6/src/pioner/front/resultsDataWidget.py
+-rw-rw-rw-   0        0        0      940 2023-04-17 10:43:41.000000 ppioner-0.0.6/src/pioner/front/virtualDevice.py
+-rw-rw-rw-   0        0        0      325 2023-06-22 09:20:13.000000 ppioner-0.0.6/src/pioner/runUI.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.418937 ppioner-0.0.6/src/pioner/settings/
+-rw-rw-rw-   0        0        0        0 2023-06-23 09:46:27.000000 ppioner-0.0.6/src/pioner/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.424938 ppioner-0.0.6/src/pioner/shared/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:36:31.000000 ppioner-0.0.6/src/pioner/shared/__init__.py
+-rw-rw-rw-   0        0        0     9194 2023-06-22 12:23:54.000000 ppioner-0.0.6/src/pioner/shared/calibration.py
+-rw-rw-rw-   0        0        0     3819 2023-06-23 09:33:14.000000 ppioner-0.0.6/src/pioner/shared/constants.py
+-rw-rw-rw-   0        0        0    14061 2023-06-23 09:06:34.000000 ppioner-0.0.6/src/pioner/shared/settings.py
+-rw-rw-rw-   0        0        0     2394 2023-06-22 12:15:47.000000 ppioner-0.0.6/src/pioner/shared/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:47:41.430937 ppioner-0.0.6/src/ppioner.egg-info/
+-rw-rw-rw-   0        0        0     1297 2023-06-23 09:47:41.000000 ppioner-0.0.6/src/ppioner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1149 2023-06-23 09:47:41.000000 ppioner-0.0.6/src/ppioner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 09:47:41.000000 ppioner-0.0.6/src/ppioner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-23 09:47:41.000000 ppioner-0.0.6/src/ppioner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      229 2023-06-23 09:47:41.000000 ppioner-0.0.6/src/ppioner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 09:47:41.000000 ppioner-0.0.6/src/ppioner.egg-info/top_level.txt
```

### Comparing `ppioner-0.0.5/PKG-INFO` & `ppioner-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppioner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Basic software to operate PIONER device (former Nanocal)
 Author-email: awesome author <awesome@author.edu>
 License: MIT
 Keywords: nanocalorimetry,DAQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ppioner-0.0.5/README.md` & `ppioner-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/pyproject.toml` & `ppioner-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0", 
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ppioner"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "awesome author", email = "awesome@author.edu"},
 ]
 description = "Basic software to operate PIONER device (former Nanocal)"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["nanocalorimetry", "DAQ"]
```

### Comparing `ppioner-0.0.5/src/pioner/back/ai_device.py` & `ppioner-0.0.6/src/pioner/back/ai_device.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/ao_data_generators.py` & `ppioner-0.0.6/src/pioner/back/ao_data_generators.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/ao_device.py` & `ppioner-0.0.6/src/pioner/back/ao_device.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/daq_device.py` & `ppioner-0.0.6/src/pioner/back/daq_device.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/debug.py` & `ppioner-0.0.6/src/pioner/back/debug.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/experiment_manager.py` & `ppioner-0.0.6/src/pioner/back/experiment_manager.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/fastheat.py` & `ppioner-0.0.6/src/pioner/back/fastheat.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/iso_mode.py` & `ppioner-0.0.6/src/pioner/back/iso_mode.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/back/nanocontrol_tango.py` & `ppioner-0.0.6/src/pioner/back/nanocontrol_tango.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/SetProg_widget.py` & `ppioner-0.0.6/src/pioner/front/SetProg_widget.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/calibWindow.py` & `ppioner-0.0.6/src/pioner/front/calibWindow.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/configWindow.py` & `ppioner-0.0.6/src/pioner/front/configWindow.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/mainWindow.py` & `ppioner-0.0.6/src/pioner/front/mainWindow.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/mainWindowUi.py` & `ppioner-0.0.6/src/pioner/front/mainWindowUi.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/messageWindows.py` & `ppioner-0.0.6/src/pioner/front/messageWindows.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/procFastHeatWidget.py` & `ppioner-0.0.6/src/pioner/front/procFastHeatWidget.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/resultsDataWidget.py` & `ppioner-0.0.6/src/pioner/front/resultsDataWidget.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/front/virtualDevice.py` & `ppioner-0.0.6/src/pioner/front/virtualDevice.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/shared/calibration.py` & `ppioner-0.0.6/src/pioner/shared/calibration.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/shared/constants.py` & `ppioner-0.0.6/src/pioner/shared/constants.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/shared/settings.py` & `ppioner-0.0.6/src/pioner/shared/settings.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/pioner/shared/utils.py` & `ppioner-0.0.6/src/pioner/shared/utils.py`

 * *Files identical despite different names*

### Comparing `ppioner-0.0.5/src/ppioner.egg-info/PKG-INFO` & `ppioner-0.0.6/src/ppioner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppioner
-Version: 0.0.5
+Version: 0.0.6
 Summary: Basic software to operate PIONER device (former Nanocal)
 Author-email: awesome author <awesome@author.edu>
 License: MIT
 Keywords: nanocalorimetry,DAQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ppioner-0.0.5/src/ppioner.egg-info/SOURCES.txt` & `ppioner-0.0.6/src/ppioner.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/pioner/front/configWindow.py
 src/pioner/front/mainWindow.py
 src/pioner/front/mainWindowUi.py
 src/pioner/front/messageWindows.py
 src/pioner/front/procFastHeatWidget.py
 src/pioner/front/resultsDataWidget.py
 src/pioner/front/virtualDevice.py
+src/pioner/settings/__init__.py
 src/pioner/shared/__init__.py
 src/pioner/shared/calibration.py
 src/pioner/shared/constants.py
 src/pioner/shared/settings.py
 src/pioner/shared/utils.py
 src/ppioner.egg-info/PKG-INFO
 src/ppioner.egg-info/SOURCES.txt
```

