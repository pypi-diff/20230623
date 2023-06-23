# Comparing `tmp/zigpy-xbee-0.18.0.tar.gz` & `tmp/zigpy-xbee-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-xbee-0.18.0.tar", last modified: Mon Apr 24 18:12:50 2023, max compression
+gzip compressed data, was "zigpy-xbee-0.18.1.tar", last modified: Fri Jun 23 14:43:35 2023, max compression
```

## Comparing `zigpy-xbee-0.18.0.tar` & `zigpy-xbee-0.18.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/zigpy_xbee/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/zigpy_xbee/zigbee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/zigbee/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:43:35.152186 zigpy-xbee-0.18.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-23 14:43:35.152186 zigpy-xbee-0.18.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-23 14:43:35.152186 zigpy-xbee-0.18.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:43:35.148186 zigpy-xbee-0.18.1/zigpy_xbee/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/zigpy_xbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/zigpy_xbee/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/zigpy_xbee/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/zigpy_xbee/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/zigpy_xbee/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:43:35.152186 zigpy-xbee-0.18.1/zigpy_xbee/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/zigpy_xbee/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-06-23 14:43:31.000000 zigpy-xbee-0.18.1/zigpy_xbee/zigbee/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:43:35.152186 zigpy-xbee-0.18.1/zigpy_xbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-23 14:43:35.000000 zigpy-xbee-0.18.1/zigpy_xbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-23 14:43:35.000000 zigpy-xbee-0.18.1/zigpy_xbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:43:35.000000 zigpy-xbee-0.18.1/zigpy_xbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 14:43:35.000000 zigpy-xbee-0.18.1/zigpy_xbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 14:43:35.000000 zigpy-xbee-0.18.1/zigpy_xbee.egg-info/top_level.txt
```

### Comparing `zigpy-xbee-0.18.0/COPYING` & `zigpy-xbee-0.18.1/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.18.0/LICENSE` & `zigpy-xbee-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.18.0/PKG-INFO` & `zigpy-xbee-0.18.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-xbee
-Version: 0.18.0
+Version: 0.18.1
 Summary: A library which communicates with XBee radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-xbee
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zigpy-xbee-0.18.0/README.md` & `zigpy-xbee-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.18.0/setup.cfg` & `zigpy-xbee-0.18.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.18.0/setup.py` & `zigpy-xbee-0.18.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="http://github.com/zigpy/zigpy-xbee",
     author="Russell Cloran",
     author_email="rcloran@gmail.com",
     license="GPL-3.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
-    install_requires=["zigpy>=0.51.0"],
+    install_requires=["zigpy>=0.56.0"],
     tests_require=["pytest", "asynctest", "pytest-asyncio"],
 )
```

### Comparing `zigpy-xbee-0.18.0/zigpy_xbee/api.py` & `zigpy-xbee-0.18.1/zigpy_xbee/api.py`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.18.0/zigpy_xbee/types.py` & `zigpy-xbee-0.18.1/zigpy_xbee/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.18.0/zigpy_xbee/uart.py` & `zigpy-xbee-0.18.1/zigpy_xbee/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.18.0/zigpy_xbee/zigbee/application.py` & `zigpy-xbee-0.18.1/zigpy_xbee/zigbee/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,22 @@
     async def _move_network_to_channel(
         self, new_channel: int, new_nwk_update_id: int
     ) -> None:
         """Moves the coordinator to a new channel."""
         scan_bitmask = 1 << (new_channel - 11)
         await self._api._queued_at("SC", scan_bitmask)
 
+    async def energy_scan(
+        self, channels: zigpy.types.Channels, duration_exp: int, count: int
+    ) -> dict[int, float]:
+        """Runs an energy detection scan and returns the per-channel scan results."""
+
+        LOGGER.warning("Coordinator does not support energy scanning")
+        return {c: 0 for c in channels}
+
     async def force_remove(self, dev):
         """Forcibly remove device from NCP."""
         pass
 
     async def add_endpoint(self, descriptor):
         """Register a new endpoint on the device."""
         # This is not provided by the XBee API
@@ -251,15 +259,15 @@
             )
 
         if v != TXStatus.SUCCESS:
             raise zigpy.exceptions.DeliveryError(
                 f"Failed to deliver packet: {v!r}", status=v
             )
 
-    @zigpy.util.retryable_request
+    @zigpy.util.retryable_request()
     def remote_at_command(
         self, nwk, cmd_name, *args, apply_changes=True, encryption=True
     ):
         LOGGER.debug("Remote AT%s command: %s", cmd_name, args)
         options = zigpy.types.uint8_t(0)
         if apply_changes:
             options |= 0x02
```

### Comparing `zigpy-xbee-0.18.0/zigpy_xbee.egg-info/PKG-INFO` & `zigpy-xbee-0.18.1/zigpy_xbee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-xbee
-Version: 0.18.0
+Version: 0.18.1
 Summary: A library which communicates with XBee radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-xbee
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

