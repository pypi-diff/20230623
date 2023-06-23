# Comparing `tmp/cassio-0.0.5.tar.gz` & `tmp/cassio-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassio-0.0.5.tar", last modified: Mon Jun 19 12:49:54 2023, max compression
+gzip compressed data, was "cassio-0.0.6.tar", last modified: Fri Jun 23 21:55:06 2023, max compression
```

## Comparing `cassio-0.0.5.tar` & `cassio-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-19 12:49:54.204303 cassio-0.0.5/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1084 2023-06-16 14:11:44.000000 cassio-0.0.5/README.md
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-19 12:49:54.204303 cassio-0.0.5/setup.cfg
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1606 2023-06-19 10:36:08.000000 cassio-0.0.5/setup.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.200303 cassio-0.0.5/src/
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.200303 cassio-0.0.5/src/cassio/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       93 2023-06-16 15:56:04.000000 cassio-0.0.5/src/cassio/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/cql/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2384 2023-06-16 14:33:36.000000 cassio-0.0.5/src/cassio/cql/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/db_extractor/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.5/src/cassio/db_extractor/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     3001 2023-06-16 14:33:36.000000 cassio-0.0.5/src/cassio/db_extractor/cassandra_extractor.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/history/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.5/src/cassio/history/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1622 2023-06-19 12:49:19.000000 cassio-0.0.5/src/cassio/history/history_management.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/keyvalue/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.5/src/cassio/keyvalue/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2377 2023-06-16 14:33:36.000000 cassio-0.0.5/src/cassio/keyvalue/kv_cache.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/utils/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       48 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/utils/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/utils/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       65 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/utils/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2554 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/utils/vector/distance_metrics.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       55 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     6235 2023-06-16 15:56:04.000000 cassio-0.0.5/src/cassio/vector/vector_db_driver.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio.egg-info/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      643 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/SOURCES.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/dependency_links.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/requires.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/top_level.txt
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-23 21:55:06.293569 cassio-0.0.6/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1084 2023-06-16 14:11:44.000000 cassio-0.0.6/README.md
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-23 21:55:06.293569 cassio-0.0.6/setup.cfg
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1606 2023-06-23 13:27:58.000000 cassio-0.0.6/setup.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       93 2023-06-16 15:56:04.000000 cassio-0.0.6/src/cassio/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/cql/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2384 2023-06-16 14:33:36.000000 cassio-0.0.6/src/cassio/cql/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/db_extractor/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.6/src/cassio/db_extractor/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     3001 2023-06-16 14:33:36.000000 cassio-0.0.6/src/cassio/db_extractor/cassandra_extractor.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/history/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.6/src/cassio/history/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1622 2023-06-19 12:49:19.000000 cassio-0.0.6/src/cassio/history/history_management.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/keyvalue/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.6/src/cassio/keyvalue/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2377 2023-06-16 14:33:36.000000 cassio-0.0.6/src/cassio/keyvalue/kv_cache.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/utils/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       48 2023-06-16 14:11:47.000000 cassio-0.0.6/src/cassio/utils/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/utils/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       65 2023-06-16 14:11:47.000000 cassio-0.0.6/src/cassio/utils/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2554 2023-06-16 14:11:47.000000 cassio-0.0.6/src/cassio/utils/vector/distance_metrics.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       55 2023-06-16 14:11:47.000000 cassio-0.0.6/src/cassio/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     7071 2023-06-23 21:43:46.000000 cassio-0.0.6/src/cassio/vector/vector_db_driver.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-23 21:55:06.293569 cassio-0.0.6/src/cassio.egg-info/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-23 21:55:06.000000 cassio-0.0.6/src/cassio.egg-info/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      643 2023-06-23 21:55:06.000000 cassio-0.0.6/src/cassio.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-23 21:55:06.000000 cassio-0.0.6/src/cassio.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-23 21:55:06.000000 cassio-0.0.6/src/cassio.egg-info/requires.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-23 21:55:06.000000 cassio-0.0.6/src/cassio.egg-info/top_level.txt
```

### Comparing `cassio-0.0.5/PKG-INFO` & `cassio-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
```

### Comparing `cassio-0.0.5/README.md` & `cassio-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cassio-0.0.5/setup.py` & `cassio-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='cassio',
-    version='0.0.5',
+    version='0.0.6',
     author='Stefano Lottini',
     author_email='stefano.lottini@datastax.com',
     package_dir={"": "src"},
     packages=find_packages(where='src'),
     # entry_points={
     #     "console_scripts": [
     #         # will we ever have a command-line cassio script?
```

### Comparing `cassio-0.0.5/src/cassio/cql/__init__.py` & `cassio-0.0.6/src/cassio/cql/__init__.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.5/src/cassio/db_extractor/cassandra_extractor.py` & `cassio-0.0.6/src/cassio/db_extractor/cassandra_extractor.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.5/src/cassio/history/history_management.py` & `cassio-0.0.6/src/cassio/history/history_management.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.5/src/cassio/keyvalue/kv_cache.py` & `cassio-0.0.6/src/cassio/keyvalue/kv_cache.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.5/src/cassio/utils/vector/distance_metrics.py` & `cassio-0.0.6/src/cassio/utils/vector/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `cassio-0.0.5/src/cassio/vector/vector_db_driver.py` & `cassio-0.0.6/src/cassio/vector/vector_db_driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 A common driver to operate on tables with vector-similarity-search indices.
 """
 
 import json
 from operator import itemgetter
 from typing import List, Optional, Union, Dict, Any, NamedTuple
 
-from cassandra.cluster import Session
+from cassandra.cluster import Session, ResponseFuture, ResultSet
 from cassandra.query import SimpleStatement
 
 import cassio.cql
 from cassio.utils.vector.distance_metrics import distance_metrics
 
 
 JSONType = Union[Dict[str, Any], List[Any], int, float, str, bool, None]
 
 
 class VectorMixin:
-    def _create_index(self):
+    def _create_index(self) -> None:
         index_name = f'{self.table}_embedding_idx'
         st = SimpleStatement(cassio.cql.create_vector_table_index.format(
             indexName=index_name,
             keyspace=self.keyspace,
             table=self.table
         ))
-        self._execute_cql(st, tuple())
+        self.session.execute(st)
 
-    def ann_search(self, embedding_vector, numRows):
+    def ann_search(self, embedding_vector: List[float], top_k: int) -> ResultSet:
         st = SimpleStatement(cassio.cql.search_vector_table_item.format(
             keyspace=self.keyspace,
             table=self.table
         ))
-        return self._execute_cql(st, (embedding_vector, numRows))
+        return self.session.execute(st, (embedding_vector, top_k))
 
-    def _count_rows(self):
+    def _count_rows(self) -> int:
         st = SimpleStatement(cassio.cql.count_rows.format(
             keyspace=self.keyspace,
             table=self.table
         ))
-        return self._execute_cql(st, tuple()).one().count
+        return self.session.execute(st).one().count
 
 
 class VectorTable(VectorMixin):
 
     def __init__(self, session: Session, keyspace: str, table: str, embedding_dimension: int, auto_id: bool):
         self.session = session
         self.keyspace = keyspace
@@ -52,19 +52,35 @@
         self.auto_id = auto_id
         #
         self._create_table()
         self._create_index()
 
     def put(self,
             document: str,
-            embedding_vector:
-            List[float],
+            embedding_vector: List[float],
             document_id: Optional[str],
             metadata: JSONType,
-            ttl_seconds: int):
+            ttl_seconds: int) -> None:
+        self._put(False, document, embedding_vector, document_id, metadata, ttl_seconds)
+
+    def put_async(self,
+                  document: str,
+                  embedding_vector: List[float],
+                  document_id: Optional[str],
+                  metadata: JSONType,
+                  ttl_seconds: int) -> ResponseFuture:
+        return self._put(True, document, embedding_vector, document_id, metadata, ttl_seconds)
+
+    def _put(self,
+             is_async: bool,
+             document: str,
+             embedding_vector: List[float],
+             document_id: Optional[str],
+             metadata: JSONType,
+             ttl_seconds: int) -> Optional[ResponseFuture]:
         # document_id, if not autoID, must be str
         if not self.auto_id and document_id is None:
             raise ValueError('\'document_id\' must be specified unless autoID')
         if self.auto_id and document_id is not None:
             raise ValueError('\'document_id\' cannot be passes if autoID')
         if ttl_seconds:
             ttl_spec = f' USING TTL {ttl_seconds}'
@@ -76,56 +92,58 @@
             documentIdPlaceholder='now()' if self.auto_id else '%s',
             ttlSpec=ttl_spec,
         ))
         metadata_blob = json.dumps(metadata)
         # depending on autoID, the size of the values tuple changes:
         values0 = (embedding_vector, document, metadata_blob)
         values = values0 if self.auto_id else tuple([document_id] + list(values0))
-        self._execute_cql(st, values)
+        if is_async:
+            return self.session.execute_async(st, values)
+        else:
+            return self.session.execute(st, values)
 
-    def get(self, document_id: str):
+    def get(self, document_id: str) -> Dict[str, Any]:
         if self.auto_id:
             raise ValueError('\'get\' not supported if autoID')
         else:
             st = SimpleStatement(cassio.cql.get_vector_table_item.format(
                 keyspace=self.keyspace,
                 table=self.table,
             ))
-            hits = self._execute_cql(st, (document_id, ))
+            params = (document_id, )
+            hits = self.session.execute(st, params)
             hit = hits.one()
             if hit:
                 return VectorTable._jsonify_hit(hit, distance=None)
             else:
                 return None
 
     def delete(self, document_id: str) -> None:
         """This operation goes through even if the row does not exist."""
         st = SimpleStatement(cassio.cql.delete_vector_table_item.format(
             keyspace=self.keyspace,
             table=self.table,
         ))
-        self._execute_cql(st, (document_id, ))
+        params = (document_id, )
+        self.session.execute(st, params)
 
     def search(self,
                embedding_vector: List[float],
                top_k: int,
                metric: str,
-               metric_threshold: float):
+               metric_threshold: float) -> List[Dict[str, Any]]:
         # get rows by ANN
         rows = list(self.ann_search(embedding_vector, top_k))
         if not rows:
             return []
         # sort, cut, validate and prepare for returning
         #
         # evaluate metric
         distance_function, distance_reversed = distance_metrics[metric]
-        row_embeddings = [
-            row.embedding_vector
-            for row in rows
-        ]
+        row_embeddings = [row.embedding_vector for row in rows]
         # enrich with their metric score
         rows_with_metric = list(zip(
             distance_function(row_embeddings, embedding_vector),
             rows,
         ))
         # sort rows by metric score. First handle metric/threshold
         if metric_threshold is not None:
@@ -145,36 +163,33 @@
         # we discard the scores and return an iterable of hits (as JSON)
         return [
             VectorTable._jsonify_hit(hit, distance)
             for distance, hit in sorted_passing_winners
         ]
 
     @staticmethod
-    def _jsonify_hit(hit: NamedTuple, distance: float):
+    def _jsonify_hit(hit: NamedTuple, distance: Optional[float]) -> Dict[str, Any]:
         d = {
             'document_id': hit.document_id,
             'metadata': json.loads(hit.metadata_blob),
             'document': hit.document,
             'embedding_vector': hit.embedding_vector,
         }
         if distance is not None:
             d['distance'] = distance
         return d
 
-    def clear(self):
+    def clear(self) -> None:
         st = SimpleStatement(cassio.cql.truncate_vector_table.format(
             keyspace=self.keyspace,
             table=self.table,
         ))
-        self._execute_cql(st, tuple())
+        self.session.execute(st)
 
-    def _create_table(self):
+    def _create_table(self) -> None:
         st = SimpleStatement(cassio.cql.create_vector_table.format(
             keyspace=self.keyspace,
             table=self.table,
             idType='UUID' if self.auto_id else 'TEXT',
             embeddingDimension=self.embedding_dimension,
         ))
-        self._execute_cql(st, tuple())
-
-    def _execute_cql(self, statement, params: tuple):
-        return self.session.execute(statement, params)
+        self.session.execute(st)
```

### Comparing `cassio-0.0.5/src/cassio.egg-info/PKG-INFO` & `cassio-0.0.6/src/cassio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.5
+Version: 0.0.6
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
```

### Comparing `cassio-0.0.5/src/cassio.egg-info/SOURCES.txt` & `cassio-0.0.6/src/cassio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

