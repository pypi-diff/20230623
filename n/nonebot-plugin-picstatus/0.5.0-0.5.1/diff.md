# Comparing `tmp/nonebot_plugin_picstatus-0.5.0.tar.gz` & `tmp/nonebot_plugin_picstatus-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_picstatus-0.5.0.tar", last modified: Wed Jun  7 13:35:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_picstatus-0.5.1.tar", last modified: Fri Jun 23 17:44:47 2023, max compression
```

## Comparing `nonebot_plugin_picstatus-0.5.0.tar` & `nonebot_plugin_picstatus-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-06-07 13:35:03.242865 nonebot_plugin_picstatus-0.5.0/LICENSE
--rw-r--r--   0        0        0     7150 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/README.md
--rw-r--r--   0        0        0      988 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__init__.py
--rw-r--r--   0        0        0     4123 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__main__.py
--rw-r--r--   0        0        0     1713 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/config.py
--rw-r--r--   0        0        0      251 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/const.py
--rw-r--r--   0        0        0    14152 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/draw.py
--rw-r--r--   0        0        0   378600 2023-06-07 13:35:03.246865 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_avatar.png
--rw-r--r--   0        0        0  1527158 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_bg.png
--rw-r--r--   0        0        0     1393 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/statistics.py
--rw-r--r--   0        0        0    12403 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/status.py
--rw-r--r--   0        0        0     3966 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/util.py
--rw-r--r--   0        0        0       22 2023-06-07 13:35:03.258866 nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/version.py
--rw-r--r--   0        0        0      763 2023-06-07 13:35:16.667914 nonebot_plugin_picstatus-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7830 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-23 17:44:32.675066 nonebot_plugin_picstatus-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7207 2023-06-23 17:44:32.675066 nonebot_plugin_picstatus-0.5.1/README.md
+-rw-r--r--   0        0        0      988 2023-06-23 17:44:32.675066 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/__init__.py
+-rw-r--r--   0        0        0     3844 2023-06-23 17:44:32.675066 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/__main__.py
+-rw-r--r--   0        0        0     1713 2023-06-23 17:44:32.675066 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/config.py
+-rw-r--r--   0        0        0      251 2023-06-23 17:44:32.675066 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/const.py
+-rw-r--r--   0        0        0    14152 2023-06-23 17:44:32.675066 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/draw.py
+-rw-r--r--   0        0        0   378600 2023-06-23 17:44:32.679066 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/res/default_avatar.png
+-rw-r--r--   0        0        0  1527158 2023-06-23 17:44:32.691067 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/res/default_bg.png
+-rw-r--r--   0        0        0     1393 2023-06-23 17:44:32.691067 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/statistics.py
+-rw-r--r--   0        0        0    12403 2023-06-23 17:44:32.691067 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/status.py
+-rw-r--r--   0        0        0     3966 2023-06-23 17:44:32.691067 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/util.py
+-rw-r--r--   0        0        0       22 2023-06-23 17:44:32.691067 nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/version.py
+-rw-r--r--   0        0        0      763 2023-06-23 17:44:47.382938 nonebot_plugin_picstatus-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7887 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-0.5.1/PKG-INFO
```

### Comparing `nonebot_plugin_picstatus-0.5.0/LICENSE` & `nonebot_plugin_picstatus-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/README.md` & `nonebot_plugin_picstatus-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.5.1
+
+- 使用 SAA 向 Telegram 平台发送消息
+
 ### 0.5.0
 
 - 先获取状态信息再进行画图，可以获取到更精准的状态信息
 - 添加进程占用信息的展示
 - 测试网站结果状态码后面会带上 `reason`，如 `200 OK` / `404 Not Found`
 - 添加了一些配置项（`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`, `PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`, `PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`, `PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`）
```

#### html2text {}

```diff
@@ -25,15 +25,16 @@
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ææ¢¦ API](https://api.gumengya.com) -
 éæºèæ¯å¾æ¥æº ### [LoliApi](https://docs.loliapi.com/) -
 éæºèæ¯å¾æ¥æºï¼ææ¶å¼ç¨ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.5.0 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.5.1 - ä½¿ç¨ SAA å Telegram
+å¹³å°åéæ¶æ¯ ### 0.5.0 -
 åè·åç¶æä¿¡æ¯åè¿è¡ç»å¾ï¼å¯ä»¥è·åå°æ´ç²¾åçç¶æä¿¡æ¯
 - æ·»å è¿ç¨å ç¨ä¿¡æ¯çå±ç¤º -
 æµè¯ç½ç«ç»æç¶æç åé¢ä¼å¸¦ä¸ `reason`ï¼å¦ `200 OK` / `404 Not
 Found` - æ·»å äºä¸äºéç½®é¡¹ï¼`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`,
 `PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`,
 `PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`,
 `PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`ï¼ ### 0.4.2 - æ·»å éç½®é¡¹
```

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__init__.py` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/__main__.py` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 try:
     from nonebot.adapters.onebot.v11 import MessageEvent as OBV11MessageEvent
 except:
     OBV11MessageEvent = None
 
 try:
     from nonebot.adapters.telegram.event import MessageEvent as TGMessageEvent
-    from nonebot.adapters.telegram.message import File
 except:
     TGMessageEvent = None
 
 
 async def supported_platform_rule(event: Event):
     if TGMessageEvent and isinstance(event, TGMessageEvent):
         return True
@@ -119,14 +118,8 @@
     try:
         ret = await get_stat_pic(bot, pic)
     except:
         logger.exception("获取运行状态图失败")
         await MessageFactory("获取运行状态图片失败，请检查后台输出").send(reply=config.ps_reply_target)
         await matcher.finish()
 
-    # 为什么 SAA 还不发版支持 TG
-    # 哼哼啊啊啊啊啊啊啊啊啊啊啊啊
-    if TGMessageEvent and isinstance(event, TGMessageEvent):
-        await matcher.finish(File.photo(ret))
-
-    await MessageFactory(Image(ret)).send(reply=config.ps_reply_target)
-    await matcher.finish()
+    await MessageFactory(Image(ret)).finish(reply=config.ps_reply_target)
```

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/config.py` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/draw.py` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_avatar.png` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/res/default_avatar.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/res/default_bg.png` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/res/default_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/statistics.py` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/statistics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/status.py` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/nonebot_plugin_picstatus/util.py` & `nonebot_plugin_picstatus-0.5.1/nonebot_plugin_picstatus/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.5.0/pyproject.toml` & `nonebot_plugin_picstatus-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "nonebot-plugin-picstatus"
-version = "0.5.0"
+version = "0.5.1"
 description = "A NoneBot2 plugin generates a picture which shows the status of current device"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "Pillow<10.0.0,>=9.2.0",
     "psutil<6.0.0,>=5.9.2",
     "nonebot2>=2.0.0",
-    "nonebot-plugin-send-anything-anywhere>=0.2.4",
+    "nonebot-plugin-send-anything-anywhere>=0.2.5",
     "anyio>=3.7.0",
     "httpx>=0.24.1",
     "pil-utils>=0.1.7",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
```

### Comparing `nonebot_plugin_picstatus-0.5.0/PKG-INFO` & `nonebot_plugin_picstatus-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-picstatus
-Version: 0.5.0
+Version: 0.5.1
 Summary: A NoneBot2 plugin generates a picture which shows the status of current device
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Requires-Python: <4.0,>=3.8
 Requires-Dist: Pillow<10.0.0,>=9.2.0
 Requires-Dist: psutil<6.0.0,>=5.9.2
 Requires-Dist: nonebot2>=2.0.0
-Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
+Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.5
 Requires-Dist: anyio>=3.7.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: pil-utils>=0.1.7
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
@@ -163,14 +163,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.5.1
+
+- 使用 SAA 向 Telegram 平台发送消息
+
 ### 0.5.0
 
 - 先获取状态信息再进行画图，可以获取到更精准的状态信息
 - 添加进程占用信息的展示
 - 测试网站结果状态码后面会带上 `reason`，如 `200 OK` / `404 Not Found`
 - 添加了一些配置项（`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`, `PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`, `PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`, `PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`）
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 0.5.0 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 0.5.1 Summary: A
 NoneBot2 plugin generates a picture which shows the status of current device
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus Author-Email:
 student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-picstatus Requires-Python: <4.0,>=3.8 Requires-Dist:
 Pillow<10.0.0,>=9.2.0 Requires-Dist: psutil<6.0.0,>=5.9.2 Requires-Dist:
-nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
+nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.5
 Requires-Dist: anyio>=3.7.0 Requires-Dist: httpx>=0.24.1 Requires-Dist: pil-
 utils>=0.1.7 Description-Content-Type: text/markdown
                                     [logo]
                                     [logo]
    # NoneBot-Plugin-PicStatus _â¨ è¿è¡ç¶æå¾çç for NoneBot2 â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» ä¸å¤è¯´ï¼ç´æ¥çå¾ï¼ ### ææå¾  ç¹å»å±å¼ !
@@ -35,15 +35,16 @@
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ææ¢¦ API](https://api.gumengya.com) -
 éæºèæ¯å¾æ¥æº ### [LoliApi](https://docs.loliapi.com/) -
 éæºèæ¯å¾æ¥æºï¼ææ¶å¼ç¨ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.5.0 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.5.1 - ä½¿ç¨ SAA å Telegram
+å¹³å°åéæ¶æ¯ ### 0.5.0 -
 åè·åç¶æä¿¡æ¯åè¿è¡ç»å¾ï¼å¯ä»¥è·åå°æ´ç²¾åçç¶æä¿¡æ¯
 - æ·»å è¿ç¨å ç¨ä¿¡æ¯çå±ç¤º -
 æµè¯ç½ç«ç»æç¶æç åé¢ä¼å¸¦ä¸ `reason`ï¼å¦ `200 OK` / `404 Not
 Found` - æ·»å äºä¸äºéç½®é¡¹ï¼`PS_SORT_PARTS`, `PS_SORT_PARTS_REVERSE`,
 `PS_SORT_DISK_IOS`, `PS_SORT_NETS`, `PS_SORT_SITES`, `PS_PROC_LEN`,
 `PS_IGNORE_PROCS`, `PS_PROC_SORT_BY`, `PS_PROC_CPU_MAX_100P`,
 `PS_REPLY_TARGET`, `PS_TG_MAX_FILE_SIZE`ï¼ ### 0.4.2 - æ·»å éç½®é¡¹
```

