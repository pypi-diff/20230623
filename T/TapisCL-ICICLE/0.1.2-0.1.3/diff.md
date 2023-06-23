# Comparing `tmp/TapisCL-ICICLE-0.1.2.tar.gz` & `tmp/TapisCL-ICICLE-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.1.2.tar", last modified: Fri Jun 23 16:49:08 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.1.3.tar", last modified: Fri Jun 23 17:10:01 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.1.2.tar` & `TapisCL-ICICLE-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.349958 TapisCL-ICICLE-0.1.2/
--rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    44548 2023-06-23 16:49:08.349958 TapisCL-ICICLE-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/README.md
--rw-rw-rw-   0        0        0     1178 2023-06-22 22:06:19.000000 TapisCL-ICICLE-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 16:49:08.350956 TapisCL-ICICLE-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:06.988269 TapisCL-ICICLE-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.043589 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      350 2023-06-22 22:03:39.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.151341 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     8909 2023-06-22 22:01:23.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.745942 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.760946 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     5534 2023-06-22 18:45:31.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.880470 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/systemCommands.py
--rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.026538 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0     7981 2023-06-22 21:47:15.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/serviceCheck.py
--rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.159067 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.283443 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.346957 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44548 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1677 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.863306 TapisCL-ICICLE-0.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    44548 2023-06-23 17:10:01.863306 TapisCL-ICICLE-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1178 2023-06-23 17:08:13.000000 TapisCL-ICICLE-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 17:10:01.864305 TapisCL-ICICLE-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.563549 TapisCL-ICICLE-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.610281 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      350 2023-06-22 22:03:39.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.630338 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     8909 2023-06-23 16:58:38.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.728695 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.746524 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     5788 2023-06-23 17:07:16.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.770526 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/systemCommands.py
+-rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.797181 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0     7981 2023-06-22 21:47:15.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/serviceCheck.py
+-rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.818788 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.846304 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.861305 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44548 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1677 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/__init__.py
```

### Comparing `TapisCL-ICICLE-0.1.2/LICENSE` & `TapisCL-ICICLE-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/PKG-INFO` & `TapisCL-ICICLE-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.1.2/README.md` & `TapisCL-ICICLE-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/pyproject.toml` & `TapisCL-ICICLE-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.1.2"
+version = "0.1.3"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from ..socketopts import socketOpts, schemas
     from ..commands import decorators
     from ..utilities import killableThread
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(f"{__file__}")))
-server_path = os.path.join(__location__, r'..\serverRun.py')
+server_path = os.path.join(__location__, r'../serverRun.py')
     
 
 class ClientSideConnection(socketOpts.ClientSocketOpts, handlers.Handlers):
     def __init__(self, connection, debug=False):
         super().__init__("client", debug=debug)
         self.connection = connection
```

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,17 +97,23 @@
         if self.data_type in ('string', 'int'):
             json['data_type'] = self.data_type
         else:
             json['data_type'] = self.data_type.json()
         return json
     
     def help_message(self):
-        return {"name":self.argument,
-                "syntax":f"{self.truncated_arg}/{self.full_arg} <{self.argument}>",
-                "description":f"{self.description}"}
+        help = {"name":self.argument,
+                    "description":f"{self.description}"}
+        if self.action == 'store':
+            help['syntax'] = f"{self.truncated_arg}/{self.full_arg} <{self.argument}>"
+        elif self.positional:
+            help['syntax'] = f"<{self.argument}>"
+        elif self.action != 'store':
+            help['syntax'] = f"{self.truncated_arg}/{self.full_arg}"
+        return help
     
     def check_for_copy_data(self):
         return {
             'name':self.argument,
             'action':self.action,
         }
```

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandMap.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

