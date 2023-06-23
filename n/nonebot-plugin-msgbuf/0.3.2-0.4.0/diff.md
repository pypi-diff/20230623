# Comparing `tmp/nonebot-plugin-msgbuf-0.3.2.tar.gz` & `tmp/nonebot-plugin-msgbuf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-msgbuf-0.3.2.tar", last modified: Mon Jun 19 08:03:36 2023, max compression
+gzip compressed data, was "nonebot-plugin-msgbuf-0.4.0.tar", last modified: Fri Jun 23 08:50:31 2023, max compression
```

## Comparing `nonebot-plugin-msgbuf-0.3.2.tar` & `nonebot-plugin-msgbuf-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 08:03:36.000000 nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-19 08:03:25.000000 nonebot-plugin-msgbuf-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:03:36.260136 nonebot-plugin-msgbuf-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:50:31.204234 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23081 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 08:50:31.000000 nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-23 08:50:19.000000 nonebot-plugin-msgbuf-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 08:50:31.208235 nonebot-plugin-msgbuf-0.4.0/setup.cfg
```

### Comparing `nonebot-plugin-msgbuf-0.3.2/LICENSE` & `nonebot-plugin-msgbuf-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.2/PKG-INFO` & `nonebot-plugin-msgbuf-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-msgbuf
-Version: 0.3.2
-Summary: 适用于 NoneBot2 插件的被动消息构造集成
-Author-email: HivertMoZara <worldmozara@163.com>
-License: MIT
-Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
-Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 # nonebot-plugin-msgbuf
 
 _✨ 适用于 NoneBot2 插件的被动消息构造集成 ✨_
 
 ~~代码比 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 和 [SegBuilder](https://github.com/Well2333/nonebot-plugin-segbuilder) 好看（不是）~~
@@ -48,32 +36,27 @@
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
 |                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            QQ 频道                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
+|                            Telegram                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
 nb plugin install nonebot-plugin-msgbuf
 ```
 
 ## 使用
 
-> 关于 `require()` 的使用问题：
->
-> NoneBot2 插件的**首次**导入**必须**通过 NoneBot2 自身的方式（包括但不限于 `require()`, `load_plugin()` 等）完成，否则之后使用 NoneBot2 方式导入该插件的插件将**无法**正常工作。
->
-> NoneBot2 插件体系要求**必须**使用 `require()` 加载插件依赖。
-
 ### 竞品对比
 
 这是常规的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
```

### Comparing `nonebot-plugin-msgbuf-0.3.2/README.md` & `nonebot-plugin-msgbuf-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-msgbuf
+Version: 0.4.0
+Summary: 适用于 NoneBot2 插件的被动消息构造集成
+Author-email: HivertMoZara <worldmozara@163.com>
+License: MIT
+Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
+Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 # nonebot-plugin-msgbuf
 
 _✨ 适用于 NoneBot2 插件的被动消息构造集成 ✨_
 
 ~~代码比 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 和 [SegBuilder](https://github.com/Well2333/nonebot-plugin-segbuilder) 好看（不是）~~
@@ -36,32 +48,27 @@
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
 |                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            QQ 频道                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
+|                            Telegram                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
 nb plugin install nonebot-plugin-msgbuf
 ```
 
 ## 使用
 
-> 关于 `require()` 的使用问题：
->
-> NoneBot2 插件的**首次**导入**必须**通过 NoneBot2 自身的方式（包括但不限于 `require()`, `load_plugin()` 等）完成，否则之后使用 NoneBot2 方式导入该插件的插件将**无法**正常工作。
->
-> NoneBot2 插件体系要求**必须**使用 `require()` 加载插件依赖。
-
 ### 竞品对比
 
 这是常规的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
```

### Comparing `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/__init__.py` & `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
     Raw,        Reply,      Share,      Text,       Video,      Voice
 )
 from .platforms import _BotT, _EventT, Specs, find_proxy
 
 _extra_meta_source = {
     "type": "library",
     "homepage": "https://github.com/NCBM/nonebot-plugin-msgbuf",
-    "supported_adapters": {"~onebot.v11", "~onebot.v12", "~qqguild"}
+    "supported_adapters": {"~onebot.v11", "~onebot.v12", "~qqguild", "~telegram"}
 }
 
 if (
     not nbver
     or not nbver.startswith("2.0.0")
     or not (_suf := nbver[5:])
     or _suf[0] not in "abr"
     or (_suf.startswith("rc") and int(_suf[2:]) > 4)
 ):
     _extra_meta = _extra_meta_source
 else:
     _extra_meta = {"extra": _extra_meta_source}
 
 __plugin_meta__ = PluginMetadata(
-    name="信鸽巴夫",
+    name="不雅信达",
     description="适用于 NoneBot2 插件的被动消息构造集成",
     usage="无",
     **_extra_meta
 )
 
 
 class MessageBuffer(Generic[_BotT, _EventT], MsgBufManager):
```

### Comparing `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/base.py` & `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections import deque
-from typing import Union
+from typing import Deque, Union
 
-from nonebot.adapters import Message, MessageSegment
+from nonebot.adapters import MessageSegment
 from .models import (
     Face,               File,               Image,              Location,
     Mention,            Model,              Raw,                Reply,
     Share,              SupportedFileData,  Text,               Video,
     Voice
 )
 
 
 class MsgBufManager:
     def __init__(self) -> None:
-        self.msgbuf = deque()
+        self.msgbuf: Deque[Model] = deque()
 
     def __lshift__(self, __o: Model):
         self.msgbuf.append(__o)
         return self
 
     def add(self, *m: Model):
         """批量插入消息结构"""
@@ -29,15 +29,15 @@
         
         - n: 删除个数
         """
         for _ in range(n):
             self.msgbuf.pop()
         return self
     
-    def raw(self, raw: Union[str, MessageSegment, Message]):
+    def raw(self, raw: Union[str, MessageSegment]):
         """追加原始消息/消息段"""
         self.msgbuf.append(Raw(raw))
         return self
 
     def text(self, text: str):
         """追加普通文本"""
         self.msgbuf.append(Text(text))
```

### Comparing `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/models.py` & `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from io import BytesIO
 from os.path import basename
 from pathlib import Path
-from typing import Literal, Union
+from typing import TYPE_CHECKING, Any, Literal, Optional, Union
 
-from nonebot.adapters import Message, MessageSegment
+from nonebot.adapters import MessageSegment
 
 SupportedFileData = Union[str, Path, bytes, BytesIO]
 
 # -*- stub definitions -*-
 
 
 class Model:
@@ -37,23 +37,24 @@
 
 # -*- end stub definitions -*-
 # -*- common models definitions -*-
 
 
 @dataclass
 class Raw(Mutex):
-    raw: Union[str, Message, MessageSegment]
+    raw: Union[str, MessageSegment]
 
     def alternative(self) -> str:
         return str(self.raw)
 
 
 @dataclass
 class Text(Body):
     text: str
+    rich: Optional[str] = None
 
     def alternative(self) -> str:
         return self.text
 
 
 @dataclass
 class Image(Body):
@@ -80,14 +81,29 @@
         return "[图片]"
 
 
 @dataclass
 class Mention(Body):
     user_id: str
     domain: str = ""
+    if TYPE_CHECKING:
+        from nonebot.adapters.telegram.model import User
+        tg_user: Optional[User] = None
+    else:
+        tg_user: Any = None
+
+    def __post_init__(self) -> None:
+        if self.tg_user is None:
+            return
+        self.user_id = (
+            self.user_id or self.tg_user.username
+            or self.tg_user.first_name
+            if self.tg_user.last_name is None
+            else f"{self.tg_user.first_name} {self.tg_user.last_name}"
+        )
 
     def alternative(self) -> str:
         return f"@{self.user_id} "
 
 
 @dataclass
 class Reply(Single):
```

### Comparing `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/platforms.py` & `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/platforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import asyncio
 from collections import deque
 from contextlib import suppress
 from io import BytesIO
 from pathlib import Path
 from types import TracebackType
-from typing import Any, Deque, Generic, List, Literal, NoReturn, Optional, Tuple, Type, TypeVar, Union, overload
+from typing import Any, Deque, Generic, List, Literal, NoReturn, Optional, Tuple, Type, TypeVar, Union, cast, overload
 from nonebot import logger
 
 from nonebot.adapters import Bot, Event
 from nonebot.exception import ActionFailed
 
 from .base import MsgBufManager
-from .utils import async_fish_cache
 from .models import (
     Face, File, Image, Location, Mention, Model, Mutex, Raw,
     Reply, Share, SupportedFileData, Text, Video, Voice
 )
 
 _BotT = TypeVar("_BotT", bound=Bot)
 _EventT = TypeVar("_EventT", bound=Event)
@@ -35,22 +34,27 @@
 class BaseProxy(Generic[_BotT, _EventT]):
     bot: _BotT
     event: _EventT
     specs: int
 
     prefix: str = ""
 
+    registered_proxies: List[Type["BaseProxy"]] = []
+
     def __init__(
         self, bot: _BotT, event: _EventT, *args,
         specs: int = 0, **kwargs
     ) -> None:
         self.bot = bot
         self.event = event
         self.specs = specs
 
+    def __init_subclass__(cls) -> None:
+        BaseProxy.registered_proxies.append(cls)
+
     async def convert(self, seg: Model) -> str:
         return seg.alternative()
     
     async def flush_with_log(self, msg, cres, log: str, log_level: str = "info"):
         if msg:
             logger.log(log_level, log)
             cres.append(await self.bot.send(self.event, msg))
@@ -64,33 +68,26 @@
                 self.event, "".join(
                     await asyncio.gather(*(self.convert(seg) for seg in segs))
                 )
             )
         ]
 
 
-registered_proxies: List[Type[BaseProxy]] = []
 _ProxyT = TypeVar("_ProxyT", bound=Type[BaseProxy])
 
 
-def register_proxy(proxy: _ProxyT) -> _ProxyT:
-    registered_proxies.append(proxy)
-    return proxy
-
-
 with suppress(ImportError):
     from nonebot.adapters.onebot.v11 import (
         Bot as OB11Bot,
         Event as OB11Event,
         Message as OB11Message,
         MessageSegment as OB11MS,
         MessageEvent as OB11MsgEv
     )
 
-    @register_proxy
     class OB11Proxy(BaseProxy[OB11Bot, OB11Event]):
         prefix = "nonebot.adapters.onebot.v11"
 
         async def convert(self, seg: Model) -> OB11MS:
             if isinstance(seg, Text):
                 return OB11MS.text(seg.text)
             elif isinstance(seg, Image):
@@ -111,14 +108,16 @@
                 return OB11MS.share(
                     seg.url, seg.title, seg.content or None, seg.image or None
                 )
             elif isinstance(seg, Location):
                 return OB11MS.location(
                     seg.lat, seg.lon, seg.title or None, seg.content or None
                 )
+            elif isinstance(seg, Raw) and seg.raw.__module__.startswith(self.prefix):
+                return cast(OB11MS, seg.raw)
             return OB11MS.text(seg.alternative())
         
         async def send(self, *segs: Model, use_fallback: bool = False) -> List[Any]:
             if use_fallback:
                 return await super().send(*segs)
             call_result = []
             msg = OB11Message()
@@ -188,17 +187,19 @@
             exc_val: Optional[BaseException],
             exc_tb: Optional[TracebackType]
         ) -> Optional[bool]:
             if exc_tb and not self.allow_incomplete:
                 return False
             if self.fn is not None:
                 self.fn.msgbuf.append(
-                    OB11MS(
-                        "node",
-                        {"uin": self.uid, "name": self.name, "content": await self.export()}
+                    Raw(
+                        OB11MS(
+                            "node",
+                            {"uin": self.uid, "name": self.name, "content": await self.export()}
+                        )
                     )
                 )
             else:
                 self.fb.fwdbuf.append(
                     OB11MS(
                         "node",
                         {"uin": self.uid, "name": self.name, "content": await self.export()}
@@ -344,15 +345,14 @@
     from nonebot.adapters.onebot.v12 import (
         Bot as OB12Bot,
         Event as OB12Event,
         Message as OB12Message,
         MessageSegment as OB12MS
     )
 
-    @async_fish_cache()
     async def _ob12_upload_file(bot: OB12Bot, file: SupportedFileData, name: str) -> str:
         if isinstance(file, str):
             if "://" in file:
                 res = await bot.upload_file(type="url", name=name, url=file)
             else:
                 res = await bot.upload_file(type="path", name=name, path=file)
         elif isinstance(file, Path):
@@ -362,15 +362,14 @@
         elif isinstance(file, BytesIO):
             res = await bot.upload_file(type="bytes", name=name, data=file.getvalue())
         else:
             raise ValueError("不受支持的数据形式")
         logger.info(f"成功上传文件 {name!r}")
         return res["file_id"]
 
-    @register_proxy
     class OB12Proxy(BaseProxy[OB12Bot, OB12Event]):
         prefix = "nonebot.adapters.onebot.v12"
 
         async def upload_file(self, file: SupportedFileData, name: str) -> str:
             return await _ob12_upload_file(self.bot, file, name)
 
         async def convert(self, seg: Model) -> OB12MS:
@@ -388,14 +387,16 @@
                 return OB12MS.video(await self.upload_file(seg.video, seg.name))
             elif isinstance(seg, File):
                 return OB12MS.file(await self.upload_file(seg.file, seg.name))
             elif isinstance(seg, Location):
                 return OB12MS.location(
                     seg.lat, seg.lon, seg.title, seg.content
                 )
+            elif isinstance(seg, Raw) and seg.raw.__module__.startswith(self.prefix):
+                return cast(OB12MS, seg.raw)
             return OB12MS.text(seg.alternative())
             
         async def send(self, *segs: Model, use_fallback: bool = False) -> List[Any]:
             if use_fallback:
                 return await super().send(*segs)
             call_result = []
             msg = OB12Message()
@@ -429,31 +430,32 @@
     from nonebot.adapters.qqguild import (
         Bot as QGBot,
         Event as QGEvent,
         Message as QGMessage,
         MessageSegment as QGMS
     )
 
-    @register_proxy
     class QGProxy(BaseProxy[QGBot, QGEvent]):
         prefix = "nonebot.adapters.qqguild"
 
         async def convert(self, seg: Model) -> QGMS:
             if isinstance(seg, Text):
                 return QGMS.text(seg.text)
             elif isinstance(seg, Image):
                 return QGMS.image(seg.image) if isinstance(seg.image, str) else QGMS.file_image(seg.image)
             elif isinstance(seg, Mention):
                 if seg.domain == "channel":
-                    return QGMS.mention_channel(int(seg.user_id)) 
-                return  QGMS.mention_user(int(seg.user_id))
+                    return QGMS.mention_channel(int(seg.user_id))
+                return QGMS.mention_user(int(seg.user_id))
             elif isinstance(seg, Reply):
                 return QGMS.reference(seg.msg_id)
             elif isinstance(seg, Face):
                 return QGMS.emoji(seg.face_id)
+            elif isinstance(seg, Raw) and seg.raw.__module__.startswith(self.prefix):
+                return cast(QGMS, seg.raw)
             return QGMS.text(seg.alternative())
 
         async def send(self, *segs: Model, use_fallback: bool = False) -> List[Any]:
             if use_fallback:
                 return await super().send(*segs)
             call_result = []
             msg = QGMessage()
@@ -465,27 +467,126 @@
                 elif isinstance(seg, Raw) and isinstance(
                     seg.raw, (str, QGMS, QGMessage)
                 ):
                     await self.flush_with_log(msg, call_result, "Raw 类型无法在一条内发送！")
                     call_result.append(
                         await self.bot.send(self.event, seg.raw)
                     )
-                msg.append(await self.convert(seg))
+                else:
+                    msg.append(await self.convert(seg))
             if msg:
                 call_result.append(await self.bot.send(self.event, msg))
             return call_result
 
     @overload
     def find_proxy(bot: QGBot) -> Type[QGProxy]:
         ...
 
 
+with suppress(ImportError):
+    from nonebot.adapters.telegram import (
+        Bot as TGBot,
+        Event as TGEvent,
+        Message as TGMessage,
+        MessageSegment as TGMS
+    )
+    from nonebot.adapters.telegram.message import (
+        Entity as TGRichTextMS,
+        UnCombinFile as TGFileMS
+    )
+
+    class TGProxy(BaseProxy[TGBot, TGEvent]):
+        prefix = "nonebot.adapters.telegram"
+
+        async def convert(self, seg: Model) -> TGMS:
+            if isinstance(seg, Text):
+                if not seg.rich:
+                    return TGRichTextMS.text(seg.text)
+                elif seg.rich in (
+                    "hashtag", "cashtag", "bot_command", "url", "email", "phone_number",
+                    "bold", "italic", "underline", "strikethrough", "spoiler", "code", "pre"
+                ):
+                    return getattr(TGRichTextMS, seg.rich)(seg.text)
+                logger.warning(f"未识别的富文本格式 {seg.rich!r}，将作为纯文本发送")
+            elif isinstance(seg, Image):
+                if isinstance(seg.image, BytesIO):
+                    return TGFileMS.photo(seg.image.getvalue())
+                elif isinstance(seg.image, bytes):
+                    return TGFileMS.photo(seg.image)
+                return TGFileMS.photo(File(seg.image, seg.name).local_path())
+            elif isinstance(seg, Mention):
+                if seg.tg_user is None:
+                    return TGRichTextMS.mention(f"@{seg.user_id}")
+                return TGRichTextMS.text_mention(seg.user_id, seg.tg_user)
+            elif isinstance(seg, Face):
+                return TGFileMS.sticker(seg.face_id)
+            elif isinstance(seg, Voice):
+                if isinstance(seg.voice, BytesIO):
+                    return TGFileMS.voice(seg.voice.getvalue())
+                elif isinstance(seg.voice, bytes):
+                    return TGFileMS.voice(seg.voice)
+                return TGFileMS.voice(File(seg.voice, seg.name).local_path())
+            elif isinstance(seg, Video):
+                if isinstance(seg.video, BytesIO):
+                    return TGFileMS.video(seg.video.getvalue())
+                elif isinstance(seg.video, bytes):
+                    return TGFileMS.video(seg.video)
+                return TGFileMS.video(File(seg.video, seg.name).local_path())
+            elif isinstance(seg, File):
+                if isinstance(seg.file, BytesIO):
+                    return TGFileMS.document(seg.file.getvalue())
+                elif isinstance(seg.file, bytes):
+                    return TGFileMS.document(seg.file)
+                return TGFileMS.document(seg.local_path())
+            elif isinstance(seg, Location):
+                return TGMS.location(seg.lat, seg.lon)
+            elif isinstance(seg, Raw) and seg.raw.__module__.startswith(self.prefix):
+                return cast(TGMS, seg.raw)
+            return TGRichTextMS.text(seg.alternative())
+
+        async def send(self, *segs: Model, use_fallback: bool = False) -> List[Any]:
+            if use_fallback:
+                return await super().send(*segs)
+            call_result = []
+            msg = TGMessage()
+            reply = None
+            for seg in segs:
+                if isinstance(seg, Mutex):
+                    await self.flush_with_log(msg, call_result, f"{seg.__class__.__name__} 类型与 Body 类型冲突，无法在一条内发送！")
+                    if isinstance(seg, Raw) and isinstance(
+                        seg.raw, (str, TGMS, TGMessage)
+                    ):
+                        call_result.append(
+                            await self.bot.send(self.event, seg.raw, reply_to_message_id=reply)
+                        )
+                    else:
+                        call_result.append(
+                            await self.bot.send(self.event, await self.convert(seg), reply_to_message_id=reply)
+                        )
+                else:
+                    if isinstance(seg, Reply):
+                        reply = int(seg.msg_id)
+                        continue
+                    msg.append(await self.convert(seg))
+            if msg:
+                call_result.append(await self.bot.send(self.event, msg, reply_to_message_id=reply))
+            return call_result
+
+    @overload
+    def find_proxy(bot: TGBot) -> Type[TGProxy]:
+        ...
+
+
 @overload
 def find_proxy(bot: _BotT) -> Type[BaseProxy[_BotT, Any]]:
     ...
 
 
 def find_proxy(bot: Bot) -> Type[BaseProxy]:
-    for p in registered_proxies:
-        if bot.__module__.startswith(p.prefix):
-            return p
-    return BaseProxy
+    return next(
+        (
+            p
+            for p in BaseProxy.registered_proxies
+            if bot.__module__.startswith(p.prefix)
+        ),
+        BaseProxy,
+    )
```

### Comparing `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf/utils.py` & `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.3.2/nonebot_plugin_msgbuf.egg-info/PKG-INFO` & `nonebot-plugin-msgbuf-0.4.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.3.2
+Version: 0.4.0
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -48,32 +48,27 @@
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
 |                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            QQ 频道                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
+|                            Telegram                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
 nb plugin install nonebot-plugin-msgbuf
 ```
 
 ## 使用
 
-> 关于 `require()` 的使用问题：
->
-> NoneBot2 插件的**首次**导入**必须**通过 NoneBot2 自身的方式（包括但不限于 `require()`, `load_plugin()` 等）完成，否则之后使用 NoneBot2 方式导入该插件的插件将**无法**正常工作。
->
-> NoneBot2 插件体系要求**必须**使用 `require()` 加载插件依赖。
-
 ### 竞品对比
 
 这是常规的消息构造与发送方法：
 
 <details>
 <summary>展开</summary>
```

