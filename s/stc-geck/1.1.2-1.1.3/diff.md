# Comparing `tmp/stc-geck-1.1.2.tar.gz` & `tmp/stc-geck-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.1.2.tar", last modified: Fri Jun 16 13:54:23 2023, max compression
+gzip compressed data, was "stc-geck-1.1.3.tar", last modified: Fri Jun 23 09:02:47 2023, max compression
```

## Comparing `stc-geck-1.1.2.tar` & `stc-geck-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:54:23.078138 stc-geck-1.1.2/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.2/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:54:23.077464 stc-geck-1.1.2/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.2/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-16 13:53:53.000000 stc-geck-1.1.2/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-16 08:01:51.000000 stc-geck-1.1.2/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-16 13:54:23.078377 stc-geck-1.1.2/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:54:23.067923 stc-geck-1.1.2/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     6043 2023-06-16 07:46:13.000000 stc-geck-1.1.2/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     4756 2023-06-16 13:53:08.000000 stc-geck-1.1.2/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1149 2023-06-15 11:53:46.000000 stc-geck-1.1.2/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-16 13:54:23.075997 stc-geck-1.1.2/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-16 13:54:23.000000 stc-geck-1.1.2/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-23 09:02:47.557919 stc-geck-1.1.3/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.1.3/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-23 09:02:47.557384 stc-geck-1.1.3/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.1.3/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-06-23 09:01:59.000000 stc-geck-1.1.3/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-06-23 09:01:52.000000 stc-geck-1.1.3/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-06-23 09:02:47.558183 stc-geck-1.1.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-23 09:02:47.552314 stc-geck-1.1.3/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)     6152 2023-06-18 14:44:03.000000 stc-geck-1.1.3/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6236 2023-06-18 18:47:15.000000 stc-geck-1.1.3/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.1.3/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-23 09:02:47.556494 stc-geck-1.1.3/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      344 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      300 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-06-23 09:02:47.000000 stc-geck-1.1.3/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.1.2/pyproject.toml` & `stc-geck-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.1.2"
+version = "1.1.3"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.1.2/stc_geck/cli.py` & `stc-geck-1.1.3/stc_geck/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,38 +110,44 @@
                     f.close()
                     print(f"{colored('INFO', 'green')}: File {final_file_name} is written")
             else:
                 print(f"{colored('ERROR', 'red')}: Not found CID for {query}", file=sys.stderr)
         else:
             print(f"{colored('ERROR', 'red')}: Not found {query}", file=sys.stderr)
 
-    async def create_ipfs_directory(self, output_car: str, query: str = None, limit: int = 100):
+    async def create_ipfs_directory(
+        self,
+        output_car: str,
+        query: str = None,
+        limit: int = 100,
+        name_template: str = '{id}.{extension}',
+    ):
         """
         Stream all STC documents.
 
         :return: metadata records
         """
         print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_alias}...")
         async with self.geck as geck:
-            return await geck.create_ipfs_directory(self.index_alias, output_car, query, limit)
+            return await geck.create_ipfs_directory(self.index_alias, output_car, query, limit, name_template)
 
 
 async def stc_geck_cli(
     ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
     ipfs_data_directory: str = '/ipns/standard-template-construct.org/data/',
-    index_alias: str = 'nexus_books',
+    index_alias: str = 'nexus_science',
     grpc_api_endpoint: str = '127.0.0.1:37082',
     embed: bool = True,
     timeout: int = 600,
     debug: bool = False,
 ):
     """
     :param ipfs_http_endpoint: IPFS HTTP API Endpoint
     :param ipfs_data_directory: path to the directory with index
-    :param index_alias: `nexus_books` (similar to LibGen) or `nexus_science` (similar to Crossref)
+    :param index_alias: `nexus_free` (non-classified content) or `nexus_science` (similar to Crossref)
     :param grpc_api_endpoint: port used for Summa
     :param embed: setup embedded Summa server
     :param timeout: timeout for requests to IPFS
     :param debug: add debugging output
     :return:
     """
     logging.basicConfig(stream=sys.stdout, level=logging.INFO if debug else logging.ERROR)
```

### Comparing `stc-geck-1.1.2/stc_geck/utils.py` & `stc-geck-1.1.3/stc_geck/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 import asyncio
 import os
+import re
 import tempfile
 from urllib.parse import quote
 
 import ipfs_hamt_directory_py
-import orjson
+
+
+NON_ALNUMWHITESPACE_REGEX = re.compile(r'([^\s\w])+')
+MULTIWHITESPACE_REGEX = re.compile(r"\s+")
+
+
+def cast_string_to_single_string(s):
+    processed = MULTIWHITESPACE_REGEX.sub(' ', NON_ALNUMWHITESPACE_REGEX.sub(' ', s))
+    processed = processed.strip().replace(' ', '-')
+    return processed
 
 
 async def create_car(output_car, documents, limit, name_template) -> (str, bytes):
     with tempfile.TemporaryDirectory() as td:
         input_data = os.path.join(td, 'input_data.txt')
         with open(input_data, 'wb') as f:
             async for document in documents:
-                document = orjson.loads(document)
                 if limit <= 0:
                     break
+                id_ = document.get('doi') or document.get('md5')
                 item_name = name_template.format(
-                    md5=document['md5'],
+                    title=cast_string_to_single_string(document['title']) if 'title' in document else id_,
+                    id=id_,
+                    md5=document.get('md5'),
+                    doi=document.get('doi'),
                     extension=document.get('metadata', {}).get('extension', 'pdf'),
                 )
                 f.write(quote(item_name, safe='').encode())
                 f.write(b' ')
                 f.write(document['cid'].encode())
                 f.write(b' ')
                 f.write(str(document.get('filesize') or 0).encode())
```

