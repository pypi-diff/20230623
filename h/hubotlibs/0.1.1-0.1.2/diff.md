# Comparing `tmp/hubotlibs-0.1.1.tar.gz` & `tmp/hubotlibs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubotlibs-0.1.1.tar", last modified: Fri Jun 23 13:02:11 2023, max compression
+gzip compressed data, was "hubotlibs-0.1.2.tar", last modified: Fri Jun 23 13:40:00 2023, max compression
```

## Comparing `hubotlibs-0.1.1.tar` & `hubotlibs-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:02:11.942376 hubotlibs-0.1.1/
--rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2623 2023-06-23 13:02:11.942376 hubotlibs-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 13:02:11.885925 hubotlibs-0.1.1/hubotlibs/
--rw-rw-rw-   0        0        0     1459 2023-06-23 13:01:30.000000 hubotlibs-0.1.1/hubotlibs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:02:11.914974 hubotlibs-0.1.1/hubotlibs/dar/
--rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.1/hubotlibs/dar/__init__.py
--rw-rw-rw-   0        0        0     1763 2023-06-23 13:01:30.000000 hubotlibs-0.1.1/hubotlibs/dar/load.py
--rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/log.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:02:11.938071 hubotlibs-0.1.1/hubotlibs/dar/utils/
--rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/PyroHelpers.py
--rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/adminHelpers.py
--rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/ai.py
--rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/aiohttp_helper.py
--rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/basic.py
--rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:02:11.940066 hubotlibs-0.1.1/hubotlibs/dar/utils/db/
--rw-rw-rw-   0        0        0    14687 2023-06-23 13:01:30.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/db/__init__.py
--rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/db/permit.py
--rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/function.py
--rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/get_id.py
--rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/http.py
--rw-rw-rw-   0        0        0     2055 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/inline.py
--rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/interval.py
--rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/misc.py
--rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/parser.py
--rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/pilter.py
--rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/tools.py
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/unpack.py
--rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.1/hubotlibs/dar/utils/utility.py
--rw-rw-rw-   0        0        0       47 2023-06-23 12:50:21.000000 hubotlibs-0.1.1/hubotlibs/version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:02:11.911979 hubotlibs-0.1.1/hubotlibs.egg-info/
--rw-rw-rw-   0        0        0     2623 2023-06-23 13:02:11.000000 hubotlibs-0.1.1/hubotlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-06-23 13:02:11.000000 hubotlibs-0.1.1/hubotlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:02:11.000000 hubotlibs-0.1.1/hubotlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-23 13:02:11.000000 hubotlibs-0.1.1/hubotlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 13:02:11.000000 hubotlibs-0.1.1/hubotlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 13:02:11.944105 hubotlibs-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.035838 hubotlibs-0.1.2/
+-rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2623 2023-06-23 13:40:00.035838 hubotlibs-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 13:39:59.971624 hubotlibs-0.1.2/hubotlibs/
+-rw-rw-rw-   0        0        0     1459 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/hubotlibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.000548 hubotlibs-0.1.2/hubotlibs/dar/
+-rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.1.2/hubotlibs/dar/load.py
+-rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/log.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.032323 hubotlibs-0.1.2/hubotlibs/dar/utils/
+-rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/PyroHelpers.py
+-rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/adminHelpers.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/ai.py
+-rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/aiohttp_helper.py
+-rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/basic.py
+-rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:40:00.033842 hubotlibs-0.1.2/hubotlibs/dar/utils/db/
+-rw-rw-rw-   0        0        0    14687 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/db/__init__.py
+-rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/db/permit.py
+-rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/function.py
+-rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/get_id.py
+-rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/http.py
+-rw-rw-rw-   0        0        0     2055 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/inline.py
+-rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/interval.py
+-rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/misc.py
+-rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/parser.py
+-rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/pilter.py
+-rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/tools.py
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/unpack.py
+-rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.2/hubotlibs/dar/utils/utility.py
+-rw-rw-rw-   0        0        0       47 2023-06-23 13:39:43.000000 hubotlibs-0.1.2/hubotlibs/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:39:59.995558 hubotlibs-0.1.2/hubotlibs.egg-info/
+-rw-rw-rw-   0        0        0     2623 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 13:39:59.000000 hubotlibs-0.1.2/hubotlibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 13:40:00.037814 hubotlibs-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.2/setup.py
```

### Comparing `hubotlibs-0.1.1/LICENSE` & `hubotlibs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/PKG-INFO` & `hubotlibs-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.1/README.md` & `hubotlibs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/__init__.py` & `hubotlibs-0.1.2/hubotlibs/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/__init__.py` & `hubotlibs-0.1.2/hubotlibs/dar/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/load.py` & `hubotlibs-0.1.2/hubotlibs/dar/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from haidar import *
 from haidar.config import *
 from haidar.modules import loadModule
 from pyrogram import __version__
 from pyrogram.types import InlineKeyboardButton, InlineKeyboardMarkup
 
-from hubotlibslibs.dar.utils.db import *
+from hubotlibs.dar.utils.db import *
 
 
 async def loadprem():
     modules = loadModule()
     for mod in modules:
         imported_module = import_module(f"haidar.modules.{mod}")
         if hasattr(imported_module, "__MODULE__") and imported_module.__MODULE__:
```

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/log.py` & `hubotlibs-0.1.2/hubotlibs/dar/log.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/PyroHelpers.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/adminHelpers.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/ai.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/ai.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/aiohttp_helper.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/basic.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/basic.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/constants.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/db/__init__.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/db/permit.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/function.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/function.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/get_id.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/http.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/http.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/inline.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/inline.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/interval.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/interval.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/misc.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/parser.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/parser.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/pilter.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/tools.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/unpack.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs/dar/utils/utility.py` & `hubotlibs-0.1.2/hubotlibs/dar/utils/utility.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/hubotlibs.egg-info/PKG-INFO` & `hubotlibs-0.1.2/hubotlibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.1/hubotlibs.egg-info/SOURCES.txt` & `hubotlibs-0.1.2/hubotlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.1/setup.py` & `hubotlibs-0.1.2/setup.py`

 * *Files identical despite different names*

