# Comparing `tmp/twitchify-1.1.0.tar.gz` & `tmp/twitchify-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-1.1.0.tar", last modified: Fri Jun 23 01:21:06 2023, max compression
+gzip compressed data, was "twitchify-1.1.1.tar", last modified: Fri Jun 23 19:30:58 2023, max compression
```

## Comparing `twitchify-1.1.0.tar` & `twitchify-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.022052 twitchify-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 01:20:48.000000 twitchify-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 01:21:06.022052 twitchify-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 01:20:48.000000 twitchify-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 01:21:06.022052 twitchify-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-23 01:20:48.000000 twitchify-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.014052 twitchify-1.1.0/twitch/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/broadcaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.018052 twitchify-1.1.0/twitch/types/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.018052 twitchify-1.1.0/twitch/types/eventsub/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/charity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/hypertrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/eventsub/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-23 01:20:48.000000 twitchify-1.1.0/twitch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:06.022052 twitchify-1.1.0/twitchify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 01:21:06.000000 twitchify-1.1.0/twitchify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 01:21:05.000000 twitchify-1.1.0/twitchify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.727498 twitchify-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 19:30:46.000000 twitchify-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 19:30:58.727498 twitchify-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 19:30:46.000000 twitchify-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:30:58.727498 twitchify-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-23 19:30:46.000000 twitchify-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.723498 twitchify-1.1.1/twitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.723498 twitchify-1.1.1/twitch/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.727498 twitchify-1.1.1/twitch/types/eventsub/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/charity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/hypertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.727498 twitchify-1.1.1/twitchify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-1.1.0/LICENSE` & `twitchify-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/PKG-INFO` & `twitchify-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.1.0/README.md` & `twitchify-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/setup.py` & `twitchify-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/__init__.py` & `twitchify-1.1.1/twitch/types/channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 The MIT License (MIT)
 
-Copyright (c) 2023-present MrSniFo
+Copyright (c) 2023-present Snifo
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
@@ -18,15 +18,18 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-__title__ = 'Twitchify'
-__version__ = '1.1.0'
-__license__ = 'MIT License'
-__author__ = 'Snifo'
-__email__ = 'Snifo@mail.com'
-__github__ = 'https://github.com/mrsnifo/twitchify'
+from typing import List
+from .user import Broadcaster
 
-from .client import Client
+
+class Channel(Broadcaster):
+    broadcaster_language: str
+    game_name: str
+    game_id: str
+    title: str
+    delay: int
+    tags: List[str]
```

### Comparing `twitchify-1.1.0/twitch/broadcaster.py` & `twitchify-1.1.1/twitch/broadcaster.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/channel.py` & `twitchify-1.1.1/twitch/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/client.py` & `twitchify-1.1.1/twitch/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,22 +20,21 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
 from .gateway import EventSubWebSocket
 from .state import ConnectionState
 from .utils import setup_logging
 from .http import HTTPClient
 from .channel import Channel
 from .stream import Stream
-# Libraries
+
 import asyncio
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Any, List, Optional, Callable
     from .broadcaster import Broadcaster
 
@@ -43,31 +42,55 @@
 _logger = logging.getLogger(__name__)
 
 
 class Client:
     """
     Represents a Twitch client for interacting with the Twitch API and receiving event
     notifications.
+
+    :param client_id: Client id
+    :rtype: str
+
+    :param client_secret: Client secret needed to re-generate a new access token.
+    :rtype: Optional[str]
     """
 
     def __init__(self, client_id: str, client_secret: Optional[str] = None) -> None:
         self.loop: Optional[asyncio.AbstractEventLoop] = None
         self._http = HTTPClient(dispatcher=self.dispatch, client=client_id, secret=client_secret)
         self._connection: ConnectionState = ConnectionState(dispatcher=self.dispatch,
                                                             http=self._http,
-                                                            ev=self._sub_events)
+                                                            events=self._sub_events)
 
     @property
     def user(self) -> Broadcaster:
+        """
+        Retrieve the Broadcaster.
+
+        :return: An instance of the Broadcaster class representing the user.
+        :rtype: Broadcaster
+        """
         return self._connection.broadcaster
 
     async def get_channel(self) -> Channel:
+        """
+       Retrieve the channel associated with the broadcaster.
+
+       :return: An instance of the Channel class representing the channel.
+       :rtype: Channel
+       """
         return await self._connection.broadcaster.get_channel()
 
     async def get_stream(self) -> Stream:
+        """
+        Retrieve the stream of the broadcaster if currently live.
+
+        :return: An instance of the Stream class representing the stream if live, otherwise None.
+        :rtype: Optional[Stream]
+        """
         return await self._connection.broadcaster.get_stream()
 
     @property
     def _sub_events(self) -> List[str]:
         """Retrieve the names of the subscribed events."""
         return [attr.replace('on_', '', 1) for attr in dir(self) if attr.startswith('on_')]
 
@@ -99,15 +122,15 @@
     async def on_error(event_name: str, error: str, /, *args: Any, **kwargs: Any) -> None:
         """
         The default error handler for events.
         """
         _logger.exception('Ignoring error: %s from %s, args: %s kwargs: %s', error, event_name,
                           args, kwargs)
 
-    def event(self, coro: Callable[..., Any], /):
+    def event(self, coro: Callable[..., Any], /) -> None:
         """
         Decorator to register an event coroutine.
         """
         if not asyncio.iscoroutinefunction(coro):
             raise TypeError("The registered event must be a coroutine function")
 
         setattr(self, coro.__name__, coro)
@@ -125,15 +148,15 @@
                                                    refresh_token=refresh_token)
         # Retrieving the client.
         await self._connection.get_client()
         # Creating an EventSub websocket.
         EventSub = EventSubWebSocket(http=self._http, cnx=self._connection,
                                      loop=self.loop,
                                      events=self._sub_events)
-
+        # Creating tasks.
         tasks = [
             self.loop.create_task(self._http.Refresher(expires_in=validation['expires_in']),
                                   name="Twitchify:Refresher"),
             self.loop.create_task(EventSub.connect(), name="Twitchify:EventSub")
         ]
         self.dispatch('connect')
         await asyncio.gather(*tasks)
@@ -150,14 +173,14 @@
                 await self._http.close()
             raise
         except Exception as error:
             if self._http is not None and self._http.is_open:
                 await self._http.close()
             raise error
 
-    def run(self, access_token: str, refresh_token: Optional[str] = None):
+    def run(self, access_token: str, refresh_token: Optional[str] = None) -> None:
         """
         Runs the Twitch client by establishing a connection and initiating the event loop.
         """
         async def runner():
             await self.start(access_token, refresh_token)
         asyncio.run(runner())
```

### Comparing `twitchify-1.1.0/twitch/errors.py` & `twitchify-1.1.1/twitch/errors.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/gateway.py` & `twitchify-1.1.1/twitch/gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,22 +24,21 @@
 
 from __future__ import annotations
 
 from .errors import (WebSocketError, WebsocketClosed, NotFound, SessionClosed, Forbidden,
                      SubscriptionError, WsReconnect)
 from .utils import to_json, get_subscriptions
 
-# Libraries
 from json import JSONDecodeError
 from aiohttp import WSMsgType
 import asyncio
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from .types.eventsub.subscriptions import SubscriptionPayload
+    from .types.eventsub.subscriptions import SubscriptionInfo
     from asyncio import AbstractEventLoop
     from typing import Optional, List, Dict, Any
     from aiohttp import ClientWebSocketResponse
     from .state import ConnectionState
     from .http import HTTPClient
     from .types.gateway import Session, Subscription
 
@@ -61,15 +60,15 @@
         :param cnx: The ConnectionState object.
         :param loop: The event loop.
         :param events: A list of events.
         """
         self.__http: HTTPClient = http
         self.__connection: ConnectionState = cnx
         self.__loop: AbstractEventLoop = loop
-        self.subscriptions: List[SubscriptionPayload] = get_subscriptions(events=events)
+        self.subscriptions: List[SubscriptionInfo] = get_subscriptions(events=events)
         # Default subscription
         self.subscriptions.append({'name': 'user.update', 'version': '1'})
         # Default Session KeepAlive.
         self._keep_alive: int = 10
         self._ws: Optional[ClientWebSocketResponse] = None
         self._ws_switch: Optional[ClientWebSocketResponse] = None
         self.session_id: Optional[str] = None
@@ -200,15 +199,15 @@
                     _session: Session = response['payload']['session']
                     raise WsReconnect(url=_session['reconnect_url'])
 
                 # ====> Subscription notification <====
                 elif metadata['message_type'] == 'notification':
                     _subscription: Subscription = response['payload']['subscription']
                     _event: Dict[Any] = response['payload']['event']
-                    await self.__connection.parse(event=_subscription['type'], data=_event)
+                    await self.__connection.parse(method=_subscription['type'], data=_event)
 
                 # ====> Subscription Revocation <====
                 elif metadata['message_type'] == 'revocation':
                     _subscription: Subscription = response['payload']['subscription']
                     _status = _subscription['status']
                     # Revoked the authorization token that the subscription relied on.
                     if _status == 'authorization_revoked':
```

### Comparing `twitchify-1.1.0/twitch/goals.py` & `twitchify-1.1.1/twitch/goals.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 from __future__ import annotations
 
 from .utils import parse_rfc3339_timestamp
 from .user import User
 
 from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from .types.eventsub import hypertrain as ht
     from .types.eventsub import charity as ch
     from typing import Optional, Union, List
     from .types.eventsub import goal as gl
     from datetime import datetime
```

### Comparing `twitchify-1.1.0/twitch/http.py` & `twitchify-1.1.1/twitch/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,29 +20,31 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
+from . import __version__, __github__
 from aiohttp import ClientSession, helpers
 from asyncio import Lock, sleep, Task
 from time import time
 from typing import TYPE_CHECKING, Optional, List, Callable, Any
 
 from .errors import (
     UnknownError, TwitchServerError, BadRequest, Unauthorized,
     Forbidden, HTTPException, SubscriptionError, NotFound)
 from .utils import format_seconds
 
+
 if TYPE_CHECKING:
     from .types.stream import Stream
     from .types.user import UserType
     from .types.channel import Channel
-    from .types.eventsub.subscriptions import SubscriptionPayload
+    from .types.eventsub.subscriptions import SubscriptionInfo
     from aiohttp import ClientWebSocketResponse
     from .types.http import Validate, Refresh
 
 import logging
 _logger = logging.getLogger(__name__)
 
 
@@ -82,16 +84,15 @@
         Initialize the HTTPClient object.
         """
         self._dispatch: Callable[[str, Any, Any], Task] = dispatcher
         self._client_id = client
         self._client_secret = secret
         self.__session: Optional[ClientSession] = None
         self._session_lock: Lock = Lock()
-        github = 'https://github.com/Rapptz/discord.py/blob/master/discord/http.py'
-        self._user_agent: str = f'Twitchify/1.1.0 (GitHub: {github})'
+        self._user_agent: str = f'Twitchify/{__version__} (GitHub: {__github__})'
         self._refresh_token: Optional[str] = None
 
     @property
     def is_open(self) -> bool:
         """
         Checks if the HTTP session is open.
 
@@ -326,16 +327,16 @@
                     _logger.error('Unable to make the request to URL: %s Unauthorized access.',
                                   route.url)
                     await self._validate_token(generate=True)
                     continue
                 except (Unauthorized, BadRequest):
                     raise
 
-    async def subscribe(self, *, user_id: str, session_id: str,
-                        subscriptions: List[SubscriptionPayload]) -> None:
+    async def subscribe(self, *,
+                        user_id: str, session_id: str, subscriptions: List[SubscriptionInfo]) -> None:
         """
         Subscribes to multiple events with the specified subscriptions.
 
         :param user_id:
          The user ID.
 
         :param session_id:
```

### Comparing `twitchify-1.1.0/twitch/message.py` & `twitchify-1.1.1/twitch/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/moderation.py` & `twitchify-1.1.1/twitch/moderation.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,86 +20,108 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
 from .utils import parse_rfc3339_timestamp
 from .user import User
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import moderation as md
     from typing import Optional, Union
     from datetime import datetime
 
 
 class Ban:
     """
     Represents a channel ban.
+
+    :param ban: The ban data.
     """
-    __slots__ = ('user', 'moderator', 'reason', 'banned_at', '_ends_at', 'is_permanent')
 
     def __init__(self, ban: md.Ban) -> None:
         self.user: User = User(user=ban)
         self.moderator: User = User(user=ban, prefix='moderator_user')
         self.reason: str = ban['reason']
         self.banned_at: datetime = parse_rfc3339_timestamp(timestamp=ban['banned_at'])
         self._ends_at: Optional[str] = ban['ends_at']
         self.is_permanent: bool = ban['is_permanent']
 
     @property
     def ends_at(self) -> Optional[datetime]:
+        """
+        Get the end time of the ban.
+
+        :return: The end time as a datetime object.
+        """
         if self._ends_at:
             return parse_rfc3339_timestamp(timestamp=self._ends_at)
         return None
 
     def __repr__(self) -> str:
         return f'<Ban user={self.user.__repr__()} moderator={self.moderator.__repr__()}>'
 
 
 class UnBan:
     """
     Represents a channel unban.
+
+    :param unban: The unban data.
     """
-    __slots__ = ('user', 'moderator')
 
     def __init__(self, unban: md.UnBan) -> None:
         self.user: User = User(user=unban)
         self.moderator: User = User(user=unban, prefix='moderator_user')
 
     def __repr__(self) -> str:
         return f'<UnBan user={self.user.__repr__()} moderator={self.moderator.__repr__()}>'
 
 
 class ShieldMode:
     """
     Represents a channel Shield Mode.
+
+    :param mode: The Shield Mode data.
     """
-    __slots__ = ('moderator', '_started_at', '_ended_at')
 
     def __init__(self, mode: Union[md.ShieldModeBegin, md.ShieldModeEnd]) -> None:
         self.moderator: User = User(user=mode, prefix='moderator_user')
         self._started_at: Optional[str] = mode.get('started_at')
         self._ended_at: Optional[str] = mode.get('ended_at')
 
     def __repr__(self) -> str:
-        return f'<UnBan moderator={self.moderator} _started_at={self._started_at}' \
+        return f'<ShieldMode moderator={self.moderator} _started_at={self._started_at}' \
                f' _ended_at={self._ended_at}>'
 
     @property
     def is_enabled(self) -> bool:
+        """
+        Check if Shield Mode is enabled.
+
+        :return: True if Shield Mode is enabled, False otherwise.
+        """
         return self._started_at is not None
 
     @property
     def started_at(self) -> Optional[datetime]:
+        """
+        Get the start time of Shield Mode.
+
+        :return: The start time as a datetime object.
+        """
         if self._started_at:
             return parse_rfc3339_timestamp(timestamp=self._started_at)
         return None
 
     @property
     def ended_at(self) -> Optional[datetime]:
+        """
+        Get the end time of Shield Mode.
+
+        :return: The end time as a datetime object.
+        """
         if self._ended_at:
             return parse_rfc3339_timestamp(timestamp=self._ended_at)
         return None
```

### Comparing `twitchify-1.1.0/twitch/reward.py` & `twitchify-1.1.1/twitch/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/state.py` & `twitchify-1.1.1/twitch/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 
 class ConnectionState:
     """
     Represents the state of the connection.
     """
     __slots__ = ('_http', 'broadcaster', '_dispatch', 'is_streaming', 'events')
 
-    def __init__(self, dispatcher: Callable[..., Any], http: HTTPClient, ev: List[str]) -> None:
+    def __init__(self, dispatcher: Callable[..., Any], http: HTTPClient, events: List[str]) -> None:
         self._http: HTTPClient = http
         self._dispatch: Callable[[str, Any, Any], Task] = dispatcher
         self.broadcaster: Optional[Broadcaster] = None
-        self.events: List[str] = ev
+        self.events: List[str] = events
 
     async def get_client(self) -> None:
         """
         Retrieves the broadcaster's data from the connection's HTTP client and initializes the
         Broadcaster object.
         """
         _data = await self._http.get_client()
@@ -111,23 +111,23 @@
         _user = Follower(channel=data)
         self._dispatch('follow', _user)
 
     async def parse_channel_subscribe(self, data: chl.Subscribe) -> None:
         """
         Parse a channel subscribe event.
         """
-        _user = Subscription(channel=data)
-        self._dispatch('subscribe', _user)
+        _subscription = Subscription(channel=data)
+        self._dispatch('subscribe', _subscription)
 
     async def parse_channel_subscription_end(self, data: chl.SubscriptionEnd) -> None:
         """
         Parse a channel subscription end event.
         """
-        _user = Subscription(channel=data)
-        self._dispatch('subscription_end', _user, _user)
+        _subscription = Subscription(channel=data)
+        self._dispatch('subscription_end', _subscription)
 
     async def parse_channel_subscription_gift(self, data: chl.SubscriptionGift) -> None:
         """
         Parse a channel subscription gift event.
         """
         _subscription = SubscriptionGift(channel=data)
         self._dispatch('subscription_gift', _subscription)
```

### Comparing `twitchify-1.1.0/twitch/stream.py` & `twitchify-1.1.1/twitch/stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-# Core
 from .utils import parse_rfc3339_timestamp
 from .user import User
-from datetime import datetime
-from typing import TYPE_CHECKING
 
+from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import stream as sm
-    from typing import Optional, Union, List
+    from typing import Optional, Union
     from .types import stream as mst
+    from datetime import datetime
 
 
 class Stream:
-    __slots__ = ('id', 'language', 'viewers', 'thumbnail_url', 'is_mature', 'started_at')
+    """
+    Represents a stream.
+
+    :param stream: The stream data.
+    """
 
     def __init__(self, stream: mst.Stream) -> None:
         self.id: str = stream['id']
         self.language: str = stream['language']
         self.viewers: int = stream['viewer_count']
         self.thumbnail_url: str = stream['thumbnail_url']
         self.is_mature: bool = stream['is_mature']
@@ -50,75 +53,95 @@
     def __repr__(self) -> str:
         return f'<Stream id={self.id} viewers={self.viewers} language={self.language}>'
 
 
 class Shoutout:
     """
     Represents a stream shoutout.
+
+    :param shoutout: The shoutout data.
     """
-    __slots__ = (
-        '__shoutout', 'viewer_count', 'started_at', '_cooldown_ends_at',
-        '_target_cooldown_ends_at')
 
     def __init__(self, shoutout: Union[sm.ShoutoutCreate, sm.ShoutoutReceived]) -> None:
-
         self.__shoutout = shoutout
         self.viewer_count: int = shoutout['viewer_count']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=shoutout['started_at'])
         self._cooldown_ends_at: Optional[str] = shoutout.get('cooldown_ends_at')
         self._target_cooldown_ends_at: Optional[str] = shoutout.get('target_cooldown_ends_at')
 
     def __repr__(self) -> str:
         return f'<Shoutout sender={self.sender.__repr__()} Receiver={self.receiver.__repr__()}>'
 
     @property
     def sender(self) -> User:
+        """
+        Get the sender of the shoutout.
+
+        :return: The sender User object.
+        """
         if self._cooldown_ends_at:
             return User(user=self.__shoutout, prefix='broadcaster_user')
         return User(user=self.__shoutout, prefix='from_broadcaster_user')
 
     @property
     def receiver(self):
+        """
+        Get the receiver of the shoutout.
+
+        :return: The receiver User object.
+        """
         if self._cooldown_ends_at is None:
             return User(user=self.__shoutout, prefix='broadcaster_user')
         return User(user=self.__shoutout, prefix='to_broadcaster_user')
 
     @property
     def cooldown_ends_at(self) -> Optional[datetime]:
+        """
+        Get the cooldown end time.
+
+        :return: The cooldown end time as a datetime object.
+        """
         if self._cooldown_ends_at:
             return parse_rfc3339_timestamp(timestamp=self._cooldown_ends_at)
         return None
 
     @property
     def target_cooldown_ends_at(self) -> Optional[datetime]:
+        """
+        Get the target cooldown end time.
+
+        :return: The target cooldown end time as a datetime object.
+        """
         if self._target_cooldown_ends_at:
             return parse_rfc3339_timestamp(timestamp=self._target_cooldown_ends_at)
         return None
 
 
 class Online:
     """
     Represents an online stream.
+
+    :param stream: The online stream data.
     """
-    __slots__ = ('user', 'id', 'type', 'started_at')
 
     def __init__(self, stream: sm.Online) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
         self.id: str = stream['id']
         self.type: str = stream['type']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=stream['started_at'])
 
     def __repr__(self) -> str:
         return f'<Online user={self.user} id={self.id} started_at={self.started_at}>'
 
 
 class Offline:
     """
     Represents an offline stream.
+
+    :param stream: The offline stream data.
     """
-    __slots__ = ('user',)
 
     def __init__(self, stream: sm.Offline) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
 
     def __repr__(self) -> str:
         return f'<Offline user={self.user}>'
```

### Comparing `twitchify-1.1.0/twitch/survey.py` & `twitchify-1.1.1/twitch/survey.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,219 +1,225 @@
-"""
-The MIT License (MIT)
-
-Copyright (c) 2023-present Snifo
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-
 from __future__ import annotations
 
-# Core
 from .utils import parse_rfc3339_timestamp
-from .user import User
+from .user import Predictor
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Optional, List, Union, Literal
-    from .types.eventsub import poll as pl
     from .types.eventsub import prediction as pd
+    from .types.eventsub import poll as pl
     from datetime import datetime
 
 
-class _Voting:
+class Voting:
     """
     Represents voting settings for a poll.
-    """
 
+    :param vote: The voting settings for the poll.
+    """
     __slots__ = ('enabled', 'amount_per_vote')
 
-    def __init__(self, *, vote: pl.Voting):
+    def __init__(self, vote: pl.Voting) -> None:
         self.enabled: bool = vote['is_enabled']
         self.amount_per_vote: int = vote['amount_per_vote']
 
     def __repr__(self):
         return f'<Voting enabled={self.enabled} amount_per_vote={self.amount_per_vote}>'
 
 
-class _Choice:
+class Choice:
     """
     Represents a choice in a poll.
+
+    :param choice: The choice data for the poll.
     """
     __slots__ = ('id', 'title', 'bits_votes', 'points_votes')
 
-    def __init__(self, choice: Union[pl.Choice, pl.ChoicesCount]):
+    def __init__(self, choice: Union[pl.Choice, pl.ChoicesCount]) -> None:
         self.id: str = choice['id']
         self.title: str = choice['title']
         self.bits_votes: int = choice.get('bits_votes') or 0
         self.points_votes: int = choice.get('channel_points_votes') or 0
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Choice id={self.id} title={self.title}>'
 
 
 class Poll:
     """
     Represents a channel poll.
+
+    :param poll: The poll data.
     """
     __slots__ = ('id', 'title', '_choices', 'bits_voting', 'points_voting', 'started_at',
                  '_ends_at', '_ended_at', '_status')
 
-    def __init__(self, poll: Union[pl.Begin, pl.Progress, pl.End]):
+    def __init__(self, poll: Union[pl.Begin, pl.Progress, pl.End]) -> None:
         self.id: str = poll['id']
         self.title: str = poll['title']
         self._choices: List[Union[pl.Choice, pl.ChoicesCount]] = poll['choices']
-        self.bits_voting: _Voting = _Voting(vote=poll['bits_voting'])
-        self.points_voting: _Voting = _Voting(vote=poll['channel_points_voting'])
+        self.bits_voting: Voting = Voting(vote=poll['bits_voting'])
+        self.points_voting: Voting = Voting(vote=poll['channel_points_voting'])
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=poll['started_at'])
         self._ends_at: Optional[str] = poll.get('ends_at')
         self._ended_at: Optional[str] = poll.get('ended_at')
         self._status: Literal['completed', 'archived', 'terminated'] = poll.get('status')
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Poll id={self.id} title={self.title}>'
 
     @property
-    def choices(self) -> List[_Choice]:
-        return [_Choice(choice=c) for c in self._choices]
+    def choices(self) -> List[Choice]:
+        """
+        Get the list of choices for the poll.
+
+        :return: The list of poll choices.
+        """
+        return [Choice(choice=c) for c in self._choices]
 
     @property
-    def is_ended(self):
+    def is_ended(self) -> bool:
+        """
+        Check if the poll has ended.
+
+        :return: True if the poll has ended, False otherwise.
+        """
         return self._ended_at is not None
 
     @property
     def status(self) -> Literal['active', 'completed', 'archived', 'terminated']:
+        """
+        Get the status of the poll.
+
+        :return: The status of the poll.
+        """
         if self._ended_at:
             return self._status
         return 'active'
 
     @property
     def end_at(self) -> datetime:
+        """
+        Get the end timestamp of the poll.
+
+        :return: The end timestamp of the poll.
+        """
         if self._ended_at is not None:
             return parse_rfc3339_timestamp(timestamp=self._ended_at)
         return parse_rfc3339_timestamp(timestamp=self._ends_at)
 
 
-class _Predictor:
-    """
-    Represents a predictor in a prediction.
-    """
-
-    __slots__ = ('user', 'points_used', 'points_won', '_points_won')
-
-    def __init__(self, predictor: pd.Predictor):
-        self.user = User(user=predictor)
-        self.points_used: int = predictor['channel_points_used']
-        self.points_won: int = predictor['channel_points_won'] or 0
-        self._points_won: Optional[int] = predictor['channel_points_won']
-
-    @property
-    def is_won(self) -> bool:
-        return self._points_won is not None and self.points_won != 0
-
-    def __repr__(self):
-        return f'<Predictor user={self.user.__repr__()} points_won={self.points_won}>'
-
-
-class _Outcome:
+class Outcome:
     """
     Represents an outcome in a prediction.
+
+    :param outcome: The outcome data.
     """
     __slots__ = ('id', 'title', 'color', '_users', '_top_predictors')
 
-    def __init__(self, outcome: Union[pd.BaseOutcome, pd.Outcome]):
+    def __init__(self, outcome: Union[pd.BaseOutcome, pd.Outcome]) -> None:
         self.id: str = outcome['id']
         self.title: str = outcome['title']
         self.color: str = outcome['color']
         self._users: int = outcome.get('users') or 0
         self._top_predictors: Optional[List[pd.Predictor]] = outcome.get('top_predictors')
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Outcome user={self.id} title={self.title} color={self.color}>'
 
     @property
     def users(self) -> int:
+        """
+        Get the number of users associated with the outcome.
+
+        :return: The number of users associated with the outcome.
+        """
         if self._top_predictors is None:
             return self._users
         return len(self._top_predictors)
 
     @property
-    def top_predictors(self) -> List[_Predictor]:
+    def top_predictors(self) -> List[Predictor]:
+        """
+        Get the list of top predictors for the outcome.
+
+        :return: The list of top predictors.
+        """
         if self._top_predictors:
-            return [_Predictor(predictor=p) for p in self._top_predictors]
+            return [Predictor(predictor=p) for p in self._top_predictors]
         return []
 
 
 class Prediction:
     """
     Represents a channel prediction.
+
+    :param prediction: The prediction data.
     """
     __slots__ = ('id', 'title', '_outcomes', 'started_at', '_locks_at', '_locked_at', '_ended_at',
                  '_status')
 
-    def __init__(self, *, prediction: Union[pd.Begin, pd.Progress, pd.Lock, pd.End]):
+    def __init__(self, prediction: Union[pd.Begin, pd.Progress, pd.Lock, pd.End]) -> None:
         self.id: str = prediction['id']
         self.title: str = prediction['title']
-        self._outcomes: List[Union[pd.Outcome, pd.BaseOutcome]] = prediction['outcomes']
+        self._outcomes: List[Union[pd.BaseOutcome, pd.Outcome]] = prediction['outcomes']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=prediction['started_at'])
         self._locks_at: Optional[str] = prediction.get('locks_at')
         self._locked_at: Optional[str] = prediction.get('locked_at')
         self._ended_at: Optional[str] = prediction.get('ended_at')
-        self._status: Optional[Literal['resolved', 'canceled']] = prediction.get('status')
+        self._status: Literal['active', 'completed', 'archived', 'resolved'] = prediction.get('status')
 
-    def __repr__(self):
-        return f'<Prediction user={self.id} title={self.title}>'
+    def __repr__(self) -> str:
+        return f'<Prediction id={self.id} title={self.title}>'
 
     @property
-    def outcomes(self) -> List[_Outcome]:
-        return [_Outcome(outcome=o) for o in self._outcomes]
+    def outcomes(self) -> List[Outcome]:
+        """
+        Get the list of outcomes for the prediction.
 
-    @property
-    def status(self) -> Literal['open', 'locked', 'resolved', 'canceled']:
-        if self._locks_at:
-            return 'open'
-        if self._locked_at:
-            return 'locked'
-        return self._status
+        :return: The list of prediction outcomes.
+        """
+        return [Outcome(outcome=o) for o in self._outcomes]
 
     @property
-    def is_locked(self) -> bool:
-        if self._locked_at or self._ended_at:
-            return True
-        return False
+    def is_ended(self) -> bool:
+        """
+        Check if the prediction has ended.
+
+        :return: True if the prediction has ended, False otherwise.
+        """
+        return self._ended_at is not None
 
     @property
-    def is_ended(self) -> bool:
+    def status(self) -> Literal['active', 'completed', 'archived', 'resolved']:
+        """
+        Get the status of the prediction.
+
+        :return: The status of the prediction.
+        """
         if self._ended_at:
-            return True
-        return False
+            return self._status
+        return 'active'
 
     @property
-    def lock_at(self) -> Optional[datetime]:
-        if self._locks_at:
-            return parse_rfc3339_timestamp(timestamp=self._locks_at)
-        if self._locked_at:
+    def locks_at(self) -> datetime:
+        """
+        Get the locks timestamp of the prediction.
+
+        :return: The locks timestamp of the prediction.
+        """
+        if self._locked_at is not None:
             return parse_rfc3339_timestamp(timestamp=self._locked_at)
-        return None
+        return parse_rfc3339_timestamp(timestamp=self._locks_at)
 
     @property
     def ended_at(self) -> Optional[datetime]:
+        """
+        Get the end time of Prediction.
+
+        :return: The end time as a datetime object.
+        """
         if self._ended_at:
             return parse_rfc3339_timestamp(timestamp=self._ended_at)
         return None
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/channel.py` & `twitchify-1.1.1/twitch/types/eventsub/channel.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,17 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
-from ..user import SpecificBroadcaster, SpecificUser, SpecificAnonymous, ToSpecificBroadcaster,\
-    FromSpecificBroadcaster
+from ..user import (SpecificBroadcaster, SpecificUser, SpecificAnonymous,
+                    ToSpecificBroadcaster, FromSpecificBroadcaster)
 from ..message import Message
-
-# Libraries
 from typing import Optional
 
 
 class Update(SpecificBroadcaster):
     """
     Type: Channel Update
     Name: `channel.update`
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/charity.py` & `twitchify-1.1.1/twitch/types/eventsub/charity.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificBroadcaster, SpecificUser
-# Libraries
 from typing import TypedDict
 
 
 class SpecificCharity(TypedDict):
     charity_name: str
     charity_description: str
     charity_logo: str
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/goal.py` & `twitchify-1.1.1/twitch/types/eventsub/goal.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificBroadcaster
-# Libraries
 from typing import TypedDict, Literal
 
 
 class Goal(TypedDict):
     type: Literal['follow', 'subscription', 'subscription_count', 'new_subscription',
                   'new_subscription_count']
     current_amount: int
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/hypertrain.py` & `twitchify-1.1.1/twitch/types/eventsub/hypertrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificBroadcaster, SpecificUser
-# Libraries
 from typing import Literal, List
 
 
 class Contributor(SpecificUser):
     type: Literal['bits', 'subscription', 'other']
     total: int
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/moderation.py` & `twitchify-1.1.1/twitch/types/eventsub/moderation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificBroadcaster, SpecificModerator, SpecificUser
-# Libraries
 from typing import Optional
 
 
 class Ban(SpecificBroadcaster, SpecificModerator, SpecificUser):
     """
     Type: Channel Ban
     Name: `channel.ban`
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/poll.py` & `twitchify-1.1.1/twitch/types/eventsub/poll.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/types/eventsub/prediction.py` & `twitchify-1.1.1/twitch/types/eventsub/prediction.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificBroadcaster
-# Libraries
 from typing import TypedDict, Optional, Literal, List
 
 
 class BaseOutcome(TypedDict):
     id: str
     title: str
     color: str
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/reward.py` & `twitchify-1.1.1/twitch/types/eventsub/reward.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificBroadcaster, SpecificUser
-# Libraries
 from typing import TypedDict, Optional, Literal
 
 
 class BaseReward(TypedDict):
     id: str
     title: str
     cost: int
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/stream.py` & `twitchify-1.1.1/twitch/types/eventsub/stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 # Core
-from ..user import SpecificBroadcaster, SpecificModerator, ToSpecificBroadcaster,\
-    FromSpecificBroadcaster
-# Libraries
+from ..user import (SpecificBroadcaster, SpecificModerator,
+                    ToSpecificBroadcaster, FromSpecificBroadcaster)
 from typing import Literal
 
 
 class BaseShoutout(SpecificBroadcaster):
     viewer_count: int
     started_at: str
```

### Comparing `twitchify-1.1.0/twitch/types/eventsub/user.py` & `twitchify-1.1.1/twitch/types/eventsub/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Core
 from ..user import SpecificUser
 
 
 class Update(SpecificUser, total=False):
     """
     Type: User Update
     Name: `user.update`
```

### Comparing `twitchify-1.1.0/twitch/types/gateway.py` & `twitchify-1.1.1/twitch/types/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Libraries
 from typing import Optional, TypedDict, Dict
 
 __all__ = ('Session', 'Subscription')
 
 
 class _Metadata(TypedDict):
     """
```

### Comparing `twitchify-1.1.0/twitch/types/http.py` & `twitchify-1.1.1/twitch/types/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Libraries
 from typing import TypedDict, List
 
 
 class Validate(TypedDict):
     client_id: str
     login: str
     scopes: List[str]
```

### Comparing `twitchify-1.1.0/twitch/types/message.py` & `twitchify-1.1.1/twitch/types/eventsub/subscriptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,16 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Libraries
-from typing import TypedDict, List
+from typing import TypedDict
 
 
-class Emote(TypedDict):
-    begin: int
-    end: int
-    id: str
-
-
-class Message(TypedDict):
-    text: str
-    emotes: List[Emote]
+class SubscriptionInfo(TypedDict):
+    """
+    Represents a subscription with a name and a version.
+    """
+    name: str
+    version: str
```

### Comparing `twitchify-1.1.0/twitch/types/stream.py` & `twitchify-1.1.1/twitch/types/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.0/twitch/types/user.py` & `twitchify-1.1.1/twitch/types/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-# Libraries
 from typing import TypedDict, Literal, Optional
 
 Types = Literal['admin', 'global_mod', 'staff', '']
 Tier = Literal['affiliate', 'partner', '']
 
 
 class UserImages(TypedDict):
```

### Comparing `twitchify-1.1.0/twitch/user.py` & `twitchify-1.1.1/twitch/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from __future__ import annotations
 
 from .utils import parse_rfc3339_timestamp
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from .types.eventsub import (channel as chl, user as us)
+    from .types.eventsub import (channel as chl, user as us, prediction as pd)
     from typing import Optional, Dict, Any
     from datetime import datetime
 
 
 class User:
     """
     Represents a user.
@@ -72,7 +72,35 @@
         super().__init__(user=update)
         self.description: str = update['description']
         self.email: Optional[str] = update.get('email')  # Requires user:read:email scope
         self.email_verified: bool = update['email_verified']
 
     def __repr__(self) -> str:
         return f'<Update user={super().__repr__()} description={self.description}>'
+
+
+class Predictor:
+    """
+    Represents a predictor in a prediction.
+
+    :param predictor: The predictor data.
+    """
+
+    __slots__ = ('user', 'points_used', 'points_won', '_points_won')
+
+    def __init__(self, predictor: pd.Predictor) -> None:
+        self.user = User(user=predictor)
+        self.points_used: int = predictor['channel_points_used']
+        self.points_won: int = predictor['channel_points_won'] or 0
+        self._points_won: Optional[int] = predictor['channel_points_won']
+
+    @property
+    def is_won(self) -> bool:
+        """
+       Check if the predictor has won.
+
+       :return: True if the predictor has won, False otherwise.
+       """
+        return self._points_won is not None and self.points_won != 0
+
+    def __repr__(self) -> str:
+        return f'<Predictor user={super().__repr__()} points_won={self.points_won}>'
```

### Comparing `twitchify-1.1.0/twitchify.egg-info/PKG-INFO` & `twitchify-1.1.1/twitchify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.1.0/twitchify.egg-info/SOURCES.txt` & `twitchify-1.1.1/twitchify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

