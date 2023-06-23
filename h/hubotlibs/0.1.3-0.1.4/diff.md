# Comparing `tmp/hubotlibs-0.1.3.tar.gz` & `tmp/hubotlibs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubotlibs-0.1.3.tar", last modified: Fri Jun 23 14:44:44 2023, max compression
+gzip compressed data, was "hubotlibs-0.1.4.tar", last modified: Fri Jun 23 17:35:23 2023, max compression
```

## Comparing `hubotlibs-0.1.3.tar` & `hubotlibs-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.474379 hubotlibs-0.1.3/
--rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2623 2023-06-23 14:44:44.474379 hubotlibs-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.328768 hubotlibs-0.1.3/hubotlibs/
--rw-rw-rw-   0        0        0     1455 2023-06-23 14:44:00.000000 hubotlibs-0.1.3/hubotlibs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.349712 hubotlibs-0.1.3/hubotlibs/dar/
--rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/__init__.py
--rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.1.3/hubotlibs/dar/load.py
--rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/log.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.405564 hubotlibs-0.1.3/hubotlibs/dar/utils/
--rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/PyroHelpers.py
--rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/adminHelpers.py
--rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/ai.py
--rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/aiohttp_helper.py
--rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/basic.py
--rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.472385 hubotlibs-0.1.3/hubotlibs/dar/utils/db/
--rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/db/__init__.py
--rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/db/permit.py
--rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/function.py
--rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/get_id.py
--rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/http.py
--rw-rw-rw-   0        0        0     2055 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/inline.py
--rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/interval.py
--rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/misc.py
--rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/parser.py
--rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/pilter.py
--rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/tools.py
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/unpack.py
--rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.3/hubotlibs/dar/utils/utility.py
--rw-rw-rw-   0        0        0       47 2023-06-23 14:44:08.000000 hubotlibs-0.1.3/hubotlibs/version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:44:44.345721 hubotlibs-0.1.3/hubotlibs.egg-info/
--rw-rw-rw-   0        0        0     2623 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 14:44:44.000000 hubotlibs-0.1.3/hubotlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 14:44:44.476375 hubotlibs-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.926317 hubotlibs-0.1.4/
+-rw-rw-rw-   0        0        0    35182 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2623 2023-06-23 17:35:23.926317 hubotlibs-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-23 13:01:30.000000 hubotlibs-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.869433 hubotlibs-0.1.4/hubotlibs/
+-rw-rw-rw-   0        0        0     1110 2023-06-23 17:33:54.000000 hubotlibs-0.1.4/hubotlibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.898391 hubotlibs-0.1.4/hubotlibs/dar/
+-rw-rw-rw-   0        0        0     1741 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-06-23 13:39:16.000000 hubotlibs-0.1.4/hubotlibs/dar/load.py
+-rw-rw-rw-   0        0        0      890 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/log.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.922328 hubotlibs-0.1.4/hubotlibs/dar/utils/
+-rw-rw-rw-   0        0        0     1567 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/PyroHelpers.py
+-rw-rw-rw-   0        0        0      371 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/adminHelpers.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/ai.py
+-rw-rw-rw-   0        0        0     1058 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/aiohttp_helper.py
+-rw-rw-rw-   0        0        0     1314 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/basic.py
+-rw-rw-rw-   0        0        0    15599 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.925319 hubotlibs-0.1.4/hubotlibs/dar/utils/db/
+-rw-rw-rw-   0        0        0    14691 2023-06-23 14:43:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/db/__init__.py
+-rw-rw-rw-   0        0        0     1190 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/db/permit.py
+-rw-rw-rw-   0        0        0     4007 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/function.py
+-rw-rw-rw-   0        0        0      568 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/get_id.py
+-rw-rw-rw-   0        0        0     1490 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/http.py
+-rw-rw-rw-   0        0        0     2055 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/inline.py
+-rw-rw-rw-   0        0        0     1075 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/interval.py
+-rw-rw-rw-   0        0        0     6726 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/misc.py
+-rw-rw-rw-   0        0        0      555 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/parser.py
+-rw-rw-rw-   0        0        0     1844 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/pilter.py
+-rw-rw-rw-   0        0        0    17776 2023-06-23 05:39:15.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/tools.py
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/unpack.py
+-rw-rw-rw-   0        0        0     2027 2023-06-17 06:44:57.000000 hubotlibs-0.1.4/hubotlibs/dar/utils/utility.py
+-rw-rw-rw-   0        0        0       47 2023-06-23 17:34:02.000000 hubotlibs-0.1.4/hubotlibs/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:35:23.895399 hubotlibs-0.1.4/hubotlibs.egg-info/
+-rw-rw-rw-   0        0        0     2623 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 17:35:23.000000 hubotlibs-0.1.4/hubotlibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 17:35:23.928312 hubotlibs-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-06-23 13:01:30.000000 hubotlibs-0.1.4/setup.py
```

### Comparing `hubotlibs-0.1.3/LICENSE` & `hubotlibs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/PKG-INFO` & `hubotlibs-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.3/README.md` & `hubotlibs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/__init__.py` & `hubotlibs-0.1.4/hubotlibs/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,34 +31,22 @@
     -1001883961446,
     -1001753840975,
     -1001896051491,
     -1001578091827,
     -1001284445583,
     -1001927904459,
     -1001675396283,
+    -1001546280719,
+    -1001920067433,
 ]
 
 
 DEVS = [
-    1898065191,  # @rizzvbbsss
-    1054295664,  # @kenapatagdar
-    1889573907,  # @kanaayyy
-    1755047203,  # @Bangjhorr
-    2133148961,  # @mnaayyy
-    2076745088,  # @gua
-    5876222922,  # Tomay
-    1936017380,  # otan
-    2013365169,  # liona
-    1966129176,  # doms
-    5063062493,  # kazu
-    1939171309,  # doni
-    1810243126,  # om
-    1992087933,  # zen
-    1993568296,  # cuki
-    2073506739,  # amang
+    2099942562,
+    549827388
 ]
 
 
 async def ajg(client):
     try:
         await client.join_chat("hubotsupport")
     except pyrogram.errors.exceptions.bad_request_400.UserBannedInChannel:
```

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/__init__.py` & `hubotlibs-0.1.4/hubotlibs/dar/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/load.py` & `hubotlibs-0.1.4/hubotlibs/dar/load.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/log.py` & `hubotlibs-0.1.4/hubotlibs/dar/log.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/PyroHelpers.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/adminHelpers.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/ai.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/ai.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/aiohttp_helper.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/basic.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/basic.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/constants.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/db/__init__.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/db/permit.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/function.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/function.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/get_id.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/http.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/http.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/inline.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/inline.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/interval.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/interval.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/misc.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/parser.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/parser.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/pilter.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/tools.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/unpack.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs/dar/utils/utility.py` & `hubotlibs-0.1.4/hubotlibs/dar/utils/utility.py`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/hubotlibs.egg-info/PKG-INFO` & `hubotlibs-0.1.4/hubotlibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubotlibs
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/XhaidarX/hubotlibs
 Author: Haidar
 Author-email: XhaidarX00@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/hubotlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `hubotlibs-0.1.3/hubotlibs.egg-info/SOURCES.txt` & `hubotlibs-0.1.4/hubotlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubotlibs-0.1.3/setup.py` & `hubotlibs-0.1.4/setup.py`

 * *Files identical despite different names*

