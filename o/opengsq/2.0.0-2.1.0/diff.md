# Comparing `tmp/opengsq-2.0.0.tar.gz` & `tmp/opengsq-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengsq-2.0.0.tar", last modified: Wed May 17 22:37:18 2023, max compression
+gzip compressed data, was "opengsq-2.1.0.tar", last modified: Fri Jun 23 19:44:05 2023, max compression
```

## Comparing `opengsq-2.0.0.tar` & `opengsq-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:18.346179 opengsq-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 22:37:04.000000 opengsq-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-17 22:37:18.346179 opengsq-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-17 22:37:04.000000 opengsq-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:18.342179 opengsq-2.0.0/opengsq/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/binary_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocol_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:18.346179 opengsq-2.0.0/opengsq/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/battlefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/doom3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/gamespy1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/gamespy2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/gamespy3.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/gamespy4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/quake1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/quake2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/quake3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/raknet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/samp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/satisfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/teamspeak3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/vcmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/protocols/won.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/socket_async.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 22:37:04.000000 opengsq-2.0.0/opengsq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:37:18.342179 opengsq-2.0.0/opengsq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-17 22:37:18.000000 opengsq-2.0.0/opengsq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-17 22:37:18.000000 opengsq-2.0.0/opengsq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:37:18.000000 opengsq-2.0.0/opengsq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 22:37:18.000000 opengsq-2.0.0/opengsq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 22:37:18.000000 opengsq-2.0.0/opengsq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 22:37:18.346179 opengsq-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-17 22:37:04.000000 opengsq-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:44:05.454411 opengsq-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 19:43:54.000000 opengsq-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-23 19:44:05.454411 opengsq-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-23 19:43:54.000000 opengsq-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:44:05.454411 opengsq-2.1.0/opengsq/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/binary_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocol_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:44:05.454411 opengsq-2.1.0/opengsq/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/battlefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/doom3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/gamespy1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/gamespy2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/gamespy3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/gamespy4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/quake1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/quake2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/raknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/samp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/satisfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/scum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/teamspeak3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/vcmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/protocols/won.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/socket_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 19:43:54.000000 opengsq-2.1.0/opengsq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:44:05.454411 opengsq-2.1.0/opengsq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-23 19:44:05.000000 opengsq-2.1.0/opengsq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 19:44:05.000000 opengsq-2.1.0/opengsq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:44:05.000000 opengsq-2.1.0/opengsq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 19:44:05.000000 opengsq-2.1.0/opengsq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 19:44:05.000000 opengsq-2.1.0/opengsq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 19:44:05.454411 opengsq-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-23 19:43:54.000000 opengsq-2.1.0/setup.py
```

### Comparing `opengsq-2.0.0/LICENSE` & `opengsq-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/PKG-INFO` & `opengsq-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengsq
-Version: 2.0.0
+Version: 2.1.0
 Summary: 🐍 OpenGSQ - Python library for querying game servers
 Home-page: https://github.com/opengsq/opengsq-python
 Author: OpenGSQ
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opengsq/opengsq-python/issues
 Project-URL: Source Code, https://github.com/opengsq/opengsq-python
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,15 @@
 from opengsq.protocols.minecraft import Minecraft
 from opengsq.protocols.quake1 import Quake1
 from opengsq.protocols.quake2 import Quake2
 from opengsq.protocols.quake3 import Quake3
 from opengsq.protocols.raknet import Raknet
 from opengsq.protocols.samp import Samp
 from opengsq.protocols.satisfactory import Satisfactory
+from opengsq.protocols.scum import Scum
 from opengsq.protocols.source import Source
 from opengsq.protocols.teamspeak3 import Teamspeak3
 from opengsq.protocols.unreal2 import Unreal2
 from opengsq.protocols.vcmp import Vcmp
 from opengsq.protocols.won import WON
 ```
```

### Comparing `opengsq-2.0.0/README.md` & `opengsq-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from opengsq.protocols.minecraft import Minecraft
 from opengsq.protocols.quake1 import Quake1
 from opengsq.protocols.quake2 import Quake2
 from opengsq.protocols.quake3 import Quake3
 from opengsq.protocols.raknet import Raknet
 from opengsq.protocols.samp import Samp
 from opengsq.protocols.satisfactory import Satisfactory
+from opengsq.protocols.scum import Scum
 from opengsq.protocols.source import Source
 from opengsq.protocols.teamspeak3 import Teamspeak3
 from opengsq.protocols.unreal2 import Unreal2
 from opengsq.protocols.vcmp import Vcmp
 from opengsq.protocols.won import WON
 ```
```

### Comparing `opengsq-2.0.0/opengsq/binary_reader.py` & `opengsq-2.1.0/opengsq/binary_reader.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/cli.py` & `opengsq-2.1.0/opengsq/cli.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/__init__.py` & `opengsq-2.1.0/opengsq/protocols/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 from opengsq.protocols.minecraft import Minecraft
 from opengsq.protocols.quake1 import Quake1
 from opengsq.protocols.quake2 import Quake2
 from opengsq.protocols.quake3 import Quake3
 from opengsq.protocols.raknet import Raknet
 from opengsq.protocols.samp import Samp
 from opengsq.protocols.satisfactory import Satisfactory
+from opengsq.protocols.scum import Scum
 from opengsq.protocols.source import Source
 from opengsq.protocols.teamspeak3 import Teamspeak3
 from opengsq.protocols.unreal2 import Unreal2
 from opengsq.protocols.vcmp import Vcmp
 from opengsq.protocols.won import WON
```

### Comparing `opengsq-2.0.0/opengsq/protocols/ase.py` & `opengsq-2.1.0/opengsq/protocols/ase.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/battlefield.py` & `opengsq-2.1.0/opengsq/protocols/battlefield.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/doom3.py` & `opengsq-2.1.0/opengsq/protocols/doom3.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/gamespy1.py` & `opengsq-2.1.0/opengsq/protocols/gamespy1.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/gamespy2.py` & `opengsq-2.1.0/opengsq/protocols/gamespy2.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/gamespy3.py` & `opengsq-2.1.0/opengsq/protocols/gamespy3.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/minecraft.py` & `opengsq-2.1.0/opengsq/protocols/minecraft.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/quake1.py` & `opengsq-2.1.0/opengsq/protocols/quake1.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/quake2.py` & `opengsq-2.1.0/opengsq/protocols/quake2.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/quake3.py` & `opengsq-2.1.0/opengsq/protocols/quake3.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/raknet.py` & `opengsq-2.1.0/opengsq/protocols/raknet.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/samp.py` & `opengsq-2.1.0/opengsq/protocols/samp.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/satisfactory.py` & `opengsq-2.1.0/opengsq/protocols/satisfactory.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/source.py` & `opengsq-2.1.0/opengsq/protocols/source.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/teamspeak3.py` & `opengsq-2.1.0/opengsq/protocols/teamspeak3.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/unreal2.py` & `opengsq-2.1.0/opengsq/protocols/unreal2.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/vcmp.py` & `opengsq-2.1.0/opengsq/protocols/vcmp.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/protocols/won.py` & `opengsq-2.1.0/opengsq/protocols/won.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq/socket_async.py` & `opengsq-2.1.0/opengsq/socket_async.py`

 * *Files identical despite different names*

### Comparing `opengsq-2.0.0/opengsq.egg-info/PKG-INFO` & `opengsq-2.1.0/opengsq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengsq
-Version: 2.0.0
+Version: 2.1.0
 Summary: 🐍 OpenGSQ - Python library for querying game servers
 Home-page: https://github.com/opengsq/opengsq-python
 Author: OpenGSQ
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opengsq/opengsq-python/issues
 Project-URL: Source Code, https://github.com/opengsq/opengsq-python
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,15 @@
 from opengsq.protocols.minecraft import Minecraft
 from opengsq.protocols.quake1 import Quake1
 from opengsq.protocols.quake2 import Quake2
 from opengsq.protocols.quake3 import Quake3
 from opengsq.protocols.raknet import Raknet
 from opengsq.protocols.samp import Samp
 from opengsq.protocols.satisfactory import Satisfactory
+from opengsq.protocols.scum import Scum
 from opengsq.protocols.source import Source
 from opengsq.protocols.teamspeak3 import Teamspeak3
 from opengsq.protocols.unreal2 import Unreal2
 from opengsq.protocols.vcmp import Vcmp
 from opengsq.protocols.won import WON
 ```
```

### Comparing `opengsq-2.0.0/opengsq.egg-info/SOURCES.txt` & `opengsq-2.1.0/opengsq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,13 @@
 opengsq/protocols/minecraft.py
 opengsq/protocols/quake1.py
 opengsq/protocols/quake2.py
 opengsq/protocols/quake3.py
 opengsq/protocols/raknet.py
 opengsq/protocols/samp.py
 opengsq/protocols/satisfactory.py
+opengsq/protocols/scum.py
 opengsq/protocols/source.py
 opengsq/protocols/teamspeak3.py
 opengsq/protocols/unreal2.py
 opengsq/protocols/vcmp.py
 opengsq/protocols/won.py
```

### Comparing `opengsq-2.0.0/setup.py` & `opengsq-2.1.0/setup.py`

 * *Files identical despite different names*

