# Comparing `tmp/pyLauda-1.0.2.tar.gz` & `tmp/pyLauda-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLauda-1.0.2.tar", last modified: Tue Mar  8 21:04:38 2022, max compression
+gzip compressed data, was "pyLauda-1.0.3.tar", last modified: Fri Jun 23 04:13:06 2023, max compression
```

## Comparing `pyLauda-1.0.2.tar` & `pyLauda-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2022-03-08 21:04:38.818996 pyLauda-1.0.2/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     1080 2022-03-08 20:35:08.000000 pyLauda-1.0.2/LICENSE
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      630 2022-03-08 21:04:38.818996 pyLauda-1.0.2/PKG-INFO
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)      514 2020-04-26 16:23:17.000000 pyLauda-1.0.2/README.md
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2022-03-08 21:04:38.814996 pyLauda-1.0.2/pyLauda/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)      117 2022-03-08 20:47:45.000000 pyLauda-1.0.2/pyLauda/__init__.py
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     6337 2022-03-08 20:32:26.000000 pyLauda-1.0.2/pyLauda/re206.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)    10266 2022-03-08 20:34:44.000000 pyLauda-1.0.2/pyLauda/variocool.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2022-03-08 21:04:38.814996 pyLauda-1.0.2/pyLauda.egg-info/
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      630 2022-03-08 21:04:38.000000 pyLauda-1.0.2/pyLauda.egg-info/PKG-INFO
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      283 2022-03-08 21:04:38.000000 pyLauda-1.0.2/pyLauda.egg-info/SOURCES.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2022-03-08 21:04:38.000000 pyLauda-1.0.2/pyLauda.egg-info/dependency_links.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        9 2022-03-08 21:04:38.000000 pyLauda-1.0.2/pyLauda.egg-info/requires.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        8 2022-03-08 21:04:38.000000 pyLauda-1.0.2/pyLauda.egg-info/top_level.txt
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      447 2022-03-08 21:04:38.818996 pyLauda-1.0.2/setup.cfg
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     1181 2022-03-08 21:00:01.000000 pyLauda-1.0.2/setup.py
-drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2022-03-08 21:04:38.818996 pyLauda-1.0.2/test/
--rw-r--r--   0 niehaus   (1000) niehaus   (1000)     1752 2020-04-26 16:23:17.000000 pyLauda-1.0.2/test/test_re206.py
--rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1378 2022-03-08 20:24:52.000000 pyLauda-1.0.2/test/test_vc.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-23 04:13:06.310816 pyLauda-1.0.3/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     2514 2022-03-28 18:30:10.000000 pyLauda-1.0.3/.gitignore
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      164 2022-03-28 18:30:10.000000 pyLauda-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       52 2020-04-22 17:40:59.000000 pyLauda-1.0.3/DESCRIPTION.rst
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     1075 2020-04-22 17:52:04.000000 pyLauda-1.0.3/LICENSE
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      582 2023-06-23 04:13:06.310816 pyLauda-1.0.3/PKG-INFO
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)      514 2020-04-22 17:51:55.000000 pyLauda-1.0.3/README.md
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-23 04:13:06.310816 pyLauda-1.0.3/doc/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)  1819510 2020-01-16 18:12:06.000000 pyLauda-1.0.3/doc/Variocool.pdf
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)   670789 2020-01-16 17:48:47.000000 pyLauda-1.0.3/doc/ecoline_re_204.pdf
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-23 04:13:06.310816 pyLauda-1.0.3/pyLauda/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)        0 2020-04-22 17:42:49.000000 pyLauda-1.0.3/pyLauda/__init__.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     6349 2022-03-28 18:30:10.000000 pyLauda-1.0.3/pyLauda/re206.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     9208 2023-06-17 15:42:32.000000 pyLauda-1.0.3/pyLauda/variocool.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-23 04:13:06.310816 pyLauda-1.0.3/pyLauda.egg-info/
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      582 2023-06-23 04:13:06.000000 pyLauda-1.0.3/pyLauda.egg-info/PKG-INFO
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)      374 2023-06-23 04:13:06.000000 pyLauda-1.0.3/pyLauda.egg-info/SOURCES.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        1 2023-06-23 04:13:06.000000 pyLauda-1.0.3/pyLauda.egg-info/dependency_links.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       14 2023-06-23 04:13:06.000000 pyLauda-1.0.3/pyLauda.egg-info/requires.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)        8 2023-06-23 04:13:06.000000 pyLauda-1.0.3/pyLauda.egg-info/top_level.txt
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)       39 2022-03-28 19:00:06.000000 pyLauda-1.0.3/requirements.txt
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)       38 2023-06-23 04:13:06.310816 pyLauda-1.0.3/setup.cfg
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     3501 2023-06-23 04:12:57.000000 pyLauda-1.0.3/setup.py
+drwxrwxr-x   0 niehaus   (1000) niehaus   (1000)        0 2023-06-23 04:13:06.310816 pyLauda-1.0.3/test/
+-rw-r--r--   0 niehaus   (1000) niehaus   (1000)     1752 2020-01-16 17:48:47.000000 pyLauda-1.0.3/test/test_re206.py
+-rw-rw-r--   0 niehaus   (1000) niehaus   (1000)     1378 2022-03-28 18:30:10.000000 pyLauda-1.0.3/test/test_vc.py
```

### Comparing `pyLauda-1.0.2/LICENSE` & `pyLauda-1.0.3/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 German Aerospace Center
+Copyright (c) 2020 Konstantin Niehaus
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyLauda-1.0.2/README.md` & `pyLauda-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyLauda-1.0.2/pyLauda/re206.py` & `pyLauda-1.0.3/pyLauda/re206.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,219 +1,210 @@
-# SPDX-FileCopyrightText: 2021 German Aerospace Center (DLR)
-#
-# SPDX-License-Identifier: MIT
-
 """
 Driver for Thermostate Lauda RE 206
 """
 
+__author__ = "konstantin.niehaus [ at ] dlr .de"
+__copyright__ = "German Aerospace Center 2020"
+__credits__ = ["Konstantin Niehaus", "Daniel Schmeling", "Andreas Westhoff"]
+__license__ = "tba"
+__version__ = "1.0.0"
+__maintainer__ = "Konstantin Niehaus"
+__email__ = "konstantin.niehaus [ at ] dlr .de"
+__status__ = "Production"
+
+
 import serial
 from serial.serialutil import SerialException
 
-
 class RE206(object):
+    """ Control and read thermostat and pump of a RE 206 Lauda device
     """
-    Control and read thermostat and pump of a RE 206 Lauda device
-    """
-
     __MAX_ATTEMPTS = 5
     __OWN_TIMEOUT = 2.0
 
-    def __init__(self, port: str):
-        """
-        Start device
+
+    def __init__(self, port):
+        """ Start device
         :param port: Path to device mounting point i.e. /dev/ttyUSB0
         :type port: str
         """
         # Set up serial communication
         self.device = self.init_RS232_to_serial(port)
         # Wake up device
         self.start()
         # Lock panel
         self.lock_control_panel()
 
-    def init_RS232_to_serial(self, port: str):
-        """
-        Start serial communication
+    def init_RS232_to_serial(self, port):
+        """ Start serial communication
         :param port: Path to device mounting point i.e. /dev/ttyUSB0
         :type port: str
         """
         try:
-            return serial.Serial(
-                port=port, baudrate=19200, rtscts=1, dsrdtr=0, timeout=1
-            )
+            return serial.Serial(port=port,
+                baudrate= 19200,
+                rtscts=1,
+                dsrdtr=0,
+                timeout=1)
         except serial.SerialException:
-            raise SerialException("Lauda RE206: Connection error for port: " + port)
+             raise SerialException('Lauda RE206: Connection error for port: ' + port)
+
 
     def start(self):
-        """
-        Switch on unit from standby
+        """ Switch on unit from standby
         """
         try:
             self.device.open()
-            self.__write("START\r")
-            msg = "[INFO] Start lauda RE20X at port " + str(self.device)
+            self.__write('START\r')
+            msg = '[INFO] Start lauda RE20X at port '+str(self.device)
             return msg
         except:
-            raise SerialException("Lauda RE206: Failed to start.")
+            raise SerialException('Lauda RE206: Failed to start.')
 
     def stop(self):
-        """
-        Switches the unit to stand-by (pump, heating, refrigeration system off)
+        """ Switches the unit to stand-by (pump, heating, refrigeration system off)
         """
         try:
-            self.__write("STOP\r")
-            msg = "[INFO] Stop lauda RE20X at port " + str(self.device)
+            self.__write('STOP\r')
+            msg = '[INFO] Stop lauda RE20X at port '+str(self.device)
             return msg
         except:
-            raise SerialException("Lauda RE206: Failed to stop.")
+            raise SerialException('Lauda RE206: Failed to stop.')
 
-    def set_control_parameters(self, Xp: float, Tn: float):
-        """
-        Set PID parameters Xp and Tn (see. manual p35)
+
+    def set_control_parameters(self, Xp, Tn):
+        """ Set PID parameters Xp and Tn (see. manual p35)
         :param Xp: proportional value
-        :type Xp: float
+	:type Xp: float
         :param Tn: time value
-        :type Tn: float
-        """
+	:type Tn: float
+	"""
         try:
-            self.__write("OUT_PAR_00_{:3.2}".format(Xp))
-            self.__write("OUT_PAR_01_{:3.2}".format(Tn))
-            msg = (
-                "[INFO] Set Xp = " + Xp + " and " + Tn + " at port " + str(self.device)
-            )
+            self.__write('OUT_PAR_00_{:3.2}'.format(Xp))
+            self.__write('OUT_PAR_01_{:3.2}'.format(Tn))
+            msg = '[INFO] Set Xp = '+Xp+' and '+Tn+' at port '+str(self.device)
             return msg
         except:
-            raise SerialException("Lauda RE206: initialization error")
+            raise SerialException('Lauda RE206: initialization error')
+
 
     def lock_control_panel(self):
-        """
-        Lock control panel of lauda
-        """
+        """ Lock control panel of lauda """
 
         try:
-            self.__write("OUT_MODE_00_0\r")
-            msg = "[INFO] lock control panel at port " + str(self.device)
+            self.__write('OUT_MODE_00_0\r')
+            msg = '[INFO] lock control panel at port '+str(self.device)
             return msg
         except:
-            raise SerialException("Lauda RE206: Failed to lock control panel")
+            raise SerialException('Lauda RE206: Failed to lock control panel')
+
 
     @property
     def pump(self):
-        """
-        Read current pump level
-        """
-        self.__write("IN_SP_01\r")
+        """ Read current pump level """
+        self.__write('IN_SP_01\r')
         answ = str(self.device.readline())
         answ = int(answ[3:-8])
         return answ
-
     @pump.setter
     def pump(self, level):
-        """
-        Set pump level
+        """ Set pump level
         :param level: Set level from 1 to 5
         :param type: int or float
         """
-        assert level in range(1, 6)
+        assert level in range(1,6)
         try:
-            self.__write("OUT_SP_01_{:1.0f}\r".format(level))
-            msg = "[INFO] Set pump level " + str(level) + " port " + str(self.device)
+            self.__write('OUT_SP_01_{:1.0f}\r'.format(level))
+            msg = '[INFO] Set pump level '+str(level)+' port '+str(self.device)
             return msg
         except:
-            raise SerialException("Lauda RE206: Error during setting pump level.")
+            raise SerialException('Lauda RE206: Error during setting pump level.')
+
 
     def clear_buffer(self):
-        """
-        Discard all pending readings
-        """
+        """ Discard all pending readings """
         try:
             buf = self.device.readline()
             while buf:
                 buf = self.device.readline()
-            msg = "[INFO] Buffer cleared port " + str(self.device)
+            msg = '[INFO] Buffer cleared port '+str(self.device)
         except:
-            raise SerialException("Lauda RE206: Error during buffer clearing.")
+            raise SerialException('Lauda RE206: Error during buffer clearing.')
 
     def read_buffer(self):
-        """
-        Read all pending readings
-        """
+        """ Read all pending readings """
         msg_list = []
         msg_list.append(self.device.readline())
         while self.device.readline():
             msg_list.append(self.device.readline())
         return msg_list
 
+
     @property
     def temperature(self):
-        """
-        Get current bath temperature
-        """
-        self.__write("IN_PV_00\r")
+        """ Get current bath temperature """
+        self.__write('IN_PV_00\r')
         answ = str(self.device.readline())
         answ = float(answ[3:-5])
         return answ
 
     @temperature.setter
     def temperature(self, temperature):
-        """
-        Register new set temperature
+        """ Register new set temperature
         :param temperature: New temperature in [deg C]
         :type temperature: float
         """
         try:
-            self.__write("OUT_SP_00_{:03.2f}\r".format(temperature))
+            self.__write('OUT_SP_00_{:03.2f}\r'.format(temperature))
             return float(temperature)
 
         except:
-            raise SerialException("Lauda RE206: initialization error")
+            raise SerialException('Lauda RE206: initialization error')
 
     def get_SetTemperature(self):
-        """
-        Get set temperature
-        """
-        self.__write("IN_SP_00\r")
+        """ Get set temperature """
+        self.__write('IN_SP_00\r')
         answ = str(self.device.readline())
         answ = float(answ[3:-5])
         return answ
 
     def checkConnection(self):
-        """
-        Send test request
+        """ Send test request
         :return: Connection state
         :type: boolean
         """
         try:
-            self.__write("IN_PV_00\r")
+            self.__write('IN_PV_00\r')
             self.__readline()
             return True
         except:
             return False
 
     def __write(self, cmd):
         self.clear_buffer()
         self.device.write(str.encode(cmd))
 
     def __readline(self):
         # own timeout
         attempts = 1
-        out = ""
+        out = ''
         while attempts <= self.__MAX_ATTEMPTS:
             # look for waiting bytes
             bytesWaiting = self.device.inWaiting()
             # 0 waiting bytes:
             if bytesWaiting <= 0:
                 # sleep OWN_TIMEOUT seconds
                 time.sleep(self.__OWN_TIMEOUT)
             else:
                 # more than 0 waiting bytes:
                 while bytesWaiting > 0:
                     # append to out until \r is found
                     b = self.device.read(1)
                     out += b
-                    if b == "\r" or b == "\n":
+                    if (b == '\r' or b == '\n'):
                         return out
             # increase attempts after trying to detect waiting bytes
             attempts = attempts + 1
         # MAX_ATTEMPTS reached: raise Exception
-        raise SerialException("Lauda: timed out.")
+        raise SerialException('Lauda: timed out.')
+
+
```

### Comparing `pyLauda-1.0.2/pyLauda/variocool.py` & `pyLauda-1.0.3/pyLauda/variocool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,312 +1,255 @@
-# SPDX-FileCopyrightText: 2022 German Aerospace Center (DLR)
-#
-# SPDX-License-Identifier: MIT
-
+"""
+Driver for Thermostate Lauda RE 206
+"""
 
 import serial
 import time
 import sys
 from serial import SerialException
 import logging
-
+import timeout_decorator
+from timeout_decorator.timeout_decorator import TimeoutError
 
 class Variocool(object):
     """
-    Driver for Thermostate Lauda VC
     Control and read thermostat and pump of a RE 206 Lauda device
     """
-
     __MAX_ATTEMPTS = 5
     __OWN_TIMEOUT = 0.25
     __DEVICE_IDENTIFIER = "VCXXXX"
 
-    def __init__(self, port: str):
-        """
-        Start device
+    def __init__(self, port, loglvl=logging.INFO):
+        """ Start device
         :param port: Path to device mounting point i.e. /dev/ttyUSB0
         :type port: str
         """
         stream_handler = logging.StreamHandler(sys.stdout)
 
         # Initialize logging instance
         self._log = logging.getLogger("Lauda@" + port)
         self._log.addHandler(stream_handler)
-        self._log.level = logging.DEBUG
+        self._log.level = loglvl
 
         # Set up serial communication
         self.device = self.init_RS232_to_serial(port)
         if self.device.isOpen():
             self.device.close()
         self.device.open()
 
-        # Lock panel
-        self.lock_control_panel()
-
-    def init_RS232_to_serial(self, port: str):
-        """
-        Start serial communication
+    def init_RS232_to_serial(self, port):
+        """ Start serial communication
         :param port: Path to device mounting point i.e. /dev/ttyUSB0
         :type port: serial.Serial
         """
         try:
-            return serial.Serial(
-                port=port,
-                baudrate=9600,
-                parity=serial.PARITY_NONE,
-                stopbits=serial.STOPBITS_ONE,
-                bytesize=serial.EIGHTBITS,
-                timeout=1,
-            )
+            return serial.Serial(port=port,
+               baudrate=9600,
+               parity=serial.PARITY_NONE,
+               stopbits=serial.STOPBITS_ONE,
+               bytesize=serial.EIGHTBITS,
+               timeout=1)
         except SerialException:
-            self._log.error("Error while opening communication.")
-            raise SerialException(
-                "Lauda "
-                + self.__DEVICE_IDENTIFIER
-                + ": Connection error for port: "
-                + port
-            )
+             self._log.error("Error while opening communication.")
+             raise SerialException('Lauda ' + self.__DEVICE_IDENTIFIER + ': Connection error for port: ' + port)
 
     def start(self):
-        """
-        Switch on unit from standby
+        """ Switch on unit from standby
         """
         try:
             try:
                 self.device.open()
             except serial.SerialException:
                 self.device.close()
                 self.device.open()
             if self.temperature is None:
                 self._log.error("Temperature not set. -> Start aborted")
-                raise ValueError(
-                    "Lauda "
-                    + self.__DEVICE_IDENTIFIER
-                    + ": Failed to start due to missing temperature."
-                )
+                raise ValueError('Lauda ' + self.__DEVICE_IDENTIFIER + ': Failed to start due to missing temperature.')
 
-            self.__write("START")
+            self.__write('START')
             self._log.info("Device started")
         except SerialException:
             self._log.error("Communication error while start request")
-            raise SerialException(
-                "Lauda " + self.__DEVICE_IDENTIFIER + ": Failed to start."
-            )
+            raise SerialException('Lauda ' + self.__DEVICE_IDENTIFIER + ': Failed to start.')
 
     def stop(self):
-        """
-        Switches the unit to stand-by (pump, heating, refrigeration system off)
+        """ Switches the unit to stand-by (pump, heating, refrigeration system off)
         """
         try:
-            self.__write("STOP")
+            self.__write('STOP')
             self._log.info("Device stopped")
         except SerialException:
             self._log.error("Communication error while sending stop request")
-            raise SerialException(
-                "Lauda " + self.__DEVICE_IDENTIFIER + ": Failed to stop."
-            )
+            raise SerialException('Lauda ' + self.__DEVICE_IDENTIFIER + ': Failed to stop.')
 
-    def set_control_parameters(self, Xp: float, Tn: float):
-        """
-        Set PID parameters Xp and Tn (see. manual p35)
+
+    def set_control_parameters(self, Xp, Tn):
+        """ Set PID parameters Xp and Tn (see. manual p35)
         :param Xp: proportional value
-        :type Xp: float
+	:type Xp: float
         :param Tn: time value
-        :type Tn: float
-        """
+	:type Tn: float
+	"""
         try:
-            self.__write("OUT_PAR_00_{:3.2}".format(Xp))
-            self.__write("OUT_PAR_01_{:3.2}".format(Tn))
+            self.__write('OUT_PAR_00_{:3.2}'.format(Xp))
+            self.__write('OUT_PAR_01_{:3.2}'.format(Tn))
             self._log.info(f"Set Xp = {Xp} and {Tn}")
         except SerialException:
-            raise SerialException(
-                "Lauda " + self.__DEVICE_IDENTIFIER + ": initialization error"
-            )
+            raise SerialException('Lauda ' + self.__DEVICE_IDENTIFIER + ': initialization error')
+
 
     def lock_control_panel(self):
-        """
-        Lock control panel of lauda
-        """
+        """ Lock control panel of lauda """
         try:
-            self.__write("OUT_MODE_00_0")
+            self.__write('OUT_MODE_00_0')
             self._log.info(f"Locked control panel.")
         except SerialException:
-            raise SerialException("Lauda RE206: Failed to lock control panel")
+            raise SerialException('Lauda RE206: Failed to lock control panel')
+
 
     def clear_buffer(self):
-        """
-        Discard all pending readings
-        """
+        """ Discard all pending readings """
         try:
             buf = self.device.readline()
             while buf:
                 buf = self.device.readline()
             self._log.info(f"Buffer cleared port")
         except SerialException:
-            raise SerialException("Lauda RE206: Error during buffer clearing.")
+            raise SerialException('Lauda RE206: Error during buffer clearing.')
 
     def read_buffer(self):
-        """
-        Read all pending readings
-        """
+        """ Read all pending readings """
         msg_list = []
         msg_list.append(self.device.readline())
         while self.device.readline():
             msg_list.append(self.device.readline())
         return msg_list
 
+
     @property
     def temperature(self):
-        """
-        Get set temperature
-        """
-        answ = self.__txrx("IN_SP_00")
+        """ Get set temperature """
+        answ = self.__txrx('IN_SP_00')
         if len(answ) > 5:
             self._log.debug(f"Current set temperature {answ}.")
-            answ = answ.replace(b"\r", b"").replace(b" ", b"")
+            answ = answ.replace(b'\r',b'').replace(b' ', b'')
             return float(answ)
         else:
             self._log.error(f"Failed to read temperature.")
             return None
 
     @temperature.setter
     def temperature(self, temperature):
-        """
-        Register new set temperature
+        """ Register new set temperature
         :param temperature: New temperature in [deg C]
         :type temperature: float
         :returns: Temperature
         :rtype: float
         """
         self._log.debug(f"New set temperature {temperature}.")
-        self.__write("OUT_SP_00_{:03.2f}".format(temperature))
+        self.__write('OUT_SP_00_{:03.2f}'.format(temperature))
         return float(temperature)
 
     @property
     def t_ext(self):
-        """
-        Get external temperature
-        """
-        answ = self.__txrx("IN_PV_01")
+        """ Get external temperature """
+        answ = self.__txrx('IN_PV_01')
         temperature = None
         try:
-            answ = answ.replace(b"\r", b"").replace(b" ", b"")
+            answ = answ.replace(b'\r',b'').replace(b' ', b'')
             temperature = float(answ)
         except ValueError:
             state = self.get_device_state()
             self._log.debug(f"Lauda Error {answ}, state: {state}")
         self._log.debug(f"New ext. temperature {temperature}.")
         return answ
 
     @t_ext.setter
     def t_ext(self, temperature):
-        """
-        Register new external temperature
+        """ Register new external temperature
         :param temperature: New external temperature in [deg C]
         :type temperature: float
         :returns: Temperature
         :rtype: float
         """
-        answ = self.__txrx("OUT_PV_05_{:03.2f}".format(temperature))
+        answ = self.__txrx('OUT_PV_05_{:03.2f}'.format(temperature))
         self._log.debug(f"New ext. temperature {temperature}.")
         return float(temperature)
 
     def checkConnection(self):
-        """
-        Send test request
+        """ Send test request
         :return: Connection state
         :type: boolean
         """
         try:
-            self.__write("IN_PV_00")
+            self.__write('IN_PV_00')
             self.__readline()
             return True
         except:
             return False
 
     def get_device_state(self):
-        """
-        Request current device status
+        """ Request current device status
         :return: 0 if no error occured otherwise see manuel p. 35
         :type: int
         """
-        return self.__txrx("STAT")
-
-    def test(self):
-        """
-        Check if device is reponsive
-        :return: device availability
-        :type: boolean
-        """
-        version_ctrl = self.__txrx("VERSION_R")
-        self._log.info(f"Serial version: {version_ctrl}")
-
-        typ = self.__txrx("TYPE").decode("utf-8").strip("\r\n")
-        self._log.info(f"Device type: {typ}")
-
-        state = self.__txrx("STAT").decode("utf-8").strip("\r\n")
-        self._log.info(f"Device state: {state}")
-
-        if typ == "VC" and int(state) == 0:
-            return True
+        return self.__txrx('STAT')
 
     def RS232moduleSN(self):
-        return self.__txrx("VERSION_V").decode("utf-8").strip("\r\n").replace(" ", "")
+        return self.__txrx('VERSION_V').decode('utf-8').strip('\r\n').replace(" ", "")
 
     def checkConnection(self):
-        """
-        Send test request
+        """ Send test request
         :return: Connection state
         :type: boolean
         """
         try:
-            self.__write("IN_PV_00")
+            self.__write('IN_PV_00')
             self.__readline()
             return True
         except:
             return False
 
     def get_device_state(self):
-        """
-        Request current device status
+        """ Request current device status
         :return: 0 if no error occured otherwise see manuel p. 35
         :type: int
         """
-        return self.__txrx("STAT")
+        return self.__txrx('STAT')
 
+    @timeout_decorator.timeout(1, timeout_exception=TimeoutError)
     def test(self):
         """
         Check if device is reponsive
         :return: device availability
         :type: boolean
         """
-        version_ctrl = self.__txrx("VERSION_R")
+        version_ctrl = self.__txrx('VERSION_R')
         self._log.info(f"Serial version: {version_ctrl}")
-        typ = self.__txrx("TYPE").decode("utf-8").strip("\r\n")
+
+        typ = self.__txrx('TYPE').decode('utf-8').strip('\r\n')
         self._log.info(f"Device type: {typ}")
 
-        state = self.__txrx("STAT").decode("utf-8").strip("\r\n")
+        state = self.__txrx('STAT').decode('utf-8').strip('\r\n')
         self._log.info(f"Device state: {state}")
 
         if typ == "VC" and int(state) == 0:
             return True
 
         return False
 
     def __write(self, cmd):
         try:
             self.device.write(str.encode(cmd + "\r"))
         except SerialException:
-            raise SerialException(
-                "Lauda " + self.__DEVICE_IDENTIFIER + ": Error while writing."
-            )
+            raise SerialException('Lauda ' +  self.__DEVICE_IDENTIFIER + ': Error while writing.')
 
     def __readline(self, n=0):
         out = bytearray()
-        eol = b"\r"
+        eol = b'\r'
         leneol = len(eol)
         c = None
         if self.device is None:
             self._log.error(f"Device not defined.")
             return out
 
         if not self.device.isOpen():
@@ -317,33 +260,33 @@
             c = self.device.read(1)
             if c:
                 out += c
                 if out[-leneol:] == eol:
                     break
             else:
                 break
-        if not out and n < 30:
-            self._log.warning(f"Retry reading once.")
+        if not out and n<30:
+            self._log.warning(f"Retry reading.")
             time.sleep(0.5)
             if self.device.isOpen():
                 self.device.close()
             self.device.open()
             self.read_buffer()
-            self.__readline(n=n + 1)
+            self.__readline(n=n+1)
 
         return out
 
     def __txrx(self, cmd):
-        """
-        Write command and consequently perform a read operation.
+        """ Write command and consequently perform a read operation.
         """
         answ = None
         for i in range(3):
             self.read_buffer()
             self.__write(cmd)
             time.sleep(0.1)
             answ = self.__readline()
             if answ is not None:
                 break
         self._log.debug(f"CMD: {cmd}\t Return: {answ}")
 
         return answ
+
```

### Comparing `pyLauda-1.0.2/test/test_re206.py` & `pyLauda-1.0.3/test/test_re206.py`

 * *Files identical despite different names*

### Comparing `pyLauda-1.0.2/test/test_vc.py` & `pyLauda-1.0.3/test/test_vc.py`

 * *Files identical despite different names*

