# Comparing `tmp/nonebot_plugin_al-0.3.6.tar.gz` & `tmp/nonebot_plugin_al-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.7.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.6.tar` & `nonebot_plugin_al-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/LICENSE
--rw-r--r--   0        0        0     4218 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/README.md
--rw-r--r--   0        0        0     6408 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    70845 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3348 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0     1961 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/config.py
--rw-r--r--   0        0        0    69109 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10142 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7691 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13688 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     5792 2023-06-23 05:01:03.628173 nonebot_plugin_al-0.3.6/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1055 2023-06-23 05:01:03.632173 nonebot_plugin_al-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/LICENSE
+-rw-r--r--   0        0        0     4218 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/README.md
+-rw-r--r--   0        0        0     6408 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    70845 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3283 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0     1878 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/config.py
+-rw-r--r--   0        0        0    69109 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10142 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7691 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13688 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5792 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1101 2023-06-23 05:12:38.612160 nonebot_plugin_al-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.7/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.6/LICENSE` & `nonebot_plugin_al-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/README.md` & `nonebot_plugin_al-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/bili.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import asyncio
 from bs4 import BeautifulSoup
 from pathlib import Path
 import time
 
-from nonebot import require
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import (
     html_to_pic,
 )
-require("nonebot_plugin_htmlrender")
 
 
 from .api import get_data
 
 async def jinghao(tag):
     data = await get_data('https://wiki.biligame.com/blhx/井号碧蓝榜合集')
     soup = BeautifulSoup(data, 'html.parser')
```

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/config.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,14 @@
         self.save()
 
     @property
     def config_list(self) -> List[str]:
         return list(self.config.dict(by_alias=True).keys())
 
     def save(self):
-        if not os.path.exists("./data/al/"):
-            os.makedirs("./data/al/")
         with self.file_path.open('w', encoding='utf-8') as f:
             yaml.dump(
                 self.config.dict(by_alias=True),
                 f,
                 indent=2,
                 Dumper=yaml.RoundTripDumper,
                 allow_unicode=True)
```

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/send_message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.7/nonebot_plugin_al/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.6/pyproject.toml` & `nonebot_plugin_al-0.3.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.6"
+version = "0.3.7"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_al-0.3.6/PKG-INFO` & `nonebot_plugin_al-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.6
+Version: 0.3.7
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
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.6 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.7 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

