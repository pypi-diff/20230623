# Comparing `tmp/airstack-0.0.5.tar.gz` & `tmp/airstack-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airstack-0.0.5.tar", last modified: Wed Jun 21 07:33:40 2023, max compression
+gzip compressed data, was "airstack-0.0.6.tar", last modified: Fri Jun 23 13:29:12 2023, max compression
```

## Comparing `airstack-0.0.5.tar` & `airstack-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 07:33:40.353691 airstack-0.0.5/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-21 07:33:40.353757 airstack-0.0.5/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2785 2023-06-19 07:46:20.000000 airstack-0.0.5/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 airstack-0.0.5/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      704 2023-06-21 07:33:40.354008 airstack-0.0.5/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 07:33:40.350775 airstack-0.0.5/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 07:33:40.352641 airstack-0.0.5/src/airstack/
--rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 airstack-0.0.5/src/airstack/__init__.py
--rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 airstack-0.0.5/src/airstack/constant.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     9033 2023-06-21 06:14:44.000000 airstack-0.0.5/src/airstack/execute_query.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     8944 2023-06-21 06:14:44.000000 airstack-0.0.5/src/airstack/generic.py
--rw-r--r--   0 sarvesh    (501) staff       (20)    25580 2023-06-21 06:14:44.000000 airstack-0.0.5/src/airstack/popular_queries.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 airstack-0.0.5/src/airstack/send_request.py
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-21 07:33:40.353555 airstack-0.0.5/src/airstack.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-21 07:33:40.000000 airstack-0.0.5/src/airstack.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      378 2023-06-21 07:33:40.000000 airstack-0.0.5/src/airstack.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-21 07:33:40.000000 airstack-0.0.5/src/airstack.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-21 07:33:40.000000 airstack-0.0.5/src/airstack.egg-info/requires.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-21 07:33:40.000000 airstack-0.0.5/src/airstack.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-23 13:29:12.557075 airstack-0.0.6/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-23 13:29:12.557138 airstack-0.0.6/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2785 2023-06-19 07:46:20.000000 airstack-0.0.6/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-06-09 12:45:46.000000 airstack-0.0.6/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      704 2023-06-23 13:29:12.557408 airstack-0.0.6/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-23 13:29:12.554735 airstack-0.0.6/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-23 13:29:12.556093 airstack-0.0.6/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-09 12:45:46.000000 airstack-0.0.6/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      308 2023-06-09 12:45:46.000000 airstack-0.0.6/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     9018 2023-06-23 13:28:56.000000 airstack-0.0.6/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     8944 2023-06-21 06:14:44.000000 airstack-0.0.6/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)    25577 2023-06-23 13:28:56.000000 airstack-0.0.6/src/airstack/popular_queries.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1811 2023-06-09 12:45:46.000000 airstack-0.0.6/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-23 13:29:12.556935 airstack-0.0.6/src/airstack.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3285 2023-06-23 13:29:12.000000 airstack-0.0.6/src/airstack.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      378 2023-06-23 13:29:12.000000 airstack-0.0.6/src/airstack.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-23 13:29:12.000000 airstack-0.0.6/src/airstack.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)       35 2023-06-23 13:29:12.000000 airstack-0.0.6/src/airstack.egg-info/requires.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-23 13:29:12.000000 airstack-0.0.6/src/airstack.egg-info/top_level.txt
```

### Comparing `airstack-0.0.5/PKG-INFO` & `airstack-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `airstack-0.0.5/README.md` & `airstack-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `airstack-0.0.5/setup.cfg` & `airstack-0.0.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = airstack
-version = 0.0.5
+version = 0.0.6
 author = Airstack
 author_email = support@airstack.xyz
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `airstack-0.0.5/src/airstack/execute_query.py` & `airstack-0.0.6/src/airstack/execute_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         Returns:
             object: execute query obiect
         """
         execute_query = ExecuteQuery(query=query, variables=variables, url=self.url,
         api_key=self.api_key, timeout=self.timeout)
         return execute_query
 
-    def create_popular_queries_object(self):
+    def queries_object(self):
         """Create popular query object for popular queries
 
         Returns:
             object: execute popular query obiect
         """
         from airstack.popular_queries import ExecutePopularQueries
         execute_popular_query = ExecutePopularQueries(url=self.url,api_key=self.api_key,
```

### Comparing `airstack-0.0.5/src/airstack/generic.py` & `airstack-0.0.6/src/airstack/generic.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.5/src/airstack/popular_queries.py` & `airstack-0.0.6/src/airstack/popular_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             api_key (str, required): api key. Defaults to None.
 
         """
         self.url = url
         self.timeout = timeout
         self.api_key = api_key
 
-    async def get_all_tokens(self, variables):
+    async def get_token_balances(self, variables):
         """Func to get all tokens
 
         Args:
             variables (dict): Variables required for the query.
             - identity (Identity): The wallet address identity.
             - tokenType (list): List of token types.
             - blockchain (TokenBlockchain): The blockchain type.
@@ -208,15 +208,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_query()
 
-    async def get_all_nfts(self, variables):
+    async def get_nfts(self, variables):
         """Func to get all nfts of a collection
 
         Args:
             variables (dict): Variables required for the query.
             - address (Address): Nft token address.
             - blockchain (TokenBlockchain): The blockchain type.
             - limit (int): The limit of items to retrieve.
@@ -271,15 +271,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_paginated_query()
 
-    async def get_nft_image(self, variables):
+    async def get_nft_images(self, variables):
         """Func to get image of a nft
 
         Args:
             variables (dict): Variables required for the query.
             - address (Address): Nft token address.
             - tokenId (String): tokenId.
             - blockchain (TokenBlockchain): The blockchain type.
@@ -299,15 +299,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_query()
 
-    async def get_wallet_social_and_ens(self, variables):
+    async def get_wallet_ens_and_social(self, variables):
         """Func to get all social profile and ENS name of an wallet
 
         Args:
             variables (dict): Variables required for the query.
             - identity (Identity): The wallet address identity.
             - blockchain (TokenBlockchain): The blockchain type.
         """
@@ -370,15 +370,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_query()
 
-    async def get_wallet_balance_for_token(self, variables):
+    async def get_balance_of_token(self, variables):
         """Func to get balance of wallet address for a particular token
 
         Args:
             variables (dict): Variables required for the query.
             - blockchain (TokenBlockchain): The blockchain type.
             - tokenAddress (Address): Token address.
             - owner (Identity): The wallet address identity.
@@ -436,15 +436,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_query()
 
-    async def get_token_collection_owner(self, variables):
+    async def get_holders_of_collection(self, variables):
         """Func to get owners of a token collection
 
         Args:
             variables (dict): Variables required for the query.
             - tokenAddress (Address): Token address.
             - blockchain (TokenBlockchain): The blockchain type.
             - limit (int): The limit of items to retrieve.
@@ -504,15 +504,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_paginated_query()
 
-    async def get_nft_owners(self, variables):
+    async def get_holders_of_nft(self, variables):
         """Func to get owner(s) of the NFT
 
         Args:
             variables (dict): Variables required for the query.
             - tokenAddress (Address): Token address.
             - tokenId (String): tokenId.
             - blockchain (TokenBlockchain): The blockchain type.
@@ -572,15 +572,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_paginated_query()
 
-    async def get_primary_domain(self, variables):
+    async def get_primary_ens(self, variables):
         """Func to get Primary Domain for an address
 
         Args:
             variables (dict): Variables required for the query.
             - identity (Identity): The wallet address identity.
             - blockchain (TokenBlockchain): The blockchain type.
         """
@@ -601,15 +601,15 @@
                 }
             }
         """
         execute_query_object = AirstackClient.create_execute_query_object(self,
         query=_query, variables=variables)
         return await execute_query_object.execute_query()
 
-    async def get_subdomains(self, variables):
+    async def get_ens_subdomains(self, variables):
         """Func to get sub domains for an address
 
         Args:
             variables (dict): Variables required for the query.
             - owner (Identity): domain owner.
             - blockchain (TokenBlockchain): The blockchain type.
         """
```

### Comparing `airstack-0.0.5/src/airstack/send_request.py` & `airstack-0.0.6/src/airstack/send_request.py`

 * *Files identical despite different names*

### Comparing `airstack-0.0.5/src/airstack.egg-info/PKG-INFO` & `airstack-0.0.6/src/airstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airstack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Airstack
 Author-email: support@airstack.xyz
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

