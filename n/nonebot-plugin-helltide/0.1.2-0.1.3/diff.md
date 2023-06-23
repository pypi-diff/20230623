# Comparing `tmp/nonebot_plugin_helltide-0.1.2.tar.gz` & `tmp/nonebot_plugin_helltide-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_helltide-0.1.2.tar", last modified: Fri Jun 23 16:08:38 2023, max compression
+gzip compressed data, was "nonebot_plugin_helltide-0.1.3.tar", last modified: Fri Jun 23 16:21:37 2023, max compression
```

## Comparing `nonebot_plugin_helltide-0.1.2.tar` & `nonebot_plugin_helltide-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/LICENSE
--rw-r--r--   0        0        0     2598 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/README.md
--rw-r--r--   0        0        0     3093 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/.gitignore
--rw-r--r--   0        0        0    11578 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/__init__.py
--rw-r--r--   0        0        0      219 2023-06-23 16:08:27.885153 nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/config.py
--rw-r--r--   0        0        0      790 2023-06-23 16:08:38.721228 nonebot_plugin_helltide-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2598 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/README.md
+-rw-r--r--   0        0        0     3093 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/.gitignore
+-rw-r--r--   0        0        0    11578 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-23 16:21:30.022890 nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/config.py
+-rw-r--r--   0        0        0     1045 2023-06-23 16:21:37.742993 nonebot_plugin_helltide-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 nonebot_plugin_helltide-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_helltide-0.1.2/LICENSE` & `nonebot_plugin_helltide-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.2/README.md` & `nonebot_plugin_helltide-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/.gitignore` & `nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.2/nonebot_plugin_helltide/__init__.py` & `nonebot_plugin_helltide-0.1.3/nonebot_plugin_helltide/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helltide-0.1.2/pyproject.toml` & `nonebot_plugin_helltide-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "nonebot-plugin-helltide"
-version = "0.1.2"
+version = "0.1.3"
 description = "Diablo 4 Helltide Event Tracker work with nonebot2"
 authors = [
     { name = "qbkira", email = "qbuouo@gmail.com" },
 ]
 dependencies = [
     "nonebot2",
     "nonebot2[fastapi]",
@@ -37,7 +37,12 @@
     "nonebot-plugin-apscheduler",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
+
+[project.urls]
+homepage = "https://github.com/QBkira/nonebot-plugin-helltide"
+repository = "https://github.com/QBkira/nonebot-plugin-helltide/tree/master/nonebot_plugin_helltide"
+documentation = "https://github.com/QBkira/nonebot-plugin-helltide#readme"
```

### Comparing `nonebot_plugin_helltide-0.1.2/PKG-INFO` & `nonebot_plugin_helltide-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helltide
-Version: 0.1.2
+Version: 0.1.3
 Summary: Diablo 4 Helltide Event Tracker work with nonebot2
+Home-page: https://github.com/QBkira/nonebot-plugin-helltide
 Author-Email: qbkira <qbuouo@gmail.com>
 License: MIT
+Project-URL: Homepage, https://github.com/QBkira/nonebot-plugin-helltide
+Project-URL: Repository, https://github.com/QBkira/nonebot-plugin-helltide/tree/master/nonebot_plugin_helltide
+Project-URL: Documentation, https://github.com/QBkira/nonebot-plugin-helltide#readme
 Requires-Python: >=3.8
 Requires-Dist: nonebot2
 Requires-Dist: nonebot2[fastapi]
 Requires-Dist: pydantic
 Requires-Dist: aiohttp
 Requires-Dist: aiofiles
 Requires-Dist: httpx
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.2 Summary:
-Diablo 4 Helltide Event Tracker work with nonebot2 Author-Email: qbkira
-gmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2
-Requires-Dist: nonebot2[fastapi] Requires-Dist: pydantic Requires-Dist: aiohttp
-Requires-Dist: aiofiles Requires-Dist: httpx Requires-Dist: nonebot-adapter-
-onebot Requires-Dist: nonebot-plugin-apscheduler Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-helltide Version: 0.1.3 Summary:
+Diablo 4 Helltide Event Tracker work with nonebot2 Home-page: https://
+github.com/QBkira/nonebot-plugin-helltide Author-Email: qbkira
+gmail.com> License: MIT Project-URL: Homepage, https://github.com/QBkira/
+nonebot-plugin-helltide Project-URL: Repository, https://github.com/QBkira/
+nonebot-plugin-helltide/tree/master/nonebot_plugin_helltide Project-URL:
+Documentation, https://github.com/QBkira/nonebot-plugin-helltide#readme
+Requires-Python: >=3.8 Requires-Dist: nonebot2 Requires-Dist: nonebot2[fastapi]
+Requires-Dist: pydantic Requires-Dist: aiohttp Requires-Dist: aiofiles
+Requires-Dist: httpx Requires-Dist: nonebot-adapter-onebot Requires-Dist:
+nonebot-plugin-apscheduler Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                         # nonebot-plugin-helltide _â¨
 ä¸ä¸ªDiablo4çhelltideåä¸çbossçæéå°å©æ â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç»
 æ·»å æºå¨äººå°ç¾¤èä¸­ï¼è®¢éä¹åå¨ç¾¤éä¼æéè®¢éBosså·æ°ï¼å°ç±çæ½®æéï¼ï¼è¿æåå¢çå·æ°æ¶é´ï¼
```

