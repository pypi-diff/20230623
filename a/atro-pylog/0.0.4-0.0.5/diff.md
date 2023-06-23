# Comparing `tmp/atro-pylog-0.0.4.tar.gz` & `tmp/atro-pylog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pylog-0.0.4.tar", last modified: Fri Jun 23 16:04:13 2023, max compression
+gzip compressed data, was "atro-pylog-0.0.5.tar", last modified: Fri Jun 23 17:03:49 2023, max compression
```

## Comparing `atro-pylog-0.0.4.tar` & `atro-pylog-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.4/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/atro_pylog.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      333 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)       91 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/pylog/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1267 2023-06-21 19:51:58.000000 atro-pylog-0.0.4/pylog/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      857 2023-06-21 19:47:46.000000 atro-pylog-0.0.4/pylog/level.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      835 2023-06-23 16:04:07.000000 atro-pylog-0.0.4/pylog/logger_base.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      371 2023-06-21 19:10:23.000000 atro-pylog-0.0.4/pylog/logger_type.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1020 2023-06-23 15:53:52.000000 atro-pylog-0.0.4/pylog/loguru_logger.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     2200 2023-06-23 15:54:04.000000 atro-pylog-0.0.4/pylog/opentelemetry_logger.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      471 2023-06-21 19:47:46.000000 atro-pylog-0.0.4/pylog/settings.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1118 2023-06-23 15:58:47.000000 atro-pylog-0.0.4/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 17:03:49.222070 atro-pylog-0.0.5/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-23 17:03:49.222070 atro-pylog-0.0.5/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.5/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 17:03:49.222070 atro-pylog-0.0.5/atro_pylog.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-23 17:03:49.000000 atro-pylog-0.0.5/atro_pylog.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      333 2023-06-23 17:03:49.000000 atro-pylog-0.0.5/atro_pylog.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-23 17:03:49.000000 atro-pylog-0.0.5/atro_pylog.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      105 2023-06-23 17:03:49.000000 atro-pylog-0.0.5/atro_pylog.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-23 17:03:49.000000 atro-pylog-0.0.5/atro_pylog.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 17:03:49.222070 atro-pylog-0.0.5/pylog/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1137 2023-06-23 16:59:18.000000 atro-pylog-0.0.5/pylog/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      857 2023-06-21 19:47:46.000000 atro-pylog-0.0.5/pylog/level.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1202 2023-06-23 17:02:45.000000 atro-pylog-0.0.5/pylog/logger_base.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      371 2023-06-21 19:10:23.000000 atro-pylog-0.0.5/pylog/logger_type.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1107 2023-06-23 16:59:59.000000 atro-pylog-0.0.5/pylog/loguru_logger.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     2285 2023-06-23 17:00:11.000000 atro-pylog-0.0.5/pylog/opentelemetry_logger.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      800 2023-06-23 16:54:23.000000 atro-pylog-0.0.5/pylog/settings.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-23 17:03:49.222070 atro-pylog-0.0.5/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1142 2023-06-23 17:02:29.000000 atro-pylog-0.0.5/setup.py
```

### Comparing `atro-pylog-0.0.4/PKG-INFO` & `atro-pylog-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.4/atro_pylog.egg-info/PKG-INFO` & `atro-pylog-0.0.5/atro_pylog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.4/pylog/level.py` & `atro-pylog-0.0.5/pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.0.4/pylog/loguru_logger.py` & `atro-pylog-0.0.5/pylog/loguru_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from loguru import logger as loguru_logger
+from pylog.settings import BaseLoggerSettings
 
 from pylog.level import level_to_str
 from pylog.logger_base import Logger
 from pylog.settings import LoguruLoggerSettings
 
 
 class LoguruLogger(Logger):
-    def __init__(self, settings: LoguruLoggerSettings | None = None):
-        super().__init__()
+    def __init__(self, base_settings: BaseLoggerSettings | None = None, settings: LoguruLoggerSettings | None = None):
         self.settings = settings or LoguruLoggerSettings()
         self.logger = loguru_logger
-        self.logger.level("DEBUG")
+        super().__init__(base_settings=base_settings)
 
     def debug(self, message: str) -> None:
         self.logger.debug(message)
 
     def info(self, message: str) -> None:
         self.logger.info(message)
```

### Comparing `atro-pylog-0.0.4/pylog/opentelemetry_logger.py` & `atro-pylog-0.0.5/pylog/opentelemetry_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from opentelemetry import trace
 from opentelemetry._logs import set_logger_provider
 from opentelemetry.exporter.otlp.proto.grpc._log_exporter import OTLPLogExporter
 from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
+from pydantic import BaseSettings
 
 from pylog.level import str_to_level
 from pylog.logger_base import Logger
-from pylog.settings import OpenTelemetryLoggerSettings
+from pylog.settings import BaseLoggerSettings, OpenTelemetryLoggerSettings
 
 
 class OpenTelemetryLogger(Logger):
-    def __init__(self, settings: OpenTelemetryLoggerSettings | None = None):
-        super().__init__()
+    def __init__(self, base_settings:BaseLoggerSettings | None = None ,settings: OpenTelemetryLoggerSettings | None = None):
         self.settings = settings or OpenTelemetryLoggerSettings()
         trace.set_tracer_provider(TracerProvider())
         self.logger_provider = LoggerProvider(
             resource=Resource.create(
                 {
                     "service.name": self.settings.service_name or "",
                     "service.instance.id": self.settings.instance_id or "",
@@ -31,15 +31,15 @@
         self.exporter = OTLPLogExporter(insecure=True, endpoint=self.settings.endpoint)
         self.logger_provider.add_log_record_processor(BatchLogRecordProcessor(self.exporter))
         self.handler = LoggingHandler(level=logging.NOTSET, logger_provider=self.logger_provider)
 
         # Attach OTLP handler to root logger
         logging.getLogger().addHandler(self.handler)
         self.logger = logging.getLogger(__name__)
-        self.logger.setLevel(logging.DEBUG)
+        super().__init__(base_settings=base_settings)
 
     def debug(self, message: str):
         self.logger.debug(message)
 
     def info(self, message: str):
         self.logger.info(message)
```

### Comparing `atro-pylog-0.0.4/setup.py` & `atro-pylog-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pylog",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
     install_requires=[
         "loguru",
         "opentelemetry-api",
         "opentelemetry-exporter-otlp-proto-grpc",
         "opentelemetry-sdk",
         "pydantic",
+        "python-dotenv"
     ],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

