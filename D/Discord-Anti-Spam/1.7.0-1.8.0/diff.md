# Comparing `tmp/Discord Anti-Spam-1.7.0.tar.gz` & `tmp/Discord Anti-Spam-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Discord Anti-Spam-1.7.0.tar", last modified: Fri Feb 17 23:51:14 2023, max compression
+gzip compressed data, was "Discord Anti-Spam-1.8.0.tar", last modified: Fri Jun 23 14:01:06 2023, max compression
```

## Comparing `Discord Anti-Spam-1.7.0.tar` & `Discord Anti-Spam-1.8.0.tar`

### file list

```diff
@@ -1,74 +1,92 @@
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.667397 Discord Anti-Spam-1.7.0/Discord_Anti_Spam.egg-info/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2939 2023-02-17 23:51:14.000000 Discord Anti-Spam-1.7.0/Discord_Anti_Spam.egg-info/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1727 2023-02-17 23:51:14.000000 Discord Anti-Spam-1.7.0/Discord_Anti_Spam.egg-info/SOURCES.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2023-02-17 23:51:14.000000 Discord Anti-Spam-1.7.0/Discord_Anti_Spam.egg-info/dependency_links.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       23 2023-02-17 23:51:14.000000 Discord Anti-Spam-1.7.0/Discord_Anti_Spam.egg-info/requires.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        9 2023-02-17 23:51:14.000000 Discord Anti-Spam-1.7.0/Discord_Anti_Spam.egg-info/top_level.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1072 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/LICENSE
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       17 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/MANIFEST.in
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2939 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/PKG-INFO
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.667397 Discord Anti-Spam-1.7.0/antispam/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1737 2023-02-17 23:34:12.000000 Discord Anti-Spam-1.7.0/antispam/__init__.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.667397 Discord Anti-Spam-1.7.0/antispam/abc/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       98 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/abc/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     6581 2022-09-01 15:03:04.000000 Discord Anti-Spam-1.7.0/antispam/abc/cache.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    17971 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/abc/lib.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    33798 2023-02-17 23:28:42.000000 Discord Anti-Spam-1.7.0/antispam/anti_spam_handler.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2734 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/base_plugin.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.667397 Discord Anti-Spam-1.7.0/antispam/caches/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1136 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/caches/__init__.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.667397 Discord Anti-Spam-1.7.0/antispam/caches/memory/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1143 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/caches/memory/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5971 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/caches/memory/memory.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.667397 Discord Anti-Spam-1.7.0/antispam/caches/mongo/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       36 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/caches/mongo/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    17353 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/caches/mongo/document.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     7989 2022-09-01 15:08:26.000000 Discord Anti-Spam-1.7.0/antispam/caches/mongo/mongo_cache.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.667397 Discord Anti-Spam-1.7.0/antispam/caches/redis/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1140 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/caches/redis/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     8016 2022-09-20 07:01:09.000000 Discord Anti-Spam-1.7.0/antispam/caches/redis/redis.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    23617 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/core.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/antispam/dataclasses/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1329 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/dataclasses/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3072 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/dataclasses/core.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1961 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/dataclasses/guild.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2018 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/dataclasses/member.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1533 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/dataclasses/message.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    16326 2022-12-19 05:24:38.000000 Discord Anti-Spam-1.7.0/antispam/dataclasses/options.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1357 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/dataclasses/propagate_data.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      363 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/deprecation.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/antispam/enums/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1232 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/enums/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1497 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/enums/ignored_types.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1435 2023-02-17 23:28:34.000000 Discord Anti-Spam-1.7.0/antispam/enums/library.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1403 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/enums/reset_type.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3273 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/exceptions.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5027 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/factory.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/antispam/libs/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1167 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/libs/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    17159 2022-12-19 05:24:38.000000 Discord Anti-Spam-1.7.0/antispam/libs/dpy.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       55 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2046 2022-12-19 05:24:38.000000 Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/base_fork.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5767 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/lib_disnake.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2288 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/lib_enhanced_dpy.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2072 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/lib_nextcord.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    17159 2022-12-19 05:24:38.000000 Discord Anti-Spam-1.7.0/antispam/libs/lib_hikari.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/antispam/libs/shared/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      309 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/libs/shared/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    14909 2022-12-19 05:24:38.000000 Discord Anti-Spam-1.7.0/antispam/libs/shared/base.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      780 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/libs/shared/substitute_args.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5000 2023-02-17 23:31:46.000000 Discord Anti-Spam-1.7.0/antispam/libs/shared/timed_cache.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5638 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/plugin_cache.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/antispam/plugins/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1396 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/plugins/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     7582 2022-12-19 05:24:38.000000 Discord Anti-Spam-1.7.0/antispam/plugins/admin_logs.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     8433 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/plugins/anti_mass_mention.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)    14317 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/plugins/anti_spam_tracker.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3336 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/plugins/max_message_limiter.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     3961 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/plugins/stats.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1246 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/antispam/util.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2125 2022-06-29 03:17:30.000000 Discord Anti-Spam-1.7.0/readme.md
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2023-02-17 23:51:14.671397 Discord Anti-Spam-1.7.0/setup.cfg
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1826 2022-06-29 03:17:58.000000 Discord Anti-Spam-1.7.0/setup.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.858370 Discord Anti-Spam-1.8.0/
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.838370 Discord Anti-Spam-1.8.0/Discord_Anti_Spam.egg-info/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2883 2023-06-23 14:01:06.000000 Discord Anti-Spam-1.8.0/Discord_Anti_Spam.egg-info/PKG-INFO
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2174 2023-06-23 14:01:06.000000 Discord Anti-Spam-1.8.0/Discord_Anti_Spam.egg-info/SOURCES.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)        1 2023-06-23 14:01:06.000000 Discord Anti-Spam-1.8.0/Discord_Anti_Spam.egg-info/dependency_links.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       23 2023-06-23 14:01:06.000000 Discord Anti-Spam-1.8.0/Discord_Anti_Spam.egg-info/requires.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)        9 2023-06-23 14:01:06.000000 Discord Anti-Spam-1.8.0/Discord_Anti_Spam.egg-info/top_level.txt
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1072 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/LICENSE
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       17 2021-09-20 02:17:18.000000 Discord Anti-Spam-1.8.0/MANIFEST.in
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2883 2023-06-23 14:01:06.858370 Discord Anti-Spam-1.8.0/PKG-INFO
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.842370 Discord Anti-Spam-1.8.0/antispam/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1737 2023-06-23 13:59:13.000000 Discord Anti-Spam-1.8.0/antispam/__init__.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.842370 Discord Anti-Spam-1.8.0/antispam/abc/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       98 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/abc/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     6581 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/abc/cache.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    17971 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/abc/lib.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    33798 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/anti_spam_handler.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2734 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/base_plugin.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.842370 Discord Anti-Spam-1.8.0/antispam/caches/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1136 2022-06-14 13:38:59.000000 Discord Anti-Spam-1.8.0/antispam/caches/__init__.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.842370 Discord Anti-Spam-1.8.0/antispam/caches/memory/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1143 2021-11-08 05:05:35.000000 Discord Anti-Spam-1.8.0/antispam/caches/memory/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     5971 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/caches/memory/memory.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.846370 Discord Anti-Spam-1.8.0/antispam/caches/mongo/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       36 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/caches/mongo/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    17353 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/caches/mongo/document.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     7989 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/caches/mongo/mongo_cache.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.846370 Discord Anti-Spam-1.8.0/antispam/caches/redis/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1140 2021-11-08 05:05:35.000000 Discord Anti-Spam-1.8.0/antispam/caches/redis/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     8016 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/caches/redis/redis.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    23617 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/core.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.846370 Discord Anti-Spam-1.8.0/antispam/dataclasses/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1329 2022-06-14 13:58:16.000000 Discord Anti-Spam-1.8.0/antispam/dataclasses/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     3072 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/dataclasses/core.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1961 2022-06-14 13:58:16.000000 Discord Anti-Spam-1.8.0/antispam/dataclasses/guild.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2018 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/dataclasses/member.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1533 2021-11-08 05:05:35.000000 Discord Anti-Spam-1.8.0/antispam/dataclasses/message.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    16326 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/dataclasses/options.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1357 2021-11-08 05:05:35.000000 Discord Anti-Spam-1.8.0/antispam/dataclasses/propagate_data.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      363 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/deprecation.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.846370 Discord Anti-Spam-1.8.0/antispam/enums/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1232 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/enums/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1497 2021-11-08 05:05:35.000000 Discord Anti-Spam-1.8.0/antispam/enums/ignored_types.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1435 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/enums/library.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1403 2021-11-08 05:05:35.000000 Discord Anti-Spam-1.8.0/antispam/enums/reset_type.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     3273 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/exceptions.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     5027 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/factory.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.850370 Discord Anti-Spam-1.8.0/antispam/libs/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1167 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/libs/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    17324 2023-06-23 13:52:13.000000 Discord Anti-Spam-1.8.0/antispam/libs/dpy.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.850370 Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       55 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2046 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/base_fork.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     5767 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/lib_disnake.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2288 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/lib_enhanced_dpy.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2072 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/lib_nextcord.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    17159 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/libs/lib_hikari.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.850370 Discord Anti-Spam-1.8.0/antispam/libs/shared/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      309 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/libs/shared/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    14909 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/libs/shared/base.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      780 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/libs/shared/substitute_args.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     5000 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/libs/shared/timed_cache.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     5638 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/plugin_cache.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.854370 Discord Anti-Spam-1.8.0/antispam/plugins/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1396 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/plugins/__init__.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     7582 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/antispam/plugins/admin_logs.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     8433 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/plugins/anti_mass_mention.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    14317 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/plugins/anti_spam_tracker.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     3336 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/plugins/max_message_limiter.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     3961 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/antispam/plugins/stats.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1246 2021-11-08 05:05:35.000000 Discord Anti-Spam-1.8.0/antispam/util.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2125 2022-06-14 13:38:59.000000 Discord Anti-Spam-1.8.0/readme.md
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)       38 2023-06-23 14:01:06.858370 Discord Anti-Spam-1.8.0/setup.cfg
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1826 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/setup.py
+drwxr-xr-x   0 skelmis   (1000) skelmis   (1000)        0 2023-06-23 14:01:06.858370 Discord Anti-Spam-1.8.0/tests/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     1486 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_admin_logs.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     4525 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_anti_mass_mention.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    37084 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/tests/test_anti_spam_handler.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    10206 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_anti_spam_tracker.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)    15532 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_core.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2619 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_exceptions.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      400 2021-09-20 02:17:18.000000 Discord Anti-Spam-1.8.0/tests/test_extras.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     5705 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_factory.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     9670 2023-06-23 13:59:01.000000 Discord Anti-Spam-1.8.0/tests/test_lib_dpy.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     6235 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_memory_cache.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     7671 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/tests/test_mongo_cache.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     3777 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_plugin_cache.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     8250 2023-06-23 13:23:28.000000 Discord Anti-Spam-1.8.0/tests/test_redis_cache.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)      614 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_shared_base.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     3631 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_stats.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2245 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_timed_cache.py
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     8865 2022-04-07 05:16:04.000000 Discord Anti-Spam-1.8.0/tests/test_tracker_example_subclass.py
```

### Comparing `Discord Anti-Spam-1.7.0/Discord_Anti_Spam.egg-info/PKG-INFO` & `Discord Anti-Spam-1.8.0/Discord_Anti_Spam.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: Discord-Anti-Spam
-Version: 1.7.0
+Version: 1.8.0
 Summary: An easy to use package for anti-spam features in python discord libraries.
-Home-page: UNKNOWN
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
-License: UNKNOWN
 Project-URL: Support server, https://discord.gg/BqPNSH2jPg
 Project-URL: Issue tracker, https://github.com/Skelmis/DPY-Anti-Spam/issues
 Project-URL: Documentation, https://dpy-anti-spam.readthedocs.io/en/latest
 Project-URL: Homepage, https://github.com/Skelmis/DPY-Anti-Spam
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -79,9 +76,7 @@
 
 Want realtime help? Join the discord [here](https://discord.gg/BqPNSH2jPg).
 
 ---
 
 ### License
 This project is licensed under the MIT license
-
-
```

### Comparing `Discord Anti-Spam-1.7.0/LICENSE` & `Discord Anti-Spam-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/PKG-INFO` & `Discord Anti-Spam-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: Discord Anti-Spam
-Version: 1.7.0
+Version: 1.8.0
 Summary: An easy to use package for anti-spam features in python discord libraries.
-Home-page: UNKNOWN
 Author: Skelmis
 Author-email: ethan@koldfusion.xyz
-License: UNKNOWN
 Project-URL: Support server, https://discord.gg/BqPNSH2jPg
 Project-URL: Issue tracker, https://github.com/Skelmis/DPY-Anti-Spam/issues
 Project-URL: Documentation, https://dpy-anti-spam.readthedocs.io/en/latest
 Project-URL: Homepage, https://github.com/Skelmis/DPY-Anti-Spam
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -79,9 +76,7 @@
 
 Want realtime help? Join the discord [here](https://discord.gg/BqPNSH2jPg).
 
 ---
 
 ### License
 This project is licensed under the MIT license
-
-
```

### Comparing `Discord Anti-Spam-1.7.0/antispam/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 import logging
 import sys
 from collections import namedtuple
 
 from antispam.exceptions import *
 from antispam.anti_spam_handler import AntiSpamHandler
 from antispam.base_plugin import BasePlugin
 from antispam.dataclasses import CorePayload, Options
 from antispam.plugin_cache import PluginCache
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 VersionInfo = namedtuple("VersionInfo", "major minor micro releaselevel serial")
-version_info = VersionInfo(major=1, minor=7, micro=0, releaselevel="final", serial=0)
+version_info = VersionInfo(major=1, minor=8, micro=0, releaselevel="final", serial=0)
 
 
 if sys.version_info[1] < 8:
     raise RuntimeError("This package requires python 3.8 or higher.")
```

### Comparing `Discord Anti-Spam-1.7.0/antispam/abc/cache.py` & `Discord Anti-Spam-1.8.0/antispam/abc/cache.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/abc/lib.py` & `Discord Anti-Spam-1.8.0/antispam/abc/lib.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/anti_spam_handler.py` & `Discord Anti-Spam-1.8.0/antispam/anti_spam_handler.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/base_plugin.py` & `Discord Anti-Spam-1.8.0/antispam/base_plugin.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/caches/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/caches/memory/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/caches/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/caches/memory/memory.py` & `Discord Anti-Spam-1.8.0/antispam/caches/memory/memory.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/caches/mongo/document.py` & `Discord Anti-Spam-1.8.0/antispam/caches/mongo/document.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/caches/mongo/mongo_cache.py` & `Discord Anti-Spam-1.8.0/antispam/caches/mongo/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/caches/redis/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/caches/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/caches/redis/redis.py` & `Discord Anti-Spam-1.8.0/antispam/caches/redis/redis.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/core.py` & `Discord Anti-Spam-1.8.0/antispam/core.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/dataclasses/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/dataclasses/core.py` & `Discord Anti-Spam-1.8.0/antispam/dataclasses/core.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/dataclasses/guild.py` & `Discord Anti-Spam-1.8.0/antispam/dataclasses/guild.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/dataclasses/member.py` & `Discord Anti-Spam-1.8.0/antispam/dataclasses/member.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/dataclasses/message.py` & `Discord Anti-Spam-1.8.0/antispam/dataclasses/message.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/dataclasses/options.py` & `Discord Anti-Spam-1.8.0/antispam/dataclasses/options.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/dataclasses/propagate_data.py` & `Discord Anti-Spam-1.8.0/antispam/dataclasses/propagate_data.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/enums/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/enums/ignored_types.py` & `Discord Anti-Spam-1.8.0/antispam/enums/ignored_types.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/enums/library.py` & `Discord Anti-Spam-1.8.0/antispam/enums/library.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/enums/reset_type.py` & `Discord Anti-Spam-1.8.0/antispam/enums/reset_type.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/exceptions.py` & `Discord Anti-Spam-1.8.0/antispam/exceptions.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/factory.py` & `Discord Anti-Spam-1.8.0/antispam/factory.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/dpy.py` & `Discord Anti-Spam-1.8.0/antispam/libs/dpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -456,20 +456,24 @@
                 message,
                 delete_after=delete_after_time,
             )
 
     async def timeout_member(
         self, member, original_message, until: datetime.timedelta
     ) -> None:
-        raise UnsupportedAction(
-            "Timeouts are not supported for discord.py, if you "
-            "are using a fork please specify it explicitly."
+        guild = original_message.guild
+        perms = guild.me.guild_permissions
+        if not perms.moderate_members:
+            raise MissingGuildPermissions(
+                "moderate_members is required to timeout members.\n"
+                f"Tried timing out Member(id={member.id}) in Guild(id={member.guild.id})"
+            )
+
+        await member.timeout(
+            until=until, reason="Automated timeout from Discord-Anti-Spam"
         )
 
     async def is_member_currently_timed_out(self, member) -> bool:
-        raise UnsupportedAction(
-            "Timeouts are not supported for discord.py, if you "
-            "are using a fork please specify it explicitly."
-        )
+        return member.timed_out_until is not None
 
     def is_dm(self, message) -> bool:
         return not bool(message.guild)
```

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/base_fork.py` & `Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/base_fork.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/lib_disnake.py` & `Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/lib_disnake.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/lib_enhanced_dpy.py` & `Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/lib_enhanced_dpy.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/dpy_forks/lib_nextcord.py` & `Discord Anti-Spam-1.8.0/antispam/libs/dpy_forks/lib_nextcord.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/lib_hikari.py` & `Discord Anti-Spam-1.8.0/antispam/libs/lib_hikari.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/shared/base.py` & `Discord Anti-Spam-1.8.0/antispam/libs/shared/base.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/shared/substitute_args.py` & `Discord Anti-Spam-1.8.0/antispam/libs/shared/substitute_args.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/libs/shared/timed_cache.py` & `Discord Anti-Spam-1.8.0/antispam/libs/shared/timed_cache.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/plugin_cache.py` & `Discord Anti-Spam-1.8.0/antispam/plugin_cache.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/plugins/__init__.py` & `Discord Anti-Spam-1.8.0/antispam/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/plugins/admin_logs.py` & `Discord Anti-Spam-1.8.0/antispam/plugins/admin_logs.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/plugins/anti_mass_mention.py` & `Discord Anti-Spam-1.8.0/antispam/plugins/anti_mass_mention.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/plugins/anti_spam_tracker.py` & `Discord Anti-Spam-1.8.0/antispam/plugins/anti_spam_tracker.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/plugins/max_message_limiter.py` & `Discord Anti-Spam-1.8.0/antispam/plugins/max_message_limiter.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/plugins/stats.py` & `Discord Anti-Spam-1.8.0/antispam/plugins/stats.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/antispam/util.py` & `Discord Anti-Spam-1.8.0/antispam/util.py`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/readme.md` & `Discord Anti-Spam-1.8.0/readme.md`

 * *Files identical despite different names*

### Comparing `Discord Anti-Spam-1.7.0/setup.py` & `Discord Anti-Spam-1.8.0/setup.py`

 * *Files identical despite different names*

