# Comparing `tmp/better_web3-1.0.0.tar.gz` & `tmp/better_web3-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-1.0.0.tar", max compression
+gzip compressed data, was "better_web3-1.1.0.tar", max compression
```

## Comparing `better_web3-1.0.0.tar` & `better_web3-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,33 @@
--rw-r--r--   0        0        0      361 2023-06-09 17:01:02.289000 better_web3-1.0.0/better_web3/__init__.py
--rw-r--r--   0        0        0    46649 2023-06-13 20:28:07.542000 better_web3-1.0.0/better_web3/chain.py
--rw-r--r--   0        0        0      202 2023-06-04 17:02:17.456000 better_web3-1.0.0/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.0.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.0.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0      604 2023-06-05 07:45:48.506000 better_web3-1.0.0/better_web3/contract/__pycache__/abi.cpython-311.pyc
--rw-r--r--   0        0        0     3132 2023-06-07 15:59:49.144000 better_web3-1.0.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     8967 2023-06-07 15:59:53.327000 better_web3-1.0.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     6418 2023-06-06 08:36:22.616000 better_web3-1.0.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0      808 2023-06-05 09:50:56.141000 better_web3-1.0.0/better_web3/contract/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     1284 2023-06-05 16:58:24.463000 better_web3-1.0.0/better_web3/contract/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0    10577 2023-06-05 16:58:24.377000 better_web3-1.0.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.0.0/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.0.0/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.0.0/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.0.0/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.0.0/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0      290 2023-06-05 07:40:59.110000 better_web3-1.0.0/better_web3/contract/abi.py
--rw-r--r--   0        0        0     1347 2023-06-07 12:04:43.463000 better_web3-1.0.0/better_web3/contract/contract.py
--rw-r--r--   0        0        0     5030 2023-06-07 11:41:23.034000 better_web3-1.0.0/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     3636 2023-06-05 18:54:54.691000 better_web3-1.0.0/better_web3/contract/erc721.py
--rw-r--r--   0        0        0      164 2023-06-05 09:36:29.405000 better_web3-1.0.0/better_web3/contract/exceptions.py
--rw-r--r--   0        0        0      342 2023-06-05 16:09:26.806000 better_web3-1.0.0/better_web3/contract/model.py
--rw-r--r--   0        0        0     7263 2023-06-05 16:09:26.747000 better_web3-1.0.0/better_web3/contract/multicall.py
--rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.0.0/better_web3/enums.py
--rw-r--r--   0        0        0     3477 2023-06-13 20:28:07.471000 better_web3-1.0.0/better_web3/exceptions.py
--rw-r--r--   0        0        0     2256 2023-06-10 15:04:17.723000 better_web3-1.0.0/better_web3/explorer.py
--rw-r--r--   0        0        0      723 2023-06-10 15:04:17.431000 better_web3-1.0.0/better_web3/gas_station.py
--rw-r--r--   0        0        0     1209 2023-06-09 18:55:57.955000 better_web3-1.0.0/better_web3/models.py
--rw-r--r--   0        0        0      140 2023-06-05 13:43:52.746000 better_web3-1.0.0/better_web3/types.py
--rw-r--r--   0        0        0      505 2023-06-13 11:36:45.357000 better_web3-1.0.0/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      755 2023-06-13 11:36:47.198000 better_web3-1.0.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3888 2023-06-13 11:36:47.231000 better_web3-1.0.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     1392 2023-06-04 17:49:31.548000 better_web3-1.0.0/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0      808 2023-06-05 09:50:55.894000 better_web3-1.0.0/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0     2381 2023-06-13 11:34:00.354000 better_web3-1.0.0/better_web3/utils/eth.py
--rw-r--r--   0        0        0      467 2023-06-04 15:48:03.874000 better_web3-1.0.0/better_web3/utils/file.py
--rw-r--r--   0        0        0      315 2023-06-04 15:48:04.240000 better_web3-1.0.0/better_web3/utils/other.py
--rw-r--r--   0        0        0      455 2023-06-13 20:41:51.431000 better_web3-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      349 2023-06-05 15:41:18.596000 better_web3-1.0.0/README.md
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 better_web3-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      332 2023-06-23 09:35:05.770000 better_web3-1.1.0/better_web3/__init__.py
+-rw-r--r--   0        0        0     9431 2023-06-22 18:23:50.481000 better_web3-1.1.0/better_web3/batch_call.py
+-rw-r--r--   0        0        0    12399 2023-06-23 10:58:37.851000 better_web3-1.1.0/better_web3/chain.py
+-rw-r--r--   0        0        0      202 2023-06-04 17:02:17.456000 better_web3-1.1.0/better_web3/contract/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.1.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.1.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      604 2023-06-05 07:45:48.506000 better_web3-1.1.0/better_web3/contract/__pycache__/abi.cpython-311.pyc
+-rw-r--r--   0        0        0     3132 2023-06-07 15:59:49.144000 better_web3-1.1.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
+-rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.1.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.1.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.1.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.1.0/better_web3/contract/_paths.py
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.1.0/better_web3/contract/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.1.0/better_web3/contract/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.1.0/better_web3/contract/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.1.0/better_web3/contract/abi/multicall_v3.json
+-rw-r--r--   0        0        0      290 2023-06-05 07:40:59.110000 better_web3-1.1.0/better_web3/contract/abi.py
+-rw-r--r--   0        0        0     1347 2023-06-07 12:04:43.463000 better_web3-1.1.0/better_web3/contract/contract.py
+-rw-r--r--   0        0        0     1749 2023-06-22 18:23:50.372000 better_web3-1.1.0/better_web3/contract/erc20.py
+-rw-r--r--   0        0        0     2873 2023-06-22 18:23:50.412000 better_web3-1.1.0/better_web3/contract/erc721.py
+-rw-r--r--   0        0        0     6182 2023-06-22 17:29:46.245000 better_web3-1.1.0/better_web3/contract/multicall.py
+-rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.1.0/better_web3/enums.py
+-rw-r--r--   0        0        0      554 2023-06-23 09:34:50.577000 better_web3-1.1.0/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-23 09:34:51.967000 better_web3-1.1.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.1.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     1167 2023-06-23 09:34:52.007000 better_web3-1.1.0/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     1125 2023-06-23 09:34:52.052000 better_web3-1.1.0/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.1.0/better_web3/utils/eth.py
+-rw-r--r--   0        0        0      301 2023-06-23 09:34:50.776000 better_web3-1.1.0/better_web3/utils/file.py
+-rw-r--r--   0        0        0      550 2023-06-23 09:34:50.673000 better_web3-1.1.0/better_web3/utils/other.py
+-rw-r--r--   0        0        0      455 2023-06-19 19:00:52.064000 better_web3-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-06-23 11:07:22.626000 better_web3-1.1.0/README.md
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 better_web3-1.1.0/PKG-INFO
```

### Comparing `better_web3-1.0.0/better_web3/contract/__pycache__/abi.cpython-311.pyc` & `better_web3-1.1.0/better_web3/contract/__pycache__/abi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.0.0/better_web3/contract/__pycache__/contract.cpython-311.pyc` & `better_web3-1.1.0/better_web3/contract/__pycache__/contract.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.0.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-1.1.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,553 +1,562 @@
 magic:    0xa70d0d0a
-moddate:  0xb6087e64 (Mon Jun  5 16:09:26 2023 UTC)
-files sz: 7263
+moddate:  0x0a859464 (Thu Jun 22 17:29:46 2023 UTC)
+files sz: 6182
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a046d
-      055a056d065a066d075a076d085a080100640164046c095a09640164056c
-      0a6d0b5a0b0100640164066c0c6d0d5a0d6d0e5a0e6d0f5a0f0100640164
-      076c106d115a110100640164086c126d135a130100640164096c146d155a
-      1501006401640a6c166d175a1701006401640b6c186d195a190100640c64
-      0d6c1a6d1b5a1b0100640e640f6c1c6d1d5a1d0100640e64106c1e6d1f5a
-      1f0100640164116c036d205a20010065207206640c64126c216d225a2201
-      0064135a23650202004700641484006415a6020000ab0200000000000000
-      00a6000000ab0000000000000000005a24650202004700641684006417a6
-      020000ab020000000000000000a6000000ab0000000000000000005a2502
-      004700641884006419651fa6030000ab0300000000000000005a26640453
-      00
+      055a050100640164046c065a06640164056c076d085a080100640164066c
+      096d0a5a0a6d0b5a0b6d0c5a0c0100640164076c0d6d0e5a0e0100640164
+      086c0f6d105a100100640164096c116d125a1201006401640a6c136d145a
+      1401006401640b6c156d165a160100640c640d6c176d185a180100640c64
+      0e6c196d1a5a1a01006401640f6c036d1b5a1b0100651b7206641064116c
+      1c6d1d5a1d010064125a1e650202004700641384006414a6020000ab0200
+      00000000000000a6000000ab0000000000000000005a1f65020200470064
+      1584006416a6020000ab020000000000000000a6000000ab000000000000
+      0000005a20020047006417840064186521a6030000ab0300000000000000
+      005a220200470064198400641a651aa6030000ab0300000000000000005a
+      2364045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('More about MulticallV3: https://github.com/mds1/multicall\n')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('dataclass',))
                 10 IMPORT_NAME              1 (dataclasses)
                 12 IMPORT_FROM              2 (dataclass)
                 14 STORE_NAME               2 (dataclass)
                 16 POP_TOP
    
      4          18 LOAD_CONST               1 (0)
-                20 LOAD_CONST               3 (('Any', 'List', 'Optional', 'Sequence', 'Tuple'))
+                20 LOAD_CONST               3 (('Any', 'Sequence'))
                 22 IMPORT_NAME              3 (typing)
                 24 IMPORT_FROM              4 (Any)
                 26 STORE_NAME               4 (Any)
-                28 IMPORT_FROM              5 (List)
-                30 STORE_NAME               5 (List)
-                32 IMPORT_FROM              6 (Optional)
-                34 STORE_NAME               6 (Optional)
-                36 IMPORT_FROM              7 (Sequence)
-                38 STORE_NAME               7 (Sequence)
-                40 IMPORT_FROM              8 (Tuple)
-                42 STORE_NAME               8 (Tuple)
-                44 POP_TOP
-   
-     6          46 LOAD_CONST               1 (0)
-                48 LOAD_CONST               4 (None)
-                50 IMPORT_NAME              9 (eth_abi)
-                52 STORE_NAME               9 (eth_abi)
-   
-     7          54 LOAD_CONST               1 (0)
-                56 LOAD_CONST               5 (('DecodingError',))
-                58 IMPORT_NAME             10 (eth_abi.exceptions)
-                60 IMPORT_FROM             11 (DecodingError)
-                62 STORE_NAME              11 (DecodingError)
-                64 POP_TOP
-   
-     8          66 LOAD_CONST               1 (0)
-                68 LOAD_CONST               6 (('BlockIdentifier', 'BlockNumber', 'ChecksumAddress'))
-                70 IMPORT_NAME             12 (eth_typing)
-                72 IMPORT_FROM             13 (BlockIdentifier)
-                74 STORE_NAME              13 (BlockIdentifier)
-                76 IMPORT_FROM             14 (BlockNumber)
-                78 STORE_NAME              14 (BlockNumber)
-                80 IMPORT_FROM             15 (ChecksumAddress)
-                82 STORE_NAME              15 (ChecksumAddress)
+                28 IMPORT_FROM              5 (Sequence)
+                30 STORE_NAME               5 (Sequence)
+                32 POP_TOP
+   
+     6          34 LOAD_CONST               1 (0)
+                36 LOAD_CONST               4 (None)
+                38 IMPORT_NAME              6 (eth_abi)
+                40 STORE_NAME               6 (eth_abi)
+   
+     7          42 LOAD_CONST               1 (0)
+                44 LOAD_CONST               5 (('DecodingError',))
+                46 IMPORT_NAME              7 (eth_abi.exceptions)
+                48 IMPORT_FROM              8 (DecodingError)
+                50 STORE_NAME               8 (DecodingError)
+                52 POP_TOP
+   
+     8          54 LOAD_CONST               1 (0)
+                56 LOAD_CONST               6 (('BlockIdentifier', 'BlockNumber', 'ChecksumAddress'))
+                58 IMPORT_NAME              9 (eth_typing)
+                60 IMPORT_FROM             10 (BlockIdentifier)
+                62 STORE_NAME              10 (BlockIdentifier)
+                64 IMPORT_FROM             11 (BlockNumber)
+                66 STORE_NAME              11 (BlockNumber)
+                68 IMPORT_FROM             12 (ChecksumAddress)
+                70 STORE_NAME              12 (ChecksumAddress)
+                72 POP_TOP
+   
+     9          74 LOAD_CONST               1 (0)
+                76 LOAD_CONST               7 (('HexBytes',))
+                78 IMPORT_NAME             13 (hexbytes)
+                80 IMPORT_FROM             14 (HexBytes)
+                82 STORE_NAME              14 (HexBytes)
                 84 POP_TOP
    
-     9          86 LOAD_CONST               1 (0)
-                88 LOAD_CONST               7 (('HexBytes',))
-                90 IMPORT_NAME             16 (hexbytes)
-                92 IMPORT_FROM             17 (HexBytes)
-                94 STORE_NAME              17 (HexBytes)
+    10          86 LOAD_CONST               1 (0)
+                88 LOAD_CONST               8 (('map_abi_data',))
+                90 IMPORT_NAME             15 (web3._utils.abi)
+                92 IMPORT_FROM             16 (map_abi_data)
+                94 STORE_NAME              16 (map_abi_data)
                 96 POP_TOP
    
-    10          98 LOAD_CONST               1 (0)
-               100 LOAD_CONST               8 (('map_abi_data',))
-               102 IMPORT_NAME             18 (web3._utils.abi)
-               104 IMPORT_FROM             19 (map_abi_data)
-               106 STORE_NAME              19 (map_abi_data)
+    11          98 LOAD_CONST               1 (0)
+               100 LOAD_CONST               9 (('BASE_RETURN_NORMALIZERS',))
+               102 IMPORT_NAME             17 (web3._utils.normalizers)
+               104 IMPORT_FROM             18 (BASE_RETURN_NORMALIZERS)
+               106 STORE_NAME              18 (BASE_RETURN_NORMALIZERS)
                108 POP_TOP
    
-    11         110 LOAD_CONST               1 (0)
-               112 LOAD_CONST               9 (('BASE_RETURN_NORMALIZERS',))
-               114 IMPORT_NAME             20 (web3._utils.normalizers)
-               116 IMPORT_FROM             21 (BASE_RETURN_NORMALIZERS)
-               118 STORE_NAME              21 (BASE_RETURN_NORMALIZERS)
+    12         110 LOAD_CONST               1 (0)
+               112 LOAD_CONST              10 (('ContractFunction',))
+               114 IMPORT_NAME             19 (web3.contract.contract)
+               116 IMPORT_FROM             20 (ContractFunction)
+               118 STORE_NAME              20 (ContractFunction)
                120 POP_TOP
    
-    12         122 LOAD_CONST               1 (0)
-               124 LOAD_CONST              10 (('ContractFunction',))
-               126 IMPORT_NAME             22 (web3.contract.contract)
-               128 IMPORT_FROM             23 (ContractFunction)
-               130 STORE_NAME              23 (ContractFunction)
+    13         122 LOAD_CONST               1 (0)
+               124 LOAD_CONST              11 (('ContractLogicError',))
+               126 IMPORT_NAME             21 (web3.exceptions)
+               128 IMPORT_FROM             22 (ContractLogicError)
+               130 STORE_NAME              22 (ContractLogicError)
                132 POP_TOP
    
-    13         134 LOAD_CONST               1 (0)
-               136 LOAD_CONST              11 (('ContractLogicError',))
-               138 IMPORT_NAME             24 (web3.exceptions)
-               140 IMPORT_FROM             25 (ContractLogicError)
-               142 STORE_NAME              25 (ContractLogicError)
+    15         134 LOAD_CONST              12 (1)
+               136 LOAD_CONST              13 (('MULTICALL_V3_ABI',))
+               138 IMPORT_NAME             23 (abi)
+               140 IMPORT_FROM             24 (MULTICALL_V3_ABI)
+               142 STORE_NAME              24 (MULTICALL_V3_ABI)
                144 POP_TOP
    
-    15         146 LOAD_CONST              12 (2)
-               148 LOAD_CONST              13 (('BatchCallFunctionFailed',))
-               150 IMPORT_NAME             26 (exceptions)
-               152 IMPORT_FROM             27 (BatchCallFunctionFailed)
-               154 STORE_NAME              27 (BatchCallFunctionFailed)
+    16         146 LOAD_CONST              12 (1)
+               148 LOAD_CONST              14 (('Contract',))
+               150 IMPORT_NAME             25 (contract)
+               152 IMPORT_FROM             26 (Contract)
+               154 STORE_NAME              26 (Contract)
                156 POP_TOP
    
-    16         158 LOAD_CONST              14 (1)
-               160 LOAD_CONST              15 (('MULTICALL_V3_ABI',))
-               162 IMPORT_NAME             28 (abi)
-               164 IMPORT_FROM             29 (MULTICALL_V3_ABI)
-               166 STORE_NAME              29 (MULTICALL_V3_ABI)
+    18         158 LOAD_CONST               1 (0)
+               160 LOAD_CONST              15 (('TYPE_CHECKING',))
+               162 IMPORT_NAME              3 (typing)
+               164 IMPORT_FROM             27 (TYPE_CHECKING)
+               166 STORE_NAME              27 (TYPE_CHECKING)
                168 POP_TOP
    
-    17         170 LOAD_CONST              14 (1)
-               172 LOAD_CONST              16 (('Contract',))
-               174 IMPORT_NAME             30 (contract)
-               176 IMPORT_FROM             31 (Contract)
-               178 STORE_NAME              31 (Contract)
-               180 POP_TOP
-   
-    19         182 LOAD_CONST               1 (0)
-               184 LOAD_CONST              17 (('TYPE_CHECKING',))
-               186 IMPORT_NAME              3 (typing)
-               188 IMPORT_FROM             32 (TYPE_CHECKING)
-               190 STORE_NAME              32 (TYPE_CHECKING)
-               192 POP_TOP
-   
-    20         194 LOAD_NAME               32 (TYPE_CHECKING)
-               196 POP_JUMP_FORWARD_IF_FALSE     6 (to 210)
-   
-    21         198 LOAD_CONST              12 (2)
-               200 LOAD_CONST              18 (('Chain',))
-               202 IMPORT_NAME             33 (chain)
-               204 IMPORT_FROM             34 (Chain)
-               206 STORE_NAME              34 (Chain)
-               208 POP_TOP
-   
-    24     >>  210 LOAD_CONST              19 ('0xcA11bde05977b3631167028862bE2a173976CA11')
-               212 STORE_NAME              35 (MULTICALL_V3_ADDRESS)
-   
-    27         214 LOAD_NAME                2 (dataclass)
-   
-    28         216 PUSH_NULL
-               218 LOAD_BUILD_CLASS
-               220 LOAD_CONST              20 (<code object MulticallResult, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 27>)
-               222 MAKE_FUNCTION            0
-               224 LOAD_CONST              21 ('MulticallResult')
-               226 PRECALL                  2
-               230 CALL                     2
-   
-    27         240 PRECALL                  0
-               244 CALL                     0
-   
-    28         254 STORE_NAME              36 (MulticallResult)
-   
-    33         256 LOAD_NAME                2 (dataclass)
-   
-    34         258 PUSH_NULL
-               260 LOAD_BUILD_CLASS
-               262 LOAD_CONST              22 (<code object MulticallDecodedResult, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 33>)
-               264 MAKE_FUNCTION            0
-               266 LOAD_CONST              23 ('MulticallDecodedResult')
-               268 PRECALL                  2
-               272 CALL                     2
-   
-    33         282 PRECALL                  0
-               286 CALL                     0
-   
-    34         296 STORE_NAME              37 (MulticallDecodedResult)
-   
-    39         298 PUSH_NULL
-               300 LOAD_BUILD_CLASS
-               302 LOAD_CONST              24 (<code object Multicall, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 39>)
-               304 MAKE_FUNCTION            0
-               306 LOAD_CONST              25 ('Multicall')
-               308 LOAD_NAME               31 (Contract)
-               310 PRECALL                  3
-               314 CALL                     3
-               324 STORE_NAME              38 (Multicall)
-               326 LOAD_CONST               4 (None)
-               328 RETURN_VALUE
+    19         170 LOAD_NAME               27 (TYPE_CHECKING)
+               172 POP_JUMP_FORWARD_IF_FALSE     6 (to 186)
+   
+    20         174 LOAD_CONST              16 (2)
+               176 LOAD_CONST              17 (('Chain',))
+               178 IMPORT_NAME             28 (chain)
+               180 IMPORT_FROM             29 (Chain)
+               182 STORE_NAME              29 (Chain)
+               184 POP_TOP
+   
+    23     >>  186 LOAD_CONST              18 ('0xcA11bde05977b3631167028862bE2a173976CA11')
+               188 STORE_NAME              30 (MULTICALL_V3_ADDRESS)
+   
+    26         190 LOAD_NAME                2 (dataclass)
+   
+    27         192 PUSH_NULL
+               194 LOAD_BUILD_CLASS
+               196 LOAD_CONST              19 (<code object MulticallResult, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 26>)
+               198 MAKE_FUNCTION            0
+               200 LOAD_CONST              20 ('MulticallResult')
+               202 PRECALL                  2
+               206 CALL                     2
+   
+    26         216 PRECALL                  0
+               220 CALL                     0
+   
+    27         230 STORE_NAME              31 (MulticallResult)
+   
+    32         232 LOAD_NAME                2 (dataclass)
+   
+    33         234 PUSH_NULL
+               236 LOAD_BUILD_CLASS
+               238 LOAD_CONST              21 (<code object MulticallDecodedResult, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 32>)
+               240 MAKE_FUNCTION            0
+               242 LOAD_CONST              22 ('MulticallDecodedResult')
+               244 PRECALL                  2
+               248 CALL                     2
+   
+    32         258 PRECALL                  0
+               262 CALL                     0
+   
+    33         272 STORE_NAME              32 (MulticallDecodedResult)
+   
+    38         274 PUSH_NULL
+               276 LOAD_BUILD_CLASS
+               278 LOAD_CONST              23 (<code object MulticallFailed, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 38>)
+               280 MAKE_FUNCTION            0
+               282 LOAD_CONST              24 ('MulticallFailed')
+               284 LOAD_NAME               33 (Exception)
+               286 PRECALL                  3
+               290 CALL                     3
+               300 STORE_NAME              34 (MulticallFailed)
+   
+    42         302 PUSH_NULL
+               304 LOAD_BUILD_CLASS
+               306 LOAD_CONST              25 (<code object Multicall, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 42>)
+               308 MAKE_FUNCTION            0
+               310 LOAD_CONST              26 ('Multicall')
+               312 LOAD_NAME               26 (Contract)
+               314 PRECALL                  3
+               318 CALL                     3
+               328 STORE_NAME              35 (Multicall)
+               330 LOAD_CONST               4 (None)
+               332 RETURN_VALUE
    consts
       'More about MulticallV3: https://github.com/mds1/multicall\n'
       0
       ('dataclass',)
-      ('Any', 'List', 'Optional', 'Sequence', 'Tuple')
+      ('Any', 'Sequence')
       None
       ('DecodingError',)
       ('BlockIdentifier', 'BlockNumber', 'ChecksumAddress')
       ('HexBytes',)
       ('map_abi_data',)
       ('BASE_RETURN_NORMALIZERS',)
       ('ContractFunction',)
       ('ContractLogicError',)
-      2
-      ('BatchCallFunctionFailed',)
       1
       ('MULTICALL_V3_ABI',)
       ('Contract',)
       ('TYPE_CHECKING',)
+      2
       ('Chain',)
       '0xcA11bde05977b3631167028862bE2a173976CA11'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
-            0x970065005a0164005a0255006503650464013c00000065056506190000
-            00000000000000650464023c00000064035300
-          27           0 RESUME                   0
+            0x970065005a0164005a0255006503650464013c000000650564027a0700
+            00650464033c00000064025300
+          26           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MulticallResult')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          29          12 LOAD_NAME                3 (bool)
+          28          12 LOAD_NAME                3 (bool)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('success')
                       18 STORE_SUBSCR
          
-          30          22 LOAD_NAME                5 (Optional)
-                      24 LOAD_NAME                6 (bytes)
-                      26 BINARY_SUBSCR
-                      36 LOAD_NAME                4 (__annotations__)
-                      38 LOAD_CONST               2 ('return_data')
-                      40 STORE_SUBSCR
-                      44 LOAD_CONST               3 (None)
-                      46 RETURN_VALUE
+          29          22 LOAD_NAME                5 (bytes)
+                      24 LOAD_CONST               2 (None)
+                      26 BINARY_OP                7 (|)
+                      30 LOAD_NAME                4 (__annotations__)
+                      32 LOAD_CONST               3 ('return_data')
+                      34 STORE_SUBSCR
+                      38 LOAD_CONST               2 (None)
+                      40 RETURN_VALUE
          consts
             'MulticallResult'
             'success'
-            'return_data'
             None
-         names      ('__name__', '__module__', '__qualname__', 'bool', '__annotations__', 'Optional', 'bytes')
+            'return_data'
+         names      ('__name__', '__module__', '__qualname__', 'bool', '__annotations__', 'bytes')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
          name       'MulticallResult'
-         firstlineno 27
+         firstlineno 26
          lnotab 0x0c020a01
       'MulticallResult'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
-            0x970065005a0164005a0255006503650464013c00000065056506190000
-            00000000000000650464023c00000064035300
-          33           0 RESUME                   0
+            0x970065005a0164005a0255006503650464013c000000650564027a0700
+            00650464033c00000064025300
+          32           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MulticallDecodedResult')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          35          12 LOAD_NAME                3 (bool)
+          34          12 LOAD_NAME                3 (bool)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('success')
                       18 STORE_SUBSCR
          
-          36          22 LOAD_NAME                5 (Optional)
-                      24 LOAD_NAME                6 (Any)
-                      26 BINARY_SUBSCR
-                      36 LOAD_NAME                4 (__annotations__)
-                      38 LOAD_CONST               2 ('return_data_decoded')
-                      40 STORE_SUBSCR
-                      44 LOAD_CONST               3 (None)
-                      46 RETURN_VALUE
+          35          22 LOAD_NAME                5 (Any)
+                      24 LOAD_CONST               2 (None)
+                      26 BINARY_OP                7 (|)
+                      30 LOAD_NAME                4 (__annotations__)
+                      32 LOAD_CONST               3 ('return_data_decoded')
+                      34 STORE_SUBSCR
+                      38 LOAD_CONST               2 (None)
+                      40 RETURN_VALUE
          consts
             'MulticallDecodedResult'
             'success'
-            'return_data_decoded'
             None
-         names      ('__name__', '__module__', '__qualname__', 'bool', '__annotations__', 'Optional', 'Any')
+            'return_data_decoded'
+         names      ('__name__', '__module__', '__qualname__', 'bool', '__annotations__', 'Any')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
          name       'MulticallDecodedResult'
-         firstlineno 33
+         firstlineno 32
          lnotab 0x0c020a01
       'MulticallDecodedResult'
       code
          argcount  : 0
          nlocals   : 0
+         stacksize : 1
+         flags     : 0
+         code 0x970065005a0164005a0264015300
+          38           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('MulticallFailed')
+                       8 STORE_NAME               2 (__qualname__)
+         
+          39          10 LOAD_CONST               1 (None)
+                      12 RETURN_VALUE
+         consts
+            'MulticallFailed'
+            None
+         names      ('__name__', '__module__', '__qualname__')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
+         name       'MulticallFailed'
+         firstlineno 38
+         lnotab 0x0a01
+      'MulticallFailed'
+      code
+         argcount  : 0
+         nlocals   : 0
          stacksize : 11
          flags     : 0
          code
-            0x8700970065005a0164005a020900090064156402640364046503650465
-            057a070000190000000000000000006604880066016405840d5a06650764
-            0665086509190000000000000000006407650a650b650a6504650c660219
-            00000000000000000019000000000000000000650b650b650d1900000000
-            000000000019000000000000000000660219000000000000000000660464
-            088404a6000000ab0000000000000000005a0e6507640965086505190000
-            00000000000000640a650c64076503650d19000000000000000000660664
-            0b8404a6000000ab0000000000000000005a0f09006416640d6508650a65
-            04650c66021900000000000000000019000000000000000000640e650365
-            10190000000000000000006407650a6511650b6503650d19000000000000
-            000000190000000000000000006602190000000000000000006606640f84
-            055a120900641664066508650919000000000000000000640e6503651019
-            00000000000000000064076513651165146503650d190000000000000000
-            00190000000000000000006602190000000000000000006606641084055a
-            15090009006417640d650865136504650c66021900000000000000000019
-            00000000000000000064126516640e650365101900000000000000000064
-            0765146517190000000000000000006608641384055a1809000900641764
-            06650865091900000000000000000064126516640e650365101900000000
-            0000000000640765146519190000000000000000006608641484055a1a88
-            0078015a1b5300
+            0x8700970065005a0164005a02090009006415640264036404650365047a
+            0700006604880066016405840d5a05650664066507650819000000000000
+            00000064076509650a65096503650b660219000000000000000000190000
+            00000000000000650a650a650c1900000000000000000019000000000000
+            000000660219000000000000000000660464088404a6000000ab00000000
+            00000000005a0d650664096507650419000000000000000000640a650b64
+            07650c64017a0700006606640b8404a6000000ab0000000000000000005a
+            0e09006416640d650765096503650b660219000000000000000000190000
+            00000000000000640e650f640765096510650a650c64017a070000190000
+            000000000000006602190000000000000000006606640f84055a11090064
+            1664066507650819000000000000000000640e650f640765096510650a65
+            0c64017a0700001900000000000000000066021900000000000000000066
+            06641084055a12090009006417640d650765096503650b66021900000000
+            00000000001900000000000000000064126513640e650f6407650a651419
+            0000000000000000006608641384055a1509000900641764066507650819
+            00000000000000000064126513640e650f6407650a651619000000000000
+            0000006608641484055a17880078015a185300
                        0 MAKE_CELL                0 (__class__)
          
-          39           2 RESUME                   0
+          42           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Multicall')
                       10 STORE_NAME               2 (__qualname__)
          
-          43          12 NOP
+          46          12 NOP
          
-          44          14 NOP
+          47          14 NOP
          
-          40          16 LOAD_CONST              21 ((None, None))
+          43          16 LOAD_CONST              21 ((None, None))
                       18 LOAD_CONST               2 ('chain')
          
-          42          20 LOAD_CONST               3 ('Chain')
+          45          20 LOAD_CONST               3 ('Chain')
          
-          40          22 LOAD_CONST               4 ('address')
+          43          22 LOAD_CONST               4 ('address')
          
-          43          24 LOAD_NAME                3 (Optional)
-                      26 LOAD_NAME                4 (ChecksumAddress)
-                      28 LOAD_NAME                5 (str)
-                      30 BINARY_OP                7 (|)
-                      34 BINARY_SUBSCR
-         
-          40          44 BUILD_TUPLE              4
-                      46 LOAD_CLOSURE             0 (__class__)
-                      48 BUILD_TUPLE              1
-                      50 LOAD_CONST               5 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 40>)
-                      52 MAKE_FUNCTION           13 (defaults, annotations, closure)
-                      54 STORE_NAME               6 (__init__)
-         
-          50          56 LOAD_NAME                7 (staticmethod)
-         
-          51          58 LOAD_CONST               6 ('contract_functions')
-         
-          52          60 LOAD_NAME                8 (Sequence)
-                      62 LOAD_NAME                9 (ContractFunction)
-                      64 BINARY_SUBSCR
-         
-          51          74 LOAD_CONST               7 ('return')
-         
-          53          76 LOAD_NAME               10 (tuple)
-                      78 LOAD_NAME               11 (list)
-                      80 LOAD_NAME               10 (tuple)
-                      82 LOAD_NAME                4 (ChecksumAddress)
-                      84 LOAD_NAME               12 (bytes)
-                      86 BUILD_TUPLE              2
-                      88 BINARY_SUBSCR
-                      98 BINARY_SUBSCR
-                     108 LOAD_NAME               11 (list)
-                     110 LOAD_NAME               11 (list)
-                     112 LOAD_NAME               13 (Any)
-                     114 BINARY_SUBSCR
+          46          24 LOAD_NAME                3 (ChecksumAddress)
+                      26 LOAD_NAME                4 (str)
+                      28 BINARY_OP                7 (|)
+         
+          43          32 BUILD_TUPLE              4
+                      34 LOAD_CLOSURE             0 (__class__)
+                      36 BUILD_TUPLE              1
+                      38 LOAD_CONST               5 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 43>)
+                      40 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                      42 STORE_NAME               5 (__init__)
+         
+          53          44 LOAD_NAME                6 (staticmethod)
+         
+          54          46 LOAD_CONST               6 ('contract_functions')
+         
+          55          48 LOAD_NAME                7 (Sequence)
+                      50 LOAD_NAME                8 (ContractFunction)
+                      52 BINARY_SUBSCR
+         
+          54          62 LOAD_CONST               7 ('return')
+         
+          56          64 LOAD_NAME                9 (tuple)
+                      66 LOAD_NAME               10 (list)
+                      68 LOAD_NAME                9 (tuple)
+                      70 LOAD_NAME                3 (ChecksumAddress)
+                      72 LOAD_NAME               11 (bytes)
+                      74 BUILD_TUPLE              2
+                      76 BINARY_SUBSCR
+                      86 BINARY_SUBSCR
+                      96 LOAD_NAME               10 (list)
+                      98 LOAD_NAME               10 (list)
+                     100 LOAD_NAME               12 (Any)
+                     102 BINARY_SUBSCR
+                     112 BINARY_SUBSCR
+                     122 BUILD_TUPLE              2
                      124 BINARY_SUBSCR
-                     134 BUILD_TUPLE              2
-                     136 BINARY_SUBSCR
          
-          51         146 BUILD_TUPLE              4
-                     148 LOAD_CONST               8 (<code object _build_payload, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 50>)
-                     150 MAKE_FUNCTION            4 (annotations)
-         
-          50         152 PRECALL                  0
-                     156 CALL                     0
-         
-          51         166 STORE_NAME              14 (_build_payload)
-         
-          69         168 LOAD_NAME                7 (staticmethod)
-         
-          70         170 LOAD_CONST               9 ('output_type')
-                     172 LOAD_NAME                8 (Sequence)
-                     174 LOAD_NAME                5 (str)
-                     176 BINARY_SUBSCR
-                     186 LOAD_CONST              10 ('data')
-                     188 LOAD_NAME               12 (bytes)
-                     190 LOAD_CONST               7 ('return')
-                     192 LOAD_NAME                3 (Optional)
-                     194 LOAD_NAME               13 (Any)
-                     196 BINARY_SUBSCR
-                     206 BUILD_TUPLE              6
-                     208 LOAD_CONST              11 (<code object _decode_data, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 69>)
-                     210 MAKE_FUNCTION            4 (annotations)
-         
-          69         212 PRECALL                  0
-                     216 CALL                     0
-         
-          70         226 STORE_NAME              15 (_decode_data)
-         
-          97         228 NOP
-         
-          94         230 LOAD_CONST              22 (('latest',))
-                     232 LOAD_CONST              13 ('targets_with_data')
-         
-          96         234 LOAD_NAME                8 (Sequence)
-                     236 LOAD_NAME               10 (tuple)
-                     238 LOAD_NAME                4 (ChecksumAddress)
-                     240 LOAD_NAME               12 (bytes)
-                     242 BUILD_TUPLE              2
-                     244 BINARY_SUBSCR
-                     254 BINARY_SUBSCR
-         
-          94         264 LOAD_CONST              14 ('block_identifier')
-         
-          97         266 LOAD_NAME                3 (Optional)
-                     268 LOAD_NAME               16 (BlockIdentifier)
-                     270 BINARY_SUBSCR
-         
-          94         280 LOAD_CONST               7 ('return')
-         
-          98         282 LOAD_NAME               10 (tuple)
-                     284 LOAD_NAME               17 (BlockNumber)
-                     286 LOAD_NAME               11 (list)
-                     288 LOAD_NAME                3 (Optional)
-                     290 LOAD_NAME               13 (Any)
-                     292 BINARY_SUBSCR
-                     302 BINARY_SUBSCR
-                     312 BUILD_TUPLE              2
-                     314 BINARY_SUBSCR
-         
-          94         324 BUILD_TUPLE              6
-                     326 LOAD_CONST              15 (<code object _aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 94>)
-                     328 MAKE_FUNCTION            5 (defaults, annotations)
-                     330 STORE_NAME              18 (_aggregate)
-         
-         119         332 NOP
-         
-         116         334 LOAD_CONST              22 (('latest',))
-                     336 LOAD_CONST               6 ('contract_functions')
-         
-         118         338 LOAD_NAME                8 (Sequence)
-                     340 LOAD_NAME                9 (ContractFunction)
-                     342 BINARY_SUBSCR
-         
-         116         352 LOAD_CONST              14 ('block_identifier')
-         
-         119         354 LOAD_NAME                3 (Optional)
-                     356 LOAD_NAME               16 (BlockIdentifier)
-                     358 BINARY_SUBSCR
-         
-         116         368 LOAD_CONST               7 ('return')
-         
-         120         370 LOAD_NAME               19 (Tuple)
-                     372 LOAD_NAME               17 (BlockNumber)
-                     374 LOAD_NAME               20 (List)
-                     376 LOAD_NAME                3 (Optional)
-                     378 LOAD_NAME               13 (Any)
-                     380 BINARY_SUBSCR
-                     390 BINARY_SUBSCR
-                     400 BUILD_TUPLE              2
-                     402 BINARY_SUBSCR
-         
-         116         412 BUILD_TUPLE              6
-                     414 LOAD_CONST              16 (<code object aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 116>)
-                     416 MAKE_FUNCTION            5 (defaults, annotations)
-                     418 STORE_NAME              21 (aggregate)
-         
-         142         420 NOP
-         
-         143         422 NOP
-         
-         139         424 LOAD_CONST              23 ((False, 'latest'))
-                     426 LOAD_CONST              13 ('targets_with_data')
-         
-         141         428 LOAD_NAME                8 (Sequence)
-                     430 LOAD_NAME               19 (Tuple)
-                     432 LOAD_NAME                4 (ChecksumAddress)
-                     434 LOAD_NAME               12 (bytes)
-                     436 BUILD_TUPLE              2
-                     438 BINARY_SUBSCR
-                     448 BINARY_SUBSCR
+          54         134 BUILD_TUPLE              4
+                     136 LOAD_CONST               8 (<code object _build_payload, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 53>)
+                     138 MAKE_FUNCTION            4 (annotations)
+         
+          53         140 PRECALL                  0
+                     144 CALL                     0
+         
+          54         154 STORE_NAME              13 (_build_payload)
+         
+          72         156 LOAD_NAME                6 (staticmethod)
+         
+          73         158 LOAD_CONST               9 ('output_type')
+                     160 LOAD_NAME                7 (Sequence)
+                     162 LOAD_NAME                4 (str)
+                     164 BINARY_SUBSCR
+                     174 LOAD_CONST              10 ('data')
+                     176 LOAD_NAME               11 (bytes)
+                     178 LOAD_CONST               7 ('return')
+                     180 LOAD_NAME               12 (Any)
+                     182 LOAD_CONST               1 (None)
+                     184 BINARY_OP                7 (|)
+                     188 BUILD_TUPLE              6
+                     190 LOAD_CONST              11 (<code object _decode_data, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 72>)
+                     192 MAKE_FUNCTION            4 (annotations)
          
-         139         458 LOAD_CONST              18 ('require_success')
+          72         194 PRECALL                  0
+                     198 CALL                     0
          
-         142         460 LOAD_NAME               22 (bool)
+          73         208 STORE_NAME              14 (_decode_data)
          
-         139         462 LOAD_CONST              14 ('block_identifier')
+         100         210 NOP
          
-         143         464 LOAD_NAME                3 (Optional)
-                     466 LOAD_NAME               16 (BlockIdentifier)
-                     468 BINARY_SUBSCR
+          97         212 LOAD_CONST              22 (('latest',))
+                     214 LOAD_CONST              13 ('targets_with_data')
          
-         139         478 LOAD_CONST               7 ('return')
+          99         216 LOAD_NAME                7 (Sequence)
+                     218 LOAD_NAME                9 (tuple)
+                     220 LOAD_NAME                3 (ChecksumAddress)
+                     222 LOAD_NAME               11 (bytes)
+                     224 BUILD_TUPLE              2
+                     226 BINARY_SUBSCR
+                     236 BINARY_SUBSCR
          
-         144         480 LOAD_NAME               20 (List)
-                     482 LOAD_NAME               23 (MulticallResult)
-                     484 BINARY_SUBSCR
+          97         246 LOAD_CONST              14 ('block_identifier')
          
-         139         494 BUILD_TUPLE              8
-                     496 LOAD_CONST              19 (<code object _try_aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 139>)
-                     498 MAKE_FUNCTION            5 (defaults, annotations)
-                     500 STORE_NAME              24 (_try_aggregate)
+         100         248 LOAD_NAME               15 (BlockIdentifier)
          
-         177         502 NOP
+          97         250 LOAD_CONST               7 ('return')
          
-         178         504 NOP
+         101         252 LOAD_NAME                9 (tuple)
+                     254 LOAD_NAME               16 (BlockNumber)
+                     256 LOAD_NAME               10 (list)
+                     258 LOAD_NAME               12 (Any)
+                     260 LOAD_CONST               1 (None)
+                     262 BINARY_OP                7 (|)
+                     266 BINARY_SUBSCR
+                     276 BUILD_TUPLE              2
+                     278 BINARY_SUBSCR
          
-         174         506 LOAD_CONST              23 ((False, 'latest'))
-                     508 LOAD_CONST               6 ('contract_functions')
+          97         288 BUILD_TUPLE              6
+                     290 LOAD_CONST              15 (<code object _aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 97>)
+                     292 MAKE_FUNCTION            5 (defaults, annotations)
+                     294 STORE_NAME              17 (_aggregate)
          
-         176         510 LOAD_NAME                8 (Sequence)
-                     512 LOAD_NAME                9 (ContractFunction)
-                     514 BINARY_SUBSCR
+         118         296 NOP
          
-         174         524 LOAD_CONST              18 ('require_success')
+         115         298 LOAD_CONST              22 (('latest',))
+                     300 LOAD_CONST               6 ('contract_functions')
          
-         177         526 LOAD_NAME               22 (bool)
+         117         302 LOAD_NAME                7 (Sequence)
+                     304 LOAD_NAME                8 (ContractFunction)
+                     306 BINARY_SUBSCR
          
-         174         528 LOAD_CONST              14 ('block_identifier')
+         115         316 LOAD_CONST              14 ('block_identifier')
          
-         178         530 LOAD_NAME                3 (Optional)
-                     532 LOAD_NAME               16 (BlockIdentifier)
-                     534 BINARY_SUBSCR
+         118         318 LOAD_NAME               15 (BlockIdentifier)
          
-         174         544 LOAD_CONST               7 ('return')
+         115         320 LOAD_CONST               7 ('return')
          
-         179         546 LOAD_NAME               20 (List)
-                     548 LOAD_NAME               25 (MulticallDecodedResult)
-                     550 BINARY_SUBSCR
+         119         322 LOAD_NAME                9 (tuple)
+                     324 LOAD_NAME               16 (BlockNumber)
+                     326 LOAD_NAME               10 (list)
+                     328 LOAD_NAME               12 (Any)
+                     330 LOAD_CONST               1 (None)
+                     332 BINARY_OP                7 (|)
+                     336 BINARY_SUBSCR
+                     346 BUILD_TUPLE              2
+                     348 BINARY_SUBSCR
          
-         174         560 BUILD_TUPLE              8
-                     562 LOAD_CONST              20 (<code object try_aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 174>)
-                     564 MAKE_FUNCTION            5 (defaults, annotations)
-                     566 STORE_NAME              26 (try_aggregate)
-                     568 LOAD_CLOSURE             0 (__class__)
-                     570 COPY                     1
-                     572 STORE_NAME              27 (__classcell__)
-                     574 RETURN_VALUE
+         115         358 BUILD_TUPLE              6
+                     360 LOAD_CONST              16 (<code object aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 115>)
+                     362 MAKE_FUNCTION            5 (defaults, annotations)
+                     364 STORE_NAME              18 (aggregate)
+         
+         133         366 NOP
+         
+         134         368 NOP
+         
+         130         370 LOAD_CONST              23 ((False, 'latest'))
+                     372 LOAD_CONST              13 ('targets_with_data')
+         
+         132         374 LOAD_NAME                7 (Sequence)
+                     376 LOAD_NAME                9 (tuple)
+                     378 LOAD_NAME                3 (ChecksumAddress)
+                     380 LOAD_NAME               11 (bytes)
+                     382 BUILD_TUPLE              2
+                     384 BINARY_SUBSCR
+                     394 BINARY_SUBSCR
+         
+         130         404 LOAD_CONST              18 ('require_success')
+         
+         133         406 LOAD_NAME               19 (bool)
+         
+         130         408 LOAD_CONST              14 ('block_identifier')
+         
+         134         410 LOAD_NAME               15 (BlockIdentifier)
+         
+         130         412 LOAD_CONST               7 ('return')
+         
+         135         414 LOAD_NAME               10 (list)
+                     416 LOAD_NAME               20 (MulticallResult)
+                     418 BINARY_SUBSCR
+         
+         130         428 BUILD_TUPLE              8
+                     430 LOAD_CONST              19 (<code object _try_aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 130>)
+                     432 MAKE_FUNCTION            5 (defaults, annotations)
+                     434 STORE_NAME              21 (_try_aggregate)
+         
+         159         436 NOP
+         
+         160         438 NOP
+         
+         156         440 LOAD_CONST              23 ((False, 'latest'))
+                     442 LOAD_CONST               6 ('contract_functions')
+         
+         158         444 LOAD_NAME                7 (Sequence)
+                     446 LOAD_NAME                8 (ContractFunction)
+                     448 BINARY_SUBSCR
+         
+         156         458 LOAD_CONST              18 ('require_success')
+         
+         159         460 LOAD_NAME               19 (bool)
+         
+         156         462 LOAD_CONST              14 ('block_identifier')
+         
+         160         464 LOAD_NAME               15 (BlockIdentifier)
+         
+         156         466 LOAD_CONST               7 ('return')
+         
+         161         468 LOAD_NAME               10 (list)
+                     470 LOAD_NAME               22 (MulticallDecodedResult)
+                     472 BINARY_SUBSCR
+         
+         156         482 BUILD_TUPLE              8
+                     484 LOAD_CONST              20 (<code object try_aggregate, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 156>)
+                     486 MAKE_FUNCTION            5 (defaults, annotations)
+                     488 STORE_NAME              23 (try_aggregate)
+                     490 LOAD_CLOSURE             0 (__class__)
+                     492 COPY                     1
+                     494 STORE_NAME              24 (__classcell__)
+                     496 RETURN_VALUE
          consts
             'Multicall'
             None
             'chain'
             'Chain'
             'address'
             code
@@ -558,27 +567,27 @@
                code
                   0x950197007c0270067400000000000000000000007d027c037006740200
                   0000000000000000007d03740500000000000000000000a6000000ab0000
                   00000000000000a00300000000000000000000000000000000000000007c
                   017c027c03a6030000ab030000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-                40           2 RESUME                   0
+                43           2 RESUME                   0
                
-                46           4 LOAD_FAST                2 (address)
+                49           4 LOAD_FAST                2 (address)
                              6 JUMP_IF_TRUE_OR_POP      6 (to 20)
                              8 LOAD_GLOBAL              0 (MULTICALL_V3_ADDRESS)
                        >>   20 STORE_FAST               2 (address)
                
-                47          22 LOAD_FAST                3 (abi)
+                50          22 LOAD_FAST                3 (abi)
                             24 JUMP_IF_TRUE_OR_POP      6 (to 38)
                             26 LOAD_GLOBAL              2 (MULTICALL_V3_ABI)
                        >>   38 STORE_FAST               3 (abi)
                
-                48          40 LOAD_GLOBAL              5 (NULL + super)
+                51          40 LOAD_GLOBAL              5 (NULL + super)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 LOAD_METHOD              3 (__init__)
                             88 LOAD_FAST                1 (chain)
                             90 LOAD_FAST                2 (address)
                             92 LOAD_FAST                3 (abi)
                             94 PRECALL                  3
@@ -590,15 +599,15 @@
                   None
                names      ('MULTICALL_V3_ADDRESS', 'MULTICALL_V3_ABI', 'super', '__init__')
                varnames   ('self', 'chain', 'address', 'abi')
                freevars   ('__class__',)
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       '__init__'
-               firstlineno 40
+               firstlineno 43
                lnotab 0x040612011201
             'contract_functions'
             'return'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 8
@@ -608,80 +617,80 @@
                   000000000000000000000000007c036a0100000000000000007405000000
                   000000000000007c03a00300000000000000000000000000000000000000
                   00a6000000ab000000000000000000a6010000ab01000000000000000066
                   02a6010000ab01000000000000000001007c02a000000000000000000000
                   0000000000000000000000640184007c036a040000000000000000640219
                   0000000000000000004400a6000000ab000000000000000000a6010000ab
                   01000000000000000001008c687c017c0266025300
-                50           0 RESUME                   0
+                53           0 RESUME                   0
                
-                54           2 BUILD_LIST               0
+                57           2 BUILD_LIST               0
                              4 STORE_FAST               1 (targets_with_data)
                
-                55           6 BUILD_LIST               0
+                58           6 BUILD_LIST               0
                              8 STORE_FAST               2 (output_types)
                
-                56          10 LOAD_FAST                0 (contract_functions)
+                59          10 LOAD_FAST                0 (contract_functions)
                             12 GET_ITER
                        >>   14 FOR_ITER               103 (to 222)
                             16 STORE_FAST               3 (contract_function)
                
-                57          18 LOAD_FAST                1 (targets_with_data)
+                60          18 LOAD_FAST                1 (targets_with_data)
                             20 LOAD_METHOD              0 (append)
                
-                59          42 LOAD_FAST                3 (contract_function)
+                62          42 LOAD_FAST                3 (contract_function)
                             44 LOAD_ATTR                1 (address)
                
-                60          54 LOAD_GLOBAL              5 (NULL + HexBytes)
+                63          54 LOAD_GLOBAL              5 (NULL + HexBytes)
                             66 LOAD_FAST                3 (contract_function)
                             68 LOAD_METHOD              3 (_encode_transaction_data)
                             90 PRECALL                  0
                             94 CALL                     0
                            104 PRECALL                  1
                            108 CALL                     1
                
-                58         118 BUILD_TUPLE              2
+                61         118 BUILD_TUPLE              2
                
-                57         120 PRECALL                  1
+                60         120 PRECALL                  1
                            124 CALL                     1
                            134 POP_TOP
                
-                63         136 LOAD_FAST                2 (output_types)
+                66         136 LOAD_FAST                2 (output_types)
                            138 LOAD_METHOD              0 (append)
                
-                64         160 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 64>)
+                67         160 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 67>)
                            162 MAKE_FUNCTION            0
                            164 LOAD_FAST                3 (contract_function)
                            166 LOAD_ATTR                4 (abi)
                            176 LOAD_CONST               2 ('outputs')
                            178 BINARY_SUBSCR
                            188 GET_ITER
                            190 PRECALL                  0
                            194 CALL                     0
                
-                63         204 PRECALL                  1
+                66         204 PRECALL                  1
                            208 CALL                     1
                            218 POP_TOP
                            220 JUMP_BACKWARD          104 (to 14)
                
-                67     >>  222 LOAD_FAST                1 (targets_with_data)
+                70     >>  222 LOAD_FAST                1 (targets_with_data)
                            224 LOAD_FAST                2 (output_types)
                            226 BUILD_TUPLE              2
                            228 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                         00
-                      64           0 RESUME                   0
+                      67           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                                    8 STORE_FAST               1 (output)
                                   10 LOAD_FAST                1 (output)
                                   12 LOAD_CONST               0 ('type')
                                   14 BINARY_SUBSCR
@@ -692,24 +701,24 @@
                         'type'
                      names      ()
                      varnames   ('.0', 'output')
                      freevars   ()
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                      name       '<listcomp>'
-                     firstlineno 64
+                     firstlineno 67
                      lnotab 0x
                   'outputs'
                names      ('append', 'address', 'HexBytes', '_encode_transaction_data', 'abi')
                varnames   ('contract_functions', 'targets_with_data', 'output_types', 'contract_function')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       '_build_payload'
-               firstlineno 50
+               firstlineno 53
                lnotab 0x020404010401080118020c0140fe02ff100618012cff1204
             'output_type'
             'data'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
@@ -719,82 +728,82 @@
                   007c007c01a6020000ab0200000000000000007d02740500000000000000
                   0000007406000000000000000000007c007c02a6030000ab030000000000
                   0000007d037409000000000000000000007c03a6010000ab010000000000
                   00000064016b020000000072087c0364021900000000000000000053007c
                   0353002300740a00000000000000000000240072160100740d0000000000
                   000000000064037c017c00a6030000ab03000000000000000001007c0163
                   0259005300770078035900770164045300
-                69           0 RESUME                   0
+                72           0 RESUME                   0
                
-                78           2 LOAD_FAST                1 (data)
+                81           2 LOAD_FAST                1 (data)
                              4 POP_JUMP_FORWARD_IF_FALSE   108 (to 222)
                
-                79           6 NOP
+                82           6 NOP
                
-                80           8 LOAD_GLOBAL              1 (NULL + eth_abi)
+                83           8 LOAD_GLOBAL              1 (NULL + eth_abi)
                             20 LOAD_ATTR                1 (decode)
                             30 LOAD_FAST                0 (output_type)
                             32 LOAD_FAST                1 (data)
                             34 PRECALL                  2
                             38 CALL                     2
                             48 STORE_FAST               2 (decoded_values)
                
-                81          50 LOAD_GLOBAL              5 (NULL + map_abi_data)
+                84          50 LOAD_GLOBAL              5 (NULL + map_abi_data)
                
-                82          62 LOAD_GLOBAL              6 (BASE_RETURN_NORMALIZERS)
+                85          62 LOAD_GLOBAL              6 (BASE_RETURN_NORMALIZERS)
                             74 LOAD_FAST                0 (output_type)
                             76 LOAD_FAST                2 (decoded_values)
                
-                81          78 PRECALL                  3
+                84          78 PRECALL                  3
                             82 CALL                     3
                             92 STORE_FAST               3 (normalized_data)
                
-                84          94 LOAD_GLOBAL              9 (NULL + len)
+                87          94 LOAD_GLOBAL              9 (NULL + len)
                            106 LOAD_FAST                3 (normalized_data)
                            108 PRECALL                  1
                            112 CALL                     1
                            122 LOAD_CONST               1 (1)
                            124 COMPARE_OP               2 (==)
                            130 POP_JUMP_FORWARD_IF_FALSE     8 (to 148)
                
-                85         132 LOAD_FAST                3 (normalized_data)
+                88         132 LOAD_FAST                3 (normalized_data)
                            134 LOAD_CONST               2 (0)
                            136 BINARY_SUBSCR
                            146 RETURN_VALUE
                
-                87     >>  148 LOAD_FAST                3 (normalized_data)
+                90     >>  148 LOAD_FAST                3 (normalized_data)
                            150 RETURN_VALUE
                        >>  152 PUSH_EXC_INFO
                
-                88         154 LOAD_GLOBAL             10 (DecodingError)
+                91         154 LOAD_GLOBAL             10 (DecodingError)
                            166 CHECK_EXC_MATCH
                            168 POP_JUMP_FORWARD_IF_FALSE    22 (to 214)
                            170 POP_TOP
                
-                89         172 LOAD_GLOBAL             13 (NULL + print)
+                92         172 LOAD_GLOBAL             13 (NULL + print)
                
-                90         184 LOAD_CONST               3 ('Cannot decode %s using output-type %s')
+                93         184 LOAD_CONST               3 ('Cannot decode %s using output-type %s')
                            186 LOAD_FAST                1 (data)
                            188 LOAD_FAST                0 (output_type)
                
-                89         190 PRECALL                  3
+                92         190 PRECALL                  3
                            194 CALL                     3
                            204 POP_TOP
                
-                92         206 LOAD_FAST                1 (data)
+                95         206 LOAD_FAST                1 (data)
                            208 SWAP                     2
                            210 POP_EXCEPT
                            212 RETURN_VALUE
                
-                88     >>  214 RERAISE                  0
+                91     >>  214 RERAISE                  0
                        >>  216 COPY                     3
                            218 POP_EXCEPT
                            220 RERAISE                  1
                
-                78     >>  222 LOAD_CONST               4 (None)
+                81     >>  222 LOAD_CONST               4 (None)
                            224 RETURN_VALUE
                ExceptionTable:
                  8 to 144 -> 152 [0]
                  148 to 148 -> 152 [0]
                  152 to 208 -> 216 [1] lasti
                  214 to 214 -> 216 [1] lasti
                consts
@@ -805,15 +814,15 @@
                   None
                names      ('eth_abi', 'decode', 'map_abi_data', 'BASE_RETURN_NORMALIZERS', 'len', 'DecodingError', 'print')
                varnames   ('output_type', 'data', 'decoded_values', 'normalized_data')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       '_decode_data'
-               firstlineno 69
+               firstlineno 72
                lnotab
                   0x0209040102012a010c0110ff100326011002060112010c0106ff100308
                   fc08f6
             'latest'
             'targets_with_data'
             'block_identifier'
             code
@@ -825,215 +834,215 @@
                   0x9700640184007c014400a6000000ab0000000000000000007d0309007c
                   006a0000000000000000006a010000000000000000a00200000000000000
                   000000000000000000000000007c03a6010000ab010000000000000000a0
                   0300000000000000000000000000000000000000007c02ac02a6010000ab
                   01000000000000000053002300740800000000000000000000740a000000
                   000000000000006602240072080100740c00000000000000000000820177
                   00780359007701
-                94           0 RESUME                   0
+                97           0 RESUME                   0
                
-               106           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 106>)
+               105           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 105>)
                              4 MAKE_FUNCTION            0
                
-               107           6 LOAD_FAST                1 (targets_with_data)
+               106           6 LOAD_FAST                1 (targets_with_data)
                
-               106           8 GET_ITER
+               105           8 GET_ITER
                             10 PRECALL                  0
                             14 CALL                     0
                             24 STORE_FAST               3 (aggregate_parameter)
                
-               109          26 NOP
+               108          26 NOP
                
-               110          28 LOAD_FAST                0 (self)
+               109          28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                0 (contract)
                             40 LOAD_ATTR                1 (functions)
                             50 LOAD_METHOD              2 (aggregate)
                             72 LOAD_FAST                3 (aggregate_parameter)
                             74 PRECALL                  1
                             78 CALL                     1
                             88 LOAD_METHOD              3 (call)
                
-               111         110 LOAD_FAST                2 (block_identifier)
+               110         110 LOAD_FAST                2 (block_identifier)
                
-               110         112 KW_NAMES                 2
+               109         112 KW_NAMES                 2
                            114 PRECALL                  1
                            118 CALL                     1
                            128 RETURN_VALUE
                        >>  130 PUSH_EXC_INFO
                
-               113         132 LOAD_GLOBAL              8 (ContractLogicError)
+               112         132 LOAD_GLOBAL              8 (ContractLogicError)
                            144 LOAD_GLOBAL             10 (OverflowError)
                            156 BUILD_TUPLE              2
                            158 CHECK_EXC_MATCH
                            160 POP_JUMP_FORWARD_IF_FALSE     8 (to 178)
                            162 POP_TOP
                
-               114         164 LOAD_GLOBAL             12 (BatchCallFunctionFailed)
+               113         164 LOAD_GLOBAL             12 (MulticallFailed)
                            176 RAISE_VARARGS            1
                
-               113     >>  178 RERAISE                  0
+               112     >>  178 RERAISE                  0
                        >>  180 COPY                     3
                            182 POP_EXCEPT
                            184 RERAISE                  1
                ExceptionTable:
                  28 to 126 -> 130 [0]
                  130 to 178 -> 180 [1] lasti
                consts
-                  '\n\n        :param targets_with_data: List of target `addresses` and `data` to be called in each Contract\n        :param block_identifier:\n        :return:\n        :raises: BatchCallFunctionFailed\n        '
+                  '\n        :param targets_with_data: List of target `addresses` and `data` to be called in each Contract\n        '
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d0a5c0200007d017d027c017c0264009c0291028c0b53
                         00
-                     106           0 RESUME                   0
+                     105           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                      
-                     107           8 UNPACK_SEQUENCE          2
+                     106           8 UNPACK_SEQUENCE          2
                                   12 STORE_FAST               1 (target)
                                   14 STORE_FAST               2 (data)
                                   16 LOAD_FAST                1 (target)
                                   18 LOAD_FAST                2 (data)
                                   20 LOAD_CONST               0 (('target', 'callData'))
                                   22 BUILD_CONST_KEY_MAP      2
                      
-                     106          24 LIST_APPEND              2
+                     105          24 LIST_APPEND              2
                                   26 JUMP_BACKWARD           11 (to 6)
                              >>   28 RETURN_VALUE
                      consts
                         ('target', 'callData')
                      names      ()
                      varnames   ('.0', 'target', 'data')
                      freevars   ()
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                      name       '<listcomp>'
-                     firstlineno 106
+                     firstlineno 105
                      lnotab 0x080110ff
                   ('block_identifier',)
-               names      ('contract', 'functions', 'aggregate', 'call', 'ContractLogicError', 'OverflowError', 'BatchCallFunctionFailed')
+               names      ('contract', 'functions', 'aggregate', 'call', 'ContractLogicError', 'OverflowError', 'MulticallFailed')
                varnames   ('self', 'targets_with_data', 'block_identifier', 'aggregate_parameter')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       '_aggregate'
-               firstlineno 94
-               lnotab 0x020c040102ff12030201520102ff140320010eff
+               firstlineno 97
+               lnotab 0x0208040102ff12030201520102ff140320010eff
             code
                argcount  : 3
                nlocals   : 8
                stacksize : 5
                flags     : 3
                code
                   0x870097008900a00000000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000005c0200007d037d048900a001000000
                   00000000000000000000000000000000007c037c02ac01a6020000ab0200
                   000000000000005c0200007d057d06880066016402840874050000000000
                   00000000007c047c06a6020000ab0200000000000000004400a6000000ab
                   0000000000000000007d077c057c0766025300
                              0 MAKE_CELL                0 (self)
                
-               116           2 RESUME                   0
+               115           2 RESUME                   0
                
-               129           4 LOAD_DEREF               0 (self)
+               120           4 LOAD_DEREF               0 (self)
                              6 LOAD_METHOD              0 (_build_payload)
                             28 LOAD_FAST                1 (contract_functions)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               3 (targets_with_data)
                             50 STORE_FAST               4 (output_types)
                
-               130          52 LOAD_DEREF               0 (self)
+               121          52 LOAD_DEREF               0 (self)
                             54 LOAD_METHOD              1 (_aggregate)
                
-               131          76 LOAD_FAST                3 (targets_with_data)
+               122          76 LOAD_FAST                3 (targets_with_data)
                             78 LOAD_FAST                2 (block_identifier)
                
-               130          80 KW_NAMES                 1
+               121          80 KW_NAMES                 1
                             82 PRECALL                  2
                             86 CALL                     2
                             96 UNPACK_SEQUENCE          2
                            100 STORE_FAST               5 (block_number)
                            102 STORE_FAST               6 (results)
                
-               133         104 LOAD_CLOSURE             0 (self)
+               124         104 LOAD_CLOSURE             0 (self)
                            106 BUILD_TUPLE              1
-                           108 LOAD_CONST               2 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 133>)
+                           108 LOAD_CONST               2 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 124>)
                            110 MAKE_FUNCTION            8 (closure)
                
-               135         112 LOAD_GLOBAL              5 (NULL + zip)
+               126         112 LOAD_GLOBAL              5 (NULL + zip)
                            124 LOAD_FAST                4 (output_types)
                            126 LOAD_FAST                6 (results)
                            128 PRECALL                  2
                            132 CALL                     2
                
-               133         142 GET_ITER
+               124         142 GET_ITER
                            144 PRECALL                  0
                            148 CALL                     0
                            158 STORE_FAST               7 (decoded_results)
                
-               137         160 LOAD_FAST                5 (block_number)
+               128         160 LOAD_FAST                5 (block_number)
                            162 LOAD_FAST                7 (decoded_results)
                            164 BUILD_TUPLE              2
                            166 RETURN_VALUE
                consts
-                  "\n        Calls aggregate on MakerDAO's Multicall contract. If a function called raises an error execution is stopped\n\n        :param contract_functions:\n        :param block_identifier:\n        :return: A tuple with the ``blockNumber`` and a list with the decoded return values\n        :raises: BatchCallFunctionFailed\n        "
+                  None
                   ('block_identifier',)
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 6
                      flags     : 19
                      code
                         0x9501970067007c005d1b5c0200007d017d028903a00000000000000000
                         000000000000000000000000007c017c02a6020000ab0200000000000000
                         0091028c1c5300
                                    0 COPY_FREE_VARS           1
                      
-                     133           2 RESUME                   0
+                     124           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                27 (to 64)
                      
-                     135          10 UNPACK_SEQUENCE          2
+                     126          10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (output_type)
                                   16 STORE_FAST               2 (data)
                      
-                     134          18 LOAD_DEREF               3 (self)
+                     125          18 LOAD_DEREF               3 (self)
                                   20 LOAD_METHOD              0 (_decode_data)
                                   42 LOAD_FAST                1 (output_type)
                                   44 LOAD_FAST                2 (data)
                                   46 PRECALL                  2
                                   50 CALL                     2
                      
-                     133          60 LIST_APPEND              2
+                     124          60 LIST_APPEND              2
                                   62 JUMP_BACKWARD           28 (to 8)
                              >>   64 RETURN_VALUE
                      consts
                      names      ('_decode_data',)
                      varnames   ('.0', 'output_type', 'data')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                      name       '<listcomp>'
-                     firstlineno 133
+                     firstlineno 124
                      lnotab 0x0a0208ff2aff
                names      ('_build_payload', '_aggregate', 'zip')
                varnames   ('self', 'contract_functions', 'block_identifier', 'targets_with_data', 'output_types', 'block_number', 'results', 'decoded_results')
                freevars   ()
                cellvars   ('self',)
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       'aggregate'
-               firstlineno 116
-               lnotab 0x040d3001180104ff180308021efe1204
+               firstlineno 115
+               lnotab 0x04053001180104ff180308021efe1204
             False
             'require_success'
             code
                argcount  : 4
                nlocals   : 6
                stacksize : 5
                flags     : 3
@@ -1043,137 +1052,137 @@
                   0000007c027c04a6020000ab020000000000000000a00200000000000000
                   000000000000000000000000007c03ac02a6010000ab0100000000000000
                   007d057c0272156403640484007c054400a6000000ab0000000000000000
                   00760072077406000000000000000000008201640584007c054400a60000
                   00ab00000000000000000053002300740800000000000000000000740a00
                   000000000000000000740c00000000000000000000660324007208010074
                   060000000000000000000082017700780359007701
-               139           0 RESUME                   0
+               130           0 RESUME                   0
                
-               155           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 155>)
+               136           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 136>)
                              4 MAKE_FUNCTION            0
                
-               156           6 LOAD_FAST                1 (targets_with_data)
+               137           6 LOAD_FAST                1 (targets_with_data)
                
-               155           8 GET_ITER
+               136           8 GET_ITER
                             10 PRECALL                  0
                             14 CALL                     0
                             24 STORE_FAST               4 (aggregate_parameter)
                
-               158          26 NOP
+               140          26 NOP
                
-               159          28 LOAD_FAST                0 (self)
+               141          28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                0 (functions)
                             40 LOAD_METHOD              1 (tryAggregate)
                
-               160          62 LOAD_FAST                2 (require_success)
+               142          62 LOAD_FAST                2 (require_success)
                             64 LOAD_FAST                4 (aggregate_parameter)
                
-               159          66 PRECALL                  2
+               141          66 PRECALL                  2
                             70 CALL                     2
                
-               161          80 LOAD_METHOD              2 (call)
+               143          80 LOAD_METHOD              2 (call)
                            102 LOAD_FAST                3 (block_identifier)
                            104 KW_NAMES                 2
                            106 PRECALL                  1
                            110 CALL                     1
                
-               159         120 STORE_FAST               5 (result)
+               141         120 STORE_FAST               5 (result)
                
-               163         122 LOAD_FAST                2 (require_success)
+               145         122 LOAD_FAST                2 (require_success)
                            124 POP_JUMP_FORWARD_IF_FALSE    21 (to 168)
                            126 LOAD_CONST               3 (b'')
-                           128 LOAD_CONST               4 (<code object <genexpr>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 163>)
+                           128 LOAD_CONST               4 (<code object <genexpr>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 145>)
                            130 MAKE_FUNCTION            0
                            132 LOAD_FAST                5 (result)
                            134 GET_ITER
                            136 PRECALL                  0
                            140 CALL                     0
                            150 CONTAINS_OP              0
                            152 POP_JUMP_FORWARD_IF_FALSE     7 (to 168)
                
-               165         154 LOAD_GLOBAL              6 (BatchCallFunctionFailed)
+               147         154 LOAD_GLOBAL              6 (MulticallFailed)
                            166 RAISE_VARARGS            1
                
-               167     >>  168 LOAD_CONST               5 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 167>)
+               149     >>  168 LOAD_CONST               5 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 149>)
                            170 MAKE_FUNCTION            0
                
-               169         172 LOAD_FAST                5 (result)
+               151         172 LOAD_FAST                5 (result)
                
-               167         174 GET_ITER
+               149         174 GET_ITER
                            176 PRECALL                  0
                            180 CALL                     0
                            190 RETURN_VALUE
                        >>  192 PUSH_EXC_INFO
                
-               171         194 LOAD_GLOBAL              8 (ContractLogicError)
+               153         194 LOAD_GLOBAL              8 (ContractLogicError)
                            206 LOAD_GLOBAL             10 (OverflowError)
                            218 LOAD_GLOBAL             12 (ValueError)
                            230 BUILD_TUPLE              3
                            232 CHECK_EXC_MATCH
                            234 POP_JUMP_FORWARD_IF_FALSE     8 (to 252)
                            236 POP_TOP
                
-               172         238 LOAD_GLOBAL              6 (BatchCallFunctionFailed)
+               154         238 LOAD_GLOBAL              6 (MulticallFailed)
                            250 RAISE_VARARGS            1
                
-               171     >>  252 RERAISE                  0
+               153     >>  252 RERAISE                  0
                        >>  254 COPY                     3
                            256 POP_EXCEPT
                            258 RERAISE                  1
                ExceptionTable:
                  28 to 188 -> 192 [0]
                  192 to 252 -> 254 [1] lasti
                consts
-                  "\n        Calls ``try_aggregate`` on MakerDAO's Multicall contract.\n\n        :param targets_with_data:\n        :param require_success: If ``True``, an exception in any of the functions will stop the execution. Also, an\n            invalid decoded value will stop the execution\n        :param block_identifier:\n        :return: A list with the decoded return values\n        "
+                  None
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d0a5c0200007d017d027c017c0264009c0291028c0b53
                         00
-                     155           0 RESUME                   0
+                     136           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                      
-                     156           8 UNPACK_SEQUENCE          2
+                     137           8 UNPACK_SEQUENCE          2
                                   12 STORE_FAST               1 (target)
                                   14 STORE_FAST               2 (data)
                                   16 LOAD_FAST                1 (target)
                                   18 LOAD_FAST                2 (data)
                                   20 LOAD_CONST               0 (('target', 'callData'))
                                   22 BUILD_CONST_KEY_MAP      2
                      
-                     155          24 LIST_APPEND              2
+                     136          24 LIST_APPEND              2
                                   26 JUMP_BACKWARD           11 (to 6)
                              >>   28 RETURN_VALUE
                      consts
                         ('target', 'callData')
                      names      ()
                      varnames   ('.0', 'target', 'data')
                      freevars   ()
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                      name       '<listcomp>'
-                     firstlineno 155
+                     firstlineno 136
                      lnotab 0x080110ff
                   ('block_identifier',)
                   b''
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 3
                      flags     : 51
                      code
                         0x4b00010097007c005d095c0200007d017d027c025600970101008c0a64
                         005300
-                     163           0 RETURN_GENERATOR
+                     145           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                 9 (to 28)
                                   10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (_)
                                   16 STORE_FAST               2 (data)
@@ -1188,66 +1197,66 @@
                         None
                      names      ()
                      varnames   ('.0', '_', 'data')
                      freevars   ()
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                      name       '<genexpr>'
-                     firstlineno 163
+                     firstlineno 145
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 6
                      flags     : 19
                      code
                         0x970067007c005d195c0200007d017d027401000000000000000000007c
                         017c0272027c026e016400a6020000ab02000000000000000091028c1a53
                         00
-                     167           0 RESUME                   0
+                     149           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                25 (to 58)
                      
-                     169           8 UNPACK_SEQUENCE          2
+                     151           8 UNPACK_SEQUENCE          2
                                   12 STORE_FAST               1 (success)
                                   14 STORE_FAST               2 (data)
                      
-                     168          16 LOAD_GLOBAL              1 (NULL + MulticallResult)
+                     150          16 LOAD_GLOBAL              1 (NULL + MulticallResult)
                                   28 LOAD_FAST                1 (success)
                                   30 LOAD_FAST                2 (data)
                                   32 POP_JUMP_FORWARD_IF_FALSE     2 (to 38)
                                   34 LOAD_FAST                2 (data)
                                   36 JUMP_FORWARD             1 (to 40)
                              >>   38 LOAD_CONST               0 (None)
                              >>   40 PRECALL                  2
                                   44 CALL                     2
                      
-                     167          54 LIST_APPEND              2
+                     149          54 LIST_APPEND              2
                                   56 JUMP_BACKWARD           26 (to 6)
                              >>   58 RETURN_VALUE
                      consts
                         None
                      names      ('MulticallResult',)
                      varnames   ('.0', 'success', 'data')
                      freevars   ()
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                      name       '<listcomp>'
-                     firstlineno 167
+                     firstlineno 149
                      lnotab 0x080208ff26ff
-               names      ('functions', 'tryAggregate', 'call', 'BatchCallFunctionFailed', 'ContractLogicError', 'OverflowError', 'ValueError')
+               names      ('functions', 'tryAggregate', 'call', 'MulticallFailed', 'ContractLogicError', 'OverflowError', 'ValueError')
                varnames   ('self', 'targets_with_data', 'require_success', 'block_identifier', 'aggregate_parameter', 'result')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       '_try_aggregate'
-               firstlineno 139
+               firstlineno 130
                lnotab
-                  0x0210040102ff12030201220104ff0e0228fe020420020e02040202fe14
+                  0x0206040102ff12040201220104ff0e0228fe020420020e02040202fe14
                   042c010eff
             code
                argcount  : 4
                nlocals   : 7
                stacksize : 5
                flags     : 3
                code
@@ -1255,142 +1264,142 @@
                   01a6010000ab0100000000000000005c0200007d047d058900a001000000
                   00000000000000000000000000000000007c047c027c03ac01a6030000ab
                   0300000000000000007d0688006601640284087405000000000000000000
                   007c057c06a6020000ab0200000000000000004400a6000000ab00000000
                   00000000005300
                              0 MAKE_CELL                0 (self)
                
-               174           2 RESUME                   0
+               156           2 RESUME                   0
                
-               188           4 LOAD_DEREF               0 (self)
+               167           4 LOAD_DEREF               0 (self)
                              6 LOAD_METHOD              0 (_build_payload)
                             28 LOAD_FAST                1 (contract_functions)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (targets_with_data)
                             50 STORE_FAST               5 (output_types)
                
-               189          52 LOAD_DEREF               0 (self)
+               168          52 LOAD_DEREF               0 (self)
                             54 LOAD_METHOD              1 (_try_aggregate)
                
-               190          76 LOAD_FAST                4 (targets_with_data)
+               169          76 LOAD_FAST                4 (targets_with_data)
                
-               191          78 LOAD_FAST                2 (require_success)
+               170          78 LOAD_FAST                2 (require_success)
                
-               192          80 LOAD_FAST                3 (block_identifier)
+               171          80 LOAD_FAST                3 (block_identifier)
                
-               189          82 KW_NAMES                 1
+               168          82 KW_NAMES                 1
                             84 PRECALL                  3
                             88 CALL                     3
                             98 STORE_FAST               6 (results)
                
-               194         100 LOAD_CLOSURE             0 (self)
+               173         100 LOAD_CLOSURE             0 (self)
                            102 BUILD_TUPLE              1
-                           104 LOAD_CONST               2 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 194>)
+                           104 LOAD_CONST               2 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\multicall.py", line 173>)
                            106 MAKE_FUNCTION            8 (closure)
                
-               201         108 LOAD_GLOBAL              5 (NULL + zip)
+               180         108 LOAD_GLOBAL              5 (NULL + zip)
                            120 LOAD_FAST                5 (output_types)
                            122 LOAD_FAST                6 (results)
                            124 PRECALL                  2
                            128 CALL                     2
                
-               194         138 GET_ITER
+               173         138 GET_ITER
                            140 PRECALL                  0
                            144 CALL                     0
                            154 RETURN_VALUE
                consts
-                  "\n        Calls ``try_aggregate`` on MakerDAO's Multicall contract.\n\n        :param contract_functions:\n        :param require_success: If ``True``, an exception in any of the functions will stop the execution\n        :param block_identifier:\n        :return: A list with the decoded return values\n        "
+                  "\n        Calls ``try_aggregate`` on MakerDAO's Multicall contract.\n\n        :param require_success: If ``True``, an exception in any of the functions will stop the execution\n        "
                   ('require_success', 'block_identifier')
                   code
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 9
                      flags     : 19
                      code
                         0x9501970067007c005d415c0200007d017d027401000000000000000000
                         007c026a0100000000000000007c026a010000000000000000721b8903a0
                         0200000000000000000000000000000000000000007c017c026a03000000
                         0000000000a6020000ab0200000000000000006e067c026a030000000000
                         000000a6020000ab02000000000000000091028c425300
                                    0 COPY_FREE_VARS           1
                      
-                     194           2 RESUME                   0
+                     173           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                65 (to 140)
                      
-                     201          10 UNPACK_SEQUENCE          2
+                     180          10 UNPACK_SEQUENCE          2
                                   14 STORE_FAST               1 (output_type)
                                   16 STORE_FAST               2 (multicall_result)
                      
-                     195          18 LOAD_GLOBAL              1 (NULL + MulticallDecodedResult)
+                     174          18 LOAD_GLOBAL              1 (NULL + MulticallDecodedResult)
                      
-                     196          30 LOAD_FAST                2 (multicall_result)
+                     175          30 LOAD_FAST                2 (multicall_result)
                                   32 LOAD_ATTR                1 (success)
                      
-                     198          42 LOAD_FAST                2 (multicall_result)
+                     177          42 LOAD_FAST                2 (multicall_result)
                                   44 LOAD_ATTR                1 (success)
                      
-                     197          54 POP_JUMP_FORWARD_IF_FALSE    27 (to 110)
+                     176          54 POP_JUMP_FORWARD_IF_FALSE    27 (to 110)
                                   56 LOAD_DEREF               3 (self)
                                   58 LOAD_METHOD              2 (_decode_data)
                                   80 LOAD_FAST                1 (output_type)
                                   82 LOAD_FAST                2 (multicall_result)
                                   84 LOAD_ATTR                3 (return_data)
                                   94 PRECALL                  2
                                   98 CALL                     2
                                  108 JUMP_FORWARD             6 (to 122)
                      
-                     199     >>  110 LOAD_FAST                2 (multicall_result)
+                     178     >>  110 LOAD_FAST                2 (multicall_result)
                                  112 LOAD_ATTR                3 (return_data)
                      
-                     195     >>  122 PRECALL                  2
+                     174     >>  122 PRECALL                  2
                                  126 CALL                     2
                      
-                     194         136 LIST_APPEND              2
+                     173         136 LIST_APPEND              2
                                  138 JUMP_BACKWARD           66 (to 8)
                              >>  140 RETURN_VALUE
                      consts
                      names      ('MulticallDecodedResult', 'success', '_decode_data', 'return_data')
                      varnames   ('.0', 'output_type', 'multicall_result')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                      name       '<listcomp>'
-                     firstlineno 194
+                     firstlineno 173
                      lnotab 0x0a0708fa0c010c020cff38020cfc0eff
                names      ('_build_payload', '_try_aggregate', 'zip')
                varnames   ('self', 'contract_functions', 'require_success', 'block_identifier', 'targets_with_data', 'output_types', 'results')
                freevars   ()
                cellvars   ('self',)
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
                name       'try_aggregate'
-               firstlineno 174
-               lnotab 0x040e300118010201020102fd120508071ef9
+               firstlineno 156
+               lnotab 0x040b300118010201020102fd120508071ef9
             (None, None)
             ('latest',)
             (False, 'latest')
-         names      ('__name__', '__module__', '__qualname__', 'Optional', 'ChecksumAddress', 'str', '__init__', 'staticmethod', 'Sequence', 'ContractFunction', 'tuple', 'list', 'bytes', 'Any', '_build_payload', '_decode_data', 'BlockIdentifier', 'BlockNumber', '_aggregate', 'Tuple', 'List', 'aggregate', 'bool', 'MulticallResult', '_try_aggregate', 'MulticallDecodedResult', 'try_aggregate', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'staticmethod', 'Sequence', 'ContractFunction', 'tuple', 'list', 'bytes', 'Any', '_build_payload', '_decode_data', 'BlockIdentifier', 'BlockNumber', '_aggregate', 'aggregate', 'bool', 'MulticallResult', '_try_aggregate', 'MulticallDecodedResult', 'try_aggregate', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
          name       'Multicall'
-         firstlineno 39
+         firstlineno 42
          lnotab
-            0x0c04020102fc040202fe020314fd0c0a020102010eff020246fe06ff0e
-            01021202012aff0e01021b02fd04021efe02030efd02042afc081902fd04
-            020efe02030efd02042afc081a020102fc04021efe020302fd02040efc02
-            050efb0826020102fc04020efe020302fd02040efc02050efb
+            0x0c04020102fc040202fe020308fd0c0a020102010eff020246fe06ff0e
+            010212020124ff0e01021b02fd04021efe020302fd020424fc081502fd04
+            020efe020302fd020424fc0812020102fc04021efe020302fd020402fc02
+            050efb081d020102fc04020efe020302fd020402fc02050efb
       'Multicall'
-   names      ('__doc__', 'dataclasses', 'dataclass', 'typing', 'Any', 'List', 'Optional', 'Sequence', 'Tuple', 'eth_abi', 'eth_abi.exceptions', 'DecodingError', 'eth_typing', 'BlockIdentifier', 'BlockNumber', 'ChecksumAddress', 'hexbytes', 'HexBytes', 'web3._utils.abi', 'map_abi_data', 'web3._utils.normalizers', 'BASE_RETURN_NORMALIZERS', 'web3.contract.contract', 'ContractFunction', 'web3.exceptions', 'ContractLogicError', 'exceptions', 'BatchCallFunctionFailed', 'abi', 'MULTICALL_V3_ABI', 'contract', 'Contract', 'TYPE_CHECKING', 'chain', 'Chain', 'MULTICALL_V3_ADDRESS', 'MulticallResult', 'MulticallDecodedResult', 'Multicall')
+   names      ('__doc__', 'dataclasses', 'dataclass', 'typing', 'Any', 'Sequence', 'eth_abi', 'eth_abi.exceptions', 'DecodingError', 'eth_typing', 'BlockIdentifier', 'BlockNumber', 'ChecksumAddress', 'hexbytes', 'HexBytes', 'web3._utils.abi', 'map_abi_data', 'web3._utils.normalizers', 'BASE_RETURN_NORMALIZERS', 'web3.contract.contract', 'ContractFunction', 'web3.exceptions', 'ContractLogicError', 'abi', 'MULTICALL_V3_ABI', 'contract', 'Contract', 'TYPE_CHECKING', 'chain', 'Chain', 'MULTICALL_V3_ADDRESS', 'MulticallResult', 'MulticallDecodedResult', 'Exception', 'MulticallFailed', 'Multicall')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\multicall.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104020c011c0208010c0114010c010c010c010c010c020c010c
-      010c020c0104010c030403020118ff0e010205020118ff0e010205
+      0x00ff020104020c01100208010c0114010c010c010c010c010c020c010c
+      020c0104010c030403020118ff0e010205020118ff0e0102051c04
```

### Comparing `better_web3-1.0.0/better_web3/contract/abi/erc1155.json` & `better_web3-1.1.0/better_web3/contract/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.0.0/better_web3/contract/abi/erc20.json` & `better_web3-1.1.0/better_web3/contract/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.0.0/better_web3/contract/abi/erc721.json` & `better_web3-1.1.0/better_web3/contract/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.0.0/better_web3/contract/abi/multicall_v3.json` & `better_web3-1.1.0/better_web3/contract/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.0.0/better_web3/contract/contract.py` & `better_web3-1.1.0/better_web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.0.0/better_web3/contract/erc721.py` & `better_web3-1.1.0/better_web3/contract/erc721.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,90 @@
-from typing import TYPE_CHECKING, cast, Iterable
+from typing import TYPE_CHECKING, Iterable
 
-from eth_abi.exceptions import DecodingError
 from eth_typing import ChecksumAddress, BlockIdentifier
 from eth_utils import to_checksum_address
 
 from .abi import ERC721_ABI
 from .contract import Contract
-from .exceptions import InvalidERC721Info
-from .model import Erc721Info
+from ..utils import cache
 
 if TYPE_CHECKING:
     from ..chain import Chain
 
 
 class ERC721(Contract):
-    """
-    Реализация ERC721 контракта
-    """
-
     def __init__(
             self,
             chain: "Chain",
             address: ChecksumAddress | str,
             abi=None,
     ):
         abi = abi or ERC721_ABI
         super().__init__(chain, address, abi)
 
+    @property
+    @cache
+    def name(self) -> str:
+        return self.functions.name().call()
+
+    @property
+    @cache
+    def symbol(self) -> str:
+        return self.functions.symbol().call()
+
     def get_balance(
             self,
             address: ChecksumAddress,
-            block_identifier: BlockIdentifier | None = "latest",
+            block_identifier: BlockIdentifier = "latest",
     ) -> int:
-        balance = self.functions.balanceOf(address).call(block_identifier=block_identifier)
-        return balance
+        return self.functions.balanceOf(address).call(block_identifier=block_identifier)
 
     def get_balances(
             self,
             addresses: Iterable[ChecksumAddress],
-            block_identifier: BlockIdentifier | None = "latest",
-    ) -> dict[ChecksumAddress: int]:
-        """
-        If there's a problem with a token_address `0` will be returned for balance
-        """
+            block_identifier: BlockIdentifier = "latest",
+            **kwargs,
+    ) -> Iterable[dict[str: ChecksumAddress, str: int]]:
         if not addresses:
             return []
-        addresses = list(addresses)
-        balances = self.chain.batch_call(
+
+        balances = self.chain.batch_request.contract_request(
             [self.functions.balanceOf(address) for address in addresses],
-            block_identifier=block_identifier,
-            raise_exception=False,
+            block_identifier,
+            **kwargs,
         )
-        return {address: balance if isinstance(balance, int) else 0
-                for address, balance in zip(addresses, balances)}
+        for address, balance_data in zip(addresses, balances):
+            yield {"address": address, "balance":  balance_data["result"]}
 
     def get_owners(
             self,
             token_ids: Iterable[int],
-            block_identifier: BlockIdentifier | None = "latest",
-    ) -> dict[int: ChecksumAddress]:
+            block_identifier: BlockIdentifier = "latest",
+            **kwargs,
+    ) -> Iterable[dict[str: int, str: ChecksumAddress]]:
         if not token_ids:
             return []
-        token_ids = list(token_ids)
-        owners = self.chain.batch_call(
+
+        owners = self.chain.batch_request.contract_request(
             [self.functions.ownerOf(token_id) for token_id in token_ids],
-            block_identifier=block_identifier,
-            raise_exception=False,
+            block_identifier,
+            **kwargs,
         )
-        return {token_id: to_checksum_address(owner) if isinstance(owner, str) else None
-                for token_id, owner in zip(token_ids, owners)}
+        for token_id, owner_data in zip(token_ids, owners):
+            yield {"token_id": token_id, "owner": to_checksum_address(owner_data["result"])}
 
     def get_token_uris(
             self,
             token_ids: Iterable[int],
-            block_identifier: BlockIdentifier | None = "latest",
-    ) -> dict[int: str]:
+            block_identifier: BlockIdentifier = "latest",
+            **kwargs,
+    ) -> Iterable[dict[str: int, str: str]]:
         if not token_ids:
             return []
-        token_ids = list(token_ids)
-        token_uris = self.chain.batch_call(
+
+        token_uris = self.chain.batch_request.contract_request(
             [self.functions.tokenURI(token_id) for token_id in token_ids],
             block_identifier=block_identifier,
-            raise_exception=False,
+            **kwargs,
         )
-        return {token_id: token_uri if isinstance(token_uri, str) else None
-                for token_id, token_uri in zip(token_ids, token_uris)}
-
-    def get_info(self) -> Erc721Info:
-        """
-        Get erc721 information (`name`, `symbol`)
-        Use batching to get all info in the same request
-        """
-        try:
-            name, symbol = cast(
-                list[str],
-                self.chain.batch_call(
-                    [
-                        self.functions.name(),
-                        self.functions.symbol(),
-                    ]
-                ),
-            )
-            return Erc721Info(name, symbol)
-        except (DecodingError, ValueError):  # Not all the ERC721 have metadata
-            raise InvalidERC721Info
+        for token_id, uri_data in zip(token_ids, token_uris):
+            yield {"token_id": token_id, "uri": uri_data["result"]}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `better_web3-1.0.0/better_web3/contract/multicall.py` & `better_web3-1.1.0/better_web3/contract/multicall.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 """More about MulticallV3: https://github.com/mds1/multicall
 """
 from dataclasses import dataclass
-from typing import Any, List, Optional, Sequence, Tuple
+from typing import Any, Sequence
 
 import eth_abi
 from eth_abi.exceptions import DecodingError
 from eth_typing import BlockIdentifier, BlockNumber, ChecksumAddress
 from hexbytes import HexBytes
 from web3._utils.abi import map_abi_data
 from web3._utils.normalizers import BASE_RETURN_NORMALIZERS
 from web3.contract.contract import ContractFunction
 from web3.exceptions import ContractLogicError
 
-from ..exceptions import BatchCallFunctionFailed
 from .abi import MULTICALL_V3_ABI
 from .contract import Contract
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from ..chain import Chain
 
 
 MULTICALL_V3_ADDRESS = "0xcA11bde05977b3631167028862bE2a173976CA11"
 
 
 @dataclass
 class MulticallResult:
     success: bool
-    return_data: Optional[bytes]
+    return_data: bytes | None
 
 
 @dataclass
 class MulticallDecodedResult:
     success: bool
-    return_data_decoded: Optional[Any]
+    return_data_decoded: Any | None
+
+
+class MulticallFailed(Exception):
+    pass
 
 
 class Multicall(Contract):
     def __init__(
         self,
         chain: "Chain",
-        address: Optional[ChecksumAddress | str] = None,
+        address: ChecksumAddress | str = None,
         abi=None,
     ):
         address = address or MULTICALL_V3_ADDRESS
         abi = abi or MULTICALL_V3_ABI
         super().__init__(chain, address, abi)
 
     @staticmethod
@@ -63,15 +66,15 @@
             output_types.append(
                 [output["type"] for output in contract_function.abi["outputs"]]
             )
 
         return targets_with_data, output_types
 
     @staticmethod
-    def _decode_data(output_type: Sequence[str], data: bytes) -> Optional[Any]:
+    def _decode_data(output_type: Sequence[str], data: bytes) -> Any | None:
         """
 
         :param output_type:
         :param data:
         :return:
         :raises: DecodingError
         """
@@ -90,104 +93,80 @@
                     "Cannot decode %s using output-type %s", data, output_type
                 )
                 return data
 
     def _aggregate(
         self,
         targets_with_data: Sequence[tuple[ChecksumAddress, bytes]],
-        block_identifier: Optional[BlockIdentifier] = "latest",
-    ) -> tuple[BlockNumber, list[Optional[Any]]]:
+        block_identifier: BlockIdentifier = "latest",
+    ) -> tuple[BlockNumber, list[Any | None]]:
         """
-
         :param targets_with_data: List of target `addresses` and `data` to be called in each Contract
-        :param block_identifier:
-        :return:
-        :raises: BatchCallFunctionFailed
         """
         aggregate_parameter = [
             {"target": target, "callData": data} for target, data in targets_with_data
         ]
         try:
             return self.contract.functions.aggregate(aggregate_parameter).call(
                 block_identifier=block_identifier
             )
         except (ContractLogicError, OverflowError):
-            raise BatchCallFunctionFailed
+            raise MulticallFailed
 
     def aggregate(
         self,
         contract_functions: Sequence[ContractFunction],
-        block_identifier: Optional[BlockIdentifier] = "latest",
-    ) -> Tuple[BlockNumber, List[Optional[Any]]]:
-        """
-        Calls aggregate on MakerDAO's Multicall contract. If a function called raises an error execution is stopped
-
-        :param contract_functions:
-        :param block_identifier:
-        :return: A tuple with the ``blockNumber`` and a list with the decoded return values
-        :raises: BatchCallFunctionFailed
-        """
+        block_identifier: BlockIdentifier = "latest",
+    ) -> tuple[BlockNumber, list[Any | None]]:
         targets_with_data, output_types = self._build_payload(contract_functions)
         block_number, results = self._aggregate(
             targets_with_data, block_identifier=block_identifier
         )
         decoded_results = [
             self._decode_data(output_type, data)
             for output_type, data in zip(output_types, results)
         ]
         return block_number, decoded_results
 
     def _try_aggregate(
         self,
-        targets_with_data: Sequence[Tuple[ChecksumAddress, bytes]],
+        targets_with_data: Sequence[tuple[ChecksumAddress, bytes]],
         require_success: bool = False,
-        block_identifier: Optional[BlockIdentifier] = "latest",
-    ) -> List[MulticallResult]:
-        """
-        Calls ``try_aggregate`` on MakerDAO's Multicall contract.
-
-        :param targets_with_data:
-        :param require_success: If ``True``, an exception in any of the functions will stop the execution. Also, an
-            invalid decoded value will stop the execution
-        :param block_identifier:
-        :return: A list with the decoded return values
-        """
-
+        block_identifier: BlockIdentifier = "latest",
+    ) -> list[MulticallResult]:
         aggregate_parameter = [
             {"target": target, "callData": data} for target, data in targets_with_data
         ]
+
         try:
             result = self.functions.tryAggregate(
                 require_success, aggregate_parameter
             ).call(block_identifier=block_identifier)
 
             if require_success and b"" in (data for _, data in result):
                 # `b''` values are decoding errors/missing contracts/missing functions
-                raise BatchCallFunctionFailed
+                raise MulticallFailed
 
             return [
                 MulticallResult(success, data if data else None)
                 for success, data in result
             ]
         except (ContractLogicError, OverflowError, ValueError):
-            raise BatchCallFunctionFailed
+            raise MulticallFailed
 
     def try_aggregate(
         self,
         contract_functions: Sequence[ContractFunction],
         require_success: bool = False,
-        block_identifier: Optional[BlockIdentifier] = "latest",
-    ) -> List[MulticallDecodedResult]:
+        block_identifier: BlockIdentifier = "latest",
+    ) -> list[MulticallDecodedResult]:
         """
         Calls ``try_aggregate`` on MakerDAO's Multicall contract.
 
-        :param contract_functions:
         :param require_success: If ``True``, an exception in any of the functions will stop the execution
-        :param block_identifier:
-        :return: A list with the decoded return values
         """
         targets_with_data, output_types = self._build_payload(contract_functions)
         results = self._try_aggregate(
             targets_with_data,
             require_success=require_success,
             block_identifier=block_identifier,
         )
```

### Comparing `better_web3-1.0.0/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-1.1.0/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,25 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0x28548864 (Tue Jun 13 11:34:00 2023 UTC)
-files sz: 2381
+moddate:  0x97799064 (Mon Jun 19 15:51:51 2023 UTC)
+files sz: 1907
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 9
+   stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c045a04640064046c056d065a060100640064056c076d085a08010064
-      0064066c096d0a5a0a6d0b5a0b0100640064076c0c6d0d5a0d6d0e5a0e01
-      00640064086c0f6d105a100100640064096c116d125a126d135a13010064
-      0a6514640b6508640c65146606640d84045a15640e6516640c6514660464
-      0f84045a1764106501650d7001651419000000000000000000640c651865
-      0d190000000000000000006604641184045a1964125a1a64135a1b640e65
-      166602641484045a1c090009006419641565126416651364176513640c65
-      126608641884055a1d64035300
+      0064066c096d0a5a0a0100640064076c0b6d0c5a0c6d0d5a0d0100640064
+      086c0e6d0f5a0f6d105a106d115a11010064095a12640a6513640b650864
+      0c65136606640d84045a14640e6515640c65136604640f84045a16641065
+      01650c7001651319000000000000000000640c6517650d19000000000000
+      0000006604641184045a1864125a1964135a1a640e65156602641484045a
+      1b64156510640c6511650f7a0700006604641684045a1c64035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Iterable',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Iterable)
                 10 STORE_NAME               1 (Iterable)
@@ -48,175 +47,160 @@
                 48 LOAD_CONST               5 (('LocalAccount',))
                 50 IMPORT_NAME              7 (eth_account.account)
                 52 IMPORT_FROM              8 (LocalAccount)
                 54 STORE_NAME               8 (LocalAccount)
                 56 POP_TOP
    
      7          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               6 (('to_checksum_address', 'is_checksum_address'))
+                60 LOAD_CONST               6 (('to_checksum_address',))
                 62 IMPORT_NAME              9 (eth_utils)
                 64 IMPORT_FROM             10 (to_checksum_address)
                 66 STORE_NAME              10 (to_checksum_address)
-                68 IMPORT_FROM             11 (is_checksum_address)
-                70 STORE_NAME              11 (is_checksum_address)
-                72 POP_TOP
-   
-     8          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               7 (('AnyAddress', 'ChecksumAddress'))
-                78 IMPORT_NAME             12 (eth_typing)
-                80 IMPORT_FROM             13 (AnyAddress)
-                82 STORE_NAME              13 (AnyAddress)
-                84 IMPORT_FROM             14 (ChecksumAddress)
-                86 STORE_NAME              14 (ChecksumAddress)
-                88 POP_TOP
-   
-     9          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               8 (('ContractFunction',))
-                94 IMPORT_NAME             15 (web3.contract.contract)
-                96 IMPORT_FROM             16 (ContractFunction)
-                98 STORE_NAME              16 (ContractFunction)
-               100 POP_TOP
-   
-    10         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               9 (('TxParams', 'Wei'))
-               106 IMPORT_NAME             17 (web3.types)
-               108 IMPORT_FROM             18 (TxParams)
-               110 STORE_NAME              18 (TxParams)
-               112 IMPORT_FROM             19 (Wei)
-               114 STORE_NAME              19 (Wei)
-               116 POP_TOP
-   
-    13         118 LOAD_CONST              10 ('message')
-               120 LOAD_NAME               20 (str)
-               122 LOAD_CONST              11 ('account')
-               124 LOAD_NAME                8 (LocalAccount)
-               126 LOAD_CONST              12 ('return')
-               128 LOAD_NAME               20 (str)
-               130 BUILD_TUPLE              6
-               132 LOAD_CONST              13 (<code object sign_message, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 13>)
-               134 MAKE_FUNCTION            4 (annotations)
-               136 STORE_NAME              21 (sign_message)
-   
-    19         138 LOAD_CONST              14 ('data')
-               140 LOAD_NAME               22 (bytes)
-               142 LOAD_CONST              12 ('return')
-               144 LOAD_NAME               20 (str)
-               146 BUILD_TUPLE              4
-               148 LOAD_CONST              15 (<code object decode_string_or_bytes32, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 19>)
-               150 MAKE_FUNCTION            4 (annotations)
-               152 STORE_NAME              23 (decode_string_or_bytes32)
-   
-    31         154 LOAD_CONST              16 ('addresses')
-               156 LOAD_NAME                1 (Iterable)
-               158 LOAD_NAME               13 (AnyAddress)
-               160 JUMP_IF_TRUE_OR_POP      1 (to 164)
-               162 LOAD_NAME               20 (str)
-           >>  164 BINARY_SUBSCR
-               174 LOAD_CONST              12 ('return')
-               176 LOAD_NAME               24 (list)
-               178 LOAD_NAME               13 (AnyAddress)
-               180 BINARY_SUBSCR
-               190 BUILD_TUPLE              4
-               192 LOAD_CONST              17 (<code object to_checksum_addresses, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 31>)
-               194 MAKE_FUNCTION            4 (annotations)
-               196 STORE_NAME              25 (to_checksum_addresses)
-   
-    36         198 LOAD_CONST              18 (4)
-               200 STORE_NAME              26 (GAS_CALL_DATA_ZERO_BYTE)
-   
-    37         202 LOAD_CONST              19 (16)
-               204 STORE_NAME              27 (GAS_CALL_DATA_BYTE)
-   
-    40         206 LOAD_CONST              14 ('data')
-               208 LOAD_NAME               22 (bytes)
-               210 BUILD_TUPLE              2
-               212 LOAD_CONST              20 (<code object estimate_data_gas, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 40>)
-               214 MAKE_FUNCTION            4 (annotations)
-               216 STORE_NAME              28 (estimate_data_gas)
-   
-    53         218 NOP
-   
-    54         220 NOP
-   
-    53         222 LOAD_CONST              25 ((None, None))
-               224 LOAD_CONST              21 ('tx_params')
-               226 LOAD_NAME               18 (TxParams)
-               228 LOAD_CONST              22 ('max_fee_per_gas')
-               230 LOAD_NAME               19 (Wei)
-               232 LOAD_CONST              23 ('max_priority_fee_per_gas')
-   
-    54         234 LOAD_NAME               19 (Wei)
-   
-    53         236 LOAD_CONST              12 ('return')
-   
-    55         238 LOAD_NAME               18 (TxParams)
-   
-    53         240 BUILD_TUPLE              8
-               242 LOAD_CONST              24 (<code object set_eip1559_fees, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 53>)
-               244 MAKE_FUNCTION            5 (defaults, annotations)
-               246 STORE_NAME              29 (set_eip1559_fees)
-               248 LOAD_CONST               3 (None)
-               250 RETURN_VALUE
+                68 POP_TOP
+   
+     8          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               7 (('AnyAddress', 'ChecksumAddress'))
+                74 IMPORT_NAME             11 (eth_typing)
+                76 IMPORT_FROM             12 (AnyAddress)
+                78 STORE_NAME              12 (AnyAddress)
+                80 IMPORT_FROM             13 (ChecksumAddress)
+                82 STORE_NAME              13 (ChecksumAddress)
+                84 POP_TOP
+   
+     9          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               8 (('BlockParams', 'BlockIdentifier', 'HexStr'))
+                90 IMPORT_NAME             14 (web3.types)
+                92 IMPORT_FROM             15 (BlockParams)
+                94 STORE_NAME              15 (BlockParams)
+                96 IMPORT_FROM             16 (BlockIdentifier)
+                98 STORE_NAME              16 (BlockIdentifier)
+               100 IMPORT_FROM             17 (HexStr)
+               102 STORE_NAME              17 (HexStr)
+               104 POP_TOP
+   
+    12         106 LOAD_CONST               9 (('latest', 'earliest', 'pending', 'safe', 'finalized'))
+               108 STORE_NAME              18 (BLOCK_PARAMS)
+   
+    15         110 LOAD_CONST              10 ('message')
+               112 LOAD_NAME               19 (str)
+               114 LOAD_CONST              11 ('account')
+               116 LOAD_NAME                8 (LocalAccount)
+               118 LOAD_CONST              12 ('return')
+               120 LOAD_NAME               19 (str)
+               122 BUILD_TUPLE              6
+               124 LOAD_CONST              13 (<code object sign_message, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 15>)
+               126 MAKE_FUNCTION            4 (annotations)
+               128 STORE_NAME              20 (sign_message)
+   
+    21         130 LOAD_CONST              14 ('data')
+               132 LOAD_NAME               21 (bytes)
+               134 LOAD_CONST              12 ('return')
+               136 LOAD_NAME               19 (str)
+               138 BUILD_TUPLE              4
+               140 LOAD_CONST              15 (<code object decode_string_or_bytes32, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 21>)
+               142 MAKE_FUNCTION            4 (annotations)
+               144 STORE_NAME              22 (decode_string_or_bytes32)
+   
+    33         146 LOAD_CONST              16 ('addresses')
+               148 LOAD_NAME                1 (Iterable)
+               150 LOAD_NAME               12 (AnyAddress)
+               152 JUMP_IF_TRUE_OR_POP      1 (to 156)
+               154 LOAD_NAME               19 (str)
+           >>  156 BINARY_SUBSCR
+               166 LOAD_CONST              12 ('return')
+               168 LOAD_NAME               23 (list)
+               170 LOAD_NAME               13 (ChecksumAddress)
+               172 BINARY_SUBSCR
+               182 BUILD_TUPLE              4
+               184 LOAD_CONST              17 (<code object to_checksum_addresses, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 33>)
+               186 MAKE_FUNCTION            4 (annotations)
+               188 STORE_NAME              24 (to_checksum_addresses)
+   
+    37         190 LOAD_CONST              18 (4)
+               192 STORE_NAME              25 (GAS_CALL_DATA_ZERO_BYTE)
+   
+    38         194 LOAD_CONST              19 (16)
+               196 STORE_NAME              26 (GAS_CALL_DATA_BYTE)
+   
+    41         198 LOAD_CONST              14 ('data')
+               200 LOAD_NAME               21 (bytes)
+               202 BUILD_TUPLE              2
+               204 LOAD_CONST              20 (<code object estimate_data_gas, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 41>)
+               206 MAKE_FUNCTION            4 (annotations)
+               208 STORE_NAME              27 (estimate_data_gas)
+   
+    54         210 LOAD_CONST              21 ('block_identifier')
+               212 LOAD_NAME               16 (BlockIdentifier)
+               214 LOAD_CONST              12 ('return')
+               216 LOAD_NAME               17 (HexStr)
+               218 LOAD_NAME               15 (BlockParams)
+               220 BINARY_OP                7 (|)
+               224 BUILD_TUPLE              4
+               226 LOAD_CONST              22 (<code object hex_block_identifier, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 54>)
+               228 MAKE_FUNCTION            4 (annotations)
+               230 STORE_NAME              28 (hex_block_identifier)
+               232 LOAD_CONST               3 (None)
+               234 RETURN_VALUE
    consts
       0
       ('Iterable',)
       ('HexBytes',)
       None
       ('encode_defunct',)
       ('LocalAccount',)
-      ('to_checksum_address', 'is_checksum_address')
+      ('to_checksum_address',)
       ('AnyAddress', 'ChecksumAddress')
-      ('ContractFunction',)
-      ('TxParams', 'Wei')
+      ('BlockParams', 'BlockIdentifier', 'HexStr')
+      ('latest', 'earliest', 'pending', 'safe', 'finalized')
       'message'
       'account'
       'return'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000007c00ac01a6010000ab010000000000
             0000007d007c01a00100000000000000000000000000000000000000007c
             00a6010000ab0100000000000000007d027c026a020000000000000000a0
             030000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-          13           0 RESUME                   0
+          15           0 RESUME                   0
          
-          14           2 LOAD_GLOBAL              1 (NULL + encode_defunct)
+          16           2 LOAD_GLOBAL              1 (NULL + encode_defunct)
                       14 LOAD_FAST                0 (message)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 STORE_FAST               0 (message)
          
-          15          34 LOAD_FAST                1 (account)
+          17          34 LOAD_FAST                1 (account)
                       36 LOAD_METHOD              1 (sign_message)
                       58 LOAD_FAST                0 (message)
                       60 PRECALL                  1
                       64 CALL                     1
                       74 STORE_FAST               2 (signed_message)
          
-          16          76 LOAD_FAST                2 (signed_message)
+          18          76 LOAD_FAST                2 (signed_message)
                       78 LOAD_ATTR                2 (signature)
                       88 LOAD_METHOD              3 (hex)
                      110 PRECALL                  0
                      114 CALL                     0
                      124 RETURN_VALUE
          consts
             None
             ('text',)
          names      ('encode_defunct', 'sign_message', 'signature', 'hex')
          varnames   ('message', 'account', 'signed_message')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'sign_message'
-         firstlineno 13
+         firstlineno 15
          lnotab 0x020120012a01
       'data'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
@@ -228,79 +212,79 @@
             0000006402190000000000000000007d017c01a003000000000000000000
             00000000000000000000006404a6010000ab0100000000000000007d027c
             0264056b020000000072167c01a001000000000000000000000000000000
             0000000000a6000000ab0000000000000000006302590053007c0164007c
             02850219000000000000000000a001000000000000000000000000000000
             0000000000a6000000ab0000000000000000006302590053007700780359
             007701
-          19           0 RESUME                   0
+          21           0 RESUME                   0
          
-          20           2 NOP
+          22           2 NOP
          
-          21           4 LOAD_GLOBAL              1 (NULL + eth_abi)
+          23           4 LOAD_GLOBAL              1 (NULL + eth_abi)
                       16 LOAD_ATTR                1 (decode)
                       26 LOAD_CONST               1 ('string')
                       28 BUILD_LIST               1
                       30 LOAD_FAST                0 (data)
                       32 PRECALL                  2
                       36 CALL                     2
                       46 LOAD_CONST               2 (0)
                       48 BINARY_SUBSCR
                       58 RETURN_VALUE
                  >>   60 PUSH_EXC_INFO
          
-          22          62 LOAD_GLOBAL              4 (OverflowError)
+          24          62 LOAD_GLOBAL              4 (OverflowError)
                       74 CHECK_EXC_MATCH
                       76 POP_JUMP_FORWARD_IF_FALSE   108 (to 294)
                       78 POP_TOP
          
-          23          80 LOAD_GLOBAL              1 (NULL + eth_abi)
+          25          80 LOAD_GLOBAL              1 (NULL + eth_abi)
                       92 LOAD_ATTR                1 (decode)
                      102 LOAD_CONST               3 ('bytes32')
                      104 BUILD_LIST               1
                      106 LOAD_FAST                0 (data)
                      108 PRECALL                  2
                      112 CALL                     2
                      122 LOAD_CONST               2 (0)
                      124 BINARY_SUBSCR
                      134 STORE_FAST               1 (name)
          
-          24         136 LOAD_FAST                1 (name)
+          26         136 LOAD_FAST                1 (name)
                      138 LOAD_METHOD              3 (find)
                      160 LOAD_CONST               4 (b'\x00')
                      162 PRECALL                  1
                      166 CALL                     1
                      176 STORE_FAST               2 (end_position)
          
-          25         178 LOAD_FAST                2 (end_position)
+          27         178 LOAD_FAST                2 (end_position)
                      180 LOAD_CONST               5 (-1)
                      182 COMPARE_OP               2 (==)
                      188 POP_JUMP_FORWARD_IF_FALSE    22 (to 234)
          
-          26         190 LOAD_FAST                1 (name)
+          28         190 LOAD_FAST                1 (name)
                      192 LOAD_METHOD              1 (decode)
                      214 PRECALL                  0
                      218 CALL                     0
                      228 SWAP                     2
                      230 POP_EXCEPT
                      232 RETURN_VALUE
          
-          28     >>  234 LOAD_FAST                1 (name)
+          30     >>  234 LOAD_FAST                1 (name)
                      236 LOAD_CONST               0 (None)
                      238 LOAD_FAST                2 (end_position)
                      240 BUILD_SLICE              2
                      242 BINARY_SUBSCR
                      252 LOAD_METHOD              1 (decode)
                      274 PRECALL                  0
                      278 CALL                     0
                      288 SWAP                     2
                      290 POP_EXCEPT
                      292 RETURN_VALUE
          
-          22     >>  294 RERAISE                  0
+          24     >>  294 RERAISE                  0
                  >>  296 COPY                     3
                      298 POP_EXCEPT
                      300 RERAISE                  1
          ExceptionTable:
            4 to 56 -> 60 [0]
            60 to 228 -> 296 [1] lasti
            234 to 288 -> 296 [1] lasti
@@ -314,205 +298,208 @@
             -1
          names      ('eth_abi', 'decode', 'OverflowError', 'find')
          varnames   ('data', 'name', 'end_position')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'decode_string_or_bytes32'
-         firstlineno 19
+         firstlineno 21
          lnotab 0x020102013a01120138012a010c012c023cfa
       'addresses'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code 0x9700640184007c004400a6000000ab0000000000000000005300
-          31           0 RESUME                   0
+          33           0 RESUME                   0
          
-          32           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 32>)
+          34           2 LOAD_CONST               1 (<code object <listcomp>, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\eth.py", line 34>)
                        4 MAKE_FUNCTION            0
-         
-          33           6 LOAD_FAST                0 (addresses)
-         
-          32           8 GET_ITER
+                       6 LOAD_FAST                0 (addresses)
+                       8 GET_ITER
                       10 PRECALL                  0
                       14 CALL                     0
                       24 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
-                  0x970067007c005d227d017401000000000000000000007c01a6010000ab
-                  01000000000000000072027c016e0e7403000000000000000000007c01a6
-                  010000ab01000000000000000091028c235300
-                32           0 RESUME                   0
+                  0x970067007c005d117d017401000000000000000000007c01a6010000ab
+                  01000000000000000091028c125300
+                34           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
-                       >>    6 FOR_ITER                34 (to 76)
-               
-                33           8 STORE_FAST               1 (address)
-               
-                32          10 LOAD_GLOBAL              1 (NULL + is_checksum_address)
+                       >>    6 FOR_ITER                17 (to 42)
+                             8 STORE_FAST               1 (address)
+                            10 LOAD_GLOBAL              1 (NULL + to_checksum_address)
                             22 LOAD_FAST                1 (address)
                             24 PRECALL                  1
                             28 CALL                     1
-                            38 POP_JUMP_FORWARD_IF_FALSE     2 (to 44)
-                            40 LOAD_FAST                1 (address)
-                            42 JUMP_FORWARD            14 (to 72)
-                       >>   44 LOAD_GLOBAL              3 (NULL + to_checksum_address)
-                            56 LOAD_FAST                1 (address)
-                            58 PRECALL                  1
-                            62 CALL                     1
-                       >>   72 LIST_APPEND              2
-                            74 JUMP_BACKWARD           35 (to 6)
-                       >>   76 RETURN_VALUE
+                            38 LIST_APPEND              2
+                            40 JUMP_BACKWARD           18 (to 6)
+                       >>   42 RETURN_VALUE
                consts
-               names      ('is_checksum_address', 'to_checksum_address')
+               names      ('to_checksum_address',)
                varnames   ('.0', 'address')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
                name       '<listcomp>'
-               firstlineno 32
-               lnotab 0x080102ff
+               firstlineno 34
+               lnotab 0x
          names      ()
          varnames   ('addresses',)
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'to_checksum_addresses'
-         firstlineno 31
-         lnotab 0x0201040102ff
+         firstlineno 33
+         lnotab 0x0201
       4
       16
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007c00740200000000000000000000a6
             020000ab020000000000000000720f7405000000000000000000007c00a6
             010000ab0100000000000000007d0064017d017c0044005d197d027c0273
             0b7c017406000000000000000000007a0d00007d018c0f7c017408000000
             000000000000007a0d00007d018c1a7c015300
-          40           0 RESUME                   0
+          41           0 RESUME                   0
          
-          41           2 LOAD_GLOBAL              1 (NULL + isinstance)
+          42           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (data)
                       16 LOAD_GLOBAL              2 (str)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_FALSE    15 (to 74)
          
-          42          44 LOAD_GLOBAL              5 (NULL + HexBytes)
+          43          44 LOAD_GLOBAL              5 (NULL + HexBytes)
                       56 LOAD_FAST                0 (data)
                       58 PRECALL                  1
                       62 CALL                     1
                       72 STORE_FAST               0 (data)
          
-          44     >>   74 LOAD_CONST               1 (0)
+          45     >>   74 LOAD_CONST               1 (0)
                       76 STORE_FAST               1 (gas)
          
-          45          78 LOAD_FAST                0 (data)
+          46          78 LOAD_FAST                0 (data)
                       80 GET_ITER
                  >>   82 FOR_ITER                25 (to 134)
                       84 STORE_FAST               2 (byte)
          
-          46          86 LOAD_FAST                2 (byte)
+          47          86 LOAD_FAST                2 (byte)
                       88 POP_JUMP_FORWARD_IF_TRUE    11 (to 112)
          
-          47          90 LOAD_FAST                1 (gas)
+          48          90 LOAD_FAST                1 (gas)
                       92 LOAD_GLOBAL              6 (GAS_CALL_DATA_ZERO_BYTE)
                      104 BINARY_OP               13 (+=)
                      108 STORE_FAST               1 (gas)
                      110 JUMP_BACKWARD           15 (to 82)
          
-          49     >>  112 LOAD_FAST                1 (gas)
+          50     >>  112 LOAD_FAST                1 (gas)
                      114 LOAD_GLOBAL              8 (GAS_CALL_DATA_BYTE)
                      126 BINARY_OP               13 (+=)
                      130 STORE_FAST               1 (gas)
                      132 JUMP_BACKWARD           26 (to 82)
          
-          50     >>  134 LOAD_FAST                1 (gas)
+          51     >>  134 LOAD_FAST                1 (gas)
                      136 RETURN_VALUE
          consts
             None
             0
          names      ('isinstance', 'str', 'HexBytes', 'GAS_CALL_DATA_ZERO_BYTE', 'GAS_CALL_DATA_BYTE')
          varnames   ('data', 'gas', 'byte')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
          name       'estimate_data_gas'
-         firstlineno 40
+         firstlineno 41
          lnotab 0x02012a011e0204010801040116021601
-      'tx_params'
-      'max_fee_per_gas'
-      'max_priority_fee_per_gas'
+      'block_identifier'
       code
-         argcount  : 3
-         nlocals   : 3
-         stacksize : 3
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 4
          flags     : 3
          code
-            0x97007c00a0000000000000000000000000000000000000000000a60000
-            00ab0000000000000000007d0064017c00760072037c0064013d007c017c
-            0064023c0000007c027c0064033c0000007c005300
-          53           0 RESUME                   0
-         
-          70           2 LOAD_FAST                0 (tx_params)
-                       4 LOAD_METHOD              0 (copy)
-                      26 PRECALL                  0
-                      30 CALL                     0
-                      40 STORE_FAST               0 (tx_params)
-         
-          72          42 LOAD_CONST               1 ('gasPrice')
-                      44 LOAD_FAST                0 (tx_params)
-                      46 CONTAINS_OP              0
-                      48 POP_JUMP_FORWARD_IF_FALSE     3 (to 56)
-         
-          73          50 LOAD_FAST                0 (tx_params)
-                      52 LOAD_CONST               1 ('gasPrice')
-                      54 DELETE_SUBSCR
-         
-          75     >>   56 LOAD_FAST                1 (max_fee_per_gas)
-                      58 LOAD_FAST                0 (tx_params)
-                      60 LOAD_CONST               2 ('maxFeePerGas')
-                      62 STORE_SUBSCR
-         
-          76          66 LOAD_FAST                2 (max_priority_fee_per_gas)
-                      68 LOAD_FAST                0 (tx_params)
-                      70 LOAD_CONST               3 ('maxPriorityFeePerGas')
-                      72 STORE_SUBSCR
-         
-          78          76 LOAD_FAST                0 (tx_params)
-                      78 RETURN_VALUE
+            0x97007c00740000000000000000000000760072027c0053007403000000
+            000000000000007c00740400000000000000000000a6020000ab02000000
+            000000000072107407000000000000000000007c00a6010000ab01000000
+            00000000007d006e367403000000000000000000007c0074080000000000
+            0000000000a6020000ab0200000000000000007221740b00000000000000
+            0000007c00a6010000ab010000000000000000a003000000000000000000
+            0000000000000000000000a6000000ab0000000000000000007d00740d00
+            0000000000000000007c00a6010000ab0100000000000000005300
+          54           0 RESUME                   0
+         
+          55           2 LOAD_FAST                0 (block_identifier)
+                       4 LOAD_GLOBAL              0 (BLOCK_PARAMS)
+                      16 CONTAINS_OP              0
+                      18 POP_JUMP_FORWARD_IF_FALSE     2 (to 24)
+         
+          56          20 LOAD_FAST                0 (block_identifier)
+                      22 RETURN_VALUE
+         
+          57     >>   24 LOAD_GLOBAL              3 (NULL + isinstance)
+                      36 LOAD_FAST                0 (block_identifier)
+                      38 LOAD_GLOBAL              4 (int)
+                      50 PRECALL                  2
+                      54 CALL                     2
+                      64 POP_JUMP_FORWARD_IF_FALSE    16 (to 98)
+         
+          58          66 LOAD_GLOBAL              7 (NULL + hex)
+                      78 LOAD_FAST                0 (block_identifier)
+                      80 PRECALL                  1
+                      84 CALL                     1
+                      94 STORE_FAST               0 (block_identifier)
+                      96 JUMP_FORWARD            54 (to 206)
+         
+          59     >>   98 LOAD_GLOBAL              3 (NULL + isinstance)
+                     110 LOAD_FAST                0 (block_identifier)
+                     112 LOAD_GLOBAL              8 (bytes)
+                     124 PRECALL                  2
+                     128 CALL                     2
+                     138 POP_JUMP_FORWARD_IF_FALSE    33 (to 206)
+         
+          60         140 LOAD_GLOBAL             11 (NULL + HexBytes)
+                     152 LOAD_FAST                0 (block_identifier)
+                     154 PRECALL                  1
+                     158 CALL                     1
+                     168 LOAD_METHOD              3 (hex)
+                     190 PRECALL                  0
+                     194 CALL                     0
+                     204 STORE_FAST               0 (block_identifier)
+         
+          61     >>  206 LOAD_GLOBAL             13 (NULL + HexStr)
+                     218 LOAD_FAST                0 (block_identifier)
+                     220 PRECALL                  1
+                     224 CALL                     1
+                     234 RETURN_VALUE
          consts
-            '\n    Sets the transaction parameters in EIP1559 format.\n\n    Args:\n        tx_params (TxParams): The transaction parameters.\n        max_fee_per_gas (Wei): The maximum fee per gas.\n        max_priority_fee_per_gas (Wei): The maximum priority fee per gas.\n\n    Returns:\n        TxParams: The updated transaction parameters in EIP1559 format.\n\n    Raises:\n        ValueError: If EIP1559 is not supported.\n    '
-            'gasPrice'
-            'maxFeePerGas'
-            'maxPriorityFeePerGas'
-         names      ('copy',)
-         varnames   ('tx_params', 'max_fee_per_gas', 'max_priority_fee_per_gas')
+            None
+         names      ('BLOCK_PARAMS', 'isinstance', 'int', 'hex', 'bytes', 'HexBytes', 'HexStr')
+         varnames   ('block_identifier',)
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
-         name       'set_eip1559_fees'
-         firstlineno 53
-         lnotab 0x02112802080106020a010a02
-      (None, None)
-   names      ('typing', 'Iterable', 'hexbytes', 'HexBytes', 'eth_abi', 'eth_account.messages', 'encode_defunct', 'eth_account.account', 'LocalAccount', 'eth_utils', 'to_checksum_address', 'is_checksum_address', 'eth_typing', 'AnyAddress', 'ChecksumAddress', 'web3.contract.contract', 'ContractFunction', 'web3.types', 'TxParams', 'Wei', 'str', 'sign_message', 'bytes', 'decode_string_or_bytes32', 'list', 'to_checksum_addresses', 'GAS_CALL_DATA_ZERO_BYTE', 'GAS_CALL_DATA_BYTE', 'estimate_data_gas', 'set_eip1559_fees')
+         name       'hex_block_identifier'
+         firstlineno 54
+         lnotab 0x0201120104012a0120012a014201
+   names      ('typing', 'Iterable', 'hexbytes', 'HexBytes', 'eth_abi', 'eth_account.messages', 'encode_defunct', 'eth_account.account', 'LocalAccount', 'eth_utils', 'to_checksum_address', 'eth_typing', 'AnyAddress', 'ChecksumAddress', 'web3.types', 'BlockParams', 'BlockIdentifier', 'HexStr', 'BLOCK_PARAMS', 'str', 'sign_message', 'bytes', 'decode_string_or_bytes32', 'list', 'to_checksum_addresses', 'GAS_CALL_DATA_ZERO_BYTE', 'GAS_CALL_DATA_BYTE', 'estimate_data_gas', 'hex_block_identifier')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\eth.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c0208010c010c01100110010c0110031406100c2c0504
-      0104030c0d020102ff0c0102ff020202fe
+      0x00ff02010c010c0208010c010c010c011001140304031406100c2c0404
+      0104030c0d
```

### Comparing `better_web3-1.0.0/better_web3/utils/eth.py` & `better_web3-1.1.0/better_web3/utils/eth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Iterable
 from hexbytes import HexBytes
 
 import eth_abi
 from eth_account.messages import encode_defunct
 from eth_account.account import LocalAccount
-from eth_utils import to_checksum_address, is_checksum_address
+from eth_utils import to_checksum_address
 from eth_typing import AnyAddress, ChecksumAddress
-from web3.contract.contract import ContractFunction
-from web3.types import TxParams, Wei
+from web3.types import BlockParams, BlockIdentifier, HexStr
+
+
+BLOCK_PARAMS = ("latest", "earliest", "pending", "safe", "finalized")
 
 
 def sign_message(message: str, account: LocalAccount) -> str:
     message = encode_defunct(text=message)
     signed_message = account.sign_message(message)
     return signed_message.signature.hex()
 
@@ -24,17 +26,16 @@
         end_position = name.find(b"\x00")
         if end_position == -1:
             return name.decode()
         else:
             return name[:end_position].decode()
 
 
-def to_checksum_addresses(addresses: Iterable[AnyAddress or str]) -> list[AnyAddress]:
-    return [address if is_checksum_address(address) else to_checksum_address(address)
-            for address in addresses]
+def to_checksum_addresses(addresses: Iterable[AnyAddress or str]) -> list[ChecksumAddress]:
+    return [to_checksum_address(address) for address in addresses]
 
 
 GAS_CALL_DATA_ZERO_BYTE = 4
 GAS_CALL_DATA_BYTE = 16  # 68 before Istanbul
 
 
 def estimate_data_gas(data: bytes):
@@ -46,33 +47,15 @@
         if not byte:
             gas += GAS_CALL_DATA_ZERO_BYTE
         else:
             gas += GAS_CALL_DATA_BYTE
     return gas
 
 
-def set_eip1559_fees(tx_params: TxParams, max_fee_per_gas: Wei = None,
-                     max_priority_fee_per_gas: Wei = None,
-                     ) -> TxParams:
-    """
-    Sets the transaction parameters in EIP1559 format.
-
-    Args:
-        tx_params (TxParams): The transaction parameters.
-        max_fee_per_gas (Wei): The maximum fee per gas.
-        max_priority_fee_per_gas (Wei): The maximum priority fee per gas.
-
-    Returns:
-        TxParams: The updated transaction parameters in EIP1559 format.
-
-    Raises:
-        ValueError: If EIP1559 is not supported.
-    """
-    tx_params = tx_params.copy()
-
-    if "gasPrice" in tx_params:
-        del tx_params["gasPrice"]
-
-    tx_params["maxFeePerGas"] = max_fee_per_gas
-    tx_params["maxPriorityFeePerGas"] = max_priority_fee_per_gas
-
-    return tx_params
+def hex_block_identifier(block_identifier: BlockIdentifier) -> HexStr | BlockParams:
+    if block_identifier in BLOCK_PARAMS:
+        return block_identifier
+    elif isinstance(block_identifier, int):
+        block_identifier = hex(block_identifier)
+    elif isinstance(block_identifier, bytes):
+        block_identifier = HexBytes(block_identifier).hex()
+    return HexStr(block_identifier)
```

### Comparing `better_web3-1.0.0/PKG-INFO` & `better_web3-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 1.0.0
+Version: 1.1.0
 Summary: Chain, Explorer, Contracts(Multicall, ERC20/ERC721), batch calls and other..
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: web3 (>=6.4.0,<7.0.0)
+Requires-Dist: web3 (>=6.5.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Better Web3.py
+[ [Telegram](https://t.me/Cum_Insider) ] [ [PyPi](https://pypi.org/project/better-web3) ]
 
-## Код был собран из кусков с этих репозиториев:
+```bash
+pip install better-web3
+```
+
+## Credits
 - [safe-global](https://github.com/safe-global) / [Safe-eth-py (previosly known as Gnosis-py)](https://github.com/safe-global/safe-eth-py)
 - [Whynot63](https://github.com/Whynot63) / [web3-premium](https://github.com/Whynot63/web3-premium)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

