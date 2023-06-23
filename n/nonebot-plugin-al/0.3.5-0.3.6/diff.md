# Comparing `tmp/nonebot_plugin_al-0.3.5.tar.gz` & `tmp/nonebot_plugin_al-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.6.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.5.tar` & `nonebot_plugin_al-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-06-23 03:29:04.640192 nonebot_plugin_al-0.3.5/LICENSE
--rw-r--r--   0        0        0     4110 2023-06-23 03:29:04.640192 nonebot_plugin_al-0.3.5/README.md
--rw-r--r--   0        0        0     6408 2023-06-23 03:29:04.640192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    70845 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3348 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0     1826 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/config.py
--rw-r--r--   0        0        0    69109 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10152 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7691 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13687 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     5820 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1055 2023-06-23 03:29:04.644192 nonebot_plugin_al-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/LICENSE
+-rw-r--r--   0        0        0     4218 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/README.md
+-rw-r--r--   0        0        0     6408 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    70845 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3348 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0     1961 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/config.py
+-rw-r--r--   0        0        0    69109 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10142 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7691 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13688 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5792 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1055 2023-06-23 05:01:03.632173 nonebot_plugin_al-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.6/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.5/LICENSE` & `nonebot_plugin_al-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.5/README.md` & `nonebot_plugin_al-0.3.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 git clone https://github.com/Agnes4m/nonebot_plugin_AL.git
 ```
 
 ## 资源包
 
 本项的图片资源基本都来源于本地，具体在项目的images文件夹里，大小在3.5G左右，项目在[api](https://github.com/AzurAPI/azurapi-js-setup) 打包下载，将下载来的项目里的images文件夹放入bot目录下`data/al/ship_html`里面，也就是说路径为`data/al/ship_html/images/`这点十分重要，blhx_wiki功能90%依赖这个资源包，请自行留意它的更新
 
+<!-- 除了图片文件，还有一些其它的，比如原作者仓库的 一些(划掉) 好多东西 -->
+
 百度云盘：链接：https://pan.baidu.com/s/1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk 
 提取码：57uk
 
 ## 指令
 
 ### 【总】碧蓝帮助 | 碧蓝指令
```

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/config.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
 )
 
 CONFIG_PATH = Path().joinpath('data/al/config.yml')
-
+CONFIG_PATH.parent.mkdir(parents=True,exist_ok=True)
 driver = get_driver()
 COMMAND_START = list[driver.config.command_start]
 try:
     NICKNAME: str = list(driver.config.nickname)[0]
 except Exception:
     NICKNAME = '小加加(VC装甲钢36D版)'
 
@@ -45,14 +45,16 @@
         self.save()
 
     @property
     def config_list(self) -> List[str]:
         return list(self.config.dict(by_alias=True).keys())
 
     def save(self):
+        if not os.path.exists("./data/al/"):
+            os.makedirs("./data/al/")
         with self.file_path.open('w', encoding='utf-8') as f:
             yaml.dump(
                 self.config.dict(by_alias=True),
                 f,
                 indent=2,
                 Dumper=yaml.RoundTripDumper,
                 allow_unicode=True)
```

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 from PIL import Image, ImageDraw, ImageFont
-import os
 from .api import get_ship_data_by_id
 import asyncio
 
 
 from .name import *
 # 这个数组存放的是每张卡的中心点位置
 GACHA_OFFSET = [(389, 366), (649, 366), (909, 366), (1169, 366), (1429, 366),
```

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/send_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         #             "兵装推荐榜\n", "专武推荐榜\n", "兑换装备推荐榜\n", "研发装备推荐榜\n", "改造推荐榜\n", "跨队舰船推荐榜\n",
         #             "氪金榜\n" , "打捞主线榜\n","打捞作战榜'\n"]
         msg = "仅代表个人观点，完全不等于绝对客观，可能存在各种主观评判或者真爱加成，不过目标是努力去进行符合环境需求的客观评定\n"
         msg_list = []
         if len(div_list) != 0:
             for i in range(0, len(div_list)):
                 msg += Message(str(div_list[i].find('img')['alt']) + MessageSegment.image(file=str(div_list[i].find('img')['src'])) + "\n")
-                msg_list.append(msg)
+            msg_list.append(msg)
             forward_msg = render_forward_msg(msg_list,bot=bot)
             if isinstance(event,GroupMessageEvent):
                 await bot.call_api('send_group_forward_msg',group_id=event.group_id, messages=forward_msg)
                 return
         else:
             await bot.send(event=event,message='暂无信息', at_sender=True)
 
@@ -144,27 +144,27 @@
         arg:Message = CommandArg()
         ):
 
         logger.info("命令确认，正在删除")
         try:
             await bot.send(event=event,message='正在更新，首先请确保网络能访问github的文件中心，否则容易出现翻车风险！', at_sender=True)
             await force_update_offline()
-            os.rename(PATH, BACK_PATH)  # 备份源文件省得出意外翻车
+            Path(PATH).rename(BACK_PATH)  # 备份源文件省得出意外翻车
             await force_update_offline()  # 再更新
             shutil.rmtree(BACK_PATH)  # 更新完成再删除备份
             version_info = await get_local_version()
             version = str(version_info['version-number'])
             await UpdateName()
             await bot.send(event=event,message='强制更新完成.强制更新内容仅在离线模式下有效，当前版本V'+version, at_sender=True)
         except:
             # 出问题赶紧回滚
             traceback.print_exc()
             await bot.send(event=event,message='更新失败！尝试回滚...', at_sender=True)
             try:
-                os.rename(BACK_PATH, PATH)
+                Path(BACK_PATH).rename(PATH)
                 await bot.send(event=event,message='回滚成功，差点您就没了。', at_sender=True)
             except:
                 await bot.send(event=event,message=f'回滚失败！', at_sender=True)
 
 
     async def get_recently_event(        
         matcher:Matcher,
@@ -310,8 +310,8 @@
             traceback.print_exc()
             await bot.send(event=event,message=str(msg), at_sender=True)
             return
 
 
 
 
-blhx = BLHX_BASE()
+blhx = BLHX_BASE()
```

### Comparing `nonebot_plugin_al-0.3.5/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.6/nonebot_plugin_al/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import cv2
 import pypinyin
 import json
 import aiofiles
 
 from typing import Optional
 from pathlib import Path
-from nonebot import get_bot
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot_plugin_htmlrender import html_to_pic
 from nonebot.log import logger
 
 from .config import NICKNAME
 SAVE_PATH = Path().joinpath('data/al')
 tool_path = SAVE_PATH.joinpath('wkhtmltopdf', 'bin', 'wkhtmltoimage.exe')
```

### Comparing `nonebot_plugin_al-0.3.5/pyproject.toml` & `nonebot_plugin_al-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.5"
+version = "0.3.6"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
```

### Comparing `nonebot_plugin_al-0.3.5/PKG-INFO` & `nonebot_plugin_al-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.5
+Version: 0.3.6
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -86,14 +86,16 @@
 git clone https://github.com/Agnes4m/nonebot_plugin_AL.git
 ```
 
 ## 资源包
 
 本项的图片资源基本都来源于本地，具体在项目的images文件夹里，大小在3.5G左右，项目在[api](https://github.com/AzurAPI/azurapi-js-setup) 打包下载，将下载来的项目里的images文件夹放入bot目录下`data/al/ship_html`里面，也就是说路径为`data/al/ship_html/images/`这点十分重要，blhx_wiki功能90%依赖这个资源包，请自行留意它的更新
 
+<!-- 除了图片文件，还有一些其它的，比如原作者仓库的 一些(划掉) 好多东西 -->
+
 百度云盘：链接：https://pan.baidu.com/s/1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk 
 提取码：57uk
 
 ## 指令
 
 ### 【总】碧蓝帮助 | 碧蓝指令
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.5 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.6 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

