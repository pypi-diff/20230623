# Comparing `tmp/websocket-client-1.6.0.tar.gz` & `tmp/websocket-client-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket-client-1.6.0.tar", last modified: Sat Jun 17 08:11:40 2023, max compression
+gzip compressed data, was "websocket-client-1.6.1.tar", last modified: Fri Jun 23 11:10:33 2023, max compression
```

## Comparing `websocket-client-1.6.0.tar` & `websocket-client-1.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    17445 2023-06-17 07:49:46.000000 websocket-client-1.6.0/ChangeLog
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-06-12 20:33:24.000000 websocket-client-1.6.0/LICENSE
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-06-12 20:33:24.000000 websocket-client-1.6.0/MANIFEST.in
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-17 08:11:39.993661 websocket-client-1.6.0/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-06-12 20:33:24.000000 websocket-client-1.6.0/README.md
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.989661 websocket-client-1.6.0/examples/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-06-12 20:33:24.000000 websocket-client-1.6.0/examples/echo_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-06-12 20:33:24.000000 websocket-client-1.6.0/examples/echoapp_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-06-12 20:33:24.000000 websocket-client-1.6.0/examples/rel_client.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-06-17 08:11:39.993661 websocket-client-1.6.0/setup.cfg
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-06-17 07:47:12.000000 websocket-client-1.6.0/setup.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-06-17 07:47:23.000000 websocket-client-1.6.0/websocket/__init__.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13656 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20991 2023-06-17 07:46:23.000000 websocket-client-1.6.0/websocket/_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2164 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20110 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_core.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2116 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_exceptions.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6709 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_handshake.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11816 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2220 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_logging.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5000 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_socket.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_ssl_compat.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4917 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3667 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_utils.py
--rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     7106 2023-06-12 20:33:41.000000 websocket-client-1.6.0/websocket/_wsdump.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket/tests/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/__init__.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket/tests/data/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/data/header01.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/data/header02.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/data/header03.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      486 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/echo-server.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_abnf.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12681 2023-06-17 07:58:21.000000 websocket-client-1.6.0/websocket/tests/test_app.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_cookiejar.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_http.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_url.py
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-06-12 20:33:24.000000 websocket-client-1.6.0/websocket/tests/test_websocket.py
-drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-17 08:11:39.993661 websocket-client-1.6.0/websocket_client.egg-info/
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/PKG-INFO
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/SOURCES.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/dependency_links.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/entry_points.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/requires.txt
--rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-06-17 08:11:39.000000 websocket-client-1.6.0/websocket_client.egg-info/top_level.txt
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-23 11:10:33.618825 websocket-client-1.6.1/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    17537 2023-06-23 11:06:33.000000 websocket-client-1.6.1/ChangeLog
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11339 2023-06-12 20:33:24.000000 websocket-client-1.6.1/LICENSE
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       81 2023-06-12 20:33:24.000000 websocket-client-1.6.1/MANIFEST.in
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-23 11:10:33.622825 websocket-client-1.6.1/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5997 2023-06-12 20:33:24.000000 websocket-client-1.6.1/README.md
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-23 11:10:33.610824 websocket-client-1.6.1/examples/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      344 2023-06-12 20:33:24.000000 websocket-client-1.6.1/examples/echo_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1009 2023-06-12 20:33:24.000000 websocket-client-1.6.1/examples/echoapp_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      351 2023-06-12 20:33:24.000000 websocket-client-1.6.1/examples/rel_client.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       59 2023-06-23 11:10:33.622825 websocket-client-1.6.1/setup.cfg
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2641 2023-06-23 11:04:55.000000 websocket-client-1.6.1/setup.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-23 11:10:33.614825 websocket-client-1.6.1/websocket/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      801 2023-06-23 11:04:47.000000 websocket-client-1.6.1/websocket/__init__.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    13656 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    21207 2023-06-23 11:03:57.000000 websocket-client-1.6.1/websocket/_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2164 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    20110 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_core.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2116 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_exceptions.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     6709 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_handshake.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    11816 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     2220 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_logging.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     5000 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_socket.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1122 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_ssl_compat.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4917 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     3667 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_utils.py
+-rwxrwxr-x   0 drift3r   (1000) drift3r   (1000)     7106 2023-06-12 20:33:41.000000 websocket-client-1.6.1/websocket/_wsdump.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-23 11:10:33.618825 websocket-client-1.6.1/websocket/tests/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        0 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/__init__.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-23 11:10:33.618825 websocket-client-1.6.1/websocket/tests/data/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      163 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/data/header01.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      161 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/data/header02.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      216 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/data/header03.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)      486 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/echo-server.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4175 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/test_abnf.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    12681 2023-06-17 07:58:21.000000 websocket-client-1.6.1/websocket/tests/test_app.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     4325 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/test_cookiejar.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     9623 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/test_http.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    14589 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/test_url.py
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)    18072 2023-06-12 20:33:24.000000 websocket-client-1.6.1/websocket/tests/test_websocket.py
+drwxrwxr-x   0 drift3r   (1000) drift3r   (1000)        0 2023-06-23 11:10:33.618825 websocket-client-1.6.1/websocket_client.egg-info/
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     7350 2023-06-23 11:10:33.000000 websocket-client-1.6.1/websocket_client.egg-info/PKG-INFO
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)     1014 2023-06-23 11:10:33.000000 websocket-client-1.6.1/websocket_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)        1 2023-06-23 11:10:33.000000 websocket-client-1.6.1/websocket_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       50 2023-06-23 11:10:33.000000 websocket-client-1.6.1/websocket_client.egg-info/entry_points.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       94 2023-06-23 11:10:33.000000 websocket-client-1.6.1/websocket_client.egg-info/requires.txt
+-rw-rw-r--   0 drift3r   (1000) drift3r   (1000)       10 2023-06-23 11:10:33.000000 websocket-client-1.6.1/websocket_client.egg-info/top_level.txt
```

### Comparing `websocket-client-1.6.0/ChangeLog` & `websocket-client-1.6.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 ChangeLog
 ============
 
+- 1.6.1
+  - Fix Dispatcher keyboard interrupt. Should solve reconnect loop with rel (#924)
+
 - 1.6.0
   - Fix teardown issue when ping thread is not properly ended (#918)
   - Fix double ping wait time on first ping (#912)
   - Minor typehints improvements (eda6724, 54b3013)
 
 - 1.5.3
   - Add logic to avoid error in the case where content-length header does not exist, bug introduced in 1.5.2 (#911)
```

### Comparing `websocket-client-1.6.0/LICENSE` & `websocket-client-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/PKG-INFO` & `websocket-client-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.6.0
+Version: 1.6.1
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.6.0/README.md` & `websocket-client-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/examples/echoapp_client.py` & `websocket-client-1.6.1/examples/echoapp_client.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/setup.py` & `websocket-client-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-VERSION = "1.6.0"
+VERSION = "1.6.1"
 
 install_requires = []
 tests_require = []
 
 setup(
     name="websocket-client",
     version=VERSION,
```

### Comparing `websocket-client-1.6.0/websocket/__init__.py` & `websocket-client-1.6.1/websocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 from ._abnf import *
 from ._app import WebSocketApp, setReconnect
 from ._core import *
 from ._exceptions import *
 from ._logging import *
 from ._socket import *
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
```

### Comparing `websocket-client-1.6.0/websocket/_abnf.py` & `websocket-client-1.6.1/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_app.py` & `websocket-client-1.6.1/websocket/_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         try:
             _logging.info("reconnect() - retrying in {seconds_count} seconds [{frame_count} frames in stack]".format(
                 seconds_count=seconds, frame_count=len(inspect.stack())))
             time.sleep(seconds)
             reconnector(reconnecting=True)
         except KeyboardInterrupt as e:
             _logging.info("User exited {err}".format(err=e))
+            raise e
 
 
 class Dispatcher(DispatcherBase):
     """
     Dispatcher
     """
     def read(self, sock: socket.socket, read_callback: Callable, check_callback: Callable) -> None:
@@ -498,17 +499,21 @@
 
         try:
             setSock()
             if not custom_dispatcher and reconnect:
                 while self.keep_running:
                     _logging.debug("Calling dispatcher reconnect [{frame_count} frames in stack]".format(frame_count=len(inspect.stack())))
                     dispatcher.reconnect(reconnect, setSock)
-        finally:
-            # Ensure teardown was called before returning from run_forever
+        except (KeyboardInterrupt, Exception) as e:
+            _logging.info("tearing down on exception {err}".format(err=e))
             teardown()
+        finally:
+            if not custom_dispatcher:
+                # Ensure teardown was called before returning from run_forever
+                teardown()
 
         return self.has_errored
 
     def create_dispatcher(self, ping_timeout: int, dispatcher: Dispatcher = None, is_ssl: bool = False) -> DispatcherBase:
         if dispatcher:  # If custom dispatcher is set, use WrappedDispatcher
             return WrappedDispatcher(self, ping_timeout, dispatcher)
         timeout = ping_timeout or 10
```

### Comparing `websocket-client-1.6.0/websocket/_cookiejar.py` & `websocket-client-1.6.1/websocket/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_core.py` & `websocket-client-1.6.1/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_exceptions.py` & `websocket-client-1.6.1/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_handshake.py` & `websocket-client-1.6.1/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_http.py` & `websocket-client-1.6.1/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_logging.py` & `websocket-client-1.6.1/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_socket.py` & `websocket-client-1.6.1/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_ssl_compat.py` & `websocket-client-1.6.1/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_url.py` & `websocket-client-1.6.1/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_utils.py` & `websocket-client-1.6.1/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/_wsdump.py` & `websocket-client-1.6.1/websocket/_wsdump.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/tests/test_abnf.py` & `websocket-client-1.6.1/websocket/tests/test_abnf.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/tests/test_app.py` & `websocket-client-1.6.1/websocket/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/tests/test_cookiejar.py` & `websocket-client-1.6.1/websocket/tests/test_cookiejar.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/tests/test_http.py` & `websocket-client-1.6.1/websocket/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/tests/test_url.py` & `websocket-client-1.6.1/websocket/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket/tests/test_websocket.py` & `websocket-client-1.6.1/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.0/websocket_client.egg-info/PKG-INFO` & `websocket-client-1.6.1/websocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.6.0
+Version: 1.6.1
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
 Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
```

### Comparing `websocket-client-1.6.0/websocket_client.egg-info/SOURCES.txt` & `websocket-client-1.6.1/websocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

