# Comparing `tmp/plutous_trade-0.0.7.tar.gz` & `tmp/plutous_trade-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous_trade-0.0.7.tar", max compression
+gzip compressed data, was "plutous_trade-0.0.9.tar", max compression
```

## Comparing `plutous_trade-0.0.7.tar` & `plutous_trade-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.7/LICENSE
--rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.7/README.md
--rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.7/plutous/__init__.py
--rw-r--r--   0        0        0       83 2023-06-08 17:53:22.823146 plutous_trade-0.0.7/plutous/trade/__init__.py
--rw-r--r--   0        0        0     3380 2023-05-23 04:04:54.046424 plutous_trade-0.0.7/plutous/trade/alembic.ini
--rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.7/plutous/trade/app/__init__.py
--rw-r--r--   0        0        0     2266 2023-06-05 08:34:15.090392 plutous_trade-0.0.7/plutous/trade/app/main.py
--rw-r--r--   0        0        0     1097 2023-06-05 08:32:07.209117 plutous_trade-0.0.7/plutous/trade/app/models.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:41.262810 plutous_trade-0.0.7/plutous/trade/cli/__init__.py
--rw-r--r--   0        0        0      565 2023-05-21 14:49:47.617177 plutous_trade-0.0.7/plutous/trade/cli/database.py
--rw-r--r--   0        0        0      253 2023-05-16 09:53:06.465010 plutous_trade-0.0.7/plutous/trade/cli/main.py
--rw-r--r--   0        0        0      221 2023-05-22 15:46:21.868004 plutous_trade-0.0.7/plutous/trade/enums/__init__.py
--rw-r--r--   0        0        0       78 2023-05-21 16:59:31.441696 plutous_trade-0.0.7/plutous/trade/enums/action.py
--rw-r--r--   0        0        0      575 2023-05-16 18:35:53.699585 plutous_trade-0.0.7/plutous/trade/enums/asset_type.py
--rw-r--r--   0        0        0       90 2023-05-22 03:47:08.998276 plutous_trade-0.0.7/plutous/trade/enums/bot_type.py
--rw-r--r--   0        0        0      105 2023-06-08 14:42:13.454051 plutous_trade-0.0.7/plutous/trade/enums/position_side.py
--rw-r--r--   0        0        0      111 2023-05-21 18:52:25.169077 plutous_trade-0.0.7/plutous/trade/enums/strategy_direction.py
--rw-r--r--   0        0        0      244 2023-05-21 15:33:24.216798 plutous_trade-0.0.7/plutous/trade/enums/strategy_type.py
--rw-r--r--   0        0        0       38 2023-05-16 07:55:03.225919 plutous_trade-0.0.7/plutous/trade/migrations/README
--rw-r--r--   0        0        0     2252 2023-05-27 03:28:54.379452 plutous_trade-0.0.7/plutous/trade/migrations/env.py
--rw-r--r--   0        0        0      510 2023-05-16 07:55:03.225919 plutous_trade-0.0.7/plutous/trade/migrations/script.py.mako
--rw-r--r--   0        0        0     8199 2023-06-08 14:48:14.391442 plutous_trade-0.0.7/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py
--rw-r--r--   0        0        0      159 2023-05-22 03:55:30.430494 plutous_trade-0.0.7/plutous/trade/models/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-22 15:48:07.454158 plutous_trade-0.0.7/plutous/trade/models/api_key.py
--rw-r--r--   0        0        0      401 2023-05-22 13:39:10.362131 plutous_trade-0.0.7/plutous/trade/models/base.py
--rw-r--r--   0        0        0     1104 2023-06-05 08:20:14.105393 plutous_trade-0.0.7/plutous/trade/models/bot.py
--rw-r--r--   0        0        0      998 2023-05-29 13:29:59.635867 plutous_trade-0.0.7/plutous/trade/models/position.py
--rw-r--r--   0        0        0      647 2023-05-22 13:38:30.726320 plutous_trade-0.0.7/plutous/trade/models/strategy.py
--rw-r--r--   0        0        0      968 2023-05-22 18:41:14.933111 plutous_trade-0.0.7/plutous/trade/models/trade.py
--rw-r--r--   0        0        0      560 2023-06-08 17:53:28.583679 plutous_trade-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 plutous_trade-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.9/LICENSE
+-rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.9/README.md
+-rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.9/plutous/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-08 18:58:25.560164 plutous_trade-0.0.9/plutous/trade/__init__.py
+-rw-r--r--   0        0        0     3380 2023-05-23 04:04:54.046424 plutous_trade-0.0.9/plutous/trade/alembic.ini
+-rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.9/plutous/trade/app/__init__.py
+-rw-r--r--   0        0        0     2787 2023-06-08 18:02:55.928165 plutous_trade-0.0.9/plutous/trade/app/main.py
+-rw-r--r--   0        0        0     1097 2023-06-05 08:32:07.209117 plutous_trade-0.0.9/plutous/trade/app/models.py
+-rw-r--r--   0        0        0        0 2023-05-16 09:19:41.262810 plutous_trade-0.0.9/plutous/trade/cli/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-21 14:49:47.617177 plutous_trade-0.0.9/plutous/trade/cli/database.py
+-rw-r--r--   0        0        0      253 2023-05-16 09:53:06.465010 plutous_trade-0.0.9/plutous/trade/cli/main.py
+-rw-r--r--   0        0        0      221 2023-05-22 15:46:21.868004 plutous_trade-0.0.9/plutous/trade/enums/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-21 16:59:31.441696 plutous_trade-0.0.9/plutous/trade/enums/action.py
+-rw-r--r--   0        0        0      575 2023-05-16 18:35:53.699585 plutous_trade-0.0.9/plutous/trade/enums/asset_type.py
+-rw-r--r--   0        0        0       90 2023-05-22 03:47:08.998276 plutous_trade-0.0.9/plutous/trade/enums/bot_type.py
+-rw-r--r--   0        0        0      105 2023-06-08 14:42:13.454051 plutous_trade-0.0.9/plutous/trade/enums/position_side.py
+-rw-r--r--   0        0        0      111 2023-05-21 18:52:25.169077 plutous_trade-0.0.9/plutous/trade/enums/strategy_direction.py
+-rw-r--r--   0        0        0      244 2023-05-21 15:33:24.216798 plutous_trade-0.0.9/plutous/trade/enums/strategy_type.py
+-rw-r--r--   0        0        0       38 2023-05-16 07:55:03.225919 plutous_trade-0.0.9/plutous/trade/migrations/README
+-rw-r--r--   0        0        0     2252 2023-05-27 03:28:54.379452 plutous_trade-0.0.9/plutous/trade/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-05-16 07:55:03.225919 plutous_trade-0.0.9/plutous/trade/migrations/script.py.mako
+-rw-r--r--   0        0        0     8199 2023-06-08 14:48:14.391442 plutous_trade-0.0.9/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py
+-rw-r--r--   0        0        0      159 2023-05-22 03:55:30.430494 plutous_trade-0.0.9/plutous/trade/models/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-22 15:48:07.454158 plutous_trade-0.0.9/plutous/trade/models/api_key.py
+-rw-r--r--   0        0        0      401 2023-05-22 13:39:10.362131 plutous_trade-0.0.9/plutous/trade/models/base.py
+-rw-r--r--   0        0        0     1104 2023-06-05 08:20:14.105393 plutous_trade-0.0.9/plutous/trade/models/bot.py
+-rw-r--r--   0        0        0      998 2023-05-29 13:29:59.635867 plutous_trade-0.0.9/plutous/trade/models/position.py
+-rw-r--r--   0        0        0      647 2023-05-22 13:38:30.726320 plutous_trade-0.0.9/plutous/trade/models/strategy.py
+-rw-r--r--   0        0        0      968 2023-05-22 18:41:14.933111 plutous_trade-0.0.9/plutous/trade/models/trade.py
+-rw-r--r--   0        0        0      560 2023-06-08 18:58:31.016668 plutous_trade-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 plutous_trade-0.0.9/PKG-INFO
```

### Comparing `plutous_trade-0.0.7/LICENSE` & `plutous_trade-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/alembic.ini` & `plutous_trade-0.0.9/plutous/trade/alembic.ini`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/app/main.py` & `plutous_trade-0.0.9/plutous/trade/app/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi import Depends, FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from sqlalchemy.orm import Session
 
 from plutous.app.utils.session import get_session
-from plutous.trade.models import ApiKey, Bot, Strategy
+from plutous.trade.models import ApiKey, Bot, Position, Strategy, Trade
 
 from .models import ApiKeyPost, BotGet, BotPatch, BotPost, StrategyPost
 
 app = FastAPI(
     title="Plutous Trade API",
     version="0.0.1",
 )
@@ -89,7 +89,23 @@
     bot = session.query(Bot).filter(Bot.id == bot_id).first()
 
     for key, value in bot_patch.dict().items():
         if value is not None:
             setattr(bot, key, value)
     session.commit()
     return bot_patch
+
+
+@app.delete("/bot/{bot_id}")
+def delete_bot(
+    bot_id: int,
+    session: Session = Depends(get_session),
+):
+    session.query(Trade).filter(
+        Trade.position_id == Position.id, Position.bot_id == bot_id
+    ).delete(synchronize_session=False)
+    session.query(Position).filter(Position.bot_id == bot_id).delete(
+        synchronize_session=False
+    )
+    session.query(Bot).filter(Bot.id == bot_id).delete(synchronize_session=False)
+    session.commit()
+    return {"message": "Bot deleted"}
```

### Comparing `plutous_trade-0.0.7/plutous/trade/app/models.py` & `plutous_trade-0.0.9/plutous/trade/app/models.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/cli/database.py` & `plutous_trade-0.0.9/plutous/trade/cli/database.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/enums/asset_type.py` & `plutous_trade-0.0.9/plutous/trade/enums/asset_type.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/migrations/env.py` & `plutous_trade-0.0.9/plutous/trade/migrations/env.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py` & `plutous_trade-0.0.9/plutous/trade/migrations/versions/2023-05-23_03-57_3e037c0f4152_init.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/models/api_key.py` & `plutous_trade-0.0.9/plutous/trade/models/api_key.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/models/bot.py` & `plutous_trade-0.0.9/plutous/trade/models/bot.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/models/position.py` & `plutous_trade-0.0.9/plutous/trade/models/position.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/models/strategy.py` & `plutous_trade-0.0.9/plutous/trade/models/strategy.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/plutous/trade/models/trade.py` & `plutous_trade-0.0.9/plutous/trade/models/trade.py`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.7/pyproject.toml` & `plutous_trade-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous-trade"
-version = "0.0.7"
+version = "0.0.9"
 description = "Plutous Trading Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous_trade-0.0.7/PKG-INFO` & `plutous_trade-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutous-trade
-Version: 0.0.7
+Version: 0.0.9
 Summary: Plutous Trading Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

