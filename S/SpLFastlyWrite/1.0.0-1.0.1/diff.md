# Comparing `tmp/SpLFastlyWrite-1.0.0.tar.gz` & `tmp/SpLFastlyWrite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpLFastlyWrite-1.0.0.tar", last modified: Thu Jun 22 05:43:51 2023, max compression
+gzip compressed data, was "SpLFastlyWrite-1.0.1.tar", last modified: Fri Jun 23 08:07:49 2023, max compression
```

## Comparing `SpLFastlyWrite-1.0.0.tar` & `SpLFastlyWrite-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-22 05:43:51.132856 SpLFastlyWrite-1.0.0/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-06-22 05:36:52.000000 SpLFastlyWrite-1.0.0/LICENSE
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      692 2023-06-22 05:43:51.132856 SpLFastlyWrite-1.0.0/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-06-22 05:36:52.000000 SpLFastlyWrite-1.0.0/README.md
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-22 05:43:51.126855 SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      692 2023-06-22 05:43:51.000000 SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      959 2023-06-22 05:43:51.000000 SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/SOURCES.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-22 05:43:51.000000 SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/dependency_links.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-22 05:43:50.000000 SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/not-zip-safe
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-06-22 05:43:51.000000 SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/top_level.txt
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-22 05:43:51.126855 SpLFastlyWrite-1.0.0/Spoiled/
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-22 05:43:51.128855 SpLFastlyWrite-1.0.0/Spoiled/Database/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      187 2023-06-22 05:36:57.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-06-22 05:36:56.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/chat_words.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-06-22 05:36:56.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/chats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-06-22 05:36:56.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-06-22 05:36:56.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/completed.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-06-22 05:36:57.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/global_stats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-06-22 05:36:57.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/privacy.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-06-22 05:36:57.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/record.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-06-22 05:36:57.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/user_chat_info.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-06-22 05:36:57.000000 SpLFastlyWrite-1.0.0/Spoiled/Database/users.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-22 05:43:51.132856 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-06-22 05:36:55.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     8172 2023-06-22 05:36:53.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/callbacks.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      552 2023-06-22 05:36:53.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6638 2023-06-22 05:36:53.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/eval.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2801 2023-06-22 05:36:54.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/fw.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-06-22 05:36:54.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/help.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      952 2023-06-22 05:36:54.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/image.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-06-22 05:36:54.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/inline.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-06-22 05:36:54.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/leaderboard.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-06-22 05:36:55.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/served.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3695 2023-06-22 05:36:55.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/start.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-06-22 05:36:55.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/templates.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-06-22 05:36:55.000000 SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/watchers.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       28 2023-06-22 05:36:53.000000 SpLFastlyWrite-1.0.0/Spoiled/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-06-22 05:43:51.132856 SpLFastlyWrite-1.0.0/setup.cfg
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1034 2023-06-22 05:42:48.000000 SpLFastlyWrite-1.0.0/setup.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-23 08:07:49.142083 SpLFastlyWrite-1.0.1/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-06-23 08:03:51.000000 SpLFastlyWrite-1.0.1/LICENSE
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-23 08:07:49.142083 SpLFastlyWrite-1.0.1/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-06-23 08:03:51.000000 SpLFastlyWrite-1.0.1/README.md
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-23 08:07:49.135082 SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-23 08:07:49.000000 SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      959 2023-06-23 08:07:49.000000 SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/SOURCES.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-23 08:07:49.000000 SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/dependency_links.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-23 08:07:48.000000 SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/not-zip-safe
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-06-23 08:07:49.000000 SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/top_level.txt
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-23 08:07:49.135082 SpLFastlyWrite-1.0.1/Spoiled/
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-23 08:07:49.138082 SpLFastlyWrite-1.0.1/Spoiled/Database/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      187 2023-06-23 08:03:55.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/chat_words.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/chats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/completed.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/global_stats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-06-23 08:03:55.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/privacy.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-06-23 08:03:55.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/record.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-06-23 08:03:55.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/user_chat_info.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-06-23 08:03:55.000000 SpLFastlyWrite-1.0.1/Spoiled/Database/users.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-23 08:07:49.141083 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     8172 2023-06-23 08:03:52.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/callbacks.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      552 2023-06-23 08:03:52.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6638 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/eval.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2801 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/fw.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/help.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      952 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/image.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/inline.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/leaderboard.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/served.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3695 2023-06-23 08:03:53.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/start.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/templates.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-06-23 08:03:54.000000 SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/watchers.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       64 2023-06-23 08:03:52.000000 SpLFastlyWrite-1.0.1/Spoiled/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-06-23 08:07:49.142083 SpLFastlyWrite-1.0.1/setup.cfg
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-06-23 08:03:52.000000 SpLFastlyWrite-1.0.1/setup.py
```

### Comparing `SpLFastlyWrite-1.0.0/LICENSE` & `SpLFastlyWrite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/PKG-INFO` & `SpLFastlyWrite-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.0
-Summary: Easier access and Less Waits library for pyrogram
+Version: 1.0.1
+Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
 Project-URL: Community, https://t.me/SpLBots
```

### Comparing `SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/PKG-INFO` & `SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.0
-Summary: Easier access and Less Waits library for pyrogram
+Version: 1.0.1
+Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
 Project-URL: Community, https://t.me/SpLBots
```

### Comparing `SpLFastlyWrite-1.0.0/SpLFastlyWrite.egg-info/SOURCES.txt` & `SpLFastlyWrite-1.0.1/SpLFastlyWrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/chat_words.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/chat_words.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/chats.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/chats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/coins.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/coins.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/completed.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/completed.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/global_stats.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/global_stats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/privacy.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/privacy.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/user_chat_info.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/user_chat_info.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/Database/users.py` & `SpLFastlyWrite-1.0.1/Spoiled/Database/users.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/__init__.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/__init__.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/callbacks.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/coins.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/coins.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/eval.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/eval.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/fw.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/fw.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/help.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/help.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/image.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/image.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/inline.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/inline.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/leaderboard.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/leaderboard.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/served.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/served.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/start.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/start.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/Spoiled/SpoiledPlugins/templates.py` & `SpLFastlyWrite-1.0.1/Spoiled/SpoiledPlugins/templates.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.0/setup.py` & `SpLFastlyWrite-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, Extension, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="SpLFastlyWrite",
-    version="1.0.0",
-    description="Easier access and Less Waits library for pyrogram",
+    version="1.0.1",
+    description="SpLFastlyWrite",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/ShutupKeshav/SpLFastlyWrite",
     download_url="https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest",
     author="ShutupKeshav",
     author_email="keshavatripathi@yahoo.com",
     license="MIT",
```

