# Comparing `tmp/nonebot-plugin-ocgbot-v2-0.1.0.tar.gz` & `tmp/nonebot-plugin-ocgbot-v2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-ocgbot-v2-0.1.0.tar", last modified: Fri Jun 23 06:38:58 2023, max compression
+gzip compressed data, was "nonebot-plugin-ocgbot-v2-0.1.1.tar", last modified: Fri Jun 23 07:40:01 2023, max compression
```

## Comparing `nonebot-plugin-ocgbot-v2-0.1.0.tar` & `nonebot-plugin-ocgbot-v2-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 06:38:58.793117 nonebot-plugin-ocgbot-v2-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-06-23 05:31:03.000000 nonebot-plugin-ocgbot-v2-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4184 2023-06-23 06:38:58.793117 nonebot-plugin-ocgbot-v2-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3983 2023-06-23 05:51:25.000000 nonebot-plugin-ocgbot-v2-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 06:38:58.708501 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/
--rw-rw-rw-   0        0        0     3190 2023-06-23 06:04:43.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/__init__.py
--rw-rw-rw-   0        0        0    65672 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/cardPieChart.py
--rw-rw-rw-   0        0        0      178 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/config.py
--rw-rw-rw-   0        0        0     5179 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/daily.py
--rw-rw-rw-   0        0        0      585 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/data_update.py
--rw-rw-rw-   0        0        0    15072 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/guess_card.py
--rw-rw-rw-   0        0        0     1368 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/help.py
-drwxrwxrwx   0        0        0        0 2023-06-23 06:38:58.793117 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/
--rw-rw-rw-   0        0        0    10019 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/Card.py
--rw-rw-rw-   0        0        0      597 2023-06-22 10:09:41.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py
--rw-rw-rw-   0        0        0     3315 2023-06-23 06:01:38.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py
--rw-rw-rw-   0        0        0     1434 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py
--rw-rw-rw-   0        0        0     5252 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/guessManage.py
--rw-rw-rw-   0        0        0     4241 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/image.py
--rw-rw-rw-   0        0        0     4773 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py
--rw-rw-rw-   0        0        0      978 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py
--rw-rw-rw-   0        0        0     2197 2022-09-19 08:41:41.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/searchManage.py
--rw-rw-rw-   0        0        0     9795 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/sendAction.py
--rw-rw-rw-   0        0        0       69 2023-06-23 04:16:42.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/staticvar.py
--rw-rw-rw-   0        0        0      581 2023-06-08 00:48:04.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/tool.py
--rw-rw-rw-   0        0        0     1665 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/maiPic.py
--rw-rw-rw-   0        0        0     7947 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/ocg.py
--rw-rw-rw-   0        0        0     2216 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/priceSearch.py
-drwxrwxrwx   0        0        0        0 2023-06-23 06:38:58.777494 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2.egg-info/
--rw-rw-rw-   0        0        0     4184 2023-06-23 06:38:58.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-06-23 06:38:58.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 06:38:58.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-23 06:38:58.000000 nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      402 2023-06-23 06:31:23.000000 nonebot-plugin-ocgbot-v2-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 06:38:58.793117 nonebot-plugin-ocgbot-v2-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.663509 nonebot-plugin-ocgbot-v2-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-06-23 05:31:03.000000 nonebot-plugin-ocgbot-v2-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4184 2023-06-23 07:40:01.663231 nonebot-plugin-ocgbot-v2-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3983 2023-06-23 05:51:25.000000 nonebot-plugin-ocgbot-v2-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.628514 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/
+-rw-rw-rw-   0        0        0     3190 2023-06-23 06:04:43.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/__init__.py
+-rw-rw-rw-   0        0        0    65672 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/cardPieChart.py
+-rw-rw-rw-   0        0        0      178 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/config.py
+-rw-rw-rw-   0        0        0     5127 2023-06-23 07:31:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/daily.py
+-rw-rw-rw-   0        0        0      585 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/data_update.py
+-rw-rw-rw-   0        0        0    15072 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/guess_card.py
+-rw-rw-rw-   0        0        0     1368 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/help.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.647580 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/
+-rw-rw-rw-   0        0        0    10019 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/Card.py
+-rw-rw-rw-   0        0        0      597 2023-06-22 10:09:41.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py
+-rw-rw-rw-   0        0        0     3315 2023-06-23 06:01:38.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py
+-rw-rw-rw-   0        0        0     1434 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py
+-rw-rw-rw-   0        0        0     5252 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/guessManage.py
+-rw-rw-rw-   0        0        0     4197 2023-06-23 07:31:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/image.py
+-rw-rw-rw-   0        0        0     4773 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py
+-rw-rw-rw-   0        0        0      978 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py
+-rw-rw-rw-   0        0        0     2197 2022-09-19 08:41:41.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/searchManage.py
+-rw-rw-rw-   0        0        0     9795 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/sendAction.py
+-rw-rw-rw-   0        0        0       69 2023-06-23 04:16:42.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/staticvar.py
+-rw-rw-rw-   0        0        0      581 2023-06-08 00:48:04.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/tool.py
+-rw-rw-rw-   0        0        0     1665 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/maiPic.py
+-rw-rw-rw-   0        0        0     7947 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/ocg.py
+-rw-rw-rw-   0        0        0     2216 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/priceSearch.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.628514 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/
+-rw-rw-rw-   0        0        0     4184 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1172 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      611 2023-06-23 07:39:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:40:01.663509 nonebot-plugin-ocgbot-v2-0.1.1/setup.cfg
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/LICENSE` & `nonebot-plugin-ocgbot-v2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/PKG-INFO` & `nonebot-plugin-ocgbot-v2-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ocgbot-v2
-Version: 0.1.0
+Version: 0.1.1
 Summary: nonebot-plugin-ocgbot-v2
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.1 Summary:
 nonebot-plugin-ocgbot-v2 Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-ocgbot-v2 _â¨ æä¾æ¸¸æçç¸å³æå¡ â¨_ [license]
                                 [pypi] [python]
 æä¾åæ¬æ¥å¡ãéæºæ½å¡ãçå¡ç­åè½çæä»¶ ## ð ä»ç»
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/README.md` & `nonebot-plugin-ocgbot-v2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/__init__.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/cardPieChart.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/cardPieChart.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/daily.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/daily.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import copy
+
 import datetime
-from io import BytesIO
 
-import requests
 from PIL import Image, ImageFont, ImageDraw
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import Bot, Event, Message, MessageSegment
 from nonebot.typing import T_State
 
 from nonebot_plugin_ocgbot_v2.libraries.globalMessage import static_path, image_path,font_path
 from nonebot_plugin_ocgbot_v2.libraries.staticvar import daily_card
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/data_update.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/data_update.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/guess_card.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/guess_card.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/help.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/help.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/Card.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/Card.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/guessManage.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/guessManage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/image.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import base64
 from io import BytesIO
 
-import nonebot
 from PIL import ImageFont, ImageDraw, Image
-from nonebot import Config
 
 from nonebot_plugin_ocgbot_v2.libraries.globalMessage import font_path,image_path
 
 fontpath = font_path+"msyh.ttc"
 background = Image.open(image_path+"background.png")
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/searchManage.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/searchManage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/sendAction.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/sendAction.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/libraries/tool.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/tool.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/maiPic.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/maiPic.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/ocg.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/ocg.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2/priceSearch.py` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/priceSearch.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ocgbot-v2
-Version: 0.1.0
+Version: 0.1.1
 Summary: nonebot-plugin-ocgbot-v2
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.1 Summary:
 nonebot-plugin-ocgbot-v2 Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-ocgbot-v2 _â¨ æä¾æ¸¸æçç¸å³æå¡ â¨_ [license]
                                 [pypi] [python]
 æä¾åæ¬æ¥å¡ãéæºæ½å¡ãçå¡ç­åè½çæä»¶ ## ð ä»ç»
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.0/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt` & `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

