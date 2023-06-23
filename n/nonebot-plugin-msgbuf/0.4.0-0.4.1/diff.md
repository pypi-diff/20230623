# Comparing `tmp/nonebot-plugin-msgbuf-0.4.0.tar.gz` & `tmp/nonebot-plugin-msgbuf-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-msgbuf-0.4.0.tar", last modified: Fri Jun 23 08:50:31 2023, max compression
+gzip compressed data, was "nonebot-plugin-msgbuf-0.4.1.tar", last modified: Fri Jun 23 09:33:52 2023, max compression
```

## Comparing `nonebot-plugin-msgbuf-0.4.0.tar` & `nonebot-plugin-msgbuf-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:50:31.204234 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    23081 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:33:52.212684 nonebot-plugin-msgbuf-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-23 09:33:52.212684 nonebot-plugin-msgbuf-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:33:52.208684 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23081 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:33:52.212684 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-23 09:33:52.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 09:33:52.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:33:52.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 09:33:52.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 09:33:52.000000 nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-23 09:33:41.000000 nonebot-plugin-msgbuf-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:33:52.212684 nonebot-plugin-msgbuf-0.4.1/setup.cfg
```

### Comparing `nonebot-plugin-msgbuf-0.4.0/LICENSE` & `nonebot-plugin-msgbuf-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.4.0/PKG-INFO` & `nonebot-plugin-msgbuf-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.4.0
+Version: 0.4.1
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-plugin-msgbuf-0.4.0/README.md` & `nonebot-plugin-msgbuf-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/__init__.py` & `nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     or (_suf.startswith("rc") and int(_suf[2:]) > 4)
 ):
     _extra_meta = _extra_meta_source
 else:
     _extra_meta = {"extra": _extra_meta_source}
 
 __plugin_meta__ = PluginMetadata(
-    name="不雅信达",
+    name="雅信达",
     description="适用于 NoneBot2 插件的被动消息构造集成",
     usage="无",
     **_extra_meta
 )
 
 
 class MessageBuffer(Generic[_BotT, _EventT], MsgBufManager):
```

### Comparing `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/base.py` & `nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/base.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/models.py` & `nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/models.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/platforms.py` & `nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/platforms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/utils.py` & `nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO` & `nonebot-plugin-msgbuf-0.4.1/nonebot_plugin_msgbuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.4.0
+Version: 0.4.1
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

