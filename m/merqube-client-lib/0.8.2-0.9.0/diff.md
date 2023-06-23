# Comparing `tmp/merqube_client_lib-0.8.2.tar.gz` & `tmp/merqube_client_lib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.8.2.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.9.0.tar", max compression
```

## Comparing `merqube_client_lib-0.8.2.tar` & `merqube_client_lib-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-24 14:52:02.241294 merqube_client_lib-0.8.2/LICENSE
--rw-r--r--   0        0        0     5272 2023-05-24 14:52:02.241294 merqube_client_lib-0.8.2/README.md
--rw-r--r--   0        0        0        0 2023-05-24 14:52:02.241294 merqube_client_lib-0.8.2/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 14:52:02.241294 merqube_client_lib-0.8.2/merqube_client_lib/api_client/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-24 14:52:02.241294 merqube_client_lib-0.8.2/merqube_client_lib/api_client/base.py
--rw-r--r--   0        0        0     2535 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/api_client/indexapi.py
--rw-r--r--   0        0        0     6722 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/api_client/merqube_client.py
--rw-r--r--   0        0        0    11322 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/api_client/secapi.py
--rw-r--r--   0        0        0      367 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      595 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     4170 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/py.typed
--rw-r--r--   0        0        0    71154 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/pydantic_types.py
--rw-r--r--   0        0        0        0 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    11712 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/session.py
--rw-r--r--   0        0        0      414 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1829 2023-05-24 14:52:02.245294 merqube_client_lib-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 merqube_client_lib-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5272 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/api_client/__init__.py
+-rw-r--r--   0        0        0    14624 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/api_client/base.py
+-rw-r--r--   0        0        0     6661 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/api_client/merqube_client.py
+-rw-r--r--   0        0        0      367 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      595 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     4170 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0    71154 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/pydantic_types.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    11712 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      414 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1829 2023-05-25 12:36:36.657901 merqube_client_lib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 merqube_client_lib-0.9.0/PKG-INFO
```

### Comparing `merqube_client_lib-0.8.2/LICENSE` & `merqube_client_lib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/README.md` & `merqube_client_lib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/api_client/merqube_client.py` & `merqube_client_lib-0.9.0/merqube_client_lib/api_client/merqube_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 Combined API Client for all merqube APIs
 """
 from typing import Any, cast
 
 import pandas as pd
 from cachetools import LRUCache, cached
 
-from merqube_client_lib.api_client.indexapi import IndexAPIClient
-from merqube_client_lib.api_client.secapi import SecAPIClient
+from merqube_client_lib.api_client import base
 from merqube_client_lib.pydantic_types import IndexDefinitionPatchPutGet as Index
 from merqube_client_lib.session import MerqubeAPISession
 from merqube_client_lib.types import Manifest
 
 
-class MerqubeAPIClient(IndexAPIClient, SecAPIClient):
+class MerqubeAPIClient(base._IndexAPIClient, base._SecAPIClient):  # noqa
     """
     Combined API Client for indexapi + secapi, for methods that do not pertain to a particular index
     (general queries, CRUD of indices, etc)
     For a client pertaining to a specific existing index, use MerqubeAPIClientSingleIndex
     """
```

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/api_client/secapi.py` & `merqube_client_lib-0.9.0/merqube_client_lib/api_client/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,126 @@
 """
-Main SecAPI client class
-
-MerqubeAPIClient is a superset of this and the other clients.
+Base class for all Merqube API Clients
 """
 import operator
 from collections import abc
-from typing import Any, Iterable, Optional
+from typing import Any, Iterable, Optional, cast
 
 import pandas as pd
 from cachetools import TTLCache, cachedmethod
 
-from merqube_client_lib.api_client.base import MerqubeApiClientBase
+# import like this so monkeypatch works as expected
+from merqube_client_lib import session
 from merqube_client_lib.constants import DEFAULT_CACHE_TTL
+from merqube_client_lib.pydantic_types import IndexDefinitionPatchPutGet as Index
 from merqube_client_lib.session import MerqubeAPISession
+from merqube_client_lib.types import Manifest, ManifestList
 from merqube_client_lib.types.secapi import (
     AddlSecapiOptions,
     MappingTable,
     SecapiMetricDefinition,
     SecAPIRecordsResponse,
 )
 from merqube_client_lib.util import batch_post_payload
 
 
-class SecAPIClient(MerqubeApiClientBase):
+class _MerqubeApiClientBase:
+    """
+    base class that contains validation functions
+    """
+
+    def __init__(
+        self,
+        user_session: Optional[session.MerqubeAPISession] = None,
+        token: Optional[str] = None,
+        **session_kwargs: Any,
+    ):
+        self.session = user_session or session.get_merqube_session(token=token, **session_kwargs)
+
+    def _collection_helper(
+        self,
+        *,
+        url: str,
+        query_options: dict[str, str | Iterable[str] | None] | None = None,
+    ) -> ManifestList:
+        """
+        common function to /security metrics and definitions
+        """
+        options: dict[str, str | list[str]] = {}
+
+        for qo, v in (query_options or {}).items():
+            if v is not None:
+                options[qo] = v if isinstance(v, str) else ",".join(v)
+
+        return self.session.get_collection(url=url, options=options)
+
+
+class _IndexAPIClient(_MerqubeApiClientBase):
+    """
+    Indexapi class that contains methods that deal with multiple indices, creation of indices etc
+    """
+
+    def get_index_defs(
+        self, index_names: str | list[str] | None = None, include_nonprod: bool = False
+    ) -> dict[str, Manifest]:
+        """
+        Get index definitions for specified names, or all permissioned indices as a dictionary with ids as keys and index definitions as values
+
+        supports index_names:
+        - XXX - single name
+        - XXX,YYY - comma separated names
+        - [XXX,YYY] - list of names
+
+        Note that MerQube's "collection apis" never return a 404 - these are search apis, and will return an empty list if no results are found
+        """
+
+        endpoint = "/index"
+        if include_nonprod:
+            endpoint += "?type=all"
+
+        if not index_names:
+            all_indices = self.session.get_collection(endpoint)
+            return {i["id"]: i for i in all_indices}
+
+        names_arg = index_names if isinstance(index_names, str) else ",".join(index_names)
+
+        prod_clause = "&type=all" if include_nonprod else ""
+        url = f"/index?names={names_arg}{prod_clause}"
+        res = self.session.get_collection(url)
+        return {i["id"]: i for i in res}
+
+    def create_index(self, index_def: Index) -> dict[str, str]:
+        """
+        Create an index
+        Returns a dictionary containing the id of the index and its related securities (index, intraday_index)
+
+        TODO: examples and index templates to be added to this repo.
+        """
+        return cast(dict[str, str], self.session.post("/index", json=index_def.dict()).json())
+
+    def update_index(self, index_id: str, index_def: Index) -> None:
+        """
+        Update (full object replacement) an index
+        """
+        self.session.put(f"/index/{index_id}", json=index_def.dict())
+
+    def patch_index(self, index_id: str, index_updates: Manifest) -> None:
+        """
+        Patch an index - index_updates is a partial index manifest
+        """
+        self.session.patch(f"/index/{index_id}", json=index_updates)
+
+    def delete_index(self, index_id: str) -> None:
+        """
+        Delete an index
+        """
+        self.session.delete(f"/index/{index_id}")
+
+
+class _SecAPIClient(_MerqubeApiClientBase):
     """
     Secapi client class
     """
 
     def __init__(
         self,
         user_session: Optional[MerqubeAPISession] = None,
```

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/exceptions.py` & `merqube_client_lib-0.9.0/merqube_client_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/logging.py` & `merqube_client_lib-0.9.0/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/mocker.py` & `merqube_client_lib-0.9.0/merqube_client_lib/mocker.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/pydantic_types.py` & `merqube_client_lib-0.9.0/merqube_client_lib/pydantic_types.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/session.py` & `merqube_client_lib-0.9.0/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/merqube_client_lib/util.py` & `merqube_client_lib-0.9.0/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.8.2/pyproject.toml` & `merqube_client_lib-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.8.2"
+version = "0.9.0"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

### Comparing `merqube_client_lib-0.8.2/PKG-INFO` & `merqube_client_lib-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.8.2
+Version: 0.9.0
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

