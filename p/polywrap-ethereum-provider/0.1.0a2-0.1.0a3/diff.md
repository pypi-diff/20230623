# Comparing `tmp/polywrap_ethereum_provider-0.1.0a2.tar.gz` & `tmp/polywrap_ethereum_provider-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_ethereum_provider-0.1.0a2.tar", max compression
+gzip compressed data, was "polywrap_ethereum_provider-0.1.0a3.tar", max compression
```

## Comparing `polywrap_ethereum_provider-0.1.0a2.tar` & `polywrap_ethereum_provider-0.1.0a3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6850 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connection.py
--rw-r--r--   0        0        0     2837 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connections.py
--rw-r--r--   0        0        0     1451 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/networks.py
--rw-r--r--   0        0        0        0 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/py.typed
--rw-r--r--   0        0        0      163 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/__init__.py
--rw-r--r--   0        0        0     2637 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/module.py
--rw-r--r--   0        0        0      843 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/types.py
--rw-r--r--   0        0        0     5228 2023-05-09 17:51:45.292402 polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/wrap_info.py
--rw-r--r--   0        0        0     1561 2023-05-09 17:51:20.952227 polywrap_ethereum_provider-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     6661 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/__init__.py
+-rw-r--r--   0        0        0     1789 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connection.py
+-rw-r--r--   0        0        0     2759 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connections.py
+-rw-r--r--   0        0        0     1451 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/networks.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/py.typed
+-rw-r--r--   0        0        0      163 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/__init__.py
+-rw-r--r--   0        0        0     2481 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/module.py
+-rw-r--r--   0        0        0      816 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/types.py
+-rw-r--r--   0        0        0     7359 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1632 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a3/PKG-INFO
```

### Comparing `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/__init__.py` & `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """This package provides a Polywrap plugin for interacting with EVM networks."""
 # pylint: disable=no-value-for-parameter
 # pylint: disable=protected-access
 import json
-from typing import Optional, cast
+from typing import Any, Optional, cast
 
 from eth_account import Account
 from eth_account._utils.signing import sign_message_hash  # type: ignore
 from eth_account.datastructures import SignedMessage, SignedTransaction
 from eth_account.messages import encode_defunct, encode_structured_data  # type: ignore
 from eth_utils.crypto import keccak
 from hexbytes import HexBytes
-from polywrap_core import Env, InvokerClient, UriPackageOrWrapper
+from polywrap_core import InvokerClient
 from polywrap_plugin import PluginPackage
 from web3 import Web3
 from web3._utils.threads import Timeout
 from web3.exceptions import TransactionNotFound
 from web3.types import RPCEndpoint
 
 from polywrap_ethereum_provider.connections import Connections
@@ -32,19 +32,19 @@
 
 class EthereumProviderPlugin(Module[Connections]):
     """A Polywrap plugin for interacting with EVM networks."""
     def __init__(self, connections: Connections):
         super().__init__(connections)
         self.connections = connections
 
-    async def request(
+    def request(
         self,
         args: ArgsRequest,
-        client: InvokerClient[UriPackageOrWrapper],
-        env: Optional[Env] = None,
+        client: InvokerClient,
+        env: Optional[Any] = None,
     ) -> str:
         """Send a remote RPC request to the registered provider."""
         connection = self.connections.get_connection(args.get("connection"))
         web3 = Web3(connection.provider)
 
         method = args["method"]
         params = json.loads(args.get("params") or "[]")
@@ -66,46 +66,46 @@
         response = connection.provider.make_request(
             method=RPCEndpoint(method), params=params
         )
         if error := response.get("error"):
             raise RuntimeError(error)
         return json.dumps(response.get("result"))
 
-    async def signer_address(
+    def signer_address(
         self,
         args: ArgsSignerAddress,
-        client: InvokerClient[UriPackageOrWrapper],
-        env: Optional[Env] = None,
+        client: InvokerClient,
+        env: Optional[Any] = None,
     ) -> Optional[str]:
         """Get the ethereum address of the signer. Return null if signer is missing."""
         connection = self.connections.get_connection(args.get("connection"))
         if connection.has_signer():
             return Account.from_key(
                 connection.signer
             ).address
         return None
 
-    async def wait_for_transaction(
+    def wait_for_transaction(
         self,
         args: ArgsWaitForTransaction,
-        client: InvokerClient[UriPackageOrWrapper],
-        env: Optional[Env] = None,
+        client: InvokerClient,
+        env: Optional[Any] = None,
     ) -> bool:
         """Wait for a transaction to be mined."""
         connection = self.connections.get_connection(args.get("connection"))
         web3 = Web3(connection.provider)
         poll_latency = 0.1
         confirmation_latency = 0.5
         timeout = args.get("timeout", 300)
 
         try:
             with Timeout(cast(float, timeout)) as _timeout:
                 # Wait for the transaction receipt
                 while (
-                    tx_receipt := await self._get_transaction_receipt(args, client, env)
+                    tx_receipt := self._get_transaction_receipt(args, client, env)
                 ) is None:
                     _timeout.sleep(poll_latency)
 
                 # Get the block number of the transaction
                 tx_block_number = tx_receipt["block_number"]
 
                 # Calculate the target block number
@@ -114,33 +114,33 @@
                 # Wait for the blockchain to reach the target block number
                 while web3.eth.block_number < target_block_number:
                     _timeout.sleep(confirmation_latency)
             return True
         except Timeout as e:
             raise TimeoutError("Transaction timed out") from e
 
-    async def sign_message(
+    def sign_message(
         self,
         args: ArgsSignMessage,
-        client: InvokerClient[UriPackageOrWrapper],
+        client: InvokerClient,
         env: None,
     ) -> str:
         """Sign a message and return the signature. Throws if signer is missing."""
         connection = self.connections.get_connection(args.get("connection"))
         web3 = Web3(connection.provider)
         signable_message = encode_defunct(args["message"])
         signed_message: SignedMessage = web3.eth.account.sign_message(
             signable_message, connection.signer
         )
         return signed_message.signature.hex()
 
-    async def sign_transaction(
+    def sign_transaction(
         self,
         args: ArgsSignTransaction,
-        client: InvokerClient[UriPackageOrWrapper],
+        client: InvokerClient,
         env: None,
     ) -> str:
         """
         Sign a serialized unsigned transaction and return the signature.\
         Throws if signer is missing.\
         This method requires a wallet-based signer with a private key,\
         and is not needed for most use cases.\
@@ -151,19 +151,19 @@
         account = Account.from_key(
             connection.signer
         )
         key_obj = account._key_obj  # type: ignore
         (v, r, s, eth_signature_bytes) = sign_message_hash(key_obj, tx_hash)  # type: ignore
         return HexBytes(cast(bytes, eth_signature_bytes)).hex()
 
-    async def _get_transaction_receipt(
+    def _get_transaction_receipt(
         self,
         args: ArgsWaitForTransaction,
-        client: InvokerClient[UriPackageOrWrapper],
-        env: Optional[Env] = None,
+        client: InvokerClient,
+        env: Optional[Any] = None,
     ):
         connection = self.connections.get_connection(args.get("connection"))
         try:
             response = connection.provider.make_request(
                 method=RPCEndpoint("eth_getTransactionReceipt"), params=[args["txHash"]]
             )
             if error := response.get("error"):
```

### Comparing `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connection.py` & `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains a connection class for an EVM network."""
 from typing import Optional, Tuple
 
 from web3 import Web3
 from web3.providers.base import JSONBaseProvider
 
-from polywrap_ethereum_provider.networks import KnownNetwork
+from .networks import KnownNetwork
 
 
 class Connection:
     """Defines a connection to an EVM network."""
 
     __slots__: Tuple[str, str] = ("_provider", "_signer")
```

### Comparing `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/connections.py` & `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module contains a connections class for an EVM network."""
 from typing import Dict, Optional, Tuple, cast
 
-from polywrap_ethereum_provider.connection import Connection
-from polywrap_ethereum_provider.networks import KnownNetwork
-from polywrap_ethereum_provider.wrap.types import Connection as SchemaConnection
+from .connection import Connection
+from .networks import KnownNetwork
+from .wrap.types import Connection as SchemaConnection
 
 
 class Connections:
     """Defines a set of connections to EVM networks."""
     __slots__: Tuple[str, str, str] = ("connections", "default_network", "signer")
 
     connections: Dict[str, Connection]
```

### Comparing `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/networks.py` & `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/networks.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a2/polywrap_ethereum_provider/wrap/types.py` & `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: This is an auto-generated file. All modifications will be overwritten.
 # type: ignore
 from __future__ import annotations
 
 from typing import TypedDict, Optional
-from enum import IntEnum, auto
+from enum import IntEnum
 
-from polywrap_core import InvokerClient, Uri, UriPackageOrWrapper
+from polywrap_core import InvokerClient, Uri
 from polywrap_msgpack import GenericMap
 
 
 ### Env START ###
 
 Env = TypedDict("Env", {
     "connection": Optional["Connection"],
```

### Comparing `polywrap_ethereum_provider-0.1.0a2/pyproject.toml` & `polywrap_ethereum_provider-0.1.0a3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-ethereum-provider"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "Ethereum provider in python"
-authors = ["Cesar <cesar@polywrap.io>"]
+authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 
 include = ["polywrap_ethereum_provider/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "6.1.0"
 eth_account = "0.8.0"
-polywrap-plugin = "0.1.0a29"
-polywrap-core = "^0.1.0a29"
-polywrap-msgpack = "^0.1.0a29"
-polywrap-manifest = "^0.1.0a29"
+polywrap-plugin = "0.1.0a33"
+polywrap-core = "0.1.0a33"
+polywrap-msgpack = "0.1.0a33"
+polywrap-manifest = "0.1.0a33"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
 pydocstyle = "^6.1.1"
-polywrap-client = "0.1.0a29"
-polywrap-client-config-builder = "0.1.0a29"
-polywrap-uri-resolvers = "^0.1.0a29"
+polywrap-client = "0.1.0a33"
+polywrap-client-config-builder = "0.1.0a33"
+polywrap-uri-resolvers = "^0.1.0a33"
 
 [tool.poetry.group.dev.dependencies]
 eth-tester = "^0.8.0b3"
+polywrap-client-config-builder = "^0.1.0a33"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
 exclude = [
```

