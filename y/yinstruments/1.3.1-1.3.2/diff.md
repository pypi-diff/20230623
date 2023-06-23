# Comparing `tmp/yinstruments-1.3.1.tar.gz` & `tmp/yinstruments-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yinstruments-1.3.1.tar", last modified: Mon Jun 12 19:01:14 2023, max compression
+gzip compressed data, was "yinstruments-1.3.2.tar", last modified: Fri Jun 23 14:49:37 2023, max compression
```

## Comparing `yinstruments-1.3.1.tar` & `yinstruments-1.3.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-12 19:01:14.706849 yinstruments-1.3.1/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-06-12 19:01:14.706849 yinstruments-1.3.1/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      446 2023-06-12 19:00:57.000000 yinstruments-1.3.1/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/test/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      268 2023-06-12 18:57:50.000000 yinstruments-1.3.1/test/test_packaging.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/yinstruments/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 18:59:11.000000 yinstruments-1.3.1/yinstruments/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3633 2023-06-06 14:51:33.000000 yinstruments-1.3.1/yinstruments/async_reader.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/yinstruments/pdu/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 18:59:19.000000 yinstruments-1.3.1/yinstruments/pdu/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1780 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/pdu/cli.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2880 2023-06-12 18:57:50.000000 yinstruments-1.3.1/yinstruments/pdu/lindy.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1982 2023-06-12 18:57:50.000000 yinstruments-1.3.1/yinstruments/pdu/netbooter.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      650 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/pdu/pdu.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     5828 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/powersupply.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4131 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/usb_finder.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3564 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/usb_power.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/yinstruments.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      478 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       13 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-23 14:49:37.264465 yinstruments-1.3.2/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-23 14:49:37.264465 yinstruments-1.3.2/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-06-23 14:49:37.264465 yinstruments-1.3.2/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      521 2023-06-23 14:49:29.000000 yinstruments-1.3.2/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-23 14:49:37.264465 yinstruments-1.3.2/test/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      268 2023-06-22 15:14:42.000000 yinstruments-1.3.2/test/test_packaging.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-23 14:49:37.264465 yinstruments-1.3.2/yinstruments/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-22 15:14:42.000000 yinstruments-1.3.2/yinstruments/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3633 2023-06-22 15:14:42.000000 yinstruments-1.3.2/yinstruments/async_reader.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-23 14:49:37.264465 yinstruments-1.3.2/yinstruments/pdu/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-22 15:14:42.000000 yinstruments-1.3.2/yinstruments/pdu/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1662 2023-06-23 14:42:51.000000 yinstruments-1.3.2/yinstruments/pdu/cli.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3339 2023-06-23 14:39:10.000000 yinstruments-1.3.2/yinstruments/pdu/lindy.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2350 2023-06-23 14:39:10.000000 yinstruments-1.3.2/yinstruments/pdu/netbooter.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1152 2023-06-23 14:48:41.000000 yinstruments-1.3.2/yinstruments/pdu/pdu.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     5828 2023-06-22 15:14:42.000000 yinstruments-1.3.2/yinstruments/powersupply.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4131 2023-06-22 15:14:42.000000 yinstruments-1.3.2/yinstruments/usb_finder.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3564 2023-06-22 15:14:42.000000 yinstruments-1.3.2/yinstruments/usb_power.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-23 14:49:37.264465 yinstruments-1.3.2/yinstruments.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-23 14:49:37.000000 yinstruments-1.3.2/yinstruments.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      517 2023-06-23 14:49:37.000000 yinstruments-1.3.2/yinstruments.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-06-23 14:49:37.000000 yinstruments-1.3.2/yinstruments.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       51 2023-06-23 14:49:37.000000 yinstruments-1.3.2/yinstruments.egg-info/entry_points.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-06-23 14:49:37.000000 yinstruments-1.3.2/yinstruments.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       13 2023-06-23 14:49:37.000000 yinstruments-1.3.2/yinstruments.egg-info/top_level.txt
```

### Comparing `yinstruments-1.3.1/yinstruments/async_reader.py` & `yinstruments-1.3.2/yinstruments/async_reader.py`

 * *Files identical despite different names*

### Comparing `yinstruments-1.3.1/yinstruments/pdu/lindy.py` & `yinstruments-1.3.2/yinstruments/pdu/lindy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+"""This file contains the Lindy class which inherits from the 
+PDU class"""
+
 import subprocess
 from .pdu import PDU
 
-OID = "iso.3.6.1.4.1.17420.1.2.9.1.13.0"  # standard OID for the functions we will be doing
+# standard OID for the functions we will be doing
+OID = "iso.3.6.1.4.1.17420.1.2.9.1.13.0"
 
 
 class Lindy(PDU):
+    """This is the Lindy class"""
+
+    def __init__(self, ip_address, port, timeout=3.0):
+        super().__init__(ip_address, port)
+
+    def __str__(self):
+        return f"{self.ip_address}:{self.port}"
+
     def on(self, port_num):
-        if (
-            int(port_num) > 8
-        ):  # Since we are working with the LindyIPowerClassic8, we don't want to accept a larger integer than 8
+        if int(port_num) > 8:  # Since we are working with the LindyIPowerClassic8,
+            # we don't want to accept a larger integer than 8
             raise Exception("ERROR: port_num given out of range")
 
-        status_list = self.get_status(OID).split(",")
+        status_list = self.get_status().split(",")
 
         for i in range(
             1, len(status_list) + 1
         ):  # search the newly formed list for the index of the port num
             if i == int(port_num):
                 status_list[i - 1] = "1"
 
@@ -36,20 +47,19 @@
         # execute the command
         subprocess.check_output(command)
 
         # print that the port_num is now on
         # print("On:", port_num)
 
     def off(self, port_num):
-        if (
-            int(port_num) > 8
-        ):  # Since we are working with the LindyIPowerClassic8, we don't want to accept a larger integer than 8
+        if int(port_num) > 8:  # Since we are working with the LindyIPowerClassic8,
+            # we don't want to accept a larger integer than 8
             raise Exception("ERROR: port_num given out of range")
-        OID = "iso.3.6.1.4.1.17420.1.2.9.1.13.0"  # standard OID for the functions we will be doing
-        status_list = self.get_status(OID).split(",")
+
+        status_list = self.get_status().split(",")
 
         for i in range(
             1, len(status_list) + 1
         ):  # search the newly formed list for the index of the port num
             if i == int(port_num):
                 status_list[i - 1] = "0"
 
@@ -70,23 +80,33 @@
         # execute the command
         subprocess.check_output(command)
 
     def reboot(self, port_num):
         self.off(port_num)
         self.on(port_num)
 
-    def get_status(self, OID="iso.3.6.1.4.1.17420.1.2.9.1.13.0"):
+    def get_status(self):
         # command that is going to be executed
         command = [
             "snmpwalk",
             "-v1",
             "-c",
             "public",
             f"{self.ip_address}",
             f"{OID}",
         ]
         # Run the command and capture the output
         output = subprocess.check_output(command)
         # return output
         string = output.decode()[43:60]
-        # return string is a string of comma separated 1's and 0's. 1 means the port is on, 0 means the port is off.
+        # return string is a string of comma separated 1's and 0's.
         return string[1:16]
+
+    def is_on(self, port_num):
+        if int(port_num) > 8:  # Since we are working with the LindyIPowerClassic8,
+            # we don't want to accept a larger integer than 8
+            raise Exception("ERROR: port_num given out of range")
+
+        status_list = self.get_status().split(",")
+        if status_list[int(port_num) - 1] == "1":
+            return "ON"
+        return "OFF"
```

### Comparing `yinstruments-1.3.1/yinstruments/pdu/netbooter.py` & `yinstruments-1.3.2/yinstruments/pdu/netbooter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-from .pdu import PDU
+"""This file contians the Netbooter class which inherits
+from the PDU class"""
+
 import telnetlib
-import re
 import time
+import re
+from .pdu import PDU
 
 
 class Netbooter(PDU):
-    # reboots port on netbooter
+    """This is the Netbooter class"""
+
+    def __init__(self, ip_address, port, timeout=3.0):
+        super().__init__(ip_address, port)
+
+    def __str__(self):
+        return f"{self.ip_address}:{self.port}"
+
     def reboot(self, port_num):
-        tn = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
+        telnet = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
 
-        s = tn.read_some()
-        time.sleep(self._SLEEP_TIME)
+        string = telnet.read_some()
+        time.sleep(self.sleep_time)
 
-        s = ("rb " + str(port_num)).encode("ascii") + b"\r\n\r\n"
-        tn.write(s)
-        time.sleep(self._SLEEP_TIME)
-        tn.close()
+        string = ("rb " + str(port_num)).encode("ascii") + b"\r\n\r\n"
+        telnet.write(string)
+        time.sleep(self.sleep_time)
+        telnet.close()
 
-    # turns port_num on
     def on(self, port_num):
-        tn = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
+        telnet = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
 
-        s = tn.read_some()
-        time.sleep(self._SLEEP_TIME)
+        string = telnet.read_some()
+        time.sleep(self.sleep_time)
 
-        s = ("pset " + str(port_num) + " 1").encode("ascii") + b"\r\n\r\n"
-        tn.write(s)
-        time.sleep(self._SLEEP_TIME)
-        tn.close()
+        string = ("pset " + str(port_num) + " 1").encode("ascii") + b"\r\n\r\n"
+        telnet.write(string)
+        time.sleep(self.sleep_time)
+        telnet.close()
 
-    # turns port_num off
     def off(self, port_num):
-        tn = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
+        telnet = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
 
-        s = tn.read_some()
+        string = telnet.read_some()
 
-        time.sleep(self._SLEEP_TIME)
+        time.sleep(self.sleep_time)
 
-        s = ("pset " + str(port_num) + " 0").encode("ascii") + b"\r\n\r\n"
-        tn.write(s)
-        time.sleep(self._SLEEP_TIME)
-        tn.close()
+        string = ("pset " + str(port_num) + " 0").encode("ascii") + b"\r\n\r\n"
+        telnet.write(string)
+        time.sleep(self.sleep_time)
+        telnet.close()
 
     def get_status(self):
-        tn = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
-
-        s = tn.read_some()
-        time.sleep(self._SLEEP_TIME)
+        telnet = telnetlib.Telnet(self.ip_address, self.port, timeout=self.timeout)
 
-        s = "pshow".encode("ascii") + b"\r\n"
-        tn.write(s)
-        time.sleep(self._SLEEP_TIME)
+        string = telnet.read_some()
+        time.sleep(self.sleep_time)
 
-        s = ""
+        string = "pshow".encode("ascii") + b"\r\n"
+        telnet.write(string)
+        time.sleep(self.sleep_time)
+        string = ""
         while True:
-            text = tn.read_eager()
-            s += text.decode()
+            text = telnet.read_eager()
+            string += text.decode()
             if len(text) == 0:
                 break
 
-        tn.close()
+        telnet.close()
         # returns a organized graphic of the ports and the status of the ports
-        return s
+        return string
 
     def is_on(self, port_num):
         text = self.get_status()
         lines = text.splitlines()
 
-        for l in lines:
-            m = re.match(r"\d+\|\s+Outlet" + str(port_num) + r"\|\s+(\w+)\s*\|", l.strip())
-            if m:
-                return m.group(1) == "ON"
-        return None
+        for line in lines:
+            message = re.match(r"\d+\|\s+Outlet" + str(port_num) + r"\|\s+(\w+)\s*\|", line.strip())
+            if message:
+                return message.group(1) == "ON"
+        return "OFF"
```

### Comparing `yinstruments-1.3.1/yinstruments/powersupply.py` & `yinstruments-1.3.2/yinstruments/powersupply.py`

 * *Files identical despite different names*

### Comparing `yinstruments-1.3.1/yinstruments/usb_finder.py` & `yinstruments-1.3.2/yinstruments/usb_finder.py`

 * *Files identical despite different names*

### Comparing `yinstruments-1.3.1/yinstruments/usb_power.py` & `yinstruments-1.3.2/yinstruments/usb_power.py`

 * *Files identical despite different names*

