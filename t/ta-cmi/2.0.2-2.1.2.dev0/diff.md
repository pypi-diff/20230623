# Comparing `tmp/ta-cmi-2.0.2.tar.gz` & `tmp/ta-cmi-2.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ta-cmi-2.0.2.tar", last modified: Fri Apr 21 23:44:29 2023, max compression
+gzip compressed data, was "ta-cmi-2.1.2.dev0.tar", last modified: Fri Jun 23 15:24:13 2023, max compression
```

## Comparing `ta-cmi-2.0.2.tar` & `ta-cmi-2.1.2.dev0.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:44:29.982145 ta-cmi-2.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8082 2023-04-21 23:44:29.982145 ta-cmi-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6511 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 23:44:29.982145 ta-cmi-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:44:29.980145 ta-cmi-2.0.2/ta_cmi/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/api.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/channel.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/cmi.py
--rw-rw-rw-   0 root         (0) root         (0)     2614 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/cmi_api.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/cmi_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/coe.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/coe_api.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/coe_channel.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/const.py
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-04-21 23:44:13.000000 ta-cmi-2.0.2/ta_cmi/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:44:29.982145 ta-cmi-2.0.2/ta_cmi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8082 2023-04-21 23:44:29.000000 ta-cmi-2.0.2/ta_cmi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-21 23:44:29.000000 ta-cmi-2.0.2/ta_cmi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 23:44:29.000000 ta-cmi-2.0.2/ta_cmi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-21 23:44:29.000000 ta-cmi-2.0.2/ta_cmi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-21 23:44:29.000000 ta-cmi-2.0.2/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 15:24:13.663198 ta-cmi-2.1.2.dev0/
+-rw-rw-rw-   0        0        0     1067 2023-04-18 18:49:16.000000 ta-cmi-2.1.2.dev0/LICENSE
+-rw-rw-rw-   0        0        0     8236 2023-06-23 15:24:13.662682 ta-cmi-2.1.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     6511 2023-04-18 20:27:27.000000 ta-cmi-2.1.2.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 15:24:13.663198 ta-cmi-2.1.2.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      639 2023-06-23 15:24:07.000000 ta-cmi-2.1.2.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 15:24:13.651378 ta-cmi-2.1.2.dev0/ta_cmi/
+-rw-rw-rw-   0        0        0      423 2023-04-21 23:42:49.000000 ta-cmi-2.1.2.dev0/ta_cmi/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-06-22 14:12:04.000000 ta-cmi-2.1.2.dev0/ta_cmi/api.py
+-rw-rw-rw-   0        0        0     1212 2023-04-21 23:42:39.000000 ta-cmi-2.1.2.dev0/ta_cmi/channel.py
+-rw-rw-rw-   0        0        0      638 2023-04-18 18:49:16.000000 ta-cmi-2.1.2.dev0/ta_cmi/cmi.py
+-rw-rw-rw-   0        0        0     2618 2023-06-22 12:53:24.000000 ta-cmi-2.1.2.dev0/ta_cmi/cmi_api.py
+-rw-rw-rw-   0        0        0      527 2023-04-21 23:42:39.000000 ta-cmi-2.1.2.dev0/ta_cmi/cmi_channel.py
+-rw-rw-rw-   0        0        0     2469 2023-06-22 16:11:01.000000 ta-cmi-2.1.2.dev0/ta_cmi/coe.py
+-rw-rw-rw-   0        0        0     4351 2023-06-22 15:13:25.000000 ta-cmi-2.1.2.dev0/ta_cmi/coe_api.py
+-rw-rw-rw-   0        0        0      403 2023-04-21 23:42:39.000000 ta-cmi-2.1.2.dev0/ta_cmi/coe_channel.py
+-rw-rw-rw-   0        0        0     3514 2023-04-18 18:49:17.000000 ta-cmi-2.1.2.dev0/ta_cmi/const.py
+-rw-rw-rw-   0        0        0     4467 2023-04-21 23:05:23.000000 ta-cmi-2.1.2.dev0/ta_cmi/device.py
+drwxrwxrwx   0        0        0        0 2023-06-23 15:24:13.655375 ta-cmi-2.1.2.dev0/ta_cmi.egg-info/
+-rw-rw-rw-   0        0        0     8236 2023-06-23 15:24:13.000000 ta-cmi-2.1.2.dev0/ta_cmi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-23 15:24:13.000000 ta-cmi-2.1.2.dev0/ta_cmi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 15:24:13.000000 ta-cmi-2.1.2.dev0/ta_cmi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-23 15:24:13.000000 ta-cmi-2.1.2.dev0/ta_cmi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 15:24:13.000000 ta-cmi-2.1.2.dev0/ta_cmi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 15:24:13.661610 ta-cmi-2.1.2.dev0/tests/
+-rw-rw-rw-   0        0        0     3672 2023-06-22 14:19:28.000000 ta-cmi-2.1.2.dev0/tests/test_api.py
+-rw-rw-rw-   0        0        0      624 2023-04-18 18:49:17.000000 ta-cmi-2.1.2.dev0/tests/test_cmi.py
+-rw-rw-rw-   0        0        0     5005 2023-06-22 13:06:44.000000 ta-cmi-2.1.2.dev0/tests/test_cmi_api.py
+-rw-rw-rw-   0        0        0      967 2023-04-18 18:49:17.000000 ta-cmi-2.1.2.dev0/tests/test_cmi_channel.py
+-rw-rw-rw-   0        0        0     3974 2023-06-22 16:19:45.000000 ta-cmi-2.1.2.dev0/tests/test_coe.py
+-rw-rw-rw-   0        0        0     4151 2023-06-22 15:14:17.000000 ta-cmi-2.1.2.dev0/tests/test_coe_api.py
+-rw-rw-rw-   0        0        0    11517 2023-04-18 18:49:17.000000 ta-cmi-2.1.2.dev0/tests/test_device.py
```

### Comparing `ta-cmi-2.0.2/LICENSE` & `ta-cmi-2.1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.0.2/PKG-INFO` & `ta-cmi-2.1.2.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-Metadata-Version: 2.1
-Name: ta-cmi
-Version: 2.0.2
-Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
-Home-page: https://gitlab.com/DeerMaximum/ta-cmi
-Author: DeerMaximum
-Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
-License: MIT License
-        
-        Copyright (c) 2021 DeerMaximum
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TA-CMI
-A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
-
-## How to use package
-
-### Json API
-
-```python
-import asyncio
-
-from ta_cmi import CMI, Languages, ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError, ChannelType
-
-
-async def main():
-    try:
-        cmi = CMI("http://192.168.1.101", "admin", "admin")
-
-        devices = await cmi.get_devices()
-
-        device = devices[0]
-
-        # Set type automatically
-        await device.fetch_type()
-
-        # Set type manually
-        device.set_device_type("UVR16x2")
-
-        await device.update()
-
-        print(str(device))
-
-        inputChannels = device.get_channels(ChannelType.INPUT)
-        outputChannels = device.get_channels(ChannelType.OUTPUT)
-        analogLogging = device.get_channels(ChannelType.ANALOG_LOGGING)
-
-        for i in inputChannels:
-            ch = inputChannels.get(i)
-            print(str(ch))
-
-        for o in outputChannels:
-            ch = outputChannels.get(o)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-        for al in analogLogging:
-            ch = analogLogging.get(al)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
-        print(f"Error: {error}")
-
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-loop.close()
-```
-
-## Supported data types
-
-| Device type | Inputs | Outputs | DL-inputs | System-values: General | System-values: Date | System-values: Time | System-values: Sun | System-values: Electrical power | Analog network inputs | Digital network inputs | M-Bus | Modbus | KNX | Analog logging | Digital logging |
-|-------------|:------:|:-------:|:---------:|:----------------------:|:-------------------:|:-------------------:|:------------------:|:-------------------------------:|:---------------------:|:----------------------:|:-----:|:------:|:---:|:--------------:|:---------------:|
-| UVR1611     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ✔           |           ✔            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| UVR16x2     |   ✔    |    ✔    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ✔        |        ✔        |
-| RSM610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-I/O45   |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-EZ2     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ✔                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-MTx2    |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-BC2     |   ❌    |    ❌    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ✔    |  ✔  |       ❌        |        ❌        |
-| UVR65       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-EZ3     |   ❌    |    ❌    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ✔                |           ❌           |           ❌            |   ❌   |   ✔    |  ❌  |       ✔        |        ✔        |
-| UVR610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
-| UVR67       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-
-> **Note**
-> The supported data types may differ from the official API. If a device type supports other data types than listed here, please create an issue.
-
-### CoE Server
-
-Data can be retrieved using [this](https://gitlab.com/DeerMaximum/ta-coe) CoE to HTTP server
-
-```python
-import asyncio
-
-from ta_cmi import (
-    ApiError,
-    ChannelMode,
-    CoE,
-    InvalidCredentialsError,
-    InvalidDeviceError,
-    Languages,
-    RateLimitError,
-)
-
-
-async def main():
-    try:
-        coe = CoE("http://192.168.2.201:9000")
-
-        await coe.update()
-
-        analog_channels = coe.get_channels(ChannelMode.ANALOG)
-        digital_channels = coe.get_channels(ChannelMode.DIGITAL)
-
-        for i in analog_channels:
-            ch = analog_channels.get(i)
-            print(str(ch))
-
-        for o in digital_channels:
-            ch = digital_channels.get(o)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
-        print(f"Error: {error}")
-
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-loop.close()
-```
+Metadata-Version: 2.1
+Name: ta-cmi
+Version: 2.1.2.dev0
+Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+Home-page: https://gitlab.com/DeerMaximum/ta-cmi
+Author: DeerMaximum
+Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
+License: MIT License
+        
+        Copyright (c) 2021 DeerMaximum
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# TA-CMI
+A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+
+## How to use package
+
+### Json API
+
+```python
+import asyncio
+
+from ta_cmi import CMI, Languages, ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError, ChannelType
+
+
+async def main():
+    try:
+        cmi = CMI("http://192.168.1.101", "admin", "admin")
+
+        devices = await cmi.get_devices()
+
+        device = devices[0]
+
+        # Set type automatically
+        await device.fetch_type()
+
+        # Set type manually
+        device.set_device_type("UVR16x2")
+
+        await device.update()
+
+        print(str(device))
+
+        inputChannels = device.get_channels(ChannelType.INPUT)
+        outputChannels = device.get_channels(ChannelType.OUTPUT)
+        analogLogging = device.get_channels(ChannelType.ANALOG_LOGGING)
+
+        for i in inputChannels:
+            ch = inputChannels.get(i)
+            print(str(ch))
+
+        for o in outputChannels:
+            ch = outputChannels.get(o)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+        for al in analogLogging:
+            ch = analogLogging.get(al)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
+        print(f"Error: {error}")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+loop.close()
+```
+
+## Supported data types
+
+| Device type | Inputs | Outputs | DL-inputs | System-values: General | System-values: Date | System-values: Time | System-values: Sun | System-values: Electrical power | Analog network inputs | Digital network inputs | M-Bus | Modbus | KNX | Analog logging | Digital logging |
+|-------------|:------:|:-------:|:---------:|:----------------------:|:-------------------:|:-------------------:|:------------------:|:-------------------------------:|:---------------------:|:----------------------:|:-----:|:------:|:---:|:--------------:|:---------------:|
+| UVR1611     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ✔           |           ✔            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| UVR16x2     |   ✔    |    ✔    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ✔        |        ✔        |
+| RSM610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-I/O45   |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-EZ2     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ✔                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-MTx2    |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-BC2     |   ❌    |    ❌    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ✔    |  ✔  |       ❌        |        ❌        |
+| UVR65       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-EZ3     |   ❌    |    ❌    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ✔                |           ❌           |           ❌            |   ❌   |   ✔    |  ❌  |       ✔        |        ✔        |
+| UVR610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
+| UVR67       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+
+> **Note**
+> The supported data types may differ from the official API. If a device type supports other data types than listed here, please create an issue.
+
+### CoE Server
+
+Data can be retrieved using [this](https://gitlab.com/DeerMaximum/ta-coe) CoE to HTTP server
+
+```python
+import asyncio
+
+from ta_cmi import (
+    ApiError,
+    ChannelMode,
+    CoE,
+    InvalidCredentialsError,
+    InvalidDeviceError,
+    Languages,
+    RateLimitError,
+)
+
+
+async def main():
+    try:
+        coe = CoE("http://192.168.2.201:9000")
+
+        await coe.update()
+
+        analog_channels = coe.get_channels(ChannelMode.ANALOG)
+        digital_channels = coe.get_channels(ChannelMode.DIGITAL)
+
+        for i in analog_channels:
+            ch = analog_channels.get(i)
+            print(str(ch))
+
+        for o in digital_channels:
+            ch = digital_channels.get(o)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
+        print(f"Error: {error}")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+loop.close()
+```
```

### Comparing `ta-cmi-2.0.2/README.md` & `ta-cmi-2.1.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.0.2/setup.py` & `ta-cmi-2.1.2.dev0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
-with open("README.md", "r") as f:
+with open("README.md", "r", encoding="utf8") as f:
     readme = f.read()
 
-with open("LICENSE", "r") as f:
+with open("LICENSE", "r", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="ta-cmi",
-    version="2.0.2",
+    version="2.1.2.dev",
     description="A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/DeerMaximum/ta-cmi",
     author="DeerMaximum",
     author_email="2629822-DeerMaximum@users.noreply.gitlab.com",
     license=license,
```

### Comparing `ta-cmi-2.0.2/ta_cmi/cmi.py` & `ta-cmi-2.1.2.dev0/ta_cmi/cmi.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.0.2/ta_cmi/cmi_api.py` & `ta-cmi-2.1.2.dev0/ta_cmi/cmi_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         url: str = f"{self.host}{self.DEVICE_DATA.replace('PARAMS', parameter).replace('ID', node_id)}"
 
         return await self._make_data_request(url)
 
     async def _make_data_request(self, url: str) -> Dict[str, Any]:
         """Retrieve data from CMI API."""
-        data = await self._make_request(url)
+        data = await self._make_request_get(url)
 
         STATUS_CODE = "Status code"
 
         if data[STATUS_CODE] != 0:
             _LOGGER.debug("Failed response received: %s", json.dumps(data))
 
         if data[STATUS_CODE] == 0:
```

### Comparing `ta-cmi-2.0.2/ta_cmi/const.py` & `ta-cmi-2.1.2.dev0/ta_cmi/const.py`

 * *Files identical despite different names*

### Comparing `ta-cmi-2.0.2/ta_cmi/device.py` & `ta-cmi-2.1.2.dev0/ta_cmi/device.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import asyncio
-from typing import Any, Dict, List
-
-from .channel import Channel
-from .cmi_api import CMIAPI
-from .cmi_channel import CMIChannel
-from .const import _LOGGER, DEVICES, SUPPORTED_PARAMS_FOR_DEVICE, ChannelType
-
-
-class Device:
-    """Class to interact with a device."""
-
-    def __init__(self, node_id: str, api: CMIAPI) -> None:
-        """Initialize."""
-        super().__init__()
-
-        self._channels: Dict[ChannelType, Dict[int, CMIChannel]] = {}
-
-        self.id = node_id
-        self._api = api
-
-        self.api_version: int = 0
-        self.device_id: str = "00"
-
-    def _extract_device_info(self, json: Dict[str, Any]) -> None:
-        """Extract device info from request response."""
-        self.api_version: int = json["Header"]["Version"]
-        self.device_id: str = json["Header"]["Device"]
-
-        if self.device_id not in DEVICES.keys():
-            raise InvalidDeviceError(f"Invalid device id: {self.device_id}")
-
-    @staticmethod
-    def _extract_channels(
-        mode: ChannelType, raw_channels: List[Dict[str, Any]]
-    ) -> Dict[int, CMIChannel]:
-        """Extract channel info from data array from request."""
-        list_of_channels: Dict[int, CMIChannel] = {}
-        for channel_raw in raw_channels:
-            ch: CMIChannel = CMIChannel(mode, channel_raw)
-            list_of_channels[ch.index] = ch
-
-        return list_of_channels
-
-    def _get_json_params(self) -> str:
-        """Compose json params based on the device type."""
-        default_params = "I,O"
-        return SUPPORTED_PARAMS_FOR_DEVICE.get(self.device_id, default_params)
-
-    async def _make_request_to_device(self) -> Dict[str, Any]:
-        """Make a request to the device."""
-        params = self._get_json_params()
-
-        data: dict[str, Any] = {}
-
-        if len(params.split(",")) > 7:
-            first_params = ",".join(params.split(",")[:7])
-            params = ",".join(params.split(",")[7:])
-
-            data = await self._api.get_device_data(self.id, first_params)
-
-            await asyncio.sleep(61)
-
-        if len(data.keys()) == 0:
-            return await self._api.get_device_data(self.id, params)
-
-        data["Data"].update((await self._api.get_device_data(self.id, params))["Data"])
-
-        return data
-
-    async def fetch_type(self) -> None:
-        """Fetch the device type without parsing the data from the device."""
-        self._extract_device_info(await self._make_request_to_device())
-
-    async def update(self) -> None:
-        """Update data."""
-        _LOGGER.debug("Update device: %s", self.id)
-        res: Dict[str, Any] = await self._make_request_to_device()
-
-        if self.device_id == "00":
-            self._extract_device_info(res)
-            _LOGGER.debug("Device had no id. Set new id to %s", self.device_id)
-
-        for channel_type_text in res["Data"]:
-            channel_type = ChannelType(channel_type_text)
-            self._channels[channel_type] = self._extract_channels(
-                channel_type, res["Data"][channel_type_text]
-            )
-
-    def set_device_type(self, device_name: str) -> None:
-        """Set the type of the device manually."""
-        type_id = [i for i in DEVICES if DEVICES[i] == device_name]
-
-        if len(type_id) != 1:
-            raise InvalidDeviceError(f"Invalid device name: {device_name}")
-
-        self.device_id = type_id[0]
-
-    def get_device_type(self) -> str:
-        """Get the type of the device."""
-        return DEVICES.get(self.device_id, "Unknown")
-
-    def get_channels(self, channel_type: ChannelType) -> Dict[int, CMIChannel]:
-        """Get all the fetched channels from a type."""
-        return self._channels.get(channel_type, {})
-
-    def has_channel_type(self, channel_type: ChannelType) -> bool:
-        """Check if a channel type was fetched."""
-        return self._channels.get(channel_type, None) is not None
-
-    def __repr__(self) -> str:
-        text = f"Node {self.id}: Type: {self.get_device_type()}"
-
-        for channel_type in self._channels:
-            text += f", {channel_type.value}: {len(self._channels[channel_type])}"
-
-        return text
-
-
-class InvalidDeviceError(Exception):
-    """Triggered when an invalid device type is set."""
-
-    def __init__(self, status: str) -> None:
-        """Initialize."""
-        super().__init__(status)
-        self.status = status
+import asyncio
+from typing import Any, Dict, List
+
+from .channel import Channel
+from .cmi_api import CMIAPI
+from .cmi_channel import CMIChannel
+from .const import _LOGGER, DEVICES, SUPPORTED_PARAMS_FOR_DEVICE, ChannelType
+
+
+class Device:
+    """Class to interact with a device."""
+
+    def __init__(self, node_id: str, api: CMIAPI) -> None:
+        """Initialize."""
+        super().__init__()
+
+        self._channels: Dict[ChannelType, Dict[int, CMIChannel]] = {}
+
+        self.id = node_id
+        self._api = api
+
+        self.api_version: int = 0
+        self.device_id: str = "00"
+
+    def _extract_device_info(self, json: Dict[str, Any]) -> None:
+        """Extract device info from request response."""
+        self.api_version: int = json["Header"]["Version"]
+        self.device_id: str = json["Header"]["Device"]
+
+        if self.device_id not in DEVICES.keys():
+            raise InvalidDeviceError(f"Invalid device id: {self.device_id}")
+
+    @staticmethod
+    def _extract_channels(
+        mode: ChannelType, raw_channels: List[Dict[str, Any]]
+    ) -> Dict[int, CMIChannel]:
+        """Extract channel info from data array from request."""
+        list_of_channels: Dict[int, CMIChannel] = {}
+        for channel_raw in raw_channels:
+            ch: CMIChannel = CMIChannel(mode, channel_raw)
+            list_of_channels[ch.index] = ch
+
+        return list_of_channels
+
+    def _get_json_params(self) -> str:
+        """Compose json params based on the device type."""
+        default_params = "I,O"
+        return SUPPORTED_PARAMS_FOR_DEVICE.get(self.device_id, default_params)
+
+    async def _make_request_to_device(self) -> Dict[str, Any]:
+        """Make a request to the device."""
+        params = self._get_json_params()
+
+        data: dict[str, Any] = {}
+
+        if len(params.split(",")) > 7:
+            first_params = ",".join(params.split(",")[:7])
+            params = ",".join(params.split(",")[7:])
+
+            data = await self._api.get_device_data(self.id, first_params)
+
+            await asyncio.sleep(61)
+
+        if len(data.keys()) == 0:
+            return await self._api.get_device_data(self.id, params)
+
+        data["Data"].update((await self._api.get_device_data(self.id, params))["Data"])
+
+        return data
+
+    async def fetch_type(self) -> None:
+        """Fetch the device type without parsing the data from the device."""
+        self._extract_device_info(await self._make_request_to_device())
+
+    async def update(self) -> None:
+        """Update data."""
+        _LOGGER.debug("Update device: %s", self.id)
+        res: Dict[str, Any] = await self._make_request_to_device()
+
+        if self.device_id == "00":
+            self._extract_device_info(res)
+            _LOGGER.debug("Device had no id. Set new id to %s", self.device_id)
+
+        for channel_type_text in res["Data"]:
+            channel_type = ChannelType(channel_type_text)
+            self._channels[channel_type] = self._extract_channels(
+                channel_type, res["Data"][channel_type_text]
+            )
+
+    def set_device_type(self, device_name: str) -> None:
+        """Set the type of the device manually."""
+        type_id = [i for i in DEVICES if DEVICES[i] == device_name]
+
+        if len(type_id) != 1:
+            raise InvalidDeviceError(f"Invalid device name: {device_name}")
+
+        self.device_id = type_id[0]
+
+    def get_device_type(self) -> str:
+        """Get the type of the device."""
+        return DEVICES.get(self.device_id, "Unknown")
+
+    def get_channels(self, channel_type: ChannelType) -> Dict[int, CMIChannel]:
+        """Get all the fetched channels from a type."""
+        return self._channels.get(channel_type, {})
+
+    def has_channel_type(self, channel_type: ChannelType) -> bool:
+        """Check if a channel type was fetched."""
+        return self._channels.get(channel_type, None) is not None
+
+    def __repr__(self) -> str:
+        text = f"Node {self.id}: Type: {self.get_device_type()}"
+
+        for channel_type in self._channels:
+            text += f", {channel_type.value}: {len(self._channels[channel_type])}"
+
+        return text
+
+
+class InvalidDeviceError(Exception):
+    """Triggered when an invalid device type is set."""
+
+    def __init__(self, status: str) -> None:
+        """Initialize."""
+        super().__init__(status)
+        self.status = status
```

### Comparing `ta-cmi-2.0.2/ta_cmi.egg-info/PKG-INFO` & `ta-cmi-2.1.2.dev0/ta_cmi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-Metadata-Version: 2.1
-Name: ta-cmi
-Version: 2.0.2
-Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
-Home-page: https://gitlab.com/DeerMaximum/ta-cmi
-Author: DeerMaximum
-Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
-License: MIT License
-        
-        Copyright (c) 2021 DeerMaximum
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TA-CMI
-A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
-
-## How to use package
-
-### Json API
-
-```python
-import asyncio
-
-from ta_cmi import CMI, Languages, ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError, ChannelType
-
-
-async def main():
-    try:
-        cmi = CMI("http://192.168.1.101", "admin", "admin")
-
-        devices = await cmi.get_devices()
-
-        device = devices[0]
-
-        # Set type automatically
-        await device.fetch_type()
-
-        # Set type manually
-        device.set_device_type("UVR16x2")
-
-        await device.update()
-
-        print(str(device))
-
-        inputChannels = device.get_channels(ChannelType.INPUT)
-        outputChannels = device.get_channels(ChannelType.OUTPUT)
-        analogLogging = device.get_channels(ChannelType.ANALOG_LOGGING)
-
-        for i in inputChannels:
-            ch = inputChannels.get(i)
-            print(str(ch))
-
-        for o in outputChannels:
-            ch = outputChannels.get(o)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-        for al in analogLogging:
-            ch = analogLogging.get(al)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
-        print(f"Error: {error}")
-
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-loop.close()
-```
-
-## Supported data types
-
-| Device type | Inputs | Outputs | DL-inputs | System-values: General | System-values: Date | System-values: Time | System-values: Sun | System-values: Electrical power | Analog network inputs | Digital network inputs | M-Bus | Modbus | KNX | Analog logging | Digital logging |
-|-------------|:------:|:-------:|:---------:|:----------------------:|:-------------------:|:-------------------:|:------------------:|:-------------------------------:|:---------------------:|:----------------------:|:-----:|:------:|:---:|:--------------:|:---------------:|
-| UVR1611     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ✔           |           ✔            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| UVR16x2     |   ✔    |    ✔    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ✔        |        ✔        |
-| RSM610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-I/O45   |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-EZ2     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ✔                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-MTx2    |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-BC2     |   ❌    |    ❌    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ✔    |  ✔  |       ❌        |        ❌        |
-| UVR65       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-| CAN-EZ3     |   ❌    |    ❌    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ✔                |           ❌           |           ❌            |   ❌   |   ✔    |  ❌  |       ✔        |        ✔        |
-| UVR610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
-| UVR67       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
-
-> **Note**
-> The supported data types may differ from the official API. If a device type supports other data types than listed here, please create an issue.
-
-### CoE Server
-
-Data can be retrieved using [this](https://gitlab.com/DeerMaximum/ta-coe) CoE to HTTP server
-
-```python
-import asyncio
-
-from ta_cmi import (
-    ApiError,
-    ChannelMode,
-    CoE,
-    InvalidCredentialsError,
-    InvalidDeviceError,
-    Languages,
-    RateLimitError,
-)
-
-
-async def main():
-    try:
-        coe = CoE("http://192.168.2.201:9000")
-
-        await coe.update()
-
-        analog_channels = coe.get_channels(ChannelMode.ANALOG)
-        digital_channels = coe.get_channels(ChannelMode.DIGITAL)
-
-        for i in analog_channels:
-            ch = analog_channels.get(i)
-            print(str(ch))
-
-        for o in digital_channels:
-            ch = digital_channels.get(o)
-            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
-
-    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
-        print(f"Error: {error}")
-
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-loop.close()
-```
+Metadata-Version: 2.1
+Name: ta-cmi
+Version: 2.1.2.dev0
+Summary: A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+Home-page: https://gitlab.com/DeerMaximum/ta-cmi
+Author: DeerMaximum
+Author-email: 2629822-DeerMaximum@users.noreply.gitlab.com
+License: MIT License
+        
+        Copyright (c) 2021 DeerMaximum
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# TA-CMI
+A Python wrapper to read out  sensors from Technische Alternative using the C.M.I.
+
+## How to use package
+
+### Json API
+
+```python
+import asyncio
+
+from ta_cmi import CMI, Languages, ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError, ChannelType
+
+
+async def main():
+    try:
+        cmi = CMI("http://192.168.1.101", "admin", "admin")
+
+        devices = await cmi.get_devices()
+
+        device = devices[0]
+
+        # Set type automatically
+        await device.fetch_type()
+
+        # Set type manually
+        device.set_device_type("UVR16x2")
+
+        await device.update()
+
+        print(str(device))
+
+        inputChannels = device.get_channels(ChannelType.INPUT)
+        outputChannels = device.get_channels(ChannelType.OUTPUT)
+        analogLogging = device.get_channels(ChannelType.ANALOG_LOGGING)
+
+        for i in inputChannels:
+            ch = inputChannels.get(i)
+            print(str(ch))
+
+        for o in outputChannels:
+            ch = outputChannels.get(o)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+        for al in analogLogging:
+            ch = analogLogging.get(al)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
+        print(f"Error: {error}")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+loop.close()
+```
+
+## Supported data types
+
+| Device type | Inputs | Outputs | DL-inputs | System-values: General | System-values: Date | System-values: Time | System-values: Sun | System-values: Electrical power | Analog network inputs | Digital network inputs | M-Bus | Modbus | KNX | Analog logging | Digital logging |
+|-------------|:------:|:-------:|:---------:|:----------------------:|:-------------------:|:-------------------:|:------------------:|:-------------------------------:|:---------------------:|:----------------------:|:-----:|:------:|:---:|:--------------:|:---------------:|
+| UVR1611     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ✔           |           ✔            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| UVR16x2     |   ✔    |    ✔    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ✔        |        ✔        |
+| RSM610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-I/O45   |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-EZ2     |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ✔                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-MTx2    |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-BC2     |   ❌    |    ❌    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ✔    |  ✔  |       ❌        |        ❌        |
+| UVR65       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+| CAN-EZ3     |   ❌    |    ❌    |     ✔     |           ✔            |          ✔          |          ✔          |         ✔          |                ✔                |           ❌           |           ❌            |   ❌   |   ✔    |  ❌  |       ✔        |        ✔        |
+| UVR610      |   ✔    |    ✔    |     ✔     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ✔   |   ❌    |  ❌  |       ❌        |        ❌        |
+| UVR67       |   ✔    |    ✔    |     ❌     |           ❌            |          ❌          |          ❌          |         ❌          |                ❌                |           ❌           |           ❌            |   ❌   |   ❌    |  ❌  |       ❌        |        ❌        |
+
+> **Note**
+> The supported data types may differ from the official API. If a device type supports other data types than listed here, please create an issue.
+
+### CoE Server
+
+Data can be retrieved using [this](https://gitlab.com/DeerMaximum/ta-coe) CoE to HTTP server
+
+```python
+import asyncio
+
+from ta_cmi import (
+    ApiError,
+    ChannelMode,
+    CoE,
+    InvalidCredentialsError,
+    InvalidDeviceError,
+    Languages,
+    RateLimitError,
+)
+
+
+async def main():
+    try:
+        coe = CoE("http://192.168.2.201:9000")
+
+        await coe.update()
+
+        analog_channels = coe.get_channels(ChannelMode.ANALOG)
+        digital_channels = coe.get_channels(ChannelMode.DIGITAL)
+
+        for i in analog_channels:
+            ch = analog_channels.get(i)
+            print(str(ch))
+
+        for o in digital_channels:
+            ch = digital_channels.get(o)
+            print(f"{str(ch)} - {ch.get_unit(Languages.DE)}")
+
+    except (ApiError, RateLimitError, InvalidCredentialsError, InvalidDeviceError) as error:
+        print(f"Error: {error}")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+loop.close()
+```
```

