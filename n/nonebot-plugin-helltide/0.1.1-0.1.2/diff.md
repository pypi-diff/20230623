# Comparing `tmp/nonebot_plugin_helltide-0.1.1.tar.gz` & `tmp/nonebot_plugin_helltide-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_helltide-0.1.1.tar", last modified: Fri Jun 23 15:54:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_helltide-0.1.2.tar", last modified: Fri Jun 23 16:08:38 2023, max compression
```

## Comparing `nonebot_plugin_helltide-0.1.1.tar` & `nonebot_plugin_helltide-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-06-23 10:24:24.649445 nonebot_plugin_helltide-0.1.1/LICENSE
--rw-r--r--   0        0        0     2683 2023-06-23 15:00:03.579347 nonebot_plugin_helltide-0.1.1/README.md
--rw-r--r--   0        0        0     3255 2023-06-23 10:24:24.682446 nonebot_plugin_helltide-0.1.1/nonebot_plugin_helltide/.gitignore
--rw-r--r--   0        0        0    11825 2023-06-23 15:06:45.849480 nonebot_plugin_helltide-0.1.1/nonebot_plugin_helltide/__init__.py
--rw-r--r--   0        0        0      226 2023-06-23 10:24:24.682945 nonebot_plugin_helltide-0.1.1/nonebot_plugin_helltide/config.py
--rw-r--r--   0        0        0      761 2023-06-23 15:54:39.940010 nonebot_plugin_helltide-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2598 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/README.md
+-rw-r--r--   0        0        0     3093 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/.gitignore
+-rw-r--r--   0        0        0    11578 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/config.py
+-rw-r--r--   0        0        0      790 2023-06-23 16:08:38.721228 nonebot_plugin_helltide-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_helltide-0.1.1/README.md` & `nonebot_plugin_helltide-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-helltide
-
-_✨ 一个Diablo4的helltide和世界boss的提醒小助手 ✨_
-
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/qbkira/nonebot-plugin-helltide.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-helltide">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-helltide.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-## 📖 介绍
-
-添加机器人到群聊中，订阅之后在群里会提醒订阅Boss刷新，地狱狂潮提醒，（还有军团的刷新时间）
-
-## 💿 安装
-
-<details>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-helltide
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-helltide
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-helltide
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-helltide
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-helltide
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_helltide"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| event_check_interval | 否 | 1 | 每隔1分钟检查一下 |
-
-## 🎉 使用
-### 指令表
-| 指令 | 权限 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|:----:|
-| d4 | 群员 | 是 | 群聊 | 查询 Diablo4 事件信息 |
-| d4订阅 | 群员 | 是 | 群聊 | 订阅 Diablo4 定时消息提醒 |
-| d4取消订阅 | 群员 | 是 | 群聊 | 取消订阅 Diablo4 定时消息提醒 |
-| d4查询订阅 | 群员 | 是 | 群聊 | 查询当前订阅 Diablo4 定时消息提醒的用户 |
-| d4帮助 | 群员 | 是 | 群聊 | 显示帮助信息 |
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-helltide
+
+_✨ 一个Diablo4的helltide和世界boss的提醒小助手 ✨_
+
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/qbkira/nonebot-plugin-helltide.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-helltide">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-helltide.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+## 📖 介绍
+
+添加机器人到群聊中，订阅之后在群里会提醒订阅Boss刷新，地狱狂潮提醒，（还有军团的刷新时间）
+
+## 💿 安装
+
+<details>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-helltide
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-helltide
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-helltide
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-helltide
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-helltide
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_helltide"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| event_check_interval | 否 | 1 | 每隔1分钟检查一下 |
+
+## 🎉 使用
+### 指令表
+| 指令 | 权限 | 需要@ | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|:----:|
+| d4 | 群员 | 是 | 群聊 | 查询 Diablo4 事件信息 |
+| d4订阅 | 群员 | 是 | 群聊 | 订阅 Diablo4 定时消息提醒 |
+| d4取消订阅 | 群员 | 是 | 群聊 | 取消订阅 Diablo4 定时消息提醒 |
+| d4查询订阅 | 群员 | 是 | 群聊 | 查询当前订阅 Diablo4 定时消息提醒的用户 |
+| d4帮助 | 群员 | 是 | 群聊 | 显示帮助信息 |
```

### Comparing `nonebot_plugin_helltide-0.1.1/nonebot_plugin_helltide/__init__.py` & `nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-from nonebot import require, Bot, get_driver
-from nonebot.plugin import PluginMetadata
-import nonebot
-import httpx
-from .config import Config
-from nonebot import on_command
-from nonebot.rule import to_me
-from nonebot.adapters.onebot.v11 import (
-    GroupMessageEvent,
-    MessageEvent,
-)
-import datetime
-
-__plugin_meta__ = PluginMetadata(
-    name="helltide",
-    description="一个Diablo4的helltide和世界boss的提醒小助手",
-    # BEGIN: 7d7f3c7b5d4a
-    usage="这是一个diablo4插件，可以订阅游戏中的事件，如boss刷新、地狱潮汐等，\n当事件即将发生时会自动提醒订阅用户。使用方法：\n1. 订阅事件：d4订阅 boss/helltide\n2. 取消订阅事件：d4取消订阅 boss/helltide\n3. 查询订阅列表：d4查询订阅",
-    type="application",
-    config=Config,
-    # END: 7d7f3c7b5d4a
-    extra={"author": "qbkira"},
-)
-
-my_config = Config.parse_obj(get_driver().config)
-
-import json
-import os
-from pathlib import Path
-import aiofiles
-from typing import Dict, List
-
-data_path = Path("data/diablo4").resolve() / "data.json"
-
-
-subscription_dict = {}
-
-def load_data():
-    print(f"load_data path: {data_path}")
-    if not os.path.exists(data_path.parent):
-        os.makedirs(data_path.parent)
-    if os.path.exists(data_path):
-        with open(data_path, mode='r') as f:
-            subscription_dict = json.loads(f.read())
-    else:
-        subscription_dict = {}
-        with open(data_path, mode='w') as f:
-            f.write(json.dumps(subscription_dict))
-    print(f"订阅用户：{subscription_dict}")
-    return subscription_dict
-    
-async def save_data():
-    async with aiofiles.open(data_path, mode='w') as f:
-        await f.write(json.dumps(subscription_dict))
-        
-subscription_dict = load_data()
-
-require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler
-
-
-# Add a dictionary to store the notice status of each event
-notice_status = {}
-
-@scheduler.scheduled_job("interval", minutes=my_config.event_check_interval)
-async def check_event():
-    url = my_config.url_api
-    try:
-        async with httpx.AsyncClient() as client:
-            response = await client.get(url)
-            data = parse_event_data(response)
-            for group_id in subscription_dict:
-                subscription_list = subscription_dict[group_id]
-                if group_id not in notice_status:
-                    notice_status[group_id] = {
-                        "boss": False,
-                        "helltide": False
-                    }
-                if subscription_list:
-                    if data["boss"]["expected"] - datetime.datetime.now().timestamp() <= 600:
-                        if not notice_status[group_id]["boss"]:
-                            await boss_notice_subscription_users(group_id, data)
-                            notice_status[group_id]["boss"] = True
-                    else:
-                        notice_status[group_id]["boss"] = False
-                    if data["helltide"]["expected"] - datetime.datetime.now().timestamp() <= 600:
-                        if not notice_status[group_id]["helltide"]:
-                            await helltide_notice_subscription_users(group_id, data)
-                            notice_status[group_id]["helltide"] = True
-                    else:
-                        notice_status[group_id]["helltide"] = False
-    except Exception as e:
-        print(f"Error occurred while checking event: {e}")
-
-# Add command to query current subscribed users
-d4_query_subscriptions = on_command("d4查询订阅", aliases={"d4query"}, block=True, rule=to_me(), priority=1)
-
-@d4_query_subscriptions.handle()
-async def query_subscriptions_handler(bot: Bot, event: MessageEvent):
-    group_id = str(event.group_id)
-    print(f"subscription_dict: {subscription_dict}")
-    if group_id not in subscription_dict:
-        subscription_dict[group_id] = []
-    subscription_list = subscription_dict[group_id]
-    if not subscription_list:
-        await bot.send(event, "当前没有用户订阅 Diablo4 定时消息提醒。\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
-    else:
-        subscribed_users = "\n".join([f"{i+1}. {user_id}" for i, user_id in enumerate(subscription_list)])
-        await bot.send(event, f"当前订阅 Diablo4 定时消息提醒的用户有：\n{subscribed_users}\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
-
-d4_subscribe = on_command("d4订阅", aliases={"d4sub"}, block=True, rule=to_me(), priority=1)
-
-@d4_subscribe.handle()
-async def subscribe_handler(bot: Bot, event: MessageEvent):
-    group_id = str(event.group_id)
-    user_id = event.user_id
-    if group_id not in subscription_dict:
-        subscription_dict[group_id] = []
-    subscription_list = subscription_dict[group_id]
-    if user_id not in subscription_list:
-        subscription_list.append(user_id)
-        subscription_dict[group_id] = subscription_list
-        await save_data()
-        await bot.send(event, "订阅成功！\n使用[@机器人 d4取消订阅] 可以取消订阅 Diablo4 定时消息提醒。")
-    else:
-        await bot.send(event, "您已经订阅了 Diablo4 定时消息提醒。\n使用[@机器人 d4取消订阅] 可以取消订阅 Diablo4 定时消息提醒。")
-
-d4_unsubscribe = on_command("d4取消订阅", aliases={"d4unsub"}, block=True, rule=to_me(), priority=1)
-
-@d4_unsubscribe.handle()
-async def unsubscribe_handler(bot: Bot, event: MessageEvent):
-    group_id = str(event.group_id)
-    user_id = event.user_id
-    if group_id not in subscription_dict:
-        subscription_dict[group_id] = []
-    subscription_list = subscription_dict[group_id]
-    if user_id in subscription_list:
-        subscription_list.remove(user_id)
-        subscription_dict[group_id] = subscription_list
-        await save_data()
-        await bot.send(event, "取消订阅成功！\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
-    else:
-        await bot.send(event, "您还没有订阅 Diablo4 定时消息提醒。\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
-
-d4armory = on_command("diablo4", aliases={"d4"}, block=True, rule=to_me(), priority=1)
-
-@d4armory.handle()
-async def diablo4(event: MessageEvent) -> None:
-    if isinstance(event, GroupMessageEvent):
-        group_id = str(event.group_id)
-        if group_id not in subscription_dict:
-            subscription_dict[group_id] = []
-        subscription_list = subscription_dict[group_id]
-        result = await response_event_info()
-        if subscription_list:
-            at_users = " ".join([f"[CQ:at,qq={user_id}]" for user_id in subscription_list])
-            result = f"{result}\n\n{at_users}"
-        await d4armory.send(result)
-    else:
-        result = await response_event_info()
-        await d4armory.send(result)
-
-async def response_event_info():
-    try:
-        url = my_config.url_api
-        async with httpx.AsyncClient() as client:
-            response = await client.get(url)
-            data = parse_event_data(response)
-            return parse_event_info(data)
-    except Exception as e:
-        print(f"Error occurred while fetching event info: {e}")
-        return "无法获取 Diablo4 事件信息，请稍后再试。"
-
-async def helltide_notice_subscription_users(group_id, data):
-    bot = nonebot.get_bot()
-    info = parse_event_info(data)
-    subscription_list = subscription_dict[group_id]
-    if subscription_list:
-        at_users = " ".join([f"[CQ:at,qq={user_id}]" for user_id in subscription_list])
-        message = f"{info}\n\n{at_users}\n[地狱狂潮]刷新时间还差不到10分钟，请做好准备！\n使用[@机器人 d4订阅] 可以订阅定时消息提醒。"
-        await bot.send_group_msg(group_id=group_id, message=message)
-
-                
-async def boss_notice_subscription_users(group_id, data):
-    bot = nonebot.get_bot()
-    info = parse_event_info(data)
-    subscription_list = subscription_dict[group_id]
-    if subscription_list:
-        at_users = " ".join([f"[CQ:at,qq={user_id}]" for user_id in subscription_list])
-        message = f"{info}\n\n{at_users}\n[Boss]刷新时间还差不到10分钟，请做好准备！\n使用[@机器人 d4订阅] 可以订阅定时消息提醒。"
-        await bot.send_group_msg(group_id=group_id, message=message)
-
-
-def parse_event_data(response):
-    data = response.json()
-    helltide = data["helltide"]
-    helltide["expected"] = helltide["timestamp"] + 2*60*60 + 15*60 # Add expected attribute to helltide
-    return data
-
-def parse_event_info(data):
-    boss = data["boss"]
-    helltide = data["helltide"]
-    legion = data["legion"]
-    now = datetime.datetime.now().timestamp()
-    boss_expected_name = boss["expectedName"]
-    boss_expected_timestamp = datetime.datetime.fromtimestamp(boss["expected"]).strftime('%Y-%m-%d %H:%M:%S')
-    if now - helltide["timestamp"] <= 3600:
-        helltide_expected = datetime.datetime.fromtimestamp(helltide["timestamp"] + 3600).strftime('%Y-%m-%d %H:%M:%S')
-        result = f"Boss名字: {boss_expected_name}\nBoss刷新: {boss_expected_timestamp}\n狂潮(中): {helltide_expected}结束\n军团时间: {datetime.datetime.fromtimestamp(legion['timestamp']).strftime('%Y-%m-%d %H:%M:%S')}"
-    else:
-        result = f"Boss名字: {boss_expected_name}\nBoss刷新: {boss_expected_timestamp}\n狂潮刷新: {datetime.datetime.fromtimestamp(helltide['expected']).strftime('%Y-%m-%d %H:%M:%S')}\n军团时间: {datetime.datetime.fromtimestamp(legion['timestamp']).strftime('%Y-%m-%d %H:%M:%S')}"
-    return result
-
-# Add command to trigger event check for debugging purposes
-d4_debug = on_command("d4调试", aliases={"d4debug"}, block=True, rule=to_me(), priority=1)
-
-@d4_debug.handle()
-async def debug_handler(bot: nonebot.Bot, event: MessageEvent):
-    url = "https://d4armory.io/api/events/recent"
-    async with httpx.AsyncClient() as client:
-        response = await client.get(url)
-        group_id = str(event.group_id)
-        data = parse_event_data(response)
-        await boss_notice_subscription_users(group_id, data)
-        await helltide_notice_subscription_users(group_id, data)
-
-# Add command to display help information
-d4_help = on_command("d4帮助", aliases={"d4help"}, block=True, rule=to_me(), priority=1)
-
-### 指令表
-# | 指令 | 权限 | 需要@ | 范围 | 说明 |
-# |:-----:|:----:|:----:|:----:|:----:|
-# | [@机器人 d4] | 群员 | 是 | 群聊 | 查询 Diablo4 事件信息 |
-# | [@机器人 d4订阅] | 群员 | 是 | 群聊 | 订阅 Diablo4 定时消息提醒 |
-# | [@机器人 d4取消订阅] | 群员 | 是 | 群聊 | 取消订阅 Diablo4 定时消息提醒 |
-# | [@机器人 d4查询订阅] | 群员 | 是 | 群聊 | 查询当前订阅 Diablo4 定时消息提醒的用户 |
-# | [@机器人 d4帮助] | 群员 | 是 | 群聊 | 显示帮助信息 |
-@d4_help.handle()
-async def help_handler(bot: nonebot.Bot, event: MessageEvent):
-    help_info = "以下是 Diablo4 定时消息提醒机器人的指令说明：\n\n"
-    help_info += "[@机器人 d4] - 查询 Diablo4 事件信息\n"
-    help_info += "[@机器人 d4订阅] - 订阅 Diablo4 定时消息提醒\n"
-    help_info += "[@机器人 d4取消订阅] - 取消订阅 Diablo4 定时消息提醒\n"
-    help_info += "[@机器人 d4查询订阅] - 查询当前订阅 Diablo4 定时消息提醒的用户\n"
-    help_info += "[@机器人 d4帮助] - 显示帮助信息\n"
-    # help_info += "[@机器人 d4调试] - 触发事件检查以进行调试\n"
-    await bot.send(event, help_info)
+from nonebot import require, Bot, get_driver
+from nonebot.plugin import PluginMetadata
+import nonebot
+import httpx
+from .config import Config
+from nonebot import on_command
+from nonebot.rule import to_me
+from nonebot.adapters.onebot.v11 import (
+    GroupMessageEvent,
+    MessageEvent,
+)
+import datetime
+
+__plugin_meta__ = PluginMetadata(
+    name="helltide",
+    description="一个Diablo4的helltide和世界boss的提醒小助手",
+    # BEGIN: 7d7f3c7b5d4a
+    usage="这是一个diablo4插件，可以订阅游戏中的事件，如boss刷新、地狱潮汐等，\n当事件即将发生时会自动提醒订阅用户。使用方法：\n1. 订阅事件：d4订阅 boss/helltide\n2. 取消订阅事件：d4取消订阅 boss/helltide\n3. 查询订阅列表：d4查询订阅",
+    type="application",
+    config=Config,
+    # END: 7d7f3c7b5d4a
+    extra={"author": "qbkira"},
+)
+
+my_config = Config.parse_obj(get_driver().config)
+
+import json
+import os
+from pathlib import Path
+import aiofiles
+from typing import Dict, List
+
+data_path = Path("data/diablo4").resolve() / "data.json"
+
+
+subscription_dict = {}
+
+def load_data():
+    print(f"load_data path: {data_path}")
+    if not os.path.exists(data_path.parent):
+        os.makedirs(data_path.parent)
+    if os.path.exists(data_path):
+        with open(data_path, mode='r') as f:
+            subscription_dict = json.loads(f.read())
+    else:
+        subscription_dict = {}
+        with open(data_path, mode='w') as f:
+            f.write(json.dumps(subscription_dict))
+    print(f"订阅用户：{subscription_dict}")
+    return subscription_dict
+    
+async def save_data():
+    async with aiofiles.open(data_path, mode='w') as f:
+        await f.write(json.dumps(subscription_dict))
+        
+subscription_dict = load_data()
+
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler
+
+
+# Add a dictionary to store the notice status of each event
+notice_status = {}
+
+@scheduler.scheduled_job("interval", minutes=my_config.event_check_interval)
+async def check_event():
+    url = my_config.url_api
+    try:
+        async with httpx.AsyncClient() as client:
+            response = await client.get(url)
+            data = parse_event_data(response)
+            for group_id in subscription_dict:
+                subscription_list = subscription_dict[group_id]
+                if group_id not in notice_status:
+                    notice_status[group_id] = {
+                        "boss": False,
+                        "helltide": False
+                    }
+                if subscription_list:
+                    if data["boss"]["expected"] - datetime.datetime.now().timestamp() <= 600:
+                        if not notice_status[group_id]["boss"]:
+                            await boss_notice_subscription_users(group_id, data)
+                            notice_status[group_id]["boss"] = True
+                    else:
+                        notice_status[group_id]["boss"] = False
+                    if data["helltide"]["expected"] - datetime.datetime.now().timestamp() <= 600:
+                        if not notice_status[group_id]["helltide"]:
+                            await helltide_notice_subscription_users(group_id, data)
+                            notice_status[group_id]["helltide"] = True
+                    else:
+                        notice_status[group_id]["helltide"] = False
+    except Exception as e:
+        print(f"Error occurred while checking event: {e}")
+
+# Add command to query current subscribed users
+d4_query_subscriptions = on_command("d4查询订阅", aliases={"d4query"}, block=True, rule=to_me(), priority=1)
+
+@d4_query_subscriptions.handle()
+async def query_subscriptions_handler(bot: Bot, event: MessageEvent):
+    group_id = str(event.group_id)
+    print(f"subscription_dict: {subscription_dict}")
+    if group_id not in subscription_dict:
+        subscription_dict[group_id] = []
+    subscription_list = subscription_dict[group_id]
+    if not subscription_list:
+        await bot.send(event, "当前没有用户订阅 Diablo4 定时消息提醒。\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
+    else:
+        subscribed_users = "\n".join([f"{i+1}. {user_id}" for i, user_id in enumerate(subscription_list)])
+        await bot.send(event, f"当前订阅 Diablo4 定时消息提醒的用户有：\n{subscribed_users}\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
+
+d4_subscribe = on_command("d4订阅", aliases={"d4sub"}, block=True, rule=to_me(), priority=1)
+
+@d4_subscribe.handle()
+async def subscribe_handler(bot: Bot, event: MessageEvent):
+    group_id = str(event.group_id)
+    user_id = event.user_id
+    if group_id not in subscription_dict:
+        subscription_dict[group_id] = []
+    subscription_list = subscription_dict[group_id]
+    if user_id not in subscription_list:
+        subscription_list.append(user_id)
+        subscription_dict[group_id] = subscription_list
+        await save_data()
+        await bot.send(event, "订阅成功！\n使用[@机器人 d4取消订阅] 可以取消订阅 Diablo4 定时消息提醒。")
+    else:
+        await bot.send(event, "您已经订阅了 Diablo4 定时消息提醒。\n使用[@机器人 d4取消订阅] 可以取消订阅 Diablo4 定时消息提醒。")
+
+d4_unsubscribe = on_command("d4取消订阅", aliases={"d4unsub"}, block=True, rule=to_me(), priority=1)
+
+@d4_unsubscribe.handle()
+async def unsubscribe_handler(bot: Bot, event: MessageEvent):
+    group_id = str(event.group_id)
+    user_id = event.user_id
+    if group_id not in subscription_dict:
+        subscription_dict[group_id] = []
+    subscription_list = subscription_dict[group_id]
+    if user_id in subscription_list:
+        subscription_list.remove(user_id)
+        subscription_dict[group_id] = subscription_list
+        await save_data()
+        await bot.send(event, "取消订阅成功！\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
+    else:
+        await bot.send(event, "您还没有订阅 Diablo4 定时消息提醒。\n使用[@机器人 d4订阅] 可以订阅 Diablo4 定时消息提醒。")
+
+d4armory = on_command("diablo4", aliases={"d4"}, block=True, rule=to_me(), priority=1)
+
+@d4armory.handle()
+async def diablo4(event: MessageEvent) -> None:
+    if isinstance(event, GroupMessageEvent):
+        group_id = str(event.group_id)
+        if group_id not in subscription_dict:
+            subscription_dict[group_id] = []
+        subscription_list = subscription_dict[group_id]
+        result = await response_event_info()
+        if subscription_list:
+            at_users = " ".join([f"[CQ:at,qq={user_id}]" for user_id in subscription_list])
+            result = f"{result}\n\n{at_users}"
+        await d4armory.send(result)
+    else:
+        result = await response_event_info()
+        await d4armory.send(result)
+
+async def response_event_info():
+    try:
+        url = my_config.url_api
+        async with httpx.AsyncClient() as client:
+            response = await client.get(url)
+            data = parse_event_data(response)
+            return parse_event_info(data)
+    except Exception as e:
+        print(f"Error occurred while fetching event info: {e}")
+        return "无法获取 Diablo4 事件信息，请稍后再试。"
+
+async def helltide_notice_subscription_users(group_id, data):
+    bot = nonebot.get_bot()
+    info = parse_event_info(data)
+    subscription_list = subscription_dict[group_id]
+    if subscription_list:
+        at_users = " ".join([f"[CQ:at,qq={user_id}]" for user_id in subscription_list])
+        message = f"{info}\n\n{at_users}\n[地狱狂潮]刷新时间还差不到10分钟，请做好准备！\n使用[@机器人 d4订阅] 可以订阅定时消息提醒。"
+        await bot.send_group_msg(group_id=group_id, message=message)
+
+                
+async def boss_notice_subscription_users(group_id, data):
+    bot = nonebot.get_bot()
+    info = parse_event_info(data)
+    subscription_list = subscription_dict[group_id]
+    if subscription_list:
+        at_users = " ".join([f"[CQ:at,qq={user_id}]" for user_id in subscription_list])
+        message = f"{info}\n\n{at_users}\n[Boss]刷新时间还差不到10分钟，请做好准备！\n使用[@机器人 d4订阅] 可以订阅定时消息提醒。"
+        await bot.send_group_msg(group_id=group_id, message=message)
+
+
+def parse_event_data(response):
+    data = response.json()
+    helltide = data["helltide"]
+    helltide["expected"] = helltide["timestamp"] + 2*60*60 + 15*60 # Add expected attribute to helltide
+    return data
+
+def parse_event_info(data):
+    boss = data["boss"]
+    helltide = data["helltide"]
+    legion = data["legion"]
+    now = datetime.datetime.now().timestamp()
+    boss_expected_name = boss["expectedName"]
+    boss_expected_timestamp = datetime.datetime.fromtimestamp(boss["expected"]).strftime('%Y-%m-%d %H:%M:%S')
+    if now - helltide["timestamp"] <= 3600:
+        helltide_expected = datetime.datetime.fromtimestamp(helltide["timestamp"] + 3600).strftime('%Y-%m-%d %H:%M:%S')
+        result = f"Boss名字: {boss_expected_name}\nBoss刷新: {boss_expected_timestamp}\n狂潮(中): {helltide_expected}结束\n军团时间: {datetime.datetime.fromtimestamp(legion['timestamp']).strftime('%Y-%m-%d %H:%M:%S')}"
+    else:
+        result = f"Boss名字: {boss_expected_name}\nBoss刷新: {boss_expected_timestamp}\n狂潮刷新: {datetime.datetime.fromtimestamp(helltide['expected']).strftime('%Y-%m-%d %H:%M:%S')}\n军团时间: {datetime.datetime.fromtimestamp(legion['timestamp']).strftime('%Y-%m-%d %H:%M:%S')}"
+    return result
+
+# Add command to trigger event check for debugging purposes
+d4_debug = on_command("d4调试", aliases={"d4debug"}, block=True, rule=to_me(), priority=1)
+
+@d4_debug.handle()
+async def debug_handler(bot: nonebot.Bot, event: MessageEvent):
+    url = "https://d4armory.io/api/events/recent"
+    async with httpx.AsyncClient() as client:
+        response = await client.get(url)
+        group_id = str(event.group_id)
+        data = parse_event_data(response)
+        await boss_notice_subscription_users(group_id, data)
+        await helltide_notice_subscription_users(group_id, data)
+
+# Add command to display help information
+d4_help = on_command("d4帮助", aliases={"d4help"}, block=True, rule=to_me(), priority=1)
+
+### 指令表
+# | 指令 | 权限 | 需要@ | 范围 | 说明 |
+# |:-----:|:----:|:----:|:----:|:----:|
+# | [@机器人 d4] | 群员 | 是 | 群聊 | 查询 Diablo4 事件信息 |
+# | [@机器人 d4订阅] | 群员 | 是 | 群聊 | 订阅 Diablo4 定时消息提醒 |
+# | [@机器人 d4取消订阅] | 群员 | 是 | 群聊 | 取消订阅 Diablo4 定时消息提醒 |
+# | [@机器人 d4查询订阅] | 群员 | 是 | 群聊 | 查询当前订阅 Diablo4 定时消息提醒的用户 |
+# | [@机器人 d4帮助] | 群员 | 是 | 群聊 | 显示帮助信息 |
+@d4_help.handle()
+async def help_handler(bot: nonebot.Bot, event: MessageEvent):
+    help_info = "以下是 Diablo4 定时消息提醒机器人的指令说明：\n\n"
+    help_info += "[@机器人 d4] - 查询 Diablo4 事件信息\n"
+    help_info += "[@机器人 d4订阅] - 订阅 Diablo4 定时消息提醒\n"
+    help_info += "[@机器人 d4取消订阅] - 取消订阅 Diablo4 定时消息提醒\n"
+    help_info += "[@机器人 d4查询订阅] - 查询当前订阅 Diablo4 定时消息提醒的用户\n"
+    help_info += "[@机器人 d4帮助] - 显示帮助信息\n"
+    # help_info += "[@机器人 d4调试] - 触发事件检查以进行调试\n"
+    await bot.send(event, help_info)
```

### Comparing `nonebot_plugin_helltide-0.1.1/pyproject.toml` & `nonebot_plugin_helltide-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 ]
 
 [tool.nonebot]
 adapters = [
     { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
 ]
 plugins = [
-    "nonebot-plugin-helltide",
+    "nonebot_plugin_helltide",
 ]
 plugin_dirs = []
 builtin_plugins = []
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "nonebot-plugin-helltide"
-version = "0.1.1"
+version = "0.1.2"
 description = "Diablo 4 Helltide Event Tracker work with nonebot2"
 authors = [
     { name = "qbkira", email = "qbuouo@gmail.com" },
 ]
 dependencies = [
     "nonebot2",
     "nonebot2[fastapi]",
     "pydantic",
     "aiohttp",
+    "aiofiles",
+    "httpx",
     "nonebot-adapter-onebot",
     "nonebot-plugin-apscheduler",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
```

### Comparing `nonebot_plugin_helltide-0.1.1/PKG-INFO` & `nonebot_plugin_helltide-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helltide
-Version: 0.1.1
+Version: 0.1.2
 Summary: Diablo 4 Helltide Event Tracker work with nonebot2
 Author-Email: qbkira <qbuouo@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2
 Requires-Dist: nonebot2[fastapi]
 Requires-Dist: pydantic
 Requires-Dist: aiohttp
+Requires-Dist: aiofiles
+Requires-Dist: httpx
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-apscheduler
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.2 Summary:
 Diablo 4 Helltide Event Tracker work with nonebot2 Author-Email: qbkira
 gmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2
 Requires-Dist: nonebot2[fastapi] Requires-Dist: pydantic Requires-Dist: aiohttp
-Requires-Dist: nonebot-adapter-onebot Requires-Dist: nonebot-plugin-apscheduler
-Description-Content-Type: text/markdown
+Requires-Dist: aiofiles Requires-Dist: httpx Requires-Dist: nonebot-adapter-
+onebot Requires-Dist: nonebot-plugin-apscheduler Description-Content-Type:
+text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                         # nonebot-plugin-helltide _â¨
 ä¸ä¸ªDiablo4çhelltideåä¸çbossçæéå°å©æ â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç»
 æ·»å æºå¨äººå°ç¾¤èä¸­ï¼è®¢éä¹åå¨ç¾¤éä¼æéè®¢éBosså·æ°ï¼å°ç±çæ½®æéï¼ï¼è¿æåå¢çå·æ°æ¶é´ï¼
```

