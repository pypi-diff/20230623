# Comparing `tmp/nonebot-plugin-ocgbot-v2-0.1.1.tar.gz` & `tmp/nonebot-plugin-ocgbot-v2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-ocgbot-v2-0.1.1.tar", last modified: Fri Jun 23 07:40:01 2023, max compression
+gzip compressed data, was "nonebot-plugin-ocgbot-v2-0.1.2.tar", last modified: Fri Jun 23 08:22:35 2023, max compression
```

## Comparing `nonebot-plugin-ocgbot-v2-0.1.1.tar` & `nonebot-plugin-ocgbot-v2-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.663509 nonebot-plugin-ocgbot-v2-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-06-23 05:31:03.000000 nonebot-plugin-ocgbot-v2-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4184 2023-06-23 07:40:01.663231 nonebot-plugin-ocgbot-v2-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3983 2023-06-23 05:51:25.000000 nonebot-plugin-ocgbot-v2-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.628514 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/
--rw-rw-rw-   0        0        0     3190 2023-06-23 06:04:43.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/__init__.py
--rw-rw-rw-   0        0        0    65672 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/cardPieChart.py
--rw-rw-rw-   0        0        0      178 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/config.py
--rw-rw-rw-   0        0        0     5127 2023-06-23 07:31:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/daily.py
--rw-rw-rw-   0        0        0      585 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/data_update.py
--rw-rw-rw-   0        0        0    15072 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/guess_card.py
--rw-rw-rw-   0        0        0     1368 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/help.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.647580 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/
--rw-rw-rw-   0        0        0    10019 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/Card.py
--rw-rw-rw-   0        0        0      597 2023-06-22 10:09:41.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py
--rw-rw-rw-   0        0        0     3315 2023-06-23 06:01:38.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py
--rw-rw-rw-   0        0        0     1434 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py
--rw-rw-rw-   0        0        0     5252 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/guessManage.py
--rw-rw-rw-   0        0        0     4197 2023-06-23 07:31:29.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/image.py
--rw-rw-rw-   0        0        0     4773 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py
--rw-rw-rw-   0        0        0      978 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py
--rw-rw-rw-   0        0        0     2197 2022-09-19 08:41:41.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/searchManage.py
--rw-rw-rw-   0        0        0     9795 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/sendAction.py
--rw-rw-rw-   0        0        0       69 2023-06-23 04:16:42.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/staticvar.py
--rw-rw-rw-   0        0        0      581 2023-06-08 00:48:04.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/tool.py
--rw-rw-rw-   0        0        0     1665 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/maiPic.py
--rw-rw-rw-   0        0        0     7947 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/ocg.py
--rw-rw-rw-   0        0        0     2216 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/priceSearch.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:40:01.628514 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/
--rw-rw-rw-   0        0        0     4184 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-23 07:40:01.000000 nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      611 2023-06-23 07:39:39.000000 nonebot-plugin-ocgbot-v2-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 07:40:01.663509 nonebot-plugin-ocgbot-v2-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 08:22:35.186909 nonebot-plugin-ocgbot-v2-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-23 05:31:03.000000 nonebot-plugin-ocgbot-v2-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4184 2023-06-23 08:22:35.186909 nonebot-plugin-ocgbot-v2-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3983 2023-06-23 05:51:25.000000 nonebot-plugin-ocgbot-v2-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 08:22:35.086454 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/
+-rw-rw-rw-   0        0        0     2667 2023-06-23 07:51:31.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/__init__.py
+-rw-rw-rw-   0        0        0    65672 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/cardPieChart.py
+-rw-rw-rw-   0        0        0      178 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/config.py
+-rw-rw-rw-   0        0        0     5127 2023-06-23 07:31:29.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/daily.py
+-rw-rw-rw-   0        0        0      585 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/data_update.py
+-rw-rw-rw-   0        0        0    15072 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/guess_card.py
+-rw-rw-rw-   0        0        0     1368 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/help.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:22:35.171288 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/
+-rw-rw-rw-   0        0        0    10019 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/Card.py
+-rw-rw-rw-   0        0        0      597 2023-06-22 10:09:41.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py
+-rw-rw-rw-   0        0        0     3315 2023-06-23 06:01:38.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py
+-rw-rw-rw-   0        0        0     1434 2023-06-23 06:09:29.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py
+-rw-rw-rw-   0        0        0     5252 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/guessManage.py
+-rw-rw-rw-   0        0        0     4197 2023-06-23 07:31:29.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/image.py
+-rw-rw-rw-   0        0        0     4773 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py
+-rw-rw-rw-   0        0        0      978 2023-06-23 05:56:40.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py
+-rw-rw-rw-   0        0        0     2197 2022-09-19 08:41:41.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/searchManage.py
+-rw-rw-rw-   0        0        0     9795 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/sendAction.py
+-rw-rw-rw-   0        0        0       69 2023-06-23 04:16:42.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/staticvar.py
+-rw-rw-rw-   0        0        0      581 2023-06-08 00:48:04.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/tool.py
+-rw-rw-rw-   0        0        0     1665 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/maiPic.py
+-rw-rw-rw-   0        0        0     7947 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/ocg.py
+-rw-rw-rw-   0        0        0     2216 2023-06-23 05:56:39.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/priceSearch.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:22:35.155665 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2.egg-info/
+-rw-rw-rw-   0        0        0     4184 2023-06-23 08:22:35.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1172 2023-06-23 08:22:35.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:22:35.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-23 08:22:35.000000 nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      562 2023-06-23 08:22:23.000000 nonebot-plugin-ocgbot-v2-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:22:35.186909 nonebot-plugin-ocgbot-v2-0.1.2/setup.cfg
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/LICENSE` & `nonebot-plugin-ocgbot-v2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/PKG-INFO` & `nonebot-plugin-ocgbot-v2-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ocgbot-v2
-Version: 0.1.1
+Version: 0.1.2
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
-Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.2 Summary:
 nonebot-plugin-ocgbot-v2 Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-ocgbot-v2 _â¨ æä¾æ¸¸æçç¸å³æå¡ â¨_ [license]
                                 [pypi] [python]
 æä¾åæ¬æ¥å¡ãéæºæ½å¡ãçå¡ç­åè½çæä»¶ ## ð ä»ç»
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/README.md` & `nonebot-plugin-ocgbot-v2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/__init__.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,20 @@
 
 __plugin_meta__ = PluginMetadata(
     name="nonbot-plugin-ocgbot-v2",
     description="提供游戏王相关服务",
     usage="提供包括查卡、随机抽卡、猜卡等功能",
 
     type="application",
-    # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
     homepage="https://github.com/fireinsect/nonebot-plugin-ocgbot-v2/",
-    # 发布必填。
 
     config=Config,
-    # 插件配置项类，如无需配置可不填写。
 
-    supported_adapters={"~onebot.v11", "~telegram"},
-    # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
-    # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
+    supported_adapters={"~onebot.v11"},
 )
 
 
 async def nickNameInit():
     nick_path = json_path + "nickname.json"
     try:
         # 尝试读取
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/cardPieChart.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/cardPieChart.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/daily.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/daily.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/data_update.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/data_update.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/guess_card.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/guess_card.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/help.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/help.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/Card.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/Card.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/SqliteUtils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/forbideGet.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/globalMessage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/guessManage.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/guessManage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/image.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/image.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/permissionManage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/raiseCard.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/searchManage.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/searchManage.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/sendAction.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/sendAction.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/libraries/tool.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/libraries/tool.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/maiPic.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/maiPic.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/ocg.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/ocg.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2/priceSearch.py` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2/priceSearch.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ocgbot-v2
-Version: 0.1.1
+Version: 0.1.2
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
-Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ocgbot-v2 Version: 0.1.2 Summary:
 nonebot-plugin-ocgbot-v2 Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-ocgbot-v2 _â¨ æä¾æ¸¸æçç¸å³æå¡ â¨_ [license]
                                 [pypi] [python]
 æä¾åæ¬æ¥å¡ãéæºæ½å¡ãçå¡ç­åè½çæä»¶ ## ð ä»ç»
```

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt` & `nonebot-plugin-ocgbot-v2-0.1.2/nonebot_plugin_ocgbot_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-ocgbot-v2-0.1.1/pyproject.toml` & `nonebot-plugin-ocgbot-v2-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [project]
 name = "nonebot-plugin-ocgbot-v2"
-version = "0.1.1"
+version = "0.1.2"
 description = "nonebot-plugin-ocgbot-v2"
 readme = "README.md"
 requires-python = ">=3.8, <4.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-nonebot2 = ">=2.0.0b3"
-nonebot-adapter-onebot = ">=2.0.0b1"
+nonebot2 = ">=2.0.0"
+nonebot-adapter-onebot = ">=2.2.3"
 requests_html = ">=0.10.0"
 Pillow = ">=9.5.0"
 numpy = ">=1.25.0"
 matplotlib = ">=3.7.1"
 
 [tool.nonebot]
 adapters = [
     { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" }
 ]
-dependencies = [
-    "nonebot2>=2.0.0",
-]
 plugins = []
 plugin_dirs = ["nonebot_plugin_ocgbot_v2"]
 builtin_plugins = ["echo"]
```

