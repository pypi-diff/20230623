# Comparing `tmp/mercury-sync-0.2.2.tar.gz` & `tmp/mercury-sync-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.2.2.tar", last modified: Sat Jun 17 18:58:16 2023, max compression
+gzip compressed data, was "mercury-sync-0.3.0.tar", last modified: Fri Jun 23 15:18:59 2023, max compression
```

## Comparing `mercury-sync-0.2.2.tar` & `mercury-sync-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.149856 mercury-sync-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:58:16.149856 mercury-sync-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.149856 mercury-sync-0.2.2/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.149856 mercury-sync-0.2.2/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.149856 mercury-sync-0.2.2/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:58:16.145856 mercury-sync-0.2.2/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:58:16.000000 mercury-sync-0.2.2/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 18:58:16.000000 mercury-sync-0.2.2/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:58:16.000000 mercury-sync-0.2.2/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:58:16.000000 mercury-sync-0.2.2/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 18:58:16.000000 mercury-sync-0.2.2/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:58:16.149856 mercury-sync-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 18:58:12.000000 mercury-sync-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.392506 mercury-sync-0.3.0/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/models/ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/mercury_sync/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/types/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/mercury_sync/types/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:59.396507 mercury-sync-0.3.0/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 15:18:59.000000 mercury-sync-0.3.0/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:18:59.400507 mercury-sync-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-23 15:18:51.000000 mercury-sync-0.3.0/setup.py
```

### Comparing `mercury-sync-0.2.2/LICENSE` & `mercury-sync-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/PKG-INFO` & `mercury-sync-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.2.2
+Version: 0.3.0
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.2.2/README.md` & `mercury-sync-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.3.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import asyncio
+import errno
 import pickle
 import socket
 import ssl
 import zstandard
 from collections import deque, defaultdict
 from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
@@ -43,83 +44,161 @@
         self.port = port
 
         self.events: Dict[
             str,
             Coroutine
         ] = {}
 
-        self._client_transports: Dict[str, asyncio.Transport] = {}
-        self._server: asyncio.Server = None
-        self._loop = asyncio.get_event_loop()
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
         self.parsers: Dict[str, Message] = {}
+        self.connected = False
+        self._running = False
+
+        self._client_transports: Dict[str, asyncio.Transport] = {}
+        self._server: asyncio.Server = None
+        self._loop: Union[asyncio.AbstractEventLoop, None] = None
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
         self._pending_responses: Deque[asyncio.Task]= deque()
         self._last_call: Deque[str] = deque()
 
         self._sent_values = deque()
-        self.connected = False
         self._server_socket = None
         self._stream = False
         
         self._client_key_path: Union[str, None] = None
         self._client_cert_path: Union[str, None] = None
 
         self._server_key_path: Union[str, None] = None
         self._server_cert_path: Union[str, None] = None 
         
         self._client_ssl_context: Union[ssl.SSLContext, None] = None
         self._server_ssl_context: Union[ssl.SSLContext, None] = None
         
         self._encryptor = AESGCMFernet(env)
-        self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
-        self._compressor = zstandard.ZstdCompressor()
-
-        self._decompressor = zstandard.ZstdDecompressor()
-        self._running = False
+        self._semaphore: Union[asyncio.Semaphore, None] = None
+        self._compressor: Union[zstandard.ZstdCompressor, None] = None
+        self._decompressor: Union[zstandard.ZstdDecompressor, None] = None
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
+        self._max_concurrency = env.MERCURY_SYNC_MAX_CONCURRENCY
 
     def connect(
         self,
         cert_path: Optional[str]=None,
-        key_path: Optional[str]=None
+        key_path: Optional[str]=None,
+        worker_socket: Optional[socket.socket]=None
     ):
 
+        try:
+
+            self._loop = asyncio.get_event_loop()
+
+        except Exception:
+            self._loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(self._loop)
+            
         self._running = True
+        self._semaphore = asyncio.Semaphore(self._max_concurrency)
+
+        self._compressor = zstandard.ZstdCompressor()
+        self._decompressor = zstandard.ZstdDecompressor()
 
         if cert_path and key_path:
             self._server_ssl_context = self._create_server_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
-        if self.connected is False:
-
+        if self.connected is False and worker_socket is None:
             self._server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             self._server_socket.bind((self.host, self.port))
 
             self._server_socket.setblocking(False)
 
+        elif self.connected is False:
+            self._server_socket = worker_socket
+            host, port = worker_socket.getsockname()
+            self.host = host
+            self.port = port
+
+        if self.connected is False:
+
             server = self._loop.create_server(
                 lambda: MercurySyncTCPServerProtocol(
                     self.read
                 ),
                 sock=self._server_socket,
                 ssl=self._server_ssl_context
             )
 
             self._server = self._loop.run_until_complete(server)
 
             self.connected = True
 
             self._cleanup_task = self._loop.create_task(self._cleanup())
 
+    async def connect_async(
+        self,
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None,
+        worker_socket: Optional[socket.socket]=None
+    ):
+
+        try:
+
+            self._loop = asyncio.get_event_loop()
+
+        except Exception:
+            self._loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(self._loop)
+
+        self._running = True
+        self._semaphore = asyncio.Semaphore(self._max_concurrency)
+
+        self._compressor = zstandard.ZstdCompressor()
+        self._decompressor = zstandard.ZstdDecompressor()
+
+        if cert_path and key_path:
+            self._server_ssl_context = self._create_server_ssl_context(
+                cert_path=cert_path,
+                key_path=key_path
+            ) 
+
+        if self.connected is False and worker_socket is None:
+            self._server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self._server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self._server_socket.bind((self.host, self.port))
+
+            self._server_socket
+
+            self._server_socket.setblocking(False)
+
+        elif self.connected is False:
+            self._server_socket = worker_socket
+            host, port = worker_socket.getsockname()
+            self.host = host
+            self.port = port
+
+        if self.connected is False:
+
+            server = self._loop.create_server(
+                lambda: MercurySyncTCPServerProtocol(
+                    self.read
+                ),
+                sock=self._server_socket,
+                ssl=self._server_ssl_context
+            )
+
+            self._server = await server
+            self.connected = True
+
+            self._cleanup_task = self._loop.create_task(self._cleanup())
+
     def _create_server_ssl_context(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ) -> ssl.SSLContext:
         
         if self._server_cert_path is None:
@@ -144,33 +223,32 @@
     async def connect_client(
         self,
         address: Tuple[str, int],
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ) -> Coroutine[Any, Any, asyncio.Transport]:
         
+        self._loop = asyncio.get_event_loop()
         if cert_path and key_path:
             self._client_ssl_context = self._create_client_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
-        host, port = address
         tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         tcp_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         await self._loop.run_in_executor(None, tcp_socket.connect, address)
 
         tcp_socket.setblocking(False)
 
         client_transport, _ = await self._loop.create_connection(
             lambda: MercurySyncTCPClientProtocol(
                 self.read
             ),
-            host=host,
-            port=port,
+            sock=tcp_socket,
             ssl=self._client_ssl_context
         )
 
         self._client_transports[address] = client_transport
 
         return client_transport
     
@@ -332,15 +410,15 @@
 
                 waiter = self._loop.create_future()
                 self._waiters[event_name].append(waiter)
 
                 await waiter
 
 
-            while len(self.queue[event_name]) > 0 and self._stream:
+            while bool(self.queue[event_name]) and self._stream:
 
                 (
                     _,
                     shard_id,
                     _,
                     response_data,
                     _, 
@@ -371,21 +449,27 @@
                     self._send_error(
                         error_message=str(decompression_error),
                         transport=transport
                     )
                 )
             )
 
-            if len(self._last_call) > 0:
+            if bool(self._last_call):
                 event_name = self._last_call.pop()
                 event_waiter = self._waiters[event_name]
 
-                if len(event_waiter) > 0:
+                if bool(event_waiter):
                     waiter = event_waiter.pop()
-                    waiter.set_result(None)
+
+                    try:
+
+                        waiter.set_result(None)
+
+                    except asyncio.InvalidStateError:
+                        pass
 
             return
 
         decrypted = self._encryptor.decrypt(decompressed)
 
         result: Tuple[
             str, 
@@ -437,17 +521,23 @@
                         transport
                     )
                 )
             )
 
             event_waiter = self._waiters[event_name]
 
-            if len(event_waiter) > 0:
+            if bool(event_waiter):
                 waiter = event_waiter.pop()
-                waiter.set_result(None)
+
+                try:
+
+                    waiter.set_result(None)
+
+                except asyncio.InvalidStateError:
+                    pass
 
         elif message_type == 'stream' or message_type == "stream_connect":
 
             self.queue[event_name].append((
                 message_type, 
                 shard_id,
                 event_name,
@@ -467,39 +557,50 @@
                         transport
                     )
                 )
             )
 
             event_waiter = self._waiters[event_name]
 
-            if len(event_waiter) > 0:
+            if bool(event_waiter):
                 waiter = event_waiter.pop()
-                waiter.set_result(None)
 
+                try:
+
+                    waiter.set_result(None)
+
+                except asyncio.InvalidStateError:
+                    pass
 
         else:
 
-            if event_name is None and len(self._last_call) > 0:
+            if event_name is None and bool(self._last_call):
                 event_name = self._last_call.pop()
 
             self.queue[event_name].append((
                 message_type, 
                 shard_id,
                 event_name,
                 payload, 
                 incoming_host,
                 incoming_port
             ))
 
                 
             event_waiter = self._waiters[event_name]
 
-            if len(event_waiter) > 0:
+            if bool(event_waiter):
                 waiter = event_waiter.pop()
-                waiter.set_result(None)
+
+                try:
+
+                    waiter.set_result(None)
+
+                except asyncio.InvalidStateError:
+                    pass
 
     async def _read(
         self,
         event_name: str,
         coroutine: Coroutine,
         transport: asyncio.Transport
     ) -> Coroutine[Any, Any, None]:
@@ -597,25 +698,26 @@
 
         transport.write(compressed)
         
     async def close(self) -> None:
         self._stream = False
         self._running = False
         
-        self._cleanup_task.cancel()
-        if self._cleanup_task.cancelled() is False:
-            try:
-                self._sleep_task.cancel()
-                if not self._sleep_task.cancelled():
-                    await self._sleep_task
+        if self._cleanup_task:
+            self._cleanup_task.cancel()
+            if self._cleanup_task.cancelled() is False:
+                try:
+                    self._sleep_task.cancel()
+                    if not self._sleep_task.cancelled():
+                        await self._sleep_task
 
-            except asyncio.CancelledError:
-                pass
+                except asyncio.CancelledError:
+                    pass
 
-            try:
+                try:
 
-                await self._cleanup_task
+                    await self._cleanup_task
 
-            except asyncio.CancelledError:
-                pass
+                except asyncio.CancelledError:
+                    pass
 
-        
+
```

### Comparing `mercury-sync-0.2.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.3.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.3.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from __future__ import annotations
 import asyncio
 import pickle
 import socket
 import ssl
 import zstandard
 from collections import deque, defaultdict
 from dtls import do_patch
@@ -44,69 +45,152 @@
 
         self.events: Dict[
             str,
             Coroutine
         ] = {}
 
         self._transport: asyncio.DatagramTransport = None
-        self._loop = asyncio.get_event_loop()
+        self._loop: Union[asyncio.AbstractEventLoop, None] = None
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
         self.parsers: Dict[str, Message] = {}
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
         self._pending_responses: Deque[asyncio.Task] = deque()
 
         self._udp_cert_path: Union[str, None] = None
         self._udp_key_path: Union[str, None] = None
         self._udp_ssl_context: Union[ssl.SSLContext, None] = None
 
         self._encryptor = AESGCMFernet(env)
-        self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
-        self._compressor = zstandard.ZstdCompressor()
-        self._decompressor = zstandard.ZstdDecompressor()
+        self._semaphore: Union[asyncio.Semaphore, None] = None
+        self._compressor: Union[zstandard.ZstdCompressor, None] = None
+        self._decompressor: Union[zstandard.ZstdDecompressor, None] = None
         
         self._running = False
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
-
+        self._max_concurrency = env.MERCURY_SYNC_MAX_CONCURRENCY
 
     def connect(
         self, 
         cert_path: Optional[str]=None,
-        key_path: Optional[str]=None
+        key_path: Optional[str]=None,
+        worker_socket: Optional[socket.socket]=None
     ) -> None:
         
+        try:
+
+            self._loop = asyncio.get_event_loop()
+
+        except Exception:
+            self._loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(self._loop)
+
         self._running = True
 
-        udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
-        udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self._semaphore = asyncio.Semaphore(self._max_concurrency)
+
+        self._compressor = zstandard.ZstdCompressor()
+        self._decompressor = zstandard.ZstdDecompressor()
+
+        if worker_socket is None:
+            udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+            udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            udp_socket.bind((
+                self.host,
+                self.port
+            ))
+
+            udp_socket.setblocking(False)
+
+        else:
+            udp_socket = worker_socket
+
 
         if cert_path and key_path:
             self._udp_ssl_context = self._create_udp_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path,
             )
 
             udp_socket = self._udp_ssl_context.wrap_socket(udp_socket)
 
-        udp_socket.bind((
-            self.host,
-            self.port
-        ))
+        server = self._loop.create_datagram_endpoint(
+            lambda: MercurySyncUDPProtocol(
+                self.read
+            ),
+            sock=udp_socket
+        )
 
-        udp_socket.setblocking(False)
+        transport, _ = self._loop.run_until_complete(server)
+        self._transport = transport
+
+        self._cleanup_task = self._loop.create_task(self._cleanup())
+
+    def copy_to_connection(self, new_udp_connection: MercurySyncUDPConnection) -> MercurySyncUDPConnection:
+        new_udp_connection.parsers.update(self.parsers)
+        new_udp_connection._udp_cert_path = self._udp_cert_path
+        new_udp_connection._udp_key_path = self._udp_key_path
+        new_udp_connection._udp_ssl_context = self._udp_ssl_context
+        new_udp_connection._running = True
+
+        new_udp_connection._semaphore = asyncio.Semaphore(self._max_concurrency)
+
+        new_udp_connection._compressor = zstandard.ZstdCompressor()
+        new_udp_connection._decompressor = zstandard.ZstdDecompressor()
+        new_udp_connection._transport = self._transport
+        new_udp_connection._cleanup_task = self._loop.create_task(new_udp_connection._cleanup())
+
+        return new_udp_connection
+
+    async def connect_async(
+        self, 
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None,
+        worker_socket: Optional[socket.socket]=None
+    ) -> None:
+        
+        self._loop = asyncio.get_event_loop()
+        self._running = True
+
+        self._semaphore = asyncio.Semaphore(self._max_concurrency)
+
+        self._compressor = zstandard.ZstdCompressor()
+        self._decompressor = zstandard.ZstdDecompressor()
+
+        if worker_socket is None:
+            udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
+            udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            udp_socket.bind((
+                self.host,
+                self.port
+            ))
+
+            udp_socket.setblocking(False)
+
+        else:
+            udp_socket = worker_socket
+
+
+        if cert_path and key_path:
+            self._udp_ssl_context = self._create_udp_ssl_context(
+                cert_path=cert_path,
+                key_path=key_path,
+            )
+
+            udp_socket = self._udp_ssl_context.wrap_socket(udp_socket)
 
         server = self._loop.create_datagram_endpoint(
             lambda: MercurySyncUDPProtocol(
                 self.read
             ),
             sock=udp_socket
         )
 
-        transport, _ = self._loop.run_until_complete(server)
+        transport, _ = await server
         self._transport = transport
 
         self._cleanup_task = self._loop.create_task(self._cleanup())
 
     def _create_udp_ssl_context(
         self,
         cert_path: Optional[str]=None,
@@ -149,15 +233,15 @@
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
     ) -> Tuple[int, Dict[str, Any]]:
 
         item = pickle.dumps((
             'request',
-            next(self.id_generator),
+            self.id_generator.generate(),
             event_name,
             data
         ), protocol=pickle.HIGHEST_PROTOCOL)
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
         
@@ -187,15 +271,15 @@
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
     ) -> AsyncIterable[Tuple[int, Dict[str, Any]]]: 
 
         item = pickle.dumps((
             'stream',
-            next(self.id_generator),
+            self.id_generator.generate(),
             event_name,
             data
         ), protocol=pickle.HIGHEST_PROTOCOL)
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
         
@@ -277,44 +361,49 @@
                         ),
                         addr
                     )
                 )
             )
 
         else:
-
             self.queue[event_name].append((
                 message_type, 
                 shard_id,
                 event_name,
                 payload, 
                 incoming_host,
                 incoming_port
             ))
 
             event_waiter = self._waiters[event_name]
 
-
-            if len(event_waiter) > 0:
+            
+            if bool(event_waiter):
                 waiter = event_waiter.pop()
-                waiter.set_result(None)
+                
+                try:
+                    
+                    waiter.set_result(None)
+                
+                except asyncio.InvalidStateError:
+                    pass
 
 
     async def _read(
         self,
         event_name: str,
         coroutine: Coroutine,
         addr: Tuple[str, int]
     ) -> Coroutine[Any, Any, None]:
         response: Message = await coroutine
 
         item = pickle.dumps(
             (
                 'response', 
-                next(self.id_generator),
+                self.id_generator.generate(),
                 event_name,
                 response.to_data()
             ),
             protocol=pickle.HIGHEST_PROTOCOL
         )
 
         encrypted_message = self._encryptor.encrypt(item)
@@ -329,38 +418,38 @@
         addr: Tuple[str, int]    
     ) -> Coroutine[Any, Any, None]:
         async for response in coroutine:
 
             item = pickle.dumps(
                 (
                     'response', 
-                    next(self.id_generator),
+                    self.id_generator.generate(),
                     event_name,
                     response.to_data()
                 ),
                 protocol=pickle.HIGHEST_PROTOCOL
             )
 
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
-
             self._transport.sendto(compressed, addr)
 
     async def close(self) -> None:
         self._running = False
         
-        self._cleanup_task.cancel()
-        if self._cleanup_task.cancelled() is False:
-            try:
-                self._sleep_task.cancel()
-                if not self._sleep_task.cancelled():
-                    await self._sleep_task
-
-            except asyncio.CancelledError:
-                pass
+        if self._cleanup_task:
+            self._cleanup_task.cancel()
+            if self._cleanup_task.cancelled() is False:
+                try:
+                    self._sleep_task.cancel()
+                    if not self._sleep_task.cancelled():
+                        await self._sleep_task
+
+                except asyncio.CancelledError:
+                    pass
 
-            try:
+                try:
 
-                await self._cleanup_task
+                    await self._cleanup_task
 
-            except asyncio.CancelledError:
-                pass
+                except asyncio.CancelledError:
+                    pass
```

### Comparing `mercury-sync-0.2.2/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.3.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.3.0/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/mercury_sync/env/env.py` & `mercury-sync-0.3.0/mercury_sync/env/env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 from pydantic import (
     BaseModel,
     StrictStr,
-    StrictInt
+    StrictInt,
+    StrictFloat
 )
 from typing import (
     Dict, 
     Union,
     Callable
 )
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
+    MERCURY_SYNC_BOOT_WAIT: StrictStr='5s'
+    MERCURY_SYNC_MAX_SUSPECT_TIMEOUT: StrictStr='10s'
+    MERCURY_SYNC_HEALTH_CHECK_TIMEOUT: StrictStr='1s'
+    MERCURY_SYNC_REGISTRATION_TIMEOUT: StrictStr='1m'
+    MERCURY_SYNC_HEALTH_POLL_INTERVAL: StrictFloat='0.2s'
+    MERCURY_SYNC_INDIRECT_CHECK_NODES: StrictInt=1
     MERCURY_SYNC_CLEANUP_INTERVAL: StrictStr='10s'
     MERCURY_SYNC_MAX_CONCURRENCY: StrictInt=2048
     MERCURY_SYNC_AUTH_SECRET: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
+            'MERCURY_SYNC_MAX_SUSPECT_TIMEOUT': str,
+            'MERCURY_SYNC_BOOT_WAIT': str,
+            'MERCURY_SYNC_REGISTRATION_TIMEOUT': str,
+            'MERCURY_SYNC_HEALTH_POLL_INTERVAL': str,
+            'MERCURY_SYNC_INDIRECT_CHECK_NODES': int,
             'MERCURY_SYNC_CLEANUP_INTERVAL': str,
             'MERCURY_SYNC_MAX_CONCURRENCY': int,
             'MERCURY_SYNC_AUTH_SECRET': str
         }
```

### Comparing `mercury-sync-0.2.2/mercury_sync/env/load_env.py` & `mercury-sync-0.3.0/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.3.0/mercury_sync/hooks/client_hook.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 from mercury_sync.service import Service
-from typing import Dict, Tuple, Any, Coroutine
+from mercury_sync.service.controller import Controller
+from typing import Union
 
 
 def client(
     call_name: str, 
     as_tcp: bool=False
 ):
 
@@ -14,24 +15,24 @@
         func.target = call_name
 
         @functools.wraps(func)
         async def decorator(
             *args,
             **kwargs
         ):
-            connection: Service = args[0]
+            connection: Union[Service, Controller] = args[0]
 
             if as_tcp:
                 return await connection.send_tcp(
                     call_name,
                     await func(*args, **kwargs)
                 )
 
             else:
                 return await connection.send(
                     call_name,
                     await func(*args, **kwargs)
                 )
-            
+
         return decorator
     
     return wraps
```

### Comparing `mercury-sync-0.2.2/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.3.0/mercury_sync/hooks/stream_hook.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
             
 
 import functools
 from mercury_sync.service import Service
-from typing import Dict, Any, AsyncIterable, Tuple, Coroutine
+from mercury_sync.service.controller import Controller
+from typing import Union
 
 
 def stream(
     call_name: str, 
     as_tcp: bool=False
 ):
 
@@ -17,15 +18,15 @@
         func.target = call_name
 
         @functools.wraps(func)
         async def decorator(
             *args,
             **kwargs
         ):
-            connection: Service = args[0]
+            connection: Union[Service, Controller] = args[0]
 
             if as_tcp:
 
                 async for data in func(*args, **kwargs):
                     async for response in connection.stream_tcp(
                         call_name,
                         data
```

### Comparing `mercury-sync-0.2.2/mercury_sync/service/service.py` & `mercury-sync-0.3.0/mercury_sync/service/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,50 @@
+from __future__ import annotations
 import asyncio
 import random
+import socket
 import inspect
 from inspect import signature
 from mercury_sync.connection.tcp.mercury_sync_tcp_connection import MercurySyncTCPConnection
 from mercury_sync.connection.udp.mercury_sync_udp_connection import MercurySyncUDPConnection
 from mercury_sync.env import load_env, Env
 from mercury_sync.models.error import Error
 from mercury_sync.models.message import Message
 from typing import (
     Tuple, 
     Dict, 
+    List,
     Optional,
     get_args,
     Union,
     AsyncIterable
 )
 
 class Service:
     
     def __init__(
         self,
         host: str,
-        port: int
+        port: int,
+        cert_path: Optional[str]=None,
+        key_path: Optional[str]=None,
+        env: Optional[Env]=None
     ) -> None:
         self.name = self.__class__.__name__
         self._instance_id = random.randint(0, 2**16)
         self._response_parsers: Dict[str, Message] = {}
 
-        env = load_env(Env.types_map())
+        self.host = host
+        self.port = port
+        self.cert_path = cert_path
+        self.key_path = key_path
+
+        if env is None:
+            env = load_env(Env.types_map())
+
         self._udp_connection = MercurySyncUDPConnection(
             host,
             port,
             self._instance_id,
             env
         )
 
@@ -63,15 +76,14 @@
             not_reserved = method_name not in reserved_methods
             is_server = hasattr(method, 'server_only')
             is_client = hasattr(method, 'client_only')
 
             rpc_signature = signature(method)
 
             if not_internal and not_reserved and is_server:
-
                 
                 for param_type in rpc_signature.parameters.values():
                     if param_type.annotation in Message.__subclasses__():
 
                         model = param_type.annotation
 
                         self._tcp_connection.parsers[method_name] = model
@@ -84,47 +96,97 @@
 
                 is_stream = inspect.isasyncgenfunction(method)
 
                 if is_stream:
 
                     response_type = rpc_signature.return_annotation
                     args = get_args(response_type)
-                    response_model: Message = args[0]
 
-                    self._response_parsers[method.target] = response_model
+                    response_call_type: Tuple[int, Message] = args[0]
+                    self._response_parsers[method.target] = get_args(response_call_type)[1]
 
                 else:
 
-                    response_model = rpc_signature.return_annotation
+                    response_type = rpc_signature.return_annotation
+                    args = get_args(response_type)
+                    response_model: Tuple[int, Message] = args[1]
+
                     self._response_parsers[method.target] = response_model
 
 
 
-        self._loop = asyncio.get_event_loop()
+
+        self._loop: Union[ asyncio.AbstractEventLoop, None] = None
 
     def start(
         self,
-        cert_path: Optional[str]=None,
-        key_path: Optional[str]=None
+        tcp_worker_socket: Optional[socket.socket]=None,
+        udp_worker_socket: Optional[socket.socket]=None
     ) -> None:
+        
+        self._loop = asyncio.get_event_loop()
+
         self._tcp_connection.connect(
-            cert_path=cert_path,
-            key_path=key_path
+            cert_path=self.cert_path,
+            key_path=self.key_path,
+            worker_socket=tcp_worker_socket
         )
-        self._udp_connection.connect(cert_path=cert_path)
+        self._udp_connection.connect(
+            cert_path=self.cert_path,
+            key_path=self.key_path,
+            worker_socket=udp_worker_socket
+        )
+
+    def create_pool(self, size: int) -> List[Service]:
+
+        port_pool_size = size * 2
+
+        ports = [
+            self.port + idx for idx in range(0, port_pool_size, 2)
+        ]
+
+        return [
+            self._copy(
+                port=port
+            ) for port in ports
+        ]
+
+    def _copy(
+        self,
+        host: str=None,
+        port: int= None
+    ):
+        
+        if host is None:
+            host = self.host
+
+        if port is None:
+            port = self.port
+
+        return type(self)(
+            host,
+            port
+        )
+
 
     async def connect(
         self,
         remote: Message,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ) -> None:
         address = (remote.host, remote.port)
         self._host_map[remote.__class__.__name__] = address
 
+        if cert_path is None:
+            cert_path = self.cert_path
+
+        if key_path is None:
+            key_path = self.key_path
+
         await self._tcp_connection.connect_client(
             (remote.host, remote.port + 1),
             cert_path=cert_path,
             key_path=key_path
         )
 
     async def send(
```

### Comparing `mercury-sync-0.2.2/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.3.0/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.2/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.3.0/mercury_sync/snowflake/snowflake_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     @classmethod
     def from_snowflake(cls, sf: Snowflake) -> 'SnowflakeGenerator':
         return cls(sf.instance, seq=sf.seq, epoch=sf.epoch, timestamp=sf.timestamp)
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> Optional[int]:
+    def generate(self) -> Optional[int]:
 
         current = int(time() * 1000)
 
         if self._ts == current:
 
             if self._seq == MAX_SEQ:
                 return None
```

### Comparing `mercury-sync-0.2.2/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.3.0/mercury_sync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.2.2
+Version: 0.3.0
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.2.2/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.3.0/mercury_sync.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 mercury_sync/env/time_parser.py
 mercury_sync/hooks/__init__.py
 mercury_sync/hooks/client_hook.py
 mercury_sync/hooks/server_hook.py
 mercury_sync/hooks/stream_hook.py
 mercury_sync/models/__init__.py
 mercury_sync/models/error.py
+mercury_sync/models/healthcheck.py
 mercury_sync/models/message.py
+mercury_sync/models/ticket.py
 mercury_sync/service/__init__.py
+mercury_sync/service/controller.py
+mercury_sync/service/monitor.py
 mercury_sync/service/service.py
 mercury_sync/snowflake/__init__.py
 mercury_sync/snowflake/constants.py
 mercury_sync/snowflake/snowflake.py
-mercury_sync/snowflake/snowflake_generator.py
+mercury_sync/snowflake/snowflake_generator.py
+mercury_sync/types/__init__.py
+mercury_sync/types/call.py
+mercury_sync/types/stream.py
```

### Comparing `mercury-sync-0.2.2/setup.py` & `mercury-sync-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,11 +38,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     install_requires=[
         'pydantic',
         'python3-dtls',
-        'zstandard'
+        'zstandard',
+        'cryptography',
+        'python-dotenv'
     ],
     python_requires='>=3.10'
 )
```

