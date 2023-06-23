# Comparing `tmp/serial_packets-0.1.6.tar.gz` & `tmp/serial_packets-0.1.8.tar.gz`

## Comparing `serial_packets-0.1.6.tar` & `serial_packets-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.6/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 serial_packets-0.1.6/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 serial_packets-0.1.6/src/serial_packets/client.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 serial_packets-0.1.6/src/serial_packets/packet_decoder.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 serial_packets-0.1.6/src/serial_packets/packet_encoder.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.6/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.6/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.6/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.6/LICENSE
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.6/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/packet_decoder.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/packet_encoder.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.8/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.8/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.8/LICENSE
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.1.8/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.1.8/PKG-INFO
```

### Comparing `serial_packets-0.1.6/src/serial_packets/_packets.py` & `serial_packets-0.1.8/src/serial_packets/_packets.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,7 +32,8 @@
 
 # Do not change the numeric tags since the will change
 # the wire representation.
 class PacketType(Enum):
     COMMAND = 1
     RESPONSE = 2
     MESSAGE = 3
+    LOG = 4
```

### Comparing `serial_packets-0.1.6/src/serial_packets/client.py` & `serial_packets-0.1.8/src/serial_packets/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from enum import Enum
 from typing import Optional, Tuple, Dict, Callable
 from asyncio.transports import BaseTransport
 from .packet_encoder import PacketEncoder
 from .packet_decoder import PacketDecoder, DecodedCommandPacket, DecodedResponsePacket, DecodedMessagePacket
 from ._packets import PacketType, MAX_DATA_LEN, MIN_CMD_TIMEOUT, MAX_CMD_TIMEOUT, DEFAULT_CMD_TIMEOUT, MIN_WORKERS_COUNT, MAX_WORKERS_COUNT, DEFAULT_WORKERS_COUNT
-# from ._interval_tracker import IntervalTracker
 from .packets import PacketStatus, PacketsEvent, PacketsEventType, PacketsEvent, PacketData, MAX_USER_ENDPOINT
 
 logger = logging.getLogger(__name__)
 
 # pyserial_asyncio is documented at
 # https://github.com/pyserial/pyserial-asyncio
 
@@ -178,19 +177,15 @@
             logger.error("%s", e)
             if logging.DEBUG >= logger.getEffectiveLevel():
                 traceback.print_exception(e)
             return False
         self.__protocol.set(self, self.__port, self.__packet_decoder, self.__work_queue)
         return True
 
-    # def __on_decoded_packet(self, decoded_packet: DecodedCommandPacket | DecodedResponsePacket |
-    #                         DecodedMessagePacket):
-    #     """Called from the packet decoder on each receive packet"""
-    #     logger.debug("Queuing incoming packet of type [%s.]", type(decoded_packet).__name__)
-    #     self.__work_queue.put_nowait(decoded_packet)
+  
 
     def __create_loop_runner_task(self, task_loop, name):
         logger.debug("Creating task '%s'", name)
         task = asyncio.create_task(self.__loop_runner_task(task_loop), name=name)
         self.__background_tasks.append(task)
 
     async def __loop_runner_task(self, task_loop):
```

### Comparing `serial_packets-0.1.6/src/serial_packets/packet_decoder.py` & `serial_packets-0.1.8/src/serial_packets/packet_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,23 @@
 
     def __init__(self, endpoint: int, data: PacketData):
         self.endpoint: int = endpoint
         self.data: PacketData = data
 
     def __str__(self):
         return f"Message packet: {self.endpoint}, {self.data.size()}"
+      
+      
+class DecodedLogPacket:
+
+    def __init__(self,  data: PacketData):
+        self.data: PacketData = data
+
+    def __str__(self):
+        return f"Log packet: {self.data.size()}"
 
 
 class PacketDecoder:
 
     def __init__(self):
         # assert (decoded_packet_callback is not None)
         self.__crc_calc = CRCCCITT("FFFF")
@@ -58,21 +67,15 @@
         return f"In_packet ={self.__in_packet}, pending_escape={self.__pending_escape}, len={len(self.__packet_bytes)}"
 
     def __reset_packet(self, in_packet: bool):
         self.__in_packet = in_packet
         self.__pending_escape = False
         self.__packet_bfr.clear()
 
-    # async def get_next_packet(self):
-    #     """Blocking asyncio fetch of next pending packet."""
-    #     return await self.__packets_queue.get()
-
-    # def receive(self, data: bytes):
-    #     for b in data:
-    #         self.__receive_byte(b)
+   
 
     def receive_byte(
         self, b: int
     ) -> Optional(DecodedCommandPacket | DecodedResponsePacket
                   | DecodedMessagePacket):
         """ Returns a decoded packet or None."""
         # If not already in a packet, wait for next flag.
@@ -173,17 +176,20 @@
             status = rx_bfr[5]
             data = PacketData().add_bytes(rx_bfr[6:-2])
             decoded_packet = DecodedResponsePacket(cmd_id, status, data)
         elif type_value == PacketType.MESSAGE.value:
             endpoint = rx_bfr[1]
             data = PacketData().add_bytes(rx_bfr[2:-2])
             decoded_packet = DecodedMessagePacket(endpoint, data)
+        elif type_value == PacketType.LOG.value:
+            data = PacketData().add_bytes(rx_bfr[1:-2])
+            decoded_packet = DecodedLogPacket(data)
         else:
             logger.error("Invalid packet type %02x, dropping packet",
-                         type.value)
+                         type_value)
             return None
 
         if data.size() > MAX_DATA_LEN:
             logger.error("Packet data too long (type=%d, len=%d), dropping",
                          type_value, data.size())
             return None
```

### Comparing `serial_packets-0.1.6/src/serial_packets/packet_encoder.py` & `serial_packets-0.1.8/src/serial_packets/packet_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,24 @@
         packet.append(PacketType.MESSAGE.value)
         packet.append(endpoint)
         packet.extend(data)
         crc = self.__crc_calc.calculate(bytes(packet))
         packet.extend(crc.to_bytes(2, 'big'))
         assert (len(packet) <= MAX_PACKET_LEN)
         return packet
+      
+    def __construct_log_packet(self,  data: bytearray):
+        """Constructs a log packet, before byte stuffing"""
+        packet = bytearray()
+        packet.append(PacketType.LOG.value)
+        packet.extend(data)
+        crc = self.__crc_calc.calculate(bytes(packet))
+        packet.extend(crc.to_bytes(2, 'big'))
+        assert (len(packet) <= MAX_PACKET_LEN)
+        return packet
 
     def __byte_stuffing(self, packet: bytearray):
         """Byte stuff the packet using HDLC format. Also adds packet flag(s)"""
         result = bytearray()
         result.append(PACKET_START_FLAG)
         for byte in packet:
             if byte == PACKET_START_FLAG or byte == PACKET_END_FLAG or byte == PACKET_ESC:
@@ -79,7 +89,14 @@
 
     def encode_message_packet(self, endpoint: int, data: bytearray):
         """Returns the message packet in wire format"""
         assert (len(data) <= MAX_DATA_LEN)
         packet = self.__construct_message_packet(endpoint, data)
         stuffed_packet = self.__byte_stuffing(packet)
         return stuffed_packet
+      
+    def encode_log_packet(self,  data: bytearray):
+        """Returns the log packet in wire format"""
+        assert (len(data) <= MAX_DATA_LEN)
+        packet = self.__construct_log_packet(data)
+        stuffed_packet = self.__byte_stuffing(packet)
+        return stuffed_packet
```

### Comparing `serial_packets-0.1.6/src/serial_packets/packets.py` & `serial_packets-0.1.8/src/serial_packets/packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.6/LICENSE` & `serial_packets-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.6/README.md` & `serial_packets-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.6/pyproject.toml` & `serial_packets-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.6"
+version = "0.1.8"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.6/PKG-INFO` & `serial_packets-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.6
+Version: 0.1.8
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

