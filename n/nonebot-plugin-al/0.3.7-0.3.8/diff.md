# Comparing `tmp/nonebot_plugin_al-0.3.7.tar.gz` & `tmp/nonebot_plugin_al-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.8.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.7.tar` & `nonebot_plugin_al-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/LICENSE
--rw-r--r--   0        0        0     4218 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/README.md
--rw-r--r--   0        0        0     6408 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    70845 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3283 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0     1878 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/config.py
--rw-r--r--   0        0        0    69109 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10142 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7691 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13688 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     5792 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1101 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-23 14:38:05.053306 nonebot_plugin_al-0.3.8/LICENSE
+-rw-r--r--   0        0        0     4218 2023-06-23 14:38:05.053306 nonebot_plugin_al-0.3.8/README.md
+-rw-r--r--   0        0        0     6408 2023-06-23 14:38:05.053306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    70845 2023-06-23 14:38:05.053306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3283 2023-06-23 14:38:05.053306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0     1878 2023-06-23 14:38:05.053306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/config.py
+-rw-r--r--   0        0        0    69109 2023-06-23 14:38:05.057306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-23 14:38:05.057306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10142 2023-06-23 14:38:05.057306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7691 2023-06-23 14:38:05.057306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13688 2023-06-23 14:38:05.057306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5792 2023-06-23 14:38:05.057306 nonebot_plugin_al-0.3.8/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1119 2023-06-23 14:38:05.057306 nonebot_plugin_al-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.8/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.7/LICENSE` & `nonebot_plugin_al-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/README.md` & `nonebot_plugin_al-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/config.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/send_message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.8/nonebot_plugin_al/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.7/pyproject.toml` & `nonebot_plugin_al-0.3.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.7"
+version = "0.3.8"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
@@ -23,14 +23,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.2.1"
 nonebot_plugin_htmlrender = "^0.2.0.3"
 aiohttp = ">=3.8.3"
+pillow = "^9.5.0"
 bs4 = "^0.0.1"
 aiofiles = "^23.1.0"
 pypinyin = "^0.49.0"
 imgkit = "^1.2.3"
 opencv-python = "^4.7.0"
 "ruamel.yaml" = "^0.17.21"
```

### Comparing `nonebot_plugin_al-0.3.7/PKG-INFO` & `nonebot_plugin_al-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.7
+Version: 0.3.8
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -19,14 +19,15 @@
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: imgkit (>=1.2.3,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0)
 Requires-Dist: opencv-python (>=4.7.0,<5.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pypinyin (>=0.49.0,<0.50.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.7 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.8 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
 Dist: aiohttp (>=3.8.3) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist:
 imgkit (>=1.2.3,<2.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
 nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist: opencv-python
-(>=4.7.0,<5.0.0) Requires-Dist: pypinyin (>=0.49.0,<0.50.0) Requires-Dist:
-ruamel.yaml (>=0.17.21,<0.18.0) Project-URL: Repository, https://github.com/
-Agnes4m/nonebot_plugin_AL Description-Content-Type: text/markdown
+(>=4.7.0,<5.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
+pypinyin (>=0.49.0,<0.50.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
+Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_al 0.3.0 __â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨__ [GitHub_stars]
            [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## åè½ 1ãbç«wikiäºå·æ¦ä¸å¾æµ 2ãè°è¹è£å¤å¾é´ 3ã
 (70%å®æ)ç§»æ¤å¤§é¨å[blhx](https://github.com/Gaylone/
 blhx_wiki)ï¼åhoshinoæ¹é¡¹ç®ï¼çå¤§é¨ååè½ ## å®è£
```

