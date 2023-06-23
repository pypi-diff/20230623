# Comparing `tmp/TapisCL-ICICLE-0.1.1.tar.gz` & `tmp/TapisCL-ICICLE-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.1.1.tar", last modified: Thu Jun 22 21:29:34 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.1.2.tar", last modified: Fri Jun 23 16:49:08 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.1.1.tar` & `TapisCL-ICICLE-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.914935 TapisCL-ICICLE-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    44548 2023-06-22 21:29:34.913936 TapisCL-ICICLE-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/README.md
--rw-rw-rw-   0        0        0     1178 2023-06-22 21:28:28.000000 TapisCL-ICICLE-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 21:29:34.914935 TapisCL-ICICLE-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.719040 TapisCL-ICICLE-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.730597 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      350 2023-06-22 21:22:04.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.742639 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     8949 2023-06-22 21:21:28.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.797239 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.805247 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     5534 2023-06-22 18:45:31.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.818740 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/systemCommands.py
--rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.846442 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0     7904 2023-06-22 19:13:30.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/server/serviceCheck.py
--rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.861735 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.893727 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-22 21:29:34.911939 TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44548 2023-06-22 21:29:34.000000 TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1677 2023-06-22 21:29:34.000000 TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 21:29:34.000000 TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-22 21:29:34.000000 TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-06-22 21:29:34.000000 TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-22 21:29:34.000000 TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.349958 TapisCL-ICICLE-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    44548 2023-06-23 16:49:08.349958 TapisCL-ICICLE-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1178 2023-06-22 22:06:19.000000 TapisCL-ICICLE-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 16:49:08.350956 TapisCL-ICICLE-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:06.988269 TapisCL-ICICLE-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.043589 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      350 2023-06-22 22:03:39.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.151341 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     8909 2023-06-22 22:01:23.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.745942 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.760946 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     5534 2023-06-22 18:45:31.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:07.880470 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/systemCommands.py
+-rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.026538 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0     7981 2023-06-22 21:47:15.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/serviceCheck.py
+-rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.159067 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.283443 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:49:08.346957 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44548 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1677 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-23 16:49:06.000000 TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.2/src/__init__.py
```

### Comparing `TapisCL-ICICLE-0.1.1/LICENSE` & `TapisCL-ICICLE-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/PKG-INFO` & `TapisCL-ICICLE-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.1.1/README.md` & `TapisCL-ICICLE-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/pyproject.toml` & `TapisCL-ICICLE-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.1.1"
+version = "0.1.2"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.connection = connection
     
     def close(self):
         self.connection.close()
 
 
 class CLI(handlers.Handlers):
-    debug=True
+    debug=False
     """
     Receive user input, either direct from bash environment or from the custom interface, then parse these commands and send them to the server to be executed. 
     """
     def __init__(self, IP: str, PORT: int):
         super().__init__()
 
         self.term = Terminal()
@@ -68,15 +68,14 @@
     def configure_parser(self, arguments):
         parser = argparse.ArgumentParser(description="Command Line Argument Parser", exit_on_error=False, usage=argparse.SUPPRESS, add_help=False, conflict_handler='resolve')
         parser.add_argument('command_selection')
         parser.add_argument('positionals', nargs='*', default='default1')
         parser.error = self.parser_error
 
         for arg_name, arg in arguments.items():
-            print(arg['truncated_arg'])
             parser.add_argument(f"-{arg['truncated_arg']}", arg['full_arg'],
                                 action=arg['action'])
         return parser
 
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
```

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandMap.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,31 @@
 
     async def close(self):
         self.writer.close()
         await self.writer.wait_closed()
         
 
 class TaskCallback:
-    def __init__(self, logger, task: asyncio.Task):
+    def __init__(self, logger, task: asyncio.Task, task_list: list):
+        self.task_list = task_list
         self.logger, self.task = logger, task
-        print("DOING THE INIT")
 
     def __call__(self, result):
+        self.task_list.remove(self.task)
         print(result)
         result = self.task.result()
         self.logger.info(result)
 
 
 class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup, auth.ServerSideAuth):
     """
     Receives commands from the client and executes Tapis operations
     """
     SESSION_TIME = 1200
-    debug=False
+    debug=True
     def __init__(self, IP: str, PORT: int):
         super().__init__()
         self.initial = True
 
         self.t = None
         self.url = None
         self.access_token = None
@@ -124,15 +125,15 @@
         setup_response: schemas.ResponseData = await connection.receive()
         if not setup_response.request_content['setup_success']:
             self.logger.warning(f"The setup of the connection {connection.name} failed")
             return
 
         loop = asyncio.get_event_loop()
         task: asyncio.Task = loop.create_task(self.receive_and_execute(connection))
-        callback = TaskCallback(self.logger, task)
+        callback = TaskCallback(self.logger, task, self.task_list)
         task.add_done_callback(callback)
         self.task_list.append(task)
 
     def timeout_handler(self):  
         """
         checks if the timeout has been exceeded
         """
```

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.1.2/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.1.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.1.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

