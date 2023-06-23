# Comparing `tmp/lightning_rod-0.2.2.tar.gz` & `tmp/lightning_rod-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_rod-0.2.2.tar", max compression
+gzip compressed data, was "lightning_rod-0.2.3.tar", max compression
```

## Comparing `lightning_rod-0.2.2.tar` & `lightning_rod-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1061 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/LICENSE
--rw-r--r--   0        0        0      347 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/README.md
--rw-r--r--   0        0        0      307 2023-05-31 12:31:47.509746 lightning_rod-0.2.2/lightning_rod/__init__.py
--rw-r--r--   0        0        0      667 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/advancement.bolt
--rw-r--r--   0        0        0      565 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/api.bolt
--rw-r--r--   0        0        0     4574 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/bossbar.bolt
--rw-r--r--   0        0        0       38 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/cancel_momentum.bolt
--rw-r--r--   0        0        0      314 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/clear.bolt
--rw-r--r--   0        0        0       85 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/comment.bolt
--rw-r--r--   0        0        0      144 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/config.bolt
--rw-r--r--   0        0        0     1593 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/effect.bolt
--rw-r--r--   0        0        0      581 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/gamemode.bolt
--rw-r--r--   0        0        0      157 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/give.bolt
--rw-r--r--   0        0        0       25 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/kill.bolt
--rw-r--r--   0        0        0     2418 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/math.bolt
--rw-r--r--   0        0        0       35 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/raw_cmd.bolt
--rw-r--r--   0        0        0       86 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/tag.bolt
--rw-r--r--   0        0        0     1047 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/time.bolt
--rw-r--r--   0        0        0      300 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/utils.bolt
--rw-r--r--   0        0        0     2111 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/modules/xp.bolt
--rw-r--r--   0        0        0        0 2023-05-31 12:30:58.440086 lightning_rod-0.2.2/lightning_rod/py.typed
--rw-r--r--   0        0        0     1242 2023-05-31 12:31:47.525747 lightning_rod-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 lightning_rod-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-23 07:04:03.462174 lightning_rod-0.2.3/LICENSE
+-rw-r--r--   0        0        0      347 2023-06-23 07:04:03.462174 lightning_rod-0.2.3/README.md
+-rw-r--r--   0        0        0      307 2023-06-23 07:05:07.371057 lightning_rod-0.2.3/lightning_rod/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/advancement.bolt
+-rw-r--r--   0        0        0      566 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/api.bolt
+-rw-r--r--   0        0        0     4574 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/bossbar.bolt
+-rw-r--r--   0        0        0       38 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/cancel_momentum.bolt
+-rw-r--r--   0        0        0      314 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/clear.bolt
+-rw-r--r--   0        0        0       85 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/comment.bolt
+-rw-r--r--   0        0        0      144 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/config.bolt
+-rw-r--r--   0        0        0     1593 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/effect.bolt
+-rw-r--r--   0        0        0      581 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/gamemode.bolt
+-rw-r--r--   0        0        0      157 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/give.bolt
+-rw-r--r--   0        0        0       25 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/kill.bolt
+-rw-r--r--   0        0        0     2418 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/math.bolt
+-rw-r--r--   0        0        0       35 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/raw_cmd.bolt
+-rw-r--r--   0        0        0       86 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/tag.bolt
+-rw-r--r--   0        0        0     1047 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/time.bolt
+-rw-r--r--   0        0        0      300 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/utils.bolt
+-rw-r--r--   0        0        0     2142 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/modules/xp.bolt
+-rw-r--r--   0        0        0        0 2023-06-23 07:04:03.466174 lightning_rod-0.2.3/lightning_rod/py.typed
+-rw-r--r--   0        0        0     1242 2023-06-23 07:05:07.391058 lightning_rod-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 lightning_rod-0.2.3/PKG-INFO
```

### Comparing `lightning_rod-0.2.2/LICENSE` & `lightning_rod-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/advancement.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/advancement.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/api.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/api.bolt`

 * *Files 0% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 from ./give import give
 from ./clear import clear
 from ./gamemode import get_gamemode, set_gamemode
 from ./math import random, sqrt, pow
 from ./time import get_gametime, get_time, get_day, set_time
 from ./xp import get_xp, get_level, set_xp, set_level, set_xp_percent
 from ./comment import add_comment
+
```

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/bossbar.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/bossbar.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/effect.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/effect.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/gamemode.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/gamemode.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/math.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/math.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/time.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/time.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.2/lightning_rod/modules/xp.bolt` & `lightning_rod-0.2.3/lightning_rod/modules/xp.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
             xp query @s levels
 
     return output
 
 def _set_xp_from_expression(amount: ExpressionNode, mode: str):
     amt = StaticVar(Int)
 
+    raw_cmd(f"xp set @s 0 {mode}")
     amt = amount
-    
+
     execute function f"{_WORKING_DIR}/set_{mode}":
         for n in binary_progression(28, reversed=True):
             if amt >= n:
                 execute function f"{_WORKING_DIR}/set_{mode}/{n}":
                     amt -= n
                     raw_cmd(f"xp add @s {n} {mode}")
```

### Comparing `lightning_rod-0.2.2/pyproject.toml` & `lightning_rod-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning_rod"
-version = "0.2.2"
+version = "0.2.3"
 description = "Function library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/lightning-rod"
 readme = "README.md"
```

### Comparing `lightning_rod-0.2.2/PKG-INFO` & `lightning_rod-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-rod
-Version: 0.2.2
+Version: 0.2.3
 Summary: Function library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/lightning-rod
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

