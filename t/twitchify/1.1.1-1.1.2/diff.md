# Comparing `tmp/twitchify-1.1.1.tar.gz` & `tmp/twitchify-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-1.1.1.tar", last modified: Fri Jun 23 19:30:58 2023, max compression
+gzip compressed data, was "twitchify-1.1.2.tar", last modified: Fri Jun 23 20:11:24 2023, max compression
```

## Comparing `twitchify-1.1.1.tar` & `twitchify-1.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.727498 twitchify-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 19:30:46.000000 twitchify-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 19:30:58.727498 twitchify-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 19:30:46.000000 twitchify-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:30:58.727498 twitchify-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-23 19:30:46.000000 twitchify-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.723498 twitchify-1.1.1/twitch/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/broadcaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.723498 twitchify-1.1.1/twitch/types/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.727498 twitchify-1.1.1/twitch/types/eventsub/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/charity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/hypertrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/eventsub/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-06-23 19:30:46.000000 twitchify-1.1.1/twitch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:30:58.727498 twitchify-1.1.1/twitchify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 19:30:58.000000 twitchify-1.1.1/twitchify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 20:11:10.000000 twitchify-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 20:11:24.562590 twitchify-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 20:11:10.000000 twitchify-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 20:11:24.562590 twitchify-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-23 20:11:10.000000 twitchify-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.558590 twitchify-1.1.2/twitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/twitch/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/twitch/types/eventsub/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/charity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/hypertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/eventsub/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-06-23 20:11:10.000000 twitchify-1.1.2/twitch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:11:24.562590 twitchify-1.1.2/twitchify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 20:11:24.000000 twitchify-1.1.2/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-1.1.1/LICENSE` & `twitchify-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/PKG-INFO` & `twitchify-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.1.1/README.md` & `twitchify-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/setup.py` & `twitchify-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/broadcaster.py` & `twitchify-1.1.2/twitch/broadcaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types import channel as ch
     from .types import stream as stm
     from typing import Optional
     from .http import HTTPClient
 
+__all__ = ('Broadcaster',)
+
 
 class Images:
     """
     Represents images associated with a Twitch user.
 
     :param user: The user's image data.
     """
@@ -76,27 +78,25 @@
 
     @cache_decorator(expiry_seconds=20)
     async def get_channel(self) -> Channel:
         """
         Retrieve the channel associated with the broadcaster.
 
         :return: An instance of the Channel class representing the channel.
-        :rtype: Channel
         """
         data: ch.Channel = await self.__http.get_channel(broadcaster_id=self.id)
         _channel = Channel(channel=data)
         _channel.description = self.bio
         return _channel
 
     @cache_decorator(expiry_seconds=12)
     async def get_stream(self) -> Optional[Stream]:
         """
         Retrieve the stream of the broadcaster if currently live.
 
         :return: An instance of the Stream class representing the stream if live, otherwise None.
-        :rtype: Optional[Stream]
         """
         data: Optional[stm.Stream] = await self.__http.get_stream(user_id=self.id)
         if data:
             _stream = Stream(stream=data)
             return _stream
         return None
```

### Comparing `twitchify-1.1.1/twitch/channel.py` & `twitchify-1.1.2/twitch/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import channel as chl
     from .types import channel as ch
     from typing import Optional, List, Union
 
+__all__ = ('Channel', 'Update', 'Subscription', 'SubscriptionGift', 'SubscriptionMessage', 'Cheer', 'Raid')
+
 
 class Category:
     """
     Represents a category for a channel.
 
     :param channel: The channel data.
     """
```

### Comparing `twitchify-1.1.1/twitch/client.py` & `twitchify-1.1.2/twitch/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,24 @@
 if TYPE_CHECKING:
     from typing import Any, List, Optional, Callable
     from .broadcaster import Broadcaster
 
 import logging
 _logger = logging.getLogger(__name__)
 
+__all__ = ('Client',)
+
 
 class Client:
     """
     Represents a Twitch client for interacting with the Twitch API and receiving event
     notifications.
 
     :param client_id: Client id
-    :rtype: str
-
     :param client_secret: Client secret needed to re-generate a new access token.
-    :rtype: Optional[str]
     """
 
     def __init__(self, client_id: str, client_secret: Optional[str] = None) -> None:
         self.loop: Optional[asyncio.AbstractEventLoop] = None
         self._http = HTTPClient(dispatcher=self.dispatch, client=client_id, secret=client_secret)
         self._connection: ConnectionState = ConnectionState(dispatcher=self.dispatch,
                                                             http=self._http,
@@ -63,33 +62,30 @@
 
     @property
     def user(self) -> Broadcaster:
         """
         Retrieve the Broadcaster.
 
         :return: An instance of the Broadcaster class representing the user.
-        :rtype: Broadcaster
         """
         return self._connection.broadcaster
 
     async def get_channel(self) -> Channel:
         """
        Retrieve the channel associated with the broadcaster.
 
        :return: An instance of the Channel class representing the channel.
-       :rtype: Channel
        """
         return await self._connection.broadcaster.get_channel()
 
     async def get_stream(self) -> Stream:
         """
         Retrieve the stream of the broadcaster if currently live.
 
         :return: An instance of the Stream class representing the stream if live, otherwise None.
-        :rtype: Optional[Stream]
         """
         return await self._connection.broadcaster.get_stream()
 
     @property
     def _sub_events(self) -> List[str]:
         """Retrieve the names of the subscribed events."""
         return [attr.replace('on_', '', 1) for attr in dir(self) if attr.startswith('on_')]
```

### Comparing `twitchify-1.1.1/twitch/errors.py` & `twitchify-1.1.2/twitch/errors.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/gateway.py` & `twitchify-1.1.2/twitch/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/goals.py` & `twitchify-1.1.2/twitch/goals.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 from .utils import parse_rfc3339_timestamp
-from .user import User
+from .user import User, Contributor
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import hypertrain as ht
     from .types.eventsub import charity as ch
     from typing import Optional, Union, List
     from .types.eventsub import goal as gl
     from datetime import datetime
 
+__all__ = ('Charity', 'Donation', 'Goal', 'Train', 'HyperTrain')
+
 
 class CharityInfo:
     """
     Information about a charity.
 
     :param charity: A dictionary containing charity information.
     """
@@ -111,15 +113,15 @@
         self.user: User = User(user=donation)
         self.amount: CharityAmount = CharityAmount(amount=donation['amount'])
 
     def __repr__(self) -> str:
         return f'<Donation id={self.id} user={self.user.__repr__()}>'
 
 
-class _GoalAmount:
+class GoalAmount:
     """
     Represents the amount and type of goal.
 
     :param goal: A dictionary containing goal information.
     """
 
     def __init__(self, goal: gl.Goal) -> None:
@@ -137,45 +139,28 @@
     :param goal: An object representing a goal.
     """
     __slots__ = ('id', 'description', 'amount', 'started_at', 'is_achieved', '_ended_at')
 
     def __init__(self, goal: Union[gl.Begin, gl.Progress, gl.End]) -> None:
         self.id: str = goal['id']
         self.description: str = goal['description']
-        self.amount: _GoalAmount = _GoalAmount(goal=goal)
+        self.amount: GoalAmount = GoalAmount(goal=goal)
         self.started_at: datetime = parse_rfc3339_timestamp(goal['started_at'])
         self.is_achieved: bool = goal.get('is_achieved') or False
         self._ended_at: Optional[str] = goal.get('ended_at')
 
     def __repr__(self) -> str:
         return f'<Goal id={self.id} amount={self.amount.__repr__()} started_at={self.started_at}>'
 
     @property
     def ended_at(self) -> Optional[datetime]:
         """The datetime when the goal ended."""
         return parse_rfc3339_timestamp(self._ended_at) if self._ended_at else None
 
 
-class _Contributor:
-    """
-    Hyper train top contributor.
-
-    :param contributor: A dictionary containing contributor information.
-    """
-    __slots__ = ('user', 'type', 'total')
-
-    def __init__(self, contributor: ht.Contributor) -> None:
-        self.user: User = User(user=contributor)
-        self.type: str = contributor['type']
-        self.total: int = contributor['total']
-
-    def __repr__(self) -> str:
-        return f'<_Contributor user={self.user.__repr__()} total={self.total} type={self.type}>'
-
-
 class Train:
     """
     Hyper train progress.
     """
     __slots__ = ('progress', 'goal', 'expires_at', '_last_contribution')
 
     def __init__(self, train: ht.Begin) -> None:
@@ -184,17 +169,17 @@
         self.expires_at: datetime = parse_rfc3339_timestamp(train['expires_at'])
         self._last_contribution: List[ht.Contributor] = train['last_contribution']
 
     def __repr__(self) -> str:
         return f'<_Train goal={self.goal} progress={self.progress} expires_at={self.expires_at}>'
 
     @property
-    def last_contribution(self) -> List[_Contributor]:
+    def last_contribution(self) -> List[Contributor]:
         """The list of top contributors in the last contribution."""
-        return [_Contributor(contributor=c) for c in self._last_contribution]
+        return [Contributor(contributor=c) for c in self._last_contribution]
 
 
 class HyperTrain:
     """
     Represents a channel Hyper Train.
 
     :param hypertrain: An object representing a Hyper Train.
@@ -213,17 +198,17 @@
         self._ended_at: Optional[str] = hypertrain.get('ended_at')
         self._cooldown_ends_at: Optional[str] = hypertrain.get('cooldown_ends_at')
 
     def __repr__(self) -> str:
         return f'<HyperTrain id={self.id} level={self.level} total={self.total}>'
 
     @property
-    def top_contributions(self) -> List[_Contributor]:
+    def top_contributions(self) -> List[Contributor]:
         """The list of top contributors in the Hyper Train."""
-        return [_Contributor(contributor=c) for c in self._top_contributions]
+        return [Contributor(contributor=c) for c in self._top_contributions]
 
     @property
     def train(self) -> Optional[Train]:
         """The Hyper Train progress if it's ongoing, None otherwise."""
         if not self._ended_at:
             return Train(train=self.__hypertrain)
         return None
```

### Comparing `twitchify-1.1.1/twitch/http.py` & `twitchify-1.1.2/twitch/http.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/message.py` & `twitchify-1.1.2/twitch/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/moderation.py` & `twitchify-1.1.2/twitch/moderation.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import moderation as md
     from typing import Optional, Union
     from datetime import datetime
 
+__all__ = ('Ban', 'UnBan', 'ShieldMode')
+
 
 class Ban:
     """
     Represents a channel ban.
 
     :param ban: The ban data.
     """
```

### Comparing `twitchify-1.1.1/twitch/reward.py` & `twitchify-1.1.2/twitch/reward.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,181 +20,182 @@
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
     from .types.eventsub import reward as rd
     from datetime import datetime
     from typing import Optional
 
+__all__ = ('Reward', 'Redemption')
 
-class _Image:
+
+class Image:
     """
     Represents a custom image for a reward.
-    """
 
-    __slots__ = ('url_1x', 'url_2x', 'url_4x')
+    :param image: The image data.
+    """
 
-    def __init__(self, *, image: rd.Image) -> None:
+    def __init__(self, image: rd.Image) -> None:
         self.url_1x: str = image['url_1x']
         self.url_2x: str = image['url_2x']
         self.url_4x: str = image['url_4x']
 
 
-class _OptionalImage:
+class OptionalImage:
     """
     Represents an optional custom image for a reward.
-    """
 
-    __slots__ = ('url_1x', 'url_2x', 'url_4x')
+    :param image: The image data.
+    """
 
-    def __init__(self, *, image: rd.OptionalImage) -> None:
+    def __init__(self, image: rd.OptionalImage) -> None:
         self.url_1x: Optional[str] = image['url_1x']
         self.url_2x: Optional[str] = image['url_2x']
         self.url_4x: Optional[str] = image['url_4x']
 
 
-class _MaxValue:
+class MaxValue:
     """
     Represents a maximum value setting for a reward.
-    """
 
-    __slots__ = ('is_enabled', 'value')
+    :param data: The maximum value data.
+    """
 
-    def __init__(self, *, data: rd.MaxValue) -> None:
+    def __init__(self, data: rd.MaxValue) -> None:
         self.is_enabled: bool = data['is_enabled']
         self.value: int = data['value']
 
 
-class _MaxCooldown:
+class MaxCooldown:
     """
     Represents a maximum cooldown setting for a reward.
-    """
 
-    __slots__ = ('is_enabled', 'seconds')
+    :param data: The maximum cooldown data.
+    """
 
-    def __init__(self, *, data: rd.Cooldown):
+    def __init__(self, data: rd.Cooldown) -> None:
         self.is_enabled: bool = data['is_enabled']
         self.seconds: int = data['seconds']
 
 
-class _Status:
+class Status:
     """
     Represents the status of a reward.
-    """
 
-    __slots__ = ('is_enabled', 'is_paused', 'is_in_stock')
+    :param reward: The reward data.
+    """
 
-    def __init__(self, *, reward: rd.Reward) -> None:
+    def __init__(self, reward: rd.Reward) -> None:
         self.is_enabled: bool = reward['is_enabled']
         self.is_paused: bool = reward['is_paused']
         self.is_in_stock: bool = reward['is_in_stock']
 
 
-class _Appearance:
+class Appearance:
     """
     Represents the appearance settings for a reward.
-    """
 
-    __slots__ = ('title', 'description', 'is_in_stock', 'background_color', 'image',
-                 'default_image')
+    :param reward: The reward data.
+    """
 
-    def __init__(self, *, reward: rd.Reward) -> None:
+    def __init__(self, reward: rd.Reward) -> None:
         self.title: str = reward['title']
         self.description: str = reward['prompt']
         self.background_color: str = reward['background_color']
-        self.image: _OptionalImage = _OptionalImage(image=reward['image'])
-        self.default_image: _Image = _Image(image=reward['default_image'])
+        self.image: OptionalImage = OptionalImage(image=reward['image'])
+        self.default_image: Image = Image(image=reward['default_image'])
 
 
-class _Options:
+class Options:
     """
     Represents the options for a reward.
-    """
 
-    __slots__ = ('redemptions_skip_request_queue', 'max_per_stream', 'max_per_user_per_stream',
-                 'is_user_input_required')
+    :param reward: The reward data.
+    """
 
-    def __init__(self, *, reward: rd.Reward) -> None:
+    def __init__(self, reward: rd.Reward) -> None:
         self.redemptions_skip_request_queue: bool = reward['should_redemptions_skip_request_queue']
-        self.max_per_stream: _MaxValue = _MaxValue(data=reward['max_per_stream'])
-        self.max_per_user_per_stream: _MaxValue = _MaxValue(data=reward['max_per_user_per_stream'])
+        self.max_per_stream: MaxValue = MaxValue(data=reward['max_per_stream'])
+        self.max_per_user_per_stream: MaxValue = MaxValue(data=reward['max_per_user_per_stream'])
         self.is_user_input_required: bool = reward['is_user_input_required']
 
 
-class _Cooldown:
+class Cooldown:
     """
     Represents the cooldown settings for a reward.
-    """
 
-    __slots__ = ('duration', '_cooldown_expires_at')
+    :param reward: The reward data.
+    """
 
-    def __init__(self, *, reward: rd.Reward) -> None:
-        self.duration: _MaxCooldown = _MaxCooldown(data=reward['global_cooldown'])
+    def __init__(self, reward: rd.Reward) -> None:
+        self.duration: MaxCooldown = MaxCooldown(data=reward['global_cooldown'])
         self._cooldown_expires_at: Optional[str] = reward['cooldown_expires_at']
 
     @property
     def expires_at(self) -> Optional[datetime]:
         if self._cooldown_expires_at:
             return parse_rfc3339_timestamp(timestamp=self._cooldown_expires_at)
         return None
 
 
 class Reward:
     """
     Represents a channel reward.
+
+    :param reward: The reward data.
     """
-    __slots__ = ('id', 'cost', 'status', 'appearance', 'options', 'cooldown',
-                 'redeemed_current_stream')
 
-    def __init__(self, *, reward: rd.Reward) -> None:
+    def __init__(self, reward: rd.Reward) -> None:
         self.id: str = reward['id']
         self.cost: int = reward['cost']
-        self.status: _Status = _Status(reward=reward)
-        self.appearance: _Appearance = _Appearance(reward=reward)
-        self.options: _Options = _Options(reward=reward)
-        self.cooldown: _Cooldown = _Cooldown(reward=reward)
+        self.status: Status = Status(reward=reward)
+        self.appearance: Appearance = Appearance(reward=reward)
+        self.options: Options = Options(reward=reward)
+        self.cooldown: Cooldown = Cooldown(reward=reward)
         self.redeemed_current_stream: Optional[int] = reward['redemptions_redeemed_current_stream']
 
     def __repr__(self) -> str:
         return f'<Reward id={self.id} redeemed_current_stream={self.redeemed_current_stream}>'
 
 
-class _Reward:
+class RewardInfo:
     """
-    Represents a base reward.
+    Represents reward information.
+
+    :param reward: The reward data.
     """
-    __slots__ = ('id', 'title', 'cost', 'description')
 
-    def __init__(self, reward: rd.BaseReward):
+    def __init__(self, reward: rd.BaseReward) -> None:
         self.id: str = reward['id']
         self.title: str = reward['title']
         self.cost: int = reward['cost']
         self.description: str = reward['prompt']
 
     def __repr__(self) -> str:
         return f'<_Reward id={self.id} title={self.title} cost={self.cost}>'
 
 
 class Redemption:
     """
     Represents a reward redemption.
+
+    :param redemption: The redemption data.
     """
-    __slots__ = ('id', 'user', 'status', 'reward', 'redeemed_at')
 
     def __init__(self, redemption: rd.Redemption) -> None:
         self.id: str = redemption['id']
         self.user: User = User(user=redemption)
         self.status: str = redemption['status']
-        self.reward: _Reward = _Reward(reward=redemption['reward'])
+        self.reward: RewardInfo = RewardInfo(reward=redemption['reward'])
         self.redeemed_at: datetime = parse_rfc3339_timestamp(timestamp=redemption['redeemed_at'])
 
     def __repr__(self) -> str:
         return f'<Redemption id={self.id} user={self.user} reward={self.reward.__repr__()}>'
```

### Comparing `twitchify-1.1.1/twitch/state.py` & `twitchify-1.1.2/twitch/state.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/stream.py` & `twitchify-1.1.2/twitch/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub import stream as sm
     from typing import Optional, Union
     from .types import stream as mst
     from datetime import datetime
 
+__all__ = ('Stream', 'Shoutout', 'Online', 'Offline')
+
 
 class Stream:
     """
     Represents a stream.
 
     :param stream: The stream data.
     """
```

### Comparing `twitchify-1.1.1/twitch/survey.py` & `twitchify-1.1.2/twitch/survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 if TYPE_CHECKING:
     from typing import Optional, List, Union, Literal
     from .types.eventsub import prediction as pd
     from .types.eventsub import poll as pl
     from datetime import datetime
 
+__all__ = ('Poll', 'Prediction')
+
 
 class Voting:
     """
     Represents voting settings for a poll.
 
     :param vote: The voting settings for the poll.
     """
```

### Comparing `twitchify-1.1.1/twitch/types/channel.py` & `twitchify-1.1.2/twitch/types/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/channel.py` & `twitchify-1.1.2/twitch/types/eventsub/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/charity.py` & `twitchify-1.1.2/twitch/types/eventsub/charity.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/goal.py` & `twitchify-1.1.2/twitch/types/eventsub/goal.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/hypertrain.py` & `twitchify-1.1.2/twitch/types/eventsub/hypertrain.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/moderation.py` & `twitchify-1.1.2/twitch/types/eventsub/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/poll.py` & `twitchify-1.1.2/twitch/types/eventsub/poll.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/prediction.py` & `twitchify-1.1.2/twitch/types/eventsub/prediction.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/reward.py` & `twitchify-1.1.2/twitch/types/eventsub/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/stream.py` & `twitchify-1.1.2/twitch/types/eventsub/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/subscriptions.py` & `twitchify-1.1.2/twitch/types/eventsub/subscriptions.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/eventsub/user.py` & `twitchify-1.1.2/twitch/types/eventsub/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/gateway.py` & `twitchify-1.1.2/twitch/types/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/http.py` & `twitchify-1.1.2/twitch/types/http.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/message.py` & `twitchify-1.1.2/twitch/types/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/stream.py` & `twitchify-1.1.2/twitch/types/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/types/user.py` & `twitchify-1.1.2/twitch/types/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitch/user.py` & `twitchify-1.1.2/twitch/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,18 +24,23 @@
 
 from __future__ import annotations
 
 from .utils import parse_rfc3339_timestamp
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from .types.eventsub import (channel as chl, user as us, prediction as pd)
+    from .types.eventsub import (channel as chl,
+                                 user as us,
+                                 prediction as pd,
+                                 hypertrain as ht)
     from typing import Optional, Dict, Any
     from datetime import datetime
 
+__all__ = ('User', 'Follower', 'UserUpdate', 'Predictor', 'Contributor')
+
 
 class User:
     """
     Represents a user.
     """
     __slots__ = ('id', 'name', 'display_name')
 
@@ -100,7 +105,24 @@
 
        :return: True if the predictor has won, False otherwise.
        """
         return self._points_won is not None and self.points_won != 0
 
     def __repr__(self) -> str:
         return f'<Predictor user={super().__repr__()} points_won={self.points_won}>'
+
+
+class Contributor:
+    """
+    Represents a Hyper train contributor.
+
+    :param contributor: A dictionary containing contributor information.
+    """
+    __slots__ = ('user', 'type', 'total')
+
+    def __init__(self, contributor: ht.Contributor) -> None:
+        self.user: User = User(user=contributor)
+        self.type: str = contributor['type']
+        self.total: int = contributor['total']
+
+    def __repr__(self) -> str:
+        return f'<_Contributor user={self.user.__repr__()} total={self.total} type={self.type}>'
```

### Comparing `twitchify-1.1.1/twitch/utils.py` & `twitchify-1.1.2/twitch/utils.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.1.1/twitchify.egg-info/PKG-INFO` & `twitchify-1.1.2/twitchify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchify-1.1.1/twitchify.egg-info/SOURCES.txt` & `twitchify-1.1.2/twitchify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

