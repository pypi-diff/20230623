# Comparing `tmp/nonebot_plugin_game_collection-2.2.6.tar.gz` & `tmp/nonebot_plugin_game_collection-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.2.6.tar", last modified: Fri Jun 23 21:43:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.2.7.tar", last modified: Fri Jun 23 21:49:34 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.2.6.tar` & `nonebot_plugin_game_collection-2.2.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.036644 nonebot_plugin_game_collection-2.2.6/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.6/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-23 21:43:51.036142 nonebot_plugin_game_collection-2.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.975735 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    19558 2023-06-23 21:38:06.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.993822 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    19332 2023-06-23 14:22:48.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    18448 2023-06-23 21:09:29.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.999827 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.025635 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5166 2023-06-23 21:28:38.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.027135 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:51.034141 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    13638 2023-06-23 21:00:43.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:43:50.985815 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1947 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-23 21:43:50.000000 nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 21:43:51.036644 nonebot_plugin_game_collection-2.2.6/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-06-23 21:43:45.000000 nonebot_plugin_game_collection-2.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.338017 nonebot_plugin_game_collection-2.2.7/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.2.7/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-23 21:49:34.336015 nonebot_plugin_game_collection-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.268810 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    19558 2023-06-23 21:38:06.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    60126 2023-06-22 17:20:27.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.287689 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-20 12:33:55.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    13713 2023-06-23 11:42:31.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    19332 2023-06-23 14:22:48.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    18448 2023-06-23 21:09:29.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    29223 2023-06-23 14:03:04.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0     5586 2023-06-20 12:48:06.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.294698 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.323003 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5166 2023-06-23 21:28:38.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.327747 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-20 13:08:13.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.333997 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-06-20 11:54:28.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    13602 2023-06-23 21:48:13.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-23 21:24:50.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:49:34.278019 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1947 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-23 21:49:34.000000 nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 21:49:34.338017 nonebot_plugin_game_collection-2.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-06-23 21:49:23.000000 nonebot_plugin_game_collection-2.2.7/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.2.6/LICENSE` & `nonebot_plugin_game_collection-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/README.md` & `nonebot_plugin_game_collection-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from PIL import Image,ImageDraw,ImageFont
 from PIL.Image import Image as IMG
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 
-from pil_utils import Text2Image
-
 from .avatar import download_avatar,download_groupavatar
 
 from ..data import UserDict, GroupAccount
 from ..data import resourcefile
 
 from ..config import BG_image,fontname
```

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.2.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.2.6/setup.py` & `nonebot_plugin_game_collection-2.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.2.6',
+version='2.2.7',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

