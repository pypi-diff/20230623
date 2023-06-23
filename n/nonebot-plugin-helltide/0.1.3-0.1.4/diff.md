# Comparing `tmp/nonebot_plugin_helltide-0.1.3.tar.gz` & `tmp/nonebot_plugin_helltide-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_helltide-0.1.3.tar", last modified: Fri Jun 23 16:21:37 2023, max compression
+gzip compressed data, was "nonebot_plugin_helltide-0.1.4.tar", last modified: Fri Jun 23 16:38:18 2023, max compression
```

## Comparing `nonebot_plugin_helltide-0.1.3.tar` & `nonebot_plugin_helltide-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/LICENSE
--rw-r--r--   0        0        0     2598 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/README.md
--rw-r--r--   0        0        0     3093 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/.gitignore
--rw-r--r--   0        0        0    11578 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/__init__.py
--rw-r--r--   0        0        0      219 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/config.py
--rw-r--r--   0        0        0     1045 2023-06-23 16:21:37.742993 nonebot_plugin_helltide-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-23 16:38:11.592182 nonebot_plugin_helltide-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2598 2023-06-23 16:38:11.592182 nonebot_plugin_helltide-0.1.4/README.md
+-rw-r--r--   0        0        0     3093 2023-06-23 16:38:11.592182 nonebot_plugin_helltide-0.1.4/nonebot_plugin_helltide/.gitignore
+-rw-r--r--   0        0        0    11574 2023-06-23 16:38:11.592182 nonebot_plugin_helltide-0.1.4/nonebot_plugin_helltide/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-23 16:38:11.592182 nonebot_plugin_helltide-0.1.4/nonebot_plugin_helltide/config.py
+-rw-r--r--   0        0        0     1045 2023-06-23 16:38:18.868161 nonebot_plugin_helltide-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_helltide-0.1.3/LICENSE` & `nonebot_plugin_helltide-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.3/README.md` & `nonebot_plugin_helltide-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/.gitignore` & `nonebot_plugin_helltide-0.1.4/nonebot_plugin_helltide/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/__init__.py` & `nonebot_plugin_helltide-0.1.4/nonebot_plugin_helltide/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import datetime
 
 __plugin_meta__ = PluginMetadata(
     name="helltide",
     description="一个Diablo4的helltide和世界boss的提醒小助手",
     # BEGIN: 7d7f3c7b5d4a
     usage="这是一个diablo4插件，可以订阅游戏中的事件，如boss刷新、地狱潮汐等，\n当事件即将发生时会自动提醒订阅用户。使用方法：\n1. 订阅事件：d4订阅 boss/helltide\n2. 取消订阅事件：d4取消订阅 boss/helltide\n3. 查询订阅列表：d4查询订阅",
-    type="application",
+    type="library",
     config=Config,
     # END: 7d7f3c7b5d4a
     extra={"author": "qbkira"},
 )
 
 my_config = Config.parse_obj(get_driver().config)
```

### Comparing `nonebot_plugin_helltide-0.1.3/pyproject.toml` & `nonebot_plugin_helltide-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "nonebot-plugin-helltide"
-version = "0.1.3"
+version = "0.1.4"
 description = "Diablo 4 Helltide Event Tracker work with nonebot2"
 authors = [
     { name = "qbkira", email = "qbuouo@gmail.com" },
 ]
 dependencies = [
     "nonebot2",
     "nonebot2[fastapi]",
```

### Comparing `nonebot_plugin_helltide-0.1.3/PKG-INFO` & `nonebot_plugin_helltide-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helltide
-Version: 0.1.3
+Version: 0.1.4
 Summary: Diablo 4 Helltide Event Tracker work with nonebot2
 Home-page: https://github.com/QBkira/nonebot-plugin-helltide
 Author-Email: qbkira <qbuouo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/QBkira/nonebot-plugin-helltide
 Project-URL: Repository, https://github.com/QBkira/nonebot-plugin-helltide/tree/master/nonebot_plugin_helltide
 Project-URL: Documentation, https://github.com/QBkira/nonebot-plugin-helltide#readme
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.4 Summary:
 Diablo 4 Helltide Event Tracker work with nonebot2 Home-page: https://
 github.com/QBkira/nonebot-plugin-helltide Author-Email: qbkira
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/QBkira/
 nonebot-plugin-helltide Project-URL: Repository, https://github.com/QBkira/
 nonebot-plugin-helltide/tree/master/nonebot_plugin_helltide Project-URL:
 Documentation, https://github.com/QBkira/nonebot-plugin-helltide#readme
 Requires-Python: >=3.8 Requires-Dist: nonebot2 Requires-Dist: nonebot2[fastapi]
```

