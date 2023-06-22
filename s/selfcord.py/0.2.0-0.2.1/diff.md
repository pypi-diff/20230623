# Comparing `tmp/selfcord.py-0.2.0.tar.gz` & `tmp/selfcord.py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.2.0.tar", last modified: Fri Jun 16 16:12:03 2023, max compression
+gzip compressed data, was "selfcord.py-0.2.1.tar", last modified: Thu Jun 22 22:39:40 2023, max compression
```

## Comparing `selfcord.py-0.2.0.tar` & `selfcord.py-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/selfcord/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 16:12:03.000000 selfcord.py-0.2.0/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:12:03.747854 selfcord.py-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-16 16:11:50.000000 selfcord.py-0.2.0/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-22 22:39:26.000000 selfcord.py-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26478 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/tests/test_commands.py
```

### Comparing `selfcord.py-0.2.0/PKG-INFO` & `selfcord.py-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -15,15 +15,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.0-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.1-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.0 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.1 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.0-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.1-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.0/README.md` & `selfcord.py-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.0-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.1-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.0-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.1-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.0/selfcord/api/errors.py` & `selfcord.py-0.2.1/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.0/selfcord/api/events.py` & `selfcord.py-0.2.1/selfcord/api/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,33 +3,27 @@
 import asyncio
 import time
 from time import perf_counter
 from typing import TYPE_CHECKING
 
 from aioconsole import aprint
 
-from ..models import (
-    Client,
-    DMChannel,
-    GroupChannel,
-    Guild,
-    Message,
-    TextChannel,
-    User,
-    VoiceChannel,
-)
+from selfcord.models.sessions import Event_Session
+
+from ..models import (Client, DMChannel, GroupChannel, Guild, Message,
+                      TextChannel, User, VoiceChannel)
 from ..models.role import Role
 from ..utils import logging
 from .voice import Voice
 
 if TYPE_CHECKING:
     from ..bot import Bot
     from .http import http
 
-log = logging.getLogger("Event")
+log = logging.getLogger(__name__)
 
 
 class EventHandler:
     """
     Used to handle discord events
     """
 
@@ -274,15 +268,15 @@
             for guild in self.user.guilds:
                 for channel in guild.channels:
                     if channel.id == id:
                         await self.bot.emit("channel_delete", channel)
                         guild.channels.remove(channel)
                         return
 
-    async def handle_guild_role_create(self, role, user: Client, http: http):
+    async def handle_guild_role_create(self, role: dict, user: Client, http: http):
         """Handles what happens when a role is created
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
@@ -419,7 +413,66 @@
         asyncio.create_task(voice.start())
         setattr(self.bot, "voice", self.voice)
         if self.debug:
             log.debug("Voice attribute created")
             log.info(
                 f"Created voice attribute with Session ID: {self.session_id} Endpoint: {self.endpoint}"
             )
+
+    async def handle_relationship_add(self, data: dict, user: Client, http: http):
+        """Handles relationships being added
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
+        types = {
+            "NONE": 0,
+            "FRIEND": 1,
+            "BLOCKED": 2,
+            "PENDING_INCOMING": 3,
+            "PENDING_OUTGOING": 4,
+        }
+        user = User(data.get("user"), self.bot, self.http)
+        since = data.get("since")
+        for type, value in types.items():
+            if data.get("type") == value:
+                rs_type = type
+        await self.bot.emit("relationship_add", user, rs_type, since)
+    
+    async def handle_sessions_replace(self, data: list[dict], user: Client, http: http):
+        """Handles sessions being created/removed. Used to log initial data.
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
+    
+        sessions = [Event_Session(session, self.bot, self.http) for session in data]
+        await self.bot.emit("session", sessions)
+        
+
+
+    async def handle_relationship_remove(self, data: dict, user: Client, http: http):
+        """Handles relationships being removed
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
+        types = {
+            "NONE": 0,
+            "FRIEND": 1,
+            "BLOCKED": 2,
+            "PENDING_INCOMING": 3,
+            "PENDING_OUTGOING": 4,
+        }
+
+        id = data['id']
+        since = data['since']
+        for type, value in types.items():
+            if data.get("type") == value:
+                rs_type = type
+        await self.bot.emit("relationship_remove", id, rs_type, since)
```

### Comparing `selfcord.py-0.2.0/selfcord/api/gateway.py` & `selfcord.py-0.2.1/selfcord/api/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import asyncio
-import json
 import os
 import time
 import zlib
 from traceback import format_exception
 
 import requests
+import ujson
 import websockets
 
 from selfcord.models.client import Client
 
 from ..utils import logging
 from .errors import ReconnectWebsocket
 from .events import EventHandler
 
-log = logging.getLogger("Gateway")
+log = logging.getLogger(__name__)
 
 
 class Activity:
     @staticmethod
     def Game(
         name: str,
         details: str,
@@ -333,15 +333,15 @@
         if item:
             if self.fired:
                 log.info(f"{item}")
             try:
                 item = self.zlib.decompress(item)
             except Exception as e:
                 log.error(f"Could not decompress\n{e}")
-            item = json.loads(item)  # Get json message from gateway
+            item = ujson.loads(item)  # Get json message from gateway
 
             op = item.get("op")  # Op code
             data = item.get("d")  # Data
             event = item.get("t")  # The event
             s = item.get("s")
             if op == self.RECONNECT:
                 await self.close()
@@ -377,16 +377,17 @@
                     val = await asyncio.gather(
                         asyncio.create_task(method(data, self.user, self.http)),
                         return_exceptions=True,
                     )  # A background task is created to run the handler
                     for item in val:
                         if item is None:
                             break
-                        else:
-                            await self.bot.emit("error", item)
+                        error = "".join(format_exception(item, item, item.__traceback__))
+                        log.error(f"Error occurred when handling events\n {error}")
+                        await self.bot.emit("error", item)
 
                     # asyncio.create_task(method(data, self.user, self.http))
                 # Handlers are all situated in events.py
 
     def roundup(self, n):
         import math
 
@@ -458,15 +459,15 @@
 
     async def send_json(self, payload: dict):
         """Send json to the gateway
 
         Args:
             payload (dict): Valid payload to send to the gateway
         """
-        await self.ws.send(json.dumps(payload))
+        await self.ws.send(ujson.dumps(payload))
 
     async def reconnect(self, seq: int):
         """Reconnect to discord gateway"""
         self.ws = await websockets.connect(
             f"{self.bot.resume_url}?encoding=json&v=9&compress=zlib-stream"
         )
         self.alive = True
@@ -516,15 +517,15 @@
 
     async def heartbeat(self, interval):
         """Heartbeat for gateway to maintain connection
 
         Args:
             interval (int): Interval between sends
         """
-        log.info(f"Hearbeat loop has began with the interval of {interval} seconds!")
+        log.info(f"Heartbeat loop has begun with the interval of {interval} seconds!")
         heartbeatJSON = {"op": 1, "d": time.time()}
         while True:
             await asyncio.sleep(interval)
             await self.send_json(heartbeatJSON)
             self.last_send = time.perf_counter()
             if self.debug:
                 log.debug("Sent heartbeat")
```

### Comparing `selfcord.py-0.2.0/selfcord/api/http.py` & `selfcord.py-0.2.1/selfcord/api/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 import asyncio
 import random
 from base64 import b64encode
 from traceback import format_exception
 from typing import TYPE_CHECKING
 
 import aiohttp
+import ujson
 from aiohttp import ClientSession
 
 from ..models import Client, User
 from ..utils import logging
 
-log = logging.getLogger("HTTP")
+lib, _, _ = __name__.partition(".")
+log = logging.getLogger(__name__)
 
 
 class http:
     """Base HTTP class to aid making requests via discord api"""
 
     def __init__(self, debug=False) -> None:
         self.debug = debug
@@ -46,15 +48,15 @@
         if self.debug:
             log.debug("Finished Static login")
             log.info(f"Gathered information on {self.client}")
         return data
 
     async def get_cookie(self):
         """Gather cookie for user upon client start"""
-        async with aiohttp.ClientSession() as session:
+        async with aiohttp.ClientSession(json_serialize=ujson.dumps) as session:
             async with session.get(
                 "https://discord.com",
                 headers={
                     "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36"
                 },
             ) as resp:
                 dcf = resp.headers["set-cookie"].split("__dcfduid=")[0].split(";")[0]
@@ -112,14 +114,15 @@
             "x-debug-options": "logGatewayEvents,logOverlayEvents,logAnalyticsEvents,bugReporterEnabled",
             "x-fingerprint": self.fingerprint,
             "x-discord-timezone": "Europe/London",
             "TE": "trailers",
         }
 
         async with ClientSession(
+            json_serialize=ujson.dumps,
             timeout=aiohttp.ClientTimeout(
                 total=10000, connect=10000, sock_read=10000, sock_connect=10000
             ),
             connector=aiohttp.TCPConnector(
                 limit=0, limit_per_host=0, ttl_dns_cache=300
             ),
             headers=headers,
@@ -142,29 +145,29 @@
                             text = await resp.text()
                             log.error(f"Error upon parsing json : {text}")
                             if self.debug:
                                 log.error(f"Error upon parsing json : \n{error}")
                                 log.info(
                                     f"Attempted to send request to URL: {url} PAYLOAD: {kwargs}"
                                 )
-                            break
+                            raise Exception(e) from e
 
                     elif resp.status == 401:
                         json = await resp.json()
                         log.error(f"{json} -- {resp.status}")
-                        break
+                        raise Exception(f"{json}")
 
                     elif resp.status == 403:
                         json = await resp.json()
                         log.error(f"403 Unauthorized: {json}")
                         if self.debug:
                             log.info(
                                 f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
                             )
-                        break
+                        raise Exception(f"{json}")
 
                     elif resp.status == 201:
                         data = await resp.json()
                         break
 
                     elif resp.status == 204:
                         data = await resp.text()
@@ -178,27 +181,19 @@
                         if self.debug:
                             log.error(f"Unknown Error: {resp.status}")
                             log.info(
                                 f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
                             )
                         try:
                             json = await resp.json()
-                            log.error(f"Error Response: {json}")
-                            break
+                            raise Exception(f"{json}")
                         except Exception as e:
                             error = "".join(format_exception(e, e, e.__traceback__))
                             log.error(f"Unable to log response: \n{error}")
-                            break
-                        try:
-                            text = await resp.text()
-                            log.error(f"{text} -- {resp.status}")
-                            break
-                        except:
-                            log.error(f"{resp.status}")
-                            break
+                            raise Exception(e) from e
         try:
             if resp.headers["set-cookie"]:
                 dcf = resp.headers["set-cookie"].split("__dcfduid=")[0].split(";")[0]
                 sdc = resp.headers["set-cookie"].split("__sdcfduid=")[0].split(";")[0]
                 cfr = resp.headers["set-cookie"].split("__cfruid=")[0].split(";")[0]
                 bm = resp.headers["set-cookie"].split("__cf_bm=")[0].split(";")[0]
```

### Comparing `selfcord.py-0.2.0/selfcord/api/voice/voice.py` & `selfcord.py-0.2.1/selfcord/api/voice/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
-import json
 import socket
 import struct
 import time
 
+import ujson
 import websockets
 from aioconsole import aprint
 
 try:
     import nacl.secret
     import nacl.utils
     import opuslib
@@ -26,15 +26,15 @@
 from ...utils import logging
 
 if TYPE_CHECKING:
     from ...api import http
     from ...bot import Bot
 
 
-log = logging.getLogger("Voice")
+log = logging.getLogger(__name__)
 
 
 class Voice:
     """Voice class used to interact with voice websockets and send data"""
 
     SAMPLING_RATE = 48000
     CHANNELS = 2
@@ -76,15 +76,15 @@
         )
         self.alive = True
 
     async def recv_msg(self):
         """
         Receives Message from websocket, encodes as json and runs tasks
         """
-        item = json.loads(await self.ws.recv())
+        item = ujson.loads(await self.ws.recv())
         op = item.get("op")  # Op code
         data = item.get("d")  # Data
         if op == self.READY:
             await self.handle_ready(data)
 
         elif op == self.HEARTBEAT:
             asyncio.create_task(self.heartbeat(data))
@@ -207,15 +207,15 @@
         await self.send_json(payload)
 
     async def send_json(self, payload: dict):
         """Send json to the websocket
         Args:
             payload (dict): Valid payload to send to the gateway
         """
-        await self.ws.send(json.dumps(payload))
+        await self.ws.send(ujson.dumps(payload))
 
     async def close(self):
         """Close the connection to websocket"""
         self.alive = False
         await self.ws.close()
 
     async def identify(self):
```

### Comparing `selfcord.py-0.2.0/selfcord/bot.py` & `selfcord.py-0.2.1/selfcord/bot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import importlib
 import inspect
 import io
+import os
 import random
 import time
 from collections import defaultdict
 from traceback import format_exception
 from typing import TYPE_CHECKING
+from urllib.parse import urlparse
 
+import aiofiles
 import aiohttp
-from aioconsole import aexec
+from aioconsole import aexec, aprint
+
+from selfcord.models.sessions import Session
 
 from .api import Activity, gateway, http
 from .models import (Client, DMChannel, GroupChannel, Guild, InteractionUtil,
-                     Option, Search, SlashCommand, TextChannel, User,
+                     Message, Option, Search, SlashCommand, TextChannel, User,
                      VoiceChannel)
 from .utils import (Command, CommandCollection, Context, Event, Extension,
                     ExtensionCollection, logging)
+from .utils.logging import handler
 
 if TYPE_CHECKING:
     from .api.gateway import gateway
     from .api.http import http
 
-log = logging.getLogger("Bot")
+log = logging.getLogger(__name__)
 
 
 class Bot:
     """Bot instance as entry point to interact with the bot
 
     Args:
         debug (bool): Whether to start the bot in debug mode, defaults to False.
@@ -60,33 +66,45 @@
         self.prefixes: list[str] = (
             prefixes if isinstance(prefixes, list) else [prefixes]
         )
         self.extensions = ExtensionCollection()
         self.user = None
         self.eval: bool = eval
         self.userbot: bool = userbot
-
+        if self.debug:
+            logging.basicConfig(
+                level=logging.DEBUG,
+                handlers=[handler],
+            )
     def run(self, token: str):
         """Used to start connection to gateway as well as gather user information
 
         Args:
             token (str): _description_
         """
         self.token = token
 
         async def runner():
             data = await self.http.static_login(token)
             self.user = Client(data)
-            await self.gateway.start(token, self.user, self)
+            try:
+                await self.gateway.start(token, self.user, self)
+            except Exception as e:
+                error = "".join(format_exception(e, e, e.__traceback__))
+                log.error(f"Error related to gateway\n{error}")
             if self.debug:
-                log.debug("Started Bot")
+                log.info("Started Bot")
                 log.info(f"Logged in as {self.user}")
 
-        with contextlib.suppress(KeyboardInterrupt):
+        try: 
             asyncio.run(runner())
+        except Exception as e:
+            error = format_exception(e, e, e.__traceback__)
+            log.error(f"Error related to initial run\n{error}")
+            return 
 
     @property
     def latency(self):
         """Latency of heartbeat ack, gateway latency essentially"""
         return self.gateway.latency
 
     # For events
@@ -174,15 +192,14 @@
                 else:
                     return content
 
             @self.cmd(description="Executes and runs code", aliases=["exec"])
             async def eval(ctx, *, code):
                 """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution."""
                 code = clean_code(code)
-
                 try:
                     with contextlib.redirect_stdout(io.StringIO()) as f:
                         await aexec(source=code, local=globals() )
                         result = f"```{f.getvalue()}\n```"
                 except Exception as e:
                     error = "".join(format_exception(e, e, e.__traceback__))
                     result = f"```\n{error}```"
@@ -195,14 +212,15 @@
         Args:
             event (str): The event to check for
         """
 
         def decorator(coro):
             if not inspect.iscoroutinefunction(coro):
                 log.error("Not a coroutine")
+                raise Exception("Not a coroutine")
             else:
                 self._events[event].append(Event(name=event, coro=coro, ext=None))
 
                 def wrapper(*args, **kwargs):
                     result = self._events[event].append(
                         Event(name=event, coro=coro, ext=None)
                     )
@@ -245,14 +263,16 @@
         if isinstance(aliases, str):
             aliases = [aliases]
 
         def decorator(coro):
             name = coro.__name__
             if not inspect.iscoroutinefunction(coro):
                 log.error("Not a coroutine")
+                raise Exception("Not a coroutine")
+                return
             else:
                 cmd = Command(
                     name=name, description=description, aliases=aliases, func=coro
                 )
                 self.commands.add(cmd)
             return cmd
 
@@ -271,14 +291,16 @@
             RuntimeWarning: If you suck and don't use a coroutine
         """
         if isinstance(aliases, str):
             aliases = [aliases]
         name = coro.__name__
         if not inspect.iscoroutinefunction(coro):
             log.error("Not a coroutine")
+            raise Exception("Not a coroutine")
+
         else:
             cmd = Command(
                 name=name, description=description, aliases=aliases, func=coro
             )
             self.commands.add(cmd)
 
     async def process_commands(self, msg):
@@ -288,44 +310,97 @@
         Args:
             msg (str): The message containing command
         """
         context = Context(self, msg, self.http)
 
         asyncio.create_task(context.invoke())
 
-    async def load_extension(self, name: str):
+    async def load_extension(self, name: str | None = None, url: str | None = None, dir: str | None = None):
         """
         Load various extensions/plugins/cogs if any.
 
         Args:
             name (str): Name of the extension to load
+            url (str): URL you want to load
+            dir (str): Directory you want to load
 
         Raises:
             ModuleNotFoundError: If you suck and don't know the name of what you want to load
         """
+        if name is None and url is None:
+            return
+        if url is not None:
+            async with aiohttp.ClientSession() as session:
+                async with session.get(url) as resp:
+                    text = await resp.text()
+
+            if dir is None:
+                path = os.path.basename(urlparse(url).path)
+
+                if path.endswith(".py"):
+                    if os.path.exists(path):
+                        log.error(f"Path already exists. {path}")
+                        return
+
+                    lines = text.splitlines()
+                    async with aiofiles.open(path, "a+") as f:
+                        for line in lines:
+                            await f.write(f"{line}\n")
+
+                    name = f"{os.path.basename(urlparse(url).path)[:-3]}"
+
+                else:
+                    log.error(f"{path} is not a python file")
+                    return
+
+            else:
+                path = f"{dir}/{os.path.basename(urlparse(url).path)}"
+                
+                if path.endswith(".py"):
+                    if os.path.exists(path):
+                        log.error(f"Path already exists. {path}")
+                        return
+                    if not os.path.exists(dir):
+                        os.makedirs(dir)
+                    lines = text.splitlines()
+                    async with aiofiles.open(path, "a+") as f:
+                        for line in lines:
+                            await f.write(f"{line}\n")
+
+                    name = f"{dir}.{os.path.basename(urlparse(url).path)[:-3]}"
+
+                else:
+                    log.error(f"{path} is not a python file")
+                    return
+
+                
+                
         try:
             name = importlib.util.resolve_name(name, None)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not resolve extension name\n{error}")
+            return
 
         spec = importlib.util.find_spec(name)
 
         lib = importlib.util.module_from_spec(spec)
 
         try:
             spec.loader.exec_module(lib)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Spec could not be loaded\n{error}")
+            return
         try:
             ext = getattr(lib, "Ext")
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Extension does not exist\n{error}")
+            return
 
         # Creates an Extension - ext in this case refers to the Ext class used for initialisation
         ext = Extension(
             name=ext.name,
             description=ext.description,
             ext=ext(self),
             _events=ext._events,
@@ -340,14 +415,18 @@
             if self.debug:
                 log.debug("Loaded Extension")
                 log.info(f"Loaded Extension {ext.name} to Bot")
 
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Failed to load extension events\n{error}")
+            return
+
+    async def logout(self):
+        await self.gateway.close()
 
     async def trigger_slash(
         self,
         command: SlashCommand,
         channel_id: str,
         bot_id: str,
         value: list[str | None] | None = None,
@@ -380,14 +459,28 @@
         Returns:
             Search object
         """
         interaction = InteractionUtil(self, self.http)
         return await interaction.interaction_search(
             query, channel_id, type, cursor, bot_id, command_id
         )
+    
+    def get_message(self, message_id: str):
+        """
+        Function to help retrieve messages from bot cache
+
+        Args:
+            message_id (str): The message id to search for
+
+        Returns:
+            Message: The Message object
+        """
+        for message in self.user.messages:
+            if message.id == message_id:
+                return Message
 
     def get_channel(self, channel_id: str):
         """
         Function to help retrieve channel from bot cache
 
         Args:
             channel_id (str): The channel id to search for
@@ -450,14 +543,29 @@
         if self.debug:
             log.debug("Finished Creating Guild")
             log.info(
                 f"Created Guild NAME: {name} TEMPLATE: {template} ICON: {icon_url}"
             )
         return Guild(json, self, self.http)
 
+    async def change_pass(self, old_pass, new_pass):
+        """
+        Method to change password.
+
+        Args:
+            old_pass: Your old password.
+            new_pass: Password you want to change to.
+        """
+        await self.http.request("patch", "/users/@me", json={"password": old_pass, "new_password": new_pass})
+    
+    async def get_sessions(self) -> list[Session] | None:
+        data = await self.http.request("get", "/auth/sessions")
+        if data.get("user_sessions") is not None:
+            return [Session(data, self, self.http) for data in data["user_sessions"]]
+
     async def add_friend(self, user_id: str):
         """
         Function to add a specific user as a friend.
 
         Args:
             user_id (str): ID of the possible random user.
```

### Comparing `selfcord.py-0.2.0/selfcord/models/channel.py` & `selfcord.py-0.2.1/selfcord/models/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,102 @@
 from __future__ import annotations
 
 import asyncio
 import os
 import random
+import time
 from traceback import format_exception
 from typing import TYPE_CHECKING
 
 import aiofiles
 import aiohttp
+from aioconsole import aprint
 
 from ..utils import logging
 from .message import Message
 from .user import User
 from .webhook import Webhook
 
 if TYPE_CHECKING:
     from ..api.http import http
     from ..bot import Bot
     from ..models.permission import Permission
 
-log = logging.getLogger("Channel")
+log = logging.getLogger(__name__)
 
 
 class Messageable:
     """Parent class specific for those classes that include a textchat for sending messages."""
 
     def __init__(self, http: http, bot: Bot) -> None:
         self.http: http = http
         self.bot: Bot = bot
 
     @property
     def make_nonce(self):
         """Generate pseudorandom number."""
         return str(random.randint(0, 100000000))
 
-    async def history(self, amount: int = 100) -> list[Message] | None:
+    async def search(
+        self,
+        content: str | None = None,
+        author: str | None = None,
+        mentions: str | None = None,
+        has: str | None = None,
+        before: float | None = None,
+        after: float | None = None,
+        offset: int | None = None,
+        ):
+        """
+        Search through channel with specific parameters
+
+        Args:
+            content (str) : Content to search for.
+            author (str) : Author to search for.
+            mentions (str) : Mention to search for.
+            has (str) : Message that contains (file, image, video, etc).
+            before (time) : Before a timestamp.
+            after (time) : After a timestamp.
+            offset (int) : How many messages after to search.
+
+        Returns:
+            total (int) : Total amount of messages possible of receiving.
+            messages (list[Message]) : List of message objects gathered
+
+        """
+        url = f"/channels/{self.id}/messages/search"
+        params = {
+            "content": content,
+            "author_id": author,
+            "mentions": mentions,
+            "has": has,
+            "max_id": before,
+            "min_id": after,
+            "offset": offset,
+        }
+        index = 0
+        for key, value in params.items():
+            if value is not None:
+                index += 1
+                param = f"{key}={value}"
+                if index == 1:
+                    param = "?" + param
+                else:
+                    param = "&" + param
+                url += param
+                
+        json = await self.http.request("get", url)
+        total = json.get("total_results")
+        messages = json['messages']if json.get("messages") is not None else []
+        
+        messages = [Message(msg, self.bot, self.http) for msgs in messages for msg in msgs]
+        return total, messages
+        
+
+    async def history(self, amount: int = 100, user: bool = False) -> list[Message] | None:
         """
         Get channel message history.
 
         Args:
             amount(int) : Amount of messages to gather. Default is 100.
 
         Returns:
@@ -52,27 +110,39 @@
         else:
             data = await self.http.request(
                 method="get", endpoint=f"/channels/{self.id}/messages?limit={amount + 5}"
             )
 
         if data is None:
             return None
-
-        messages = [Message(msg, self.bot, self.http) for msg in data]
+        if not user:
+            messages = [Message(msg, self.bot, self.http) for msg in data]
+        else:
+            messages = []
+            for msg in data:
+                msg = Message(msg, self.bot, self.http)
+                if msg.author == self.bot.user:
+                    messages.append(msg)
         while True:
             
 
             data = await self.http.request(
                 method="get",
                 endpoint=f"/channels/{self.id}/messages?limit=100&before={data[-1]['id']}",
             )
 
             if len(data) <= 0:
                 break
-            messages.extend(Message(msg, self.bot, self.http) for msg in data)
+            if not user:
+                messages.extend(Message(msg, self.bot, self.http) for msg in data)
+            else:
+                for msg in data:
+                    msg = Message(msg, self.bot, self.http)
+                    if msg.author == self.bot.user:
+                        messages.append(msg)
             if len(messages) >= amount:
                 break
 
         return messages
 
     async def upload_image(self, paths: list[str]) -> list[dict[str, int | str]]:
         files = []
@@ -80,65 +150,86 @@
         for path in paths:
             async with aiofiles.open(path, "rb") as f:
                 file = await f.read()
                 size = len(file)
                 name = os.path.basename(path)
             files.append({"file_size" : size, "filename": f"{name}", "id": id})
             id += 1
+
         json = await self.http.request("post", f"/channels/{self.id}/attachments", json={"files": files})
+
         items = []
         for key, atch in enumerate(json['attachments']):
             upload_url = atch['upload_url']
             id = atch['id']
             upload_filename = atch['upload_filename']
             async with aiohttp.ClientSession() as session:
                 async with aiofiles.open(paths[key], "rb") as f:
                     file = await f.read()
                 async with session.put(upload_url, data=file): 
                     pass
             items.append({"uploaded_filename": upload_filename, "filename": os.path.basename(upload_filename) , "id": id})
         return items
+    
+    async def delayed_delete(self, message: Message, time: int):
+        await asyncio.sleep(time)
+        await message.delete()
 
-        
 
     async def purge(self, amount: int = 0) -> None:
         """
         Delete a number of messages, starting from the most recent.
 
         Args:
             amount(int) : Number of messages to purge/delete.
 
         Returns:
             No return value
         """
-        messages = await self.history(amount)
-        if messages is None:
+        total, msgs = await self.search(author=self.bot.user.id)
+        if total == 0:
             return
-        msgs = [msg for msg in messages if str(msg.author.id) == str(self.bot.user.id)]
-        if amount != 0:
-            for i in range(0, len(msgs[:amount]), 3):
+        if amount == 0:
+            while True:
+                if len(msgs) >= total:
+                    break
+                _, new_msgs = await self.search(author=self.bot.user.id, offset=len(msgs))
+                msgs += new_msgs
+                if len(new_msgs) == 0:
+                    break
+
+            for i in range(0, len(msgs), 3):
                 await asyncio.gather(
                     *(
                         asyncio.create_task(message.delete())
-                        for message in msgs[:amount][i : i + 3]
+                        for message in msgs[i : i + 3]
                     )
                 )
-                await asyncio.sleep(0.3)
-            return
+                await asyncio.sleep(0.4)
+        else:
+            while True:
+                if len(msgs) >= amount:
+                    break
+                _, new_msgs = await self.search(author=self.bot.user.id, offset=len(msgs))
+                msgs += new_msgs
+                if len(new_msgs) == 0:
+                    break
+            for i in range(0, len(msgs), 3):
+                await asyncio.gather(
+                    *(
+                        asyncio.create_task(message.delete())
+                        for message in msgs[i : i + 3]
+                    ),
+                )
+                await asyncio.sleep(0.4)
+
 
 
-        for i in range(0, len(msgs), 3):
-            await asyncio.gather(
-                *(
-                    asyncio.create_task(message.delete())
-                    for message in msgs[i : i + 3]
-                )
-            )
-            await asyncio.sleep(0.3)
 
+        
 
 
     async def spam(self, amount: int, content: str, file_paths: list[str] = [], tts=False) -> None:
         """
         Send multiple of the same message.
 
         Args:
@@ -155,15 +246,15 @@
                 *(
                     asyncio.create_task(self.send(tts=tts, content=content, file_paths=file_paths))
                     for _ in amount[i : i + 3]
                 )
             )
             await asyncio.sleep(0.3)
 
-    async def send(self, content=None, file_paths: list[str] = [], tts=False) -> Message:
+    async def send(self, content=None, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
         """
         Send a message to the text channel.
 
         Args:
             - content(str) : Message content. Should be string type or similar. Discord `embed` type is not allowed.
             - tts(bool) : Specify whether message is text-to-speech or not
 
@@ -193,18 +284,20 @@
                 endpoint=f"/channels/{self.id}/messages",
                 headers={
                     "origin": "https://discord.com",
                     "referer": f"https://discord.com/channels/{self.id}",
                 },
                 json=json
             )
+        if delete_after is not None:
+            asyncio.create_task(self.delayed_delete(Message(resp, self.bot, self.http), delete_after))
 
         return Message(resp, self.bot, self.http)
 
-    async def reply(self, message: Message, content: str, file_paths: list[str] = [], tts=False) -> Message:
+    async def reply(self, message: Message, content: str, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
         """Reply to a specific message
 
         Args:
             message (str): Message to reply to
             content (_type_, optional): Message content to reply with. Defaults to None.
             tts (bool, optional): Specify whether message is text-to-speech or not. Defaults to False.
 
@@ -242,14 +335,16 @@
                 endpoint=f"/channels/{self.id}/messages",
                 headers={
                     "origin": "https://discord.com",
                     "referer": f"https://discord.com/channels/{self.id}",
                 },
                 json=json
             )
+        if delete_after is not None:
+            asyncio.create_task(self.delayed_delete(Message(resp, self.bot, self.http), delete_after))
         return Message(resp, self.bot, self.http)
 
 
 class Voiceable(Messageable):
     """Parent class specific for those classes that include a voice chat, or call functionality"""
 
     def __init__(self, http: http, bot: Bot) -> None:
@@ -362,15 +457,16 @@
             No arguments required
 
         Returns:
             No return value
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
-    
+   
+
     async def edit(
         self,
         name: str = None,
         parent_id: int = None,
         position: int = None,
         topic: str = None,
     ):
@@ -395,21 +491,17 @@
         if parent_id is not None:
             payload["parent_id"] = parent_id
         if position is not None:
             payload["position"] = position
         if topic is not None and topic != "":
             payload["topic"] = topic
 
-        try:
-            await self.http.request(
-                method="patch", endpoint=f"/channels/{self.id}", json=payload
-            )
-        except Exception as e:
-            error = "".join(format_exception(e, e, e.__traceback__))
-            log.error(f"Could not edit channel \n{error}")
+        await self.http.request(
+            method="patch", endpoint=f"/channels/{self.id}", json=payload
+        )
 
     async def create_webhook(self, name: str = None, avatar_url: str = None) -> Webhook:
         """
         Creates a webhook in the specified channel
 
         Args:
             name (str, optional): Name of the webhook. Defaults to None.
@@ -422,14 +514,15 @@
             NameError: Name is required
         """
         fields = {}
         if name != None:
             fields["name"] = name
         else:
             log.error("Name is required")
+            return
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
             fields["avatar"] = data
         data = await self.http.request(
             method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields
         )
         webhook = Webhook(data, self.bot, http=self.http)
@@ -518,14 +611,15 @@
         """
 
         fields = {}
         if name != None:
             fields["name"] = name
         else:
             log.error("Name is required...")
+            return None
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
             fields["avatar"] = data
         data = await self.http.request(
             method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields
         )
         webhook = Webhook(data, self.bot, self.http)
```

### Comparing `selfcord.py-0.2.0/selfcord/models/client.py` & `selfcord.py-0.2.1/selfcord/models/member.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from .channel import Voiceable
-    from .guild import Guild
-    from .message import Message
-    from .user import User
+    from .role import Role
 
 
-class Client:
-    """Client Object"""
+class Member:
+    """Member Object"""
 
     def __init__(self, UserPayload: dict) -> None:
-        self.guilds: list[Guild] = []
-        self.private_channels: list[Voiceable] = []
-        self.friends: list[User] = []
-        self.messages: list[Message] = []
-        self.deleted_messages: list[Message] = []
+        self.roles: list[Role] = []
+
         self._update(UserPayload)
 
-    def __str__(self) -> str:
+    def __str__(self):
         return f"""{self.name}#{self.discriminator}"""
 
     def __eq__(self, other):
         return self.id == other.id
 
-    def _update(self, data):
+    def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
-        self.name = data.get("username")
-        self.id = data.get("id")
-        self.discriminator = data.get("discriminator")
-        self.avatar = data.get("avatar")
-        self.banner = data.get("banner")
-        self.bio = data.get("bio")
-        self.email = data.get("email")
-        self.phone = data.get("phone")
-        self.accent_colour = data.get("accent_color")
-        self.public_flags = data.get("public_flags")
-        self.bot_acc = data.get("bot")
+        user = data.get("user")
+        self.name = user.get("username")
+        self.id = user.get("id")
+        self.discriminator = user.get("discriminator")
+        self._avatar = user.get("avatar")
+        self._banner = user.get("banner")
+        self._accent_colour = user.get("accent_color")
+        self._public_flags = user.get("public_flags")
+        self.bot_acc = user.get("bot")
+        self.joined_at = data.get("joined_at")
+        self.nick = data.get("nick")
         self.system = data.get("system")
```

### Comparing `selfcord.py-0.2.0/selfcord/models/emoji.py` & `selfcord.py-0.2.1/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.0/selfcord/models/guild.py` & `selfcord.py-0.2.1/selfcord/models/guild.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,22 @@
 
         Args:
             data (dict): JSON data from gateway
         """
         self.id = data.get("id")
         self.name = data.get("name")
         self.icon = data.get("icon")
-        self.icon_url = (
-            f"https://cdn.discordapp.com/icons/{self.id}/{self.icon}.webp?size=96"
-        )
+        if self.icon is not None:
+            if self.icon.startswith("a_"):
+                self.icon_url = f"https://cdn.discordapp.com/icons/{self.id}/{self.icon}.gif?size=4096"
+            else:
+                self.icon_url = f"https://cdn.discordapp.com/icons/{self.id}/{self.icon}.png?size=4096"
+        else:
+            self.icon_url = None
+
         self.region = data.get("region")
         self.splash = data.get("splash")
         self.mfa_level = data.get("mfa_level")
         self.features = data.get("features")
         self.member_count = data.get("member_count")
         self.unavailable = data.get("unavailable")
         self.verification_level = data.get("verification_level")
```

### Comparing `selfcord.py-0.2.0/selfcord/models/interactions.py` & `selfcord.py-0.2.1/selfcord/models/interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-import json
 import random
 import string
 import time
 from itertools import zip_longest
 from typing import TYPE_CHECKING
 
+import ujson
 from aioconsole import aprint
 
 if TYPE_CHECKING:
     from selfcord.api.http import http
     from selfcord.bot import Bot
 
 
@@ -171,14 +171,14 @@
                             {"name": opt.name, "type": opt.type, "value": value}
                         )
 
             data |= dic
         payload["data"] = data
         randstr = "".join(random.sample(string.ascii_letters + string.digits, k=16))
         boundary_val = f"----WebkitFormBoundary{randstr}"
-        req_data = f'--{boundary_val}\r\nContent-Disposition: form-data; name="payload_json"\r\n\r\n{json.dumps(payload)}\r\n--{boundary_val}--'
+        req_data = f'--{boundary_val}\r\nContent-Disposition: form-data; name="payload_json"\r\n\r\n{ujson.dumps(payload)}\r\n--{boundary_val}--'
         await self.http.request(
             "post",
             "/interactions",
             headers={"content-type": f"multipart/form-data; boundary={boundary_val}"},
             data=req_data,
         )
```

### Comparing `selfcord.py-0.2.0/selfcord/models/permission.py` & `selfcord.py-0.2.1/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.0/selfcord/models/role.py` & `selfcord.py-0.2.1/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.0/selfcord/models/user.py` & `selfcord.py-0.2.1/selfcord/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,24 +179,30 @@
         self.name = data.get("username")
         self.id = data.get("id")
         self.discriminator = data.get("discriminator")
         self.avatar = data.get("avatar")
         self.banner = data.get("banner")
         self.accent_colour = data.get("accent_color")
         self.bot_acc = data.get("bot")
-        self.avatar_url = (
-            f"https://cdn.discordapp.com/avatars/{self.id}/{self.avatar}.png?size=4096"
-            if self.avatar != None
-            else None
-        )
-        self.banner_url = (
-            f"https://cdn.discordapp.com/banners/{self.id}/{self.banner}.png?size=1024"
-            if self.banner != None
-            else None
-        )
+
+        if self.avatar is not None:
+            if self.avatar.startswith("a_"):
+                self.avatar_url = f"https://cdn.discordapp.com/avatars/{self.id}/{self.avatar}.gif?size=4096"
+            else:
+                self.avatar_url = f"https://cdn.discordapp.com/avatars/{self.id}/{self.avatar}.png?size=4096"
+        else:
+            self.avatar_url = None
+
+        if self.banner is not None:
+            if self.banner.startswith("a_"):
+                self.banner_url = f"https://cdn.discordapp.com/banners/{self.id}/{self.banner}.gif?size=4096"
+            else:
+                self.banner_url = f"https://cdn.discordapp.com/banners/{self.id}/{self.banner}.png?size=4096"
+        else:
+            self.banner_url = None
         self.system = data.get("system")
         self.raw_flags = data.get("flags") if data.get("flags") is not None else 0
         self.raw_public_flags = data.get("public_flags") if data.get("public_flags") is not None else 0
 
     async def create_dm(self):
         """Create a dm for the user"""
         await self.http.request(
```

### Comparing `selfcord.py-0.2.0/selfcord/models/webhook.py` & `selfcord.py-0.2.1/selfcord/models/webhook.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         """
         self.id = data.get("id")
         self.type = data.get("type")
         self.guild_id = data.get("guild_id")
         self.channel_id = data.get("channel_id")
         self.name = data.get("name")
         self.avatar = data.get("avatar")
+
+        if self.avatar is not None:
+            if self.avatar.startswith("a_"):
+                self.avatar_url = f"https://cdn.discordapp.com/avatars/{self.id}/{self.avatar}.gif?size=4096"
+            else:
+                self.avatar_url = f"https://cdn.discordapp.com/avatars/{self.id}/{self.avatar}.png?size=4096"
+        else:
+            self.avatar_url = None
+
         self.token = data.get("token")
         self.application_id = data.get("application_id")
         self.webhook_url = f"https://discord.com/api/webhooks/{self.id}/{self.token}"
         self.source_guild = data.get("source_guild")
         self.source_channel = data.get("source_channel")
 
     async def send(self, content: str):
```

### Comparing `selfcord.py-0.2.0/selfcord/utils/command.py` & `selfcord.py-0.2.1/selfcord/utils/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import inspect
 import re
+import shlex
 from collections import defaultdict
 from traceback import format_exception
 from typing import TYPE_CHECKING, Any
 
 from .logging import logging
 
 if TYPE_CHECKING:
     from ..api import *
     from ..bot import Bot
     from ..models import *
 
 
-log = logging.getLogger("Commands")
+log = logging.getLogger(__name__)
 
 
 class Extension:
     """Extension object. Discord.py equivalent of cogs, a helper system to help manage and organise code into multiple files"""
 
     def __init__(self, **kwargs):
         self.name: str | None = kwargs.get("name")
@@ -238,14 +239,15 @@
         if isinstance(aliases, str):
             aliases = [aliases]
 
         def decorator(coro):
             name = coro.__name__
             if not inspect.iscoroutinefunction(coro):
                 log.error("Not a coroutine")
+                raise Exception("Not a coroutine")
             else:
                 cmd = Command(
                     name=name, description=description, aliases=aliases, func=coro
                 )
                 cls.commands.add(cmd)
 
             return cmd
@@ -259,14 +261,15 @@
         Args:
             event (str): The event to check for
         """
 
         def decorator(coro):
             if not inspect.iscoroutinefunction(coro):
                 log.error("Not a coroutine")
+                raise Exception("Not a coroutine")
             else:
                 eve = Event(name=event, coro=coro, ext=cls)
                 cls._events[event].append(eve)
 
                 def wrapper(*args, **kwargs):
                     result = cls._events[event].append(eve)
                     return result
@@ -405,16 +408,20 @@
         args: list[Any] = []
         kwargs: dict[Any, Any] = {}
 
         if self.command.signature is not None:
             signature = self.command.signature
         if self.command_content == "":
             return args, kwargs
-
-        splitted = self.command_content.split(" ")[1:]
+        if self.command_content == None:
+            return args, kwargs
+        sh = shlex.shlex(self.command_content[1:], posix=False)
+        sh.whitespace = " "
+        sh.whitespace_split = True
+        splitted = list(sh)
 
         for index, item in enumerate(splitted):
             user_regex = re.findall(r"<@[0-9]{18,19}>", item)
             if len(user_regex) > 0:
                 x = re.findall(r"[0-9]{18,19}", item)
                 if len(x) > 0:
                     val = x[0]
@@ -424,20 +431,24 @@
             if name in ["ctx", "self"]:
                 continue
 
             if param.kind is param.POSITIONAL_OR_KEYWORD:
                 try:
                     arg: str | Any = self.convert(param, splitted.pop(0))
                     args.append(arg)
-                except Exception:
-                    pass
+                except Exception as e:
+                    log.error(e)
             if param.kind is param.VAR_KEYWORD:
                 for arg in splitted:
                     arg = self.convert(param, arg)
                     args.append(arg)
+            if param.kind is param.VAR_POSITIONAL:
+                for arg in splitted:
+                    arg = self.convert(param, arg)
+                    args.append(arg)
 
             if param.kind is param.KEYWORD_ONLY:
                 arg = self.convert(param, " ".join(splitted))
                 kwargs[name] = arg
 
         for key in kwargs.copy():
             if not kwargs[key]:
@@ -462,32 +473,32 @@
                 args.insert(0, self)
         try:
             await func(*args, **kwargs)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not run command \n{error}")
 
-    async def reply(self, content: str, file_paths: list[str] = [], tts=False) -> Message:
+    async def reply(self, content: str, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
         """Helper function to reply to your own message containing the command
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        message: Message = await self.channel.reply(self.message, content, file_paths, tts)
+        message: Message = await self.channel.reply(self.message, content, file_paths, delete_after, tts)
         return message
 
-    async def send(self, content: str, file_paths: list[str] = [], tts=False) -> Message:
+    async def send(self, content: str, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
         """Helper function to send message to the current channel
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        message: Message = await self.channel.send(content=content, file_paths=file_paths, tts=tts)
+        message: Message = await self.channel.send(content=content, file_paths=file_paths, delete_after=delete_after, tts=tts)
         return message
 
     async def spam(self, amount: int, content: str, file_paths: list[str] = [], tts: bool = False):
         """Helper function to spam messages in the current channel (uses asyncio.gather !!!!)
 
         Args:
             amount (int): Amount of messages to spam
@@ -499,15 +510,15 @@
         """Helper function to purge messages in the current channel, uses asyncio gather.
 
         Args:
             amount (int): The amount of messages to purge, defaults to All.
         """
         await self.channel.purge(amount)
 
-    async def edit(self, content: str, file_paths: list[str] = []) -> Message:
+    async def edit(self, content: str, file_paths: list[str] = [], delete_after: int | None = None) -> Message:
         """Helper function to edit the message you sent
 
         Args:
             content (str): Content to edit to
         """
-        message = await self.message.edit(content, file_paths)
+        message = await self.message.edit(content, file_paths, delete_after)
         return message
```

### Comparing `selfcord.py-0.2.0/selfcord/utils/logging.py` & `selfcord.py-0.2.1/selfcord/utils/logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 import logging
 import logging.config
 
-logging.config.dictConfig(
-    {
-        "version": 1,
-        "disable_existing_loggers": True,
-    }
-)
-
 logging.getLogger("websockets.client").disabled = True
 logging.getLogger("urllib3.connectionpool").disabled = True
 
 FMT = "[{asctime}][{levelname:^9}] {name}: {message}"
 
 FORMATS = {
     logging.DEBUG: f"\33[93m{FMT}\33[0m",
@@ -27,12 +20,7 @@
         log_fmt = FORMATS[record.levelno]
         formatter = logging.Formatter(log_fmt, style="{", datefmt="%H:%M:%S")
         return formatter.format(record)
 
 
 handler = logging.StreamHandler()
 handler.setFormatter(CustomFormatter())
-
-logging.basicConfig(
-    level=logging.DEBUG,
-    handlers=[handler],
-)
```

### Comparing `selfcord.py-0.2.0/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.2.1/selfcord.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -15,15 +15,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.0-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.1-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.0 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.1 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.0-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.1-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.0/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.2.1/selfcord.py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 selfcord/models/emoji.py
 selfcord/models/guild.py
 selfcord/models/interactions.py
 selfcord/models/member.py
 selfcord/models/message.py
 selfcord/models/permission.py
 selfcord/models/role.py
+selfcord/models/sessions.py
 selfcord/models/user.py
 selfcord/models/webhook.py
 selfcord/utils/__init__.py
 selfcord/utils/command.py
 selfcord/utils/logging.py
 tests/test_commands.py
```

### Comparing `selfcord.py-0.2.0/setup.py` & `selfcord.py-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,27 @@
                 "selfcord",
                 "selfcord.api",
                 "selfcord.utils",
                 "selfcord.models",
                 "selfcord.api.voice",
             ]
         ),
-        version="0.2.0",
+        version="0.2.1",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell",
         extras_require={"voice": ["pynacl==1.5.0", "opuslib==3.0.1"]},
         license="MIT",
         install_requires=[
             "aiohttp==3.7.4.post0",
             "aioconsole==0.3.3",
             "websockets==10.1",
-            "requests",
+            "ujson==5.7.0",
+            "aiofiles==0.8.0",
+            "requests==2.31.0"
         ],
         setup_requires=["pytest-runner"],
         tests_require=["pytest"],
         test_suite="tests",
         keywords=["selfbot", "discord", "discordapi", "discordwrapper"],
         long_description=long_description,
         url="https://github.com/Shell1010/Selfcord",
```

