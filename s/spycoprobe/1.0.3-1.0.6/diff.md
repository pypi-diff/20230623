# Comparing `tmp/spycoprobe-1.0.3.tar.gz` & `tmp/spycoprobe-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spycoprobe-1.0.3.tar", last modified: Tue May  2 13:31:31 2023, max compression
+gzip compressed data, was "spycoprobe-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spycoprobe-1.0.3.tar` & `spycoprobe-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.639806 spycoprobe-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 13:31:31.639806 spycoprobe-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:31:31.639806 spycoprobe-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.639806 spycoprobe-1.0.3/spycoprobe/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/spycoprobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/spycoprobe/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/spycoprobe/intelhex.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/spycoprobe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-02 13:31:22.000000 spycoprobe-1.0.3/spycoprobe/spycoprobe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:31:31.639806 spycoprobe-1.0.3/spycoprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 13:31:31.000000 spycoprobe-1.0.3/spycoprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-02 13:31:31.000000 spycoprobe-1.0.3/spycoprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:31:31.000000 spycoprobe-1.0.3/spycoprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 13:31:31.000000 spycoprobe-1.0.3/spycoprobe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 13:31:31.000000 spycoprobe-1.0.3/spycoprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 13:31:31.000000 spycoprobe-1.0.3/spycoprobe.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1073 2023-06-23 14:22:45.136625 spycoprobe-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      480 2023-06-23 14:22:45.136625 spycoprobe-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-23 14:22:45.136625 spycoprobe-1.0.6/spycoprobe/__init__.py
+-rw-r--r--   0        0        0     2648 2023-06-23 14:22:45.136625 spycoprobe-1.0.6/spycoprobe/cli.py
+-rw-r--r--   0        0        0     1668 2023-06-23 14:22:45.136625 spycoprobe-1.0.6/spycoprobe/intelhex.py
+-rw-r--r--   0        0        0      761 2023-06-23 14:22:45.136625 spycoprobe-1.0.6/spycoprobe/protocol.py
+-rw-r--r--   0        0        0     5286 2023-06-23 14:22:45.136625 spycoprobe-1.0.6/spycoprobe/spycoprobe.py
+-rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 spycoprobe-1.0.6/PKG-INFO
```

### Comparing `spycoprobe-1.0.3/LICENSE.txt` & `spycoprobe-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spycoprobe-1.0.3/spycoprobe/cli.py` & `spycoprobe-1.0.6/spycoprobe/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,21 @@
 @cli.command(short_help="Control target power supply")
 @click.option("--on/--off", required=True)
 @click.pass_context
 def target_power(ctx, on):
     ctx.obj["probe"].target_power(on)
 
 
+@cli.command(short_help="Control power supply bypass")
+@click.option("--on/--off", required=True)
+@click.pass_context
+def bypass(ctx, on):
+    ctx.obj["probe"].bypass(on)
+
+
 @cli.command(short_help="Control GPIO pin")
 @click.option("--pin-no", "-p", type=int, required=True, help="Pin number")
 @click.option(
     "--state",
     "-s",
     type=click.Choice(["high", "1", "low", "0", "input"], case_sensitive=False),
     required=True,
```

### Comparing `spycoprobe-1.0.3/spycoprobe/intelhex.py` & `spycoprobe-1.0.6/spycoprobe/intelhex.py`

 * *Files identical despite different names*

### Comparing `spycoprobe-1.0.3/spycoprobe/protocol.py` & `spycoprobe-1.0.6/spycoprobe/protocol.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,29 @@
     SBW_REQ_HALT = 2
     SBW_REQ_RELEASE = 3
     SBW_REQ_WRITE = 4
     SBW_REQ_READ = 5
     SBW_REQ_POWER = 6
     SBW_REQ_IOSET = 7
     SBW_REQ_IOGET = 8
+    SBW_REQ_BYPASS = 9
 
 
 class ReturnCode(IntEnum):
     SBW_RC_OK = 0
     SBW_RC_ERR_GENERIC = 1
     SBW_RC_ERR_UNKNOWN_REQ = 2
     SBW_RC_ERR_UNSUPPORTED = 3
 
 
+class BypassState(IntEnum):
+    BYPASS_OFF = 0
+    BYPASS_ON = 1
+
+
 class TargetPowerState(IntEnum):
     TARGET_POWER_OFF = 0
     TARGET_POWER_ON = 1
 
 
 class IOSetState(IntEnum):
     IOSET_OUT_LOW = 0
```

### Comparing `spycoprobe-1.0.3/spycoprobe/spycoprobe.py` & `spycoprobe-1.0.6/spycoprobe/spycoprobe.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,37 @@
 from typing import Union
 from serial.tools import list_ports
 
 from spycoprobe.intelhex import IntelHex16bitReader
 from spycoprobe.protocol import ReqType
 from spycoprobe.protocol import ReturnCode
 from spycoprobe.protocol import TargetPowerState
+from spycoprobe.protocol import BypassState
 from spycoprobe.protocol import IOSetState
 
 from spycoprobe.protocol import REQUEST_MAX_DATA
 from spycoprobe.protocol import RESPONSE_MAX_DATA
 
 
 class DeviceNotFoundError(Exception):
     pass
 
 
 INTERFACE_NAMES = ["Spycoprobe SBW", "Rioteeprobe SBW"]
+USB_VID = 0x1209
+USB_PIDS = [0xC8A0, 0xC8A1]
 
 
 def find_device():
     hits = list()
     for port in list_ports.comports():
-        if port.interface in INTERFACE_NAMES:
+        if (port.vid == USB_VID) and (port.pid in USB_PIDS) and (port.location.endswith("3")):
             hits.append(port.device)
+        else:
+            logging.debug(f"{port.vid:04X}, {port.pid:04X}")
 
     if not hits:
         raise DeviceNotFoundError("Couldn't find a Spycoprobe USB device.")
     elif len(hits) == 1:
         logging.info(f"Found spycoprobe at {hits[0]}")
         return hits[0]
     else:
@@ -98,14 +103,22 @@
         if state:
             pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_POWER, 1, 0x0, TargetPowerState.TARGET_POWER_ON)
         else:
             pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_POWER, 1, 0x0, TargetPowerState.TARGET_POWER_OFF)
         self._ser.write(pkt)
         self._recv_rsp()
 
+    def bypass(self, state: bool):
+        if state:
+            pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_BYPASS, 1, 0x0, BypassState.BYPASS_ON)
+        else:
+            pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_BYPASS, 1, 0x0, BypassState.BYPASS_OFF)
+        self._ser.write(pkt)
+        self._recv_rsp()
+
     def gpio_set(self, pin_no, state: IOSetState):
         pkt = struct.pack(f"=BBI2H", ReqType.SBW_REQ_IOSET, 2, 0x0, pin_no, state)
         self._ser.write(pkt)
         self._recv_rsp()
 
     def gpio_get(self, pin_no) -> bool:
         pkt = struct.pack(f"=BBIH", ReqType.SBW_REQ_IOGET, 2, 0x0, pin_no)
```

