# Comparing `tmp/herta_villa_sdk-0.2.0.tar.gz` & `tmp/herta_villa_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.2.0.tar", last modified: Wed Jun 21 17:12:13 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.3.0.tar", last modified: Fri Jun 23 09:38:37 2023, max compression
```

## Comparing `herta_villa_sdk-0.2.0.tar` & `herta_villa_sdk-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/LICENSE
--rw-r--r--   0        0        0      112 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/README.md
--rw-r--r--   0        0        0      555 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/__init__.py
--rw-r--r--   0        0        0     7197 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/bot.py
--rw-r--r--   0        0        0     4505 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/event.py
--rw-r--r--   0        0        0      738 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/exception.py
--rw-r--r--   0        0        0        0 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/handle.py
--rw-r--r--   0        0        0      353 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     1060 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1466 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/image.py
--rw-r--r--   0        0        0      594 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/post.py
--rw-r--r--   0        0        0     6188 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/text.py
--rw-r--r--   0        0        0      162 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/message/types.py
--rw-r--r--   0        0        0     2372 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/model.py
--rw-r--r--   0        0        0     2912 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/server.py
--rw-r--r--   0        0        0      558 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-06-21 17:11:41.964587 herta_villa_sdk-0.2.0/hertavilla/version.py
--rw-r--r--   0        0        0     1616 2023-06-21 17:12:13.792804 herta_villa_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 herta_villa_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2039 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0      555 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/__init__.py
+-rw-r--r--   0        0        0    11217 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/bot.py
+-rw-r--r--   0        0        0     4833 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/event.py
+-rw-r--r--   0        0        0      738 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     1761 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1617 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/image.py
+-rw-r--r--   0        0        0      981 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6095 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/text.py
+-rw-r--r--   0        0        0      369 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/message/types.py
+-rw-r--r--   0        0        0     2372 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/model.py
+-rw-r--r--   0        0        0     2932 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/server.py
+-rw-r--r--   0        0        0      558 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-06-23 09:38:03.456908 herta_villa_sdk-0.3.0/hertavilla/version.py
+-rw-r--r--   0        0        0     1986 2023-06-23 09:38:37.121166 herta_villa_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 herta_villa_sdk-0.3.0/PKG-INFO
```

### Comparing `herta_villa_sdk-0.2.0/LICENSE` & `herta_villa_sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.2.0/hertavilla/__init__.py` & `herta_villa_sdk-0.3.0/hertavilla/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.2.0/hertavilla/event.py` & `herta_villa_sdk-0.3.0/hertavilla/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,28 @@
     created_at: int
     """事件创建时间"""
     id: str
     """事件 id"""
     send_at: int
     """事件回调时间"""
 
+    @property
+    def villa_id(self) -> int:
+        return self.robot.villa_id
+
     def __init_subclass__(cls: Type[Self]) -> None:
         super().__init_subclass__()
-        type_: int = eval(cls.__annotations__["type"]).__args__[0]  # 获取类型
+        literal = cls.__annotations__["type"]
+        type_: int = (
+            eval(cls.__annotations__["type"])
+            if isinstance(literal, str)
+            else literal
+        ).__args__[
+            0
+        ]  # 获取类型
         name = cls.__name__.replace("Event", "")  # 获取名称
         events[type_] = cls, name
 
 
 # JoinVilla
 
 
@@ -172,14 +183,18 @@
     bot_msg_id: str | None
     """如果被回复的消息从属于机器人，则该字段不为空字符串"""
 
     @validator("content", pre=True)
     def str_to_json(cls, v: Any):
         return json.loads(v)
 
+    @property
+    def message(self) -> MessageChain:
+        return self.content.content
+
 
 def parse_event(payload: dict[str, Any]) -> Event:
     type_: int = payload["type"]
     cls_, name = events[type_]
     data = payload["extend_data"]["EventData"][name]
     payload.pop("extend_data")
     payload |= data
```

### Comparing `herta_villa_sdk-0.2.0/hertavilla/exception.py` & `herta_villa_sdk-0.3.0/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.2.0/hertavilla/message/image.py` & `herta_villa_sdk-0.3.0/hertavilla/message/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
-from typing import Optional, TypedDict, cast
+from typing import TYPE_CHECKING, Optional, TypedDict, cast
 
 from hertavilla.message.types import (
     MsgContent,
     MsgContentInfo,
     _Segment,
 )
 
+if TYPE_CHECKING:
+    from hertavilla.bot import VillaBot
+
 
 # MsgContentInfo for image
 class ImageMsgContentInfo(MsgContentInfo):
     content: ImageMsgContent
 
 
 # Segment for image
@@ -35,14 +38,17 @@
         else:
             raise ValueError(  # noqa: TRY003
                 "Parameter width and height are not both None or int",
             )
         self.url = url
         self.file_size = file_size
 
+    async def get_text(self, _: VillaBot) -> str:
+        return "[图片]"
+
 
 # MsgContent for image
 class ImageMsgContent(MsgContent):
     def __init__(
         self,
         url: str,
         size: Size | None = None,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `herta_villa_sdk-0.2.0/hertavilla/message/text.py` & `herta_villa_sdk-0.3.0/hertavilla/message/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
-import abc
-from typing import Any, Literal, TypedDict, cast
+from typing import TYPE_CHECKING, Any, Literal, TypedDict, cast
 
-from hertavilla.bot import VillaBot
 from hertavilla.message.types import MsgContent, MsgContentInfo, _Segment
 from hertavilla.utils import _c
 
+if TYPE_CHECKING:
+    from hertavilla.bot import VillaBot
+
 entity_types: dict[str, type["_TextEntity"]] = {}
 
 # MsgContentInfo for text
 
 
 class TextMsgContentInfo(MsgContentInfo):
     content: TextMsgContent
@@ -47,24 +48,20 @@
     length: int
     offset: int
 
 
 # Segment for text
 
 
-class _TextEntity(_Segment, abc.ABC):
+class _TextEntity(_Segment):
     type_: str
 
     def __init__(self, **kwargs) -> None:
         ...
 
-    @abc.abstractmethod
-    async def get_text(self, bot: VillaBot) -> str:
-        raise NotImplementedError
-
     def get_mention(self) -> tuple[Literal[1, 2], str] | None:
         return None
 
     def __init_subclass__(cls) -> None:
         if cls.__name__ not in {"Text", "Quote"}:
             entity_types[cls.type_] = cls
         return super().__init_subclass__()
```

### Comparing `herta_villa_sdk-0.2.0/hertavilla/model.py` & `herta_villa_sdk-0.3.0/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.2.0/hertavilla/server.py` & `herta_villa_sdk-0.3.0/hertavilla/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,16 @@
             (
                 f"[RECV] {event.__class__.__name__} "
                 f"on bot {event.robot.template.name}"
                 f"({event.robot.template.id}) "
                 f"in villa {event.robot.villa_id}"
             ),
         )
-        if bot.name is None:
-            bot.name = event.robot.template.name
+        if bot._bot_info is None:  # noqa: SLF001
+            bot.bot_info = event.robot.template
         try:
             task = asyncio.create_task(bot.handle_event(event))
             background_tasks.add(task)
             task.add_done_callback(background_tasks.discard)
             return web.json_response({"message": "", "retcode": 0})
         except Exception:
             logger.exception("Raised exceptions while handling event.")
```

### Comparing `herta_villa_sdk-0.2.0/hertavilla/utils.py` & `herta_villa_sdk-0.3.0/hertavilla/utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.2.0/pyproject.toml` & `herta_villa_sdk-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 [project]
 name = "herta-villa-sdk"
-version = "0.2.0"
+version = "0.3.0"
 description = "大别野「黑塔」Python SDK"
 authors = [
     { name = "MingxuanGame", email = "MingxuanGame@outlook.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.4",
     "pydantic>=1.10.8",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
+keywords = [
+    "mihoyo",
+    "miyoushe",
+    "bot",
+    "villa",
+]
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+Homepage = "https://github.com/MingxuanGame/Herta-villa-SDK"
+Documentation = "https://github.com/MingxuanGame/Herta-villa-SDK"
+Repository = "https://github.com/MingxuanGame/Herta-villa-SDK"
+"Bug Tracker" = "https://github.com/MingxuanGame/Herta-villa-SDK/issues"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
@@ -56,14 +68,16 @@
     "A",
     "B",
     "ASYNC",
 ]
 allowed-confusables = [
     "，",
     "。",
+    "（",
+    "）",
 ]
 
 [tool.ruff.isort]
 force-sort-within-sections = true
 extra-standard-library = [
     "typing_extensions",
 ]
```

