# Comparing `tmp/boli_orbital_api-0.9b15.tar.gz` & `tmp/boli_orbital_api-0.9b17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boli_orbital_api-0.9b15.tar", max compression
+gzip compressed data, was "boli_orbital_api-0.9b17.tar", max compression
```

## Comparing `boli_orbital_api-0.9b15.tar` & `boli_orbital_api-0.9b17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6425 2023-06-07 13:34:10.219390 boli_orbital_api-0.9b15/.gitignore
--rw-r--r--   0        0        0      649 2023-06-15 18:04:16.375821 boli_orbital_api-0.9b15/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-05 20:23:02.778565 boli_orbital_api-0.9b15/LICENSE
--rw-r--r--   0        0        0     2772 2023-06-03 22:55:11.905218 boli_orbital_api-0.9b15/README.md
--rw-r--r--   0        0        0     2922 2023-06-03 22:55:11.858554 boli_orbital_api-0.9b15/README_ES.md
--rw-r--r--   0        0        0     1305 2023-06-05 20:18:34.246061 boli_orbital_api-0.9b15/TODO.md
--rw-r--r--   0        0        0       42 2023-06-07 13:32:45.641287 boli_orbital_api-0.9b15/boli_orbital_api/__init__.py
--rw-r--r--   0        0        0     2724 2023-06-09 18:45:51.900962 boli_orbital_api-0.9b15/boli_orbital_api/logger.py
--rw-r--r--   0        0        0    62629 2023-06-15 17:47:08.136008 boli_orbital_api-0.9b15/boli_orbital_api/rpc.py
--rw-r--r--   0        0        0       14 2023-06-02 00:43:19.185603 boli_orbital_api-0.9b15/docs/using.md
--rw-r--r--   0        0        0     1255 2023-06-15 16:37:07.716044 boli_orbital_api-0.9b15/pyproject.toml
--rw-r--r--   0        0        0       16 2023-06-01 22:31:09.954549 boli_orbital_api-0.9b15/requirements.txt
--rw-r--r--   0        0        0      100 2023-06-09 18:43:19.823212 boli_orbital_api-0.9b15/requirements_freezed.txt
--rw-r--r--   0        0        0        0 2023-05-31 19:36:48.526207 boli_orbital_api-0.9b15/tests/__init__.py
--rw-r--r--   0        0        0      409 2023-06-05 19:41:08.195877 boli_orbital_api-0.9b15/tests/test.py
--rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 boli_orbital_api-0.9b15/PKG-INFO
+-rw-r--r--   0        0        0     6425 2023-06-07 13:34:10.219390 boli_orbital_api-0.9b17/.gitignore
+-rw-r--r--   0        0        0      649 2023-06-15 18:04:16.375821 boli_orbital_api-0.9b17/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-05 20:23:02.778565 boli_orbital_api-0.9b17/LICENSE
+-rw-r--r--   0        0        0     2772 2023-06-03 22:55:11.905218 boli_orbital_api-0.9b17/README.md
+-rw-r--r--   0        0        0     2922 2023-06-03 22:55:11.858554 boli_orbital_api-0.9b17/README_ES.md
+-rw-r--r--   0        0        0     1305 2023-06-05 20:18:34.246061 boli_orbital_api-0.9b17/TODO.md
+-rw-r--r--   0        0        0      186 2023-06-15 19:02:07.386266 boli_orbital_api-0.9b17/boli_orbital_api/__init__.py
+-rw-r--r--   0        0        0     2724 2023-06-09 18:45:51.900962 boli_orbital_api-0.9b17/boli_orbital_api/logger.py
+-rw-r--r--   0        0        0    66108 2023-06-23 16:30:22.540438 boli_orbital_api-0.9b17/boli_orbital_api/rpc.py
+-rw-r--r--   0        0        0       14 2023-06-02 00:43:19.185603 boli_orbital_api-0.9b17/docs/using.md
+-rw-r--r--   0        0        0     1255 2023-06-15 18:51:26.454304 boli_orbital_api-0.9b17/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-01 22:31:09.954549 boli_orbital_api-0.9b17/requirements.txt
+-rw-r--r--   0        0        0      100 2023-06-09 18:43:19.823212 boli_orbital_api-0.9b17/requirements_freezed.txt
+-rw-r--r--   0        0        0        0 2023-05-31 19:36:48.526207 boli_orbital_api-0.9b17/tests/__init__.py
+-rw-r--r--   0        0        0      409 2023-06-05 19:41:08.195877 boli_orbital_api-0.9b17/tests/test.py
+-rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 boli_orbital_api-0.9b17/PKG-INFO
```

### Comparing `boli_orbital_api-0.9b15/.gitignore` & `boli_orbital_api-0.9b17/.gitignore`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b15/CHANGELOG.md` & `boli_orbital_api-0.9b17/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b15/LICENSE` & `boli_orbital_api-0.9b17/LICENSE`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b15/README.md` & `boli_orbital_api-0.9b17/README.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b15/README_ES.md` & `boli_orbital_api-0.9b17/README_ES.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b15/TODO.md` & `boli_orbital_api-0.9b17/TODO.md`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b15/boli_orbital_api/logger.py` & `boli_orbital_api-0.9b17/boli_orbital_api/logger.py`

 * *Files identical despite different names*

### Comparing `boli_orbital_api-0.9b15/boli_orbital_api/rpc.py` & `boli_orbital_api-0.9b17/boli_orbital_api/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         BOLICOIN COMPATIBLE VERSION: v2.0.0.2-g
         Bolicoin/Bolivarcoin platform and cryptocurrency from http://bolis.info
 
     __author__: "Asdrúbal Velásquez Lagrave - Twitter/Telegram: @Visionario"
     __copyright__: "2018-2023"
     __credits__: [""]
     __license__: "MIT"
-    __version__: 0.9b15
+    __version__: 0.9b17
     __maintainer__: "Asdrúbal Velásquez Lagrave"
     __email__: "hello@orbital.center"
     __status__: "BETA"
     __app_name__: "Node API Rpc main class for Bolivarcoin/Bolicoin blockchain (Layer 1)",
     __url__: "https://orbital.center"
 
 """
@@ -25,19 +25,20 @@
 
 __all__ = [
     "Node",
     "GobjectListSignals",
     "GobjectListTypes",
     "MasternodeCountOptions",
     "MasternodeStartModes",
+    "MnListModes",
     "About",
     "VERSION",
 ]
 
-VERSION = "0.9b15"
+VERSION = "0.9b17"
 
 # LOGGER
 logger = setup_logger(__name__)
 
 
 class GobjectListSignals:
     """See gobject_list()"""
@@ -68,14 +69,30 @@
 class MasternodeStartModes:
     """See masternode_start_mode()"""
     ALL = 'all'
     MISSING = 'missing'
     DISABLED = 'disabled'
 
 
+class MnListModes:
+    """See masternodelist()"""
+    ACTIVESECONDS = 'activeseconds'
+    ADDR = 'addr'
+    FULL = 'full'
+    INFO = 'info'
+    LASTPAIDBLOCK = 'lastpaidblock'
+    LASTPAIDTIME = 'lastpaidtime'
+    LASTSEEN = 'lastseen'
+    PAYEE = 'payee'
+    PROTOCOL = 'protocol'
+    PUBKEY = 'pubkey'
+    RANK = 'rank'
+    STATUS = 'status'
+
+
 def _process_result(result):
     """Process results coming from RAW calls"""
     try:
         if result.get('result') is not None:  # OK
             return {"result": result.get('result'), 'errors': False}
         else:  # Error!!!
             return {"result": None, "errors": result.get('errors', True)}
@@ -776,14 +793,63 @@
         if mode in MASTERNODE_START_MODES:
             params = [f'start-{mode}']
         else:
             return {'result': f'Available modes are: {MASTERNODE_START_MODES}', 'errors': True}
 
         return _process_result(self.raw_call("masternode", params=params))
 
+    def masternodelist(self, mode: MnListModes = MnListModes.STATUS, mn_filter: str = ''):
+        """
+            masternodelist ( "mode" "filter" )
+            Get a list of masternodes in different modes
+
+            Arguments:
+            1. "mode"      (string, optional/required to use filter, defaults = status) The mode to run list in
+            2. "filter"    (string, optional) Filter results. Partial match by outpoint by default in all modes,
+                                                additional matches in some modes are also available
+
+            Available modes:
+              activeseconds  - Print number of seconds masternode recognized by the network as enabled
+                               (since latest issued "masternode start/start-many/start-alias")
+              addr           - Print ip address associated with a masternode (can be additionally filtered, partial match)
+              full           - Print info in format 'status protocol payee lastseen activeseconds lastpaidtime lastpaidblock IP'
+                               (can be additionally filtered, partial match)
+              info           - Print info in format 'status protocol payee lastseen activeseconds sentinelversion sentinelstate IP'
+                               (can be additionally filtered, partial match)
+              lastpaidblock  - Print the last block height a node was paid on the network
+              lastpaidtime   - Print the last time a node was paid on the network
+              lastseen       - Print timestamp of when a masternode was last seen on the network
+              payee          - Print Bolivarcoin address associated with a masternode (can be additionally filtered,
+                               partial match)
+              protocol       - Print protocol of a masternode (can be additionally filtered, exact match)
+              pubkey         - Print the masternode (not collateral) public key
+              rank           - Print rank of a masternode based on current block
+              status         - Print masternode status: PRE_ENABLED / ENABLED / EXPIRED / WATCHDOG_EXPIRED / NEW_START_REQUIRED /
+                               UPDATE_REQUIRED / POSE_BAN / OUTPOINT_SPENT (can be additionally filtered, partial match)
+
+                EXAMPLE
+                {
+                "ad06255e05cc22b5abb74187e2008fd022bd192b1bac065bc87ae3070a9761fb-0": "NEW_START_REQUIRED 70212 bJG26MWSpxiYLada8orPxz8mwpUYubvJFh 1676268599  1065786 1.1.0 current 167.86.105.73:49053",
+                }
+
+        """
+        return _process_result(self.raw_call("masternodelist", params=[mode, mn_filter]))
+
+    def mnsync_status(self):
+        """Returns the sync status (mnsync status)"""
+        return _process_result(self.raw_call("mnsync", params=['status']))
+
+    def mnsync_next(self):
+        """Returns the sync status to the next step (mnsync next)"""
+        return _process_result(self.raw_call("mnsync", params=['next']))
+
+    def mnsync_reset(self):
+        """Reset mnsync (mnsync reset)"""
+        return _process_result(self.raw_call("mnsync", params=['reset']))
+
 
 # ╻ ╻┏━╸╻  ┏━┓
 # ┣━┫┣╸ ┃  ┣━┛
 # ╹ ╹┗━╸┗━╸╹
 class _Help:
     """ Help class for get help directly from node
```

### Comparing `boli_orbital_api-0.9b15/pyproject.toml` & `boli_orbital_api-0.9b17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boli_orbital_api"
-version = "0.9b15"
+version = "0.9b17"
 description = "Orbital API RPC for Bolivarcoin/Bolicoin blockchain"
 authors = ["Asdrubal Velasquez Lagrave <hello@orbital.center>"]
 maintainers = ["Asdrubal Velasquez Lagrave <hello@orbital.center>"]
 repository = "https://github.com/Visionario/BoliOrbitalAPI"
 homepage = "https://orbital.center"
 keywords = ["bolicoin", "bolivarcoin", "criptocurrency", "blockchain", "api"]
 classifiers = [
```

### Comparing `boli_orbital_api-0.9b15/PKG-INFO` & `boli_orbital_api-0.9b17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boli-orbital-api
-Version: 0.9b15
+Version: 0.9b17
 Summary: Orbital API RPC for Bolivarcoin/Bolicoin blockchain
 Home-page: https://orbital.center
 License: MIT
 Keywords: bolicoin,bolivarcoin,criptocurrency,blockchain,api
 Author: Asdrubal Velasquez Lagrave
 Author-email: hello@orbital.center
 Maintainer: Asdrubal Velasquez Lagrave
```

