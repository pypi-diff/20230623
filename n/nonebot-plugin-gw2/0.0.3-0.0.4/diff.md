# Comparing `tmp/nonebot_plugin_gw2-0.0.3.tar.gz` & `tmp/nonebot_plugin_gw2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gw2-0.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_gw2-0.0.4.tar", max compression
```

## Comparing `nonebot_plugin_gw2-0.0.3.tar` & `nonebot_plugin_gw2-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/LICENSE
--rw-r--r--   0        0        0     1714 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/README.md
--rw-r--r--   0        0        0     3572 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/__init__.py
--rw-r--r--   0        0        0     2704 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/api.py
--rw-r--r--   0        0        0      949 2023-06-21 02:18:27.749967 nonebot_plugin_gw2-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 nonebot_plugin_gw2-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-23 05:32:05.765766 nonebot_plugin_gw2-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1714 2023-06-23 05:32:05.765766 nonebot_plugin_gw2-0.0.4/README.md
+-rw-r--r--   0        0        0     3572 2023-06-23 05:32:05.765766 nonebot_plugin_gw2-0.0.4/nonebot_plugin_gw2/__init__.py
+-rw-r--r--   0        0        0     2704 2023-06-23 05:32:05.765766 nonebot_plugin_gw2-0.0.4/nonebot_plugin_gw2/api.py
+-rw-r--r--   0        0        0      949 2023-06-23 05:32:05.765766 nonebot_plugin_gw2-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 nonebot_plugin_gw2-0.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_gw2-0.0.3/LICENSE` & `nonebot_plugin_gw2-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gw2-0.0.3/README.md` & `nonebot_plugin_gw2-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_gw2//issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_gw2" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
         <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_gw2">
-        <img src="https://img.shields.io/pypi/v/nonebot_plugin_gw2/.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-gw2">
+        <img src="https://img.shields.io/pypi/v/nonebot-plugin-gw2/.svg" alt="pypi">
 </a>
     <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
 ## 安装
```

### Comparing `nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/__init__.py` & `nonebot_plugin_gw2-0.0.4/nonebot_plugin_gw2/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gw2-0.0.3/nonebot_plugin_gw2/api.py` & `nonebot_plugin_gw2-0.0.4/nonebot_plugin_gw2/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gw2-0.0.3/pyproject.toml` & `nonebot_plugin_gw2-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "nonebot-plugin-gw2"
-version = "0.0.3"
+name = "nonebot_plugin_gw2"
+version = "0.0.4"
 description = "gw2 plugin for NoneBot"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_gw2"
 repository = "https://github.com/Agnes4m/nonebot_plugin_gw2"
 keywords = ["game", "gw2", "nonebot2", "plugin"]
@@ -22,13 +22,13 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = ">=2.1.5"
 asyncio = ">=3.4.3"
-httpx = ">=0.23.3"
+httpx = ">=0.22.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_gw2-0.0.3/PKG-INFO` & `nonebot_plugin_gw2-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gw2
-Version: 0.0.3
+Version: 0.0.4
 Summary: gw2 plugin for NoneBot
 Home-page: https://github.com/Agnes4m/nonebot_plugin_gw2
 License: MIT
 Keywords: game,gw2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3)
-Requires-Dist: httpx (>=0.23.3)
+Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_gw2
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
@@ -39,16 +39,16 @@
 </a>
 <a href="https://github.com/Agnes4m/nonebot_plugin_gw2//issues">
         <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_gw2" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
         <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
 </a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_gw2">
-        <img src="https://img.shields.io/pypi/v/nonebot_plugin_gw2/.svg" alt="pypi">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-gw2">
+        <img src="https://img.shields.io/pypi/v/nonebot-plugin-gw2/.svg" alt="pypi">
 </a>
     <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0-red.svg" alt="NoneBot">
 </div>
 
 ## 安装
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gw2 Version: 0.0.3 Summary: gw2
+Metadata-Version: 2.1 Name: nonebot-plugin-gw2 Version: 0.0.4 Summary: gw2
 plugin for NoneBot Home-page: https://github.com/Agnes4m/nonebot_plugin_gw2
 License: MIT Keywords: game,gw2,nonebot2,plugin Author: Agnes_Digital Author-
 email: Z735803792@163.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: asyncio (>=3.4.3) Requires-Dist: httpx (>=0.23.3) Requires-Dist: nonebot-
+Dist: asyncio (>=3.4.3) Requires-Dist: httpx (>=0.22.0) Requires-Dist: nonebot-
 adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Project-URL:
 Repository, https://github.com/Agnes4m/nonebot_plugin_gw2 Description-Content-
 Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_gw2 _â¨æ¿æ2 æå²¬å²æ¥è¯¢â¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
```

