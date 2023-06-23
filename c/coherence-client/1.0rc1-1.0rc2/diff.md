# Comparing `tmp/coherence_client-1.0rc1.tar.gz` & `tmp/coherence_client-1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherence_client-1.0rc1.tar", max compression
+gzip compressed data, was "coherence_client-1.0rc2.tar", max compression
```

## Comparing `coherence_client-1.0rc1.tar` & `coherence_client-1.0rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1839 2023-06-15 18:35:43.333261 coherence_client-1.0rc1/LICENSE.txt
--rw-r--r--   0        0        0     4548 2023-06-15 18:35:43.434393 coherence_client-1.0rc1/README.md
--rw-r--r--   0        0        0     1979 2023-06-15 18:38:08.997849 coherence_client-1.0rc1/pyproject.toml
--rw-r--r--   0        0        0      986 2023-06-15 18:38:39.397834 coherence_client-1.0rc1/src/coherence/__init__.py
--rw-r--r--   0        0        0    33819 2023-06-15 18:35:44.542780 coherence_client-1.0rc1/src/coherence/aggregator.py
--rw-r--r--   0        0        0    62479 2023-06-15 18:35:44.599870 coherence_client-1.0rc1/src/coherence/client.py
--rw-r--r--   0        0        0     1060 2023-06-15 18:35:44.649334 coherence_client-1.0rc1/src/coherence/comparator.py
--rw-r--r--   0        0        0    31397 2023-06-15 18:35:44.692952 coherence_client-1.0rc1/src/coherence/event.py
--rw-r--r--   0        0        0    11175 2023-06-15 18:35:44.738663 coherence_client-1.0rc1/src/coherence/extractor.py
--rw-r--r--   0        0        0    36712 2023-06-15 18:35:44.782352 coherence_client-1.0rc1/src/coherence/filter.py
--rw-r--r--   0        0        0    11698 2023-06-15 18:35:44.838742 coherence_client-1.0rc1/src/coherence/messages_pb2.py
--rw-r--r--   0        0        0      159 2023-06-15 18:35:44.839539 coherence_client-1.0rc1/src/coherence/messages_pb2_grpc.py
--rw-r--r--   0        0        0    33851 2023-06-15 18:35:44.939903 coherence_client-1.0rc1/src/coherence/processor.py
--rw-r--r--   0        0        0     9917 2023-06-15 18:35:45.083192 coherence_client-1.0rc1/src/coherence/serialization.py
--rw-r--r--   0        0        0     4040 2023-06-15 18:35:45.140812 coherence_client-1.0rc1/src/coherence/services_pb2.py
--rw-r--r--   0        0        0    45397 2023-06-15 18:35:45.142868 coherence_client-1.0rc1/src/coherence/services_pb2_grpc.py
--rw-r--r--   0        0        0    11918 2023-06-15 18:35:45.239824 coherence_client-1.0rc1/src/coherence/util.py
--rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 coherence_client-1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-06-16 15:02:06.453365 coherence_client-1.0rc2/LICENSE.txt
+-rw-r--r--   0        0        0     4548 2023-06-16 15:02:06.455855 coherence_client-1.0rc2/README.md
+-rw-r--r--   0        0        0     1995 2023-06-23 17:54:28.141523 coherence_client-1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      986 2023-06-23 17:54:28.144153 coherence_client-1.0rc2/src/coherence/__init__.py
+-rw-r--r--   0        0        0    33819 2023-06-16 15:02:06.482799 coherence_client-1.0rc2/src/coherence/aggregator.py
+-rw-r--r--   0        0        0    62507 2023-06-21 16:52:55.727619 coherence_client-1.0rc2/src/coherence/client.py
+-rw-r--r--   0        0        0     1060 2023-06-16 15:02:06.484749 coherence_client-1.0rc2/src/coherence/comparator.py
+-rw-r--r--   0        0        0    31397 2023-06-16 15:02:06.485414 coherence_client-1.0rc2/src/coherence/event.py
+-rw-r--r--   0        0        0    11175 2023-06-16 15:02:06.486394 coherence_client-1.0rc2/src/coherence/extractor.py
+-rw-r--r--   0        0        0    36712 2023-06-16 15:02:06.487527 coherence_client-1.0rc2/src/coherence/filter.py
+-rw-r--r--   0        0        0    11698 2023-06-16 15:02:06.489543 coherence_client-1.0rc2/src/coherence/messages_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-16 15:02:06.490115 coherence_client-1.0rc2/src/coherence/messages_pb2_grpc.py
+-rw-r--r--   0        0        0    33851 2023-06-16 15:02:06.491241 coherence_client-1.0rc2/src/coherence/processor.py
+-rw-r--r--   0        0        0     9917 2023-06-16 15:02:06.492224 coherence_client-1.0rc2/src/coherence/serialization.py
+-rw-r--r--   0        0        0     4040 2023-06-16 15:02:06.492853 coherence_client-1.0rc2/src/coherence/services_pb2.py
+-rw-r--r--   0        0        0    45397 2023-06-16 15:02:06.493204 coherence_client-1.0rc2/src/coherence/services_pb2_grpc.py
+-rw-r--r--   0        0        0    11918 2023-06-16 15:02:06.493808 coherence_client-1.0rc2/src/coherence/util.py
+-rw-r--r--   0        0        0     5487 1970-01-01 00:00:00.000000 coherence_client-1.0rc2/PKG-INFO
```

### Comparing `coherence_client-1.0rc1/LICENSE.txt` & `coherence_client-1.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/README.md` & `coherence_client-1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/pyproject.toml` & `coherence_client-1.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # Copyright (c) 2022, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 [tool.poetry]
 name = "coherence-client"
-version = "1.0rc1"
+version = "1.0rc2"
 description = """The Coherence Python Client allows Python applications to act as cache clients to a \
 Coherence Cluster using Google's gRPC framework as the network transport."""
 packages = [
     { include = "coherence", from = "./src"},
 ]
 readme = "README.md"
 authors = ["Oracle <dhiru.pandey@oracle.com>"]
-homepage = "https://github.com/oracle/coherenc-py-client"
-repository = "https://github.com/oracle/coherenc-py-client"
+homepage = "https://github.com/oracle/coherence-py-client"
+repository = "https://github.com/oracle/coherence-py-client"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Universal Permissive License (UPL)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.dependencies]
 python = "~3.11"
 protobuf = "~4.23"
-grpcio = "~1.54"
-grpcio-tools = "~1.54"
+grpcio = ">=1.54,<1.57"
+grpcio-tools = ">=1.54,<1.57"
 jsonpickle = "~3.0"
 pymitter = "~0.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "~7.3"
 pytest-asyncio = "~0.21"
 pytest-cov = "~4.1"
 pytest-unordered = "~0.5"
 pre-commit = "~3.3"
-Sphinx = "~4.5"
+Sphinx = "~6.2"
 sphinx-rtd-theme = "~1.2"
 sphinxcontrib-napoleon = "~0.7"
 m2r = "~0.3"
 third-party-license-file-generator = "~2023.2"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
```

### Comparing `coherence_client-1.0rc1/src/coherence/__init__.py` & `coherence_client-1.0rc2/src/coherence/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) 2022 Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
-__version__ = "1.0rc1"
+__version__ = "1.0rc2"
 
 import logging
 
 # expose these symbols in top-level namespace
 from .aggregator import Aggregators as Aggregators
 from .client import MapEntry as MapEntry
 from .client import NamedCache as NamedCache
```

### Comparing `coherence_client-1.0rc1/src/coherence/aggregator.py` & `coherence_client-1.0rc2/src/coherence/aggregator.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/client.py` & `coherence_client-1.0rc2/src/coherence/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1289,15 +1289,17 @@
             self._emitter.emit(SessionLifecycleEvent.CLOSED.value)
             for task in self._tasks:
                 task.cancel()
             self._tasks.clear()
 
             caches_copy: dict[str, NamedCache[Any, Any]] = self._caches.copy()
             for cache in caches_copy.values():
-                await cache.destroy()
+                cache.release()
+
+            self._caches.clear()
 
             await self._channel.close()  # TODO: consider grace period?
 
     def _setup_event_handlers(self, client: NamedCacheClient[K, V]) -> None:
         this: Session = self
 
         def on_destroyed(name: str) -> None:
```

### Comparing `coherence_client-1.0rc1/src/coherence/comparator.py` & `coherence_client-1.0rc2/src/coherence/comparator.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/event.py` & `coherence_client-1.0rc2/src/coherence/event.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/extractor.py` & `coherence_client-1.0rc2/src/coherence/extractor.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/filter.py` & `coherence_client-1.0rc2/src/coherence/filter.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/messages_pb2.py` & `coherence_client-1.0rc2/src/coherence/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/processor.py` & `coherence_client-1.0rc2/src/coherence/processor.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/serialization.py` & `coherence_client-1.0rc2/src/coherence/serialization.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/services_pb2.py` & `coherence_client-1.0rc2/src/coherence/services_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/services_pb2_grpc.py` & `coherence_client-1.0rc2/src/coherence/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/src/coherence/util.py` & `coherence_client-1.0rc2/src/coherence/util.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.0rc1/PKG-INFO` & `coherence_client-1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: coherence-client
-Version: 1.0rc1
+Version: 1.0rc2
 Summary: The Coherence Python Client allows Python applications to act as cache clients to a Coherence Cluster using Google's gRPC framework as the network transport.
-Home-page: https://github.com/oracle/coherenc-py-client
+Home-page: https://github.com/oracle/coherence-py-client
 Author: Oracle
 Author-email: dhiru.pandey@oracle.com
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grpcio (>=1.54,<1.55)
-Requires-Dist: grpcio-tools (>=1.54,<1.55)
+Requires-Dist: grpcio (>=1.54,<1.57)
+Requires-Dist: grpcio-tools (>=1.54,<1.57)
 Requires-Dist: jsonpickle (>=3.0,<3.1)
 Requires-Dist: protobuf (>=4.23,<4.24)
 Requires-Dist: pymitter (>=0.4,<0.5)
-Project-URL: Repository, https://github.com/oracle/coherenc-py-client
+Project-URL: Repository, https://github.com/oracle/coherence-py-client
 Description-Content-Type: text/markdown
 
 # Coherence Python Client
 
 ![CI/CD](https://github.com/oracle/coherence-py-client/actions/workflows/validate.yml/badge.svg)
 [![License](http://img.shields.io/badge/license-UPL%201.0-blue.svg)](https://oss.oracle.com/licenses/upl/)
```

