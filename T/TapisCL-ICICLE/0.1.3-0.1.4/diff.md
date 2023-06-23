# Comparing `tmp/TapisCL-ICICLE-0.1.3.tar.gz` & `tmp/TapisCL-ICICLE-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.1.3.tar", last modified: Fri Jun 23 17:10:01 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.1.4.tar", last modified: Fri Jun 23 18:50:46 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.1.3.tar` & `TapisCL-ICICLE-0.1.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.863306 TapisCL-ICICLE-0.1.3/
--rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    44548 2023-06-23 17:10:01.863306 TapisCL-ICICLE-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/README.md
--rw-rw-rw-   0        0        0     1178 2023-06-23 17:08:13.000000 TapisCL-ICICLE-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 17:10:01.864305 TapisCL-ICICLE-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.563549 TapisCL-ICICLE-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.610281 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      350 2023-06-22 22:03:39.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.630338 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     8909 2023-06-23 16:58:38.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.728695 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.746524 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     5788 2023-06-23 17:07:16.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.770526 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/systemCommands.py
--rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.797181 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0     7981 2023-06-22 21:47:15.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/serviceCheck.py
--rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.818788 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.846304 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:10:01.861305 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44548 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1677 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-23 17:10:01.000000 TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.176371 TapisCL-ICICLE-0.1.4/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    44548 2023-06-23 18:50:46.176371 TapisCL-ICICLE-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/README.md
+-rw-rw-rw-   0        0        0     1178 2023-06-23 18:49:57.000000 TapisCL-ICICLE-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 18:50:46.176371 TapisCL-ICICLE-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:45.907452 TapisCL-ICICLE-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:45.994994 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      417 2023-06-23 17:45:33.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.013548 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     8996 2023-06-23 18:46:38.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.083949 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.094318 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     5788 2023-06-23 17:07:16.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.108935 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/systemCommands.py
+-rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.128298 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0     7982 2023-06-23 17:46:27.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/serviceCheck.py
+-rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.141727 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.160917 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:50:46.174222 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44548 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1677 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-23 18:50:45.000000 TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.4/src/__init__.py
```

### Comparing `TapisCL-ICICLE-0.1.3/LICENSE` & `TapisCL-ICICLE-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/PKG-INFO` & `TapisCL-ICICLE-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.3
+Version: 0.1.4
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.1.3/README.md` & `TapisCL-ICICLE-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/pyproject.toml` & `TapisCL-ICICLE-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.1.3"
+version = "0.1.4"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 import socket
 import argparse
 import sys
 import os
 import time
 import traceback
+import subprocess
 
 import pyfiglet
 from blessed import Terminal
 
 if __name__ != "__main__":
     from . import handlers
     from ..socketopts import socketOpts, schemas
@@ -79,15 +80,15 @@
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
         """
         if 'win' in sys.platform:
             os.system(rf"pythonw {server_path}")
         else: # unix based
-            os.system(f"python {server_path} &")
+            subprocess.Popen(['nohup', 'python3', server_path, '&'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
     #@decorators.AnimatedLoading
     def connection_initialization(self):
         """
         start the local server through the client
         """
         startup_flag = False
```

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandMap.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup, auth.ServerSideAuth):
     """
     Receives commands from the client and executes Tapis operations
     """
     SESSION_TIME = 1200
-    debug=True
+    debug=False
     def __init__(self, IP: str, PORT: int):
         super().__init__()
         self.initial = True
 
         self.t = None
         self.url = None
         self.access_token = None
```

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.1.4/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.1.3
+Version: 0.1.4
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.1.3/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.1.4/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

