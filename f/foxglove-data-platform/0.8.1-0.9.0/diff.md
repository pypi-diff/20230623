# Comparing `tmp/foxglove-data-platform-0.8.1.tar.gz` & `tmp/foxglove-data-platform-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-data-platform-0.8.1.tar", last modified: Thu Jun 15 16:46:42 2023, max compression
+gzip compressed data, was "foxglove-data-platform-0.9.0.tar", last modified: Fri Jun 16 19:16:29 2023, max compression
```

## Comparing `foxglove-data-platform-0.8.1.tar` & `foxglove-data-platform-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.623011 foxglove-data-platform-0.8.1/foxglove_data_platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/foxglove_data_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/foxglove_data_platform/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/foxglove_data_platform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.623011 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 16:46:42.000000 foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:46:42.627011 foxglove-data-platform-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/api_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/string_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_json_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_protobuf_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_ros1_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-15 16:45:54.000000 foxglove-data-platform-0.8.1/tests/test_ros2_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:16:29.511344 foxglove-data-platform-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 19:16:29.511344 foxglove-data-platform-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:16:29.507344 foxglove-data-platform-0.9.0/foxglove_data_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/foxglove_data_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29251 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/foxglove_data_platform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/foxglove_data_platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:16:29.511344 foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-16 19:16:29.000000 foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-16 19:16:29.000000 foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:16:29.000000 foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 19:16:29.000000 foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-16 19:16:29.000000 foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 19:16:29.511344 foxglove-data-platform-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:16:29.511344 foxglove-data-platform-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/string_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_json_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_protobuf_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_ros1_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-16 19:16:05.000000 foxglove-data-platform-0.9.0/tests/test_ros2_messages.py
```

### Comparing `foxglove-data-platform-0.8.1/LICENSE` & `foxglove-data-platform-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/PKG-INFO` & `foxglove-data-platform-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.8.1
+Version: 0.9.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.8.1/README.md` & `foxglove-data-platform-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/foxglove_data_platform/client.py` & `foxglove-data-platform-0.9.0/foxglove_data_platform/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,61 +7,54 @@
 from typing import IO, Any, Dict, List, Optional, Union
 import base64
 
 import arrow
 import requests
 from typing_extensions import Protocol
 
+from mcap.records import Schema as McapSchema
+from mcap.well_known import MessageEncoding
+from mcap.reader import make_reader
+from mcap.decoder import DecoderFactory
 
-try:
-    from mcap.records import Schema as McapSchema
-    from mcap.reader import make_reader
-except ModuleNotFoundError:
-    McapSchema = None
-    make_reader = None
 
+class _JsonDecoderFactory(DecoderFactory):
+    def decoder_for(self, message_encoding: str, schema: Optional[McapSchema]):
+        _ = schema
 
-def _err_on_construction(err):
-    def construct():
-        raise RuntimeError(f"Error importing decoder implementation: {err}")
+        def decoder(message_content: bytes):
+            return json.loads(message_content.decode("utf-8"))
 
-    return construct
+        if message_encoding == MessageEncoding.JSON:
+            return decoder
+        return None
 
 
+DEFAULT_DECODER_FACTORIES: List[DecoderFactory] = [_JsonDecoderFactory()]
+
 try:
-    from mcap_ros1.decoder import Decoder as Ros1Decoder
-except ModuleNotFoundError as err:
-    Ros1Decoder = _err_on_construction(err)
+    from mcap_ros1.decoder import DecoderFactory as Ros1DecoderFactory
+
+    DEFAULT_DECODER_FACTORIES.append(Ros1DecoderFactory())
+except ModuleNotFoundError:
+    pass
 
 try:
-    from mcap_protobuf.decoder import Decoder as ProtobufDecoder
-except ModuleNotFoundError as err:
-    ProtobufDecoder = _err_on_construction(err)
+    from mcap_protobuf.decoder import DecoderFactory as ProtobufDecoderFactory
+
+    DEFAULT_DECODER_FACTORIES.append(ProtobufDecoderFactory())
+except ModuleNotFoundError:
+    pass
 
 try:
-    from mcap_ros2.decoder import Decoder as Ros2Decoder
-except ModuleNotFoundError as err:
-    Ros2Decoder = _err_on_construction(err)
-
-
-class JsonDecoder:
-    def decode(self, schema_, message):
-        return json.loads(message.data.decode("utf-8"))
-
-
-def decoder_for_schema_encoding(encoding_string):
-    if encoding_string == "ros1msg":
-        return Ros1Decoder()
-    if encoding_string == "ros2msg":
-        return Ros2Decoder()
-    if encoding_string == "protobuf":
-        return ProtobufDecoder()
-    if encoding_string == "jsonschema":
-        return JsonDecoder()
-    raise RuntimeError(f"No known decoder class for encoding {encoding_string}")
+    from mcap_ros2.decoder import DecoderFactory as Ros2DecoderFactory
+
+    DEFAULT_DECODER_FACTORIES.append(Ros2DecoderFactory())
+except ModuleNotFoundError:
+    pass
 
 
 def camelize(snake_name: Optional[str]) -> Optional[str]:
     """
     Convert a valid snake_case field name to camelCase for the API
     """
     if not snake_name:
@@ -279,52 +272,46 @@
         self,
         *,
         device_id: Optional[str] = None,
         device_name: Optional[str] = None,
         start: datetime.datetime,
         end: datetime.datetime,
         topics: List[str] = [],
+        decoder_factories: Optional[List[DecoderFactory]] = None,
     ):
         """
         Returns a list of tuples of (topic, raw mcap record, decoded message).
 
         device_id: The id of the device that originated the desired data.
+        device_name: The name of the device that originated the desired data.
         start: The earliest time from which to retrieve data.
         end: The latest time from which to retrieve data.
         topics: An optional list of topics to retrieve.
             All topics will be retrieved if this is omitted.
+        decoder_factories: an optional list of :py:class:`~mcap.decoder.DecoderFactory` instances
+            used to decode message content.
         """
         if device_id is None and device_name is None:
             raise RuntimeError(
                 "device_id or device_name must be provided to get_messages"
             )
-        if not McapSchema or not make_reader:
-            raise RuntimeError(
-                "Mcap library not found. Please install the mcap library."
-            )
         data = self.download_data(
             device_name=device_name,
             device_id=device_id,
             start=start,
             end=end,
             topics=topics,
         )
-        reader = make_reader(BytesIO(data))
-        decoders = {}
-        output_messages = []
-        for schema, channel, message in reader.iter_messages():
-            if schema.encoding not in decoders:
-                decoder = decoder_for_schema_encoding(schema.encoding)
-                decoders[schema.encoding] = decoder
-            else:
-                decoder = decoders[schema.encoding]
-            output_messages.append(
-                (channel.topic, message, decoder.decode(schema, message))
-            )
-        return output_messages
+        if decoder_factories is None:
+            decoder_factories = DEFAULT_DECODER_FACTORIES
+        reader = make_reader(BytesIO(data), decoder_factories=decoder_factories)
+        return [
+            (channel.topic, message, decoded_message)
+            for _, channel, message, decoded_message in reader.iter_decoded_messages()
+        ]
 
     def download_recording_data(
         self,
         *,
         id: str,
         output_format: OutputFormat = OutputFormat.mcap0,
         include_attachments: bool = False,
```

### Comparing `foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/PKG-INFO` & `foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.8.1
+Version: 0.9.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.8.1/foxglove_data_platform.egg-info/SOURCES.txt` & `foxglove-data-platform-0.9.0/foxglove_data_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/setup.cfg` & `foxglove-data-platform-0.9.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-data-platform
-version = 0.8.1
+version = 0.9.0
 description = Client library for Foxglove Data Platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/py-data-platform
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 
 [options]
 include_package_data = True
 install_requires = 
 	arrow
 	requests
 	typing_extensions
+	mcap >= 1.1.0
 packages = find:
 python_requires = >=3.7
 
 [options.package_data]
 foxglove_data_platform = py.typed
 
 [egg_info]
```

### Comparing `foxglove-data-platform-0.8.1/tests/generate.py` & `foxglove-data-platform-0.9.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/string_message_pb2.py` & `foxglove-data-platform-0.9.0/tests/string_message_pb2.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_attachments.py` & `foxglove-data-platform-0.9.0/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_client.py` & `foxglove-data-platform-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_coverage.py` & `foxglove-data-platform-0.9.0/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_data.py` & `foxglove-data-platform-0.9.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_devices.py` & `foxglove-data-platform-0.9.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_events.py` & `foxglove-data-platform-0.9.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_imports.py` & `foxglove-data-platform-0.9.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_protobuf_messages.py` & `foxglove-data-platform-0.9.0/tests/test_protobuf_messages.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 
 from foxglove_data_platform.client import Client
 
 from .generate import generate_protobuf_data
 
 
 def test_download_without_decoder():
-    with patch(
-        "foxglove_data_platform.client.decoder_for_schema_encoding",
-        MagicMock(side_effect=Exception("Not found!")),
-    ):
+    with patch("foxglove_data_platform.client.DEFAULT_DECODER_FACTORIES", []):
         client = Client("test")
         client.download_data = MagicMock(return_value=generate_protobuf_data())
         with pytest.raises(Exception):
             client.get_messages(
                 device_id="test_id", start=datetime.now(), end=datetime.now()
             )
```

### Comparing `foxglove-data-platform-0.8.1/tests/test_recordings.py` & `foxglove-data-platform-0.9.0/tests/test_recordings.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.8.1/tests/test_ros1_messages.py` & `foxglove-data-platform-0.9.0/tests/test_ros2_messages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from datetime import datetime
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from foxglove_data_platform.client import Client
 
-from .generate import generate_ros1_data
+from .generate import generate_ros2_data
 
 
 def test_download_without_decoder():
-    with patch(
-        "foxglove_data_platform.client.decoder_for_schema_encoding",
-        MagicMock(side_effect=Exception("Not found!")),
-    ):
+    with patch("foxglove_data_platform.client.DEFAULT_DECODER_FACTORIES", []):
         client = Client("test")
         client.download_data = MagicMock()
-        client.download_data.return_value = generate_ros1_data()
+        client.download_data.return_value = generate_ros2_data()
         with pytest.raises(Exception):
             client.get_messages(
                 device_id="test_id", start=datetime.now(), end=datetime.now()
             )
 
 
 def test_download_with_decoder():
     client = Client("test")
     client.download_data = MagicMock()
-    client.download_data.return_value = generate_ros1_data()
+    client.download_data.return_value = generate_ros2_data()
     messages = client.get_messages(
         device_id="test_id", start=datetime.now(), end=datetime.now()
     )
     assert len(messages) == 10
+    for i, (_, _, msg) in enumerate(messages):
+        assert msg.data == f"string message {i + 1}"
```

