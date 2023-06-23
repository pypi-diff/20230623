# Comparing `tmp/ipyeos-0.4.3.tar.gz` & `tmp/ipyeos-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyeos-0.4.3.tar", last modified: Fri Jun 16 06:18:31 2023, max compression
+gzip compressed data, was "ipyeos-0.4.4.tar", last modified: Fri Jun 23 06:21:52 2023, max compression
```

## Comparing `ipyeos-0.4.3.tar` & `ipyeos-0.4.4.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:18:31.781241 ipyeos-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-16 06:18:24.000000 ipyeos-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-16 06:18:24.000000 ipyeos-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-06-16 06:18:31.785241 ipyeos-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3911 2023-06-16 06:18:24.000000 ipyeos-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:18:31.781241 ipyeos-0.4.3/ipyeos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-06-16 06:18:31.000000 ipyeos-0.4.3/ipyeos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-16 06:18:31.000000 ipyeos-0.4.3/ipyeos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 06:18:31.000000 ipyeos-0.4.3/ipyeos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-16 06:18:31.000000 ipyeos-0.4.3/ipyeos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-16 06:18:31.000000 ipyeos-0.4.3/ipyeos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-16 06:18:31.000000 ipyeos-0.4.3/ipyeos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:18:31.781241 ipyeos-0.4.3/pysrc/
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/args.py
--rw-r--r--   0 runner    (1001) docker     (122)    17428 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/chain.py
--rw-r--r--   0 runner    (1001) docker     (122)    16925 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/chainapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    31309 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/chaintester.py
--rw-r--r--   0 runner    (1001) docker     (122)    10424 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4231 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/database.py
--rw-r--r--   0 runner    (1001) docker     (122)     4404 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/eos.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 06:18:31.781241 ipyeos-0.4.3/pysrc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/interfaces/Apply.py
--rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/interfaces/ApplyRequest.py
--rw-r--r--   0 runner    (1001) docker     (122)   156885 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/interfaces/IPCChainTester.py
--rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/interfaces/PushActions.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/interfaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/interfaces/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/ipykernel_embed.py
--rw-r--r--   0 runner    (1001) docker     (122)    15803 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/ipython_embed.py
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     5198 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/run.py
--rw-r--r--   0 runner    (1001) docker     (122)    52821 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/server.py
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-16 06:18:24.000000 ipyeos-0.4.3/pysrc/types.py
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-16 06:18:24.000000 ipyeos-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-16 06:18:31.785241 ipyeos-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-06-16 06:18:24.000000 ipyeos-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.155676 ipyeos-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-23 06:21:45.000000 ipyeos-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-23 06:21:45.000000 ipyeos-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-06-23 06:21:52.155676 ipyeos-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-06-23 06:21:45.000000 ipyeos-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.151676 ipyeos-0.4.4/ipyeos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.155676 ipyeos-0.4.4/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (122)     2056 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/args.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/block_log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18346 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16925 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/chainapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36344 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/chaintester.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10424 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   105769 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/database.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75454 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/database_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5078 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.155676 ipyeos-0.4.4/pysrc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/Apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/ApplyRequest.py
+-rw-r--r--   0 runner    (1001) docker     (122)   156885 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/IPCChainTester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/PushActions.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/ipykernel_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15803 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/ipython_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4526 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7188 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/packer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5198 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52821 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/structs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-23 06:21:45.000000 ipyeos-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-23 06:21:52.155676 ipyeos-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-23 06:21:45.000000 ipyeos-0.4.4/setup.py
```

### Comparing `ipyeos-0.4.3/LICENSE` & `ipyeos-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/__init__.py` & `ipyeos-0.4.4/pysrc/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import shlex
 import subprocess
 import sys
 import sysconfig
 
 from . import run
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 class CustomImporter(object):
     def find_module(self, fullname, mpath=None):
 #        print('+++find_module', fullname)
-        if fullname in ['_chain', '_chainapi', '_vm_api', '_database']:
+        if fullname in ['_chain', '_chainapi', '_vm_api', '_database', '_block_log']:
             return self
         return
 
     def load_module(self, module_name):
 #        print('+++load_module', module_name)
         mod = sys.modules.get(module_name)
         if mod is None:
@@ -36,14 +36,15 @@
     from . import _eos
     sys.meta_path.append(CustomImporter())
 
     import _chain
     import _chainapi
     import _vm_api
     import _database
+    import _block_log
 
 def run_ipyeos(custom_cmds=[]):
     return run.run_ipyeos(custom_cmds)
 
 def run_eosnode():
     custom_cmds=['-m', 'ipyeos', 'eosnode']
     custom_cmds.extend(sys.argv[1:])
```

### Comparing `ipyeos-0.4.3/pysrc/args.py` & `ipyeos-0.4.4/pysrc/args.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/chain.py` & `ipyeos-0.4.4/pysrc/chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 
 from . import _chain, _eos, log
-from .types import Name, PublicKey
+from .types import U8, U16, U32, U64, I64, Name, PublicKey
+from .block_log import BlockLog
 
 logger = log.get_logger(__name__)
 
 def isoformat(dt):
     return dt.isoformat(timespec='milliseconds')
 
 def handle_error(fn):
@@ -18,18 +19,18 @@
             err = self.get_last_error()
             raise Exception(err)
         return ret
     return call_method
 
 class Chain(object):
 
-    def __init__(self, config: dict, genesis: dict, protocol_features_dir: str, snapshot_dir: str):
-        self.new(config, genesis, protocol_features_dir, snapshot_dir)
+    def __init__(self, config: dict, genesis: dict, chain_id: str, protocol_features_dir: str, snapshot_dir: str):
+        self.new(config, genesis, chain_id, protocol_features_dir, snapshot_dir)
 
-    def new(self, config: dict, genesis: dict, protocol_features_dir: str, snapshot_dir: str) -> None:
+    def new(self, config: dict, genesis: dict, chain_id: str, protocol_features_dir: str, snapshot_dir: str) -> None:
         """
         Create a new Chain instance
         Code example::
             data = {
                 'key': 'value',
             }
             print(data)
@@ -43,28 +44,31 @@
         if isinstance(config, dict):
             config = json.dumps(config)
         if isinstance(genesis, dict):
             config = json.dumps(config)
         assert isinstance(config, str)
         assert isinstance(genesis, str)
 
-        self.ptr = _chain.chain_new(config, genesis, protocol_features_dir, snapshot_dir)
+        self.ptr = _chain.chain_new(config, genesis, chain_id, protocol_features_dir, snapshot_dir)
         if not self.ptr:
-            error = _eos.get_last_error()
+            error = _eos.get_last_error_and_clear()
             raise Exception(error)
 
     def startup(self, initdb: bool) -> bool:
         """
         Startup a chain
         Code example::
             chain.startup(True)
         :param bool initdb
         :returns bool: Return True on success, False on failture.
         """
-        return _chain.startup(self.ptr, initdb)
+        ret = _chain.startup(self.ptr, initdb)
+        if not ret:
+            self.ptr = 0
+            raise Exception(_eos.get_last_error_and_clear())
 
     def free(self) -> None:
         """
         Release a chain
         """
         if not self.ptr:
             return
@@ -211,17 +215,16 @@
 
     def fork_db_pending_head_block_time(self) -> str:
         return _chain.fork_db_pending_head_block_time(self.ptr)
 
     def fork_db_pending_head_block_producer(self) -> Name:
         return _chain.fork_db_pending_head_block_producer(self.ptr)
 
-    def pending_block_time(self) -> str:
-        iso_time = _chain.pending_block_time(self.ptr)
-        return datetime.strptime(iso_time, "%Y-%m-%dT%H:%M:%S.%f")
+    def pending_block_time(self) -> int:
+        return _chain.pending_block_time(self.ptr)
 
     def pending_block_producer(self) -> Name:
         return _chain.pending_block_producer(self.ptr)
 
     def pending_block_signing_key(self) -> str:
         return _chain.pending_block_signing_key(self.ptr)
 
@@ -276,15 +279,18 @@
 
     def check_contract_list(self, code: Name) -> bool:
         return _chain.check_contract_list(self.ptr, code)
 
     def check_action_list(self, code: Name, action: Name) -> bool:
         return _chain.check_action_list(self.ptr, code, action)
 
-    def check_key_list(self, pub_key: PublicKey) -> bool:
+    def check_key_list(self, pub_key: Union[str, PublicKey]) -> bool:
+        if isinstance(pub_key, PublicKey):
+            pub_key = pub_key.to_string()
+        assert isinstance(pub_key, str)
         return _chain.check_key_list(self.ptr, pub_key)
 
     def is_building_block(self) -> bool:
         return _chain.is_building_block(self.ptr)
 
     def is_speculative_block(self) -> bool:
         return _chain.is_speculative_block(self.ptr)
@@ -393,20 +399,32 @@
     #     return _chain.get_unapplied_transactions(self.ptr)
  
     def push_transaction(self, packed_trx: bytes, deadline: Union[str, datetime], billed_cpu_time_us: int, explicit_cpu_bill: int = 0, subjective_cpu_bill_us = 0) -> dict:
         if isinstance(deadline, datetime):
             deadline = deadline.isoformat(timespec='milliseconds')
         result = _chain.push_transaction(self.ptr, packed_trx, deadline, billed_cpu_time_us, explicit_cpu_bill, subjective_cpu_bill_us)
         if not result:
-            result = _eos.get_last_error()
+            result = _eos.get_last_error_and_clear()
         result = json.loads(result)
         if 'except' in result:
             raise Exception(result)
         return result
 
+    def push_block(self, log: BlockLog, block_num: int) -> bool:
+        if block_num > log.head_block_num() or block_num < log.first_block_num():
+            raise Exception("invalid block number, block_num: %d, head_block_num: %d, first_block_num: %d" % (block_num, log.head_block_num(), log.first_block_num()))
+        ret = _chain.push_block(self.ptr, log.get_block_log_ptr(), block_num)
+        if not ret:
+            err = _eos.get_last_error_and_clear()
+            if err:
+                raise Exception(err)
+            else:
+                raise Exception("invalid block num")
+        return True
+
     def get_scheduled_transaction(self, sender_id: int, sender: Name) -> dict:
         ret = _chain.get_scheduled_transaction(self.ptr, sender_id, sender)
         if ret:
             return json.loads(ret)
 
     def get_scheduled_transactions(self) -> dict:
         ret = _chain.get_scheduled_transactions(self.ptr)
@@ -470,15 +488,15 @@
 
         if isinstance(_private_keys, list):
             _private_keys = json.dumps(_private_keys)
 
         return _chain.gen_transaction(self.ptr, json_str, _actions, expiration, reference_block_id, _id, compress, _private_keys)
 
     def get_last_error(self) -> str:
-        err = _eos.get_last_error()
+        err = _eos.get_last_error_and_clear()
         try:
             return {'except': json.loads(err)}
         except json.JSONDecodeError:        
             err = json.dumps(err)
             return f'{{"except": {err}}}'
 
     def get_native_contract(self, contract: str) -> str:
```

### Comparing `ipyeos-0.4.3/pysrc/chainapi.py` & `ipyeos-0.4.4/pysrc/chainapi.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/chaintester.py` & `ipyeos-0.4.4/pysrc/chaintester.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import atexit
+from enum import Enum
+import hashlib
 import json
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
 from datetime import datetime, timedelta, timezone
@@ -11,33 +13,42 @@
 import pytest
 
 from ipyeos import chain, chainapi, database, config
 
 from . import eos, log
 from .types import Name
 
+from .packer import Decoder
+from .database_objects import GeneratedTransactionObject
+from .database import GeneratedTransactionObjectIndex
+
 logger = log.get_logger(__name__)
 
 test_dir = os.path.dirname(__file__)
 
 # default_time = datetime.fromtimestamp(946684800000/1e3, tz=timezone.utc)
 default_time = datetime.utcfromtimestamp(946684800000/1e3)
 
+class DBReadMode(Enum):
+    HEAD = 0
+    IRREVERSIBLE = 1
+    SPECULATIVE = 2
+
 chain_config = {
     "sender_bypass_whiteblacklist":[],
     "actor_whitelist":[],
     "actor_blacklist":[],
     "contract_whitelist":[],
     "contract_blacklist":[],
     "action_blacklist":[],
     "key_blacklist":[],
     "blocks_dir":"dd/blocks",
     "state_dir":"dd/state",
-    "state_size":1073741824,
-    "state_guard_size":134217728,
+    "state_size":104857600,
+    "state_guard_size":10485760,
     "sig_cpu_bill_pct":5000,
     "thread_pool_size":2,
     "max_nonprivileged_inline_action_size":4096,
     "read_only":False,
     "force_all_checks":False,
     "disable_replay_opts":False,
     "contracts_console":True,
@@ -50,15 +61,15 @@
     "wasm_runtime":"eos_vm_jit",
     "eosvmoc_config":
     {
         "cache_size":1073741824,
         "threads":1
     },
     "eosvmoc_tierup":False,
-    "read_mode":"HEAD",
+    "read_mode": DBReadMode.HEAD.name,
     "block_validation_mode":"FULL",
     "db_map_mode":"mapped",
     "resource_greylist":[],
     "trusted_producers":[],
     "greylist_limit":1000,
     "profile_accounts":[]
 }
@@ -121,52 +132,133 @@
     'EOS89jesRgvvnFVuNtLg4rkFXcBg2Qq26wjzppssdHj2a8PSoWMhx':'5JHRxntHapUryUetZgWdd3cg6BrpZLMJdqhhXnMaZiiT4qdJPhv',
     'EOS73ECcVHVWvuxJVm5ATnqBTCFMtA6WUsdDovdWH5NFHaXNq1hw1':'5Jbh1Dn57DKPUHQ6F6eExX55S2nSFNxZhpZUxNYFjJ1arKGK9Q3',
     'EOS8h8TmXCU7Pzo5XQKqyWwXAqLpPj4DPZCv5Wx9Y4yjRrB6R64ok':'5JJYrXzjt47UjHyo3ud5rVnNEPTCqWvf73yWHtVHtB1gsxtComG',
     'EOS65jj8NPh2EzLwje3YRy4utVAATthteZyhQabpQubxHNJ44mem9':'5J9PozRVudGYf2D4b8JzvGxPBswYbtJioiuvYaiXWDYaihNFGKP',
     'EOS5fVw435RSwW3YYWAX9qz548JFTWuFiBcHT3PGLryWaAMmxgjp1':'5K9AZWR2wEwtZii52vHigrxcSwCzLhhJbNpdXpVFKHP5fgFG5Tx'
 }
 
+def import_key(priv_key):
+    global key_map
+    pubkey = eos.get_public_key(priv_key)
+    key_map[pubkey] = priv_key
+    return True
+
+def import_producer_key(priv_key):
+    global producer_key_map
+    pubkey = eos.get_public_key(priv_key)
+    producer_key_map[pubkey] = priv_key
+    return True
+
 log_level_all = 0
 log_level_debug = 1
 log_level_info = 2
 log_level_warn = 3
 log_level_error = 4
 log_level_off = 5
 
+genesis_state_or_chain_id_version = 3
+
+def contains_genesis_state(version, first_block_num):
+    return version < genesis_state_or_chain_id_version or first_block_num == 1
+
+def contains_chain_id(version, first_block_num):
+    return version >= genesis_state_or_chain_id_version and first_block_num > 1
+
+def read_genesis_from_block_log(tester):
+    with open(f'{tester.data_dir}/blocks/blocks.log', 'rb') as f:
+        data = f.read()
+
+    dec = Decoder(data)
+    ver = dec.unpack_u32()
+    first_block_num = dec.unpack_u32()
+    if contains_genesis_state(ver, first_block_num):
+        # GenesisState.unpack(dec)
+        data = dec.read_bytes(68+8+34)
+        chain_id = hashlib.sha256(data).hexdigest()
+    elif contains_chain_id(ver, first_block_num):
+        chain_id = dec.read_bytes(32).hex()
+    assert chain_id == tester.api.get_info()['chain_id']
+
+def read_chain_id_from_block_log(data_dir):
+    with open(f'{data_dir}/blocks/blocks.log', 'rb') as f:
+        data = f.read(1024)
+
+    dec = Decoder(data)
+    ver = dec.unpack_u32()
+    first_block_num = dec.unpack_u32()
+    if contains_genesis_state(ver, first_block_num):
+        # GenesisState.unpack(dec)
+        data = dec.read_bytes(68+8+34)
+        return hashlib.sha256(data).hexdigest()
+    elif contains_chain_id(ver, first_block_num):
+        return dec.read_bytes(32).hex()
+    assert False, "unknown chain id"
+
 class ChainTester(object):
 
-    def __init__(self, initialize=True, log_level=log_level_debug):
+    def __init__(self, initialize=True, data_dir=None, config_dir=None, snapshot_dir='', state_size=10*1024*1024, log_level=log_level_debug):
         atexit.register(self.free)
+        self.is_temp_data_dir = True
+        self.is_temp_config_dir = True
+
+        chain_config['state_size'] = state_size
+        chain_config['state_guard_size'] = int(state_size * 0.005)
+
+        if data_dir:
+            self.data_dir = data_dir
+            self.is_temp_data_dir = False
+        else:
+            self.data_dir = tempfile.mkdtemp()
+
+        if config_dir:
+           self.config_dir = config_dir
+           self.is_temp_config_dir = False
+        else:
+            self.config_dir = tempfile.mkdtemp()
 
-        self.data_dir = tempfile.mkdtemp()
-        self.config_dir = tempfile.mkdtemp()
         logger.info('++++data_dir %s', self.data_dir)
         logger.info('++++config_dir %s', self.config_dir)
 
         chain_config['blocks_dir'] = os.path.join(self.data_dir, 'blocks')
         chain_config['state_dir'] = os.path.join(self.data_dir, 'state')
 
 
         eos.set_log_level('default', log_level)
+        
+        if snapshot_dir:
+            initialize = False
+            init_database = False
+            self.genesis_test = ''
+            self.chain_id = eos.extract_chain_id_from_snapshot(snapshot_dir)
+        elif os.path.exists(os.path.join(chain_config['state_dir'], 'shared_memory.bin')):
+            initialize = False
+            init_database = False
+            self.genesis_test = ''
+            self.chain_id = read_chain_id_from_block_log(self.data_dir)
+        else:
+            init_database = True
+            self.chain_id = ''
 
         self.chain_config = json.dumps(chain_config)
         self.genesis_test = json.dumps(genesis_test)
-        self.chain = chain.Chain(self.chain_config, self.genesis_test, os.path.join(self.config_dir, "protocol_features"), "")
-        self.chain.startup(True)
+        self.chain = chain.Chain(self.chain_config, self.genesis_test, self.chain_id, os.path.join(self.config_dir, "protocol_features"), snapshot_dir)
+        self.chain.startup(init_database)
         self.api = chainapi.ChainApi(self.chain)
 
         self.db = database.Database(self.chain.get_database())
 
         # logger.info(self.api.get_info())
         # logger.info(self.api.get_account('eosio'))
 
-        self.feature_digests = []
-
-        self.feature_digests = ['0ec7e080177b2c02b278d5088611686b49d739925a92d9bfcacd7fc6b74053bd']
-        self.start_block()
+        if not initialize:
+            self.feature_digests = []
+            self.start_block()
+        else:
+            self.feature_digests = ['0ec7e080177b2c02b278d5088611686b49d739925a92d9bfcacd7fc6b74053bd']
+            self.start_block()
         self.code_cache = {}
 
         if not initialize:
             return
 
         key = 'EOS6MRyAjQq8ud7hVNYcfnVPJqcVpscN5So8BhtHuGYqET5GDW5CV'
         systemAccounts = [
@@ -321,22 +413,28 @@
             abi = f.read()
         self.deploy_contract('eosio.mpy', code, abi)
 
     # def start_block(self):
     #     self.chain.start_block(self.calc_pending_block_time(), 0, self.feature_digests)
 
     def free(self):
-        if self.chain:
-            self.chain.free()
-            self.chain = None
-
-        if self.data_dir:
+        # in case of exception throw from __init__, chain may not be initialized
+        if not hasattr(self, 'chain'):
+            return
+        if not self.chain:
+            return
+        self.chain.free()
+        self.chain = None
+            
+        if self.is_temp_data_dir and self.data_dir:
             shutil.rmtree(self.data_dir)
-            shutil.rmtree(self.config_dir)
             self.data_dir = None
+
+        if self.is_temp_config_dir and self.config_dir:
+            shutil.rmtree(self.config_dir)
             self.config_dir = None
 
     def __del__(self):
         self.free()
 
     def get_account(self, account):
         return self.api.get_account(account)
@@ -351,18 +449,28 @@
                     pub_key = key['key']
                     pub_key = pub_key.replace('UUOS', 'EOS', 1)
                     if pub_key in key_map:
                         priv_key = key_map[pub_key]
                         keys.append(priv_key)
         return keys
 
-    def import_key(self, pubkey, priv_key):
+    @classmethod
+    def import_key(cls, priv_key):
+        global key_map
+        pubkey = eos.get_public_key(priv_key)
         key_map[pubkey] = priv_key
         return True
 
+    @classmethod
+    def import_producer_key(cls, priv_key):
+        global producer_key_map
+        pubkey = eos.get_public_key(priv_key)
+        producer_key_map[pubkey] = priv_key
+        return True
+
     def push_action(self, account: Name, action: Name, args: Union[Dict, str, bytes], permissions: Dict={}, explicit_cpu_bill=False):
         auth = []
         for actor in permissions:
             perm = permissions[actor]
             auth.append({'actor': actor, 'permission': perm})
         if not auth:
             auth.append({'actor': account, 'permission': 'active'})
@@ -500,21 +608,50 @@
             # logger.info(block_time)
             self.chain.start_block(block_time, 0, self.feature_digests)
 
         self.feature_digests.clear()
 
     def produce_block(self, next_block_time=default_time, start_block=True):
         trxs = self.chain.get_scheduled_transactions()
+        idx = GeneratedTransactionObjectIndex(self.db)
+        pending_block_time = self.chain.pending_block_time()
+        ready_txs = []
+        def get_ready_trx(data, user_data):
+            # print(tp, data)
+            dec = Decoder(data)
+            #     transaction_id_type           trx_id;
+            #     account_name                  sender;
+            #     uint128_t                     sender_id;
+            #     account_name                  payer;
+            #     time_point                    delay_until; /// this generated transaction will not be applied until the specified time
+            #     time_point                    expiration; /// this generated transaction will not be applied after this time
+            #     time_point                    published;
+            table_id = dec.unpack_u64()
+            trx_id = dec.read_bytes(32).hex()
+            sender = dec.unpack_name()
+            sender_id = dec.unpack_u128()
+            payer = dec.unpack_name()
+            delay_until = dec.unpack_i64()
+            # print('+++delay_until:', delay_until, pending_block_time)
+            if pending_block_time > delay_until:
+                return 0
+            ready_txs.append(trx_id)
+            return 1
+            # expiration = dec.unpack_i64()
+            # published = dec.unpack_i64()
+        idx.walk_by_expiration(get_ready_trx, raw_data=True)
+        # print('+++ready_txs:', ready_txs)
+
         deadline = datetime.utcnow() + timedelta(microseconds=10000000)
         priv_keys = []
         for pub_key in self.chain.get_producer_public_keys():
             if pub_key in producer_key_map:
                 priv_keys.append(producer_key_map[pub_key])
 
-        for scheduled_tx_id in trxs:
+        for scheduled_tx_id in ready_txs:
             self.chain.push_scheduled_transaction(scheduled_tx_id, deadline, 100)
         # logger.info("+++priv_keys: %s", priv_keys)
         self.chain.finalize_block(priv_keys)
         self.chain.commit_block()
         if start_block:
             self.start_block(next_block_time)
 
@@ -667,17 +804,15 @@
             'authorization':[{'actor': account, 'permission':'active'}]
         }
         actions.append(setabi)
         ret = self.push_actions_ex(actions)
         self.chain.clear_abi_cache(account)
         return ret
 
-    def transfer(self, _from: Name, _to: Name, _amount: float, _memo: str='', token_account: Name='eosio.token', token_name: str='', permission: Name='active'):
-        if not token_name:
-            token_name = self.main_token
+    def transfer(self, _from: Name, _to: Name, _amount: float, _memo: str='', token_account: Name='eosio.token', token_name: str='EOS', permission: Name='active'):
         args = {"from":_from, "to":_to, "quantity":'%.4f %s'%(_amount,token_name), "memo":_memo}
         return self.push_action(token_account, 'transfer', args, {_from:permission})
 
     def pack_action_args(self, account: Name, action: Name , args: Union[dict, str]):
         ret = self.chain.pack_action_args(account, action, args)
         if ret is None:
             error = self.chain.get_last_error()
```

### Comparing `ipyeos-0.4.3/pysrc/config.py` & `ipyeos-0.4.4/pysrc/config.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/eos.py` & `ipyeos-0.4.4/pysrc/eos.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import sys
 from typing import Union
+from enum import Enum
 
 from . import _eos
 from .types import Name
 
 
 class NativeType:
     handshake_message = 0
@@ -16,42 +17,51 @@
     sync_request_message = 6
     signed_block_v0 = 7         # which = 7
     packed_transaction_v0 = 8   # which = 8
     signed_block = 9            # which = 9
     trx_message_v1 = 10         # which = 10
     genesis_state = 11
     abi_def = 12
+    transaction_type = 13
+    global_property_type = 14
 
-LOG_LEVEL_ALL = 0
-LOG_LEVEL_DEBUG = 1
-LOG_LEVEL_INFO = 2
-LOG_LEVEL_WARN = 3
-LOG_LEVEL_ERROR = 4
-LOG_LEVEL_OFF = 5
-
-def set_log_level(logger_name: str, level: int) -> None:
+class LogLevel(Enum):
+    ALL = 0
+    DEBUG = 1
+    INFO = 2
+    WARN = 3
+    ERROR = 4
+    OFF = 5
+
+def set_log_level(logger_name: str, level: Union[int, LogLevel]) -> None:
+    if isinstance(level, LogLevel):
+        level = level.value
     _eos.set_log_level(logger_name, level)
 
-def set_all_level(logger_name: str) -> None:
-    _eos.set_log_level(logger_name, LOG_LEVEL_ALL)
+def get_log_level(logger_name: str = "default") -> int:
+    value = _eos.get_log_level(logger_name)
+    return LogLevel(value)
+
+def set_all_level(logger_name: str = 'default') -> None:
+    _eos.set_log_level(logger_name, LogLevel.ALL.value)
 
-def set_debug_level(logger_name: str) -> None:
-    _eos.set_log_level(logger_name, LOG_LEVEL_DEBUG)
+def set_debug_level(logger_name: str = 'default') -> None:
+    _eos.set_log_level(logger_name, LogLevel.DEBUG.value)
 
-def set_info_level(logger_name: str) -> None:
-    _eos.set_log_level(logger_name, LOG_LEVEL_INFO)
+def set_info_level(logger_name: str = 'default') -> None:
+    _eos.set_log_level(logger_name, LogLevel.INFO.value)
 
-def set_warn_level(logger_name: str) -> None:
-    _eos.set_log_level(logger_name, LOG_LEVEL_WARN)
+def set_warn_level(logger_name: str = 'default') -> None:
+    _eos.set_log_level(logger_name, LogLevel.WARN.value)
 
-def set_error_level(logger_name: str) -> None:
-    _eos.set_log_level(logger_name, LOG_LEVEL_ERROR)
+def set_error_level(logger_name: str = 'default') -> None:
+    _eos.set_log_level(logger_name, LogLevel.ERROR.value)
 
-def set_off_level(logger_name: str) -> None:
-    _eos.set_log_level(logger_name, LOG_LEVEL_OFF)
+def set_off_level(logger_name: str = 'default') -> None:
+    _eos.set_log_level(logger_name, LogLevel.OFF.value)
 
 def pack_native_object(_type: int, obj: Union[dict, str]) -> bytes:
     if isinstance(obj, dict):
         obj = json.dumps(obj)
     else:
         assert isinstance(obj, (str, bytes))
     return _eos.pack_native_object(_type, obj)
@@ -80,15 +90,15 @@
 def s2n(s: str) -> int:
     '''
     Convert a EOSIO name to uint64_t
     '''
     ret = _eos.s2n(s)
     if not ret == 0:
         return ret
-    err = _eos.get_last_error()
+    err = _eos.get_last_error_and_clear()
     if err:
         _eos.set_last_error("")
         raise Exception(err)
     return ret
 
 def n2s(n: int) -> str:
     '''
@@ -136,29 +146,32 @@
 def enable_debug(debug) -> None:
     _eos.enable_debug(debug)
 
 def is_debug_enabled() -> bool:
     return _eos.is_debug_enabled()
 
 def get_last_error() -> str:
-    return _eos.get_last_error()
+    return _eos.get_last_error_and_clear()
 
 def create_key(key_type: str = "K1") -> dict:
     ret = _eos.create_key(key_type)
     return json.loads(ret)
 
 def check_ret(ret):
     if not ret:
         raise Exception(get_last_error())
     return ret
 
 def get_public_key(priv_key: str) -> str:
     ret = _eos.get_public_key(priv_key)
     return check_ret(ret)
 
+def extract_chain_id_from_snapshot(snapshot: str) -> str:
+    return _eos.extract_chain_id_from_snapshot(snapshot)
+
 def sign_digest(digest: str, priv_key: str):
     ret = _eos.sign_digest(digest, priv_key)
     return check_ret(ret)
 
 def init(argv=None) -> int:
     if argv:
         return _eos.init(argv)
@@ -171,7 +184,13 @@
     return _eos.run_once()
 
 def post(fn, *args, **kwargs):
     return _eos.post(fn, *args, **kwargs)
 
 def quit() -> None:
     _eos.quit()
+
+def set_debug_producer_key(pub_key: str):
+    _eos.set_debug_producer_key(pub_key)
+
+def get_debug_producer_key() -> str:
+    return _eos.get_debug_producer_key()
```

### Comparing `ipyeos-0.4.3/pysrc/interfaces/Apply.py` & `ipyeos-0.4.4/pysrc/interfaces/Apply.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/interfaces/ApplyRequest.py` & `ipyeos-0.4.4/pysrc/interfaces/ApplyRequest.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/interfaces/IPCChainTester.py` & `ipyeos-0.4.4/pysrc/interfaces/IPCChainTester.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/interfaces/PushActions.py` & `ipyeos-0.4.4/pysrc/interfaces/PushActions.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/interfaces/ttypes.py` & `ipyeos-0.4.4/pysrc/interfaces/ttypes.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/ipykernel_embed.py` & `ipyeos-0.4.4/pysrc/ipykernel_embed.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/ipython_embed.py` & `ipyeos-0.4.4/pysrc/ipython_embed.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/main.py` & `ipyeos-0.4.4/pysrc/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 commands:
 /ipython start ipython
 /ikernel start ikernel
 /quit quit app
     '''
     return web.Response(text=commands)
 
+def print_help():
+    argv = sys.argv[1:]
+    argv[0] = 'ipyeos'
+    return eos.init(argv)
+
 def _run_eos():
     argv = sys.argv[1:]
     argv[0] = 'ipyeos'
     ret = eos.init(argv)
     if not ret == 0:
         print('init return', ret)
         return
@@ -43,14 +48,15 @@
     # while True:
     #     ret = eos.run_once()
     #     if not ret == 0:
     #         break
     #     await asyncio.sleep(0.0)
     #     print('run once')
     print('run return', ret)
+    return ret
 
 async def run_eos():
     future = asyncio.get_event_loop().run_in_executor(executor, _run_eos)
     await future
     await async_queue.put(None)
 
 
@@ -88,18 +94,18 @@
     app.router.add_get('/ipython', run_ipython)
     app.router.add_get('/ikernel', run_ikernel)
     app.router.add_get('/quit', quit_app)
     app.router.add_get('/', hello)
     runner = web.AppRunner(app)
     await runner.setup()
     try:
-        site = web.TCPSite(runner, 'localhost', 7777)
+        site = web.TCPSite(runner, host='127.0.0.1', port=7777)
     except Exception as e:
         print(e)
-        site = web.TCPSite(runner, 'localhost', 7778)
+        site = web.TCPSite(runner, host='127.0.0.1', port=7778)
     await site.start()
     print('++++++++++++server started!!')
     while True:
         await asyncio.sleep(3600) # serve forever
 
 async def heartbeat():
     while True:
@@ -124,16 +130,17 @@
             # future = asyncio.get_event_loop().run_in_executor(executor, _run_ipython)
 
     # result = await future
     # print("Result: ", result)
     print('all done!')
 
 def run():
-    result = args.parse_args()
-    if result.subparser == 'eosnode':
+    if sys.argv[1] == 'eosnode':
+        if sys.argv[2] in ['-h', '--help']:
+            return print_help()
         def start():
             asyncio.run(main())
             thread_queue.put(None)
         t = threading.Thread(target=start, daemon=True)
         t.start()
         while True:
             try:
@@ -142,12 +149,14 @@
                     break
                 if cmd == 'ikernel':
                     _run_ikernel()
                 elif cmd == 'ipython':
                     _run_ipython()
             except KeyboardInterrupt:
                 eos.post(eos.quit)
-
-    elif result.subparser == 'eosdebugger':
-        server.start_debug_server(result.addr, result.server_port, result.vm_api_port, result.apply_request_addr, result.apply_request_port, result.addr,result.rpc_server_port)
     else:
-        parser.print_help()
+        result = args.parse_args()
+        if result.subparser == 'eosdebugger':
+            result = args.parse_args()
+            server.start_debug_server(result.addr, result.server_port, result.vm_api_port, result.apply_request_addr, result.apply_request_port, result.addr,result.rpc_server_port)
+        else:
+            parser.print_help()
```

### Comparing `ipyeos-0.4.3/pysrc/rpc_server.py` & `ipyeos-0.4.4/pysrc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/run.py` & `ipyeos-0.4.4/pysrc/run.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/pysrc/server.py` & `ipyeos-0.4.4/pysrc/server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.3/setup.py` & `ipyeos-0.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'tests/contracts/micropython/*',
     'tests/test_template.py',
     'tests/activate_kv.wasm',
 ])
 
 setup(
     name="ipyeos",
-    version="0.4.3",
+    version="0.4.4",
     description="IPYEOS project",
     author='The IPYEOS Team',
     license="MIT",
     packages=[
         'ipyeos',
         'ipyeos.interfaces'
     ],
@@ -43,12 +43,13 @@
     package_data={'ipyeos': release_files},
 
     install_requires=[
         'thrift>=0.16.0',
         'pytest>=6.2.5',
         'aiohttp>=3.8.4',
         'ipython',
-        'ipykernel'
+        'ipykernel',
+        'base58'
     ],
     tests_require=[],
     include_package_data=True
 )
```

