# Comparing `tmp/labelprinterkit-0.3.0.tar.gz` & `tmp/labelprinterkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/labelprinterkit-0.3.0.tar", last modified: Fri Aug 17 13:41:48 2018, max compression
+gzip compressed data, was "labelprinterkit-0.4.0.tar", max compression
```

## Comparing `labelprinterkit-0.3.0.tar` & `labelprinterkit-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,14 @@
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/
--rw-r--r--   0 nota      (1000) nota      (1000)       50 2018-05-23 12:24:23.000000 labelprinterkit-0.3.0/pyproject.toml
--rw-r--r--   0 nota      (1000) nota      (1000)       38 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/setup.cfg
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/labelprinterkit/
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/labelprinterkit/backends/
--rw-r--r--   0 nota      (1000) nota      (1000)      696 2018-05-23 17:41:09.000000 labelprinterkit-0.3.0/labelprinterkit/backends/__init__.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/labelprinterkit/printers/
--rw-r--r--   0 nota      (1000) nota      (1000)     7101 2018-06-05 17:40:03.000000 labelprinterkit-0.3.0/labelprinterkit/printers/brother_pt700.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1656 2018-06-05 17:38:15.000000 labelprinterkit-0.3.0/labelprinterkit/printers/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)      966 2018-06-05 18:10:00.000000 labelprinterkit-0.3.0/labelprinterkit/items.py
--rw-r--r--   0 nota      (1000) nota      (1000)      146 2018-05-23 13:06:27.000000 labelprinterkit-0.3.0/labelprinterkit/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2339 2018-06-29 21:44:03.000000 labelprinterkit-0.3.0/labelprinterkit/label.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1459 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/PKG-INFO
--rw-r--r--   0 nota      (1000) nota      (1000)      883 2018-08-17 13:38:04.000000 labelprinterkit-0.3.0/setup.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11337 2018-05-22 20:05:04.000000 labelprinterkit-0.3.0/LICENSE
--rw-r--r--   0 nota      (1000) nota      (1000)      718 2018-05-28 19:05:39.000000 labelprinterkit-0.3.0/README.md
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/labelprinterkit.egg-info/
--rw-r--r--   0 nota      (1000) nota      (1000)     1459 2018-08-17 13:41:47.000000 labelprinterkit-0.3.0/labelprinterkit.egg-info/PKG-INFO
--rw-r--r--   0 nota      (1000) nota      (1000)       22 2018-08-17 13:41:47.000000 labelprinterkit-0.3.0/labelprinterkit.egg-info/requires.txt
--rw-r--r--   0 nota      (1000) nota      (1000)       16 2018-08-17 13:41:47.000000 labelprinterkit-0.3.0/labelprinterkit.egg-info/top_level.txt
--rw-r--r--   0 nota      (1000) nota      (1000)        1 2018-08-17 13:41:47.000000 labelprinterkit-0.3.0/labelprinterkit.egg-info/dependency_links.txt
--rw-r--r--   0 nota      (1000) nota      (1000)      440 2018-08-17 13:41:48.000000 labelprinterkit-0.3.0/labelprinterkit.egg-info/SOURCES.txt
--rw-r--r--   0 nota      (1000) nota      (1000)     1203 2018-05-23 10:49:26.000000 labelprinterkit-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11337 2018-12-03 22:08:27.602616 labelprinterkit-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2235 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/README.md
+-rw-r--r--   0        0        0      146 2023-06-18 22:18:49.912639 labelprinterkit-0.4.0/labelprinterkit/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/labelprinterkit/backends/__init__.py
+-rw-r--r--   0        0        0      635 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/labelprinterkit/backends/bluetooth.py
+-rw-r--r--   0        0        0      793 2023-06-23 21:07:41.479689 labelprinterkit-0.4.0/labelprinterkit/backends/network.py
+-rw-r--r--   0        0        0      802 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/backends/usb.py
+-rw-r--r--   0        0        0     2452 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/constants.py
+-rw-r--r--   0        0        0     1864 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/job.py
+-rw-r--r--   0        0        0     5075 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/label.py
+-rw-r--r--   0        0        0     2176 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/page.py
+-rw-r--r--   0        0        0     8654 2023-06-23 21:07:41.480689 labelprinterkit-0.4.0/labelprinterkit/printers.py
+-rw-r--r--   0        0        0      507 2023-06-23 21:07:41.481689 labelprinterkit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 labelprinterkit-0.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `labelprinterkit-0.3.0/labelprinterkit/backends/__init__.py` & `labelprinterkit-0.4.0/labelprinterkit/backends/usb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
+from time import sleep
+
 import usb.core
 import usb.util
-import threading
 
-def is_usb_printer(dev):
-    if dev.bDeviceClass == 7:
-        return True
-    for cfg in dev:
-        if usb.util.find_descriptor(cfg, bInterfaceClass=7) is not None:
-            return True
+from . import BaseBackend
 
 
-class PyUSBBackend():
-    def __init__(self, dev):
-        self.dev = dev
-        self.lock = threading.Lock()
-
-    @classmethod
-    def auto(cls):
-        dev = usb.core.find(custom_match=is_usb_printer)
+class PyUSBBackend(BaseBackend):
+    def __init__(self):
+        dev = usb.core.find(custom_match=self.is_usb_printer)
         if dev is None:
             raise OSError('Device not found')
-        return cls(dev)
+        self._dev = dev
+
+    @staticmethod
+    def is_usb_printer(dev) -> bool:
+        if dev.bDeviceClass == 7:
+            return True
+        for cfg in dev:
+            if usb.util.find_descriptor(cfg, bInterfaceClass=7) is not None:
+                return True
 
     def write(self, data: bytes):
-        self.dev.write(0x2, data)
+        self._dev.write(0x2, data)
 
     def read(self, count: int) -> bytes:
-        return self.dev.read(0x81, count)
+        for i in range(0, 3):
+            data = self._dev.read(0x81, count)
+            if data:
+                return data
+            sleep(0.1)
```

### Comparing `labelprinterkit-0.3.0/LICENSE` & `labelprinterkit-0.4.0/LICENSE`

 * *Files identical despite different names*

