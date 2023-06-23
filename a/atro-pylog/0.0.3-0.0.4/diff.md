# Comparing `tmp/atro-pylog-0.0.3.tar.gz` & `tmp/atro-pylog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pylog-0.0.3.tar", last modified: Wed Jun 21 19:47:17 2023, max compression
+gzip compressed data, was "atro-pylog-0.0.4.tar", last modified: Fri Jun 23 16:04:13 2023, max compression
```

## Comparing `atro-pylog-0.0.3.tar` & `atro-pylog-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.3/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/atro_pylog.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      333 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)       91 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-21 19:47:17.000000 atro-pylog-0.0.3/atro_pylog.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/pylog/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1225 2023-06-21 19:43:16.000000 atro-pylog-0.0.3/pylog/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      855 2023-06-21 19:15:38.000000 atro-pylog-0.0.3/pylog/level.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      968 2023-06-21 19:45:29.000000 atro-pylog-0.0.3/pylog/logger_base.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      371 2023-06-21 19:10:23.000000 atro-pylog-0.0.3/pylog/logger_type.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      992 2023-06-21 19:43:59.000000 atro-pylog-0.0.3/pylog/loguru_logger.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     2175 2023-06-21 19:32:22.000000 atro-pylog-0.0.3/pylog/opentelemetry_logger.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      492 2023-06-21 19:31:58.000000 atro-pylog-0.0.3/pylog/settings.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-21 19:47:17.772482 atro-pylog-0.0.3/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1118 2023-06-21 19:47:00.000000 atro-pylog-0.0.3/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.4/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/atro_pylog.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      333 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       91 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-23 16:04:13.000000 atro-pylog-0.0.4/atro_pylog.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/pylog/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1267 2023-06-21 19:51:58.000000 atro-pylog-0.0.4/pylog/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      857 2023-06-21 19:47:46.000000 atro-pylog-0.0.4/pylog/level.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      835 2023-06-23 16:04:07.000000 atro-pylog-0.0.4/pylog/logger_base.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      371 2023-06-21 19:10:23.000000 atro-pylog-0.0.4/pylog/logger_type.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1020 2023-06-23 15:53:52.000000 atro-pylog-0.0.4/pylog/loguru_logger.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     2200 2023-06-23 15:54:04.000000 atro-pylog-0.0.4/pylog/opentelemetry_logger.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      471 2023-06-21 19:47:46.000000 atro-pylog-0.0.4/pylog/settings.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-23 16:04:13.562668 atro-pylog-0.0.4/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1118 2023-06-23 15:58:47.000000 atro-pylog-0.0.4/setup.py
```

### Comparing `atro-pylog-0.0.3/PKG-INFO` & `atro-pylog-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.3/atro_pylog.egg-info/PKG-INFO` & `atro-pylog-0.0.4/atro_pylog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.3/pylog/__init__.py` & `atro-pylog-0.0.4/pylog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
+import logging
 import os
-import logging 
+
+from pylog.level import str_to_level
 from pylog.logger_base import Logger
 from pylog.logger_type import LoggerType, str_to_logger_type
 from pylog.loguru_logger import LoguruLogger
 from pylog.opentelemetry_logger import OpenTelemetryLogger
-from pylog.level import str_to_level
-from pylog.settings import OpenTelemetryLoggerSettings, LoguruLoggerSettings
+from pylog.settings import LoguruLoggerSettings, OpenTelemetryLoggerSettings
 
 
 def get_logger(type: LoggerType | str | None = None, level: str | int = logging.DEBUG, open_telemetry_settings: OpenTelemetryLoggerSettings | None = None, loguru_settings: LoguruLoggerSettings | None = None) -> Logger:
     if type is None:
         type = os.getenv("ATRO_PYLOG_TYPE", default=LoggerType.LOGURU)
     if isinstance(type, str):
         type = str_to_logger_type(type)
 
     if level is None:
         level = os.getenv("ATRO_PYLOG_LEVEL", default=logging.DEBUG)
     elif isinstance(level, str):
         level = str_to_level(level)
-        
 
     match type:
         case LoggerType.LOGURU:
-            logger =  LoguruLogger(loguru_settings)
+            logger = LoguruLogger(loguru_settings)  # type: ignore[assignment]
         case LoggerType.OPENTELEMETRY:
-            logger = OpenTelemetryLogger(open_telemetry_settings)
+            logger = OpenTelemetryLogger(open_telemetry_settings)  # type: ignore[assignment]
         case _:
             raise Exception(f"Unknown logger type: {type}")
 
     logger.level(level)
-    
+
     return logger
```

### Comparing `atro-pylog-0.0.3/pylog/level.py` & `atro-pylog-0.0.4/pylog/level.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,21 +12,22 @@
         case "error":
             return logging.ERROR
         case "critical":
             return logging.CRITICAL
         case _:
             raise Exception(f"Unknown logger level: {level}")
 
+
 def level_to_str(level: int) -> str:
     match level:
         case logging.DEBUG:
             return "DEBUG"
         case logging.INFO:
             return "INFO"
         case logging.WARNING:
             return "WARNING"
         case logging.ERROR:
             return "ERROR"
         case logging.CRITICAL:
             return "CRITICAL"
         case _:
-            raise Exception(f"Unknown logger level: {level}")
+            raise Exception(f"Unknown logger level: {level}")
```

### Comparing `atro-pylog-0.0.3/pylog/loguru_logger.py` & `atro-pylog-0.0.4/pylog/loguru_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from loguru import logger as loguru_logger
 
-from pylog.logger_base import Logger
 from pylog.level import level_to_str
+from pylog.logger_base import Logger
 from pylog.settings import LoguruLoggerSettings
 
+
 class LoguruLogger(Logger):
     def __init__(self, settings: LoguruLoggerSettings | None = None):
+        super().__init__()
         self.settings = settings or LoguruLoggerSettings()
         self.logger = loguru_logger
         self.logger.level("DEBUG")
 
     def debug(self, message: str) -> None:
         self.logger.debug(message)
```

### Comparing `atro-pylog-0.0.3/pylog/opentelemetry_logger.py` & `atro-pylog-0.0.4/pylog/opentelemetry_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pylog.level import str_to_level
 from pylog.logger_base import Logger
 from pylog.settings import OpenTelemetryLoggerSettings
 
 
 class OpenTelemetryLogger(Logger):
     def __init__(self, settings: OpenTelemetryLoggerSettings | None = None):
+        super().__init__()
         self.settings = settings or OpenTelemetryLoggerSettings()
         trace.set_tracer_provider(TracerProvider())
         self.logger_provider = LoggerProvider(
             resource=Resource.create(
                 {
                     "service.name": self.settings.service_name or "",
                     "service.instance.id": self.settings.instance_id or "",
@@ -54,9 +55,7 @@
     def shutdown(self):
         self.logger_provider.shutdown()
 
     def level(self, level: str | int):
         if isinstance(level, str):
             level = str_to_level(level)
         self.logger.setLevel(level)
-
-
```

### Comparing `atro-pylog-0.0.3/setup.py` & `atro-pylog-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pylog",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
```

