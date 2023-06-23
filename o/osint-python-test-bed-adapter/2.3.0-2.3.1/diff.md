# Comparing `tmp/osint-python-test-bed-adapter-2.3.0.tar.gz` & `tmp/osint-python-test-bed-adapter-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-test-bed-adapter-2.3.0.tar", last modified: Sat Jun 17 00:33:05 2023, max compression
+gzip compressed data, was "osint-python-test-bed-adapter-2.3.1.tar", last modified: Fri Jun 23 00:54:39 2023, max compression
```

## Comparing `osint-python-test-bed-adapter-2.3.0.tar` & `osint-python-test-bed-adapter-2.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.0/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3165 2023-06-13 08:56:50.000000 osint-python-test-bed-adapter-2.3.0/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      703 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-16 22:11:18.000000 osint-python-test-bed-adapter-2.3.0/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1389 2023-06-17 00:32:44.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3796 2023-06-17 00:23:16.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/consumer_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1699 2023-06-16 22:08:43.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/heartbeat_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2883 2023-06-16 22:08:43.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/log_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2102 2023-06-17 00:23:16.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/producer_manager.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/test_bed_options.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/helpers.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.1/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3165 2023-06-13 08:56:50.000000 osint-python-test-bed-adapter-2.3.1/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      703 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-23 00:50:22.000000 osint-python-test-bed-adapter-2.3.1/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1389 2023-06-17 00:32:44.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3897 2023-06-23 00:52:25.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/consumer_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1699 2023-06-16 22:08:43.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/heartbeat_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3074 2023-06-23 00:54:19.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/log_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2102 2023-06-17 00:23:16.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/producer_manager.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/test_bed_options.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/helpers.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.3.0/LICENSE` & `osint-python-test-bed-adapter-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/PKG-INFO` & `osint-python-test-bed-adapter-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.3.0/README.md` & `osint-python-test-bed-adapter-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/PKG-INFO` & `osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/SOURCES.txt` & `osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/setup.py` & `osint-python-test-bed-adapter-2.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osint-python-test-bed-adapter",
-    version="2.3.0",
+    version="2.3.1",
     author="TimovdK",
     author_email="timo_kuil@hotmail.com",
     description="Python adapter for Kafka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-adapter",
     include_package_data=True,
     install_requires=[
-        'confluent_kafka>=1.9.0',
+        'confluent_kafka>=2.1.1',
         'fastavro>=1.6.0'
     ],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/__init__.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/consumer_manager.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/consumer_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 from ..options.test_bed_options import TestBedOptions
 
 
 class ConsumerManager(Thread):
     def __init__(self, options: TestBedOptions, kafka_topic, handle_message):
         super().__init__()
         self.logger = logging.getLogger(__name__)
+        self.running = True
         self.daemon = True
         self.options = options
         self.handle_message = handle_message
-        self.running = True
-
         self.latest_message = None
 
         sr_conf = {'url': self.options.schema_registry}
         schema_registry_client = SchemaRegistryClient(sr_conf)
 
         self.avro_deserializer = AvroDeserializer(schema_registry_client)
         self.schema = schema_registry_client.get_latest_version(kafka_topic + "-value")
@@ -43,14 +42,16 @@
     def run(self):
         self.reset_partition_offsets()
         self.ingore_messages()
         self.use_latest_message()
         self.listen()
 
     def stop(self):
+        """Stop the consumer"""
+        self.logger.info(f"Stopping consumer for {self.kafka_topic}")
         self.running = False
 
     def reset_partition_offsets(self):
         """Reset partition offsets to beginning"""
         if self.options.offset_type != 'earliest':
             return
         try:
```

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/heartbeat_manager.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/log_manager.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/log_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,18 @@
         self.log(LogLevel.Error, msg)
 
     def critical(self, msg):
         self.log(LogLevel.Critical, msg)
 
     def log(self, level: LogLevel, msg):
         if not isinstance(msg, str):
-            msg = json.dumps(msg)
+            try:
+                msg = json.dumps(msg)
+            except:
+                msg = str(msg)
 
         # Send to console
         if level == LogLevel.Sill:
             print(f'{BColors.OKBLUE}{timestamp()}: Silly: {msg}{BColors.ENDC}')
         elif level == LogLevel.Debug:
             print(f'{BColors.OKBLUE}{timestamp()}: Debug: {msg}{BColors.ENDC}')
         elif level == LogLevel.Info:
@@ -95,8 +98,11 @@
             payload = {
                 "id": self.options.consumer_group,
                 "level": LogLevelToType(level),
                 "dateTimeSent": current_milli_time(),
                 "log": msg
             }
             message = [payload]
-            self.kafka_log_producer.send_messages(message)
+            try:
+                self.kafka_log_producer.send_messages(message)
+            except Exception as e:
+                print(f'Failed to send message to kafka: {e}')
```

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/producer_manager.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/producer_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/test_bed_options.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/test_bed_options.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/helpers.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/key.py` & `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/key.py`

 * *Files identical despite different names*

