# Comparing `tmp/srsinst.sr542-0.0.3.tar.gz` & `tmp/srsinst.sr542-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument drivers to GIT\sr542\dist\.tmp-0f6314b7\srsinst.sr542-0.0.3.tar", last modified: Tue Apr  4 16:48:11 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument drivers to GIT\sr542\dist\.tmp-vpln9xgx\srsinst.sr542-0.0.4.tar", last modified: Thu Jun 22 23:39:49 2023, max compression
```

## Comparing `srsinst.sr542-0.0.3.tar` & `srsinst.sr542-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 16:48:11.605201 srsinst.sr542-0.0.3/
--rw-rw-rw-   0        0        0     1968 2023-02-10 18:32:29.000000 srsinst.sr542-0.0.3/.gitignore
--rw-rw-rw-   0        0        0     1109 2023-02-22 20:10:02.000000 srsinst.sr542-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      979 2023-04-04 16:48:11.604190 srsinst.sr542-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-02-22 18:05:50.000000 srsinst.sr542-0.0.3/README.md
--rw-rw-rw-   0        0        0     1185 2023-02-22 18:11:17.000000 srsinst.sr542-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 16:48:11.605201 srsinst.sr542-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-02-22 20:10:14.000000 srsinst.sr542-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 16:48:11.580952 srsinst.sr542-0.0.3/srsinst/
-drwxrwxrwx   0        0        0        0 2023-04-04 16:48:11.590134 srsinst.sr542-0.0.3/srsinst/sr542/
--rw-rw-rw-   0        0        0      141 2023-04-04 16:46:47.000000 srsinst.sr542-0.0.3/srsinst/sr542/__init__.py
--rw-rw-rw-   0        0        0      485 2023-02-22 18:12:00.000000 srsinst.sr542-0.0.3/srsinst/sr542/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 16:48:11.600132 srsinst.sr542-0.0.3/srsinst/sr542/instruments/
--rw-rw-rw-   0        0        0     5526 2023-02-25 00:14:44.000000 srsinst.sr542-0.0.3/srsinst/sr542/instruments/components.py
--rw-rw-rw-   0        0        0      704 2023-02-24 22:33:47.000000 srsinst.sr542-0.0.3/srsinst/sr542/instruments/get_instruments.py
--rw-rw-rw-   0        0        0     1005 2023-02-24 22:33:04.000000 srsinst.sr542-0.0.3/srsinst/sr542/instruments/keys.py
--rw-rw-rw-   0        0        0     1111 2023-02-24 18:57:33.000000 srsinst.sr542-0.0.3/srsinst/sr542/instruments/sr542.py
--rw-rw-rw-   0        0        0       62 2023-02-22 20:14:03.000000 srsinst.sr542-0.0.3/srsinst/sr542/sr542.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-04 16:48:11.590134 srsinst.sr542-0.0.3/srsinst.sr542.egg-info/
--rw-rw-rw-   0        0        0      979 2023-04-04 16:48:11.000000 srsinst.sr542-0.0.3/srsinst.sr542.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-04-04 16:48:11.000000 srsinst.sr542-0.0.3/srsinst.sr542.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 16:48:11.000000 srsinst.sr542-0.0.3/srsinst.sr542.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-04 16:48:11.000000 srsinst.sr542-0.0.3/srsinst.sr542.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-04-04 16:48:11.000000 srsinst.sr542-0.0.3/srsinst.sr542.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-04 16:48:11.000000 srsinst.sr542-0.0.3/srsinst.sr542.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/
+-rw-rw-rw-   0        0        0     1968 2023-02-10 18:32:29.000000 srsinst.sr542-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1109 2023-02-22 20:10:02.000000 srsinst.sr542-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      979 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-02-22 18:05:50.000000 srsinst.sr542-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1184 2023-06-21 20:03:57.000000 srsinst.sr542-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-02-22 20:10:14.000000 srsinst.sr542-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.056980 srsinst.sr542-0.0.4/srsinst/
+drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.080111 srsinst.sr542-0.0.4/srsinst/sr542/
+-rw-rw-rw-   0        0        0      141 2023-06-22 23:38:27.000000 srsinst.sr542-0.0.4/srsinst/sr542/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-02-22 18:12:00.000000 srsinst.sr542-0.0.4/srsinst/sr542/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.090114 srsinst.sr542-0.0.4/srsinst/sr542/instruments/
+-rw-rw-rw-   0        0        0     6234 2023-06-21 21:19:56.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/components.py
+-rw-rw-rw-   0        0        0      699 2023-04-06 22:20:23.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/get_instruments.py
+-rw-rw-rw-   0        0        0     1005 2023-02-24 22:33:04.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/keys.py
+-rw-rw-rw-   0        0        0     1111 2023-02-24 18:57:33.000000 srsinst.sr542-0.0.4/srsinst/sr542/instruments/sr542.py
+-rw-rw-rw-   0        0        0     1270 2023-02-23 00:10:07.000000 srsinst.sr542-0.0.4/srsinst/sr542/sr542 with sr860.taskconfig
+-rw-rw-rw-   0        0        0       62 2023-02-22 20:14:03.000000 srsinst.sr542-0.0.4/srsinst/sr542/sr542.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-22 23:39:49.080111 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/
+-rw-rw-rw-   0        0        0      979 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-22 23:39:49.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 23:39:48.000000 srsinst.sr542-0.0.4/srsinst.sr542.egg-info/top_level.txt
```

### Comparing `srsinst.sr542-0.0.3/.gitignore` & `srsinst.sr542-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.3/LICENSE.txt` & `srsinst.sr542-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.3/PKG-INFO` & `srsinst.sr542-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.sr542
-Version: 0.0.3
+Version: 0.0.4
 Summary: Instrument driver package for precision optical chopper SR542 from Stanford Research Systems
 Author: Chulhoon Kim, Andrew Berger
 License: MIT license
 Keywords: SR542,SRS,Stanford Research Systems,optical chopper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsinst.sr542-0.0.3/pyproject.toml` & `srsinst.sr542-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering"
 ]
 dependencies = [
-    "numpy", "srsgui>=0.1.21",
+    "numpy", "srsgui>=0.4.0",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsinst.sr542.__version__"}
 
 [project.optional-dependencies]
```

### Comparing `srsinst.sr542-0.0.3/srsinst/sr542/instruments/components.py` & `srsinst.sr542-0.0.4/srsinst/sr542/instruments/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
-from srsgui.inst.component import Component
-from srsgui.inst.commands import Command, GetCommand,\
-                                 BoolCommand, BoolGetCommand,\
-                                 IntCommand, IntGetCommand, IntSetCommand,\
-                                 FloatCommand, FloatSetCommand, FloatGetCommand, \
-                                 DictCommand, DictGetCommand
-from srsgui.inst.indexcommands import IndexCommand, IndexGetCommand, \
-                                      IntIndexCommand, IntIndexGetCommand, \
-                                      BoolIndexCommand, BoolIndexGetCommand,\
-                                      FloatIndexCommand, FloatIndexGetCommand, \
-                                      DictIndexCommand
+from srsgui import Component
+from srsgui import Command, GetCommand,\
+                   BoolCommand, BoolGetCommand,\
+                   IntCommand, IntGetCommand, IntSetCommand,\
+                   FloatCommand, FloatSetCommand, FloatGetCommand, \
+                   DictCommand, DictGetCommand
+from srsgui import IndexCommand, IndexGetCommand, \
+                   IntIndexCommand, IntIndexGetCommand, \
+                   BoolIndexCommand, BoolIndexGetCommand,\
+                   FloatIndexCommand, FloatIndexGetCommand, \
+                   DictIndexCommand
 from .keys import Keys
 
 
 class Config(Component):
     SourceDict = {
         Keys.INTERNAL: 0,
         Keys.VCO: 1,
@@ -21,37 +21,37 @@
         Keys.EXTERNAL: 3
     }
     EdgeDict = {
         Keys.RISE: 0,
         Keys.FALL: 1,
         Keys.SINE: 2,
     }
-    
+
     ControlTargetDict = {
         Keys.SHAFT: 0,
         Keys.INNER: 1,
         Keys.OUTER: 2
     }
-    
+
     source = DictCommand('SRCE', SourceDict)
     sync_edge = DictCommand('EDGE', EdgeDict)
     control_target = DictCommand('CTRL', ControlTargetDict)
-    frequency = FloatCommand('IFRQ')
-    phase = FloatCommand('PHAS')
+    internal_freq = FloatCommand('IFRQ', 'Hz')
+    phase = FloatCommand('PHAS', '°')
     relative_phase = BoolCommand('RELP')
     multiplier = IntCommand('MULT')
     divisor = IntCommand('DIVR')
-    vco_frequency = FloatCommand('VCOS')
-    
+    vco_frequency = FloatCommand('VCOS', 'Hz')
+
     def jump_to_internal_frequency(self):
         self.comm.send('JINT')
 
-    
+
 class Operate(Component):
-    OffOnDict ={
+    OffOnDict = {
         Keys.OFF: 0,
         Keys.ON:  1
     }
     SlotDict = {
         Keys.INNER: 0,
         Keys.OUTER: 1
     }
@@ -61,16 +61,20 @@
         Keys.SHAFT: 2,
         Keys.SOURCE: 3,
         Keys.SUM: 4,
         Keys.DIFF: 5,
         Keys.CTRL: 6,
     }
     motor_state = DictCommand('MOTR', OffOnDict)
-    frequency_monitor = FloatIndexCommand('MFRQ', 6, 0, FrequencyMonitorDict)
-    slots = IntIndexGetCommand('SLOT', 1, 0, SlotDict)
+
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.frequency_monitor = FloatIndexCommand('MFRQ', 6, 0, Operate.FrequencyMonitorDict)
+        self.slots = IntIndexGetCommand('SLOT', 1, 0, Operate.SlotDict)
+        self.add_parent_to_index_commands()
 
     def run(self):
         self.motor_state = Keys.ON
 
     def stop(self):
         self.motor_state = Keys.OFF
 
@@ -87,29 +91,29 @@
         Keys.DIVM: 7,
         Keys.VCOFS: 8
     }
 
     display_mode = DictCommand('DISP', DisplayDict)
     alarm = DictCommand('ALRM', Operate.OffOnDict)
     key_click = DictCommand('KCLK', Operate.OffOnDict)
-    
+
     def save(self, location):
         self.comm.send('*SAV {}'.format(location))
-        
+
     def recall(self, location):
         self.comm.send('*RCL {}'.format(location))
-        
+
     def revert(self):
         self.comm.send('BACK')
 
 
 class Interface(Component):
     id_string = GetCommand('*IDN')
     operation_complete = BoolGetCommand('*OPC')
-    
+
     def cancel_pending_operation_complete(self):
         self.comm.send('COPC')
 
 
 class Status(Component):
     SerialPollStatusBitDict = {
         Keys.ESB: 5,
@@ -131,44 +135,48 @@
         Keys.EL: 1,
         Keys.FL: 2,
         Keys.PL: 3,
         Keys.CMAX: 4,
         Keys.TMAX: 5
     }
     ChopperEventBitDict = {
+        Keys.MON: 0,
+        Keys.EL: 1,
+        Keys.FL: 2,
+        Keys.PL: 3,
+        Keys.CMAX: 4,
+        Keys.TMAX: 5,
         Keys.ChopperHeadMemoryFail: 6,
         Keys.ChopperHeadDisconnect: 7
     }
 
     last_error = IntCommand('LERR')
-
     status_byte = IntGetCommand('*STB')
-    status_bit = BoolIndexGetCommand('*STB', 7, 0)
-
-    status_enable = IntCommand('*SRE')
-    status_enable_bit = BoolIndexCommand('*SRE', 7, 0)
-
+    status_enable_byte = IntCommand('*SRE')
     event_status_byte = IntGetCommand('*ESR')
-    event_status_bit = BoolIndexGetCommand('*ESR', 7, 0)
-
-    event_enable = IntCommand('*ESE')
-    event_enable_bit = BoolIndexCommand('*ESE', 7, 0)
-
+    event_enable_byte = IntCommand('*ESE')
     chopper_condition_byte = IntGetCommand('CHCR')
-    chopper_condition_bit = BoolGetCommand('CHCR')
-
     chopper_condition_positive_transition_byte = IntCommand('CHPT')
     chopper_condition_negative_transition_byte = IntCommand('CHNT')
-
     chopper_event_byte = IntGetCommand('CHEV')
-    chopper_event_bit = BoolIndexGetCommand('CHEV', 7, 0)
-
     chopper_event_enable = IntCommand('CHEN')
-    chopper_event_enable_bit = BoolIndexCommand('CHEN', 7, 0)
-    
+
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.status_bit = BoolIndexGetCommand('*STB', 7, 0, Status.SerialPollStatusBitDict)
+        self.status_enable_bit = BoolIndexCommand('*SRE', 7, 0, Status.SerialPollStatusBitDict)
+        self.event_status_bit = BoolIndexGetCommand('*ESR', 7, 0, Status.EventStatusBitDict)
+        self.event_enable_bit = BoolIndexCommand('*ESE', 7, 0, Status.EventStatusBitDict)
+        self.chopper_condition_bit = BoolIndexGetCommand('CHCR', 5, 0, Status.ChopperConditionBitDict)
+        self.chopper_condition_positive_transition_bit = BoolIndexCommand('CHPT', 5, 0, Status.ChopperConditionBitDict)
+        self.chopper_condition_negative_transition_bit = BoolIndexCommand('CHNT', 5, 0, Status.ChopperConditionBitDict)
+        self.chopper_event_bit = BoolIndexGetCommand('CHEV', 7, 0, Status.ChopperEventBitDict)
+        self.chopper_event_enable_bit = BoolIndexCommand('CHEN', 7, 0, Status.ChopperEventBitDict)
+        self.add_parent_to_index_commands()
+
     def clear(self):
         self.comm.send('*CLS')
 
     def get_status_text(self):
         msg = ''
         status_byte = self.status_byte
         if self.SerialPollStatusBitDict[Keys.ESB]:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `srsinst.sr542-0.0.3/srsinst/sr542/instruments/get_instruments.py` & `srsinst.sr542-0.0.4/srsinst/sr542/instruments/get_instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from srsgui.task import Task
+from srsgui import Task
 from .sr542 import SR542
 
 logger = logging.getLogger(__name__)
 
 
 def get_sr542(task: Task, name=None) -> SR542:
     """
```

### Comparing `srsinst.sr542-0.0.3/srsinst/sr542/instruments/keys.py` & `srsinst.sr542-0.0.4/srsinst/sr542/instruments/keys.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.3/srsinst/sr542/instruments/sr542.py` & `srsinst.sr542-0.0.4/srsinst/sr542/instruments/sr542.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr542-0.0.3/srsinst.sr542.egg-info/PKG-INFO` & `srsinst.sr542-0.0.4/srsinst.sr542.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.sr542
-Version: 0.0.3
+Version: 0.0.4
 Summary: Instrument driver package for precision optical chopper SR542 from Stanford Research Systems
 Author: Chulhoon Kim, Andrew Berger
 License: MIT license
 Keywords: SR542,SRS,Stanford Research Systems,optical chopper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsinst.sr542-0.0.3/srsinst.sr542.egg-info/SOURCES.txt` & `srsinst.sr542-0.0.4/srsinst.sr542.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 srsinst.sr542.egg-info/SOURCES.txt
 srsinst.sr542.egg-info/dependency_links.txt
 srsinst.sr542.egg-info/entry_points.txt
 srsinst.sr542.egg-info/requires.txt
 srsinst.sr542.egg-info/top_level.txt
 srsinst/sr542/__init__.py
 srsinst/sr542/__main__.py
+srsinst/sr542/sr542 with sr860.taskconfig
 srsinst/sr542/sr542.taskconfig
 srsinst/sr542/instruments/components.py
 srsinst/sr542/instruments/get_instruments.py
 srsinst/sr542/instruments/keys.py
 srsinst/sr542/instruments/sr542.py
```

