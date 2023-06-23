# Comparing `tmp/nonebot_plugin_bawiki-0.7.9.tar.gz` & `tmp/nonebot_plugin_bawiki-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.7.9.tar", last modified: Wed Jun  7 14:22:00 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.8.0.tar", last modified: Fri Jun 23 17:01:03 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.7.9.tar` & `nonebot_plugin_bawiki-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,45 @@
--rw-r--r--   0        0        0     1068 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/LICENSE
--rw-r--r--   0        0        0     7936 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/README.md
--rw-r--r--   0        0        0    14616 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0    23189 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/__main__.py
--rw-r--r--   0        0        0     1814 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0     5812 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_bawiki.py
--rw-r--r--   0        0        0     8291 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_gamekee.py
--rw-r--r--   0        0        0    18827 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_schaledb.py
--rw-r--r--   0        0        0     7390 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0    21514 2023-06-07 14:21:28.278101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gradient.png
--rw-r--r--   0        0        0      872 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/resource.py
--rw-r--r--   0        0        0     3555 2023-06-07 14:21:28.282101 nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1379 2023-06-07 14:22:00.566046 nonebot_plugin_bawiki-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     9275 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/LICENSE
+-rw-r--r--   0        0        0     9028 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/README.md
+-rw-r--r--   0        0        0      734 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/__init__.py
+-rw-r--r--   0        0        0     3739 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/arona.py
+-rw-r--r--   0        0        0     2320 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/calender.py
+-rw-r--r--   0        0        0     1265 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/clear_cache.py
+-rw-r--r--   0        0        0     1218 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/craft.py
+-rw-r--r--   0        0        0     1003 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/emoji.py
+-rw-r--r--   0        0        0     2580 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/event.py
+-rw-r--r--   0        0        0      976 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/furniture.py
+-rw-r--r--   0        0        0     6327 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/gacha.py
+-rw-r--r--   0        0        0     3555 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/global_future.py
+-rw-r--r--   0        0        0     1775 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/level_guide.py
+-rw-r--r--   0        0        0     1428 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/manga.py
+-rw-r--r--   0        0        0     4356 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/raid.py
+-rw-r--r--   0        0        0     3597 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_fav.py
+-rw-r--r--   0        0        0     1868 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_rank.py
+-rw-r--r--   0        0        0     1625 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_wiki_gamekee.py
+-rw-r--r--   0        0        0     2011 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/stu_wiki_schale.py
+-rw-r--r--   0        0        0     3375 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/time_atk.py
+-rw-r--r--   0        0        0     3255 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/command/voice.py
+-rw-r--r--   0        0        0     1152 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0        0 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/arona.py
+-rw-r--r--   0        0        0     5814 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/bawiki.py
+-rw-r--r--   0        0        0     9814 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/gamekee.py
+-rw-r--r--   0        0        0    18830 2023-06-23 17:00:11.616459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/schaledb.py
+-rw-r--r--   0        0        0     7390 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/gacha.py
+-rw-r--r--   0        0        0     1358 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/__init__.py
+-rw-r--r--   0        0        0     1784 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/manual.py
+-rw-r--r--   0        0        0     2216 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/pic_menu.py
+-rw-r--r--   0        0        0      919 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/__init__.py
+-rw-r--r--   0        0        0    21514 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-06-23 17:00:11.620459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-06-23 17:00:11.624459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-06-23 17:00:11.628459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gradient.png
+-rw-r--r--   0        0        0     4596 2023-06-23 17:00:11.628459 nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1481 2023-06-23 17:01:03.804653 nonebot_plugin_bawiki-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10479 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.8.0/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.7.9/LICENSE` & `nonebot_plugin_bawiki-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/README.md` & `nonebot_plugin_bawiki-0.8.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -100,46 +100,57 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置
 
-|         配置项         | 必填 | 默认值  |                          说明                           |
-| :--------------------: | :--: | :-----: | :-----------------------------------------------------: |
-|       `BA_PROXY`       |  否  | `None`  | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
-|  `BA_GACHA_COOL_DOWN`  |  否  |   `0`   |               每群每人的抽卡冷却，单位秒                |
-|  `BA_VOICE_USE_CARD`   |  否  | `False` |           是否使用自定义音乐卡片发送角色语音            |
-|    `BA_GAMEKEE_URL`    |  否  |   ...   |                  GameKee 数据源的地址                   |
-|    `BA_SCHALE_URL`     |  否  |   ...   |                SchaleDB Json 数据的地址                 |
-| `BA_SCHALE_MIRROR_URL` |  否  |   ...   |                 SchaleDB 网页截图的地址                 |
-|   `BA_BAWIKI_DB_URL`   |  否  |   ...   |                   bawiki-data 的地址                    |
+|            配置项             | 必填 | 默认值  |                           说明                            |
+| :---------------------------: | :--: | :-----: | :-------------------------------------------------------: |
+|          `BA_PROXY`           |  否  | `None`  |  访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理  |
+|     `BA_GACHA_COOL_DOWN`      |  否  |   `0`   |                每群每人的抽卡冷却，单位秒                 |
+|      `BA_VOICE_USE_CARD`      |  否  | `False` |            是否使用自定义音乐卡片发送角色语音             |
+|       `BA_GAMEKEE_URL`        |  否  |   ...   |                   GameKee 数据源的地址                    |
+|        `BA_SCHALE_URL`        |  否  |   ...   |                SchaleDB Json 数据源的地址                 |
+|    `BA_SCHALE_MIRROR_URL`     |  否  |   ...   |                  SchaleDB 网页截图的地址                  |
+|      `BA_BAWIKI_DB_URL`       |  否  |   ...   |                    bawiki-data 的地址                     |
+|      `BA_ARONA_API_URL`       |  否  |   ...   |                  Arona Bot 数据源的地址                   |
+|      `BA_ARONA_CDN_URL`       |  否  |   ...   |                  Arona Bot 图片 CDN 地址                  |
+| `BA_CLEAR_REQ_CACHE_INTERVAL` |  否  |   `3`   |             插件清理请求缓存的间隔，单位小时              |
+|  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  |   ...   | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
 
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
 **现在 BAWiki 会自动帮你把 PicMenu 的字体设为系统已安装的字体，再也不需要麻烦的手动配置了，好耶~**
 
-如果你不想用 PicMenu 的话，那么请看 [\_\_init\_\_.py](https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/__init__.py)
+如果你不想用 PicMenu 的话，那么使用 `ba帮助` 指令即可；  
+如果装载了 PicMenu，`ba帮助` 指令会调用 PicMenu 来生成帮助图片并发送
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
+### [GameKee](https://ba.gamekee.com/) & [SchaleDB](https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://doc.arona.diyigemt.com/api/)
+
+- 插件数据源提供
+
+<!--
 ### [RainNight0](https://github.com/RainNight0)
 
 - 日程表 html 模板提供（已弃用）
+-->
 
 ### `bawiki-data` 数据源贡献列表
 
 - 见 [bawiki-data](http://github.com/lgc2333/bawiki-data)
 
 ## 💰 赞助
 
@@ -151,14 +162,26 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.0
+
+- 整理项目结构
+- 添加内置帮助指令 `ba帮助`
+- 添加 Arona Bot 数据源指令 `arona`
+- 添加了配置项 `BA_ARONA_API_URL`、`BA_ARONA_CDN_URL`、`BA_CLEAR_REQ_CACHE_INTERVAL`、`BA_AUTO_CLEAR_ARONA_CACHE`
+- 其他小更改（更换 `aiohttp` 为 `httpx` 等）
+
+### 0.7.10
+
+- 添加指令 `ba关卡`
+
 ### 0.7.9
 
 - 添加配置项 `BA_VOICE_USE_CARD`
 
 ### 0.7.8
 
 - 🎉 NoneBot 2.0 🚀
```

#### html2text {}

```diff
@@ -16,44 +16,56 @@
 pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
 nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
 conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :-----: | :-------------
-----------------------------------------: | | `BA_PROXY` | å¦ | `None` |
-è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
-`BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
-`BA_VOICE_USE_CARD` | å¦ | `False` |
+é»è®¤å¼ | è¯´æ | | :---------------------------: | :--: | :-----: | :------
+-------------------------------------------------: | | `BA_PROXY` | å¦ |
+`None` | è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç |
+| `BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ |
+| `BA_VOICE_USE_CARD` | å¦ | `False` |
 æ¯å¦ä½¿ç¨èªå®ä¹é³ä¹å¡çåéè§è²è¯­é³ | | `BA_GAMEKEE_URL` | å¦
 | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` | å¦ | ... | SchaleDB
-Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
+Json æ°æ®æºçå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
 ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
-çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-PicMenu](https:
-//github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
+çå°å | | `BA_ARONA_API_URL` | å¦ | ... | Arona Bot æ°æ®æºçå°å | |
+`BA_ARONA_CDN_URL` | å¦ | ... | Arona Bot å¾ç CDN å°å | |
+`BA_CLEAR_REQ_CACHE_INTERVAL` | å¦ | `3` |
+æä»¶æ¸çè¯·æ±ç¼å­çé´éï¼åä½å°æ¶ | |
+`BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | ... |
+æ¯å¦å¨æä»¶æ¯æ¬¡å è½½æ¶èªå¨æ¸çä» Arona Bot
+æ°æ®æºç¼å­çå¾ç | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
+PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
 ä¼èªå¨å¸®ä½ æ PicMenu
 çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
-å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹è¯·ç [\_\_init\_\_.py](https://
-github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/
-__init__.py) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/
-lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)
-é®ç®±ï¼
-126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
-æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
+å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹ä½¿ç¨ `baå¸®å©` æä»¤å³å¯ï¼
+å¦æè£è½½äº PicMenuï¼`baå¸®å©` æä»¤ä¼è°ç¨ PicMenu
+æ¥çæå¸®å©å¾çå¹¶åé ## ð èç³» QQï¼3076823485 Telegramï¼
+[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
+?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
+(https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
+doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ### 0.7.8 - ð NoneBot 2.0 ð
-### 0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ###
-0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
-ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
-æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.8.0 - æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona
+Bot æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
+`BA_ARONA_API_URL`ã`BA_ARONA_CDN_URL`ã`BA_CLEAR_REQ_CACHE_INTERVAL`ã`BA_AUTO_CLEAR_ARONA_CACHE`
+- å¶ä»å°æ´æ¹ï¼æ´æ¢ `aiohttp` ä¸º `httpx` ç­ï¼ ### 0.7.10 -
+æ·»å æä»¤ `baå³å¡` ### 0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ###
+0.7.8 - ð NoneBot 2.0 ð ### 0.7.7 - ä¿®å¤ bug ### 0.7.6 -
+ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
+æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
+### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
+ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/help/pic_menu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 import json
+from io import BytesIO
 from pathlib import Path
-from typing import Optional
+from typing import Union, cast
 
-from nonebot import get_available_plugin_names, get_driver, logger
+from nonebot import get_available_plugin_names, logger, require
+from nonebot.adapters.onebot.v11 import MessageSegment
+from nonebot.internal.adapter import Message
+from nonebot.internal.matcher import Matcher
+from nonebot.params import CommandArg
+from PIL import Image
 from pil_utils.fonts import get_proper_font
-from pydantic import BaseModel, validator
 
+from ..command import help_list
 
-class Cfg(BaseModel):
-    ba_proxy: Optional[str] = None
-    ba_gacha_cool_down: int = 0
-    ba_voice_use_card: bool = False
-
-    ba_gamekee_url: str = "https://ba.gamekee.com/"
-    ba_schale_url: str = "https://schale.lgc.cyberczy.xyz/"
-    ba_schale_mirror_url: str = "https://schale.lgc.cyberczy.xyz/"
-    ba_bawiki_db_url: str = "https://bawiki.lgc.cyberczy.xyz/"
-
-    @validator(
-        "ba_gamekee_url",
-        "ba_schale_url",
-        "ba_schale_mirror_url",
-        "ba_bawiki_db_url",
+if "nonebot_plugin_PicMenu" not in get_available_plugin_names():
+    raise ImportError
+
+require("nonebot_plugin_PicMenu")
+
+from nonebot_plugin_PicMenu import menu_manager  # noqa: E402
+
+usage = "请使用指令 [ba帮助 <ft color=(238,120,0)>功能名称或序号</ft>] 查看某功能详细介绍"
+extra = {"menu_template": "default", "menu_data": help_list}
+
+
+def save_img_to_io(img: Image.Image):
+    img = img.convert("RGB")
+    img_io = BytesIO()
+    img.save(img_io, "jpeg")
+    img_io.seek(0)
+    return img_io
+
+
+async def help_handle(matcher: Matcher, arg_msg: Message = CommandArg()):
+    arg = arg_msg.extract_plain_text().strip()
+    img = cast(
+        Union[str, Image.Image],
+        (
+            menu_manager.generate_plugin_menu_image("BAWiki")
+            if not arg
+            else menu_manager.generate_func_details_image("BAWiki", arg)
+        ),
     )
-    def _(cls, val: str):  # noqa: N805
-        if not ((val.startswith(("https://", "http://"))) and val.endswith("/")):
-            raise ValueError('自定义的 URL 请以 "http(s)://" 开头，以 "/" 结尾')
-        return val
 
+    if isinstance(img, str):
+        await matcher.finish(f'出错了，可能未找到功能 "{arg}"')
 
-config = Cfg.parse_obj(get_driver().config.dict())
+    await matcher.finish(MessageSegment.image(save_img_to_io(img)))
 
 
 # 给 PicMenu 用户上个默认字体
 def set_pic_menu_font():
     pic_menu_dir = Path.cwd() / "menu_config"
     pic_menu_config = pic_menu_dir / "config.json"
 
@@ -45,12 +62,11 @@
         == "font_path"
     ):
         path = str(get_proper_font("国").path.resolve())
         pic_menu_config.write_text(json.dumps({"default": path}), encoding="u8")
         logger.info("检测到 PicMenu 已加载并且未配置字体，已自动帮您配置系统字体")
 
 
-if "nonebot_plugin_PicMenu" in get_available_plugin_names():
-    try:
-        set_pic_menu_font()
-    except:
-        logger.exception("配置 PicMenu 字体失败")
+try:
+    set_pic_menu_font()
+except:
+    logger.exception("配置 PicMenu 字体失败")
```

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_bawiki.py` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/bawiki.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime
 from io import BytesIO
 from typing import Any, Dict, List, Literal, Optional, TypedDict, cast, overload
 
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pil_utils import BuildImage
 
-from .config import config
-from .util import async_req, recover_alia
+from ..config import config
+from ..util import async_req, recover_alia
 
 
 class MangaDict(TypedDict):
     cid: int
     title: str
     detail: str
     pics: List[str]
```

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_gamekee.py` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/gamekee.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import asyncio
 import contextlib
+import itertools
 import re
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from io import BytesIO
-from typing import Any, Dict, List, Union, cast
+from typing import Any, Dict, List, NoReturn, Union, cast
 
 from bs4 import BeautifulSoup, ResultSet, Tag
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
+from nonebot.internal.matcher import Matcher
 from nonebot_plugin_htmlrender import get_new_page
 from PIL.Image import Resampling
 from pil_utils import BuildImage, text2image
 from playwright.async_api import Page
 
-from .config import config
-from .resource import RES_CALENDER_BANNER, RES_GRADIENT_BG
-from .util import async_req, parse_time_delta
+from ..config import config
+from ..resource import RES_CALENDER_BANNER, RES_GRADIENT_BG
+from ..util import async_req, parse_time_delta
 
 
-async def game_kee_request(url, **kwargs) -> Union[List, Dict[str, Any]]:
+async def game_kee_request(url: str, **kwargs) -> Union[List, Dict[str, Any]]:
     ret = cast(
         dict,
         await async_req(
-            url,
+            f"{config.ba_gamekee_url}{url}",
             headers={"game-id": "0", "game-alias": "ba"},
             proxy=None,
             **kwargs,
         ),
     )
     if ret["code"] != 0:
         raise ConnectionError(ret["msg"])
     return ret["data"]
 
 
-async def game_kee_get_calender():
-    ret = cast(list, await game_kee_request(f"{config.ba_gamekee_url}v1/wiki/index"))
+async def game_kee_get_calender() -> List[dict]:
+    ret = cast(list, await game_kee_request("v1/wiki/index"))
 
     for i in ret:
         if i["module"]["id"] == 12:
             li: list = i["list"]
 
             now = time.time()
             li = [x for x in li if (now < x["end_at"])]
@@ -49,35 +51,35 @@
             li.sort(key=lambda x: now < x["begin_at"])
             li.sort(key=lambda x: x["importance"], reverse=True)
             return li
 
     return []
 
 
-async def game_kee_get_stu_li():
-    ret = cast(dict, await game_kee_request(f"{config.ba_gamekee_url}v1/wiki/entry"))
+async def game_kee_get_stu_li() -> Dict[str, dict]:
+    ret = cast(dict, await game_kee_request("v1/wiki/entry"))
 
     for i in ret["entry_list"]:
         if i["id"] == 23941:
             for ii in i["child"]:
                 if ii["id"] == 49443:
                     return {x["name"]: x for x in ii["child"]}
 
     return {}
 
 
-async def game_kee_get_stu_cid_li():
+async def game_kee_get_stu_cid_li() -> Dict[str, int]:
     return {x: y["content_id"] for x, y in (await game_kee_get_stu_li()).items()}
 
 
-def game_kee_page_url(sid):
+def game_kee_page_url(sid: int) -> str:
     return f"{config.ba_gamekee_url}{sid}.html"
 
 
-async def game_kee_get_page(url):
+async def game_kee_get_page(url: str) -> bytes:
     async with cast(Page, get_new_page()) as page:
         await page.goto(url, timeout=60 * 1000)
 
         # 删掉header
         await page.add_script_tag(
             content='document.getElementsByClassName("wiki-header")'
             ".forEach((v)=>{v.remove()})",
@@ -96,24 +98,37 @@
 
         element = await page.query_selector('xpath=//div[@class="wiki-detail-body"]')
         if not element:
             raise ValueError
         return await element.screenshot()
 
 
-async def game_kee_calender():
+async def send_wiki_page(sid: int, matcher: Matcher) -> NoReturn:
+    url = game_kee_page_url(sid)
+    await matcher.send(f"请稍等，正在截取Wiki页面……\n{url}")
+
+    try:
+        img = await game_kee_get_page(url)
+    except:
+        logger.exception(f"截取wiki页面出错 {url}")
+        await matcher.finish("截取页面出错，请检查后台输出")
+
+    await matcher.finish(MessageSegment.image(img))
+
+
+async def game_kee_calender() -> Union[MessageSegment, str]:
     ret = await game_kee_get_calender()
     if not ret:
         return "没有获取到GameKee日程表数据"
 
     pic = await game_kee_get_calender_page(ret)
     return MessageSegment.image(pic)
 
 
-async def game_kee_get_calender_page(ret, has_pic=True):
+async def game_kee_get_calender_page(ret, has_pic=True) -> BytesIO:
     now = datetime.now()
 
     async def draw(it: dict):
         _p = None
         if has_pic and (_p := it.get("picture")):
             try:
                 _p = (
@@ -226,18 +241,18 @@
     for p in pics:
         bg.paste(p.circle_corner(10), (50, index), True)
         index += p.height + 50
 
     return bg.save_jpg()
 
 
-async def game_kee_grab_l2d(cid):
+async def game_kee_grab_l2d(cid) -> List[str]:
     ret = cast(
         dict,
-        await game_kee_request(f"{config.ba_gamekee_url}v1/content/detail/{cid}"),
+        await game_kee_request(f"v1/content/detail/{cid}"),
     )
     content: str = ret["content"]
 
     x = content.find('<div class="input-wrapper">官方介绍</div>')
     x = content.find('class="slide-item" data-index="2"', x)
     y = content.find('data-index="3"', x)
 
@@ -256,15 +271,15 @@
     url: str
 
 
 async def game_kee_get_voice(cid) -> List[GameKeeVoice]:
     wiki_html = (
         cast(
             dict,
-            await game_kee_request(f"{config.ba_gamekee_url}v1/content/detail/{cid}"),
+            await game_kee_request(f"v1/content/detail/{cid}"),
         )
     )["content"]
     bs = BeautifulSoup(wiki_html, "lxml")
     audios = bs.select(".mould-table>tbody>tr>td>div>div>audio")
 
     parsed: List[GameKeeVoice] = []
     for au in audios:
@@ -278,7 +293,35 @@
         jp = "\n".join(tds[2].stripped_strings)
 
         tr2 = tr1.next_sibling
         cn = "\n".join(tr2.stripped_strings)  # type: ignore
         parsed.append(GameKeeVoice(title, jp, cn, url))
 
     return parsed
+
+
+async def get_level_list() -> Dict[str, int]:
+    entry = cast(dict, await game_kee_request("v1/wiki/entry"))
+    entry_list: List[Dict] = entry["entry_list"]
+    guide_entry: List[Dict] = next(x["child"] for x in entry_list if x["id"] == 50284)
+    levels = itertools.chain(
+        *(x["child"] for x in guide_entry if cast(str, x["name"]).endswith("章")),
+    )
+    return {
+        n.upper(): x["content_id"]
+        for x in levels
+        if re.match(r"^(H)?(TR|\d+)-(\d+)$", (n := cast(str, x["name"])))
+    }
+
+
+async def extract_content_pic(cid: int) -> List[str]:
+    wiki_html = (
+        cast(
+            dict,
+            await game_kee_request(f"v1/content/detail/{cid}"),
+        )
+    )["content"]
+    bs = BeautifulSoup(wiki_html, "lxml")
+    img_elem = bs.find_all("img")
+    img_urls = cast(List[str], [x["src"] for x in img_elem])
+    img_urls = [f"https:{x}" if x.startswith("//") else x for x in img_urls]
+    return img_urls
```

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/data_schaledb.py` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/data/schaledb.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot_plugin_htmlrender import get_new_page
 from PIL import Image, ImageFilter
 from PIL.Image import Resampling
 from pil_utils import BuildImage, text2image
 from playwright.async_api import Page, ViewportSize
 
-from .config import config
-from .resource import RES_CALENDER_BANNER, RES_GRADIENT_BG
-from .util import async_req, img_invert_rgba, parse_time_delta
+from ..config import config
+from ..resource import RES_CALENDER_BANNER, RES_GRADIENT_BG
+from ..util import async_req, img_invert_rgba, parse_time_delta
 
 PAGE_KWARGS = {
     "is_mobile": True,
     "viewport": ViewportSize(width=767, height=800),
 }
```

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/gacha.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import aiofiles
 from nonebot import logger
 from nonebot.adapters.onebot.v11 import MessageSegment
 from pil_utils import BuildImage
 
 from .config import config
-from .data_schaledb import schale_get, schale_get_stu_dict
+from .data.schaledb import schale_get, schale_get_stu_dict
 from .resource import (
     DATA_PATH,
     RES_GACHA_BG,
     RES_GACHA_CARD_BG,
     RES_GACHA_CARD_MASK,
     RES_GACHA_NEW,
     RES_GACHA_PICKUP,
```

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/calender_banner.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_new.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_star.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/res/gradient.png` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/resource.py` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/resource/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from pathlib import Path
 
 from pil_utils import BuildImage
 
 RES_PATH = Path(__file__).parent / "res"
 
+CACHE_PATH = Path.cwd() / "cache" / "BAWiki"
+if not CACHE_PATH.exists():
+    CACHE_PATH.mkdir(parents=True)
+
 DATA_PATH = Path.cwd() / "data" / "BAWiki"
 if not DATA_PATH.exists():
     DATA_PATH.mkdir(parents=True)
 
 RES_CALENDER_BANNER = BuildImage.open(RES_PATH / "calender_banner.png")
-# RES_SCHALE_BG = BuildImage.open(RES_PATH / "schale_bg.jpg")
 RES_GRADIENT_BG = BuildImage.open(RES_PATH / "gradient.png")
 RES_GACHA_BG = BuildImage.open(RES_PATH / "gacha_bg.png")
 RES_GACHA_CARD_BG = BuildImage.open(RES_PATH / "gacha_card_bg.png")
 RES_GACHA_CARD_MASK = BuildImage.open(RES_PATH / "gacha_card_mask.png").convert("RGBA")
 RES_GACHA_NEW = BuildImage.open(RES_PATH / "gacha_new.png")
 RES_GACHA_PICKUP = BuildImage.open(RES_PATH / "gacha_pickup.png")
 RES_GACHA_STAR = BuildImage.open(RES_PATH / "gacha_star.png")
```

### Comparing `nonebot_plugin_bawiki-0.7.9/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.8.0/nonebot_plugin_bawiki/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,137 @@
 import datetime
 import json
 from copy import deepcopy
-from typing import (
-    Any,
-    Dict,
-    Iterable,
-    List,
-    Literal,
-    Optional,
-    TypeVar,
-    Union,
-    overload,
-)
+from dataclasses import dataclass
+from typing import Any, Dict, Iterable, List, Literal, Optional, TypeVar, overload
 
-from aiohttp import ClientSession
+from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import Message
+from nonebot_plugin_apscheduler import scheduler
 from PIL import Image, ImageOps
 
 from .config import config
 
 _T = TypeVar("_T")
 
-req_cache = {}
+req_cache: Dict[str, "RequestCache"] = {}
+
+
+@dataclass
+class RequestCache:
+    method: str
+    raw: bool
+    json: bool
+    params: str
+    content: Any
+
+
+def get_req_cache(
+    url: str,
+    method: Optional[str] = None,
+    raw: Optional[bool] = None,
+    json: Optional[bool] = None,
+    params: Optional[str] = None,
+) -> Optional[Any]:
+    if (c := req_cache.get(url)) and (
+        (method is None or method == c.method)
+        and (raw is None or raw == c.raw)
+        and (json is None or json == c.json)
+        and (params is None or params == c.params)
+    ):
+        return c.content
+    return None
+
+
+def clear_req_cache():
+    req_cache.clear()
+
+
+if config.ba_clear_req_cache_interval > 0:
+
+    @scheduler.scheduled_job("interval", hours=config.ba_clear_req_cache_interval)
+    async def _():
+        clear_req_cache()
 
 
 @overload
 async def async_req(
     url,
     *,
     is_json: Literal[True] = True,
     raw: Literal[False] = False,
-    ignore_cache=False,
-    proxy=config.ba_proxy,
-    method="GET",
-    session: Optional[ClientSession] = None,
+    ignore_cache: bool = False,
+    proxy: Optional[str] = config.ba_proxy,
+    method: str = "GET",
+    params: Optional[Dict[str, Any]] = None,
     **kwargs,
-) -> Union[Dict[str, Any], list]:
+) -> Any:
     ...
 
 
 @overload
 async def async_req(
     url,
     *,
     is_json: Literal[False] = False,
     raw: Literal[True] = True,
-    ignore_cache=False,
-    proxy=config.ba_proxy,
-    method="GET",
-    session: Optional[ClientSession] = None,
+    ignore_cache: bool = False,
+    proxy: Optional[str] = config.ba_proxy,
+    method: str = "GET",
+    params: Optional[Dict[str, Any]] = None,
     **kwargs,
 ) -> bytes:
     ...
 
 
 @overload
 async def async_req(
     url,
     *,
     is_json: Literal[False] = False,
     raw: Literal[False] = False,
-    ignore_cache=False,
-    proxy=config.ba_proxy,
-    method="GET",
-    session: Optional[ClientSession] = None,
+    ignore_cache: bool = False,
+    proxy: Optional[str] = config.ba_proxy,
+    method: str = "GET",
+    params: Optional[Dict[str, Any]] = None,
     **kwargs,
 ) -> str:
     ...
 
 
 async def async_req(
     url,
     is_json=True,
     raw=False,
     ignore_cache=False,
     proxy=config.ba_proxy,
     method="GET",
-    session: Optional[ClientSession] = None,
+    params=None,
     **kwargs,
 ):
-    if (not ignore_cache) and (c := req_cache.get(url)):
-        return c
+    param_json = json.dumps(params) if params else "{}"
 
-    async with (session or ClientSession()) as c:
-        async with c.request(method, url, **kwargs, proxy=proxy) as r:
-            ret = (await r.read()) if raw else (await r.text())
-            if is_json and (not raw):
-                ret = json.loads(ret)
-            req_cache[url] = ret
-            return ret
+    if (not ignore_cache) and (
+        c := get_req_cache(url, method, raw, is_json, param_json)
+    ):
+        return c
 
+    async with AsyncClient(proxies=proxy) as cli:
+        resp = await cli.request(method, url, params=params, **kwargs)
+        resp.raise_for_status()
+
+        if (not raw) and is_json:
+            ret = resp.json()
+        elif raw:
+            ret = resp.content
+        else:
+            ret = resp.text
 
-def clear_req_cache():
-    req_cache.clear()
+        req_cache[url] = RequestCache(method, raw, is_json, param_json, ret)
+        return ret
 
 
 def format_timestamp(t: int):
     return datetime.datetime.fromtimestamp(t).strftime("%Y-%m-%d %H:%M:%S")
 
 
 def recover_alia(origin: str, alia_dict: Dict[str, List[str]]):
```

### Comparing `nonebot_plugin_bawiki-0.7.9/pyproject.toml` & `nonebot_plugin_bawiki-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.7.9"
+version = "0.8.0"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
-    "aiohttp>=3.8.3",
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.1",
     "nonebot-plugin-htmlrender>=0.2.0.1",
     "nonebot-plugin-apscheduler>=0.2.0",
     "beautifulsoup4>=4.11.1",
     "lxml>=4.9.1",
     "pil-utils>=0.1.4",
+    "httpx>=0.24.1",
+    "pypinyin>=0.49.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 keywords = [
     "blue archive",
     "nonebot",
     "nonebot2",
@@ -41,14 +42,19 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc2333/nonebot-plugin-bawiki/"
 
+[project.optional-dependencies]
+menu = [
+    "nonebot-plugin-PicMenu>=0.2",
+]
+
 [tool.pdm.build]
 includes = []
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `nonebot_plugin_bawiki-0.7.9/PKG-INFO` & `nonebot_plugin_bawiki-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.7.9
+Version: 0.8.0
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -16,22 +16,25 @@
 Classifier: Topic :: Games/Entertainment :: Side-Scrolling/Arcade Games
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
 Project-URL: Homepage, https://github.com/lgc2333/nonebot-plugin-bawiki/
 Requires-Python: <4.0,>=3.8
-Requires-Dist: aiohttp>=3.8.3
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.1.1
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.1
 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: lxml>=4.9.1
 Requires-Dist: pil-utils>=0.1.4
+Requires-Dist: httpx>=0.24.1
+Requires-Dist: pypinyin>=0.49.0
+Requires-Dist: nonebot-plugin-PicMenu>=0.2; extra == "menu"
+Provides-Extra: menu
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/bawiki/nonebot-plugin-bawiki.png" width="200" height="200" alt="BAWiki"></a>
 </div>
@@ -132,46 +135,57 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置
 
-|         配置项         | 必填 | 默认值  |                          说明                           |
-| :--------------------: | :--: | :-----: | :-----------------------------------------------------: |
-|       `BA_PROXY`       |  否  | `None`  | 访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理 |
-|  `BA_GACHA_COOL_DOWN`  |  否  |   `0`   |               每群每人的抽卡冷却，单位秒                |
-|  `BA_VOICE_USE_CARD`   |  否  | `False` |           是否使用自定义音乐卡片发送角色语音            |
-|    `BA_GAMEKEE_URL`    |  否  |   ...   |                  GameKee 数据源的地址                   |
-|    `BA_SCHALE_URL`     |  否  |   ...   |                SchaleDB Json 数据的地址                 |
-| `BA_SCHALE_MIRROR_URL` |  否  |   ...   |                 SchaleDB 网页截图的地址                 |
-|   `BA_BAWIKI_DB_URL`   |  否  |   ...   |                   bawiki-data 的地址                    |
+|            配置项             | 必填 | 默认值  |                           说明                            |
+| :---------------------------: | :--: | :-----: | :-------------------------------------------------------: |
+|          `BA_PROXY`           |  否  | `None`  |  访问 `SchaleDB`、`bawiki-data` 的 json 数据时使用的代理  |
+|     `BA_GACHA_COOL_DOWN`      |  否  |   `0`   |                每群每人的抽卡冷却，单位秒                 |
+|      `BA_VOICE_USE_CARD`      |  否  | `False` |            是否使用自定义音乐卡片发送角色语音             |
+|       `BA_GAMEKEE_URL`        |  否  |   ...   |                   GameKee 数据源的地址                    |
+|        `BA_SCHALE_URL`        |  否  |   ...   |                SchaleDB Json 数据源的地址                 |
+|    `BA_SCHALE_MIRROR_URL`     |  否  |   ...   |                  SchaleDB 网页截图的地址                  |
+|      `BA_BAWIKI_DB_URL`       |  否  |   ...   |                    bawiki-data 的地址                     |
+|      `BA_ARONA_API_URL`       |  否  |   ...   |                  Arona Bot 数据源的地址                   |
+|      `BA_ARONA_CDN_URL`       |  否  |   ...   |                  Arona Bot 图片 CDN 地址                  |
+| `BA_CLEAR_REQ_CACHE_INTERVAL` |  否  |   `3`   |             插件清理请求缓存的间隔，单位小时              |
+|  `BA_AUTO_CLEAR_ARONA_CACHE`  |  否  |   ...   | 是否在插件每次加载时自动清理从 Arona Bot 数据源缓存的图片 |
 
 ## 🎉 使用
 
 ### 指令表
 
 兼容 [nonebot-plugin-PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu)
 
 **现在 BAWiki 会自动帮你把 PicMenu 的字体设为系统已安装的字体，再也不需要麻烦的手动配置了，好耶~**
 
-如果你不想用 PicMenu 的话，那么请看 [\_\_init\_\_.py](https://github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/__init__.py)
+如果你不想用 PicMenu 的话，那么使用 `ba帮助` 指令即可；  
+如果装载了 PicMenu，`ba帮助` 指令会调用 PicMenu 来生成帮助图片并发送
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
 
 ## 💡 鸣谢
 
+### [GameKee](https://ba.gamekee.com/) & [SchaleDB](https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://doc.arona.diyigemt.com/api/)
+
+- 插件数据源提供
+
+<!--
 ### [RainNight0](https://github.com/RainNight0)
 
 - 日程表 html 模板提供（已弃用）
+-->
 
 ### `bawiki-data` 数据源贡献列表
 
 - 见 [bawiki-data](http://github.com/lgc2333/bawiki-data)
 
 ## 💰 赞助
 
@@ -183,14 +197,26 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.8.0
+
+- 整理项目结构
+- 添加内置帮助指令 `ba帮助`
+- 添加 Arona Bot 数据源指令 `arona`
+- 添加了配置项 `BA_ARONA_API_URL`、`BA_ARONA_CDN_URL`、`BA_CLEAR_REQ_CACHE_INTERVAL`、`BA_AUTO_CLEAR_ARONA_CACHE`
+- 其他小更改（更换 `aiohttp` 为 `httpx` 等）
+
+### 0.7.10
+
+- 添加指令 `ba关卡`
+
 ### 0.7.9
 
 - 添加配置项 `BA_VOICE_USE_CARD`
 
 ### 0.7.8
 
 - 🎉 NoneBot 2.0 🚀
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.9 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.8.0 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy Classifier:
 Topic :: Games/Entertainment :: Side-Scrolling/Arcade Games Classifier: Topic
 :: Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content :: Wiki Project-URL: Homepage, https://github.com/
 lgc2333/nonebot-plugin-bawiki/ Requires-Python: <4.0,>=3.8 Requires-Dist:
-aiohttp>=3.8.3 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-
-onebot>=2.1.1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.1 Requires-Dist:
-nonebot-plugin-apscheduler>=0.2.0 Requires-Dist: beautifulsoup4>=4.11.1
-Requires-Dist: lxml>=4.9.1 Requires-Dist: pil-utils>=0.1.4 Description-Content-
-Type: text/markdown
+nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.1.1 Requires-Dist:
+nonebot-plugin-htmlrender>=0.2.0.1 Requires-Dist: nonebot-plugin-
+apscheduler>=0.2.0 Requires-Dist: beautifulsoup4>=4.11.1 Requires-Dist:
+lxml>=4.9.1 Requires-Dist: pil-utils>=0.1.4 Requires-Dist: httpx>=0.24.1
+Requires-Dist: pypinyin>=0.49.0 Requires-Dist: nonebot-plugin-PicMenu>=0.2;
+extra == "menu" Provides-Extra: menu Description-Content-Type: text/markdown
                                    [BAWiki]
 # NoneBot-Plugin-BAWiki _â¨ åºäº NoneBot2 çç¢§èæ¡£æ¡ Wiki æä»¶ â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð¬ åè¨
 è¯éåä½å¸®å¿æ´æ°æä»¶æ°æ®æºä»åºï¼è½å¸®è¿ä¸ªå°å°æä»¶è´¡ç®å¾®èä¹åï¼éäººææ¿ä¸å°½ï¼ï¼
 [ç¹å»è·³è½¬ bawiki-data æ¥çè¯¦ç»è´¡ç®è¯´æ](https://github.com/lgc2333/
 bawiki-data) ## ð ä»ç» ä¸ä¸ªç¢§èæ¡£æ¡ç Wiki
@@ -35,44 +36,56 @@
 pip ```bash pip install nonebot-plugin-bawiki ```   pdm ```bash pdm add
 nonebot-plugin-bawiki ```   poetry ```bash poetry add nonebot-plugin-bawiki ```
 conda ```bash conda install nonebot-plugin-bawiki ```  æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_bawiki" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | | :--------------------: | :--: | :-----: | :-------------
-----------------------------------------: | | `BA_PROXY` | å¦ | `None` |
-è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç | |
-`BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ | |
-`BA_VOICE_USE_CARD` | å¦ | `False` |
+é»è®¤å¼ | è¯´æ | | :---------------------------: | :--: | :-----: | :------
+-------------------------------------------------: | | `BA_PROXY` | å¦ |
+`None` | è®¿é® `SchaleDB`ã`bawiki-data` ç json æ°æ®æ¶ä½¿ç¨çä»£ç |
+| `BA_GACHA_COOL_DOWN` | å¦ | `0` | æ¯ç¾¤æ¯äººçæ½å¡å·å´ï¼åä½ç§ |
+| `BA_VOICE_USE_CARD` | å¦ | `False` |
 æ¯å¦ä½¿ç¨èªå®ä¹é³ä¹å¡çåéè§è²è¯­é³ | | `BA_GAMEKEE_URL` | å¦
 | ... | GameKee æ°æ®æºçå°å | | `BA_SCHALE_URL` | å¦ | ... | SchaleDB
-Json æ°æ®çå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
+Json æ°æ®æºçå°å | | `BA_SCHALE_MIRROR_URL` | å¦ | ... | SchaleDB
 ç½é¡µæªå¾çå°å | | `BA_BAWIKI_DB_URL` | å¦ | ... | bawiki-data
-çå°å | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-PicMenu](https:
-//github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
+çå°å | | `BA_ARONA_API_URL` | å¦ | ... | Arona Bot æ°æ®æºçå°å | |
+`BA_ARONA_CDN_URL` | å¦ | ... | Arona Bot å¾ç CDN å°å | |
+`BA_CLEAR_REQ_CACHE_INTERVAL` | å¦ | `3` |
+æä»¶æ¸çè¯·æ±ç¼å­çé´éï¼åä½å°æ¶ | |
+`BA_AUTO_CLEAR_ARONA_CACHE` | å¦ | ... |
+æ¯å¦å¨æä»¶æ¯æ¬¡å è½½æ¶èªå¨æ¸çä» Arona Bot
+æ°æ®æºç¼å­çå¾ç | ## ð ä½¿ç¨ ### æä»¤è¡¨ å¼å®¹ [nonebot-plugin-
+PicMenu](https://github.com/hamo-reid/nonebot_plugin_PicMenu) **ç°å¨ BAWiki
 ä¼èªå¨å¸®ä½ æ PicMenu
 çå­ä½è®¾ä¸ºç³»ç»å·²å®è£çå­ä½ï¼åä¹ä¸éè¦éº»ç¦çæå¨éç½®äºï¼å¥½è¶~**
-å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹è¯·ç [\_\_init\_\_.py](https://
-github.com/lgc2333/nonebot-plugin-bawiki/blob/master/nonebot_plugin_bawiki/
-__init__.py) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/
-lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)
-é®ç®±ï¼
-126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
-æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
+å¦æä½ ä¸æ³ç¨ PicMenu çè¯ï¼é£ä¹ä½¿ç¨ `baå¸®å©` æä»¤å³å¯ï¼
+å¦æè£è½½äº PicMenuï¼`baå¸®å©` æä»¤ä¼è°ç¨ PicMenu
+æ¥çæå¸®å©å¾çå¹¶åé ## ð èç³» QQï¼3076823485 Telegramï¼
+[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
+?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+126.com> ## ð¡ é¸£è°¢ ### [GameKee](https://ba.gamekee.com/) & [SchaleDB]
+(https://lonqie.github.io/SchaleDB/) & [Arona Bot](https://
+doc.arona.diyigemt.com/api/) - æä»¶æ°æ®æºæä¾  ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ### 0.7.8 - ð NoneBot 2.0 ð
-### 0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ###
-0.7.5 - æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
-ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
-æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.8.0 - æ´çé¡¹ç®ç»æ - æ·»å åç½®å¸®å©æä»¤ `baå¸®å©` - æ·»å  Arona
+Bot æ°æ®æºæä»¤ `arona` - æ·»å äºéç½®é¡¹
+`BA_ARONA_API_URL`ã`BA_ARONA_CDN_URL`ã`BA_CLEAR_REQ_CACHE_INTERVAL`ã`BA_AUTO_CLEAR_ARONA_CACHE`
+- å¶ä»å°æ´æ¹ï¼æ´æ¢ `aiohttp` ä¸º `httpx` ç­ï¼ ### 0.7.10 -
+æ·»å æä»¤ `baå³å¡` ### 0.7.9 - æ·»å éç½®é¡¹ `BA_VOICE_USE_CARD` ###
+0.7.8 - ð NoneBot 2.0 ð ### 0.7.7 - ä¿®å¤ bug ### 0.7.6 -
+ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
+æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
+### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
+ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

