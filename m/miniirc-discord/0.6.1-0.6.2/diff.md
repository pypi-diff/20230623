# Comparing `tmp/miniirc_discord-0.6.1.tar.gz` & `tmp/miniirc_discord-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniirc_discord-0.6.1.tar", last modified: Sun Sep 18 08:14:29 2022, max compression
+gzip compressed data, was "miniirc_discord-0.6.2.tar", last modified: Fri Jun 23 07:41:46 2023, max compression
```

## Comparing `miniirc_discord-0.6.1.tar` & `miniirc_discord-0.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 08:14:29.487131 miniirc_discord-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-09-18 08:14:22.000000 miniirc_discord-0.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     4955 2022-09-18 08:14:29.487131 miniirc_discord-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4451 2022-09-18 08:14:22.000000 miniirc_discord-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 08:14:29.487131 miniirc_discord-0.6.1/miniirc_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4955 2022-09-18 08:14:29.000000 miniirc_discord-0.6.1/miniirc_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-18 08:14:29.000000 miniirc_discord-0.6.1/miniirc_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 08:14:29.000000 miniirc_discord-0.6.1/miniirc_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-18 08:14:29.000000 miniirc_discord-0.6.1/miniirc_discord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-18 08:14:29.000000 miniirc_discord-0.6.1/miniirc_discord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15411 2022-09-18 08:14:22.000000 miniirc_discord-0.6.1/miniirc_discord.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-18 08:14:29.487131 miniirc_discord-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      855 2022-09-18 08:14:22.000000 miniirc_discord-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:41:46.485323 miniirc_discord-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-23 07:41:24.000000 miniirc_discord-0.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-23 07:41:46.485323 miniirc_discord-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-23 07:41:24.000000 miniirc_discord-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:41:46.485323 miniirc_discord-0.6.2/miniirc_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-23 07:41:46.000000 miniirc_discord-0.6.2/miniirc_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 07:41:46.000000 miniirc_discord-0.6.2/miniirc_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:41:46.000000 miniirc_discord-0.6.2/miniirc_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 07:41:46.000000 miniirc_discord-0.6.2/miniirc_discord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 07:41:46.000000 miniirc_discord-0.6.2/miniirc_discord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-06-23 07:41:24.000000 miniirc_discord-0.6.2/miniirc_discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:41:46.485323 miniirc_discord-0.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      855 2023-06-23 07:41:24.000000 miniirc_discord-0.6.2/setup.py
```

### Comparing `miniirc_discord-0.6.1/LICENSE.md` & `miniirc_discord-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniirc_discord-0.6.1/PKG-INFO` & `miniirc_discord-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniirc_discord
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Discord wrapper for miniirc.
 Author: luk3yx
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -70,16 +70,15 @@
 ```
 
 ## Supported commands
 
 ### `PRIVMSG`
 
 `PRIVMSG` operates like you'd expect and IRC formatting codes are converted to
-markdown. You cannot, however, send messages to a channel before the bot has
-received a message from the channel.
+markdown. You can use the `+draft/reply` IRCv3 tag to reply to a message.
 
 ### `CTCP ACTION` (`irc.me()`)
 
 This works similarly to `PRIVMSG`, except the CTCP ACTION is also converted to
 a Discord `/me`.
 
 ### `NOTICE`
```

### Comparing `miniirc_discord-0.6.1/README.md` & `miniirc_discord-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,15 @@
 ```
 
 ## Supported commands
 
 ### `PRIVMSG`
 
 `PRIVMSG` operates like you'd expect and IRC formatting codes are converted to
-markdown. You cannot, however, send messages to a channel before the bot has
-received a message from the channel.
+markdown. You can use the `+draft/reply` IRCv3 tag to reply to a message.
 
 ### `CTCP ACTION` (`irc.me()`)
 
 This works similarly to `PRIVMSG`, except the CTCP ACTION is also converted to
 a Discord `/me`.
 
 ### `NOTICE`
```

### Comparing `miniirc_discord-0.6.1/miniirc_discord.egg-info/PKG-INFO` & `miniirc_discord-0.6.2/miniirc_discord.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniirc-discord
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Discord wrapper for miniirc.
 Author: luk3yx
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -70,16 +70,15 @@
 ```
 
 ## Supported commands
 
 ### `PRIVMSG`
 
 `PRIVMSG` operates like you'd expect and IRC formatting codes are converted to
-markdown. You cannot, however, send messages to a channel before the bot has
-received a message from the channel.
+markdown. You can use the `+draft/reply` IRCv3 tag to reply to a message.
 
 ### `CTCP ACTION` (`irc.me()`)
 
 This works similarly to `PRIVMSG`, except the CTCP ACTION is also converted to
 a Discord `/me`.
 
 ### `NOTICE`
```

### Comparing `miniirc_discord-0.6.1/miniirc_discord.py` & `miniirc_discord-0.6.2/miniirc_discord.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 #
 # Licensed under the MIT License:
 # https://gitlab.com/luk3yx/miniirc_discord/LICENSE.md
 #
 
 import asyncio, discord, itertools, miniirc, re, threading, time, traceback
 
-ver      = (0,6,1)
-version  = '0.6.1'
+ver      = (0,6,2)
+version  = '0.6.2'
 __all__  = ['Discord', 'miniirc']
 
 assert miniirc.ver >= (1, 8, 0), 'Please update miniirc!'
 assert discord.version_info >= (2, 0, 0), 'Please update discord.py!'
 
 def _hostmask(author):
     return (
@@ -54,15 +54,21 @@
         tags['+draft/reply'] = str(message.reference.message_id)
 
     # Create the args
     channel = str(message.channel.id)
 
     if not isinstance(message.channel, discord.abc.PrivateChannel):
         channel = '#' + channel
-    args = [channel, _v1_only_colon + message.content]
+
+    lines = []
+    if message.content:
+        lines.append(message.content)
+    lines.extend(attachment.url for attachment in message.attachments)
+
+    args = [channel, _v1_only_colon + '\n'.join(lines)]
 
     irc.debug('Handling message:', hostmask, tags, args)
     irc._handle('PRIVMSG', hostmask, tags, args)
 
 
 async def _handle_reaction(irc, payload):
     # DM reactions aren't currently supported since the user name isn't sent
```

### Comparing `miniirc_discord-0.6.1/setup.py` & `miniirc_discord-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     desc = f.read()
 
 setup(
     name        = 'miniirc_discord',
-    version     = '0.6.1',
+    version     = '0.6.2',
     py_modules  = ['miniirc_discord'],
     author      = 'luk3yx',
     description = 'A Discord wrapper for miniirc.',
     license     = 'MIT',
 
     long_description              = desc,
     long_description_content_type = 'text/markdown',
```

