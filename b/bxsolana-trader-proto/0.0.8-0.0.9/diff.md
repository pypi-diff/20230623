# Comparing `tmp/bxsolana-trader-proto-0.0.8.tar.gz` & `tmp/bxsolana-trader-proto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxsolana-trader-proto-0.0.8.tar", last modified: Thu Feb 16 17:44:38 2023, max compression
+gzip compressed data, was "bxsolana-trader-proto-0.0.9.tar", last modified: Tue Feb 28 20:31:23 2023, max compression
```

## Comparing `bxsolana-trader-proto-0.0.8.tar` & `bxsolana-trader-proto-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:38.615980 bxsolana-trader-proto-0.0.8/
--rw-r--r--   0 mahmoud    (501) staff       (20)      118 2023-02-16 17:44:38.597196 bxsolana-trader-proto-0.0.8/PKG-INFO
--rw-r--r--   0 mahmoud    (501) staff       (20)      567 2023-02-16 17:31:03.000000 bxsolana-trader-proto-0.0.8/README.md
--rw-r--r--   0 mahmoud    (501) staff       (20)      315 2023-02-16 17:43:08.000000 bxsolana-trader-proto-0.0.8/pyproject.toml
--rw-r--r--   0 mahmoud    (501) staff       (20)       38 2023-02-16 17:44:38.616203 bxsolana-trader-proto-0.0.8/setup.cfg
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:37.520918 bxsolana-trader-proto-0.0.8/src/
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:37.863463 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/
--rw-r--r--   0 mahmoud    (501) staff       (20)       19 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/__init__.py
--rw-r--r--   0 mahmoud    (501) staff       (20)    63317 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/api.py
--rw-r--r--   0 mahmoud    (501) staff       (20)     1137 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/common.py
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:38.264179 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/google/
--rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/google/__init__.py
--rw-r--r--   0 mahmoud    (501) staff       (20)    18745 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/google/api.py
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:38.373416 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/
--rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/__init__.py
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:38.447136 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/gateway/
--rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/gateway/__init__.py
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:38.540411 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/
--rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/__init__.py
--rw-r--r--   0 mahmoud    (501) staff       (20)    26152 2023-02-16 17:43:17.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/options.py
-drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-16 17:44:38.078854 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto.egg-info/
--rw-r--r--   0 mahmoud    (501) staff       (20)      118 2023-02-16 17:44:37.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto.egg-info/PKG-INFO
--rw-r--r--   0 mahmoud    (501) staff       (20)      649 2023-02-16 17:44:37.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto.egg-info/SOURCES.txt
--rw-r--r--   0 mahmoud    (501) staff       (20)        1 2023-02-16 17:44:37.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto.egg-info/dependency_links.txt
--rw-r--r--   0 mahmoud    (501) staff       (20)       22 2023-02-16 17:44:37.000000 bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto.egg-info/top_level.txt
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.673829 bxsolana-trader-proto-0.0.9/
+-rw-r--r--   0 mahmoud    (501) staff       (20)      118 2023-02-28 20:31:23.673698 bxsolana-trader-proto-0.0.9/PKG-INFO
+-rw-r--r--   0 mahmoud    (501) staff       (20)      567 2023-02-23 17:58:31.000000 bxsolana-trader-proto-0.0.9/README.md
+-rw-r--r--   0 mahmoud    (501) staff       (20)      315 2023-02-28 20:30:54.000000 bxsolana-trader-proto-0.0.9/pyproject.toml
+-rw-r--r--   0 mahmoud    (501) staff       (20)       38 2023-02-28 20:31:23.673869 bxsolana-trader-proto-0.0.9/setup.cfg
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.669758 bxsolana-trader-proto-0.0.9/src/
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.671698 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/
+-rw-r--r--   0 mahmoud    (501) staff       (20)       19 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/__init__.py
+-rw-r--r--   0 mahmoud    (501) staff       (20)    62802 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/api.py
+-rw-r--r--   0 mahmoud    (501) staff       (20)     1308 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/common.py
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.672668 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/google/
+-rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/google/__init__.py
+-rw-r--r--   0 mahmoud    (501) staff       (20)    18745 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/google/api.py
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.673081 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/
+-rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/__init__.py
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.673187 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/gateway/
+-rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/gateway/__init__.py
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.673415 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/
+-rw-r--r--   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/__init__.py
+-rw-r--r--   0 mahmoud    (501) staff       (20)    26152 2023-02-28 20:29:37.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/options.py
+drwxr-xr-x   0 mahmoud    (501) staff       (20)        0 2023-02-28 20:31:23.672438 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto.egg-info/
+-rw-r--r--   0 mahmoud    (501) staff       (20)      118 2023-02-28 20:31:23.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto.egg-info/PKG-INFO
+-rw-r--r--   0 mahmoud    (501) staff       (20)      649 2023-02-28 20:31:23.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 mahmoud    (501) staff       (20)        1 2023-02-28 20:31:23.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 mahmoud    (501) staff       (20)       22 2023-02-28 20:31:23.000000 bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto.egg-info/top_level.txt
```

### Comparing `bxsolana-trader-proto-0.0.8/README.md` & `bxsolana-trader-proto-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/api.py` & `bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -872,58 +872,49 @@
 
 
 @dataclass
 class PostCancelPerpOrdersRequest(betterproto.Message):
     owner_address: str = betterproto.string_field(1)
     project: "Project" = betterproto.enum_field(2)
     contract: common.PerpContract = betterproto.enum_field(3)
+    account_address: str = betterproto.string_field(4)
 
 
 @dataclass
 class PostCancelPerpOrdersResponse(betterproto.Message):
     transaction: str = betterproto.string_field(1)
 
 
 @dataclass
 class PostCancelPerpOrderRequest(betterproto.Message):
     owner_address: str = betterproto.string_field(1)
     project: "Project" = betterproto.enum_field(2)
     contract: common.PerpContract = betterproto.enum_field(3)
     client_order_i_d: int = betterproto.uint64_field(4)
     order_i_d: int = betterproto.uint64_field(5)
+    account_address: str = betterproto.string_field(6)
 
 
 @dataclass
 class PostCancelPerpOrderResponse(betterproto.Message):
     transaction: str = betterproto.string_field(1)
 
 
 @dataclass
-class PostDepositCollateralRequest(betterproto.Message):
+class PostManageCollateralRequest(betterproto.Message):
     owner_address: str = betterproto.string_field(1)
-    amount: float = betterproto.double_field(2)
-    project: "Project" = betterproto.enum_field(3)
-    contract: common.PerpContract = betterproto.enum_field(4)
-
-
-@dataclass
-class PostDepositCollateralResponse(betterproto.Message):
-    transaction: str = betterproto.string_field(1)
-
-
-@dataclass
-class PostWithdrawCollateralRequest(betterproto.Message):
-    owner_address: str = betterproto.string_field(1)
-    amount: float = betterproto.double_field(2)
-    project: "Project" = betterproto.enum_field(3)
-    contract: common.PerpContract = betterproto.enum_field(4)
+    account_address: str = betterproto.string_field(2)
+    amount: float = betterproto.double_field(3)
+    project: "Project" = betterproto.enum_field(4)
+    type: common.PerpCollateralType = betterproto.enum_field(5)
+    token: common.PerpCollateralToken = betterproto.enum_field(6)
 
 
 @dataclass
-class PostWithdrawCollateralResponse(betterproto.Message):
+class PostManageCollateralResponse(betterproto.Message):
     transaction: str = betterproto.string_field(1)
 
 
 @dataclass
 class GetOpenPerpOrdersRequest(betterproto.Message):
     project: "Project" = betterproto.enum_field(1)
     owner_address: str = betterproto.string_field(2)
@@ -1007,15 +998,14 @@
     price: float = betterproto.double_field(10)
     client_order_i_d: int = betterproto.uint64_field(11)
 
 
 @dataclass
 class PostPerpOrderResponse(betterproto.Message):
     transaction: str = betterproto.string_field(1)
-    account_address: str = betterproto.string_field(2)
 
 
 @dataclass
 class GetNewPerpOrdersStreamRequest(betterproto.Message):
     markets: List[str] = betterproto.string_field(1)
     project: "Project" = betterproto.enum_field(3)
 
@@ -1666,19 +1656,21 @@
 
     async def post_cancel_perp_orders(
         self,
         *,
         owner_address: str = "",
         project: "Project" = 0,
         contract: common.PerpContract = 0,
+        account_address: str = "",
     ) -> PostCancelPerpOrdersResponse:
         request = PostCancelPerpOrdersRequest()
         request.owner_address = owner_address
         request.project = project
         request.contract = contract
+        request.account_address = account_address
 
         return await self._unary_unary(
             "/api.Api/PostCancelPerpOrders",
             request,
             PostCancelPerpOrdersResponse,
         )
 
@@ -1686,21 +1678,23 @@
         self,
         *,
         owner_address: str = "",
         project: "Project" = 0,
         contract: common.PerpContract = 0,
         client_order_i_d: int = 0,
         order_i_d: int = 0,
+        account_address: str = "",
     ) -> PostCancelPerpOrderResponse:
         request = PostCancelPerpOrderRequest()
         request.owner_address = owner_address
         request.project = project
         request.contract = contract
         request.client_order_i_d = client_order_i_d
         request.order_i_d = order_i_d
+        request.account_address = account_address
 
         return await self._unary_unary(
             "/api.Api/PostCancelPerpOrder",
             request,
             PostCancelPerpOrderResponse,
         )
 
@@ -1758,52 +1752,36 @@
 
         return await self._unary_unary(
             "/api.Api/GetUser",
             request,
             GetUserResponse,
         )
 
-    async def post_deposit_collateral(
-        self,
-        *,
-        owner_address: str = "",
-        amount: float = 0,
-        project: "Project" = 0,
-        contract: common.PerpContract = 0,
-    ) -> PostDepositCollateralResponse:
-        request = PostDepositCollateralRequest()
-        request.owner_address = owner_address
-        request.amount = amount
-        request.project = project
-        request.contract = contract
-
-        return await self._unary_unary(
-            "/api.Api/PostDepositCollateral",
-            request,
-            PostDepositCollateralResponse,
-        )
-
-    async def post_withdraw_collateral(
+    async def post_manage_collateral(
         self,
         *,
         owner_address: str = "",
+        account_address: str = "",
         amount: float = 0,
         project: "Project" = 0,
-        contract: common.PerpContract = 0,
-    ) -> PostWithdrawCollateralResponse:
-        request = PostWithdrawCollateralRequest()
+        type: common.PerpCollateralType = 0,
+        token: common.PerpCollateralToken = 0,
+    ) -> PostManageCollateralResponse:
+        request = PostManageCollateralRequest()
         request.owner_address = owner_address
+        request.account_address = account_address
         request.amount = amount
         request.project = project
-        request.contract = contract
+        request.type = type
+        request.token = token
 
         return await self._unary_unary(
-            "/api.Api/PostWithdrawCollateral",
+            "/api.Api/PostManageCollateral",
             request,
-            PostWithdrawCollateralResponse,
+            PostManageCollateralResponse,
         )
 
     async def get_orderbooks_stream(
         self, *, markets: List[str] = [], limit: int = 0, project: "Project" = 0
     ) -> AsyncGenerator[GetOrderbooksStreamResponse, None]:
         """streaming endpoints"""
 
@@ -1960,15 +1938,15 @@
             GetSwapsStreamResponse,
         ):
             yield response
 
     async def get_perp_orderbooks_stream(
         self, *, markets: List[str] = [], limit: int = 0, project: "Project" = 0
     ) -> AsyncGenerator[GetPerpOrderbooksStreamResponse, None]:
-        """Drift streaming endpoints"""
+        """Perp streaming endpoints"""
 
         request = GetPerpOrderbooksRequest()
         request.markets = markets
         request.limit = limit
         request.project = project
 
         async for response in self._unary_stream(
```

### Comparing `bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/common.py` & `bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,24 @@
 class PerpContract(betterproto.Enum):
     ALL = 0
     SOL_PERP = 1
     ETH_PERP = 2
     BTC_PERP = 3
 
 
+class PerpCollateralType(betterproto.Enum):
+    PCT_DEPOSIT = 0
+    PCT_WITHDRAWAL = 1
+
+
+class PerpCollateralToken(betterproto.Enum):
+    PCTK_USDC = 0
+    PCTK_SOL = 1
+
+
 class Infinity(betterproto.Enum):
     INF_NOT = 0
     INF_POSITIVE = 1
     INF_NEGATIVE = 2
 
 
 @dataclass
```

### Comparing `bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/google/api.py` & `bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/google/api.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/options.py` & `bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto/grpc/gateway/protoc_gen_openapiv2/options.py`

 * *Files identical despite different names*

### Comparing `bxsolana-trader-proto-0.0.8/src/bxsolana_trader_proto.egg-info/SOURCES.txt` & `bxsolana-trader-proto-0.0.9/src/bxsolana_trader_proto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

