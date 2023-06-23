# Comparing `tmp/nonebot_plugin_game_collection-2.2.5.tar.gz` & `tmp/nonebot_plugin_game_collection-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.2.5.tar", last modified: Thu Jun 15 19:17:22 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.2.6.tar", last modified: Fri Jun 23 21:43:51 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.2.5.tar` & `nonebot_plugin_game_collection-2.2.6.tar`

### file list

```diff
@@ -1,51 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.763799 nonebot_plugin_game_collection-2.2.5/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.5/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-15 19:17:22.762797 nonebot_plugin_game_collection-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.713992 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    21158 2023-06-15 18:18:05.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    55947 2023-06-13 16:02:57.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.727504 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    13575 2023-06-15 19:12:41.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20085 2023-06-15 19:15:09.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    16157 2023-06-06 15:49:58.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    33104 2023-06-15 18:17:34.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.734160 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.738163 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.756290 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5278 2023-06-12 13:50:26.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.757293 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.761297 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7825 2023-06-15 17:13:10.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 19:17:22.720497 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-15 19:17:22.000000 nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 19:17:22.763799 nonebot_plugin_game_collection-2.2.5/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-15 19:17:18.000000 nonebot_plugin_game_collection-2.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.036644 nonebot_plugin_game_collection-2.2.6/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.6/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-23 21:43:51.036142 nonebot_plugin_game_collection-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.975735 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    19558 2023-06-23 21:38:06.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.993822 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    19332 2023-06-23 14:22:48.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    18448 2023-06-23 21:09:29.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.999827 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.025635 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5166 2023-06-23 21:28:38.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.027135 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.034141 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    13638 2023-06-23 21:00:43.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.985815 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1947 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 21:43:51.036644 nonebot_plugin_game_collection-2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-06-23 21:43:45.000000 nonebot_plugin_game_collection-2.2.6/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.2.5/LICENSE` & `nonebot_plugin_game_collection-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/README.md` & `nonebot_plugin_game_collection-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Prop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,582 +1,510 @@
-from typing import Tuple
 from nonebot.adapters.onebot.v11 import (
-    Bot,
     MessageEvent,
     GroupMessageEvent,
-    Message,
     MessageSegment
     )
-
 import random
-import time
-import datetime
 
-from .utils.utils import line_wrap
-from .utils.chart import bbcode_to_png, bbcode_to_PIL, bar_chart,my_info_head, my_info_statistics, info_Splicing
-from .data.data import UserDict, GroupAccount
-from .data.data import props_library, props_index
-from .config import bot_name,sign_gold, revolt_gold, revolt_cd, revolt_gini, max_bet_gold
-from .Manager import BG_path, bot_list
-from .Manager import data, company_index, update_company_index
+from .utils.utils import get_message_at
+from .utils.chart import linecard,gacha_info
+from .data import props_library, props_index, element_library
+from .config import bot_name, sign_gold, revolt_gold, max_bet_gold, gacha_gold
+
+from .Manager import data,BG_path
 from . import Manager
 
 user_data = data.user
 group_data = data.group
 
-def gold_create(event:MessageEvent,gold:int) -> str:
-    """
-    获取金币
-    """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
 
-    user.gold += gold
-    group_account.gold += gold
-    return f"你获得了 {gold} 金币"
 
-def props_create(event:MessageEvent, prop_name:str, count:int) -> str:
+def random_props() -> str:
     """
-    获取道具
-    """
-    prop_code = props_index.get(prop_name)
-    if not prop_code:
-        return f"没有【{prop_name}】这种道具。"
-
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
-
-    if prop_code[1] == "3":
-        account = user
+    随机获取道具。
+        rare:稀有度
+        return:道具代码
+        道具代码规则：
+        第1位：稀有度
+        第2位：道具性质：
+            1：空气
+            2：群内道具
+            3：全局道具
+        第3位：道具时效：
+            0：时效道具
+            1：永久道具
+        4,5位：本稀有度下的道具编号
+    """
+    code = random.randint(1,100)
+    if 0 < code <= 30:
+        props = random.choice(["31001","32001","32002","33001","33101"])
+    elif 30 < code <= 40:
+        props = random.choice(["41001","42001","42101"])
+    elif 40 < code <= 50:
+        props = random.choice(["51001","51002","52001","52002","52101","52102"])
+    elif code == 51:
+        props = random.choice(["61001","62101"])
+    elif code == 52:
+        props = random.choice(["63101","63102"])
     else:
-        account = group_account
+        props = "11001"
+    return props
 
-    account.props.setdefault(prop_code,0)
-    account.props[prop_code] += count
-    return f"你获得了{count}个【{prop_name}】！"
-
-def sign(event:MessageEvent) -> str:
+def gacha(event:MessageEvent, N:int):
     """
-    签到
+    抽卡
     """
     user,group_account = Manager.locate_user(event)
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
 
-    if group_account.is_sign:
-        return "你已经签过到了哦"
+    if (gold := group_account.gold) < (cost := N * gacha_gold):
+        return f'{N}连抽卡需要{cost}金币，你的金币：{gold}。'
+    user.gold -= cost
+    group_account.gold -= cost
+    res = {}
+    star = 0
+    airstar = 0
+    air = 0
+    for i in range(N):
+        prop_code = random_props()
+        res.setdefault(prop_code,0)
+        res[prop_code] += 1
+        rare = int(prop_code[0])
+        star += rare
+        if prop_code[1] == '1':
+            airstar += rare
+            air += 1
     else:
-        gold = random.randint(sign_gold[0], sign_gold[1])
-        user.gold += gold
-        group_account.gold += gold
-        group_account.is_sign = True
-    return random.choice(["祝你好运~", "可别花光了哦~"]) + f"\n你获得了 {gold} 金币"
-
-def revolt_sign(event:MessageEvent) -> str:
-    """
-    重置签到
-    """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        data = sorted(res.items(),key = lambda x:int(x[0]),reverse=True)
 
-    if group_account.revolution:
-        return "你没有待领取的金币"
+    info = []
+    airdata = []
+    for prop_code, n in data:
+        if prop_code[1] == "2":
+            props = group_account.props
+            props.setdefault(prop_code,0)
+            props[prop_code] += n
+            quant =  "天" if prop_code[2] == "0" else "个"
+        elif prop_code[1] == "3":
+            props = user.props
+            props.setdefault(prop_code,0)
+            props[prop_code] += n
+            quant =  "天" if prop_code[2] == "0" else "个"
+        else:
+            airdata.append((prop_code, n))
+            continue
+        prop_info = props_library.get(prop_code,{"name":prop_code, "color":"black","rare":1,"intro":"未知","des":"未知"})
+        color = prop_info['color']
+        name = prop_info['name']
+        rare = prop_info['rare']
+        info.append(
+            linecard(f"[color][{color}]【{name}】[nowrap]\n[right][color][{color}]{n}{quant}\n",
+                     width = 440,
+                     height = 120,
+                     padding=(0,10),
+                     endline = rare*'☆',
+                     bg_color = "white"
+                     ))
+    user.props = {k:10 if k[2] == '0' and v > 30 else v for k, v in user.props.items()}
+    group_account.props = {k:v if v < 30 else 30 for k,v in group_account.props.items()}
+    if len(info)%2 == 1:
+        info.append(None)
+
+    for prop_code, n in airdata:
+        prop_info = props_library.get(prop_code,{"name":prop_code, "color":"black","rare":1,"intro":"未知","des":"未知"})
+        color = prop_info['color']
+        name = prop_info['name']
+        rare = prop_info['rare']
+        info.append(
+            linecard(f"[color][{color}]【{name}】[nowrap]\n[right][color][{color}]{n}次\n",
+                        width = 440,
+                        height = 120,
+                        padding=(0,10),
+                        endline = rare*'☆',
+                        bg_color = "white"
+                        ))
+    pt = star/N
+    if pt < 1.6:
+        level = "[color][#003300]理 想 气 体"
+    if pt < 1.88:
+        level = "[color][#003333]☆ 数据异常 ☆"
+    elif pt < 2.16:
+        level = "[color][#003366]☆☆ 一枚硬币 ☆☆"
+    elif pt < 2.44:
+        level = "[color][#003399]☆☆☆ 高斯分布 ☆☆☆"
+    elif pt < 2.72:
+        level = "[color][#0033CC]☆☆☆☆ 对称破缺 ☆☆☆☆"
+    elif pt < 3:
+        level = "[color][#0033FF]☆☆☆☆☆ 概率之子 ☆☆☆☆☆"
+    else:
+        level = "[color][#FF0000]☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆☆"
+
+    if N >= 10:
+        msg = (
+            f"{group_account.nickname}\n"
+            "----\n"
+            f"抽卡次数：{N}[nowrap]\n"f"[pixel][450]空气占比：{round(air*100/N,2)}%\n"
+            f"获得☆：{star}[nowrap]\n"f"[pixel][450]获得☆：{airstar}\n"
+            f"平均每抽☆数：{round(pt,3)}[nowrap]\n"f"[pixel][450]空气质量：{round(airstar/air,3)}\n"
+            f"结果评定：[nowrap]\n{level}\n"
+            )
     else:
-        gold = random.randint(revolt_gold[0], revolt_gold[1])
-        user.gold += gold
-        group_account.gold += gold
-        group_account.revolution = True
-    return f"这是你重置后获得的金币，你获得了 {gold} 金币"
+        msg = (
+            f"{group_account.nickname}\n"
+            "----\n"
+            f"抽卡次数：{N}\n"
+            )
+        
+        
+    return MessageSegment.image(gacha_info(linecard(msg,width = 880,endline = f"抽卡报告",bg_color = "white"),info))
 
-def revolution(group_id:int) -> str:
-    """
-    发动革命
-        group_id:群号
-    """
+class Prop(str):
+    def use(self, event:MessageEvent, count:int):
+        """
+        使用道具
+        """
+        if self == "03101":
+            return self.use_03101(event,count)
+        elif self == "03100":
+            return self.use_03100(event)
+        elif self == "33101":
+            return self.use_33101(event,count)
+        elif self == "42101":
+            return self.use_42101(event)
+        elif self == "52101":
+            return self.use_52101(event)
+        elif self == "52102":
+            return self.use_52102(event,count)
+        elif self == "53101":
+            return self.use_53101(event,count)
+        elif self == "63101":
+            return self.use_63101(event)
+        elif self == "63102":
+            return self.use_63102(event)
+        else:
+            return f"【{props_library[self]['name']}】不是可用道具。"
 
-    if group_id not in group_data:
-        return None
+    @classmethod
+    def use_03100(cls, event:MessageEvent) -> str:
+        """
+        使用道具：测试金库
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("03100",0) < 1:
+            return "数量不足"
+
+        props["03100"] -= 1
+        if props["03100"] < 1:
+            del props["03100"]
 
-    group = group_data[group_id]
+        return "你获得了10亿金币，100万钻石。祝你好运！"
 
-    if time.time() - group.revolution_time < revolt_cd:
-        return f"重置正在冷却中，结束时间：{datetime.datetime.fromtimestamp(group.revolution_time + revolt_cd).strftime('%H:%M:%S')}"
+    @classmethod
+    def use_03101(cls, event:MessageEvent, count:int) -> str:
+        """
+        使用道具：被冻结的资产
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("03101",0) < count:
+            return "数量不足"
+
+        props["03101"] -= count
+        if props["03101"] < 1:
+            del props["03101"]
 
-    if (gold := (Manager.group_wealths(group_id) or 0)) < (limit := 15 * max_bet_gold):
-        return f"本群金币（{round(gold,2)}）小于{limit}，未满足重置条件。"
-
-    if (gini := Manager.Gini(group_id)) < revolt_gini:
-        return f"当前基尼系数为{round(gini,3)}，未满足重置条件。"
-
-    rank = Manager.group_ranklist(group_id,"资产")
-    user_id = rank[0][0]
-    group_account = user_data[user_id].group_accounts[group_id]
-    group_account.props.setdefault("02101",0)
-    group_account.props["02101"] += 1
-
-    group.revolution_time = time.time()
-    group.Achieve_revolution.setdefault(user_id,0)
-    group.Achieve_revolution[user_id] += 1
-
-    first_name = group_account.nickname
-
-    i = 0.0
-    j = i**2
-    for x in rank[:10]:
-        user = user_data[x[0]]
-        group_account = user.group_accounts[group_id]
-        gold = int(group_account.value*j - group_account.gold*(1-j))
+        gold = count * max_bet_gold
         user.gold += gold
         group_account.gold += gold
-        company_ids = [company_id for company_id in group_account.stocks]
-        for company_id in company_ids:
-            company = group_data[company_id].company
-            if user_id in company.exchange:
-                del company.exchange[user_id]
-            company.stock += group_account.stocks[company_id]
-            del group_account.stocks[company_id]
-        i += 0.1
-        j = i**2
-    for user_id in group.namelist:
-        user_data[user_id].group_accounts[group_id].revolution = False
-    data.save()
-    return f"重置成功！恭喜{first_name}进入挂件榜☆！\n当前系数为：{round(gini,3)}，重置签到已刷新。"
-
-def transfer_gold(event:GroupMessageEvent, target:Tuple[UserDict,GroupAccount], gold:int) -> str:
-    """
-    转账处理
-        param:
-        event: GroupMessageEvent
-        target:目标账户
-        gold:  转账金币
-    """
-    self_user,self_group_account = Manager.locate_user(event)
-    target_user,target_group_account = target
+        return f"你获得了{gold}金币。"
 
-    if self_group_account.gold < gold:
-        return f"你没有足够的金币，无法完成结算。\n——你还有{self_group_account.gold}枚金币。"
+    @classmethod
+    def use_33101(cls, event:MessageEvent, count:int) -> str:
+        """
+        使用道具：初级元素
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("33101",0) < count:
+            return "数量不足"
+
+        props["33101"] -= count
+        if props["33101"] < 1:
+            del props["33101"]
+
+        res = {}
+        for i in range(count*4):
+            element_code = f"0{random.randint(1,4)}01"
+            res.setdefault(element_code,0)
+            res[element_code] += 1
+        msg = "你获得了\n"
+        for element_code in res:
+            n = res[element_code]
+            user.alchemy.setdefault(element_code,0)
+            user.alchemy[element_code] += n
+            msg += f'{element_library[element_code]["name"]}：{n}个\n' 
+        return msg + "祝你好运~"
 
-    if target_group_account.props.get("42001",0):
-        fee = 0
-        tips = f"『{props_library['42001']['name']}』免手续费"
-    else:
-        fee = int(gold * 0.02)
-        tips = f"扣除2%手续费：{fee}，实际到账金额{gold - fee}"
+    @classmethod
+    def use_42101(cls, event:MessageEvent) -> str:
+        """
+        使用道具：调查凭证
+        """
+        if isinstance(event, GroupMessageEvent):
+            group_id = event.group_id
+        else:
+            return f"此道具只能在群内使用"
 
-    self_user.gold -= gold
-    self_group_account.gold -= gold
-    target_user.gold += gold - fee
-    target_group_account.gold += gold - fee
+        if not (at := get_message_at(event.message)):
+            return "没有指定用户。"
+        else:
+            at = int(at[0])
 
-    return f"向 {target_group_account.nickname} 赠送{gold}金币\n" + tips
+        if at not in group_data[group_id].namelist:
+            return "对方没有账户。"
 
-def transfer_props(event:GroupMessageEvent, target:Tuple[UserDict,GroupAccount], prop_name:str, count:int) -> str:
-    """
-    赠送道具
-        param:
-        event: GroupMessageEvent
-        target:目标账户
-        props: 道具名
-        count: 数量
-    """
-    prop_code = props_index.get(prop_name)
-    if not prop_code:
-        return f"没有【{prop_name}】这种道具。"
-
-    self_user,self_group_account = Manager.locate_user(event)
-    target_user,target_group_account = target
+        user,group_account = Manager.locate_user(event)
+        props = group_account.props
+        if props.get("42101",0) < 1:
+            return "数量不足"
+
+        props["42101"] -= 1
+        if props["42101"] < 1:
+            del props["42101"]
+
+        target_user = user_data[at]
+        target_group_account = target_user.group_accounts[group_id]
+        N = random.randint(0,50)
+        if N < 30:
+            gold = int(group_account.gold * N / 1000)
+            gold = 0 if gold < 0 else gold
+            user.gold -= gold
+            group_account.gold -= gold
+            target_user.gold += gold
+            target_group_account.gold += gold
+            info = f"调查没有发现问题。你赔偿了对方{gold}枚金币"
+        else:
+            gold = int(target_group_account.gold * N / 1000)
+            gold = min(group_account.gold, gold)
+            gold = 0 if gold < 0 else gold
+            user.gold += gold
+            group_account.gold += gold
+            target_user.gold -= gold
+            target_group_account.gold -= gold
+            info = f"你获得了{gold}枚金币"
+            #stocks = group_account.stocks
+            #target_stocks = target_group_account.stocks
+            #for company_id, count in target_stocks.items():
+            #    if stock := int(count * N / 100):
+            #        stocks.setdefault(company_id,0)
+            #        stocks[company_id] += stock
+            #        target_stocks[company_id] -= stock
+            #        if at in (company := group_data[company_id].company):
+            #            del company.exchange[at]
+            #        info += f"{company.company_name}：{stock}\n"
+            info += f"（{N/10}%）" 
+        return info
 
-    if prop_code[1] == "3":
-        self_account = self_user
-        target_account = target_user
-    else:
-        self_account = self_group_account
-        target_account = target_group_account
+    @classmethod
+    def use_52101(cls, event:MessageEvent,) -> str:
+        """
+        使用道具：神秘天平
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = group_account.props
+        if props.get("52101",0) < 1:
+            return "数量不足"
+
+        props["52101"] -= 1
+        if props["52101"] < 1:
+            del props["52101"]
+
+        group_id = group_account.group_id
+        ranklist = Manager.group_ranklist(group_id,"金币")
+        target_id = random.choice([x[0] for x in ranklist if x[1] > revolt_gold[0]])
+        if target_id == event.user_id:
+            return f"道具使用失败，你损失了一个『{props_library['52101']['name']}』"
+        target_user = user_data[target_id]
+        target_group_account = target_user.group_accounts[group_id]
+
+        change = int((group_account.gold - target_group_account.gold) / 2)
+        limit = min((group_account.gold, target_group_account.gold))
+        limit = 0 if limit < 0 else limit
+        if change > limit:
+            change = limit
+        if change < -limit:
+            change = -limit
+
+        abschange = abs(change)
+        fee = int(abschange / 20)
+
+        flag = group_account.props.get("42001",0)
+        tag = "失去" if change > 0 else "获得"
+        if flag > 0:
+            user.gold -= change
+            group_account.gold -= change
+            msg1 = f"\n你{tag}了{abschange}金币『{props_library['42001']['name']}』。"
+        else:
+            user.gold -= change
+            user.gold -= fee
+            group_account.gold -= change
+            group_account.gold -= fee
+            msg1 = f"\n你{tag}了{abs(change + fee)}金币(扣除5%手续费：{fee})。"
+
+        flag = target_group_account.props.get("42001",0)
+        tag = "失去" if change < 0 else "获得"
+
+        if flag > 0:
+            target_user.gold += change
+            target_group_account.gold += change
+            msg2 = f"\n对方{tag}了{abschange}金币『{props_library['42001']['name']}』。"
+        else:
+            target_user.gold += change
+            target_user.gold -= fee
+            target_group_account.gold += change
+            target_group_account.gold -= fee
+            msg2 = f"\n对方{tag}了{abs(change - fee)}金币(扣除5%手续费：{fee})。"
 
-    n = self_account.props.get(prop_code,0)
-    if n < count:
-        return f"你没有足够的道具，无法完成结算。\n——你有{n}个【{prop_name}】。"
-
-    self_account.props[prop_code] -= count
-    target_account.props.setdefault(prop_code,0)
-    target_account.props[prop_code] += count
-    return f"向 {target_group_account.nickname} 送出{count}个【{prop_name}】！"
+        return f"你与{target_group_account.nickname}平分了金币。" + msg1 + msg2
 
-def connect(event:MessageEvent, group_id:str = None) -> str:
-    """
-    关联账户
-        param:
-        event: GroupMessageEvent
-        group_id:关联群号
-    """
-    user = Manager.locate_user(event)[0]
-    if group_id:
-        try:
-            group_id = int(group_id)
-        except:
-            return f"无效输入：{group_id}"
-        if group_id in user.group_accounts:
-            user.connect = group_id
+    @classmethod
+    def use_52102(cls, event:MessageEvent, count:int,) -> str:
+        """
+        使用道具：幸运硬币
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = group_account.props
+        if props.get("52102",0) < 1:
+            return "数量不足"
+
+        if count == 1:
+            gold = int(group_account.gold/2)
+            X = 1
         else:
-            return f"你在 {group_id} 无账户，关联失败。"
-    else:
-        user.connect = event.group_id
-    return f"私聊账户已关联到{group_id}"
-
-def my_gold(event:MessageEvent) -> str:
-    """
-    我的金币
-    """
-    user,group_account = Manager.locate_user(event)
-    if group_account:
-        return f"你还有 {group_account.gold} 枚金币"
-    else:
-        group_accounts = user.group_accounts
-        msg = "你的账户\n"
-        for group_id in group_accounts:
-            msg += f'{group_id} 金币：{group_accounts[group_id].gold}枚\n'
-        return msg
+            if props.get("62101",0) > 0:
+                props["62101"] -= 1
+                if props["62101"] < 1:
+                    del props["62101"]
+            else:
+                return "钻石数量不足"
+            if count == 2:
+                gold = int(group_account.gold/2)
+                X = 2
+            else:
+                gold = group_account.gold
+                X = 1
 
-async def my_info(event:MessageEvent) -> Message:
-    """
-    我的资料卡
-    """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        gold = gold if gold < (limit := 50 * max_bet_gold) else limit
 
-    info = []
-    # 加载全局信息
-    nickname = group_account.nickname
-    info.append(await my_info_head(user,nickname))
-    linestr = "[color=gray][size=15][font=simsun.ttc]────────────────────────────────────────────────────────[/font][/size][/color]\n"
-    Achieve = Manager.Achieve_list((user,group_account))
-    achieve = ""
-    msg = ""
-    # 加载道具卡片
-    for x in Achieve:
-        if x.startswith("◆◇"):
-            achieve = achieve + x + "\n"
+        props["52102"] -= 1
+        if props["52102"] < 1:
+            del props["52102"]
+
+        if random.randint(0,X) > 0:
+            user.gold += gold
+            group_account.gold += gold
+            return f"你获得了{gold}金币"
         else:
-            msg += f"[align=center][font=simsun.ttc]{x}[/font][/align]\n"
-            msg += linestr
-    if msg:
-        info.append(bbcode_to_PIL(linestr + msg[:-1], 60))
-    # 加载本群账户
-    gold = group_account.gold
-    value = group_account.value
-    is_sign = group_account.is_sign
-    if is_sign:
-        is_sign = ["已签到","green"]
-    else:
-        is_sign = ["未签到","red"]
-    security = 3 - group_account.security
-    if security:
-        security = [security,"green"]
-    else:
-        security = [security,"red"]
-        
-    msg = (
-        "[font=simsun.ttc]"+achieve+"[/font]"
-        + linestr +
-        f"金币 {'{:,}'.format(gold)}\n"
-        f"股票 {'{:,}'.format(round(value,2))}\n"
-        + linestr +
-        f'今日签到 [color={is_sign[1]}]{is_sign[0]}[/color]\n'
-        f'今日补贴 还剩 [color={security[1]}]{security[0]}[/color] 次\n'
-        + linestr +
-        "[align=right][size=30][color=gray]账户信息[/color][/size][/align]\n"
-        )
-    info.append(bbcode_to_PIL(msg,60,spacing = 20))
-    # 加载资产分析
-    dist = []
-    for x in user.group_accounts:
-        account = user.group_accounts[x]
-        if not (group_name := group_data[x].company.company_name):
-            group_name = f"（{str(x)[-4:]}）"
-        dist.append([account.gold + account.value, group_name])
-    dist = [x for x in dist if x[0] > 0]
-    if dist:
-        info.append(my_info_statistics(dist))
-    # 加载股票信息
-    msg = ""
-    for stock in group_account.stocks:
-        company_name = group_data[stock].company.company_name
-        if i := group_account.stocks[stock]:
-            msg += f"[size=40][align=left]{company_name}[/align][align=right][color=green]{i}[/color][/align][/size]"
-    if msg:
-        msg = msg + linestr + "[align=right][size=30][color=gray]股票信息[/color][/size][/align]\n"
-        info.append(bbcode_to_PIL(msg))
+            gold = int(group_account.gold/2)
+            user.gold -= gold
+            group_account.gold -= gold
+            user.props.setdefault("53101",0)
+            user.props["53101"] += 1
+            return f"你失去了{gold}金币。\n{bot_name}送你1个『{props_library['53101']['name']}』，祝你好运~"
 
-    return MessageSegment.image(info_Splicing(info,BG_path(event.user_id)))
+    @classmethod
+    def use_53101(cls, event:MessageEvent, count:int) -> str:
+        """
+        使用道具：随机红包
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("53101",0) < count:
+            return "数量不足"
+
+        props["53101"] -= count
+        if props["53101"] < 1:
+            del props["53101"]
 
-def my_props(event:MessageEvent) -> Message:
-    """
-    我的道具
-    """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        gold = random.randint(sign_gold[0] * count, revolt_gold[1] * count)
 
-    props = {}
-    props.update(user.props)
-    props.update(group_account.props)
-    props = sorted(props.items(), key = lambda x:int(x[0]))
-    linestr = "[color=gray][size=15][font=simsun.ttc]────────────────────────────────────────────────────────[/font][/size][/color]\n"
-    msg = ""
-    for seg in props:
-        if (n := seg[1]) < 1:
-            continue
-        prop_code = seg[0]
-        quant = "天" if prop_code[2] == "0" else "个"
-        prop = props_library.get(prop_code,{"name": prop_code, "color": "black","rare": 1,"intro": "未知","des": "未知"})
-        msg += (
-            f"[color={prop['color']}]【{prop['name']}】{prop['rare']*'☆'}[align=right]{n}{quant}[/align]\n" +
-            linestr +
-            "[size=40][color=gray]"
-            f"{line_wrap(prop['intro'], 38)}\n"
-            f"[align=right]{line_wrap(prop['des'], 38)}[/align]"
-            "[/color][/size]" +
-            linestr
-            )
-    if msg:
-        return MessageSegment.image(bbcode_to_png(msg,60))
-    else:
-        return "您的仓库空空如也。"
+        user.gold += gold
+        group_account.gold += gold
+        return f"你获得了{gold}金币。祝你好运~"
 
-async def info_profile(user_id:int) -> list:
-    """
-    总览资料卡
-    """
-    user = user_data[user_id]
-    info = []
-    # 加载全局信息
-    nickname = user.nickname
-    info.append(await my_info_head(user,nickname))
-    # 加载资产分析
-    dist = []
-    for x in user.group_accounts:
-        account = user.group_accounts[x]
-        if not (group_name := group_data[x].company.company_name):
-            group_name = f"（{str(x)[-4:]}）"
-        dist.append([account.gold + account.value, group_name])
-    dist = [x for x in dist if x[0] > 0]
-    if dist:
-        info.append(my_info_statistics(dist))
-    return info
+    @classmethod
+    def use_63101(cls, event:MessageEvent) -> str:
+        """
+        使用道具：超级幸运硬币
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("63101",0) < 1:
+            return "数量不足"
+
+        props["63101"] -= 1
+        if props["63101"] < 1:
+            del props["63101"]
+
+        gold = group_account.gold
+
+        if random.randint(0,1) == 0:
+            user.gold += gold
+            group_account.gold += gold
+            return f"你获得了{gold}金币"
+        else:
+            user.gold -= gold
+            group_account.gold -= gold
+            user.props.setdefault("53101",0)
+            user.props["53101"] += 1
+            return f"你失去了{gold}金币。\n{bot_name}送你1个『{props_library['53101']['name']}』，祝你好运~"
 
-def format_ranktitle(title:str = "金币"):
-    """
-    根据排行榜将数据格式化
-    """
-    if title == "金币":
-        func = lambda x:'{:,}'.format(x)
-    elif title == "总资产" or title == "资产" or title == "财富":
-        func = lambda x:'{:,}'.format(round(x,2))
-    elif title == "胜率":
-        func = lambda x:f"{round(x*100,2)}%"
-    else:
-        func = lambda x:x
-    return func
+    @classmethod
+    def use_63102(cls, event:MessageEvent) -> str:
+        """
+        使用道具：重开券
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("63102",0) < 1:
+            return "数量不足"
+
+        props["63102"] -= 1
+        if props["63102"] < 1:
+            del props["63102"]
 
-async def info_group_rank(group_id:int, title:str = "金币", top:int = 20) -> list:
-    """
-    群内排名信息
-    """
-    if not (ranklist := Manager.group_ranklist(group_id, title)):
-        return None
-    info = []
-    i = 1
-    first = ranklist[0][1]
-    for x in ranklist[:top]:
-        user = user_data[x[0]]
+        group_id = group_account.group_id
         user_id = user.user_id
-        group_account = user.group_accounts[group_id]
-        nicname = group_account.nickname
-        info.append(await bar_chart(user_id,f"{i}.{nicname}：{format_ranktitle(title)(x[1])}\n", x[1]/first))
-        i += 1
-    return info
-
-async def group_rank(event:MessageEvent, title:str = "金币") -> str:
-    """
-    生成群内排行榜
-    """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
-    user_id = user.user_id
-    group_id = group_account.group_id
-    if not (ranklist := Manager.group_ranklist(group_id, title)):
-        return "无数据。"
-    info = await info_group_rank(group_id, title, 20)
-    if info:
-        return MessageSegment.image(info_Splicing(info,BG_path(user_id)))
-    else:
-        return "无数据。"
-
-async def All_rank(event:MessageEvent, title:str = "金币", top:int = 10) -> list:
-    """
-    生成总排行榜
-    """
-    if not (ranklist := Manager.All_ranklist(title)):
-        return None
-    linestr = "[color=gray][size=15][font=simsun.ttc]────────────────────────────────────────────────────────[/font][/size][/color]\n"
-    msg = []
-    i = 1
-    l = len(user_data)
-    for x in ranklist[:top]:
-        user_id = x[0]
-        info = await info_profile(user_id)
-        tmp = (
-            "[align=center]"
-            f"{title}：{format_ranktitle(title)(x[1])}\n"
-            f'[size=300]{i}[/size]\n'
-            "[/align]"
-            + linestr +
-            f"[align=right][size=30][color=gray]{title}总排行 {i}/{l}[/color][/size][/align]\n"
-            )
-        info.append(bbcode_to_PIL(tmp,60))
-        msg.append({"type":"node",
-                    "data":{
-                        "name":f"{bot_name}",
-                        "uin":str(event.self_id),
-                        "content":MessageSegment.image(info_Splicing(info,BG_path(user_id)))}})
-        i += 1
-    return msg
-
-def transfer_fee(amount:int,limit:int) -> int:
-    limit = limit if limit > 0 else 0
-    if amount <= limit:
-        fee = amount * 0.02
-    else:
-        fee = limit * 0.02 + (amount - limit) * 0.2
-    return int(fee)
-
-def intergroup_transfer_gold(event:MessageEvent, gold:int, company_name:str):
-    """
-    跨群转移金币到自己的账户
-    """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
-    if gold > group_account.gold:
-        return f"你没有足够的金币，无法完成结算。\n——你还有{group_account.gold}枚金币。"
-
-    if company_name in company_index:
-        company_id = company_index[company_name]
-    else:
-        return f"没有 {company_name} 的注册信息"
-
-    if company_id in user.group_accounts:
-        target_group_account = user.group_accounts[company_id]
-    else:
-        return f"你在 {company_name} 没有创建账户"
-
-    user.transfer_limit += gold
-    fee = transfer_fee(gold, (10 * max_bet_gold) - user.transfer_limit)
-    user.gold -= fee
-    group_account.gold -= gold
-    target_group_account.gold += gold - fee
-
-    return f"向 {company_name} 转移 {gold}金币，扣除手续费：{fee}，实际到账金额{gold - fee}"
-
-def freeze(target:UserDict):
-    target_id = target.user_id
-    gold = target.gold
-    value = 0.0
-    company_ids = set()
-    group_accounts = target.group_accounts
-    for group_id in group_accounts:
-        group_account = group_accounts[group_id]
-        value += group_account.value
-        stocks = group_account.stocks
-        group = group_data[group_id]
-        for company_id in stocks:
-            group.company.stock += stocks[company_id]
-            company_ids.add(company_id)
-        group.namelist.remove(target_id)
-
-    for company_id in company_ids:
-        exchange = group_data[company_id].company.exchange
-        if target_id in exchange:
-            del exchange[target_id]
-
-    target.gold = 0
-    target.group_accounts = {}
-
-    x = gold + value
-    if x > 500 * max_bet_gold:
-        count = 500
-    elif x > 50 * max_bet_gold:
-        count = int (x / max_bet_gold)
+        for company_id in group_account.stocks:
+            company = group_data[company_id].company
+            company.stock += group_account.stocks[company_id]
+            exchange = company.exchange
+            if user_id in exchange:
+                del exchange[user_id]
+        user.gold -= group_account.gold
+        group_data[group_id].namelist.remove(user_id)
+        del group_account
+        return "你在本群的账户已重置，祝你好运~"
+
+def use_prop(event:MessageEvent, prop_name:str, count:int):
+    if prop_code := props_index.get(prop_name):
+        return Prop(prop_code).use(event,count)
     else:
-        count = int (x / max_bet_gold) + 1
-
-    target.props.setdefault("03101",0)
-    target.props["03101"] += count
-
-    data.save()
-
-    return f"【冻结】清算完成，总价值为 {round(x,2)}（金币 {gold} 股票 {round(value,2)}）"
-
-async def delist():
-        """
-        清理无效账户
-        """
-        mapping = {}
-        for bot in bot_list:
-            group_list = await bot.get_group_list(no_cache = True)
-            for group in group_list:
-                mapping[group["group_id"]] = bot
-        if not mapping:
-            return "群组获取失败"
-
-        # 存在的群
-        groups = set(mapping.keys())
-        # 注册过的群
-        login_groups= set(group_data.keys())
-        # 已注册但不存在的群
-        delist_group = login_groups - groups
-
-        log = ""
-        # 处理与不存在的群相关的群账户
-        for user_id in user_data:
-            user = user_data[user_id]
-            group_accounts = user.group_accounts
-            accountset = set(group_accounts.keys())
-            delist_group_accounts = accountset & delist_group
-            for group_id in accountset:
-                group_account = group_accounts[group_id]
-                if group_id in delist_group_accounts:
-                    # 删除不存在的群账户
-                    log += f'删除群账户：{user_id} - {group_id}\n'
-                    del group_account
-                else:
-                    # 删除不存在的股票
-                    group_account.stocks = {stock:count for stock, count in group_account.stocks.items() if stock not in delist_group_accounts}
-        # 删除不存在的群
-        for group_id in delist_group:
-            log += f'删除群：{group_id}\n'
-            del group_data[group_id]
-
-        # 已注册且存在的群
-        normal_groups = login_groups & groups
-        for group_id in normal_groups:
-            users = await mapping[group_id].get_group_member_list(group_id = group_id, no_cache = True)
-            if users:
-                users = set(x["user_id"] for x in users)
-            else:
-                continue
-            # 删除已注册但不存在的用户
-            namelist = group_data[group_id].namelist
-            delist_users = namelist - users
-            for user_id in delist_users:
-                log += f'删除群账户：{user_id} - {group_id}\n'
-                del user_data[user_id].group_accounts[group_id]
-                namelist.discard(user_id)
-        update_company_index()
-        # 保存数据
-        data.save()
-        return log[:-1] if log else "没有要清理的数据！"
+        return f"没有【{prop_name}】这种道具。"
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Game.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,306 +1,85 @@
 ﻿from typing import Tuple,Dict
 from pydantic import BaseModel
+from abc import ABC, abstractmethod
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     GroupMessageEvent,
     Message,
     MessageSegment
     )
 import random
 import time
 import asyncio
 
 from .utils.utils import get_message_at
 from .utils.chart import text_to_png
-from .data.data import props_library
-from .config import bot_name, security_gold, max_bet_gold, max_player, min_player
+from .data import props_library
+from .config import bot_name, security_gold, bet_gold, max_bet_gold, max_player, min_player
 
 from .HorseRace.start import load_dlcs
 from .HorseRace.race_group import race_group
 
 from .Manager import data, try_send_private_msg
 from . import Manager
 
 user_data = data.user
 group_data = data.group
 
-
-
-"""+++++++++++++++++
-——————————
-     赛马小游戏
-——————————
-+++++++++++++++++"""
-
-def race_create_check(event:GroupMessageEvent):
-    """
-    检查是否可以创建赛马
-    """
-    global current_games
-    group_id = event.group_id
-    if group_id not in current_games:
-        return None
-    session = current_games[group_id]
-    overtime = time.time() - session.time + 180
-    if session.at == -1:
-        race:race_group = session.info["race_group"]
-        if race.start == 0:
-            if overtime < 120:
-                return "一场赛马正在报名中"
-            else:
-                return None
-        else:
-            return f"一场赛马正在进行中，遇到问题可以{f'在{t}秒后' if (t := int(180 - overtime)) > 0 else ''}输入【赛马重置】重置游戏"
-    else:
-        return session.create_check(event)
-
-def RaceNew(event:GroupMessageEvent, gold:int ):
-    """
-    赛马创建
-    """
-    global current_games
-    if msg := race_create_check(event):
-        return msg
-    current_games[event.group_id] =  Session(
-        time = time.time() + 180,
-        player1_id = event.user_id,
-        at = -1,
-        gold = gold,
-        info = {"game":"horse race","race_group":race_group()}
-        )
-    return ("\n"
-             "> 创建赛马比赛成功！\n"
-             "> 输入 【赛马加入 名字】 即可加入赛马。")
-
-def RaceJoin(event:GroupMessageEvent, horsename:str):
-    """
-    赛马加入
-    """
-    global current_games
-    group_id = event.group_id
-    if group_id not in current_games:
-        return "赛马活动未开始，请输入【赛马创建】创建赛马场"
-    session = current_games[event.group_id]
-    if session.info["game"] != "horse race":
-        return "其他对战进行中。"
-    user,group_account = Manager.locate_user(event)
-    user_id = user.user_id
-    if (gold := group_account.gold) < session.gold:
-        return f"报名赛马需要{session.gold}金币，你的金币：{gold}。"
-    race:race_group = session.info["race_group"]
-    if race.start != 0:
-        return
-    if (query_of_player := race.query_of_player()) >= max_player:
-        return "加入失败！赛马场就那么大，满了满了！"
-    if race.is_player_in(user_id) == True:
-        return "加入失败！您已经加入了赛马场!"
-    if not horsename:
-        return "请输入你的马儿名字"
-    horsename = horsename[:2]+"酱" if len(horsename) > 5 else horsename
-    race.add_player(horsename, user_id, group_account.nickname)
-    user.gold -= session.gold
-    group_account.gold -= session.gold
-    return  ("\n"
-             "> 加入赛马成功\n"
-             "> 赌上马儿性命的一战即将开始!\n"
-             f"> 赛马场位置:{query_of_player + 1}/{max_player}")
-
-events_list = load_dlcs()
-
-async def RaceStart(bot:Bot, event:GroupMessageEvent):
-    """
-    赛马开始
-    """
-    global current_games
-    group_id = event.group_id
-    if group_id not in current_games or (session := current_games[event.group_id]).info["game"] != "horse race":
-        return "赛马活动未开始，请输入【赛马创建】创建赛马场"
-    race:race_group = session.info["race_group"]
-    global events_list
-    if (player_count := race.query_of_player()) == 0:
-        return
-    if race.start == 1:
-        return
-    if race.start == 0 or race.start == 2:
-        if player_count >= min_player:
-            race.start = 1
-        else:
-            return f"开始失败！赛马开局需要最少{min_player}人参与"
-    session.time = time.time() + 180
-    await bot.send(event,(f'> 比赛开始\n'
-                          f'> 当前奖金：{session.gold * player_count}金币'))
-    await asyncio.sleep(0.5)
-
-    while race.start == 1:
-        # 回合数+1
-        race.round_add()
-        #移除超时buff
-        race.del_buff_overtime()
-        #马儿全名计算
-        race.fullname()
-        #回合事件计算
-        text = race.event_start(events_list)
-        #马儿移动
-        race.move()
-        #场地显示
-        display = race.display()
-        
-        output = text_to_png(display,20)
-
-        try:
-            await bot.send(event,(Message(text) + MessageSegment.image(output)))
-        except:
-            text = ""
-            try:
-                await bot.send(event,(MessageSegment.image(output)))
-            except:
-                pass
-
-        await asyncio.sleep(0.5 + int(0.06 * len(text)))
-            
-        #全员失败计算
-        if race.is_die_all():
-            for x in race.player:
-                uid = x.playeruid
-                if uid in user_data:
-                    user = user_data[uid]
-                    user.gold += session.gold
-                    user.group_accounts[group_id].gold += session.gold
-
-            del current_games[group_id]
-            return "比赛已结束，鉴定为无马生还"
-
-        #全员胜利计算
-        winer = race.is_win_all()
-        winer_list="\n"
-        if winer != []:
-            await bot.send(event,(f'> 比赛结束\n'
-                                  f'> {bot_name}正在为您生成战报...'))
-            await asyncio.sleep(1)
-            gold = int(session.gold * player_count / len(winer))
-            for x in winer:
-                uid = x[1]
-                winer_list += "> "+ x[0] + "\n"
-                if uid in user_data:
-                    user = user_data[uid]
-                    user.gold += gold
-                    user.group_accounts[group_id].gold += gold
-            del current_games[group_id]
-            return (f"> 比赛已结束，胜者为：{winer_list}"
-                    f"> 本次奖金：{gold} 金币")
-        await asyncio.sleep(1)
-
-def RaceReStart(event:GroupMessageEvent):
-    """
-    赛马重置
-    """
-    global current_games
-    group_id = event.group_id
-    session = current_games[group_id]
-
-    overtime = time.time() - session.time + 180
-    if overtime < 180:
-        return f"当前赛马已创建 {int(overtime)} 秒，未超时。"
-    race:race_group = session.info["race_group"]
-    for x in race.player:
-        uid = x.playeruid
-        if uid in user_data:
-            user = user_data[uid]
-            user.gold += session.gold
-            user.group_accounts[group_id].gold += session.gold
-
-    del current_games[group_id]
-    return "赛马场已重置。"
-
-"""+++++++++++++++++
-——————————
-     其他小游戏
-——————————
-+++++++++++++++++"""
-
-def slot(event:MessageEvent, gold:int):
+class GameException(Exception):
     """
-    幸运花色
+    GameException
     """
-    user,group_account = Manager.locate_user(event)
-    if not group_account:
-        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
-    if gold > max_bet_gold:
-        return f'幸运花色每次最多{max_bet_gold}金币。'
-    if gold > group_account.gold:
-        return f'你没有足够的金币，你的金币：{user_data["group_account.gold:"]}。'
-    suit = {1:"♤",2:"♡",3:"♧",4:"♢"}
-    x = random.randint(1,4)
-    y = random.randint(1,4)
-    z = random.randint(1,4)
-    res = f"\n| {suit[x]} | {suit[y]} | {suit[z]} |\n"
-    l = len(set([x,y,z]))
-    if l == 1:
-        gold = gold * 7
-        msg =("你抽到的花色为：" +
-              res +
-              f"恭喜你获得了{gold}金币，祝你好运~")
-    elif l == 2:
-        gold = 0
-        msg =("你抽到的花色为：" +
-              res +
-              "祝你好运~")
-    else:
-        gold = -gold
-        msg =("你抽到的花色为：" +
-              res +
-              f"你失去了{-gold}金币 ，祝你好运~")
-    user.gold += gold
-    group_account.gold += gold
-    return msg
-
-"""+++++++++++++++++
-——————————
-      对战系统
-——————————
-+++++++++++++++++"""
 
 class Session(BaseModel):
     """
-    群内进行的游戏
+    游戏场次信息
     """
     time:float = 0.0
+    group_id = 0
     player1_id:int = None
     player2_id:int = None
     at:int = None
     round = 0
     next:int = None
     win:int = None
     gold:int = 0
-    info:dict = {}
+    bet_limit:int = 0
+
     def create(self, event:GroupMessageEvent):
         """
         创建游戏
         """
+        at = get_message_at(event.message)
+        at = int(at[0]) if at else None
         self.__init__(
             time = time.time(),
+            group_id = event.group_id,
             player1_id = event.user_id,
-            at = int(get_message_at(event.message)[0]) if get_message_at(event.message) else None
+            at = at,
+            gold = self.gold
             )
 
     def create_check(self, event:GroupMessageEvent):
         """
         检查是否可以根据event创建游戏
-        如果不能创建则返回提示
-        如果可以创建则返回None
+            如果不能创建则返回提示
+            如果可以创建则返回None
         """
         overtime = time.time() - self.time
         if overtime > 60:
             return None
         user_id = event.user_id
         if player1_id := self.player1_id:
             if player1_id == user_id:
-                return "你已发起了一场对决"
+                if not self.player2_id:
+                    return None
+                else:
+                    return "你已发起了一场对决"
             if player2_id := self.player2_id:
                 if player2_id == user_id:
                     return "你正在进行一场对决"
                 else:
                     player1_name = user_data[player1_id].group_accounts[event.group_id].nickname
                     player2_name = user_data[player2_id].group_accounts[event.group_id].nickname
                     return f"{player1_name} 与 {player2_name} 的对决还未结束！"
@@ -316,38 +95,50 @@
         如果创建失败则返回提示
         如果创建成功则返回None
         """
         if msg := self.create_check(event):
             return msg
         else:
             self.create(event)
+
     def try_join_game(self, event:GroupMessageEvent):
         """
         根据event加入游戏
-        如果加入失败则返回提示
-        如果加入成功则返回None
+            如果加入失败则返回提示
+            如果加入成功则返回None
         """
         if time.time() - self.time > 60:
             return "这场对决邀请已经过时了，请重新发起决斗..."
         user_id = event.user_id
         if self.player1_id and self.player1_id != user_id and not self.next:
             if not self.at or self.at == user_id: 
                 self.time = time.time()
                 self.player2_id = user_id
+                return None
             else:
                 return f'现在是 {user_data[self.player1_id].group_accounts[event.group_id].nickname} 发起的对决，请等待比赛结束后再开始下一轮...'
         else:
             return " "
+
+    def leave(self):
+        """
+        玩家2离开游戏
+        """
+        self.time = time.time()
+        self.player2_id = None
+        return None
+
     def nextround(self):
         """
         把session状态切换到下一回合
         """
         self.time = time.time()
         self.round += 1
         self.next = self.player1_id if self.next == self.player2_id else self.player2_id
+
     def shot_check(self, event:GroupMessageEvent):
         """
         开枪前检查游戏是否合法
         如果不合法则返回提示
         如果合法则返回None
         """
         if time.time() - self.time > 60:
@@ -366,1208 +157,1498 @@
             else:
                 return f"现在是{user_data[self.next].group_accounts[event.group_id].nickname}的回合"
         else:
             player1_name = user_data[self.player1_id].group_accounts[event.group_id].nickname
             player2_name = user_data[self.player2_id].group_accounts[event.group_id].nickname
             return f"{player1_name} v.s. {player2_name}\n正在进行中..."
 
-current_games:Dict[int,Session] = {}
-
-def accept(event:GroupMessageEvent):
+class Game(ABC):
     """
-    接受挑战
-    """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.try_join_game(event):
-        return None if msg == " " else msg
-    group_account = Manager.locate_user(event)[1]
-    if session.info["game"] == "random":
-        session.gold = random.randint(0, 0 if(mingold := min(group_account.gold,session.info["gold"])) < 0 else mingold) if session.gold == -1 else session.gold
-        game = random.choice(["russian","dice","lucky_number","cantrell", "Blackjack"])
-        if game == "russian":
-            session.info = russian_info(random.randint(1,6))
-        elif game == "dice":
-            session.info = dice_info(session.gold)
-        elif game == "poker":
-            session.info = poker_info()
-        elif game == "lucky_number":
-            session.info = lucky_number_info(session.gold)
-        elif game == "cantrell":
-            session.info = cantrell_info(session.gold)
-        elif game == "Blackjack":
-            session.info = Blackjack_info()
-    elif group_account.gold <  session.gold:
-        del current_games[group_id]
-        return Message(MessageSegment.at(event.user_id) + f"你的金币不足以接受这场对决！\n——你还有{group_account.gold}枚金币。")
+    对战游戏类：
+    需要定义的方法：
+        action：游戏进行
+        game_tips：游戏开始的提示
+        session_tips：场次提示信息
+        end_tips：结束附件
+    """
+    name:str = "undefined"
+    max_bet_gold:int = max_bet_gold
+
+    def __init__(self):
+        self.session:Session = Session()
+
+    @staticmethod
+    def parse_arg(arg:str):
+        if arg.isdigit():
+            gold = int(arg)
+        else:
+            gold = bet_gold
+        return {"gold":gold}
+
+    @classmethod
+    def creat(cls, event:GroupMessageEvent, **kwargs):
+        """
+        发起游戏
+        """
+        flag, msg = cls.start(event, **kwargs)
+        if flag == False:
+            return msg
+        return current_games[event.group_id].game_tips(msg)
+
+    @abstractmethod
+    def game_tips(self, msg):
+        """
+        游戏开始的提示
+        """
+
+    @abstractmethod
+    async def action(self, bot:Bot, event:GroupMessageEvent):
+        """
+        游戏进行
+        """
+
+    async def play(self, bot:Bot, event:GroupMessageEvent, *args):
+        try:
+            return await self.action(bot, event, *args)
+        except GameException:
+            pass
+
+    def accept(self, event:GroupMessageEvent):
+        """
+        接受挑战
+        """
+        session = self.session
+        group_id = session.group_id
+        if msg := session.try_join_game(event):
+            return None if msg == " " else msg
+        group_account = Manager.locate_user(event)[1]
+        if group_account.gold <  session.gold:
+            session.leave()
+            return Message(MessageSegment.at(event.user_id) + f"你的金币不足以接受这场对决！\n——你还有{group_account.gold}枚金币。")
+
+        bet_limit = min(
+            user_data[session.player1_id].group_accounts[group_id].gold,
+            user_data[session.player2_id].group_accounts[group_id].gold)
+        bet_limit = bet_limit if bet_limit > 0 else 0
+        session.gold = random.randint(0, bet_limit)if session.gold == -1 else session.gold
+        session.bet_limit = bet_limit
+        session.next = session.player1_id
+        return self.session_tips()
+
+    @abstractmethod
+    def session_tips(self):
+        """
+        场次提示信息
+        """
+
+    def acceptmessage(self, tip1, tip2):
+        """
+        合成接受挑战的提示信息
+        """
+        session = self.session
+        return Message(
+            f"{MessageSegment.at(session.player2_id)}接受了对决！\n" +
+            tip1 +
+            f"赌注为 {session.gold} 金币\n" +
+            f"请{MessageSegment.at(session.player1_id)}{tip2}"
+            )
+
+    def refuse(self, event:GroupMessageEvent):
+        """
+        拒绝挑战
+        """
+        session = self.session
+        group_id = session.group_id
+        if time.time() - session.time > 60:
+            del current_games[group_id]
+        if session.at == event.user_id:
+            if session.player2_id:
+                return "对决已开始，拒绝失败。"
+            else:
+                del current_games[group_id]
+                return "拒绝成功，对决已结束。"
+
+    async def overtime(self, bot:Bot, event:GroupMessageEvent):
+        """
+        超时结算
+        """
+        session = self.session
+        if (time.time() - session.time > 30 and
+            session.player1_id and
+            session.player2_id):
+            try:
+                await self.end(bot, event)
+            except GameException:
+                pass
+
+    async def fold(self, bot:Bot, event:GroupMessageEvent):
+        """
+        认输
+        """
+        session = self.session
+        user_id = event.user_id
+        if (time.time() - session.time < 60 and
+            session.player1_id and
+            session.player2_id and
+            user_id == session.player1_id or user_id == session.player2_id):
+            session.win = session.player1_id if user_id == session.player2_id else session.player2_id
+            try:
+                await self.end(bot, event)
+            except GameException:
+                pass
+
+    @classmethod
+    def start(cls, event:GroupMessageEvent, **kwargs) -> Tuple[bool,Message]:
+        """
+        发起游戏
+        """
+        gold = kwargs["gold"]
+        limit = cls.max_bet_gold
+        if gold > limit:
+            return  False, Message(MessageSegment.at(event.user_id) + f"对战金额不能超过{limit}")
+        group_account = Manager.locate_user(event)[1]
+        if gold > group_account.gold:
+            return  False, Message(MessageSegment.at(event.user_id) + f"你没有足够的金币支撑这场对决。\n——你还有{group_account.gold}枚金币。")
+
+        group_id = event.group_id
+        if group_id in current_games:
+            game = current_games[group_id]
+            if msg := game.session.create_check(event):
+                return False, msg
+
+        game = current_games[group_id] = cls(**kwargs)
+        session = game.session
+        session.create(event)
+        assert session is current_games[group_id].session
+        if at := session.at:
+            if at not in group_data[group_id].namelist:
+                del current_games[group_id]
+                return False, "没有对方的注册信息。"
+            player1_name = user_data[session.player1_id].group_accounts[event.group_id].nickname
+            player2_name = user_data[at].group_accounts[event.group_id].nickname
+            msg = (f"{player1_name} 向 {player2_name} 发起挑战！\n"
+                   f"请 {player2_name} 回复 接受挑战 or 拒绝挑战\n"
+                   "【30秒内有效】")
+        else:
+            player1_name = user_data[session.player1_id].group_accounts[event.group_id].nickname
+            msg = (f"{player1_name} 发起挑战！\n"
+                   "回复 接受挑战 即可开始对局。\n"
+                   "【30秒内有效】")
+
+        session.round = 1
+        return True, msg
+
+    def settle(self, group_id:int):
+        """
+        游戏结束结算
+            return:结算界面
+        """
+        session = self.session
+
+        win = session.win if session.win else session.player1_id if session.next == session.player2_id else session.player2_id
+        winner = user_data[win]
+        winner_group_account = winner.group_accounts[group_id]
+
+        lose = session.player1_id if session.player2_id == win else session.player2_id
+        loser = user_data[lose]
+        loser_group_account = loser.group_accounts[group_id]
+
+        gold = session.gold
+
+        if winner_group_account.props.get("42001",0) > 0:
+            fee = 0
+            fee_tip = f"『{props_library['42001']['name']}』免手续费"
+        else:
+            rand = random.randint(0, 5)
+            fee = int(gold * rand / 100)
+            fee_tip = f"手续费：{fee}({rand}%)"
+
+        maxgold = int(max_bet_gold/5)
+
+        if winner_group_account.props.get("52002",0) > 0:
+            extra = int(gold *0.1)
+            if extra < maxgold:
+                extra_tip = f"◆『{props_library['52002']['name']}』\n"
+            else:
+                extra = maxgold
+                extra_tip = f"◆『{props_library['52002']['name']}』最大奖励\n"
+        else:
+            extra_tip = ""
+            extra = 0
+
+        if gold == loser_group_account.gold and loser_group_account.security < 3:
+            loser_group_account.security += 1
+            security = random.randint(security_gold[0], security_gold[1])
+            security_tip1 = "◇『金币补贴』\n"
+            security_tip2 = f"◇已领取补贴：{security}\n"
+        else:
+            security = 0
+            security_tip1 = ""
+            security_tip2 = ""
+
+        if loser_group_account.props.get("52001",0) > 0:
+            off = int(gold * 0.1)
+            if off < maxgold:
+                off_tip = f"◇『{props_library['52001']['name']}』\n"
+            else:
+                off = maxgold
+                off_tip = f"◇『{props_library['52001']['name']}』最大补贴\n"
+
+        else:
+            off = 0
+            off_tip = ""
+
+        win_gold = gold - fee + extra
+        winner.win += 1
+        winner.Achieve_win += 1
+        winner.Achieve_lose = 0
+
+        lose_gold = gold - off
+        loser.lose += 1
+        loser.Achieve_lose += 1
+        loser.Achieve_win = 0
+
+        msg = (
+            f"结算：\n"
+            "——————————————\n" +
+            (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((winner,winner_group_account)))) else "") +
+            extra_tip +
+            f"◆胜者：{winner_group_account.nickname}\n"
+            f"◆结算：{winner_group_account.gold}（+{win_gold}）\n"
+            f"◆战绩：{winner.win}:{winner.lose}\n"
+            f"◆胜率：{round(winner.win * 100 / (winner.win + winner.lose), 2) if winner.win > 0 else 0}%\n"
+            "——————————————\n" +
+            (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((loser,loser_group_account)))) else "") +
+            security_tip1 +
+            off_tip +
+            f"◇败者：{loser_group_account.nickname}\n"
+            f"◇结算：{loser_group_account.gold}（-{lose_gold}）\n" +
+            security_tip2 +
+            f"◇战绩：{loser.win}:{loser.lose}\n"
+            f"◇胜率：{round(loser.win * 100 / (loser.win + loser.lose), 2) if loser.win > 0 else 0}%\n"
+            "——————————————\n" + 
+            fee_tip
+            )
+        winner.gold += win_gold
+        winner_group_account.gold += win_gold
+        loser.gold -= lose_gold - security
+        loser_group_account.gold -= lose_gold - security
 
-    bet_limit = min(
-        user_data[session.player1_id].group_accounts[group_id].gold,
-        user_data[session.player2_id].group_accounts[group_id].gold)
-    bet_limit = bet_limit if bet_limit > 0 else 0
-    session.info["bet_limit"] = bet_limit
-    session.next = session.player1_id
-    return acceptmessage(session)
-
-def acceptmessage(session:Session):
-    """
-    生成接受挑战的提示信息
-    """
-    game = session.info.get("game")
-    gold = session.gold
-    if game == "russian":
-        tip1 = "本场对决为【俄罗斯轮盘】\n"
-        tip2 = "开枪！"
-    elif game == "dice":
-        gold = session.info["max_gold"]
-        tip1 = "本场对决为【掷色子】\n"
-        tip2 = "开数！"
-    elif game == "poker":
-        tip1 = "本场对决为【扑克对战】\n"
-        tip2 = "加注！\n"
-        tip2 += MessageSegment.image(text_to_png(
-            "P1初始状态\n"
-            f'HP {session.info["P1"]["HP"]} SP {session.info["P1"]["SP"]} DEF {session.info["P1"]["DEF"]}\n'
-            "——————————————\n"
-            "P2初始状态\n"
-            f'HP {session.info["P2"]["HP"]} SP {session.info["P2"]["SP"]} DEF {session.info["P2"]["DEF"]}\n'
-            "——————————————\n"
-            "P1初始手牌\n" + 
-            "".join([f'【{pokerACT.suit[suit]}{pokerACT.point[point]}】' for suit, point in session.info["P1"]["hand"]])
-            ),30)
-    elif game == "lucky_number":
-        tip1 = "本场对决为【猜数字】\n"
-        tip2 = "发送数字"
-    elif game == "cantrell":
-        tip1 = "本场对决为【港式五张】\n"
-        tip2 = "开牌！\n"
-        tip2 += MessageSegment.image(text_to_png(
-                "P1初始手牌：\n"
-                "|"
-                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"][0:3]]) +
-                "   |   |"
-                "\n——————————————\n"
-                'P2初始手牌\n'
-                "|"
-                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"][0:3]]) +
-                "   |   |"
-                ),30)
-    elif game == "Blackjack":
-        hand1 = session.info["hand1"][0]
-        hand2 = session.info["hand2"][0]
-        tip1 = "本场对决为【21点】\n"
-        tip2 = "\n抽牌|停牌|双倍下注\n"
-        tip2 += (
-            f"P1：{Blackjack_suit[hand1[0]]}{Blackjack_point[hand1[1]]}\n"
-            f"P2：{Blackjack_suit[hand2[0]]}{Blackjack_point[hand2[1]]}")
-    else:
-        tip1 = ""
-        tip2 = ""
-    return Message(
-        f"{MessageSegment.at(session.player2_id)}接受了对决！\n" +
-        tip1 +
-        f"赌注为 {gold} 金币\n" +
-        f"请{MessageSegment.at(session.player1_id)}{tip2}"
-        )
-
-def refuse(event:GroupMessageEvent):
-    """
-    拒绝挑战
-    """
-    global current_games
-    group_id = event.group_id
-    session = current_games[group_id]
-    if time.time() - session.time > 60:
         del current_games[group_id]
-        return None
-    if session.at == event.user_id:
-        if session.player2_id:
-            return "对决已开始，拒绝失败。"
+        return f"这场对决是 {winner_group_account.nickname} 胜利了", msg, self.end_tips()
+
+    @abstractmethod
+    def end_tips(self):
+        """
+        结束附件
+        """
+
+    async def end(self, bot:Bot, event:GroupMessageEvent):
+        """
+        输出结算界面
+        """
+        result = self.settle(event.group_id)
+        tmp = MessageSegment.image(text_to_png(result[1], width_simple = "——————————————"))
+        await bot.send(event,result[0])
+        await bot.send(event,tmp)
+        await asyncio.sleep(0.5)
+        await bot.send(event,result[2])
+        raise GameException
+
+current_games:Dict[int,Game] = {}
+
+class Russian(Game):
+    """
+    俄罗斯轮盘
+    """
+    name = "Russian"
+    max_bet_gold:int = max_bet_gold
+
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        bullet_num = kwargs["bullet_num"]
+        self.bullet_num:int = bullet_num
+        self.bullet:list = self.random_bullet(bullet_num)
+        self.index:int = 0
+        self.session.gold = gold
+
+    @staticmethod
+    def parse_arg(arg:str):
+        gold = bet_gold
+        bullet_num = 1
+        if arg:
+            arg = arg.split()
+            if len(arg) == 1:
+                arg = arg[0]
+                if arg.isdigit():
+                    if 0 < (tmp := int(arg)) < 7:
+                        bullet_num = tmp
+                    else:
+                        gold = tmp
+            else:
+                if arg[0].isdigit():
+                    if 0 < (tmp := int(arg[0])) < 7:
+                        bullet_num = tmp
+                        if arg[1].isdigit():
+                            gold = int(arg[1])
+                    else:
+                        gold = tmp
+
+        return {"gold":gold,"bullet_num":bullet_num}
+
+    @staticmethod
+    def random_bullet(bullet_num:int):
+        """
+        随机子弹排列
+            bullet_num:装填子弹数量
+        """
+        bullet_lst = [0, 0, 0, 0, 0, 0, 0]
+        for i in random.sample([0, 1, 2, 3, 4, 5, 6], bullet_num):
+            bullet_lst[i] = 1
+        return bullet_lst
+
+    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+        """
+        开枪！！！
+        """
+        session = self.session
+        if msg := session.shot_check(event):
+            return None if msg == " " else msg
+        group_id = session.group_id
+
+        index = self.index
+        MAG = self.bullet[index:]
+        count = args[0] if args[0] else 1
+        count = len(MAG) if count < 1 else count
+
+        msg = f"连开{count}枪！\n" if count > 1 else ""
+
+        if 1 in MAG[:count]:
+            session.win = session.player1_id if event.user_id == session.player2_id else session.player2_id
+            await bot.send(event,(
+                MessageSegment.at(event.user_id) + msg +
+                random.choice(["嘭！，你直接去世了","眼前一黑，你直接穿越到了异世界...(死亡)","终究还是你先走一步..."]) +
+                f"\n第 {index + MAG.index(1) + 1} 发子弹送走了你..."
+                ))
+            await self.end(bot, event)
         else:
-            del current_games[group_id]
-            return "拒绝成功，对决已结束。"
+            session.nextround()
+            self.index += count
+            next_name = user_data[session.next].group_accounts[group_id].nickname
+            await bot.send(event,msg + (
+                random.choice(["呼呼，没有爆裂的声响，你活了下来",
+                               "虽然黑洞洞的枪口很恐怖，但好在没有子弹射出来，你活下来了",
+                               f'{"咔 "*count}，看来运气不错，你活了下来']) +
+                f"\n下一枪中弹的概率：{round(self.bullet_num * 100 / (len(MAG) - count),2)}%\n"
+                f"轮到 {next_name}了"
+                ))
 
-async def overtime(bot:Bot, event:GroupMessageEvent):
-    """
-    超时结算
-    """
-    global current_games
-    session = current_games[event.group_id]
-    if (time.time() - session.time > 30 and
-        session.player1_id and
-        session.player2_id):
-        await end(bot, event)
+    def game_tips(self, msg):
+        """
+        发起游戏：俄罗斯轮盘
+        """
+        return (("咔 " * self.bullet_num)[:-1] + "，装填完毕\n"
+                f'挑战金额：{self.session.gold}\n'
+                f'第一枪的概率为：{round(self.bullet_num * 100 / 7,2)}%\n'
+                f'{msg}')
 
-async def fold(bot:Bot, event:GroupMessageEvent):
-    """
-    认输
-    """
-    global current_games
-    session = current_games[event.group_id]
-    user_id = event.user_id
-    if (time.time() - session.time < 60 and
-        session.player1_id and
-        session.player2_id and
-        user_id == session.player1_id or user_id == session.player2_id):
-        session.win = session.player1_id if user_id == session.player2_id else session.player2_id
-        await end(bot, event)
+    def session_tips(self):
+        tip1 = "本场对决为【俄罗斯轮盘】\n"
+        tip2 = "开枪！"
+        return self.acceptmessage(tip1, tip2);
 
-def start(event:GroupMessageEvent, gold:int, max_bet_gold:int = max_bet_gold) -> Tuple[bool,Message]:
+    def end_tips(self):
+        return " ".join(("—" if x == 0 else "|") for x in self.bullet)
+
+class Dice(Game):
     """
-    发起游戏
+    掷色子
     """
-    if gold > max_bet_gold:
-        return  False, Message(MessageSegment.at(event.user_id) + f"对战金额不能超过{max_bet_gold}")
-    group_account = Manager.locate_user(event)[1]
-    if gold > group_account.gold:
-        return  False, Message(MessageSegment.at(event.user_id) + f"你没有足够的金币支撑这场对决。\n——你还有{group_account.gold}枚金币。")
+    name = "Dice"
+    max_bet_gold:int = max_bet_gold *10
 
-    global current_games
-    group_id = event.group_id
-    session = current_games.setdefault(group_id,Session())
-    if msg := session.try_create_game(event):
-        return False, msg
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        self.gold:int = gold
+        self.dice_array1:list = [random.randint(1,6) for i in range(5)]
+        self.dice_array2:list = [random.randint(1,6) for i in range(5)]
+        self.session.gold = gold
 
-    if at := session.at:
-        if at not in group_data[group_id].namelist:
-            del current_games[group_id]
-            return False, "没有对方的注册信息。"
-        player1_name = user_data[session.player1_id].group_accounts[event.group_id].nickname
-        player2_name = user_data[at].group_accounts[event.group_id].nickname
-        msg = (f"{player1_name} 向 {player2_name} 发起挑战！\n"
-               f"请 {player2_name} 回复 接受挑战 or 拒绝挑战\n"
-               "【30秒内有效】")
-    else:
-        player1_name = user_data[session.player1_id].group_accounts[event.group_id].nickname
-        msg = (f"{player1_name} 发起挑战！\n"
-               "回复 接受挑战 即可开始对局。\n"
-               "【30秒内有效】")
-    session.round += 1
-    return True, msg
-
-"""+++++++++++++++++
-——————————
-     俄罗斯轮盘
-——————————
-+++++++++++++++++"""
-
-def random_bullet(bullet_num:int):
-    """
-    随机子弹排列
-        bullet_num:装填子弹数量
-    """
-    bullet_lst = [0, 0, 0, 0, 0, 0, 0]
-    for i in random.sample([0, 1, 2, 3, 4, 5, 6], bullet_num):
-        bullet_lst[i] = 1
-    return bullet_lst
-
-def russian_info(bullet_num):
-    """
-    生成俄罗斯轮盘游戏内容
-    """
-    return {
-        "game":"russian",
-        "bullet_num":bullet_num,
-        "bullet":random_bullet(bullet_num),
-        "index":0
-        }
-
-def russian(event:GroupMessageEvent, bullet_num:int, gold:int):
-    """
-    发起游戏：俄罗斯轮盘
-        bullet_num:装填子弹数量
-    """
-    flag, msg = start(event, gold)
-    if flag == False:
-        return msg
-    session = current_games[event.group_id]
-    session.gold = gold
-    session.info = russian_info(bullet_num)
-    return (("咔 " * bullet_num)[:-1] + "，装填完毕\n"
-            f"挑战金额：{gold}\n"
-            f"第一枪的概率为：{round(bullet_num / 7.0 * 100,2)}%\n"
-            f"{msg}")
-
-async def russian_shot(bot:Bot, event:GroupMessageEvent, count:int):
-    """
-    开枪！！！
-    """
-    global current_games
-    session = current_games[event.group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    index = session.info["index"]
-    MAG = session.info["bullet"][index:]
-    count = len(MAG) if count < 1 else count
-    msg = f"连开{count}枪！\n" if count > 1 else ""
-    if 1 in MAG[:count]:
-        session.win = session.player1_id if event.user_id == session.player2_id else session.player2_id
-        await bot.send(event,(
-            MessageSegment.at(event.user_id) + msg +
-            random.choice(["嘭！，你直接去世了","眼前一黑，你直接穿越到了异世界...(死亡)","终究还是你先走一步..."]) +
-            f"\n第 {index + MAG.index(1) + 1} 发子弹送走了你..."
-            ))
-        await end(bot, event)
-    else:
-        session.nextround()
-        session.info["index"] += count
-        next_name = user_data[session.next].group_accounts[event.group_id].nickname
-        await bot.send(event,msg + (
-            random.choice(["呼呼，没有爆裂的声响，你活了下来",
-                           "虽然黑洞洞的枪口很恐怖，但好在没有子弹射出来，你活下来了",
-                           f'{"咔 "*count}，看来运气不错，你活了下来']) +
-            f"\n下一枪中弹的概率：{round(session.info['bullet_num'] * 100 / (len(MAG) - count),2)}%\n"
-            f"轮到 {next_name}了"
-            ))
-
-"""+++++++++++++++++
-——————————
-       掷色子
-——————————
-+++++++++++++++++"""
-
-def dice_pt(dice_array:list) -> int:
-    """
-    计算骰子排列pt
-    """
-    pt = 0
-    for i in range(1,7):
-        if dice_array.count(i) <= 1:
-            pt += i * dice_array.count(i)
-        elif dice_array.count(i) == 2:
-            pt += (100 + i) * (10 ** dice_array.count(i))
+    @staticmethod
+    def dice_pt(dice_array:list) -> int:
+        """
+        计算骰子排列pt
+        """
+        pt = 0
+        for i in range(1,7):
+            if dice_array.count(i) <= 1:
+                pt += i * dice_array.count(i)
+            elif dice_array.count(i) == 2:
+                pt += (100 + i) * (10 ** dice_array.count(i))
+            else:
+                pt += i * (10 ** (2 + dice_array.count(i)))
         else:
-            pt += i * (10 ** (2 + dice_array.count(i)))
-    else:
-        return pt
+            return pt
 
-def dice_pt_analyses(pt:int) -> str:
-    """
-    分析骰子pt
-    """
-    array_type = ""
-    if (yiman := int(pt/10000000)) > 0:
-        pt -= yiman * 10000000
-        array_type += f"役满 {yiman} + "
-    if (chuan := int(pt/1000000)) > 0:
-        pt -= chuan * 1000000
-        array_type += f"串 {chuan} + "
-    if (tiao := int(pt/100000)) > 0:
-        pt -= tiao * 100000
-        array_type += f"条 {tiao} + "
-    if (dui := int(pt/10000)) > 0:
-        if dui == 1:
-            pt -= 10000
-            dui = int(pt/100)
-            array_type += f"对 {dui} + "
-        else:
-            pt -= 20000
-            dui = int(pt/100)
-            array_type += f"两对 {dui} + "
-        pt -= dui * 100
-    if pt>0:
-        array_type += f"散 {pt} + "
-    return array_type[:-3]
-
-def dice_list(dice_array:list) -> str:
-    """
-    把骰子列表转成字符串
-    """
-    lst_dict = {0:"〇",1:"１",2:"２",3:"３",4:"４",5:"５",6:"６",7:"７",8:"８",9:"９"}
-    return " ".join(lst_dict[x] for x in dice_array)
-
-def dice_info(gold):
-    """
-    生成掷色子游戏内容
-    """
-    return {
-        "game":"dice",
-        "max_gold":gold,
-        "dice_array1":[random.randint(1,6) for i in range(5)],
-        "dice_array2":[random.randint(1,6) for i in range(5)],
-        }
-
-def dice(event:GroupMessageEvent, gold:int):
-    """
-    发起游戏：掷色子
-    """
-    flag, msg = start(event, gold, max_bet_gold * 10)
-    if flag == False:
-        return msg
-    session = current_games[event.group_id]
-    session.gold = int(gold/10)
-    session.info = dice_info(gold)
-    return ("哗啦哗啦~，骰子准备完毕\n"
-            f"挑战金额：{gold}\n"
-            f"{msg}")
-
-async def dice_open(bot:Bot, event:GroupMessageEvent):
-    """
-    开数！！！
-    """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
+    @staticmethod
+    def dice_pt_analyses(pt:int) -> str:
+        """
+        分析骰子pt
+        """
+        array_type = ""
+        if (yiman := int(pt/10000000)) > 0:
+            pt -= yiman * 10000000
+            array_type += f"役满 {yiman} + "
+        if (chuan := int(pt/1000000)) > 0:
+            pt -= chuan * 1000000
+            array_type += f"串 {chuan} + "
+        if (tiao := int(pt/100000)) > 0:
+            pt -= tiao * 100000
+            array_type += f"条 {tiao} + "
+        if (dui := int(pt/10000)) > 0:
+            if dui == 1:
+                pt -= 10000
+                dui = int(pt/100)
+                array_type += f"对 {dui} + "
+            else:
+                pt -= 20000
+                dui = int(pt/100)
+                array_type += f"两对 {dui} + "
+            pt -= dui * 100
+        if pt>0:
+            array_type += f"散 {pt} + "
+        return array_type[:-3]
+
+    @staticmethod
+    def dice_list(dice_array:list) -> str:
+        """
+        把骰子列表转成字符串
+        """
+        lst_dict = {0:"〇",1:"１",2:"２",3:"３",4:"４",5:"５",6:"６",7:"７",8:"８",9:"９"}
+        return " ".join(lst_dict[x] for x in dice_array)
 
-    session.gold = int(session.info["max_gold"] * session.round/10)
+    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+        """
+        开数！！！
+        """
+        session = self.session
+        if msg := session.shot_check(event):
+            return None if msg == " " else msg
+        group_id = session.group_id
 
-    player1_id = session.player1_id
-    player2_id = session.player2_id
+        session.gold += self.gold
+        session.gold = min(session.gold, session.bet_limit)
 
-    dice_array1 = (session.info["dice_array1"][:int(session.round/2+0.5)] + [0, 0, 0, 0, 0])[:5]
-    dice_array2 = (session.info["dice_array2"][:int(session.round/2)] + [0, 0, 0, 0, 0])[:5]
+        player1_id = session.player1_id
+        player2_id = session.player2_id
+
+        dice_array1 = (self.dice_array1[:int(session.round/2+0.5)] + [0, 0, 0, 0, 0])[:5]
+        dice_array2 = (self.dice_array2[:int(session.round/2)] + [0, 0, 0, 0, 0])[:5]
     
-    dice_array1.sort(reverse=True)
-    dice_array2.sort(reverse=True)
+        dice_array1.sort(reverse=True)
+        dice_array2.sort(reverse=True)
+
+        pt1 = self.dice_pt(dice_array1)
+        pt2 = self.dice_pt(dice_array2)
 
-    pt1 = dice_pt(dice_array1)
-    pt2 = dice_pt(dice_array2)
+        session.win = player1_id if pt1 > pt2 else player2_id
+        session.nextround()
 
-    session.win = player1_id if pt1 > pt2 else player2_id
-    session.nextround()
+        next_name = "结算" if session.round > 10 else user_data[session.next].group_accounts[group_id].nickname
+        msg = (
+            f'玩家：{user_data[player1_id].group_accounts[group_id].nickname}\n'
+            f"组合：{self.dice_list(dice_array1)}\n"
+            f"点数：{self.dice_pt_analyses(pt1)}\n"
+            "———————————\n"
+            f'玩家：{user_data[player2_id].group_accounts[group_id].nickname}\n'
+            f"组合：{self.dice_list(dice_array2)}\n"
+            f"点数：{self.dice_pt_analyses(pt2)}\n"
+            "———————————\n"
+            f"结算金额：{session.gold}\n"
+            f'领先：{user_data[session.win].group_accounts[group_id].nickname}\n'
+            f'下一回合：{next_name}'
+            )
+        await bot.send(event,message = MessageSegment.image(text_to_png(msg, 50, width_simple = "———————————")))
+        if session.round > 10:
+            await self.end(bot, event)
 
-    next_name = "结算" if session.round > 10 else user_data[session.next].group_accounts[group_id].nickname
-    msg = (
-        f'玩家：{user_data[player1_id].group_accounts[group_id].nickname}\n'
-        f"组合：{dice_list(dice_array1)}\n"
-        f"点数：{dice_pt_analyses(pt1)}\n"
-        "———————————\n"
-        f'玩家：{user_data[player2_id].group_accounts[group_id].nickname}\n'
-        f"组合：{dice_list(dice_array2)}\n"
-        f"点数：{dice_pt_analyses(pt2)}\n"
-        "———————————\n"
-        f"结算金额：{session.gold}\n"
-        f'领先：{user_data[session.win].group_accounts[group_id].nickname}\n'
-        f'下一回合：{next_name}'
-        )
-    await bot.send(event,message = MessageSegment.image(text_to_png(msg,30)))
-    if session.round > 10:
-        await end(bot, event)
-
-"""+++++++++++++++++
-——————————
-      扑克对战
-——————————
-+++++++++++++++++"""
-
-def random_poker():
-    """
-    生成随机牌库
-    """
-    poker_deck = [[i,j] for i in range(1,5) for j in range(1,14)]
-    random.shuffle(poker_deck)
-    return poker_deck
-
-def poker_info():
-    """
-    生成扑克对战游戏内容
-    """
-    deck = random_poker()
-    hand = deck[0:3].copy()
-    del deck[0:3]
-    return {
-        "game":"poker",
-        "deck":deck + [[0,0],[0,0],[0,0],[0,0]],
-        "ACT":1,
-        "P1":{"hand":hand,"HP":20,"ATK":0,"DEF":0,"SP":0},
-        "P2":{"hand":[],"HP":25,"ATK":0,"DEF":0,"SP":2}
-        }
-
-def poker(event:GroupMessageEvent, gold:int):
-    """
-    发起游戏：扑克对战
-    """
-    flag, msg = start(event, gold)
-    if flag == False:
-        return msg
-    session = current_games[event.group_id]
-    session.gold = gold
-    session.info = poker_info()
-    return ("唰唰~，随机牌库已生成\n"
-            f"挑战金额：{gold}\n"
-            f"{msg}")
-
-class pokerACT():
-    suit = {0:"结束",1:"防御",2:"恢复",3:"技能",4:"攻击"}
-    point = {0:"0",1:"A",2:"2",3:"3",4:"4",5:"5",6:"6",7:"7",8:"8",9:"9",10:"10",11:"11",12:"12",13:"13"}
-    @classmethod
-    def action_ACE(cls, Active:dict, roll:int = 1) -> str:
-        '''
-        手牌全部作为技能牌（ACE技能）
-            Active:行动牌生效对象
-        '''
-        card_msg = "技能牌为"
-        skill_msg = "\n"
-        for card in Active["hand"]:
+    def game_tips(self, msg):
+        """
+        发起游戏：掷色子
+        """
+        return ("哗啦哗啦~，骰子准备完毕\n"
+                f'挑战金额：{self.gold}/次\n'
+                f'{msg}')
+
+    def session_tips(self):
+        tip1 = "本场对决为【掷色子】\n"
+        tip2 = "开数！"
+        return self.acceptmessage(tip1, tip2);
+
+    def end_tips(self):
+        return (
+            f'玩家 1\n'
+            f'组合：{" ".join(str(x) for x in self.dice_array2)}\n'
+            f'玩家 2\n'
+            f'组合：{" ".join(str(x) for x in self.dice_array2)}')
+
+class Poker(Game):
+    """
+    扑克对战
+    """
+    name = "Poker"
+    max_bet_gold:int = max_bet_gold *10
+
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        deck = self.random_poker()
+        hand = deck[0:3].copy()
+        del deck[0:3]
+        self.deck:list = deck + [[0,0],[0,0],[0,0],[0,0]]
+        self.ACT:int = 1
+        self.P1:dict = {"hand":hand,"HP":20,"ATK":0,"DEF":0,"SP":0}
+        self.P2:dict = {"hand":[],"HP":25,"ATK":0,"DEF":0,"SP":2}
+        self.session.gold = gold
+
+    @staticmethod
+    def random_poker():
+        """
+        生成随机牌库
+        """
+        poker_deck = [[i,j] for i in range(1,5) for j in range(1,14)]
+        random.shuffle(poker_deck)
+        return poker_deck
+
+    class pokerACT():
+        suit = {0:"结束",1:"防御",2:"恢复",3:"技能",4:"攻击"}
+        point = {0:"0",1:"A",2:"2",3:"3",4:"4",5:"5",6:"6",7:"7",8:"8",9:"9",10:"10",11:"11",12:"12",13:"13"}
+
+        @classmethod
+        def action_ACE(cls, Active:dict, roll:int = 1) -> str:
+            '''
+            手牌全部作为技能牌（ACE技能）
+                Active:行动牌生效对象
+            '''
+            card_msg = "技能牌为"
+            skill_msg = "\n"
+            for card in Active["hand"]:
+                suit = card[0]
+                point = roll if card[1] == 1 else card[1]
+                card_msg += f'【{cls.suit[suit]} {cls.point[point]}】'
+                if suit == 1:
+                    Active["DEF"] += point
+                    skill_msg += f'♤防御力强化了 {point}\n'
+                elif suit == 2:
+                    Active["HP"] += point
+                    skill_msg += f'♡生命值增加了 {point}\n'
+                elif suit == 3:
+                    Active["SP"] += point + point
+                    skill_msg += f'♧技能点增加了 {point}\n'
+                elif suit == 4:
+                    Active["ATK"] += point
+                    skill_msg += f'♢发动了攻击 {point}\n'
+                else:
+                    return "出现未知错误"
+                Active["SP"] -= point
+                Active["SP"] = 0 if Active["SP"] < 0 else Active["SP"]
+            return card_msg + skill_msg[:-1]
+
+        @classmethod
+        def action(cls, index:int, Active:dict) -> str:
+            '''
+            行动牌生效
+                index:手牌序号
+                Active:行动牌生效对象
+            '''
+            card = Active["hand"][index]
             suit = card[0]
-            point = roll if card[1] == 1 else card[1]
-            card_msg += f'【{cls.suit[suit]} {cls.point[point]}】'
-            if suit == 1:
-                Active["DEF"] += point
-                skill_msg += f'♤防御力强化了 {point}\n'
-            elif suit == 2:
-                Active["HP"] += point
-                skill_msg += f'♡生命值增加了 {point}\n'
-            elif suit == 3:
-                Active["SP"] += point + point
-                skill_msg += f'♧技能点增加了 {point}\n'
-            elif suit == 4:
-                Active["ATK"] += point
-                skill_msg += f'♢发动了攻击 {point}\n'
+            point = card[1]
+            if point == 1:
+                roll = random.randint(1,6)
+                msg = f'发动ACE技能！六面骰子判定为 {roll}\n'
+                msg += cls.action_ACE(Active, roll)
             else:
-                return "出现未知错误"
-            Active["SP"] -= point
-            Active["SP"] = 0 if Active["SP"] < 0 else Active["SP"]
-        return card_msg + skill_msg[:-1]
-    @classmethod
-    def action(cls, index:int, Active:dict) -> str:
-        '''
-        行动牌生效
-            index:手牌序号
-            Active:行动牌生效对象
-        '''
-        card = Active["hand"][index]
-        suit = card[0]
-        point = card[1]
-        if point == 1:
-            roll = random.randint(1,6)
-            msg = f'发动ACE技能！六面骰子判定为 {roll}\n'
-            msg += cls.action_ACE(Active, roll)
-        else:
+                if suit == 1:
+                    Active["ATK"] += point
+                    msg = f"♤发动了攻击{point}"
+                elif suit == 2:
+                    Active["HP"] += point
+                    msg = f"♡生命值增加了{point}"
+                elif suit == 3:
+                    Active["SP"] += point
+                    msg = f"♧技能点增加了{point}...\n"
+                    roll = random.randint(1,20)
+                    if Active["SP"] < roll:
+                        msg += f'二十面骰判定为{roll}点，当前技能点{Active["SP"]}\n技能发动失败...'
+                    else:
+                        del Active["hand"][index]
+                        msg += f'二十面骰判定为{roll}点，当前技能点{Active["SP"]}\n技能发动成功！\n'
+                        msg += cls.action_ACE(Active)
+                elif suit == 4:
+                    Active["ATK"] = point
+                    msg = f"♢发动了攻击{point}"
+                else:
+                    msg = "出现未知错误"
+            return msg
+
+        @classmethod
+        def skill(cls, card:list, Player:dict) -> str:
+            '''
+            技能牌生效
+                card:技能牌
+                Player:技能牌生效对象
+            '''
+            suit = card[0]
+            point = card[1]
+            msg = f'技能牌为【{cls.suit[suit]} {cls.point[point]}】\n'
             if suit == 1:
-                Active["ATK"] += point
-                msg = f"♤发动了攻击{point}"
+                Player["DEF"] += point
+                msg += f"♤发动了防御 {point}"
             elif suit == 2:
-                Active["HP"] += point
-                msg = f"♡生命值增加了{point}"
+                Player["HP"] += point
+                msg += f"♡生命值增加了 {point}"
             elif suit == 3:
-                Active["SP"] += point
-                msg = f"♧技能点增加了{point}...\n"
-                roll = random.randint(1,20)
-                if Active["SP"] < roll:
-                    msg += f'二十面骰判定为{roll}点，当前技能点{Active["SP"]}\n技能发动失败...'
-                else:
-                    del Active["hand"][index]
-                    msg += f'二十面骰判定为{roll}点，当前技能点{Active["SP"]}\n技能发动成功！\n'
-                    msg += cls.action_ACE(Active)
+                Player["SP"] += point + point
+                msg += f"♧技能点增加了 {point}"
             elif suit == 4:
-                Active["ATK"] = point
-                msg = f"♢发动了攻击{point}"
+                Player["ATK"] += point
+                msg += f"♢发动了反击 {point}"
             else:
-                msg = "出现未知错误"
-        return msg
-    @classmethod
-    def skill(cls, card:list, Player:dict) -> str:
-        '''
-        技能牌生效
-            card:技能牌
-            Player:技能牌生效对象
-        '''
-        suit = card[0]
-        point = card[1]
-        msg = f'技能牌为【{cls.suit[suit]} {cls.point[point]}】\n'
-        if suit == 1:
-            Player["DEF"] += point
-            msg += f"♤发动了防御 {point}"
-        elif suit == 2:
-            Player["HP"] += point
-            msg += f"♡生命值增加了 {point}"
-        elif suit == 3:
-            Player["SP"] += point + point
-            msg += f"♧技能点增加了 {point}"
-        elif suit == 4:
-            Player["ATK"] += point
-            msg += f"♢发动了反击 {point}"
-        else:
-            msg += "启动结算程序"
-        Player["SP"] -= point
-        Player["SP"] = 0 if Player["SP"] < 0 else Player["SP"]
-        return msg
-
-async def poker_play(bot:Bot, event:GroupMessageEvent, index:str):
-    """
-    出牌
-    """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if session.info["ACT"] == 0:
-        return
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    if index not in ["1","2","3"]:
-        return "请发送【出牌 1/2/3】打出你的手牌。"
-
-    session.info["ACT"] = 0
-    session.nextround()
-
-    deck = session.info["deck"]
-
-    if event.user_id == session.player1_id:
-        Active = session.info["P1"]
-        Passive = session.info["P2"]
-    else:
-        Active = session.info["P2"]
-        Passive = session.info["P1"]  
-        
-    # 出牌判定
-    msg = pokerACT.action(int(index) - 1,Active)
-    try:
-        await bot.send(event,message = msg,at_sender=True)
-    except:
-        await bot.send(event,message = MessageSegment.image(text_to_png(msg,30)))
-
-    await asyncio.sleep(0.03*len(msg))
-
-    # 敌方技能判定
-    next_name = user_data[session.next].group_accounts[group_id].nickname
-    if Passive["SP"] > 0:
-        roll = random.randint(1,20)
-        if  Passive["SP"] < roll:
-            msg = f'{next_name} 二十面骰判定为{roll}点，当前技能点{Passive["SP"]}\n技能发动失败...'
-        else:
-            msg = f'{next_name} 二十面骰判定为{roll}点，当前技能点{Passive["SP"]}\n技能发动成功！\n'
-            msg += pokerACT.skill(deck[0], Passive)
-            del deck[0]
+                msg += "启动结算程序"
+            Player["SP"] -= point
+            Player["SP"] = 0 if Player["SP"] < 0 else Player["SP"]
+            return msg
+
+    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+        """
+        出牌
+        """
+        session = self.session
+        if self.ACT == 0:
+            return
+        if msg := session.shot_check(event):
+            return None if msg == " " else msg
+        if not 1<= (index := args[0]) <= 3:
+            return "请发送【出牌 1/2/3】打出你的手牌。"
+        group_id = session.group_id
 
+        self.ACT = 0
+        session.nextround()
+        deck = self.deck
+        if event.user_id == session.player1_id:
+            Active = self.P1
+            Passive = self.P2
+        else:
+            Active = self.P2
+            Passive = self.P1
+        
+        # 出牌判定
+        msg = self.pokerACT.action(index - 1,Active)
         try:
-            await bot.send(event,message = msg)
+            await bot.send(event,message = msg,at_sender=True)
         except:
-            await bot.send(event,message = MessageSegment.image(text_to_png(msg,30)))
+            try:
+                await bot.send(event,message = MessageSegment.image(text_to_png(msg,30)))
+            except:
+                pass
 
-    # 回合结算
-    Active["HP"] += Active["DEF"] - Active["ATK"] if Active["DEF"] < Passive["ATK"] else 0
-    Passive["HP"] += Passive["DEF"] - Active["ATK"] if Passive["DEF"] < Active["ATK"] else 0
-
-    Active["ATK"] = 0
-    Passive["ATK"] = 0
-
-    # 防御力强化保留一回合
-    Passive["DEF"] = 0 
-
-    # 下回合准备
-    hand = deck[0:3].copy()
-    Passive["hand"] = hand
-    del deck[0:3]
-
-    next_name = "游戏结束" if Active["HP"] < 1 or Passive["HP"] < 1 or Passive["HP"] >= 40 or [0,0] in hand else next_name
-
-    msg = (
-        f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
-        "状态：\n"
-        f'HP {session.info["P1"]["HP"]} SP {session.info["P1"]["SP"]} DEF {session.info["P1"]["DEF"]}\n'
-        "——————————————\n"
-        f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
-        "状态：\n"
-        f'HP {session.info["P2"]["HP"]} SP {session.info["P2"]["SP"]} DEF {session.info["P2"]["DEF"]}\n'
-        "——————————————\n"
-        f'当前回合：{next_name}\n'
-        "手牌：\n" + 
-        "".join([f'【{pokerACT.suit[suit]}{pokerACT.point[point]}】' for suit, point in Passive["hand"]])
-        )
-    await asyncio.sleep(0.5)
-    await bot.send(event, message = MessageSegment.image(text_to_png(msg,30)))
-
-    if next_name == "游戏结束":
-        Passive["HP"] = Passive["HP"] + 100 if Passive["HP"] >= 40 else Passive["HP"]
-        session.win = session.player1_id if session.info["P1"]["HP"] > session.info["P2"]["HP"] else session.player2_id
-        await end(bot, event)
-    else:
-        session.info["ACT"] = 1
+        await asyncio.sleep(0.03*len(msg))
+
+        # 敌方技能判定
+        next_name = user_data[session.next].group_accounts[group_id].nickname
+        if Passive["SP"] > 0:
+            roll = random.randint(1,20)
+            if  Passive["SP"] < roll:
+                msg = f'{next_name} 二十面骰判定为{roll}点，当前技能点{Passive["SP"]}\n技能发动失败...'
+            else:
+                msg = f'{next_name} 二十面骰判定为{roll}点，当前技能点{Passive["SP"]}\n技能发动成功！\n'
+                msg += self.pokerACT.skill(deck[0], Passive)
+                del deck[0]
+
+            try:
+                await bot.send(event,message = msg)
+            except:
+                try:
+                    await bot.send(event,message = MessageSegment.image(text_to_png(msg,30)))
+                except:
+                    pass
+
+        # 回合结算
+        Active["HP"] += Active["DEF"] - Active["ATK"] if Active["DEF"] < Passive["ATK"] else 0
+        Passive["HP"] += Passive["DEF"] - Active["ATK"] if Passive["DEF"] < Active["ATK"] else 0
+
+        Active["ATK"] = 0
+        Passive["ATK"] = 0
+
+        # 防御力强化保留一回合
+        Passive["DEF"] = 0 
+
+        # 下回合准备
+        hand = deck[0:3].copy()
+        Passive["hand"] = hand
+        del deck[0:3]
+
+        next_name = "游戏结束" if Active["HP"] < 1 or Passive["HP"] < 1 or Passive["HP"] >= 40 or [0,0] in hand else next_name
+
+        msg = (
+            f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
+            "状态：\n"
+            f'HP {self.P1["HP"]} SP {self.P1["SP"]} DEF {self.P1["DEF"]}\n'
+            "——————————————\n"
+            f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
+            "状态：\n"
+            f'HP {self.P2["HP"]} SP {self.P2["SP"]} DEF {self.P2["DEF"]}\n'
+            "——————————————\n"
+            f'当前回合：{next_name}\n'
+            "手牌：\n" + 
+            "".join([f'【{self.pokerACT.suit[suit]}{self.pokerACT.point[point]}】' for suit, point in Passive["hand"]])
+            )
+        await asyncio.sleep(0.5)
+        await bot.send(event, message = MessageSegment.image(text_to_png(msg, 50, width_simple = "——————————————")))
+
+        if next_name == "游戏结束":
+            Passive["HP"] = Passive["HP"] + 100 if Passive["HP"] >= 40 else Passive["HP"]
+            session.win = session.player1_id if self.P1["HP"] > self.P2["HP"] else session.player2_id
+            await self.end(bot, event)
+        else:
+            self.ACT = 1
+
+    def game_tips(self, msg):
+        """
+        发起游戏：扑克对战
+        """
+        return ("唰唰~，随机牌堆已生成\n"
+                f'挑战金额：{self.session.gold}'
+                f'{msg}')
+
+    def session_tips(self):
+        tip1 = "本场对决为【扑克对战】\n"
+        tip2 = "出牌！\n"
+        tip2 += MessageSegment.image(text_to_png(
+            "P1初始状态\n"
+            f'HP {self.P1["HP"]} SP {self.P1["SP"]} DEF {self.P1["DEF"]}\n'
+            "——————————————\n"
+            "P2初始状态\n"
+            f'HP {self.P2["HP"]} SP {self.P2["SP"]} DEF {self.P2["DEF"]}\n'
+            "——————————————\n"
+            "P1初始手牌\n" + 
+            "".join([f'【{self.pokerACT.suit[suit]}{self.pokerACT.point[point]}】' for suit, point in self.P1["hand"]])
+            ), 50, width_simple = "——————————————")
+        return self.acceptmessage(tip1, tip2);
 
-"""+++++++++++++++++
-——————————
-      猜数字
-——————————
-+++++++++++++++++"""
-
-def lucky_number_info(gold):
-    """
-    生成猜数字游戏内容
-    """
-    return {
-        "game":"lucky_number",
-        "gold":gold,
-        "number":random.randint(1,100),
-        }
-
-def lucky_number(event:GroupMessageEvent, gold:int):
-    """
-    发起游戏：猜数字
-    """
-    flag, msg = start(event, gold)
-    if flag == False:
-        return msg
-    session = current_games[event.group_id]
-    session.gold = gold
-    session.info = lucky_number_info(gold)
-    return (f"随机 1-100 数字已生成。"
-            f"挑战金额：{gold}/次\n"
-            f"{msg}")
+    def end_tips(self):
+        return "" 
 
-async def guess_number(bot:Bot, event:GroupMessageEvent, N:int):
+class LuckyNumber(Game):
     """
     猜数字
     """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    session.gold = min(session.info["gold"] * session.round, session.info["bet_limit"])
-    session.nextround()
-    TrueN = session.info["number"]
-    if N > TrueN:
-        return f"{N}比这个数字大\n金额：{session.gold}"
-    if N < TrueN:
-        return f"{N}比这个数字小\n金额：{session.gold}"
-    session.win = event.user_id
-    await end(bot, event)
-
-"""+++++++++++++++++
-——————————
-       梭哈
-——————————
-+++++++++++++++++"""
-
-cantrell_suit = {4:"♠",3:"♥",2:"♣",1:"♦"}
-cantrell_point = {1:"2",2:"3",3:"4",4:"5",5:"6",6:"7",7:"8",8:"9",9:"10",10:"J",11:"Q",12:"K",13:"A"}
-
-def is_straight(points):
-    """
-    判断是否为顺子
-    """
-    points = sorted(points)
-    for i in range(1, len(points)):
-        if points[i] - points[i-1] != 1:
-            return False
-    return True
-
-def cantrell_pt(hand:list) -> Tuple[int,str]:
-    """
-    牌型点数
-    """
-    pt = 0
-    name = ""
-
-    suits = [x[0] for x in hand]
-    points = [x[1] for x in hand]
-
-    setpoints = set(points)
-
-    # 判断同花
-    if len(set(suits)) == 1:
-        pt += suits[0]
-        if is_straight(points):
-            point = max(points)
-            pt += point * (100**9)
-            name += f"同花顺 {cantrell_suit[suits[0]]}{cantrell_point[point]} "
-        else:
-            point = sum(points)
-            pt += point * (100**6)
-            name += f"同花 {cantrell_suit[suits[0]]}{point + 5} "
-    else:
-        pt += sum(suits)
-        # 判断顺子
-        if is_straight(points):
-            point = max(points)
-            pt += point * (100**5)
-            name += f"顺子 {cantrell_point[point]} "
+    name = "LuckyNumber"
+    max_bet_gold:int = max_bet_gold
+
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        self.gold:int = gold
+        self.number:int = random.randint(1,100)
+        self.session.gold = gold
+
+    @staticmethod
+    def parse_arg(arg:str):
+        if arg.isdigit():
+            gold = int(arg)
         else:
-            # 判断四条或葫芦
-            if len(setpoints) == 2:
-                for point in setpoints:
-                    if points.count(point) == 4:
-                        pt += point * (100**8)
-                        name += f"四条 {cantrell_point[point]} "
-                    if points.count(point) == 3:
-                        pt += point * (100**7)
-                        name += f"葫芦 {cantrell_point[point]} "
-            else:
-                # 判断三条，两对，一对
-                exp = 1
-                tmp = 0
-                for point in setpoints:
-                    if points.count(point) == 3:
-                        pt += point * (100**4)
-                        name += f"三条 {cantrell_point[point]} "
-                        break
-                    if points.count(point) == 2:
-                        exp += 1
-                        tmp += point
-                        name += f"对{cantrell_point[point]} "
-                else:
-                    pt += tmp * (100**exp)
+            gold = int(bet_gold/10)
+        return {"gold":gold}
 
-            tmp = 0
-            for point in setpoints:
-                if points.count(point) == 1:
-                    pt += point * (100)
-                    tmp += point + 1
-            if tmp:
-                name += f"散{tmp} "
-
-    return pt,name[:-1]
-
-def max_hand(hands) -> Tuple[list,Tuple[int,str]]:
-    """
-    返回一组牌中最大的牌
-    """
-    max_pt = 0
-    for hand in hands:
-        result = cantrell_pt(hand)
-        if result[0] > max_pt:
-            max_pt = result[0]
-            max_name = result[1]
-            max_hand = hand
-    return max_hand,(max_pt,max_name)
-
-def cantrell_info(gold):
-    """
-    生成港式五张游戏内容
-    """
-    deck = random_poker()
-    return {
-        "game":"cantrell",
-        "round_gold":gold,
-        "hand1":deck[0:5],
-        "pt1":cantrell_pt(deck[0:5]),
-        "hand2":deck[5:10],
-        "pt2":cantrell_pt(deck[5:10])
-        }
-
-def happy_cantrell_info(gold, level = 2):
-    """
-    生成快乐港式五张游戏内容
-        level:抽牌次数，1次到5次。
-    """
-    deck = random_poker()
-    deck = [deck[i:i+5] for i in range(0, 50, 5)]
-
-    hand1,pt1 = max_hand(deck[0:level])
-    hand2,pt2 = max_hand(deck[level:2*level])
-
-    return {
-        "game":"cantrell",
-        "round_gold":gold,
-        "hand1":hand1,
-        "pt1":pt1,
-        "hand2":hand2,
-        "pt2":pt2
-        }
-
-def cantrell(event:GroupMessageEvent, gold:int ,level:int = 1):
-    """
-    发起游戏：港式五张
-    """
-    flag, msg = start(event, gold, max_bet_gold * 10)
-    if flag == False:
-        return msg
-    group_id = event.group_id
-    session = current_games[group_id]
-    session.gold = gold
-    if level == 1:
-        session.info = cantrell_info(gold)
-    else:
+    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+        """
+        猜数字
+        """
+        session = self.session
+        if msg := session.shot_check(event):
+            return None if msg == " " else msg
+
+        session.gold += self.gold
+        session.gold = min(session.gold, session.bet_limit)
+        session.nextround()
+
+        N = args[0]
+        TrueN = self.number
+        if N > TrueN:
+            return f"{N}比这个数字大\n金额：{session.gold}"
+        if N < TrueN:
+            return f"{N}比这个数字小\n金额：{session.gold}"
+
+        session.win = event.user_id
+        await self.end(bot, event)
+
+    def game_tips(self, msg):
+        """
+        发起游戏：扑克对战
+        """
+        return (f"随机 1-100 数字已生成。"
+                f"挑战金额：{self.gold}/次\n"
+                f"{msg}")
+
+    def session_tips(self):
+        tip1 = "本场对决为【猜数字】\n"
+        tip2 = "发送数字"
+        return self.acceptmessage(tip1, tip2);
+
+    def end_tips(self):
+        return "" 
+
+class Cantrell(Game):
+    """
+    港式五张
+    """
+    name = "Cantrell"
+    max_bet_gold:int = max_bet_gold *10
+
+    cantrell_suit = {4:"♠",3:"♥",2:"♣",1:"♦"}
+    cantrell_point = {1:"2",2:"3",3:"4",4:"5",5:"6",6:"7",7:"8",8:"9",9:"10",10:"J",11:"Q",12:"K",13:"A"}
+
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        level = kwargs["level"]
         level = 1 if level < 1 else level
         level = 5 if level > 5 else level
-        session.info = happy_cantrell_info(gold,level)
-    return (f"随机牌堆已生成\n"
-            f"开局金额：{gold}\n"
-            + (f"等级：Lv.{level}\n" if level > 1 else "") +
-            f"{msg}")
-
-async def cantrell_check(bot:Bot, event:GroupMessageEvent):
-    """
-    看牌
-    """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    session.time = time.time() + 120
-    expose = int(round((session.round  + 0.5)/ 2)) + 3
-    expose = min(expose,5)
-    if event.user_id == session.player1_id:
-        hand = "hand1"
-    else:
-        hand = "hand2"
-    msg = (
-        "你的手牌：\n"
-        + ("|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info[hand][0:expose]]) + (5 - expose)*"   |")
-        )
-    if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30))):
-        await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
-
-async def cantrell_play(bot:Bot, event:GroupMessageEvent, gold:int, max_bet_gold:int = max_bet_gold * 10):
-    """
-    加注
-    """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    if gold > max_bet_gold:
-        return MessageSegment.at(event.user_id) + f"加注金额不能超过{max_bet_gold}"
-    if session.gold + gold > session.info["bet_limit"]:
-        gold = session.info["bet_limit"] - session.gold
-    expose = session.round / 2
-    if expose == int(expose):
-        session.nextround()
-        session.time += 120
-        expose = int(expose) + 3
-        gold = max(gold,session.info["round_gold"])
-        session.gold += gold
-        msg = (
-            f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
-            "手牌：\n"
-            "|"
-            + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"][0:expose]]) + (5 - expose)*"   |"
-            "\n——————————————\n"
-            f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
-            "手牌：\n"
-            "|"
-            + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"][0:expose]]) + (5 - expose)*"   |"
-            )
-        if expose == 5:
-            if session.info["pt1"][0] > session.info["pt2"][0]:
-                session.win = session.player1_id
+        deck = Poker.random_poker()
+        if level == 1:
+            hand1 = deck[0:5]
+            pt1 = self.cantrell_pt(hand1)
+            hand2 = deck[5:10]
+            pt2 = self.cantrell_pt(hand2)
+        else:
+            deck = [deck[i:i+5] for i in range(0, 50, 5)]
+            hand1, pt1 = self.max_hand(deck[0:level])
+            hand2, pt2 = self.max_hand(deck[level:2*level])
+
+        self.gold:int = gold
+        self.level = level
+        self.hand1:list = hand1
+        self.pt1:Tuple[int,str] = pt1
+        self.hand2:list = hand2
+        self.pt2:Tuple[int,str] = pt2
+        self.session.gold = gold
+
+    @staticmethod
+    def parse_arg(arg:str):
+        gold = bet_gold
+        level = 1
+        if arg:
+            arg = arg.split()
+            if len(arg) == 1:
+                arg = arg[0]
+                if arg.isdigit():
+                    if 0 < (tmp := int(arg)) <= 5:
+                        level = tmp
+                    else:
+                        gold = tmp
             else:
-                session.win = session.player2_id
-            await end(bot, event)
+                if arg[0].isdigit():
+                    if 0 < (tmp := int(arg[0])) <= 5:
+                        level = tmp
+                        if arg[1].isdigit():
+                            gold = int(arg[1])
+                    else:
+                        gold = tmp
+
+        return {"gold":gold,"level":level}
+
+    @staticmethod
+    def is_straight(points):
+        """
+        判断是否为顺子
+        """
+        points = sorted(points)
+        for i in range(1, len(points)):
+            if points[i] - points[i-1] != 1:
+                return False
+        return True
+
+    @staticmethod
+    def cantrell_pt(hand:list) -> Tuple[int,str]:
+        """
+        牌型点数
+        """
+        pt = 0
+        name = ""
+
+        suits = [x[0] for x in hand]
+        points = [x[1] for x in hand]
+
+        setpoints = set(points)
+
+        is_straight = Cantrell.is_straight
+        cantrell_suit = Cantrell.cantrell_suit
+        cantrell_point = Cantrell.cantrell_point
+
+        # 判断同花
+        if len(set(suits)) == 1:
+            pt += suits[0]
+            if is_straight(points):
+                point = max(points)
+                pt += point * (100**9)
+                name += f"同花顺 {cantrell_suit[suits[0]]}{cantrell_point[point]} "
+            else:
+                point = sum(points)
+                pt += point * (100**6)
+                name += f"同花 {cantrell_suit[suits[0]]}{point + 5} "
         else:
-            return MessageSegment.image(text_to_png(f"您已跟注{gold}金币\n" + msg,30))
-    else:
-        session.nextround()
-        session.time += 120
-        session.info["round_gold"] = gold
-        return MessageSegment.at(event.user_id) + f"您已加注{gold}金币"
+            pt += sum(suits)
+            # 判断顺子
+            if is_straight(points):
+                point = max(points)
+                pt += point * (100**5)
+                name += f"顺子 {cantrell_point[point]} "
+            else:
+                # 判断四条或葫芦
+                if len(setpoints) == 2:
+                    for point in setpoints:
+                        if points.count(point) == 4:
+                            pt += point * (100**8)
+                            name += f"四条 {cantrell_point[point]} "
+                        if points.count(point) == 3:
+                            pt += point * (100**7)
+                            name += f"葫芦 {cantrell_point[point]} "
+                else:
+                    # 判断三条，两对，一对
+                    exp = 1
+                    tmp = 0
+                    for point in setpoints:
+                        if points.count(point) == 3:
+                            pt += point * (100**4)
+                            name += f"三条 {cantrell_point[point]} "
+                            break
+                        if points.count(point) == 2:
+                            exp += 1
+                            tmp += point
+                            name += f"对{cantrell_point[point]} "
+                    else:
+                        pt += tmp * (100**exp)
 
-"""+++++++++++++++++
-——————————
-        21点
-——————————
-+++++++++++++++++"""
-
-Blackjack_suit = {4:"♠",3:"♥",2:"♣",1:"♦"}
-Blackjack_point = {1:"A",2:"2",3:"3",4:"4",5:"5",6:"6",7:"7",8:"8",9:"9",10:"10",11:"J",12:"Q",13:"K"}
-
-def Blackjack_info():
-    """
-    生成21点游戏内容
-    """
-    deck = random_poker()
-    return {
-        "game":"Blackjack",
-        "deck":deck[2:],
-        "hand1":[deck[0],],
-        "hand2":[deck[1],],
-        }
-
-def Blackjack(event:GroupMessageEvent, gold:int):
-    """
-    发起游戏：21点
-    """
-    flag, msg = start(event, gold, max_bet_gold * 10)
-    if flag == False:
-        return msg
-    group_id = event.group_id
-    session = current_games[group_id]
-    session.gold = gold
-    session.info = Blackjack_info()
-    return ("唰唰~，随机牌库已生成\n"
-            f"挑战金额：{gold}\n"
-            f"{msg}")
-
-def Blackjack_pt(hand:list) -> int:
-    """
-    返回21点牌组点数。
-    """
-    pts = [x[1] if x[1] < 10 else 10 for x in hand]
-    pt = sum(pts)
-    if 1 in pts and pt <= 11:
-        pt += 10
-    return pt
-
-async def Blackjack_Hit(bot:Bot, event:GroupMessageEvent):
-    """
-    抽牌
-    """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    session.time = time.time()
-
-    if event.user_id == session.player1_id:
-        hand = "hand1"
-        session.win = session.player2_id
-    else:
-        hand = "hand2"
-        session.win = session.player1_id
-    deck = session.info["deck"]
-    card = deck[0]
-    del deck[0]
-    hand = session.info[hand]
-    hand.append(card)
-    pt = Blackjack_pt(hand)
-    if pt > 21:
-        await end(bot, event)
-    else:
+                tmp = 0
+                for point in setpoints:
+                    if points.count(point) == 1:
+                        pt += point * (100)
+                        tmp += point + 1
+                if tmp:
+                    name += f"散{tmp} "
+
+        return pt,name[:-1]
+
+    @staticmethod
+    def max_hand(hands) -> Tuple[list,Tuple[int,str]]:
+        """
+        返回一组牌中最大的牌
+        """
+        max_pt = 0
+        for hand in hands:
+            result = Cantrell.cantrell_pt(hand)
+            if result[0] > max_pt:
+                max_pt = result[0]
+                max_name = result[1]
+                max_hand = hand
+        return max_hand,(max_pt,max_name)
+
+    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+        """
+        看牌|加注
+        """
+        session = self.session
+        if msg := session.shot_check(event):
+            return None if msg == " " else msg
+        if args[0] == 0:
+            return await self.cantrell_check(bot, event)
+        else:
+            return await self.cantrell_play(bot, event, args[1])
+
+    async def cantrell_check(self, bot:Bot, event:GroupMessageEvent):
+        """
+        看牌
+        """
+        session = self.session
+        expose = int(round((session.round  + 0.5)/ 2)) + 3
+        expose = min(expose,5)
+        session.time = time.time() + 120
+        if event.user_id == session.player1_id:
+            hand = self.hand1
+        else:
+            hand = self.hand2
         msg = (
             "你的手牌：\n"
-            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand]))
-            + f'\n合计:{pt}点'
+            + ("|" + "".join([f'{self.cantrell_suit[suit]}{self.cantrell_point[point]}|' for suit, point in hand[0:expose]]) + (5 - expose)*"   |")
             )
-        if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30))):
+        if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg, 50))):
             await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
 
-async def Blackjack_stand(bot:Bot, event:GroupMessageEvent):
+    async def cantrell_play(self, bot:Bot, event:GroupMessageEvent, gold:int):
+        """
+        加注
+        """
+        session = self.session
+        gold = self.gold if gold == None else gold
+        gold = min(gold, session.bet_limit - session.gold)
+        if gold > self.max_bet_gold:
+            return MessageSegment.at(event.user_id) + f"加注金额不能超过{self.max_bet_gold}"
+        expose = session.round / 2
+        session.nextround()
+        session.time += 120
+        if expose == int(expose):
+            gold = max(gold, self.gold)
+            session.gold += gold
+            group_id = session.group_id
+            expose = int(expose) + 3
+            hand1 = self.hand1[0:expose]
+            hand2 = self.hand2[0:expose]
+            cantrell_suit = self.cantrell_suit
+            cantrell_point = self.cantrell_point
+
+            msg = (
+                f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
+                "手牌：\n"
+                f'|{"".join([f"{cantrell_suit[suit]}{cantrell_point[point]}|" for suit, point in hand1])}{(5 - expose)*"   |"}'
+                "\n——————————————\n"
+                f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
+                "手牌：\n"
+                f'|{"".join([f"{cantrell_suit[suit]}{cantrell_point[point]}|" for suit, point in hand2])}{(5 - expose)*"   |"}'
+                )
+
+            if expose == 5:
+                session.win = session.player1_id if self.pt1[0] > self.pt2[0] else session.player2_id
+                await self.end(bot, event)
+            else:
+                return MessageSegment.image(text_to_png(f"您已跟注{gold}金币\n" + msg, 50, width_simple = "——————————————"))
+        else:
+            self.gold = gold
+            return MessageSegment.at(event.user_id) + f"您已加注{gold}金币"
+
+    def game_tips(self, msg):
+        """
+        发起游戏：港式五张
+        """
+        return ("唰唰~，随机牌堆已生成\n"
+                f'开局金额：{self.gold}\n'
+                f'等级：Lv.{self.level}\n'
+                f'{msg}')
+
+    def session_tips(self):
+        tip1 = "本场对决为【港式五张】\n"
+        tip2 = "\n看牌|加注\n"
+        cantrell_suit = self.cantrell_suit
+        cantrell_point = self.cantrell_point
+        tip2 += MessageSegment.image(text_to_png(
+                "P1初始手牌：\n"
+                "|"
+                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand1[0:3]]) +
+                "   |   |"
+                "\n——————————————\n"
+                'P2初始手牌\n'
+                "|"
+                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand2[0:3]]) +
+                "   |   |"
+                ),50)
+        return self.acceptmessage(tip1, tip2);
+
+    def end_tips(self):
+        cantrell_suit = self.cantrell_suit
+        cantrell_point = self.cantrell_point
+        return MessageSegment.image(text_to_png((
+            "P1手牌：\n"
+            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand1]) +
+            f"\n牌型：\n{self.pt1[1]}"
+            "\n——————————————\n"
+            "P2手牌：\n"
+            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in self.hand2]) +
+            f"\n牌型：\n{self.pt2[1]}"),50))
+
+class Blackjack(Game):
     """
-    停牌
+    21点
     """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    session.time = time.time()
-    session.nextround()
-    if session.round == 2:
-        return Message(f"请{MessageSegment.at(session.player2_id)}\n抽牌|停牌|双倍下注")
-    else:
-        hand1 = session.info["hand1"]
-        hand2 = session.info["hand2"]
-        if Blackjack_pt(hand1) > Blackjack_pt(hand2):
-            session.win = session.player1_id
+    name = "Blackjack"
+    max_bet_gold:int = max_bet_gold *5
+
+    Blackjack_suit = {4:"♠",3:"♥",2:"♣",1:"♦"}
+    Blackjack_point = {1:"A",2:"2",3:"3",4:"4",5:"5",6:"6",7:"7",8:"8",9:"9",10:"10",11:"J",12:"Q",13:"K"}
+
+    def __init__(self, **kwargs):
+        super().__init__()
+        gold = kwargs["gold"]
+        deck = Poker.random_poker()
+        self.deck = deck[2:]
+        self.hand1 = [deck[0],]
+        self.hand2 = [deck[1],]
+        self.session.gold = gold
+
+    @staticmethod
+    def Blackjack_pt(hand:list) -> int:
+        """
+        返回21点牌组点数。
+        """
+        pts = [x[1] if x[1] < 10 else 10 for x in hand]
+        pt = sum(pts)
+        if 1 in pts and pt <= 11:
+            pt += 10
+        return pt
+
+    async def action(self, bot:Bot, event:GroupMessageEvent, *args):
+        """
+        抽牌|停牌|双倍下注
+        """
+        session = self.session
+        if msg := session.shot_check(event):
+            return None if msg == " " else msg
+        code = args[0]
+        if code == 0:
+            return await self.Blackjack_Stand(bot, event)
+        elif code == 1:
+            return await self.Blackjack_Hit(bot, event)
         else:
+            return await self.Blackjack_DoubleDown(bot, event)
+
+    async def Blackjack_Hit(self, bot:Bot, event:GroupMessageEvent):
+        """
+        抽牌
+        """
+        session = self.session
+        session.time = time.time()
+
+        if event.user_id == session.player1_id:
+            hand = self.hand1
             session.win = session.player2_id
-        await end(bot, event)
+        else:
+            hand = self.hand2
+            session.win = session.player1_id
+        deck = self.deck
+        card = deck[0]
+        del deck[0]
+        hand.append(card)
+        pt = self.Blackjack_pt(hand)
+        if pt > 21:
+            await self.end(bot, event)
+        else:
+            msg = (
+                "你的手牌：\n"
+                f'|{"".join([f"{self.Blackjack_suit[suit]}{self.Blackjack_point[point]}|" for suit, point in hand])}\n'
+                + f'合计:{pt}点')
+            if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,50))):
+                await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n你的手牌合计:{pt}点\n游戏继续！")
 
-async def Blackjack_DoubleDown(bot:Bot, event:GroupMessageEvent):
-    """
-    双倍下注
-    """
-    group_id = event.group_id
-    global current_games
-    session = current_games[group_id]
-    if msg := session.shot_check(event):
-        return None if msg == " " else msg
-    session.time = time.time()
-    gold = session.gold
-    bet_limit = session.info["bet_limit"]
-    gold = gold*2
-    gold = min(bet_limit, gold)
-    session.gold = gold
-    if event.user_id == session.player1_id:
-        hand = "hand1"
-        session.win = session.player2_id
-    else:
-        hand = "hand2"
-        session.win = session.player1_id
-    deck = session.info["deck"]
-    card = deck[0]
-    del deck[0]
-    hand = session.info[hand]
-    hand.append(card)
-    pt = Blackjack_pt(hand)
-    if pt > 21:
-        await end(bot, event)
-    else:
-        msg = (
-            "你的手牌：\n"
-            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand]))
-            + f'\n合计:{pt}点'
-            )
-        if not await try_send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30))):
-            await bot.send(event,f"私聊发送失败，请检查是否添加{bot_name}为好友。\n游戏继续！")
+    async def Blackjack_Stand(self, bot:Bot, event:GroupMessageEvent):
+        """
+        停牌
+        """
+        session = self.session
         session.nextround()
         if session.round == 2:
             return Message(f"请{MessageSegment.at(session.player2_id)}\n抽牌|停牌|双倍下注")
         else:
-            hand1 = session.info["hand1"]
-            hand2 = session.info["hand2"]
+            hand1 = self.hand1
+            hand2 = self.hand2
+            Blackjack_pt = self.Blackjack_pt
             if Blackjack_pt(hand1) > Blackjack_pt(hand2):
                 session.win = session.player1_id
             else:
                 session.win = session.player2_id
-            await end(bot, event)
+            await self.end(bot, event)
 
-"""+++++++++++++++++
-——————————
-      随机对战
-——————————
-+++++++++++++++++"""
-
-def random_game(event:GroupMessageEvent, gold:int):
-    """
-    发起游戏：随机对战
-    """
-    group_account = Manager.locate_user(event)[1]
-    if group_account.props.get("32002",0) < 1:
-        return f"你未持有持有【{props_library['32002']['name']}】，无法发起随机对战。"
-    flag, msg = start(event, gold)
-    if flag == False:
-        return msg
-    session = current_games[event.group_id]
-    session.gold = gold
-    session.info = {
-        "game":"random",
-        "gold":group_account.gold if gold == -1 else gold
-        }
-    return ("随机对战已生成\n"
-            f"挑战金额：{gold if gold > 0 else '随机'}\n"
-            f"{msg}")
-
-"""+++++++++++++++++
-——————————
-      游戏结束
-——————————
-+++++++++++++++++"""
-
-def settle(group_id:int):
-    """
-    游戏结束结算
-        return:结算界面
-    """
-    global current_games
-    session = current_games[group_id]
-    win = session.win if session.win else session.player1_id if session.next == session.player2_id else session.player2_id
-    lose = session.player1_id if session.player2_id == win else session.player2_id
-    winner = user_data[win]
-    winner_group_account = winner.group_accounts[group_id]
-    loser = user_data[lose]
-    loser_group_account = loser.group_accounts[group_id]
-
-    gold = session.gold
-    if winner_group_account.props.get("42001",0) > 0:
-        fee = 0
-        fee_tip = f"『{props_library['42001']['name']}』免手续费"
-    else:
-        rand = random.randint(0, 5)
-        fee = int(gold * rand / 100)
-        fee_tip = f"手续费：{fee}({rand}%)"
-
-    maxgold = int(max_bet_gold/5)
-
-    if winner_group_account.props.get("52002",0) > 0:
-        extra = int(gold *0.1)
-        if extra < maxgold:
-            extra_tip = f"◆『{props_library['52002']['name']}』\n"
-        else:
-            extra = maxgold
-            extra_tip = f"◆『{props_library['52002']['name']}』最大奖励\n"
-    else:
-        extra_tip = ""
-        extra = 0
+    async def Blackjack_DoubleDown(self, bot:Bot, event:GroupMessageEvent):
+        """
+        双倍下注
+        """
+        session = self.session
+        session.gold += session.gold
+        session.gold = min(session.gold, session.bet_limit)
+        await self.Blackjack_Hit(bot,event)
+        return await self.Blackjack_Stand(bot,event)
 
-    if gold == loser_group_account.gold and loser_group_account.security < 3:
-        loser_group_account.security += 1
-        security = random.randint(security_gold[0], security_gold[1])
-        security_tip1 = "◇『金币补贴』\n"
-        security_tip2 = f"◇已领取补贴：{security}\n"
-    else:
-        security = 0
-        security_tip1 = ""
-        security_tip2 = ""
-
-    if loser_group_account.props.get("52001",0) > 0:
-        off = int(gold * 0.1)
-        if off < maxgold:
-            off_tip = f"◇『{props_library['52001']['name']}』\n"
-        else:
-            off = maxgold
-            off_tip = f"◇『{props_library['52001']['name']}』最大补贴\n"
+    def game_tips(self, msg):
+        """
+        发起游戏：21点
+        """
+        return ("唰唰~，随机牌堆已生成\n"
+                f'挑战金额：{self.session.gold}\n'
+                f'{msg}')
+
+    def session_tips(self):
+        hand1 = self.hand1[0]
+        hand2 = self.hand2[0]
+        Blackjack_suit = self.Blackjack_suit
+        Blackjack_point = self.Blackjack_point
 
-    else:
-        off = 0
-        off_tip = ""
+        tip1 = "本场对决为【21点】\n"
+        tip2 = "\n抽牌|停牌|双倍下注\n"
+        tip2 += f'P1：{Blackjack_suit[hand1[0]]}{Blackjack_point[hand1[1]]}|P2：{Blackjack_suit[hand2[0]]}{Blackjack_point[hand2[1]]}'
+        return self.acceptmessage(tip1, tip2);
 
-    win_gold = gold - fee + extra
-    lose_gold = gold - off
-    winner.win += 1
-    winner.Achieve_win += 1
-    winner.Achieve_lose = 0
-    loser.lose += 1
-    loser.Achieve_lose += 1
-    loser.Achieve_win = 0
-    msg = (
-        f"结算：\n"
-        "——————————————\n" +
-        (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((winner,winner_group_account)))) else "") +
-        extra_tip +
-        f"◆胜者：{winner_group_account.nickname}\n"
-        f"◆结算：{winner_group_account.gold}（+{win_gold}）\n"
-        f"◆战绩：{winner.win}:{winner.lose}\n"
-        f"◆胜率：{round(winner.win * 100 / (winner.win + winner.lose), 2) if winner.win > 0 else 0}%\n"
-        "——————————————\n" +
-        (tmp + "\n" if (tmp := "\n".join(x for x in Manager.Achieve_list((loser,loser_group_account)))) else "") +
-        security_tip1 +
-        off_tip +
-        f"◇败者：{loser_group_account.nickname}\n"
-        f"◇结算：{loser_group_account.gold}（-{lose_gold}）\n" +
-        security_tip2 +
-        f"◇战绩：{loser.win}:{loser.lose}\n"
-        f"◇胜率：{round(loser.win * 100 / (loser.win + loser.lose), 2) if loser.win > 0 else 0}%\n"
-        "——————————————\n" + 
-        fee_tip
-        )
-    winner.gold += win_gold
-    winner_group_account.gold += win_gold
-    loser.gold -= lose_gold - security
-    loser_group_account.gold -= lose_gold - security
-    res = game_str(session)
-    del current_games[group_id]
-    return f"这场对决是 {winner_group_account.nickname} 胜利了", msg, res
-
-def game_str(session:Session):
-    """
-    结束附件
-    """
-    game = session.info["game"]
-    if game == "russian":
-        return " ".join(("—" if x == 0 else "|") for x in session.info["bullet"])
-    if game == "dice":
-        return (
-            f'玩家 1\n'
-            f'组合：{" ".join(str(x) for x in session.info["dice_array1"])}\n'
-            f'玩家 2\n'
-            f'组合：{" ".join(str(x) for x in session.info["dice_array2"])}')
-    if game == "cantrell":
+    def end_tips(self):
+        hand1 = self.hand1
+        hand2 = self.hand2
+        Blackjack_suit = self.Blackjack_suit
+        Blackjack_point = self.Blackjack_point
+        Blackjack_pt = self.Blackjack_pt
         return MessageSegment.image(text_to_png((
             "P1手牌：\n"
-            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"]]) +
-            f"\n牌型：\n{session.info['pt1'][1]}"
+            f'|{"".join([f"{Blackjack_suit[suit]}{Blackjack_point[point]}|" for suit, point in hand1])}\n'
+            + f'合计:{Blackjack_pt(hand1)}点'
             "\n——————————————\n"
             "P2手牌：\n"
-            "|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"]]) +
-            f"\n牌型：\n{session.info['pt2'][1]}"),30))
-    if game == "Blackjack":
-        hand1 = session.info["hand1"]
-        hand2 = session.info["hand2"]
-        return MessageSegment.image(text_to_png((
-            "P1手牌：\n"
-            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand1]))
-            + f'\n合计:{Blackjack_pt(hand1)}点'
-            "\n——————————————\n"
-            "P2手牌：\n"
-            + ("|" + "".join([f'{Blackjack_suit[suit]}{Blackjack_point[point]}|' for suit, point in hand2]))
-            + f'\n合计:{Blackjack_pt(hand2)}点'),30))
+            f'|{"".join([f"{Blackjack_suit[suit]}{Blackjack_point[point]}|" for suit, point in hand2])}\n'
+            f'合计:{Blackjack_pt(hand2)}点'),50))
+
+class AROF():
+    """
+    其他类
+    """
+    def accept(self, event:GroupMessageEvent):
+        """
+        接受挑战
+        """
+        return None
+
+    def refuse(self, event:GroupMessageEvent):
+        """
+        拒绝挑战
+        """
+        return None
+
+    async def overtime(self, bot:Bot, event:GroupMessageEvent):
+        """
+        超时结算
+        """
+        return None
+
+    async def fold(self, bot:Bot, event:GroupMessageEvent):
+        """
+        认输
+        """
+        return None
+
+class HorseRace(AROF):
+    """
+    赛马小游戏
+    """
+    name:str = "HorseRace"
+
+    events_list = load_dlcs()
+
+    def __init__(self, event:GroupMessageEvent, gold:int ):
+        self.session = Session(
+            time = time.time() + 180,
+            player1_id = event.user_id,
+            at = -1,
+            gold = gold,
+            )
+        self.race_group = race_group()
+
+    def create_check(self):
+        session = self.session
+        race:race_group = self.race_group
+        overtime = time.time() - session.time + 180
+        if race.start == 0:
+            if overtime < 120:
+                return "一场赛马正在报名中"
+        else:
+            return f"一场赛马正在进行中，遇到问题可以{f'在{t}秒后' if (t := int(180 - overtime)) > 0 else ''}输入【赛马重置】重置游戏"
+
+        return None
+
+    @classmethod
+    def RaceNew(cls, event:GroupMessageEvent, gold:int):
+        """
+        赛马创建
+        """
+        game = current_games.get(event.group_id)
+        if game:
+            if game.name == cls.name and (msg := game.create_check()):
+                return msg
+            if msg := game.session.create_check(event):
+                return msg
+        current_games[event.group_id] =  cls(event, gold)
+        return ("\n"
+                 "> 创建赛马比赛成功！\n"
+                 "> 输入 【赛马加入 名字】 即可加入赛马。")
+
+    def RaceJoin(self, event:GroupMessageEvent, horsename:str):
+        """
+        赛马加入
+        """
+        if self.name != "HorseRace":
+            return "其他对战进行中。"
+        user,group_account = Manager.locate_user(event)
+        user_id = user.user_id
+        session = self.session
+        if (gold := group_account.gold) < session.gold:
+            return f"报名赛马需要{self.session.gold}金币，你的金币：{gold}。"
+        race:race_group = self.race_group
+        if race.start != 0:
+            return
+        if (query_of_player := race.query_of_player()) >= max_player:
+            return "加入失败！赛马场就那么大，满了满了！"
+        if race.is_player_in(user_id) == True:
+            return "加入失败！您已经加入了赛马场!"
+        if not horsename:
+            return "请输入你的马儿名字"
+        horsename = horsename[:2]+"酱" if len(horsename) > 5 else horsename
+        race.add_player(horsename, user_id, group_account.nickname)
+        user.gold -= session.gold
+        group_account.gold -= session.gold
+        return  ("\n"
+                 "> 加入赛马成功\n"
+                 "> 赌上马儿性命的一战即将开始!\n"
+                 f"> 赛马场位置:{query_of_player + 1}/{max_player}")
+
+    async def RaceStart(self, bot:Bot, event:GroupMessageEvent):
+        """
+        赛马开始
+        """
+        events_list = self.events_list
+        race:race_group = self.race_group
+        if (player_count := race.query_of_player()) == 0:
+            return
+        if race.start == 1:
+            return
+        if race.start == 0 or race.start == 2:
+            if player_count >= min_player:
+                race.start = 1
+            else:
+                return f"开始失败！赛马开局需要最少{min_player}人参与"
+
+        group_id = event.group_id
+        session = self.session
+        session.time = time.time() + 180
+        await bot.send(event,(f'> 比赛开始\n'
+                              f'> 当前奖金：{session.gold * player_count}金币'))
+        await asyncio.sleep(0.5)
+
+        while race.start == 1:
+            # 回合数+1
+            race.round_add()
+            #移除超时buff
+            race.del_buff_overtime()
+            #马儿全名计算
+            race.fullname()
+            #回合事件计算
+            text = race.event_start(events_list)
+            #马儿移动
+            race.move()
+            #场地显示
+            display = race.display()
+        
+            output = text_to_png(display,30)
+
+            try:
+                await bot.send(event,(Message(text) + MessageSegment.image(output)))
+            except:
+                text = ""
+                try:
+                    await bot.send(event,(MessageSegment.image(output)))
+                except:
+                    pass
+
+            await asyncio.sleep(0.5 + int(0.06 * len(text)))
+            
+            #全员失败计算
+            if race.is_die_all():
+                for x in race.player:
+                    uid = x.playeruid
+                    if uid in user_data:
+                        user = user_data[uid]
+                        user.gold += session.gold
+                        user.group_accounts[group_id].gold += session.gold
+
+                del current_games[group_id]
+                return "比赛已结束，鉴定为无马生还"
+
+            #全员胜利计算
+            winer = race.is_win_all()
+            winer_list="\n"
+            if winer != []:
+                await bot.send(event,(f'> 比赛结束\n'
+                                      f'> {bot_name}正在为您生成战报...'))
+                await asyncio.sleep(1)
+                gold = int(session.gold * player_count / len(winer))
+                for x in winer:
+                    uid = x[1]
+                    winer_list += "> "+ x[0] + "\n"
+                    if uid in user_data:
+                        user = user_data[uid]
+                        user.gold += gold
+                        user.group_accounts[group_id].gold += gold
+                del current_games[group_id]
+                return (f"> 比赛已结束，胜者为：{winer_list}"
+                        f"> 本次奖金：{gold} 金币")
+            await asyncio.sleep(1)
+
+    def RaceReStart(self, event:GroupMessageEvent):
+        """
+        赛马重置
+        """
+        group_id = event.group_id
+        session = self.session
+        overtime = time.time() - session.time + 180
+        if overtime < 180:
+            return f"当前赛马已创建 {int(overtime)} 秒，未超时。"
+        race:race_group = self.race_group
+        for x in race.player:
+            uid = x.playeruid
+            if uid in user_data:
+                user = user_data[uid]
+                user.gold += session.gold
+                user.group_accounts[group_id].gold += session.gold
+
+        del current_games[group_id]
+        return "赛马场已重置。"
+
+def slot(event:MessageEvent, gold:int):
+    """
+    幸运花色
+    """
+    user,group_account = Manager.locate_user(event)
+    if not group_account:
+        return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+    if gold > max_bet_gold:
+        return f'幸运花色每次最多{max_bet_gold}金币。'
+    if gold > group_account.gold:
+        return f'你没有足够的金币，你的金币：{user_data["group_account.gold:"]}。'
+    suit = {1:"♤",2:"♡",3:"♧",4:"♢"}
+    x = random.randint(1,4)
+    y = random.randint(1,4)
+    z = random.randint(1,4)
+    res = f"\n| {suit[x]} | {suit[y]} | {suit[z]} |\n"
+    l = len(set([x,y,z]))
+    if l == 1:
+        gold = gold * 7
+        msg =("你抽到的花色为：" +
+              res +
+              f"恭喜你获得了{gold}金币，祝你好运~")
+    elif l == 2:
+        gold = 0
+        msg =("你抽到的花色为：" +
+              res +
+              "祝你好运~")
     else:
-        return ""
+        gold = -gold
+        msg =("你抽到的花色为：" +
+              res +
+              f"你失去了{-gold}金币 ，祝你好运~")
+    user.gold += gold
+    group_account.gold += gold
+    return msg
 
-async def end(bot:Bot, event:GroupMessageEvent):
+def random_game(event:GroupMessageEvent, gold:int):
     """
-    输出结算界面
+    发起游戏：随机对战
     """
-    end_info = settle(event.group_id)
-    tmp = MessageSegment.image(text_to_png(end_info[1]))
-    await bot.send(event,end_info[0])
-    await bot.send(event,tmp)
-    await asyncio.sleep(0.5)
-    await bot.send(event,end_info[2])
+    group_account = Manager.locate_user(event)[1]
+    if group_account.props.get("32002",0) < 1:
+        return f"你未持有持有【{props_library['32002']['name']}】，无法发起随机对战。"
+
+    cls = random.choice([Russian,Dice,Poker,LuckyNumber,Cantrell,Blackjack])
+    return cls.creat(event, gold = gold)
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿from pathlib import Path
 from nonebot.log import logger
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
-from ..data.data import resourcefile
+from ..data import resourcefile
 
 
 def load_dlcs():
     events_list = []
     files = Path(resourcefile / "horserace").iterdir()
     for x in files:
         log = f"加载事件文件：{x.name}......"
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     MessageSegment,
     )
 from collections import Counter
 
 from .utils.utils import image_url
 from .utils.chart import text_to_png, gini_coef, default_BG
 from .utils.avatar import download_url
-from .data.data import DataBase, UserDict, GroupAccount, GroupDict
-from .data.data import props_library
+from .data import DataBase, UserDict, GroupAccount, GroupDict
+from .data import props_library
 from .config import revolt_gold, max_bet_gold, lucky_clover, path, BG_image
 
 # 加载数据
 
 datafile = path / "russian_data.json"
 
 if datafile.exists():
@@ -122,49 +122,56 @@
                 f.write(bytes_image)
             return "图片下载成功"
 
 async def del_BG_image(event:MessageEvent):
     Path.unlink(BG_image / f"{str(event.user_id)}.png", True)
     return "背景图片删除成功！"
 
-def Achieve_list(locate:Tuple[UserDict,GroupAccount]):
+def PropsCard_list(locate:Tuple[UserDict,GroupAccount]):
     """
-    成就列表
+    道具列表
     """
     user,group_account = locate
     rank = []
     count = group_account.props.get("02101",0)
     if count > 0:
         if count <= 4:
-            rank.append(f"{count*'☆'}  路灯挂件  {count*'☆'}")
+            rank.append(f"{count*'☆'} 路灯挂件 {count*'☆'}")
         else:
             rank.append(f"☆☆☆☆☆路灯挂件☆☆☆☆☆")
 
     count = group_account.props.get("32001",0)   # 四叶草标记
     if count > 0:
         rank.append(lucky_clover)
+    return rank
 
+def Achieve_list(locate:Tuple[UserDict,GroupAccount]):
+    """
+    成就列表
+    """
+    user,group_account = locate
+    rank = []
     count = group_account.gold
     if count > max_bet_gold:
         count = int(count/max_bet_gold)
         count = str(count) if count < 1000 else "MAX"
         level =f"Lv.{count}"
-        rank.append(f"◆◇ 金库 {level}")
+        rank.append(f"◆ 金库 {level}")
 
     count = user.Achieve_win
     if count >1:
         count = str(count) if count < 1000 else "MAX"
         level =f"Lv.{count}"
-        rank.append(f"◆◇ 连胜 {level}")
+        rank.append(f"◆ 连胜 {level}")
 
     count = user.Achieve_lose
     if count >1:
         count = str(count) if count < 1000 else "MAX"
         level =f"Lv.{count}"
-        rank.append(f"◆◇ 连败 {level}")
+        rank.append(f"◇ 连败 {level}")
 
     return rank
 
 def group_wealths(group_id:int) -> float:
     """
     群内总资产
     """
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Market.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from turtle import width
 from typing import Tuple
 from PIL import Image
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     GroupMessageEvent,
     MessageSegment
@@ -13,17 +14,17 @@
 import asyncio
 
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 
-from .utils.chart import bbcode_to_PIL, group_info_head, info_Splicing
-from .data.data import GroupAccount, Company, ExchangeInfo
-from .data.data import OHLC, props_library
+from .utils.chart import linecard, group_info_head, info_Splicing
+from .data import GroupAccount, Company, ExchangeInfo
+from .data import OHLC, props_library
 from .config import bot_name, revolt_gini, max_bet_gold, path
 
 from .Manager import data, company_index
 from .Manager import BG_path, update_company_index
 
 from . import Manager
 
@@ -417,34 +418,29 @@
     if member_count == 0:
         member_count = 3000
     else:
         member_count = member_count - 1
 
     info.append(await group_info_head(group_name, company_name, group_id, (len(group.namelist),member_count)))
 
-    linestr = "[color=gray][size=15][font=simsun.ttc]────────────────────────────────────────────────────────[/font][/size][/color]\n"
-
     msg = ""
     ranklist = list(group.Achieve_revolution.items())
     ranklist.sort(key=lambda x:x[1],reverse=True)
     for x in ranklist[:10]:
-        msg += f"{user_data[x[0]].group_accounts[group_id].nickname}[align=right]{x[1]}次[/align]\n"
+        msg += f"{user_data[x[0]].group_accounts[group_id].nickname}[nowrap]\n[right]{x[1]}次\n"
     if msg:
-        info.append(bbcode_to_PIL("[align=center]路灯挂件[/align]" + linestr + msg[:-1], 60))
+        info.append(linecard(msg, width = 880, endline = "路灯挂件"))
 
     # 加载公司信息
     if company_name:
         msg = (
             f"公司等级 {company.level}\n"
             f"成立时间 {datetime.datetime.fromtimestamp(company.time).strftime('%Y 年 %m 月 %d 日')}\n"
             )
-
-        info.append(bbcode_to_PIL(msg + linestr + "[align=right][size=30][color=gray]注册信息[/color][/size][/align]", 60))
-
-        info.append(bbcode_to_PIL(stock_profile(company) + linestr + "[align=right][size=30][color=gray]产业信息[/color][/size][/align]", 60))
+        info.append(linecard(msg + stock_profile(company), width = 880, endline = "注册信息"))
 
         p = OHLC(path, group_id)
 
         overtime = time.time() + 30
         while (returncode := p.poll()) == None:
             if time.time() > overtime:
                 returncode = 1
@@ -454,21 +450,20 @@
         if returncode == 0:
             info.append(Image.open(path / "candlestick" / f"{group_id}.png"))
 
         ranklist = list(company.exchange.items())
         ranklist.sort(key=lambda x:x[1].quote)
         msg = ""
         for x in ranklist[:10]:
-            msg += f"{user_data[x[0]].nickname}[align=right]单价 {x[1].quote} 数量 {x[1].n}[/align]\n"
+            msg += f"{user_data[x[0]].nickname}\n[pixel][20]单价 {x[1].quote}[nowrap]\n[pixel][400]数量 {x[1].n}\n"
         if msg:
-            info.append(bbcode_to_PIL(msg + linestr + "[align=right][size=30][color=gray]市场详情[/color][/size][/align]", 40))
-
+            info.append(linecard(msg, width = 880, font_size = 40,endline = "市场详情"))
         msg = company.intro
         if msg:
-            info.append(bbcode_to_PIL(msg + "\n" +linestr + "[align=right][size=30][color=gray]公司介绍[/color][/size][/align]", 40))
+            info.append(linecard(msg + '\n', width = 880, font_size = 40,endline = "公司介绍"))
 
     return MessageSegment.image(info_Splicing(info, BG_path(event.user_id)))
 
 def stock_profile(company:Company) -> str:
     """
     产业信息
     """
@@ -493,20 +488,19 @@
     companys = []
     for company_id in company_ids:
         company = group_data[company_id].company
         companys.append(company)
     companys.sort(key = lambda x:x.group_gold, reverse = True)
 
     lst = [companys[i:i+5] for i in range(0, len(companys), 5)]
-    linestr = "[color=gray][size=15][font=simsun.ttc]────────────────────────────────────────────────────────[/font][/size][/color]\n"
     msg = []
     for seg in lst:
         info = []
         for company in seg:
-            info.append(bbcode_to_PIL(company.company_name +"\n" + linestr + stock_profile(company), 60))
+            info.append(linecard(company.company_name +"\n" + "----\n" + stock_profile(company)[:-1],width = 880))
         msg.append({"type":"node",
                     "data":{
                         "name":f"{bot_name}",
                         "uin":str(event.self_id),
                         "content":MessageSegment.image(info_Splicing(info, BG_path(event.user_id)))}})
     return msg
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,29 +24,30 @@
 
 import random
 import time
 import datetime
 import re
 import shutil
 
-from .utils.utils import get_message_at, number
-from .data.data import ExchangeInfo
-from .config import revolt_cd, bet_gold, path, backup
-from .Manager import data, company_index
-
 from . import Manager
 from . import Account
 from . import Market
 from . import Game
 from . import Prop
 
+from .utils.utils import get_message_at, number
+from .data import ExchangeInfo
+from .config import revolt_cd, bet_gold, path, backup
+from .Manager import data, company_index
+from .Game import current_games
+
 
 try:
     from nonebot.plugin import PluginMetadata
-    from .data.data import menu_data
+    from .data import menu_data
     __plugin_meta__ = PluginMetadata(
         name = "小游戏合集",
         description = "各种群内小游戏",
         usage = "",
         extra = {
             'menu_data':menu_data,
             'menu_template':'default'
@@ -64,76 +65,94 @@
 @RaceNew.handle()
 async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
     gold = arg.extract_plain_text().strip()
     if gold.isdigit():
         gold = int(gold)
     else:
         gold = bet_gold
-    msg =  Game.RaceNew(event, gold)
-    await sign.finish(msg, at_sender = True)
+    msg =  Game.HorseRace.RaceNew(event, gold)
+    await RaceNew.finish(msg, at_sender = True)
 
 # 赛马加入
-RaceJoin = on_command("赛马加入", aliases = {"加入赛马"}, permission = GROUP, priority = 20, block = True)
+RaceJoin = on_command(
+    "赛马加入",
+    aliases = {"加入赛马"},
+    permission = GROUP,
+    priority = 20,
+    block = True
+    )
 
 @RaceJoin.handle()
 async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    msg =  Game.RaceJoin(event, arg.extract_plain_text().strip())
+    if not (game := current_games.get(event.group_id)):
+        msg = "赛马活动未开始，请输入【赛马创建】创建赛马场"
+    elif game.name == "HorseRace":
+        msg =  game.RaceJoin(event, arg.extract_plain_text().strip())
     await RaceJoin.finish(msg, at_sender = True)
 
 # 赛马开始
-RaceStart = on_command("赛马开始", aliases = {"开始赛马"}, permission = GROUP, priority = 20, block = True)
+RaceStart = on_command(
+    "赛马开始",
+    aliases = {"开始赛马"},
+    permission = GROUP,
+    priority = 20,
+    block = True
+    )
 @RaceStart.handle()
 async def _(bot:Bot, event:GroupMessageEvent):
-    msg = await Game.RaceStart(bot, event)
+    if not (game := current_games.get(event.group_id)):
+        msg = "赛马活动未开始，请输入【赛马创建】创建赛马场"
+    elif game.name == "HorseRace":
+        msg = await game.RaceStart(bot, event)
     await RaceStart.finish(msg)
 
 # 赛马重置
 RaceReStart = on_command(
     "赛马重置",
     aliases = {"重置赛马"},
-    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "horse race",
     permission = GROUP,
     priority = 20,
     block = True
     )
 
 @RaceReStart.handle()
 
 async def _(event:GroupMessageEvent):
-    msg =  Game.RaceReStart(event)
+    if not (game := current_games.get(event.group_id)):
+        msg = "赛马活动未开始，请输入【赛马创建】创建赛马场"
+    elif game.name == "HorseRace":
+        msg = game.RaceReStart(event)
     await RaceReStart.finish(msg)
 
 # 赛马暂停
 RaceStop = on_command(
     "赛马暂停",
     aliases = {"暂停赛马"},
-    rule = lambda event:isinstance(event,GroupMessageEvent) and event.group_id in current_games and current_games[event.group_id].info.get("game") == "horse race",
+    rule = lambda event:isinstance(event,GroupMessageEvent) and event.group_id in current_games and current_games[event.group_id].name == "HorseRace",
     permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority = 20,
     block = True
     )
 
 @RaceStop.handle()
 async def _(event:GroupMessageEvent):
-    global current_games
-    current_games[event.group_id].info["race_group"].start = 2
+    current_games[event.group_id].race_group.start = 2
 
 # GameClear
 GameClear = on_command(
     "GameClear",
     aliases = {"清除游戏", "清除对局", "清除对决", "清除对战"},
     rule = lambda event:isinstance(event,GroupMessageEvent) and event.group_id in current_games,
     permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority = 20,
     block = True
     )
 
 @GameClear.handle()
 async def _(event:GroupMessageEvent):
-    global current_games
     del current_games[event.group_id]
 
 # 获取金币
 gold_create = on_command("获取金币", permission = SUPERUSER, priority = 20, block = True)
 
 @gold_create.handle()
 async def _(event:MessageEvent, arg:Message = CommandArg()):
@@ -237,307 +256,168 @@
 
     target = await Manager.locate_user_at(bot, event, int(at))
     msg = Account.transfer_props(event, target, prop_name, count)
     await give_props.finish(msg, at_sender = True)
 
 from .Game import current_games
 
-# 俄罗斯轮盘
-russian = on_command("俄罗斯轮盘", aliases={"装弹", "俄罗斯转盘"}, permission = GROUP, priority = 20, block = True)
-
-@russian.handle()
-async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
-    if not (msg := arg.extract_plain_text().strip().split()):
-        bullet_num = 1
-        gold = bet_gold
-    else:
-        if len(msg) == 1:
-            msg = msg[0]
-            if not msg.isdigit():
-                return
-            if 0 < (msg := int(msg)) < 7:
-                bullet_num = msg
-                gold = bet_gold
-            else:
-                bullet_num = 1
-                gold = int(msg)
-        else:
-            if not (msg[0].isdigit() and msg[1].isdigit()):
-                return
-            bullet_num = int(msg[0])
-            gold = int(msg[1])
-            if 0 < bullet_num < 7:
-                pass
-            elif 0 < gold < 7:
-                bullet_num ,gold = gold, bullet_num
-            else:
-                return
-    msg = Game.russian(event,bullet_num,gold)
-    await russian.finish(msg)
-
-# 开枪
-russian_shot = on_command(
-    "开枪",
-    aliases = {"咔", "嘭", "嘣"},
-    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "russian",
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
-
-@russian_shot.handle()
-async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
-    count = arg.extract_plain_text().strip()
-    if count.isdigit():
-        count = int(count)
-    else:
-        count = 1
-    msg = await Game.russian_shot(bot, event, count)
-    await russian_shot.finish(msg)
-
-# 掷色子
-dice = on_command("掷色子", aliases={"摇色子", "掷骰子", "摇骰子"}, permission = GROUP, priority = 20, block = True)
-
-@dice.handle()
-async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
-    else:
-        gold = bet_gold
-    msg = Game.dice(event, gold)
-    await dice.finish(msg)
-
-# 开数
-dice_open = on_command(
-    "取出",
-    aliases={"开数", "开点"},
-    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "dice",
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
-@dice_open.handle() 
-async def _(bot:Bot, event:GroupMessageEvent):
-    msg = await Game.dice_open(bot, event)
-    await dice_open.finish(msg)
-
-# 扑克对战
-poker = on_command("扑克对战",aliases={"扑克对决", "扑克决斗"}, permission = GROUP, priority = 20, block = True)
-
-@poker.handle()
-async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
-    else:
-        gold = bet_gold
-    msg = Game.poker(event, gold)
-    await poker.finish(msg)
-
-# 出牌
-poker_play = on_command(
-    "出牌",
-    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "poker",
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
-
-@poker_play.handle()
-async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
-    msg = await Game.poker_play(bot, event, arg.extract_plain_text())
-    await poker_play.finish(msg)
-
-# 猜数字
-lucky_number = on_command("猜数字", permission = GROUP, priority = 20, block = True)
-
-@lucky_number.handle()
-async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
-    else:
-        gold = int(bet_gold/10)
-    msg = Game.lucky_number(event, gold)
-    await lucky_number.finish(msg)
-
-# 报数
-guess_number = on_regex(
-    r"^\d{1,3}$",
-    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "lucky_number",
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
-
-@guess_number.handle()
-async def _(bot:Bot, event:GroupMessageEvent):
-    msg = await Game.guess_number(bot, event, int(event.get_plaintext()))
-    await guess_number.finish(msg)
-
-# 港式五张
-cantrell = on_command("同花顺", aliases = {"五张牌","港式五张","梭哈"}, permission = GROUP, priority = 20, block = True)
-
-@cantrell.handle()
-async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
-    arg = arg.extract_plain_text().strip().split()
-    if not arg:
-        gold = bet_gold
-        level = 1
-    else:
-        test = len(arg)
-        if test == 1:
-            gold = arg[0]
-            if gold.isdigit():
-                gold = int(gold)
-            else:
-                gold = bet_gold
-            level = 1
-        else:
-            gold = arg[0]
-            if gold.isdigit():
-                gold = int(gold)
-            else:
-                gold = bet_gold
-            level = arg[1]
-            if level.isdigit():
-                level = int(level)
-            else:
-                level = 1
-
-    msg = Game.cantrell(event, gold, level)
-    await cantrell.finish(msg)
-
-# 看牌
-cantrell_check = on_command(
-    "看牌",
-    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "cantrell",
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
+# 创建游戏
 
-@cantrell_check.handle()
-async def _(bot:Bot, event:GroupMessageEvent):
-    msg = await Game.cantrell_check(bot, event)
-    await cantrell_check.finish(msg)
+AllCreateGameCommand = {
+    "Russian":{"俄罗斯轮盘","装弹"},
+    "Dice":{"掷色子", "摇色子", "掷骰子", "摇骰子"},
+    "Poker":{"扑克对战", "扑克对决", "扑克决斗"},
+    "LuckyNumber":{"猜数字"},
+    "Cantrell":{"同花顺","港式五张","梭哈"},
+    "Blackjack":{"21点"},
+    }
 
-# 加注
-cantrell_play = on_command(
-    "加注",
-    aliases = {"跟注","开牌"},
-    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "cantrell",
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
+AllCreateGameCommand = {cmd: name for name, cmds in AllCreateGameCommand.items() for cmd in cmds}
 
-@cantrell_play.handle()
-async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
+def create_game_rule(event:GroupMessageEvent, state:T_State)-> bool:
+    """
+    规则：创建对局
+    """
+    msg = str(event.message)
+    AllGames = {
+        "Russian":Game.Russian,
+        "Dice":Game.Dice,
+        "Poker":Game.Poker,
+        "LuckyNumber":Game.LuckyNumber,
+        "Cantrell":Game.Cantrell,
+        "Blackjack":Game.Blackjack,
+        }
+    for cmd in AllCreateGameCommand:
+        if msg.startswith(cmd):
+            state["Game"] = AllGames[AllCreateGameCommand[cmd]]
+            state["arg"] = msg[len(cmd):].strip()
+            return True
     else:
-        gold =  current_games[event.group_id].info["round_gold"]
-    msg = await Game.cantrell_play(bot, event, gold)
-    await cantrell_play.finish(msg)
-
-# 21点
-Blackjack = on_command("21点", permission = GROUP, priority = 20, block = True)
+        return False
 
-@Blackjack.handle()
-async def _(event:MessageEvent, arg:Message = CommandArg()):
-    gold = arg.extract_plain_text().strip()
-    if gold.isdigit():
-        gold = int(gold)
-    else:
-        gold = bet_gold
-    msg = Game.Blackjack(event, gold)
-    await Blackjack.finish(msg)
+create_game = on_message(rule = create_game_rule, permission = GROUP, priority = 20, block = True)
 
-# 抽牌
+@create_game.handle()
+async def _(event:GroupMessageEvent, state:T_State):
+    game = state["Game"]
+    kwargs = game.parse_arg(state["arg"])
+    msg = game.creat(event,**kwargs)
+    await create_game.finish(msg)
+
+# 进行游戏
+
+AllPlayGameCommand = {
+    "Russian":{"开枪","咔", "嘭", "嘣"},
+    "Dice":{"取出","开数", "开点"},
+    "Poker":{"出牌"},
+    "LuckyNumber":{"^\d{1,3}$"},
+    "Cantrell":{"看牌","加注","跟注","开牌"},
+    "Blackjack":{"停牌","抽牌","双倍下注"},
+    }
 
-def is_Blackjack(event:GroupMessageEvent,state:T_State) -> bool:
-    if event.group_id in current_games and current_games[event.group_id].info.get("game") == "Blackjack":
-        command = str(event.message)
-        if command == "抽牌":
-            state["Blackjack_play"] = Game.Blackjack_Hit
-        elif command == "停牌":
-            state["Blackjack_play"] = Game.Blackjack_stand
-        elif command == "双倍下注":
-            state["Blackjack_play"] = Game.Blackjack_DoubleDown
+def game_play_rule(event:GroupMessageEvent, state:T_State)-> bool:
+    """
+    规则：游戏进行
+    """
+    group_id = event.group_id
+    game = current_games.get(group_id)
+    if game and (Name := game.name) not in ["HorseRace"]:
+        msg = str(event.message)
+        state["game"] = game
+        if Name == "LuckyNumber":
+            if msg.isdigit() and 0 < (N := int(msg)) <= 100:
+                state["arg"] = [N]
+                return True
         else:
-            return False
-        return True
-    else:
-        return False
-
-Blackjack_play = on_message(
-    rule = is_Blackjack,
-    permission = GROUP,
-    priority = 20,
-    block = True
-    )
-
-@Blackjack_play.handle()
-async def _(bot:Bot, event:GroupMessageEvent,state:T_State):
-    Blackjack_play = state["Blackjack_play"]
-    msg = await Blackjack_play(bot, event)
-    await cantrell_play.finish(msg)
+            cmdlst = AllPlayGameCommand.get(Name)
+            for cmd in cmdlst:
+                if msg.startswith(cmd):
+                    msg = msg[len(cmd):].strip()
+                    if Name == "Cantrell":
+                        if msg.isdigit():
+                            gold = int(msg)
+                        else:
+                            gold = None
+                        state["arg"] = [{"看牌":0,"加注":1,"跟注":1,"开牌":1}[cmd], gold]
+                    elif Name == "Blackjack":
+                        state["arg"] = [{"停牌":0,"抽牌":1,"双倍下注":2}[cmd]]
+                    elif msg.isdigit():
+                        state["arg"] = [int(msg)]
+                    else:
+                        state["arg"] = [None]
+
+                    return True
+    return False
+
+game_play = on_message(rule = game_play_rule, permission = GROUP, priority = 20, block = True)
+
+@game_play.handle()
+async def _(bot:Bot, event:GroupMessageEvent, state:T_State):
+    game = state["game"]
+    msg = await game.play(bot, event, *state["arg"])
+    await create_game.finish(msg)
 
 # 随机对战
 random_game = on_command("随机对战", permission = GROUP, priority = 5, block = True)
 
 @random_game.handle()
-async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
+async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
     gold = arg.extract_plain_text().strip()
     if gold.isdigit():
         gold = int(gold)
     else:
         gold = -1
     msg = Game.random_game(event, gold)
     await random_game.finish(msg)
 
-async def session_check(event:GroupMessageEvent):
+async def session_check(event:GroupMessageEvent, state:T_State):
     """
     本群有对局
     """
-    return event.group_id in current_games
+    group_id = event.group_id
+    if group_id in current_games:
+        state["game"] = current_games[group_id]
+        return True
+    else:
+        return False
 
 # 接受挑战
 accept = on_command("接受挑战", aliases = {"接受决斗", "接受对决"}, rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @accept.handle()
-async def _(event:GroupMessageEvent):
-    msg = Game.accept(event)
+async def _(event:GroupMessageEvent, state:T_State):
+    game = state["game"]
+    msg = game.accept(event)
     await accept.finish(msg)
 
 # 拒绝挑战
 refuse = on_command("拒绝挑战", aliases={"拒绝决斗", "拒绝对决"}, rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @refuse.handle()
-async def _(event:GroupMessageEvent):
-    msg = Game.refuse(event)
+async def _(event:GroupMessageEvent, state:T_State):
+    game = state["game"]
+    msg = game.refuse(event)
     await refuse.finish(msg)
 
 # 超时结算
 overtime = on_command("超时结算", rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @overtime.handle()
-async def _(bot:Bot, event:GroupMessageEvent):
-    msg = await Game.overtime(bot, event)
+async def _(bot:Bot, event:GroupMessageEvent, state:T_State):
+    game = state["game"]
+    msg = await game.overtime(bot, event)
     await overtime.finish(msg)
 
 # 认输结算
 fold = on_fullmatch(("认输", "投降", "结束"), rule = session_check, permission = GROUP, priority = 20, block = True)
 
 @fold.handle()
-async def _(bot:Bot, event:GroupMessageEvent):
-    await Game.fold(bot, event)
+async def _(bot:Bot, event:GroupMessageEvent, state:T_State):
+    game = state["game"]
+    await game.fold(bot, event)
 
 # 幸运花色
 slot = on_command("幸运花色", aliases = {"抽花色"}, permission = PRIVATE, priority = 20, block = True)
 
 @slot.handle()
 async def _(event:MessageEvent, arg:Message = CommandArg()):
     gold = arg.extract_plain_text().strip()
@@ -665,21 +545,15 @@
     )
 
 @russian_All_rank.handle()
 async def _(bot:Bot, event:MessageEvent):
     cmd = event.get_plaintext().strip().split()
     title = re.search(r"^(金币|资产|财富|胜率|胜场|败场|路灯挂件)(总排行|总榜)",cmd[0]).group(1)
     msg = await Account.All_rank(event, title)
-    if msg:
-        if isinstance(event, GroupMessageEvent):
-            await bot.send_group_forward_msg(group_id = event.group_id, messages = msg)
-        else:
-            await bot.send_private_forward_msg(user_id = event.user_id, messages = msg)
-    else:
-        await russian_All_rank.finish("无数据。")
+    await russian_All_rank.finish(msg)
 
 # 公司上市
 Market_public = on_command(
     "市场注册",
     aliases = {"公司注册","注册公司"},
     rule = to_me(),
     permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 ——————————
     下面是实例~♡
 ——————————
 +++++++++++++++++"""
 
 import os
 
-resourcefile = Path(os.path.join(os.path.dirname(__file__),"../resource"))
+resourcefile = Path(os.path.join(os.path.dirname(__file__),"./resource"))
 
 # 加载道具库
 with open(resourcefile / "props_library.json", "r", encoding="utf8") as f:
     props_library = json.load(f)
 
 def update_props_index(props_index):
     """
@@ -197,15 +197,14 @@
 
 def OHLC(path, company_id):
     """
     OHLC子程序
     """
     return subprocess.Popen([python,f"{resourcefile}/subprocess/ohlc.py", path, str(company_id)], shell = True)
 
-
 """
 from . import Data
 from .Data import (
     DataBase,
     UserData,
     UserDict,
     GroupAccount,
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874999999999999%*

 * *Differences: {"'41001'": "{'intro': '与空气相比，这个比较高级。\\n你抽到了四星道具，但是不知道要给你什么。'}",*

 * * "'42001'": "{'des': '取消了对大额跨群转账的适用。'}",*

 * * "'42101'": "{'intro': '随机获得对方在本群3%~5%的金币和持有股票。'}",*

 * * "'52001'": "{'intro': '庄家提供的保险单，在对局中失败时庄家为您承担10%的损失。\\n在详细审核这个业务之后，股东大会一致认为这是一门稳赔不赚的买卖。'}",*

 * * "'52002'": "{'intro': '庄家提供的保险单，在对局中胜利时庄家为您提供10%的额外奖励。'}",*

 * * "'62101'": "{'des': '可以用来。。。'}"}*

```diff
@@ -68,29 +68,29 @@
         "intro": "\u6253\u5f00\u53ef\u4ee5\u83b7\u5f97\u968f\u673a\u56db\u4e2a\u5143\u7d20\u3002",
         "name": "\u521d\u7ea7\u5143\u7d20",
         "rare": 3
     },
     "41001": {
         "color": "#66CCFF",
         "des": "\u603b\u4e4b\u6bd4\u8f83\u9ad8\u7ea7\u3002",
-        "intro": "\u4e0e\u7a7a\u6c14\u76f8\u6bd4\uff0c\u8fd9\u4e2a\u6bd4\u8f83\u9ad8\u7ea7\u3002\n\n\u4f60\u62bd\u5230\u4e86\u56db\u661f\u9053\u5177\uff0c\u4f46\u662f\u4e0d\u77e5\u9053\u8981\u7ed9\u4f60\u4ec0\u4e48\u3002",
+        "intro": "\u4e0e\u7a7a\u6c14\u76f8\u6bd4\uff0c\u8fd9\u4e2a\u6bd4\u8f83\u9ad8\u7ea7\u3002\n\u4f60\u62bd\u5230\u4e86\u56db\u661f\u9053\u5177\uff0c\u4f46\u662f\u4e0d\u77e5\u9053\u8981\u7ed9\u4f60\u4ec0\u4e48\u3002",
         "name": "\u9ad8\u7ea7\u7a7a\u6c14",
         "rare": 4
     },
     "42001": {
         "color": "#4169E1",
-        "des": "\u6587\u9171\u6700\u8fd1\u53d6\u6d88\u4e86\u5bf9\u5927\u989d\u8de8\u7fa4\u8f6c\u8d26\u7684\u9002\u7528\u3002",
+        "des": "\u53d6\u6d88\u4e86\u5bf9\u5927\u989d\u8de8\u7fa4\u8f6c\u8d26\u7684\u9002\u7528\u3002",
         "intro": "\u8eab\u4efd\u5c0a\u8d35\u7684\u6807\u5fd7\uff0c\u53ef\u4ee5\u5728\u8f6c\u8d26\u548c\u7ed3\u7b97\u65f6\u514d\u9664\u624b\u7eed\u8d39\u3002",
         "name": "\u94bb\u77f3\u4f1a\u5458\u5361",
         "rare": 4
     },
     "42101": {
         "color": "#003366",
         "des": "\u795d\u4f60\u597d\u8fd0\u3002",
-        "intro": "\u968f\u673a\u83b7\u5f97\u5bf9\u65b9\u5728\u672c\u7fa42%~5%\u7684\u91d1\u5e01\u548c\u6301\u6709\u80a1\u7968\u3002",
+        "intro": "\u968f\u673a\u83b7\u5f97\u5bf9\u65b9\u5728\u672c\u7fa43%~5%\u7684\u91d1\u5e01\u548c\u6301\u6709\u80a1\u7968\u3002",
         "name": "\u8c03\u67e5\u51ed\u8bc1",
         "rare": 4
     },
     "51001": {
         "color": "#66CCFF",
         "des": "\u770b\u8d77\u6765\u5c31\u5f88\u8d35\u3002",
         "intro": "\u9ad8\u538b\u94a2\u74f6\u5305\u88c5\uff0c\u5185\u542b78%\u7684\u6c2e\u6c14\u300121%\u7684\u6c27\u6c14\u30010.94%\u7684\u7a00\u6709\u6c14\u4f53,0.03%\u7684\u4e8c\u6c27\u5316\u78b3,0.03%\u7684\u5176\u5b83\u6c14\u4f53\u3002",
@@ -103,22 +103,22 @@
         "intro": "\u522b\u95ee\u4e3a\u4ec0\u4e48\u7a00\u6709\u5ea6\u8fd9\u4e48\u9ad8\uff0c\u8d35\u5c31\u8d35\u5728\u8fd0\u8d39\u3002",
         "name": "\u8fdb\u53e3\u7a7a\u6c14",
         "rare": 5
     },
     "52001": {
         "color": "#A0522D",
         "des": "--likaris",
-        "intro": "\u5e84\u5bb6\u63d0\u4f9b\u7684\u4fdd\u9669\u5355\uff0c\u5728\u5bf9\u5c40\u4e2d\u5931\u8d25\u65f6\u5e84\u5bb6\u4e3a\u60a8\u627f\u62c510%\u7684\u635f\u5931\u3002\n\n\u5728\u8be6\u7ec6\u5ba1\u6838\u8fd9\u4e2a\u4e1a\u52a1\u4e4b\u540e\uff0c\u80a1\u4e1c\u5927\u4f1a\u4e00\u81f4\u8ba4\u4e3a\u8fd9\u662f\u4e00\u95e8\u7a33\u8d54\u4e0d\u8d5a\u7684\u4e70\u5356\u3002",
+        "intro": "\u5e84\u5bb6\u63d0\u4f9b\u7684\u4fdd\u9669\u5355\uff0c\u5728\u5bf9\u5c40\u4e2d\u5931\u8d25\u65f6\u5e84\u5bb6\u4e3a\u60a8\u627f\u62c510%\u7684\u635f\u5931\u3002\n\u5728\u8be6\u7ec6\u5ba1\u6838\u8fd9\u4e2a\u4e1a\u52a1\u4e4b\u540e\uff0c\u80a1\u4e1c\u5927\u4f1a\u4e00\u81f4\u8ba4\u4e3a\u8fd9\u662f\u4e00\u95e8\u7a33\u8d54\u4e0d\u8d5a\u7684\u4e70\u5356\u3002",
         "name": "10%\u7ed3\u7b97\u8865\u8d34",
         "rare": 5
     },
     "52002": {
         "color": "#B22222",
         "des": "--likaris",
-        "intro": "\u5e84\u5bb6\u63d0\u4f9b\u7684\u4fdd\u9669\u5355\uff0c\u5728\u5bf9\u5c40\u4e2d\u80dc\u5229\u65f6\u5e84\u5bb6\u4e3a\u60a8\u63d0\u4f9b10%\u7684\u989d\u5916\u5956\u52b1\u3002\n\n\u6211\u89c9\u5f97\u6211\u4eec\u6709\u5fc5\u8981\u63d0\u9192\u4f60\u54b1\u4eec\u7684\u4e1a\u52a1\u5e76\u4e0d\u662f\u641e\u6148\u5584\u3002",
+        "intro": "\u5e84\u5bb6\u63d0\u4f9b\u7684\u4fdd\u9669\u5355\uff0c\u5728\u5bf9\u5c40\u4e2d\u80dc\u5229\u65f6\u5e84\u5bb6\u4e3a\u60a8\u63d0\u4f9b10%\u7684\u989d\u5916\u5956\u52b1\u3002",
         "name": "10%\u989d\u5916\u5956\u52b1",
         "rare": 5
     },
     "52101": {
         "color": "#9999FF",
         "des": "\u4f7f\u7528\u795e\u79d8\u5929\u5e73\u9700\u8981\u4e00\u70b9\u70b9\u624b\u7eed\u8d39\u3002",
         "intro": "\u4e0e\u968f\u673a\u4e00\u4e2a\u4eba\u5e73\u5206\u91d1\u5e01\u3002",
@@ -144,15 +144,15 @@
         "des": "",
         "intro": "",
         "name": "\u7eaf\u51c0\u7a7a\u6c14",
         "rare": 6
     },
     "62101": {
         "color": "#0099FF",
-        "des": "\u201c\u94bb\u77f3\u6709\u4ec0\u4e48\u7528\uff1f\u201d\n\u201c\u6ca1\u7528\u3002\u201d",
+        "des": "\u53ef\u4ee5\u7528\u6765\u3002\u3002\u3002",
         "intro": "\u65e0\u6bd4\u73cd\u8d35\u7684\u94bb\u77f3\uff0c\u53ea\u6709\u5343\u5206\u4e4b\u4e94\u7684\u6982\u7387\u83b7\u5f97\uff0c\u4ee5\u540e\u53ef\u80fd\u6709\u7528\u3002",
         "name": "\u94bb\u77f3",
         "rare": 6
     },
     "63101": {
         "color": "#FF3300",
         "des": "\u4f60\u53ef\u4ee5\u4e00\u76f4\u76f8\u4fe1\u81ea\u5df1\u7684\u8fd0\u6c14\u3002",
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from typing import Tuple
 from pathlib import Path
 
 import mplfinance as mpf
 import pandas as pd
 
-import time
 import sys
-
+import time
+from datetime import datetime
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 
-def market_candlestick(figsize:Tuple[int,int], lenth:int, history:list, savefig):
+def market_candlestick(figsize:Tuple[int,int], length:int, history:list, savefig):
     """
     生成股价K线图
         figsize:图片尺寸
-        lenth:OHLC采样长度
+        length:OHLC采样长度
         history:历史数据
         title:标题
     """
     T, buy, sell = zip(*history)
     l = len(T)
-    T = [T[i:i+lenth] for i in range(0, l, lenth)]
-    buy = [buy[i:i+lenth] for i in range(0, l, lenth)]
-    sell = [sell[i:i+lenth] for i in range(0, l, lenth)]
+    T = [T[i:i+length] for i in range(0, l, length)]
+    buy = [buy[i:i+length] for i in range(0, l, length)]
+    sell = [sell[i:i+length] for i in range(0, l, length)]
     D,O,H,L,C = [],[],[],[],[]
     for i in range(len(sell)):
-        D.append(pd.to_datetime(T[i][0], unit='s'))
+        D.append(datetime.fromtimestamp(T[i][0]))
         O.append(sell[i][0])
         H.append(max(sell[i]))
         L.append(min(sell[i]))
         C.append(sell[i][-1])
-
     data = pd.DataFrame({'date': D,'open': O,'high': H,'low': L,'close': C})
     data = data.set_index('date')
     style = mpf.make_mpf_style(
         base_mpf_style = "charles",
         marketcolors = mpf.make_marketcolors(
             up = "#a02128",
             down = "#006340",
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -44,31 +44,8 @@
     try:
         n = int(N)
     except ValueError:
         try:
             n = int(unicodedata.numeric(N))
         except (TypeError, ValueError):
             n = 0
-    return n
-
-def line_wrap(msg:str, n:int= 24) -> str:
-    """
-    自动换行
-    """
-    newmsg = ""
-    flag = 0
-    for x in msg:
-        newmsg += x
-        if x == "\n":
-            flag = 0
-        elif flag > n:
-            newmsg += "\n"
-            flag = 0
-        else:
-            if ord(x) < 0x200:
-                flag += 1
-            else:
-                flag += 2
-
-    newmsg += "\n"
-    newmsg = re.sub('[\r\n]+', '\n', newmsg)
-    return newmsg
+    return n
```

### Comparing `nonebot_plugin_game_collection-2.2.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 nonebot_plugin_game_collection/Account.py
 nonebot_plugin_game_collection/Game.py
 nonebot_plugin_game_collection/Manager.py
 nonebot_plugin_game_collection/Market.py
 nonebot_plugin_game_collection/Prop.py
 nonebot_plugin_game_collection/__init__.py
 nonebot_plugin_game_collection/config.py
+nonebot_plugin_game_collection/data.py
 nonebot_plugin_game_collection.egg-info/PKG-INFO
 nonebot_plugin_game_collection.egg-info/SOURCES.txt
 nonebot_plugin_game_collection.egg-info/dependency_links.txt
 nonebot_plugin_game_collection.egg-info/requires.txt
 nonebot_plugin_game_collection.egg-info/top_level.txt
 nonebot_plugin_game_collection/HorseRace/events_main.py
 nonebot_plugin_game_collection/HorseRace/horse.py
 nonebot_plugin_game_collection/HorseRace/race_group.py
 nonebot_plugin_game_collection/HorseRace/start.py
-nonebot_plugin_game_collection/data/api.py
-nonebot_plugin_game_collection/data/data.py
-nonebot_plugin_game_collection/data/run.py
 nonebot_plugin_game_collection/resource/element_library.json
 nonebot_plugin_game_collection/resource/menu_data.json
 nonebot_plugin_game_collection/resource/props_library.json
 nonebot_plugin_game_collection/resource/horserace/Stand.json
 nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
 nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
 nonebot_plugin_game_collection/resource/horserace/基础事件.json
```

### Comparing `nonebot_plugin_game_collection-2.2.5/setup.py` & `nonebot_plugin_game_collection-2.2.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.2.5',
+version='2.2.6',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
 platforms='all',
-install_requires=["nonebot2","nonebot-adapter-onebot","nonebot_plugin_apscheduler","nonebot_plugin_imageutils","mplfinance","seaborn"],
+install_requires=["nonebot2","nonebot-adapter-onebot","nonebot_plugin_apscheduler","mplfinance","seaborn"],
 url='https://github.com/KarisAya/nonebot_plugin_game_collection',
 )
```

