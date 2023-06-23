# Comparing `tmp/embedchain-0.0.6.tar.gz` & `tmp/embedchain-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.0.6.tar", last modified: Wed Jun 21 10:40:49 2023, max compression
+gzip compressed data, was "embedchain-0.0.7.tar", last modified: Fri Jun 23 11:54:01 2023, max compression
```

## Comparing `embedchain-0.0.6.tar` & `embedchain-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.550436 embedchain-0.0.6/
--rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.6/LICENSE
--rw-r--r--   0 tj         (501) staff       (20)     6349 2023-06-21 10:40:49.550268 embedchain-0.0.6/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)     5854 2023-06-21 10:39:51.000000 embedchain-0.0.6/README.md
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.547526 embedchain-0.0.6/embedchain/
--rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/__init__.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.549232 embedchain-0.0.6/embedchain/chunkers/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/base_chunker.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.6/embedchain/chunkers/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/chunkers/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)     6661 2023-06-21 10:39:51.000000 embedchain-0.0.6/embedchain/embedchain.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.550006 embedchain-0.0.6/embedchain/loaders/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/loaders/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/loaders/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.6/embedchain/loaders/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/loaders/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.6/embedchain/utils.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-21 10:40:49.548414 embedchain-0.0.6/embedchain.egg-info/
--rw-r--r--   0 tj         (501) staff       (20)     6349 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/SOURCES.txt
--rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/dependency_links.txt
--rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/requires.txt
--rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-21 10:40:49.000000 embedchain-0.0.6/embedchain.egg-info/top_level.txt
--rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-21 10:40:49.550475 embedchain-0.0.6/setup.cfg
--rw-r--r--   0 tj         (501) staff       (20)      979 2023-06-21 10:39:51.000000 embedchain-0.0.6/setup.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.843268 embedchain-0.0.7/
+-rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.7/LICENSE
+-rw-r--r--   0 tj         (501) staff       (20)     6446 2023-06-23 11:54:01.843098 embedchain-0.0.7/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)     5951 2023-06-21 17:11:27.000000 embedchain-0.0.7/README.md
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.839888 embedchain-0.0.7/embedchain/
+-rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/__init__.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.842050 embedchain-0.0.7/embedchain/chunkers/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/chunkers/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-23 11:36:20.000000 embedchain-0.0.7/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.7/embedchain/chunkers/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     6559 2023-06-23 11:44:19.000000 embedchain-0.0.7/embedchain/embedchain.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.842777 embedchain-0.0.7/embedchain/loaders/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/loaders/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-23 11:25:48.000000 embedchain-0.0.7/embedchain/loaders/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-23 11:25:48.000000 embedchain-0.0.7/embedchain/loaders/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-23 11:25:48.000000 embedchain-0.0.7/embedchain/loaders/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/utils.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.841049 embedchain-0.0.7/embedchain.egg-info/
+-rw-r--r--   0 tj         (501) staff       (20)     6446 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/requires.txt
+-rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/top_level.txt
+-rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-23 11:54:01.843312 embedchain-0.0.7/setup.cfg
+-rw-r--r--   0 tj         (501) staff       (20)      979 2023-06-23 11:52:42.000000 embedchain-0.0.7/setup.py
```

### Comparing `embedchain-0.0.6/LICENSE` & `embedchain-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.6/PKG-INFO` & `embedchain-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.6
+Version: 0.0.7
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # embedchain
 
+[![](https://dcbadge.vercel.app/api/server/nhvCbCtKV?style=flat)](https://discord.gg/nhvCbCtKV)
+
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
```

### Comparing `embedchain-0.0.6/README.md` & `embedchain-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # embedchain
 
+[![](https://dcbadge.vercel.app/api/server/nhvCbCtKV?style=flat)](https://discord.gg/nhvCbCtKV)
+
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
```

### Comparing `embedchain-0.0.6/embedchain/chunkers/base_chunker.py` & `embedchain-0.0.7/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.6/embedchain/embedchain.py` & `embedchain-0.0.7/embedchain/embedchain.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-import chromadb
 import openai
 import os
 
-from chromadb.utils import embedding_functions
 from dotenv import load_dotenv
 from langchain.docstore.document import Document
 from langchain.embeddings.openai import OpenAIEmbeddings
 
 from embedchain.loaders.youtube_video import YoutubeVideoLoader
 from embedchain.loaders.pdf_file import PdfFileLoader
 from embedchain.loaders.web_page import WebPageLoader
 from embedchain.chunkers.youtube_video import YoutubeVideoChunker
 from embedchain.chunkers.pdf_file import PdfFileChunker
 from embedchain.chunkers.web_page import WebPageChunker
+from embedchain.vectordb.chroma_db import ChromaDB
 
 load_dotenv()
 
 embeddings = OpenAIEmbeddings()
 
 ABS_PATH = os.getcwd()
 DB_DIR = os.path.join(ABS_PATH, "db")
 
-openai_ef = embedding_functions.OpenAIEmbeddingFunction(
-    api_key=os.getenv("OPENAI_API_KEY"),
-    model_name="text-embedding-ada-002"
-)
-
 
 class EmbedChain:
-    def __init__(self):
+    def __init__(self, db=None):
         """
-        Initializes the EmbedChain instance, sets up a ChromaDB client and
-        creates a ChromaDB collection.
+         Initializes the EmbedChain instance, sets up a vector DB client and
+        creates a collection.
+
+        :param db: The instance of the VectorDB subclass.
         """
-        self.chromadb_client = self._get_or_create_db()
-        self.collection = self._get_or_create_collection()
+        if db is None:
+            db = ChromaDB()
+        self.db_client = db.client
+        self.collection = db.collection
         self.user_asks = []
 
     def _get_loader(self, data_type):
         """
         Returns the appropriate data loader for the given data type.
 
         :param data_type: The type of the data to load.
@@ -83,49 +81,44 @@
         :param url: The URL where the data is located.
         """
         loader = self._get_loader(data_type)
         chunker = self._get_chunker(data_type)
         self.user_asks.append([data_type, url])
         self.load_and_embed(loader, chunker, url)
 
-    def _get_or_create_db(self):
-        """
-        Returns a ChromaDB client, creates a new one if needed.
-
-        :return: The ChromaDB client.
-        """
-        client_settings = chromadb.config.Settings(
-            chroma_db_impl="duckdb+parquet",
-            persist_directory=DB_DIR,
-            anonymized_telemetry=False
-        )
-        return chromadb.Client(client_settings)
-
-    def _get_or_create_collection(self):
-        """
-        Returns a ChromaDB collection, creates a new one if needed.
-
-        :return: The ChromaDB collection.
-        """
-        return self.chromadb_client.get_or_create_collection(
-            'embedchain_store', embedding_function=openai_ef,
-        )
-
     def load_and_embed(self, loader, chunker, url):
         """
         Loads the data from the given URL, chunks it, and adds it to the database.
 
         :param loader: The loader to use to load the data.
         :param chunker: The chunker to use to chunk the data.
         :param url: The URL where the data is located.
         """
         embeddings_data = chunker.create_chunks(loader, url)
         documents = embeddings_data["documents"]
         metadatas = embeddings_data["metadatas"]
         ids = embeddings_data["ids"]
+        # get existing ids, and discard doc if any common id exist.
+        existing_docs = self.collection.get(
+            ids=ids,
+            # where={"url": url}
+        )
+        existing_ids = set(existing_docs["ids"])
+
+        if len(existing_ids):
+            data_dict = {id: (doc, meta) for id, doc, meta in zip(ids, documents, metadatas)}
+            data_dict = {id: value for id, value in data_dict.items() if id not in existing_ids}
+
+            if not data_dict:
+                print(f"All data from {url} already exists in the database.")
+                return
+
+            ids = list(data_dict.keys())
+            documents, metadatas = zip(*data_dict.values())
+
         self.collection.add(
             documents=documents,
             metadatas=metadatas,
             ids=ids
         )
         print(f"Successfully saved {url}. Total chunks count: {self.collection.count()}")
```

### Comparing `embedchain-0.0.6/embedchain/loaders/pdf_file.py` & `embedchain-0.0.7/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.6/embedchain/loaders/web_page.py` & `embedchain-0.0.7/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.6/embedchain/loaders/youtube_video.py` & `embedchain-0.0.7/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.6/embedchain.egg-info/PKG-INFO` & `embedchain-0.0.7/embedchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.6
+Version: 0.0.7
 Summary: embedchain is a framework to easily create LLM powered bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # embedchain
 
+[![](https://dcbadge.vercel.app/api/server/nhvCbCtKV?style=flat)](https://discord.gg/nhvCbCtKV)
+
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
```

### Comparing `embedchain-0.0.6/embedchain.egg-info/SOURCES.txt` & `embedchain-0.0.7/embedchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.6/setup.py` & `embedchain-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="embedchain",
-    version="0.0.6",
+    version="0.0.7",
     author="Taranjeet Singh",
     author_email="reachtotj@gmail.com",
     description="embedchain is a framework to easily create LLM powered bots over any dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/embedchain/embedchain",
     packages=setuptools.find_packages(),
```

