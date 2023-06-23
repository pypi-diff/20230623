# Comparing `tmp/nonebot_plugin_al-0.3.4.tar.gz` & `tmp/nonebot_plugin_al-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.5.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.4.tar` & `nonebot_plugin_al-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/LICENSE
--rw-r--r--   0        0        0     4110 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/README.md
--rw-r--r--   0        0        0     6368 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    70845 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3348 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0     1790 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/config.py
--rw-r--r--   0        0        0    69109 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10152 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7691 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13687 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     5972 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1055 2023-06-21 02:11:17.616454 nonebot_plugin_al-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-23 03:29:04.640192 nonebot_plugin_al-0.3.5/LICENSE
+-rw-r--r--   0        0        0     4110 2023-06-23 03:29:04.640192 nonebot_plugin_al-0.3.5/README.md
+-rw-r--r--   0        0        0     6408 2023-06-23 03:29:04.640192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    70845 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3348 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0     1826 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/config.py
+-rw-r--r--   0        0        0    69109 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10152 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7691 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13687 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5820 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1055 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.5/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.4/LICENSE` & `nonebot_plugin_al-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/README.md` & `nonebot_plugin_al-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
+from nonebot import require
+require('nonebot_plugin_htmlrender')
 
 from nonebot import on_command
 from nonebot.permission import SUPERUSER
 from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters.onebot.v11 import (
     Message,
     MessageSegment,
-    Bot,
-    Event,
-    GroupMessageEvent,
 )
-import traceback
 from pathlib import Path
 try:
     import ujson as json
 except:
     import json
 
 
@@ -99,24 +97,24 @@
         # 井号榜
         await matcher.finish(MessageSegment.image(await get_data(await jinghao(word))))
     elif word.startswith("角色"):
         # 舰船搜索
         with open((Path(__file__).parent.joinpath("data/ship.json")),
           mode='r',encoding='utf-8')as f:
             ships = json.load(f)
-        word = word.replace("角色","")
+        word = word.replace("角色","").replace(" ", "")
         for key, value in ships.items():
             if any(word in sublist for sublist in value):
                 await matcher.finish(MessageSegment.image(await get_ship_msg(key)))
         await matcher.finish("没有这个角色~")
     elif word.startswith("装备"):
         with open((Path(__file__).parent.joinpath("data/eq.json")),
           mode='r',encoding='utf-8')as f:
             eq = json.load(f)
-        word = word.replace("装备","")
+        word = word.replace("装备","").replace(" ", "")
         for key, value in eq.items():
             if any(word in sublist for sublist in value):
                 await matcher.finish(MessageSegment.image(await get_ship_msg(key)))
         await matcher.finish("没有这个装备~")
     else:
         await matcher.finish()
         
@@ -181,8 +179,8 @@
     handlers=[blhx.quick_search_skin]
 )
 on_command(
     "blhx 大建", 
     block=True, 
     priority=10,
     handlers=[blhx.building]
-)
+)
```

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/config.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from nonebot import get_driver
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
 )
 
-CONFIG_PATH = Path().joinpath('data/al')
+CONFIG_PATH = Path().joinpath('data/al/config.yml')
 
 driver = get_driver()
 COMMAND_START = list[driver.config.command_start]
 try:
     NICKNAME: str = list(driver.config.nickname)[0]
 except Exception:
-    NICKNAME = 'bot'
+    NICKNAME = '小加加(VC装甲钢36D版)'
 
 
 ADMIN = SUPERUSER | GROUP_ADMIN | GROUP_OWNER 
 # ADMINISTRATOR = SUPERUSER | GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND
 
 
 class AzurConfig(BaseModel):
```

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/send_message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.4/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.5/nonebot_plugin_al/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 from pathlib import Path
 from nonebot import get_bot
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot_plugin_htmlrender import html_to_pic
 from nonebot.log import logger
 
+from .config import NICKNAME
 SAVE_PATH = Path().joinpath('data/al')
 tool_path = SAVE_PATH.joinpath('wkhtmltopdf', 'bin', 'wkhtmltoimage.exe')
 """
 方法名：print_img
 参数列表：无
 用处：调用打印工具，打印ship_info.html成图片
 返回值：无返回值，从html文件夹里读取html文件，打印的图片输出到images文件夹
@@ -152,20 +153,15 @@
     async with aiofiles.open(SAVE_PATH.joinpath('azurapi_data', 'version-info.json'), 'r',
               encoding='utf-8') as load_f:
         load_dict = await load_f.read()
         load_dict:dict = json.loads(load_dict)
         load_dict:dict = json.loads(load_dict) # 别删除，否则会有类型错误
     return load_dict['ships']
 
-def render_forward_msg(msg_list: list, uid=1916714922, name='小加加(VC装甲钢36D版)',bot:Bot = None):
-    try:
-        uid = bot.self_id
-        name = list(bot.config.nickname)[0]
-    except Exception as e:
-        logger.warning(f'获取bot信息错误\n{e}')
+def render_forward_msg(msg_list: list, uid=1916714922, name=NICKNAME ,bot:Bot = None):
     forward_msg = []
     for msg in msg_list:
         forward_msg.append({
             "type": "node",
             "data": {
                 "name": str(name),
                 "uin": str(uid),
```

### Comparing `nonebot_plugin_al-0.3.4/pyproject.toml` & `nonebot_plugin_al-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.4"
+version = "0.3.5"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
```

### Comparing `nonebot_plugin_al-0.3.4/PKG-INFO` & `nonebot_plugin_al-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.4
+Version: 0.3.5
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.4 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.5 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

