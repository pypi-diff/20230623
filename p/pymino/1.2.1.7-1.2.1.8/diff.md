# Comparing `tmp/pymino-1.2.1.7.tar.gz` & `tmp/pymino-1.2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\fde\pymino\dist\.tmp-a_jwzy15\pymino-1.2.1.7.tar", last modified: Thu Jun 22 04:18:58 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\fde\pymino\dist\.tmp-b88fet99\pymino-1.2.1.8.tar", last modified: Fri Jun 23 14:09:45 2023, max compression
```

## Comparing `pymino-1.2.1.7.tar` & `pymino-1.2.1.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.698957 pymino-1.2.1.7/
--rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.7/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-06-22 04:18:58.699453 pymino-1.2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.637454 pymino-1.2.1.7/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-22 04:17:43.000000 pymino-1.2.1.7/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/bot.py
--rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.663742 pymino-1.2.1.7/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/account.py
--rw-rw-rw-   0        0        0   343858 2023-06-22 04:17:24.000000 pymino-1.2.1.7/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   342341 2023-06-22 04:17:35.000000 pymino-1.2.1.7/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42101 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.687550 pymino-1.2.1.7/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-06-22 03:04:45.000000 pymino-1.2.1.7/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-06-22 04:13:53.000000 pymino-1.2.1.7/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.697965 pymino-1.2.1.7/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-22 01:21:21.000000 pymino-1.2.1.7/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-22 04:18:58.646408 pymino-1.2.1.7/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 04:18:58.000000 pymino-1.2.1.7/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-22 04:18:58.705406 pymino-1.2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:09:45.834818 pymino-1.2.1.8/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 01:21:21.000000 pymino-1.2.1.8/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-06-23 14:09:45.834818 pymino-1.2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-06-22 01:21:56.000000 pymino-1.2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 14:09:45.767858 pymino-1.2.1.8/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-23 13:55:18.000000 pymino-1.2.1.8/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/bot.py
+-rw-rw-rw-   0        0        0    65900 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:09:45.798610 pymino-1.2.1.8/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    13871 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   343766 2023-06-23 13:53:34.000000 pymino-1.2.1.8/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    19900 2023-06-23 13:18:55.000000 pymino-1.2.1.8/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25389 2023-06-23 14:06:59.000000 pymino-1.2.1.8/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   342510 2023-06-23 13:54:12.000000 pymino-1.2.1.8/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    43801 2023-06-23 14:06:48.000000 pymino-1.2.1.8/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1856 2023-06-23 11:30:38.000000 pymino-1.2.1.8/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:09:45.822913 pymino-1.2.1.8/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-06-22 03:04:45.000000 pymino-1.2.1.8/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-06-22 04:13:53.000000 pymino-1.2.1.8/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6657 2023-06-23 12:31:19.000000 pymino-1.2.1.8/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:09:45.833826 pymino-1.2.1.8/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-06-23 12:42:05.000000 pymino-1.2.1.8/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-22 01:21:21.000000 pymino-1.2.1.8/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10355 2023-06-23 13:30:36.000000 pymino-1.2.1.8/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:09:45.780754 pymino-1.2.1.8/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-06-23 14:09:45.000000 pymino-1.2.1.8/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-06-23 14:09:45.000000 pymino-1.2.1.8/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:09:45.000000 pymino-1.2.1.8/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-23 14:09:45.000000 pymino-1.2.1.8/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 14:09:45.000000 pymino-1.2.1.8/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-23 14:09:45.841266 pymino-1.2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-06-22 01:21:21.000000 pymino-1.2.1.8/setup.py
```

### Comparing `pymino-1.2.1.7/LICENSE` & `pymino-1.2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/PKG-INFO` & `pymino-1.2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.7
+Version: 1.2.1.8
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.7 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.8 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.7/README.md` & `pymino-1.2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/__init__.py` & `pymino-1.2.1.8/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.1.7'
+__version__ = '1.2.1.8'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.2.1.7/pymino/async_bot.py` & `pymino-1.2.1.8/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/bot.py` & `pymino-1.2.1.8/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/client.py` & `pymino-1.2.1.8/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/account.py` & `pymino-1.2.1.8/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/async_community.py` & `pymino-1.2.1.8/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         >>> def my_function(self, comId: str):
         >>>     # Function code
         """
         async def community_func(*args, **kwargs) -> Any:
             if not args[0].userId:
                 raise NotLoggedIn("You are not logged in. Please login before using this function.")
             if not any([args[0].community_id, kwargs.get("comId")]):
-                raise MissingCommunityId("Please provide a community id to the bot before running it or add it to the function call.")
+                raise MissingCommunityId()
             return await func(*args, **kwargs)
         community_func.__annotations__ = func.__annotations__
         return community_func
 
 
     @community
     async def invite_code(self, comId: Union[str, int] = None) -> CommunityInvitation:
```

### Comparing `pymino-1.2.1.7/pymino/ext/async_context.py` & `pymino-1.2.1.8/pymino/ext/async_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,20 @@
     @property
     def api(self) -> str:
         """The API url."""
         return "http://service.aminoapps.com/api/v1"
 
 
     @property
+    def cache(self) -> Cache:
+        """The cache."""
+        return Cache("cache")
+
+
+    @property
     def __message_endpoint__(self) -> str:
         """The message endpoint."""
         return f"/{self.communityId}/s/chat/thread/{self.message.chatId}/message"
 
 
     def _run(func: Callable) -> Callable:
         async def wrapper(*args, **kwargs):
@@ -127,39 +133,76 @@
         return ApiResponse(
             await self.request.handler(
                 method = "DELETE",
                 url = f"/{self.communityId}/s/chat/thread/{self.message.chatId}/message/{delete_message.messageId}"
             ))
 
 
-    async def wait_for_message(self, message: str, timeout: int = 10) -> Message:
+    async def wait_for_message(self, message: str, timeout: int = 10) -> int:
+        """
+        `wait_for_message` - This waits for a specific message within a certain timeout period. 
+        
+        `**Parameters**`
+        - `message` : str
+            The specific message to wait for in the cache.
+        - `timeout` : int, optional
+            The maximum time to wait for the message in seconds. Default is 10.
+        
+        `**Returns**`
+        - `int` 
+            The method returns a status code indicating the result of the operation:
+            200 - If the desired message is found within the timeout.
+            404 - If a different message is found within the timeout.
+            500 - If the timeout is reached without finding the desired message.
+        
+        `**Example**`
+        ```py
+        @bot.on_member_join()
+        async def on_member_join(ctx: Context):
+            if ctx.comId != bot.community.community_id:
+                return
+                
+            TIMEOUT = 15
+
+            await ctx.send(content="Welcome to the chat! Please verify yourself by typing `$verify` in the chat.", delete_after=TIMEOUT)
+
+            response = await ctx.wait_for_message(message="$verify", timeout=15)
+
+            if response == 500:
+                await ctx.send(content="You took too long to verify yourself. You have been kicked from the chat.", delete_after=TIMEOUT)
+                return await bot.community.kick(userId=ctx.author.userId, chatId=ctx.chatId, allowRejoin=True, comId=ctx.comId)
+
+            elif response == 404:
+                return await ctx.send(content="Invalid verification code. You have been kicked from the chat.", delete_after=TIMEOUT)
+
+            else:
+                return await ctx.send(content="You have been verified!", delete_after=TIMEOUT)
+        ```
+        """
         if not self.intents:
             raise IntentsNotEnabled
 
         start = time()
-        cache = Cache("cache")
-
-        while time() - start < timeout:
-            cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
 
-            if cached_message == message:
-                print("Message found!")
-                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
-                return self.message
-
-            if all([cached_message is not None, cached_message != message]):
-                print("Message not found!")
-                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
-                return None
+        with self.cache as cache:
+            while time() - start < timeout:
+                cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
+
+                if cached_message == message:
+                    cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                    return 200
+
+                if all([cached_message is not None, cached_message != message]):
+                    cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                    return 404
 
-            print("No message found!")
-            await asyncio.sleep(0.1)
+                await asyncio.sleep(0.1)
 
-        cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
-        return None
+            cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+            return 500
 
 
     @_run
     async def send(self, content: str, delete_after: int= None, mentioned: Union[str, List[str]]= None) -> CMessage:
         """
         `send` - This sends a message.
```

### Comparing `pymino-1.2.1.7/pymino/ext/async_socket.py` & `pymino-1.2.1.8/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/community.py` & `pymino-1.2.1.8/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,20 +95,26 @@
     ```
 
     """
 
     def __init__(self, bot, session, community_id: Union[str, int] = None) -> None:
         self.bot = bot
         self.session = session
-        self.cache = Cache("cache")
         self.community_id: Union[str, int] = community_id
         self.userId: Optional[str] = None
         if self.userId is None: return
 
 
+    @property
+    def cache(self) -> Cache:
+        """
+        The cache object used by the client.
+        """
+        return self.bot.cache
+
     def community(func: F) -> F:
         """
         A decorator that ensures the user is logged in and a community ID is present before running the decorated function.
 
         :param func: The function to be decorated.
         :type func: Callable
         :raises NotLoggedIn: If the user is not logged in.
@@ -126,18 +132,19 @@
         >>> client.community_id = 123456789
 
         >>> @community
         >>> def my_function(self, comId: str):
         >>>     # Function code
         """
         def community_func(*args, **kwargs) -> Any:
+            
             if not args[0].userId:
                 raise NotLoggedIn("You are not logged in. Please login before using this function.")
             if not any([args[0].community_id, kwargs.get("comId")]):
-                raise MissingCommunityId("Please provide a community id to the bot before running it or add it to the function call.")
+                raise MissingCommunityId()
             return func(*args, **kwargs)
         community_func.__annotations__ = func.__annotations__
         return community_func
 
 
     @community
     def invite_code(self, comId: Union[str, int] = None) -> CommunityInvitation:
@@ -177,26 +184,26 @@
             data = {"duration": 0, "force": True, "timestamp": int(time() * 1000)}
             ))
 
 
     @community
     def fetch_object(
         self,
-        objectId: str,
-        objectType: ObjectTypes = ObjectTypes.USER,
+        object_id: str,
+        object_type: ObjectTypes = ObjectTypes.USER,
         comId: Union[str, int] = None,
         **kwargs
         ) -> LinkInfo:
         """
         Fetches the link information of an object given its ID.
 
-        :param objectId: The ID of the object whose link information is to be fetched.
-        :type objectId: str
-        :param objectType: The type of the object, defaults to ObjectTypes.USER.
-        :type objectType: ObjectTypes, optional
+        :param object_id: The ID of the object whose link information is to be fetched.
+        :type object_id: str
+        :param object_type: The type of the object, defaults to ObjectTypes.USER.
+        :type object_type: ObjectTypes, optional
         :param comId: The ID of the community, defaults to None.
         :type comId: Union[str, int], optional
         :raises NotLoggedIn: If the user is not logged in.
         :raises MissingCommunityId: If the community ID is missing.
         :return: A LinkInfo object containing the link information of the object.
         :rtype: LinkInfo
 
@@ -226,31 +233,33 @@
         - `objectType`: The type of the object.
 
         **Example usage:**
 
         >>> link_info = client.community.fetch_object(objectId="0000-00000-00000-0000", objectType=ObjectTypes.BLOG, comId=123456)
         >>> print(link_info.fullPath)
         """
-        if "object_type" in kwargs: #TODO: Remove this in the near future.
-            objectType = kwargs["object_type"]
-            print("Warning: The 'object_type' parameter is deprecated. Please use 'objectType' instead.")
-
-        KEY = str((objectId, self.community_id if comId is None else comId))
-        if not self.cache.get(KEY):
-            self.cache.set(KEY, self.session.handler(
-                method = "POST",
-                url = f"/g/s-x{self.community_id if comId is None else comId}/link-resolution",
-                data = {
-                    "objectId": objectId,
-                    "targetCode": 1,
-                    "objectType": objectType.value if isinstance(objectType, ObjectTypes) else objectType,
-                    "timestamp": int(time() * 1000)
-                    }
-                ))
-        return LinkInfo(self.cache.get(KEY))
+        if "objectType" in kwargs:
+            object_type = kwargs["objectType"]
+            print("Warning: The 'objectType' parameter is deprecated. Please use 'object_type' instead.")
+
+        KEY = str((object_id, self.community_id if comId is None else comId))
+
+        with self.cache as cache:
+            if not cache.get(KEY):
+                cache.set(KEY, self.session.handler(
+                    method = "POST",
+                    url = f"/g/s-x{self.community_id if comId is None else comId}/link-resolution",
+                    data = {
+                        "objectId": object_id,
+                        "targetCode": 1,
+                        "objectType": object_type.value if isinstance(object_type, ObjectTypes) else object_type,
+                        "timestamp": int(time() * 1000)
+                        }
+                    ))
+            return LinkInfo(cache.get(KEY))
 
 
     def fetch_object_id(self, link: str) -> str:
         """
         Fetches the object ID given a link to the object.
 
         :param link: The link to the object.
@@ -266,20 +275,21 @@
         **Example usage:**
 
         >>> object_id = client.community.fetch_object_id(link="https://aminoapps.com/p/w2Fs6H")
         >>> print(object_id)
         """
 
         KEY = str((link, "OBJECT_ID"))
-        if not self.cache.get(KEY):
-            self.cache.set(KEY, self.session.handler(
-                method = "GET",
-                url = f"/g/s/link-resolution?q={link}"
-                ))
-        return LinkInfo(self.cache.get(KEY)).objectId
+        with self.cache as cache:
+            if not cache.get(KEY):
+                cache.set(KEY, self.session.handler(
+                    method = "GET",
+                    url = f"/g/s/link-resolution?q={link}"
+                    ))
+            return LinkInfo(cache.get(KEY)).objectId
 
 
     def fetch_object_info(self, link: str) -> LinkInfo:
         """
         Fetches information about an object given its link.
 
         :param link: The link to the object.
@@ -310,20 +320,21 @@
         **Example usage:**
 
         >>> object_info = client.community.fetch_object_info(link="https://aminoapps.com/p/w2Fs6H")
         >>> print(object_info.objectId)
         """
 
         KEY = str((link, "OBJECT_INFO"))
-        if not self.cache.get(KEY):
-            self.cache.set(KEY, self.session.handler(
-                method = "GET",
-                url = f"/g/s/link-resolution?q={link}"
-                ))
-        return LinkInfo(self.cache.get(KEY))
+        with self.cache as cache:
+            if not cache.get(KEY):
+                cache.set(KEY, self.session.handler(
+                    method = "GET",
+                    url = f"/g/s/link-resolution?q={link}"
+                    ))
+            return LinkInfo(cache.get(KEY))
 
 
     def fetch_community(self, comId: Union[str, int] = None) -> CCommunity:
         """
         Fetches information about a community given its ID.
 
         :param comId: The ID of the community to fetch. If None, the current community ID is used.
@@ -466,51 +477,51 @@
         """
         return ApiResponse(self.session.handler(
             method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/community/join", 
             data={"timestamp": int(time() * 1000)}
             ))
 
 
-    def fetch_invitationId(self, inviteCode: str, **kwargs) -> str:
+    def fetch_invitationId(self, invite_code: str, **kwargs) -> str:
         """
         Fetches the invitation ID for a given invite code.
 
-        :param inviteCode: The invite code to fetch the invitation ID for.
-        :type inviteCode: str
+        :param invite_code: The invite code to fetch the invitation ID for.
+        :type invite_code: str
         :return: The invitation ID.
         :rtype: str
 
         The function sends a GET request to the API with the invite code as a parameter.
 
         `InvitationId`:
 
         - `invitationId`: The ID of the invitation.
 
         **Example usage:**
 
         >>> invitation_id = client.fetch_invitationId(invite_code="ABCD1234")
         >>> print(invitation_id)
         """
-        if "invite_code" in kwargs: #TODO: Remove this in the near future.
-            inviteCode = kwargs["invite_code"]
-            print("The 'invite_code' parameter has been deprecated. Please use 'inviteCode' instead.")
+        if "inviteCode" in kwargs: #TODO: Remove this in the near future.
+            inviteCode = kwargs["inviteCode"]
+            print("The 'inviteCode' parameter has been deprecated. Please use 'invite_code' instead.")
 
         return InvitationId(self.session.handler(
             method = "GET",
             url = f"/g/s/community/link-identify?q={inviteCode}"
             )).invitationId
 
 
     @community
-    def join_community_by_code(self, inviteCode: str, comId: Union[str, int] = None, **kwargs) -> ApiResponse:
+    def join_community_by_code(self, invite_code: str, comId: Union[str, int] = None, **kwargs) -> ApiResponse:
         """
         Joins a community using the invite code.
 
-        :param inviteCode: The invite code of the community.
-        :type inviteCode: str
+        :param invite_code: The invite code of the community.
+        :type invite_code: str
         :param comId: The ID of the community to join. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
         :return: An ApiResponse object containing the API response data.
         :rtype: ApiResponse
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
@@ -528,23 +539,23 @@
 
         **Example usage:**
 
         >>> api_response = client.community.join_community_by_code(invite_code="ABC123")
         >>> if api_response.statuscode == 0:
         ...     print("Joined community successfully!")
         """
-        if "invite_code" in kwargs: #TODO: Remove this in the near future.
-            inviteCode = kwargs["invite_code"]
-            print("The 'invite_code' parameter has been deprecated. Please use 'inviteCode' instead.")
+        if "inviteCode" in kwargs: #TODO: Remove this in the near future.
+            invite_code = kwargs["inviteCode"]
+            print("The 'inviteCode' parameter has been deprecated. Please use 'invite_code' instead.")
 
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/community/join",
             data = {
-                "invitationId": self.fetch_invitationId(inviteCode=inviteCode),
+                "invitationId": self.fetch_invitationId(inviteCode=invite_code),
                 "timestamp": int(time() * 1000)
                 }
             ))
 
 
     @community
     def leave_community(self, comId: Union[str, int] = None) -> ApiResponse:
```

### Comparing `pymino-1.2.1.7/pymino/ext/console.py` & `pymino-1.2.1.8/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/dispatcher.py` & `pymino-1.2.1.8/pymino/ext/dispatcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Callable
-
+from threading import Thread
 
 class MessageDispatcher:
     """
     `MessageDispatcher` - Simple message dispatcher that allows you to register handlers for specific message types.
  
     `**Example**`
 
@@ -25,16 +25,18 @@
 
     def register(self, message_type: int, handler: Callable):
         self.dispatch_table[message_type] = handler
 
     def handle(self, message: dict):
         message_type = message.get("t")
         if message_type not in self.dispatch_table:
-            return
-        self.dispatch_table[message_type](message)
+            return None
+        return Thread(
+            target=self.dispatch_table[message_type],args=(message,)
+            ).start()
 
 
 class AsyncMessageDispatcher:
     """
     `AsyncMessageDispatcher` - Simple async message dispatcher that allows you to register handlers for specific message types.
  
     `**Example**`
```

### Comparing `pymino-1.2.1.7/pymino/ext/entities/acm.py` & `pymino-1.2.1.8/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/admin_log.py` & `pymino-1.2.1.8/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/api_response.py` & `pymino-1.2.1.8/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/bubble.py` & `pymino-1.2.1.8/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/chat_threads.py` & `pymino-1.2.1.8/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/comments.py` & `pymino-1.2.1.8/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/enums.py` & `pymino-1.2.1.8/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/exceptions.py` & `pymino-1.2.1.8/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/general.py` & `pymino-1.2.1.8/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/handlers.py` & `pymino-1.2.1.8/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/link_info.py` & `pymino-1.2.1.8/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/member.py` & `pymino-1.2.1.8/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/messages.py` & `pymino-1.2.1.8/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/notification.py` & `pymino-1.2.1.8/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/sticker.py` & `pymino-1.2.1.8/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/threads.py` & `pymino-1.2.1.8/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/userprofile.py` & `pymino-1.2.1.8/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/entities/wsevents.py` & `pymino-1.2.1.8/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/handle_queue.py` & `pymino-1.2.1.8/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/socket.py` & `pymino-1.2.1.8/pymino/ext/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,23 +106,22 @@
         if self.userId == _message.userId: return None
         None if any(
             [_message.ndcId is None, _message.ndcId == 0]
         ) else self._communities.add(_message.ndcId)
 
         key = self.event_types.get(f"{_message.type}:{_message.mediaType}")
         if key != None:
-            return Thread(target=self._handle_event, args=(key, _message)).start()
+            return self._handle_event(key, _message)
 
 
     def _handle_notification(self, message: dict) -> None:
         """Handles notifications."""
         notification: Notification = Notification(message)
         key = self.notif_types.get(notification.notification_type)
-        if key != None:
-            return Thread(target=self._handle_event, args=(key, notification)).start()
+        return self._handle_event(key, notification) if key else None
 
 
     def _handle_agora_channel(self, message: dict) -> None:
         """Sets the agora channel."""
         self.channel: Channel = Channel(message)
```

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.1.8/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/chat_console.py` & `pymino-1.2.1.8/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/commands.py` & `pymino-1.2.1.8/pymino/ext/utilities/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from time import time
 from typing import Callable
+from collections import defaultdict
+
 
 class Command:
     """
     `Command` - The main command class.
     
     `**Parameters**`
     - `func` - The function to run when the command is called.
@@ -18,120 +20,133 @@
         self.func:           Callable = func
         self.name:           str = name
         self.description:    str = description
         self.usage:          str = usage
         self.aliases:        list = [] if aliases is None else aliases
         self.cooldown:       int = cooldown
 
+
 class Commands:
     def __init__(self):
-        self.commands: list[Command] = []
-        self.cooldowns: dict = {}
+        self.commands: dict[str, Command] = {}
+        self.cooldowns: defaultdict[dict] = defaultdict(dict)
+
 
     def add_command(self, command: Command) -> Command:
         """
         `add_command` - Adds a command to the command list.
         
         `**Parameters**`
         - `command` - The command to add.
         
         `**Returns**`
         - `Command` - The command that was added.
         
         """
-        self.commands.append(command)
+        self.commands[command.name] = command
         return command
 
+
     def fetch_command(self, command_name: str) -> Command:
         """
         `fetch_command` - Fetches a command from the command list.
         
         `**Parameters**`
         - `command_name` - The name of the command to fetch.
         
         `**Returns**`
         - `Command` - The command that was fetched.
         
         """
-        return next((command for command in self.commands if command.name == command_name or command_name in command.aliases), None)
+        return self.commands.get(command_name) or next(
+            (command for command in self.commands.values() if command_name in command.aliases), None
+        )
+
 
     def fetch_commands(self) -> Command:
         """
         `fetch_commands` - Fetches all commands from the command list.
         
         `**Returns**`
         - `list[Command]` - The commands that were fetched.
         
         """
-        return self.commands
+        return list(self.commands.values())
+
 
     def __command_functions__(self) -> list:
         """
         `__command_functions__` - Fetches all command functions from the command list.
         
         `**Returns**`
         - `list[Callable]` - The command functions that were fetched.
         
         """
         return {command.name: command.func for command in self.commands}
 
+
     def __command_names__(self) -> list:
         """
         `__command_names__` - Fetches all command names from the command list.
         
         `**Returns**`
         - `list[str]` - The command names that were fetched.
         
         """
-        return [command.name for command in self.commands]
+        return [command.name for command in self.commands.values()]
+
 
     def __command_aliases__(self) -> list:
         """
         `__command_aliases__` - Fetches all command aliases from the command list.
         
         `**Returns**`
         - `list[str]` - The command aliases that were fetched.
         
         """
         aliases = {}
-        for command in self.commands:
+        for command in self.commands.values():
             for alias in command.aliases:
                 aliases[alias] = command.name
         return aliases
 
+
     def __command_descriptions__(self) -> list:
         """
         `__command_descriptions__` - Fetches all command descriptions from the command list.
         
         `**Returns**`
         - `list[str]` - The command descriptions that were fetched.
         
         """
         return {command.name: command.description for command in self.commands}
-    
+
+
     def __command_usages__(self) -> list:
         """
         `__command_usages__` - Fetches all command usages from the command list.
         
         `**Returns**`
         - `list[str]` - The command usages that were fetched.
         
         """
         return {command.name: command.usage for command in self.commands}
 
+
     def __command_cooldowns__(self) -> list:
         """
         `__command_cooldowns__` - Fetches all command cooldowns from the command list.
         
         `**Returns**`
         - `list[int]` - The command cooldowns that were fetched.
         
         """
         return {command.name: command.cooldown for command in self.commands}
 
+
     def set_cooldown(self, command_name: str, cooldown: int, userId: str) -> None:
         """
         `set_cooldown` - Sets the cooldown of a command for a user.
         
         `**Parameters**`
         - `command_name` - The name of the command to set the cooldown for.
         - `cooldown` - The cooldown to set.
@@ -139,43 +154,38 @@
         
         `**Returns**`
         - `None` - Nothing.
 
         """
         self.cooldowns[command_name][userId] = time() + cooldown
 
+
     def fetch_cooldown(self, command_name: str, userId: str) -> int:
         """
         `fetch_cooldown` - Fetches the cooldown of a command for a user.
         
         `**Parameters**`
         - `command_name` - The name of the command to fetch the cooldown for.
         - `userId` - The user to fetch the cooldown for.
         
         `**Returns**`
         - `int` - The cooldown that was fetched.
         
         """
-        if command_name not in self.cooldowns:
-            self.cooldowns[command_name] = {}
-        if userId not in self.cooldowns[command_name]:
-            self.cooldowns[command_name][userId] = 0
+        self.cooldowns[command_name].setdefault(userId, 0)
         return self.cooldowns[command_name][userId]
 
+
     def __help__(self):
         """
         `__help__` - Generates a help message for the bot.
         
         `**Returns**`
         - `str` - The help message that was generated.
         
         """
         help_message = "[bcu]Commands\n" + "\n[ic]This is a list of all the commands available on this bot.\n"
 
-        for command in self.commands:
+        for command in self.commands.values():
             help_message += f"\n[uc]{command.name}\n[ic]{command.description}\n[uc]Usage: {command.usage}\n"
         help_message += "\n\n[ic]This message was generated automatically. If you have any questions, please contact the bot owner."
-        return help_message
-
-    def __repr__(self):
-        """`__repr__` - Generates a string representation of the commands."""
-        return f"Commands({self.commands})"
+        return help_message
```

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/community_console.py` & `pymino-1.2.1.8/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/generate.py` & `pymino-1.2.1.8/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/menu.py` & `pymino-1.2.1.8/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/profile_console.py` & `pymino-1.2.1.8/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/pymino/ext/utilities/request_handler.py` & `pymino-1.2.1.8/pymino/ext/utilities/request_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from time import sleep
 from uuid import uuid4
 from ujson import loads, dumps
 from colorama import Fore, Style
 from typing import Optional, Union, Tuple, Callable
 
 from ..entities.handlers import orjson_exists
 from .generate import device_id, generate_signature
@@ -119,24 +120,25 @@
         
         `**Returns**``
         - `Union[int, str]` - The status code and response from the request.
         
         """
         try:
             response: HttpResponse = self.fetch_request(method)(
-                url, data=data, headers=headers, proxies=self.proxy
+                url, data=data, headers=headers, proxies=self.proxy, timeout=10 if self.proxy else 2
             )
             return response.status_code, response.text
         except (
             ConnectionError,
             ReadTimeout,
             SSLError,
             ProxyError,
             ConnectTimeout,
         ):
+            sleep(1.5)
             self.handler(method, url, data, content_type)
     
     def handler(
         self,
         method: str,
         url: str,
         data: Union[dict, bytes, None] = None,
```

### Comparing `pymino-1.2.1.7/pymino.egg-info/PKG-INFO` & `pymino-1.2.1.8/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.1.7
+Version: 1.2.1.8
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.1.7 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.8 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.1.7/pymino.egg-info/SOURCES.txt` & `pymino-1.2.1.8/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.1.7/setup.cfg` & `pymino-1.2.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e31 2e37 0d0a 6175  on = 1.2.1.7..au
+00000020: 6f6e 203d 2031 2e32 2e31 2e38 0d0a 6175  on = 1.2.1.8..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.1.7/setup.py` & `pymino-1.2.1.8/setup.py`

 * *Files identical despite different names*

