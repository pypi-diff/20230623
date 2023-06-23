# Comparing `tmp/nonebot_plugin_apex_api_query-23.3.5.tar.gz` & `tmp/nonebot_plugin_apex_api_query-23.6.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_apex_api_query-23.3.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_apex_api_query-23.6.23.tar", max compression
```

## Comparing `nonebot_plugin_apex_api_query-23.3.5.tar` & `nonebot_plugin_apex_api_query-23.6.23.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1085 2023-03-03 14:36:03.336256 nonebot_plugin_apex_api_query-23.3.5/LICENSE
--rw-r--r--   0        0        0    27449 2023-03-04 11:31:40.952034 nonebot_plugin_apex_api_query-23.3.5/nonebot_plugin_apex_api_query/__init__.py
--rw-r--r--   0        0        0      243 2023-03-03 14:36:03.338251 nonebot_plugin_apex_api_query-23.3.5/nonebot_plugin_apex_api_query/config.py
--rw-r--r--   0        0        0      808 2023-03-04 13:22:53.902739 nonebot_plugin_apex_api_query-23.3.5/pyproject.toml
--rw-r--r--   0        0        0     4241 2023-03-04 13:22:43.397107 nonebot_plugin_apex_api_query-23.3.5/README.md
--rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 nonebot_plugin_apex_api_query-23.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-23 03:33:44.167483 nonebot_plugin_apex_api_query-23.6.23/LICENSE
+-rw-r--r--   0        0        0    36530 2023-06-23 04:30:47.073325 nonebot_plugin_apex_api_query-23.6.23/nonebot_plugin_apex_api_query/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-23 03:33:44.171003 nonebot_plugin_apex_api_query-23.6.23/nonebot_plugin_apex_api_query/config.py
+-rw-r--r--   0        0        0      886 2023-06-23 04:51:58.373230 nonebot_plugin_apex_api_query-23.6.23/pyproject.toml
+-rw-r--r--   0        0        0     5384 2023-06-23 04:28:38.380271 nonebot_plugin_apex_api_query-23.6.23/README.md
+-rw-r--r--   0        0        0     6406 1970-01-01 00:00:00.000000 nonebot_plugin_apex_api_query-23.6.23/PKG-INFO
```

### Comparing `nonebot_plugin_apex_api_query-23.3.5/LICENSE` & `nonebot_plugin_apex_api_query-23.6.23/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_apex_api_query-23.3.5/pyproject.toml` & `nonebot_plugin_apex_api_query-23.6.23/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-apex-api-query"
-version = "23.3.5"
+version = "23.6.23"
 description = "基于 NoneBot2 的 Apex Legends API 查询插件"
 license = "MIT"
 authors = ["HxiaoH <412454922@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/H-xiaoH/nonebot-plugin-apex-api-query"
 repository = "https://github.com/H-xiaoH/nonebot-plugin-apex-api-query"
 documentation = "https://github.com/H-xiaoH/nonebot-plugin-apex-api-query/blob/main/README.md"
@@ -13,11 +13,13 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.23.0"
 nonebot2 = "^2.0.0rc2"
 nonebot-adapter-onebot = "^2.2.0"
 nonebot-plugin-apscheduler = "^0.2.0"
 nonebot-plugin-txt2img = "^0.2.1"
+nonebot-plugin-guild-patch = "^0.2.3"
+nonebot-plugin-localstore = "^0.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_apex_api_query-23.3.5/README.md` & `nonebot_plugin_apex_api_query-23.6.23/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 
 您可以在 [此处](https://portal.apexlegendsapi.com/) 申请您自己的 API 密钥。
 申请密钥后重新在 [此页面](https://portal.apexlegendsapi.com/) 登录 API 密钥以测试密钥是否可用。
 必须将此 API 密钥 [链接](https://portal.apexlegendsapi.com/discord-auth) 至您的 Discord 账户后您的 API 密钥才可用。
 
 由于 API 的问题，您只能在查询玩家信息时使用 EA 账户用户名并非 Steam 账户用户名。
 
+数据由 API 提供，本插件仅作 数据获取 和 内容转换 。
+
+如您遇到了 `OSError: cannot open resource` 错误，请检查 [#7](https://github.com/H-xiaoH/nonebot-plugin-apex-api-query/issues/7) 。
+
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot_plugin_apex_api_query
@@ -72,35 +76,42 @@
 | APEX_API_URL | 否 | https://api.mozambiquehe.re/ | API 链接地址 |
 | APEX_API_T2I | 否 | True | 文字转图片 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| 玩家 [玩家名称] | 无 | 否 | 私聊/群聊 | 根据玩家名称查询信息 (暂仅支持查询 PC 平台玩家信息) |
-| UID [玩家UID] | 无 | 否 | 私聊/群聊 | 根据玩家 UID 查询信息 (暂仅支持查询 PC 平台玩家信息) |
-| 地图 | 无 | 否 | 私聊/群聊 | 查询地图轮换 |
-| 猎杀 | 无 | 否 | 私聊/群聊 | 查询各平台顶尖猎杀者信息 |
-| 制造 | 无 | 否 | 私聊/群聊 | 查询复制器轮换 |
-| 服务 | 无 | 否 | 私聊/群聊 | 查询服务器状态 |
-| 订阅地图 | 管理 | 否 | 群聊 | 每整点查询地图轮换 |
-| 取消订阅地图 | 管理 | 否 | 群聊 | 取消每整点查询地图轮换 |
-| 订阅制造 | 管理 | 否 | 群聊 | 每日 2 时查询复制器轮换 |
-| 取消订阅制造 | 管理 | 否 | 群聊 | 取消每日 2 时查询复制器轮换 |
+| 玩家 [玩家名称] | 无 | 否 | 私聊/群聊/频道 | 根据玩家名称查询信息 (暂仅支持查询 PC 平台玩家信息) |
+| UID [玩家UID] | 无 | 否 | 私聊/群聊/频道 | 根据玩家 UID 查询信息 (暂仅支持查询 PC 平台玩家信息) |
+| 自查 | 无 | 否 | 私聊/群聊/频道 | 根据玩家已绑定的 UID 自动查询玩家信息 |
+| 地图 | 无 | 否 | 私聊/群聊/频道 | 查询地图轮换 |
+| 猎杀 | 无 | 否 | 私聊/群聊/频道 | 查询各平台顶尖猎杀者信息 |
+| 制造 | 无 | 否 | 私聊/群聊/频道 | 查询复制器轮换 |
+| 服务 | 无 | 否 | 私聊/群聊/频道 | 查询服务器状态 |
+| 订阅地图 | 管理员 | 否 | 群聊/频道 | 每整点查询地图轮换 |
+| 取消订阅地图 | 管理员 | 否 | 群聊/频道 | 取消每整点查询地图轮换 |
+| 订阅制造 | 管理员 | 否 | 群聊/频道 | 每日 2 时查询复制器轮换 |
+| 取消订阅制造 | 管理员 | 否 | 群聊/频道 | 取消每日 2 时查询复制器轮换 |
+| 绑定 [玩家 UID] | 无 | 否 | 私聊/群聊/频道 | 将 UID 与 QQ 账号绑定 (群聊 与 频道 信息不互通) |
+| 解绑 | 无 | 否 | 私聊/群聊/频道 | 将 UID 与 QQ 账号解除绑定 (群聊 与 频道 信息不互通) |
+
+## 🖼️ 效果图
+
+![Bridge](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/Bridge.png)
+![MapRotation](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/MapRotation.png)
+![Crafting](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/Crafting.png)
 
 ## 📄 ToDo
 
-玩家 ID 与 QQ 账号绑定。
-
-支持 QQ 频道。
-
-存储群订阅信息。
+如您有想要的功能，请提交 [Issues](https://github.com/H-xiaoH/nonebot-plugin-apex-api-query/issues) 。
 
 ## 🌸 致谢
 
-- [@nonebot](https://github.com/nonebot) 强大的 [NoneBot2 机器人框架](https://github.com/nonebot/nonebot2)。
+- [@nonebot](https://github.com/nonebot) 强大的 [NoneBot2 机器人框架](https://github.com/nonebot/nonebot2)
+
+- [@nonebot](https://github.com/nonebot) 订阅功能基于 [APScheduler 定时任务插件](https://github.com/nonebot/plugin-apscheduler)
 
-- [@nonebot](https://github.com/nonebot) 订阅功能基于 [APScheduler 定时任务插件](https://github.com/nonebot/plugin-apscheduler)。
+- [@nonebot](https://github.com/nonebot) 本地数据存储功能基于 [本地数据存储](https://github.com/nonebot/plugin-localstore)
 
-- [@A-kirami](https://github.com/A-kirami) 使用其 NoneBot Plugin [README 模板](https://github.com/A-kirami/nonebot-plugin-template)。
+- [@A-kirami](https://github.com/A-kirami) 使用其 NoneBot Plugin [README 模板](https://github.com/A-kirami/nonebot-plugin-template)
 
-- [@mobyw](https://github.com/mobyw) 文字转图片功能源于 [轻量文字转图片插件](https://github.com/mobyw/nonebot-plugin-txt2img)
+- [@mobyw](https://github.com/mobyw) 文字转图片功能源于 [轻量文字转图片插件](https://github.com/mobyw/nonebot-plugin-txt2img)
```

#### html2text {}

```diff
@@ -6,41 +6,56 @@
 API](https://apexlegendsstatus.com/) æ¥è¯¢æä»¶ã æ¨å¯ä»¥å¨ [æ­¤å¤]
 (https://portal.apexlegendsapi.com/) ç³è¯·æ¨èªå·±ç API å¯é¥ã
 ç³è¯·å¯é¥åéæ°å¨ [æ­¤é¡µé¢](https://portal.apexlegendsapi.com/) ç»å½
 API å¯é¥ä»¥æµè¯å¯é¥æ¯å¦å¯ç¨ã å¿é¡»å°æ­¤ API å¯é¥ [é¾æ¥]
 (https://portal.apexlegendsapi.com/discord-auth) è³æ¨ç Discord
 è´¦æ·åæ¨ç API å¯é¥æå¯ç¨ã ç±äº API
 çé®é¢ï¼æ¨åªè½å¨æ¥è¯¢ç©å®¶ä¿¡æ¯æ¶ä½¿ç¨ EA è´¦æ·ç¨æ·åå¹¶é
-Steam è´¦æ·ç¨æ·åã ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+Steam è´¦æ·ç¨æ·åã æ°æ®ç± API æä¾ï¼æ¬æä»¶ä»ä½ æ°æ®è·å
+å åå®¹è½¬æ¢ ã å¦æ¨éå°äº `OSError: cannot open resource`
+éè¯¯ï¼è¯·æ£æ¥ [#7](https://github.com/H-xiaoH/nonebot-plugin-apex-api-
+query/issues/7) ã ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot_plugin_apex_api_query   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot_plugin_apex_api_query
 poetry poetry add nonebot_plugin_apex_api_query  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_apex_api_query"]  ## âï¸
 éç½® å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® |
 éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
 APEX_API_KEY | æ¯ | None | API å¯é¥ | | APEX_API_URL | å¦ | https://
 api.mozambiquehe.re/ | API é¾æ¥å°å | | APEX_API_T2I | å¦ | True |
 æå­è½¬å¾ç | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ |
 èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | ç©å®¶ [ç©å®¶åç§°]
-| æ  | å¦ | ç§è/ç¾¤è | æ ¹æ®ç©å®¶åç§°æ¥è¯¢ä¿¡æ¯
+| æ  | å¦ | ç§è/ç¾¤è/é¢é | æ ¹æ®ç©å®¶åç§°æ¥è¯¢ä¿¡æ¯
 (æä»æ¯ææ¥è¯¢ PC å¹³å°ç©å®¶ä¿¡æ¯) | | UID [ç©å®¶UID] | æ  | å¦ |
-ç§è/ç¾¤è | æ ¹æ®ç©å®¶ UID æ¥è¯¢ä¿¡æ¯ (æä»æ¯ææ¥è¯¢ PC
-å¹³å°ç©å®¶ä¿¡æ¯) | | å°å¾ | æ  | å¦ | ç§è/ç¾¤è | æ¥è¯¢å°å¾è½®æ¢
-| | çæ | æ  | å¦ | ç§è/ç¾¤è | æ¥è¯¢åå¹³å°é¡¶å°çæèä¿¡æ¯ |
-| å¶é  | æ  | å¦ | ç§è/ç¾¤è | æ¥è¯¢å¤å¶å¨è½®æ¢ | | æå¡ | æ  |
-å¦ | ç§è/ç¾¤è | æ¥è¯¢æå¡å¨ç¶æ | | è®¢éå°å¾ | ç®¡ç | å¦ |
-ç¾¤è | æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | åæ¶è®¢éå°å¾ | ç®¡ç | å¦ |
-ç¾¤è | åæ¶æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | è®¢éå¶é  | ç®¡ç | å¦ |
-ç¾¤è | æ¯æ¥ 2 æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | | åæ¶è®¢éå¶é  | ç®¡ç |
-å¦ | ç¾¤è | åæ¶æ¯æ¥ 2 æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | ## ð ToDo ç©å®¶ ID
-ä¸ QQ è´¦å·ç»å®ã æ¯æ QQ é¢éã å­å¨ç¾¤è®¢éä¿¡æ¯ã ## ð¸
-è´è°¢ - [@nonebot](https://github.com/nonebot) å¼ºå¤§ç [NoneBot2
-æºå¨äººæ¡æ¶](https://github.com/nonebot/nonebot2)ã - [@nonebot](https://
-github.com/nonebot) è®¢éåè½åºäº [APScheduler å®æ¶ä»»å¡æä»¶](https:/
-/github.com/nonebot/plugin-apscheduler)ã - [@A-kirami](https://github.com/A-
-kirami) ä½¿ç¨å¶ NoneBot Plugin [README æ¨¡æ¿](https://github.com/A-kirami/
-nonebot-plugin-template)ã - [@mobyw](https://github.com/mobyw)
-æå­è½¬å¾çåè½æºäº [è½»éæå­è½¬å¾çæä»¶](https://github.com/
-mobyw/nonebot-plugin-txt2img)
+ç§è/ç¾¤è/é¢é | æ ¹æ®ç©å®¶ UID æ¥è¯¢ä¿¡æ¯ (æä»æ¯ææ¥è¯¢ PC
+å¹³å°ç©å®¶ä¿¡æ¯) | | èªæ¥ | æ  | å¦ | ç§è/ç¾¤è/é¢é |
+æ ¹æ®ç©å®¶å·²ç»å®ç UID èªå¨æ¥è¯¢ç©å®¶ä¿¡æ¯ | | å°å¾ | æ  | å¦ |
+ç§è/ç¾¤è/é¢é | æ¥è¯¢å°å¾è½®æ¢ | | çæ | æ  | å¦ | ç§è/
+ç¾¤è/é¢é | æ¥è¯¢åå¹³å°é¡¶å°çæèä¿¡æ¯ | | å¶é  | æ  | å¦ |
+ç§è/ç¾¤è/é¢é | æ¥è¯¢å¤å¶å¨è½®æ¢ | | æå¡ | æ  | å¦ | ç§è/
+ç¾¤è/é¢é | æ¥è¯¢æå¡å¨ç¶æ | | è®¢éå°å¾ | ç®¡çå | å¦ |
+ç¾¤è/é¢é | æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | åæ¶è®¢éå°å¾ | ç®¡çå
+| å¦ | ç¾¤è/é¢é | åæ¶æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | è®¢éå¶é  |
+ç®¡çå | å¦ | ç¾¤è/é¢é | æ¯æ¥ 2 æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | |
+åæ¶è®¢éå¶é  | ç®¡çå | å¦ | ç¾¤è/é¢é | åæ¶æ¯æ¥ 2
+æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | | ç»å® [ç©å®¶ UID] | æ  | å¦ | ç§è/ç¾¤è/
+é¢é | å° UID ä¸ QQ è´¦å·ç»å® (ç¾¤è ä¸ é¢é ä¿¡æ¯ä¸äºé) | |
+è§£ç» | æ  | å¦ | ç§è/ç¾¤è/é¢é | å° UID ä¸ QQ è´¦å·è§£é¤ç»å®
+(ç¾¤è ä¸ é¢é ä¿¡æ¯ä¸äºé) | ## ð¼ï¸ ææå¾ ![Bridge](https://
+oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/Bridge.png) !
+[MapRotation](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-
+api-query/MapRotation.png) ![Crafting](https://oss.hxiaoh.com/File/GitHub/
+Photos/nonebot-plugin-apex-api-query/Crafting.png) ## ð ToDo
+å¦æ¨ææ³è¦çåè½ï¼è¯·æäº¤ [Issues](https://github.com/H-xiaoH/
+nonebot-plugin-apex-api-query/issues) ã ## ð¸ è´è°¢ - [@nonebot](https://
+github.com/nonebot) å¼ºå¤§ç [NoneBot2 æºå¨äººæ¡æ¶](https://github.com/
+nonebot/nonebot2) - [@nonebot](https://github.com/nonebot) è®¢éåè½åºäº
+[APScheduler å®æ¶ä»»å¡æä»¶](https://github.com/nonebot/plugin-apscheduler)
+- [@nonebot](https://github.com/nonebot) æ¬å°æ°æ®å­å¨åè½åºäº
+[æ¬å°æ°æ®å­å¨](https://github.com/nonebot/plugin-localstore) - [@A-
+kirami](https://github.com/A-kirami) ä½¿ç¨å¶ NoneBot Plugin [README æ¨¡æ¿]
+(https://github.com/A-kirami/nonebot-plugin-template) - [@mobyw](https://
+github.com/mobyw) æå­è½¬å¾çåè½æºäº [è½»éæå­è½¬å¾çæä»¶]
+(https://github.com/mobyw/nonebot-plugin-txt2img)
```

### Comparing `nonebot_plugin_apex_api_query-23.3.5/PKG-INFO` & `nonebot_plugin_apex_api_query-23.6.23/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-apex-api-query
-Version: 23.3.5
+Version: 23.6.23
 Summary: 基于 NoneBot2 的 Apex Legends API 查询插件
 Home-page: https://github.com/H-xiaoH/nonebot-plugin-apex-api-query
 License: MIT
 Author: HxiaoH
 Author-email: 412454922@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-guild-patch (>=0.2.3,<0.3.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.4.1,<0.5.0)
 Requires-Dist: nonebot-plugin-txt2img (>=0.2.1,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
 Project-URL: Documentation, https://github.com/H-xiaoH/nonebot-plugin-apex-api-query/blob/main/README.md
 Project-URL: Repository, https://github.com/H-xiaoH/nonebot-plugin-apex-api-query
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -50,14 +52,18 @@
 
 您可以在 [此处](https://portal.apexlegendsapi.com/) 申请您自己的 API 密钥。
 申请密钥后重新在 [此页面](https://portal.apexlegendsapi.com/) 登录 API 密钥以测试密钥是否可用。
 必须将此 API 密钥 [链接](https://portal.apexlegendsapi.com/discord-auth) 至您的 Discord 账户后您的 API 密钥才可用。
 
 由于 API 的问题，您只能在查询玩家信息时使用 EA 账户用户名并非 Steam 账户用户名。
 
+数据由 API 提供，本插件仅作 数据获取 和 内容转换 。
+
+如您遇到了 `OSError: cannot open resource` 错误，请检查 [#7](https://github.com/H-xiaoH/nonebot-plugin-apex-api-query/issues/7) 。
+
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot_plugin_apex_api_query
@@ -95,35 +101,43 @@
 | APEX_API_URL | 否 | https://api.mozambiquehe.re/ | API 链接地址 |
 | APEX_API_T2I | 否 | True | 文字转图片 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| 玩家 [玩家名称] | 无 | 否 | 私聊/群聊 | 根据玩家名称查询信息 (暂仅支持查询 PC 平台玩家信息) |
-| UID [玩家UID] | 无 | 否 | 私聊/群聊 | 根据玩家 UID 查询信息 (暂仅支持查询 PC 平台玩家信息) |
-| 地图 | 无 | 否 | 私聊/群聊 | 查询地图轮换 |
-| 猎杀 | 无 | 否 | 私聊/群聊 | 查询各平台顶尖猎杀者信息 |
-| 制造 | 无 | 否 | 私聊/群聊 | 查询复制器轮换 |
-| 服务 | 无 | 否 | 私聊/群聊 | 查询服务器状态 |
-| 订阅地图 | 管理 | 否 | 群聊 | 每整点查询地图轮换 |
-| 取消订阅地图 | 管理 | 否 | 群聊 | 取消每整点查询地图轮换 |
-| 订阅制造 | 管理 | 否 | 群聊 | 每日 2 时查询复制器轮换 |
-| 取消订阅制造 | 管理 | 否 | 群聊 | 取消每日 2 时查询复制器轮换 |
+| 玩家 [玩家名称] | 无 | 否 | 私聊/群聊/频道 | 根据玩家名称查询信息 (暂仅支持查询 PC 平台玩家信息) |
+| UID [玩家UID] | 无 | 否 | 私聊/群聊/频道 | 根据玩家 UID 查询信息 (暂仅支持查询 PC 平台玩家信息) |
+| 自查 | 无 | 否 | 私聊/群聊/频道 | 根据玩家已绑定的 UID 自动查询玩家信息 |
+| 地图 | 无 | 否 | 私聊/群聊/频道 | 查询地图轮换 |
+| 猎杀 | 无 | 否 | 私聊/群聊/频道 | 查询各平台顶尖猎杀者信息 |
+| 制造 | 无 | 否 | 私聊/群聊/频道 | 查询复制器轮换 |
+| 服务 | 无 | 否 | 私聊/群聊/频道 | 查询服务器状态 |
+| 订阅地图 | 管理员 | 否 | 群聊/频道 | 每整点查询地图轮换 |
+| 取消订阅地图 | 管理员 | 否 | 群聊/频道 | 取消每整点查询地图轮换 |
+| 订阅制造 | 管理员 | 否 | 群聊/频道 | 每日 2 时查询复制器轮换 |
+| 取消订阅制造 | 管理员 | 否 | 群聊/频道 | 取消每日 2 时查询复制器轮换 |
+| 绑定 [玩家 UID] | 无 | 否 | 私聊/群聊/频道 | 将 UID 与 QQ 账号绑定 (群聊 与 频道 信息不互通) |
+| 解绑 | 无 | 否 | 私聊/群聊/频道 | 将 UID 与 QQ 账号解除绑定 (群聊 与 频道 信息不互通) |
+
+## 🖼️ 效果图
+
+![Bridge](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/Bridge.png)
+![MapRotation](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/MapRotation.png)
+![Crafting](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/Crafting.png)
 
 ## 📄 ToDo
 
-玩家 ID 与 QQ 账号绑定。
-
-支持 QQ 频道。
-
-存储群订阅信息。
+如您有想要的功能，请提交 [Issues](https://github.com/H-xiaoH/nonebot-plugin-apex-api-query/issues) 。
 
 ## 🌸 致谢
 
-- [@nonebot](https://github.com/nonebot) 强大的 [NoneBot2 机器人框架](https://github.com/nonebot/nonebot2)。
+- [@nonebot](https://github.com/nonebot) 强大的 [NoneBot2 机器人框架](https://github.com/nonebot/nonebot2)
+
+- [@nonebot](https://github.com/nonebot) 订阅功能基于 [APScheduler 定时任务插件](https://github.com/nonebot/plugin-apscheduler)
 
-- [@nonebot](https://github.com/nonebot) 订阅功能基于 [APScheduler 定时任务插件](https://github.com/nonebot/plugin-apscheduler)。
+- [@nonebot](https://github.com/nonebot) 本地数据存储功能基于 [本地数据存储](https://github.com/nonebot/plugin-localstore)
 
-- [@A-kirami](https://github.com/A-kirami) 使用其 NoneBot Plugin [README 模板](https://github.com/A-kirami/nonebot-plugin-template)。
+- [@A-kirami](https://github.com/A-kirami) 使用其 NoneBot Plugin [README 模板](https://github.com/A-kirami/nonebot-plugin-template)
 
 - [@mobyw](https://github.com/mobyw) 文字转图片功能源于 [轻量文字转图片插件](https://github.com/mobyw/nonebot-plugin-txt2img)
+
```

#### html2text {}

```diff
@@ -1,60 +1,76 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-apex-api-query Version: 23.3.5
+Metadata-Version: 2.1 Name: nonebot-plugin-apex-api-query Version: 23.6.23
 Summary: åºäº NoneBot2 ç Apex Legends API æ¥è¯¢æä»¶ Home-page: https://
 github.com/H-xiaoH/nonebot-plugin-apex-api-query License: MIT Author: HxiaoH
 Author-email: 412454922@qq.com Requires-Python: >=3.9,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.0,<3.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot-plugin-txt2img (>=0.2.1,<0.3.0) Requires-Dist: nonebot2
-(>=2.0.0rc2,<3.0.0) Project-URL: Documentation, https://github.com/H-xiaoH/
-nonebot-plugin-apex-api-query/blob/main/README.md Project-URL: Repository,
-https://github.com/H-xiaoH/nonebot-plugin-apex-api-query Description-Content-
-Type: text/markdown
+Requires-Dist: nonebot-plugin-guild-patch (>=0.2.3,<0.3.0) Requires-Dist:
+nonebot-plugin-localstore (>=0.4.1,<0.5.0) Requires-Dist: nonebot-plugin-
+txt2img (>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0) Project-
+URL: Documentation, https://github.com/H-xiaoH/nonebot-plugin-apex-api-query/
+blob/main/README.md Project-URL: Repository, https://github.com/H-xiaoH/
+nonebot-plugin-apex-api-query Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # nonebot-plugin-apex-api-query _â¨ åºäº NoneBot ç Apex Legends API
                   æ¥è¯¢æä»¶ â¨_ [license] [pypi] [python]
 ## ð ä»ç» åºäº NoneBot2 ä¸ä½¿ç¨ OneBot V11 åè®® ç [Apex Legends
 API](https://apexlegendsstatus.com/) æ¥è¯¢æä»¶ã æ¨å¯ä»¥å¨ [æ­¤å¤]
 (https://portal.apexlegendsapi.com/) ç³è¯·æ¨èªå·±ç API å¯é¥ã
 ç³è¯·å¯é¥åéæ°å¨ [æ­¤é¡µé¢](https://portal.apexlegendsapi.com/) ç»å½
 API å¯é¥ä»¥æµè¯å¯é¥æ¯å¦å¯ç¨ã å¿é¡»å°æ­¤ API å¯é¥ [é¾æ¥]
 (https://portal.apexlegendsapi.com/discord-auth) è³æ¨ç Discord
 è´¦æ·åæ¨ç API å¯é¥æå¯ç¨ã ç±äº API
 çé®é¢ï¼æ¨åªè½å¨æ¥è¯¢ç©å®¶ä¿¡æ¯æ¶ä½¿ç¨ EA è´¦æ·ç¨æ·åå¹¶é
-Steam è´¦æ·ç¨æ·åã ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+Steam è´¦æ·ç¨æ·åã æ°æ®ç± API æä¾ï¼æ¬æä»¶ä»ä½ æ°æ®è·å
+å åå®¹è½¬æ¢ ã å¦æ¨éå°äº `OSError: cannot open resource`
+éè¯¯ï¼è¯·æ£æ¥ [#7](https://github.com/H-xiaoH/nonebot-plugin-apex-api-
+query/issues/7) ã ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot_plugin_apex_api_query   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot_plugin_apex_api_query
 poetry poetry add nonebot_plugin_apex_api_query  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_apex_api_query"]  ## âï¸
 éç½® å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® |
 éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
 APEX_API_KEY | æ¯ | None | API å¯é¥ | | APEX_API_URL | å¦ | https://
 api.mozambiquehe.re/ | API é¾æ¥å°å | | APEX_API_T2I | å¦ | True |
 æå­è½¬å¾ç | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ |
 èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | ç©å®¶ [ç©å®¶åç§°]
-| æ  | å¦ | ç§è/ç¾¤è | æ ¹æ®ç©å®¶åç§°æ¥è¯¢ä¿¡æ¯
+| æ  | å¦ | ç§è/ç¾¤è/é¢é | æ ¹æ®ç©å®¶åç§°æ¥è¯¢ä¿¡æ¯
 (æä»æ¯ææ¥è¯¢ PC å¹³å°ç©å®¶ä¿¡æ¯) | | UID [ç©å®¶UID] | æ  | å¦ |
-ç§è/ç¾¤è | æ ¹æ®ç©å®¶ UID æ¥è¯¢ä¿¡æ¯ (æä»æ¯ææ¥è¯¢ PC
-å¹³å°ç©å®¶ä¿¡æ¯) | | å°å¾ | æ  | å¦ | ç§è/ç¾¤è | æ¥è¯¢å°å¾è½®æ¢
-| | çæ | æ  | å¦ | ç§è/ç¾¤è | æ¥è¯¢åå¹³å°é¡¶å°çæèä¿¡æ¯ |
-| å¶é  | æ  | å¦ | ç§è/ç¾¤è | æ¥è¯¢å¤å¶å¨è½®æ¢ | | æå¡ | æ  |
-å¦ | ç§è/ç¾¤è | æ¥è¯¢æå¡å¨ç¶æ | | è®¢éå°å¾ | ç®¡ç | å¦ |
-ç¾¤è | æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | åæ¶è®¢éå°å¾ | ç®¡ç | å¦ |
-ç¾¤è | åæ¶æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | è®¢éå¶é  | ç®¡ç | å¦ |
-ç¾¤è | æ¯æ¥ 2 æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | | åæ¶è®¢éå¶é  | ç®¡ç |
-å¦ | ç¾¤è | åæ¶æ¯æ¥ 2 æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | ## ð ToDo ç©å®¶ ID
-ä¸ QQ è´¦å·ç»å®ã æ¯æ QQ é¢éã å­å¨ç¾¤è®¢éä¿¡æ¯ã ## ð¸
-è´è°¢ - [@nonebot](https://github.com/nonebot) å¼ºå¤§ç [NoneBot2
-æºå¨äººæ¡æ¶](https://github.com/nonebot/nonebot2)ã - [@nonebot](https://
-github.com/nonebot) è®¢éåè½åºäº [APScheduler å®æ¶ä»»å¡æä»¶](https:/
-/github.com/nonebot/plugin-apscheduler)ã - [@A-kirami](https://github.com/A-
-kirami) ä½¿ç¨å¶ NoneBot Plugin [README æ¨¡æ¿](https://github.com/A-kirami/
-nonebot-plugin-template)ã - [@mobyw](https://github.com/mobyw)
-æå­è½¬å¾çåè½æºäº [è½»éæå­è½¬å¾çæä»¶](https://github.com/
-mobyw/nonebot-plugin-txt2img)
+ç§è/ç¾¤è/é¢é | æ ¹æ®ç©å®¶ UID æ¥è¯¢ä¿¡æ¯ (æä»æ¯ææ¥è¯¢ PC
+å¹³å°ç©å®¶ä¿¡æ¯) | | èªæ¥ | æ  | å¦ | ç§è/ç¾¤è/é¢é |
+æ ¹æ®ç©å®¶å·²ç»å®ç UID èªå¨æ¥è¯¢ç©å®¶ä¿¡æ¯ | | å°å¾ | æ  | å¦ |
+ç§è/ç¾¤è/é¢é | æ¥è¯¢å°å¾è½®æ¢ | | çæ | æ  | å¦ | ç§è/
+ç¾¤è/é¢é | æ¥è¯¢åå¹³å°é¡¶å°çæèä¿¡æ¯ | | å¶é  | æ  | å¦ |
+ç§è/ç¾¤è/é¢é | æ¥è¯¢å¤å¶å¨è½®æ¢ | | æå¡ | æ  | å¦ | ç§è/
+ç¾¤è/é¢é | æ¥è¯¢æå¡å¨ç¶æ | | è®¢éå°å¾ | ç®¡çå | å¦ |
+ç¾¤è/é¢é | æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | åæ¶è®¢éå°å¾ | ç®¡çå
+| å¦ | ç¾¤è/é¢é | åæ¶æ¯æ´ç¹æ¥è¯¢å°å¾è½®æ¢ | | è®¢éå¶é  |
+ç®¡çå | å¦ | ç¾¤è/é¢é | æ¯æ¥ 2 æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | |
+åæ¶è®¢éå¶é  | ç®¡çå | å¦ | ç¾¤è/é¢é | åæ¶æ¯æ¥ 2
+æ¶æ¥è¯¢å¤å¶å¨è½®æ¢ | | ç»å® [ç©å®¶ UID] | æ  | å¦ | ç§è/ç¾¤è/
+é¢é | å° UID ä¸ QQ è´¦å·ç»å® (ç¾¤è ä¸ é¢é ä¿¡æ¯ä¸äºé) | |
+è§£ç» | æ  | å¦ | ç§è/ç¾¤è/é¢é | å° UID ä¸ QQ è´¦å·è§£é¤ç»å®
+(ç¾¤è ä¸ é¢é ä¿¡æ¯ä¸äºé) | ## ð¼ï¸ ææå¾ ![Bridge](https://
+oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-api-query/Bridge.png) !
+[MapRotation](https://oss.hxiaoh.com/File/GitHub/Photos/nonebot-plugin-apex-
+api-query/MapRotation.png) ![Crafting](https://oss.hxiaoh.com/File/GitHub/
+Photos/nonebot-plugin-apex-api-query/Crafting.png) ## ð ToDo
+å¦æ¨ææ³è¦çåè½ï¼è¯·æäº¤ [Issues](https://github.com/H-xiaoH/
+nonebot-plugin-apex-api-query/issues) ã ## ð¸ è´è°¢ - [@nonebot](https://
+github.com/nonebot) å¼ºå¤§ç [NoneBot2 æºå¨äººæ¡æ¶](https://github.com/
+nonebot/nonebot2) - [@nonebot](https://github.com/nonebot) è®¢éåè½åºäº
+[APScheduler å®æ¶ä»»å¡æä»¶](https://github.com/nonebot/plugin-apscheduler)
+- [@nonebot](https://github.com/nonebot) æ¬å°æ°æ®å­å¨åè½åºäº
+[æ¬å°æ°æ®å­å¨](https://github.com/nonebot/plugin-localstore) - [@A-
+kirami](https://github.com/A-kirami) ä½¿ç¨å¶ NoneBot Plugin [README æ¨¡æ¿]
+(https://github.com/A-kirami/nonebot-plugin-template) - [@mobyw](https://
+github.com/mobyw) æå­è½¬å¾çåè½æºäº [è½»éæå­è½¬å¾çæä»¶]
+(https://github.com/mobyw/nonebot-plugin-txt2img)
```

