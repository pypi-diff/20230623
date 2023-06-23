# Comparing `tmp/nonebot_plugin_callapi-0.1.2.tar.gz` & `tmp/nonebot_plugin_callapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_callapi-0.1.2.tar", last modified: Sun Jun  4 17:15:57 2023, max compression
+gzip compressed data, was "nonebot_plugin_callapi-0.1.3.tar", last modified: Fri Jun 23 17:38:12 2023, max compression
```

## Comparing `nonebot_plugin_callapi-0.1.2.tar` & `nonebot_plugin_callapi-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/LICENSE
--rw-r--r--   0        0        0     4572 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/README.md
--rw-r--r--   0        0        0      462 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/__init__.py
--rw-r--r--   0        0        0     8442 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/__main__.py
--rw-r--r--   0        0        0      197 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/config.py
--rw-r--r--   0        0        0      661 2023-06-04 17:15:57.382979 nonebot_plugin_callapi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5178 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4723 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/README.md
+-rw-r--r--   0        0        0      530 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/__init__.py
+-rw-r--r--   0        0        0     7567 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/__main__.py
+-rw-r--r--   0        0        0      197 2023-06-23 17:38:00.305867 nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/config.py
+-rw-r--r--   0        0        0      661 2023-06-23 17:38:12.728107 nonebot_plugin_callapi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_callapi-0.1.2/LICENSE` & `nonebot_plugin_callapi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.2/README.md` & `nonebot_plugin_callapi-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -156,10 +156,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.1.3
+
+- 删除插件自身对 Telegram 消息发送的兼容，现在发送 Telegram 消息使用 SAA 接管
+
+### 0.1.2
+
+- 🎉 NoneBot 2.0 🚀
+
 ### 0.1.1
 
 - 修复文本类 Segment 未做转义处理的问题
```

#### html2text {}

```diff
@@ -35,9 +35,11 @@
 github.com/MeetWq/pil-utils) è¶å¥½ç¨ç Pillow è¾å©åº ### [felinae98/
 nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere)
 å¤ééå¨æ¶æ¯åéæ¯æï¼æ¬æä»¶ç¨æ¥åéå¾çï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.3 - å é¤æä»¶èªèº«å¯¹
+Telegram æ¶æ¯åéçå¼å®¹ï¼ç°å¨åé Telegram æ¶æ¯ä½¿ç¨ SAA æ¥ç®¡
+### 0.1.2 - ð NoneBot 2.0 ð ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
 æªåè½¬ä¹å¤ççé®é¢
```

### Comparing `nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/__main__.py` & `nonebot_plugin_callapi-0.1.3/nonebot_plugin_callapi/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 import json
 import traceback
 from contextlib import suppress
 from dataclasses import dataclass
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, cast
 
 from bbcode import Parser as BBCodeParser
-from nonebot import on_command, require
+from nonebot import on_command
 from nonebot.internal.adapter import Bot, Message, MessageSegment
 from nonebot.log import logger
 from nonebot.matcher import Matcher, current_bot, current_event
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
+from nonebot_plugin_saa import Image as SAAImage
+from nonebot_plugin_saa import MessageFactory
 from PIL import Image
 from pil_utils import BuildImage, Text2Image
 from pil_utils.fonts import DEFAULT_FALLBACK_FONTS
 from pydantic import BaseModel
 from pygments import highlight
 from pygments.formatters import BBCodeFormatter
 from pygments.lexers import get_lexer_by_name
 from pygments.style import Style
 
-try:
-    from nonebot.adapters.telegram.event import MessageEvent as TgMsgEvent
-    from nonebot.adapters.telegram.message import File as TgFile
-except ImportError:
-    TgEvent = None
-
 from .config import config
 
-require("nonebot_plugin_saa")
-from nonebot_plugin_saa import Image as SAAImage  # noqa: E402
-from nonebot_plugin_saa import MessageFactory  # noqa: E402
-
 CODE_FONTS = [
     "JetBrains Mono",
     "Cascadia Mono",
     "Segoe UI Mono",
     "Liberation Mono",
     "Menlo",
     "Monaco",
@@ -140,47 +132,26 @@
     for img in images:
         bg.paste(img, (PADDING, y), alpha=True)
         y += img.height
 
     return bg.convert("RGB").save("png").getvalue()
 
 
-# async def send_return(items: List[Union[str, Codeblock]]):
-#     if config.callapi_pic:
-#         with suppress(Exception):
-#             image = draw_image(items)
-#             await MessageFactory(SAAImage(image)).send(reply=True)
-#             return
-
-#     event = current_event.get()
-#     bot = current_bot.get()
-#     await bot.send(event, format_plain_text(items))
-
-
 async def send_return(items: List[Union[str, Codeblock]]):
     event = current_event.get()
     bot = current_bot.get()
 
     if config.callapi_pic:
-        with suppress(Exception):
-            if TgEvent and isinstance(event, TgMsgEvent):
-                # telegram
-                image = draw_image(items)
-                await bot.send(
-                    event,
-                    TgFile.photo(image),
-                    reply_to_message_id=event.message_id,
-                )
-
-            else:
-                # via saa
-                image = draw_image(items)
-                await MessageFactory(SAAImage(image)).send(reply=True)
-
-            return
+        try:
+            # via saa
+            image = draw_image(items)
+            await MessageFactory(SAAImage(image)).send(reply=True)
+        except Exception:
+            logger.exception("Error when sending image via saa, fallback to plain text")
+        return
 
     await bot.send(event, format_plain_text(items))
 
 
 def cast_param_type(param: str) -> Any:
     if param.isdigit():
         return int(param)
```

### Comparing `nonebot_plugin_callapi-0.1.2/pyproject.toml` & `nonebot_plugin_callapi-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "nonebot-plugin-callapi"
-version = "0.1.2"
+version = "0.1.3"
 description = "Use bot command to call its API"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.0",
     "pydantic>=1.10.4",
     "Pygments>=2.15.1",
     "pil-utils>=0.1.7",
-    "nonebot-plugin-send-anything-anywhere>=0.2.4",
+    "nonebot-plugin-send-anything-anywhere>=0.2.5",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_callapi-0.1.2/PKG-INFO` & `nonebot_plugin_callapi-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-callapi
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use bot command to call its API
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
 Requires-Dist: pydantic>=1.10.4
 Requires-Dist: Pygments>=2.15.1
 Requires-Dist: pil-utils>=0.1.7
-Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
+Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.5
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
@@ -173,10 +173,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.1.3
+
+- 删除插件自身对 Telegram 消息发送的兼容，现在发送 Telegram 消息使用 SAA 接管
+
+### 0.1.2
+
+- 🎉 NoneBot 2.0 🚀
+
 ### 0.1.1
 
 - 修复文本类 Segment 未做转义处理的问题
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.2 Summary: Use
+Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.3 Summary: Use
 bot command to call its API Home-page: https://github.com/lgc-NB2Dev/nonebot-
 plugin-callapi Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-callapi Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
 pydantic>=1.10.4 Requires-Dist: Pygments>=2.15.1 Requires-Dist: pil-
-utils>=0.1.7 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
+utils>=0.1.7 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.5
 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # NoneBot-Plugin-CallAPI _â¨ ä½¿ç¨æä»¤æ¥è°ç¨ Bot ç API â¨_ [python]
                            [pdm-managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç» ä½¿ç¨ Bot æä»¤æ¥ç´æ¥è°ç¨ Bot ç API å§ï¼
@@ -44,9 +44,11 @@
 github.com/MeetWq/pil-utils) è¶å¥½ç¨ç Pillow è¾å©åº ### [felinae98/
 nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere)
 å¤ééå¨æ¶æ¯åéæ¯æï¼æ¬æä»¶ç¨æ¥åéå¾çï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.3 - å é¤æä»¶èªèº«å¯¹
+Telegram æ¶æ¯åéçå¼å®¹ï¼ç°å¨åé Telegram æ¶æ¯ä½¿ç¨ SAA æ¥ç®¡
+### 0.1.2 - ð NoneBot 2.0 ð ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
 æªåè½¬ä¹å¤ççé®é¢
```

