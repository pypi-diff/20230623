# Comparing `tmp/tb-mqtt-client-1.4.1.tar.gz` & `tmp/tb-mqtt-client-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb-mqtt-client-1.4.1.tar", last modified: Thu Oct 27 14:14:59 2022, max compression
+gzip compressed data, was "tb-mqtt-client-1.5.tar", last modified: Fri Jun 23 09:47:37 2023, max compression
```

## Comparing `tb-mqtt-client-1.4.1.tar` & `tb-mqtt-client-1.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 z         (1000) z         (1000)        0 2022-10-27 14:14:59.193567 tb-mqtt-client-1.4.1/
--rw-rw-r--   0 z         (1000) z         (1000)      549 2022-05-26 11:36:23.000000 tb-mqtt-client-1.4.1/LICENSE
--rw-rw-r--   0 z         (1000) z         (1000)    10317 2022-10-27 14:14:59.193567 tb-mqtt-client-1.4.1/PKG-INFO
--rw-rw-r--   0 z         (1000) z         (1000)     9829 2022-05-26 11:36:23.000000 tb-mqtt-client-1.4.1/README.md
--rw-rw-r--   0 z         (1000) z         (1000)      669 2022-05-26 11:36:23.000000 tb-mqtt-client-1.4.1/__init__.py
--rw-rw-r--   0 z         (1000) z         (1000)     2482 2022-05-26 11:36:23.000000 tb-mqtt-client-1.4.1/sdk_utils.py
--rw-rw-r--   0 z         (1000) z         (1000)       38 2022-10-27 14:14:59.193567 tb-mqtt-client-1.4.1/setup.cfg
--rw-rw-r--   0 z         (1000) z         (1000)     1487 2022-10-27 14:11:45.000000 tb-mqtt-client-1.4.1/setup.py
--rw-rw-r--   0 z         (1000) z         (1000)    18056 2022-05-26 11:36:23.000000 tb-mqtt-client-1.4.1/tb_device_http.py
--rw-rw-r--   0 z         (1000) z         (1000)    26488 2022-09-07 12:21:02.000000 tb-mqtt-client-1.4.1/tb_device_mqtt.py
--rw-rw-r--   0 z         (1000) z         (1000)    10508 2022-09-07 12:21:02.000000 tb-mqtt-client-1.4.1/tb_gateway_mqtt.py
-drwxrwxr-x   0 z         (1000) z         (1000)        0 2022-10-27 14:14:59.193567 tb-mqtt-client-1.4.1/tb_mqtt_client.egg-info/
--rw-rw-r--   0 z         (1000) z         (1000)    10317 2022-10-27 14:14:59.000000 tb-mqtt-client-1.4.1/tb_mqtt_client.egg-info/PKG-INFO
--rw-rw-r--   0 z         (1000) z         (1000)      295 2022-10-27 14:14:59.000000 tb-mqtt-client-1.4.1/tb_mqtt_client.egg-info/SOURCES.txt
--rw-rw-r--   0 z         (1000) z         (1000)        1 2022-10-27 14:14:59.000000 tb-mqtt-client-1.4.1/tb_mqtt_client.egg-info/dependency_links.txt
--rw-rw-r--   0 z         (1000) z         (1000)       40 2022-10-27 14:14:59.000000 tb-mqtt-client-1.4.1/tb_mqtt_client.egg-info/requires.txt
--rw-rw-r--   0 z         (1000) z         (1000)        1 2022-10-27 14:14:59.000000 tb-mqtt-client-1.4.1/tb_mqtt_client.egg-info/top_level.txt
+drwxrwxr-x   0 imbeacon  (1001) imbeacon  (1002)        0 2023-06-23 09:47:37.754094 tb-mqtt-client-1.5/
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)      549 2023-06-23 09:35:41.000000 tb-mqtt-client-1.5/LICENSE
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)    10266 2023-06-23 09:47:37.754094 tb-mqtt-client-1.5/PKG-INFO
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)     9802 2023-06-23 09:35:06.000000 tb-mqtt-client-1.5/README.md
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)      608 2023-06-23 09:42:47.000000 tb-mqtt-client-1.5/__init__.py
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)     3291 2023-06-23 09:43:49.000000 tb-mqtt-client-1.5/sdk_utils.py
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)       38 2023-06-23 09:47:37.754094 tb-mqtt-client-1.5/setup.cfg
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)     1436 2023-06-23 09:42:47.000000 tb-mqtt-client-1.5/setup.py
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)    18630 2023-06-23 09:43:49.000000 tb-mqtt-client-1.5/tb_device_http.py
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)    26407 2023-06-23 09:42:47.000000 tb-mqtt-client-1.5/tb_device_mqtt.py
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)    10447 2023-06-23 09:42:47.000000 tb-mqtt-client-1.5/tb_gateway_mqtt.py
+drwxrwxr-x   0 imbeacon  (1001) imbeacon  (1002)        0 2023-06-23 09:47:37.754094 tb-mqtt-client-1.5/tb_mqtt_client.egg-info/
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)    10266 2023-06-23 09:47:37.000000 tb-mqtt-client-1.5/tb_mqtt_client.egg-info/PKG-INFO
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)      304 2023-06-23 09:47:37.000000 tb-mqtt-client-1.5/tb_mqtt_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)        1 2023-06-23 09:47:37.000000 tb-mqtt-client-1.5/tb_mqtt_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)       55 2023-06-23 09:47:37.000000 tb-mqtt-client-1.5/tb_mqtt_client.egg-info/requires.txt
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)        1 2023-06-23 09:47:37.000000 tb-mqtt-client-1.5/tb_mqtt_client.egg-info/top_level.txt
+-rw-rw-r--   0 imbeacon  (1001) imbeacon  (1002)     1704 2023-06-23 09:43:49.000000 tb-mqtt-client-1.5/utils.py
```

### Comparing `tb-mqtt-client-1.4.1/LICENSE` & `tb-mqtt-client-1.5/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-Copyright 2020. ThingsBoard
+# Copyright 2023. ThingsBoard
+# 
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+# 
+#  http://www.apache.org/licenses/LICENSE-2.0
+# 
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
 
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
 
-http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+__name__ = "tb_mqtt_client"
```

### Comparing `tb-mqtt-client-1.4.1/PKG-INFO` & `tb-mqtt-client-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: tb-mqtt-client
-Version: 1.4.1
+Version: 1.5
 Summary: ThingsBoard python client SDK
 Home-page: https://github.com/thingsboard/thingsboard-python-client-sdk
+Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.5.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
-Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.4.1.tar.gz
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ThingsBoard MQTT and HTTP client Python SDK
 [![Join the chat at https://gitter.im/thingsboard/chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/thingsboard/chat?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 <a href="https://thingsboard.io"><img src="./logo.png?raw=true" width="100" height="100"></a>
 
 ThingsBoard is an open-source IoT platform for data collection, processing, visualization, and device management.
-This project ia a Python library that provides convenient client SDK for both Device and [Gateway](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs.
+This project is a Python library that provides convenient client SDK for both Device and [Gateway](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs.
 
 SDK supports:
 - Unencrypted and encrypted (TLS v1.2) connection
 - QoS 0 and 1 (MQTT only)
 - Automatic reconnect
 - All [Device MQTT](https://thingsboard.io/docs/reference/mqtt-api/) APIs provided by ThingsBoard
 - All [Gateway MQTT](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs provided by ThingsBoard
 - Most [Device HTTP](https://thingsboard.io/docs/reference/http-api/) APIs provided by ThingsBoard
-  - Device Claiming and Firmware updates are not supported yet.
+- Device Claiming
+- Firmware updates
 
 The [Device MQTT](https://thingsboard.io/docs/reference/mqtt-api/) API and the [Gateway MQTT](https://thingsboard.io/docs/reference/gateway-mqtt-api/) API are base on the Paho MQTT library. The [Device HTTP](https://thingsboard.io/docs/reference/http-api/) API is based on the Requests library.
 
 ## Installation
 
 To install using pip:
 
@@ -290,9 +290,7 @@
  - [Community chat](https://gitter.im/thingsboard/chat)
  - [Q&A forum](https://groups.google.com/forum/#!forum/thingsboard)
  - [Stackoverflow](http://stackoverflow.com/questions/tagged/thingsboard)
 
 ## Licenses
 
 This project is released under [Apache 2.0 License](./LICENSE).
-
-
```

### Comparing `tb-mqtt-client-1.4.1/README.md` & `tb-mqtt-client-1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # ThingsBoard MQTT and HTTP client Python SDK
 [![Join the chat at https://gitter.im/thingsboard/chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/thingsboard/chat?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 <a href="https://thingsboard.io"><img src="./logo.png?raw=true" width="100" height="100"></a>
 
 ThingsBoard is an open-source IoT platform for data collection, processing, visualization, and device management.
-This project ia a Python library that provides convenient client SDK for both Device and [Gateway](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs.
+This project is a Python library that provides convenient client SDK for both Device and [Gateway](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs.
 
 SDK supports:
 - Unencrypted and encrypted (TLS v1.2) connection
 - QoS 0 and 1 (MQTT only)
 - Automatic reconnect
 - All [Device MQTT](https://thingsboard.io/docs/reference/mqtt-api/) APIs provided by ThingsBoard
 - All [Gateway MQTT](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs provided by ThingsBoard
 - Most [Device HTTP](https://thingsboard.io/docs/reference/http-api/) APIs provided by ThingsBoard
-  - Device Claiming and Firmware updates are not supported yet.
+- Device Claiming
+- Firmware updates
 
 The [Device MQTT](https://thingsboard.io/docs/reference/mqtt-api/) API and the [Gateway MQTT](https://thingsboard.io/docs/reference/gateway-mqtt-api/) API are base on the Paho MQTT library. The [Device HTTP](https://thingsboard.io/docs/reference/http-api/) API is based on the Requests library.
 
 ## Installation
 
 To install using pip:
```

### Comparing `tb-mqtt-client-1.4.1/__init__.py` & `tb-mqtt-client-1.5/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-#      Copyright 2020. ThingsBoard
-#  #
-#      Licensed under the Apache License, Version 2.0 (the "License");
-#      you may not use this file except in compliance with the License.
-#      You may obtain a copy of the License at
-#  #
-#          http://www.apache.org/licenses/LICENSE-2.0
-#  #
-#      Unless required by applicable law or agreed to in writing, software
-#      distributed under the License is distributed on an "AS IS" BASIS,
-#      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#      See the License for the specific language governing permissions and
-#      limitations under the License.
-#
-#
+Copyright 2023. ThingsBoard
 
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
 
-__name__ = "tb_mqtt_client"
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `tb-mqtt-client-1.4.1/setup.py` & `tb-mqtt-client-1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-#      Copyright 2020. ThingsBoard
-#  #
-#      Licensed under the Apache License, Version 2.0 (the "License");
-#      you may not use this file except in compliance with the License.
-#      You may obtain a copy of the License at
-#  #
-#          http://www.apache.org/licenses/LICENSE-2.0
-#  #
-#      Unless required by applicable law or agreed to in writing, software
-#      distributed under the License is distributed on an "AS IS" BASIS,
-#      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#      See the License for the specific language governing permissions and
-#      limitations under the License.
-#
+# Copyright 2023. ThingsBoard
+# 
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+# 
+#  http://www.apache.org/licenses/LICENSE-2.0
+# 
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 #
 
 from os import path
 from setuptools import setup
 
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
-VERSION = "1.4.1"
+VERSION = "1.5"
 
 setup(
     version=VERSION,
     name="tb-mqtt-client",
     author="ThingsBoard",
     author_email="info@thingsboard.io",
     license="Apache Software License (Apache Software License 2.0)",
     description="ThingsBoard python client SDK",
     url="https://github.com/thingsboard/thingsboard-python-client-sdk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.7",
     packages=["."],
-    install_requires=['paho-mqtt>=1.6', 'requests', 'mmh3', 'simplejson'],
+    install_requires=['tb-paho-mqtt-client>=1.6.3', 'requests>=2.31.0', 'simplejson'],
     download_url='https://github.com/thingsboard/thingsboard-python-client-sdk/archive/%s.tar.gz' % VERSION)
```

### Comparing `tb-mqtt-client-1.4.1/tb_device_http.py` & `tb-mqtt-client-1.5/tb_device_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023. ThingsBoard
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#  http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 """ThingsBoard HTTP API device module."""
 import threading
 import logging
 import queue
 import time
 import typing
 from datetime import datetime, timezone
```

### Comparing `tb-mqtt-client-1.4.1/tb_device_mqtt.py` & `tb-mqtt-client-1.5/tb_device_mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#      Copyright 2020. ThingsBoard
-#  #
-#      Licensed under the Apache License, Version 2.0 (the "License");
-#      you may not use this file except in compliance with the License.
-#      You may obtain a copy of the License at
-#  #
-#          http://www.apache.org/licenses/LICENSE-2.0
-#  #
-#      Unless required by applicable law or agreed to in writing, software
-#      distributed under the License is distributed on an "AS IS" BASIS,
-#      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#      See the License for the specific language governing permissions and
-#      limitations under the License.
-#
+# Copyright 2023. ThingsBoard
+# 
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+# 
+#  http://www.apache.org/licenses/LICENSE-2.0
+# 
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import paho.mqtt.client as paho
 from math import ceil
 import logging
 import time
 import queue
 from json import loads, dumps
@@ -90,15 +89,15 @@
 
     def __on_message(self, _, __, msg):
         decoded_payload = msg.payload.decode("UTF-8")
         log.info("[Provisioning client] Received data from ThingsBoard: %s" % decoded_payload)
         decoded_message = loads(decoded_payload)
         provision_device_status = decoded_message.get("status")
         if provision_device_status == "SUCCESS":
-            self.__credentials = decoded_message["credentialsValue"]
+            self.__credentials = decoded_message
         else:
             log.error("[Provisioning client] Provisioning was unsuccessful with status %s and message: %s" % (
                 provision_device_status, decoded_message["errorMsg"]))
         self.disconnect()
 
     def provision(self):
         log.info("[Provisioning client] Connecting to ThingsBoard")
```

### Comparing `tb-mqtt-client-1.4.1/tb_gateway_mqtt.py` & `tb-mqtt-client-1.5/tb_gateway_mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#      Copyright 2020. ThingsBoard
-#  #
-#      Licensed under the Apache License, Version 2.0 (the "License");
-#      you may not use this file except in compliance with the License.
-#      You may obtain a copy of the License at
-#  #
-#          http://www.apache.org/licenses/LICENSE-2.0
-#  #
-#      Unless required by applicable law or agreed to in writing, software
-#      distributed under the License is distributed on an "AS IS" BASIS,
-#      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#      See the License for the specific language governing permissions and
-#      limitations under the License.
-#
+# Copyright 2023. ThingsBoard
+# 
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+# 
+#  http://www.apache.org/licenses/LICENSE-2.0
+# 
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 #
 
 import logging
 import time
 from simplejson import dumps
 from tb_device_mqtt import TBDeviceMqttClient
```

### Comparing `tb-mqtt-client-1.4.1/tb_mqtt_client.egg-info/PKG-INFO` & `tb-mqtt-client-1.5/tb_mqtt_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: tb-mqtt-client
-Version: 1.4.1
+Version: 1.5
 Summary: ThingsBoard python client SDK
 Home-page: https://github.com/thingsboard/thingsboard-python-client-sdk
+Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.5.tar.gz
 Author: ThingsBoard
 Author-email: info@thingsboard.io
 License: Apache Software License (Apache Software License 2.0)
-Download-URL: https://github.com/thingsboard/thingsboard-python-client-sdk/archive/1.4.1.tar.gz
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ThingsBoard MQTT and HTTP client Python SDK
 [![Join the chat at https://gitter.im/thingsboard/chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/thingsboard/chat?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 <a href="https://thingsboard.io"><img src="./logo.png?raw=true" width="100" height="100"></a>
 
 ThingsBoard is an open-source IoT platform for data collection, processing, visualization, and device management.
-This project ia a Python library that provides convenient client SDK for both Device and [Gateway](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs.
+This project is a Python library that provides convenient client SDK for both Device and [Gateway](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs.
 
 SDK supports:
 - Unencrypted and encrypted (TLS v1.2) connection
 - QoS 0 and 1 (MQTT only)
 - Automatic reconnect
 - All [Device MQTT](https://thingsboard.io/docs/reference/mqtt-api/) APIs provided by ThingsBoard
 - All [Gateway MQTT](https://thingsboard.io/docs/reference/gateway-mqtt-api/) APIs provided by ThingsBoard
 - Most [Device HTTP](https://thingsboard.io/docs/reference/http-api/) APIs provided by ThingsBoard
-  - Device Claiming and Firmware updates are not supported yet.
+- Device Claiming
+- Firmware updates
 
 The [Device MQTT](https://thingsboard.io/docs/reference/mqtt-api/) API and the [Gateway MQTT](https://thingsboard.io/docs/reference/gateway-mqtt-api/) API are base on the Paho MQTT library. The [Device HTTP](https://thingsboard.io/docs/reference/http-api/) API is based on the Requests library.
 
 ## Installation
 
 To install using pip:
 
@@ -290,9 +290,7 @@
  - [Community chat](https://gitter.im/thingsboard/chat)
  - [Q&A forum](https://groups.google.com/forum/#!forum/thingsboard)
  - [Stackoverflow](http://stackoverflow.com/questions/tagged/thingsboard)
 
 ## Licenses
 
 This project is released under [Apache 2.0 License](./LICENSE).
-
-
```

