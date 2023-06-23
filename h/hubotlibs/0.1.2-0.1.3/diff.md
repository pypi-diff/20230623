# Comparing `tmp/hubotlibs-0.1.2.tar.gz` & `tmp/hubotlibs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubotlibs-0.1.2.tar", last modified: Fri Jun 23 13:40:00 2023, max compression
+gzip compressed data, was "hubotlibs-0.1.3.tar", last modified: Fri Jun 23 14:44:44 2023, max compression
```

## Comparing `hubotlibs-0.1.2.tar` & `hubotlibs-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.035838 hubotlibs-0.1.2/
--rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2623 2023-06-23 13:40:00.035838 hubotlibs-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 13:39:59.971624 hubotlibs-0.1.2/hubotlibs/
--rw-rw-rw-   0        0        0     1459 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/hubotlibs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.000548 hubotlibs-0.1.2/hubotlibs/dar/
--rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.1.2/hubotlibs/dar/load.py
--rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/log.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.032323 hubotlibs-0.1.2/hubotlibs/dar/utils/
--rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/PyroHelpers.py
--rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/adminHelpers.py
--rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/ai.py
--rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/aiohttp_helper.py
--rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/basic.py
--rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.033842 hubotlibs-0.1.2/hubotlibs/dar/utils/db/
--rw-rw-rw-   0        0        0    14687 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/db/__init__.py
--rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/db/permit.py
--rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/function.py
--rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/get_id.py
--rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/http.py
--rw-rw-rw-   0        0        0     2055 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/inline.py
--rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/interval.py
--rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/misc.py
--rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/parser.py
--rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/pilter.py
--rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/tools.py
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/unpack.py
--rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/utility.py
--rw-rw-rw-   0        0        0       47 2023-06-23 13:39:43.000000 hubotlibs-0.1.2/hubotlibs/version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:39:59.995558 hubotlibs-0.1.2/hubotlibs.egg-info/
--rw-rw-rw-   0        0        0     2623 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 13:40:00.037814 hubotlibs-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.474379 hubotlibs-0.1.3/
+-rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2623 2023-06-23 14:44:44.474379 hubotlibs-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.328768 hubotlibs-0.1.3/hubotlibs/
+-rw-rw-rw-   0        0        0     1455 2023-06-23 14:44:00.000000 hubotlibs-0.1.3/hubotlibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.349712 hubotlibs-0.1.3/hubotlibs/dar/
+-rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.1.3/hubotlibs/dar/load.py
+-rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/log.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.405564 hubotlibs-0.1.3/hubotlibs/dar/utils/
+-rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/PyroHelpers.py
+-rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/adminHelpers.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/ai.py
+-rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/aiohttp_helper.py
+-rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/basic.py
+-rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.472385 hubotlibs-0.1.3/hubotlibs/dar/utils/db/
+-rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/db/__init__.py
+-rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/db/permit.py
+-rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/function.py
+-rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/get_id.py
+-rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/http.py
+-rw-rw-rw-   0        0        0     2055 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/inline.py
+-rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/interval.py
+-rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/misc.py
+-rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/parser.py
+-rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/pilter.py
+-rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/tools.py
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/unpack.py
+-rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/utility.py
+-rw-rw-rw-   0        0        0       47 2023-06-23 14:44:08.000000 hubotlibs-0.1.3/hubotlibs/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.345721 hubotlibs-0.1.3/hubotlibs.egg-info/
+-rw-rw-rw-   0        0        0     2623 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:44:44.476375 hubotlibs-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.3/setup.py
```

### Comparing `hubotlibs-0.1.2/LICENSE` & `hubotlibs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/PKG-INFO` & `hubotlibs-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.2/README.md` & `hubotlibs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/__init__.py` & `hubotlibs-0.1.3/hubotlibs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,13 +56,13 @@
     1993568296,  # cuki
     2073506739,  # amang
 ]
 
 
 async def ajg(client):
     try:
-        await client.join_chat("hubotlibssupport")
+        await client.join_chat("hubotsupport")
     except pyrogram.errors.exceptions.bad_request_400.UserBannedInChannel:
         print(
             "Anda tidak bisa menggunakan bot ini, karna telah diban dari @hubotlibssupport\nHubungi @kenapatagdar untuk dibuka blokir nya."
         )
         sys.exit()
```

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/__init__.py` & `hubotlibs-0.1.3/hubotlibs/dar/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/load.py` & `hubotlibs-0.1.3/hubotlibs/dar/load.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/log.py` & `hubotlibs-0.1.3/hubotlibs/dar/log.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/PyroHelpers.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/adminHelpers.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/ai.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/ai.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/aiohttp_helper.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/basic.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/basic.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/constants.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/db/__init__.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/db/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         return False
 
 
 async def get_botlog(user_id: int):
     user_data = await logdb.users.find_one({"user_id": user_id})
     botlog_chat_id = user_data.get("bot_log_group_id") if user_data else None
     return botlog_chat_id
-
+babi
 
 async def set_botlog(user_id: int, botlog_chat_id: int):
     await logdb.users.update_one(
         {"user_id": user_id},
         {"$set": {"bot_log_group_id": botlog_chat_id}},
         upsert=True,
     )
```

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/db/permit.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/function.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/function.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/get_id.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/http.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/http.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/inline.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/inline.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/interval.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/interval.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/misc.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/parser.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/parser.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/pilter.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/tools.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/unpack.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs/dar/utils/utility.py` & `hubotlibs-0.1.3/hubotlibs/dar/utils/utility.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/hubotlibs.egg-info/PKG-INFO` & `hubotlibs-0.1.3/hubotlibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.2/hubotlibs.egg-info/SOURCES.txt` & `hubotlibs-0.1.3/hubotlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.2/setup.py` & `hubotlibs-0.1.3/setup.py`

 * *Files identical despite different names*

