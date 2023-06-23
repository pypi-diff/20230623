# Comparing `tmp/notion-pinecone-0.0.8.tar.gz` & `tmp/notion-pinecone-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\notion-pinecone-0.0.8.tar", last modified: Fri Jun 23 11:52:05 2023, max compression
+gzip compressed data, was "notion-pinecone-0.0.9.tar", last modified: Fri Jun 23 12:05:45 2023, max compression
```

## Comparing `notion-pinecone-0.0.8.tar` & `notion-pinecone-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 11:52:05.867739 notion-pinecone-0.0.8/
--rw-rw-rw-   0        0        0      305 2023-06-23 11:52:04.000000 notion-pinecone-0.0.8/.bumpversion.cfg
--rw-rw-rw-   0        0        0       74 2023-06-23 11:34:20.000000 notion-pinecone-0.0.8/.gitignore
--rw-rw-rw-   0        0        0     1088 2023-06-23 10:50:41.000000 notion-pinecone-0.0.8/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-23 11:52:05.848738 notion-pinecone-0.0.8/NotionPinecone/
--rw-rw-rw-   0        0        0      143 2023-06-23 11:52:04.000000 notion-pinecone-0.0.8/NotionPinecone/__init__.py
--rw-rw-rw-   0        0        0     3566 2023-06-23 11:50:44.000000 notion-pinecone-0.0.8/NotionPinecone/embedding.py
--rw-rw-rw-   0        0        0     4624 2023-06-23 11:50:00.000000 notion-pinecone-0.0.8/NotionPinecone/notion.py
--rw-rw-rw-   0        0        0     4316 2023-06-23 11:49:51.000000 notion-pinecone-0.0.8/NotionPinecone/pinecone.py
--rw-rw-rw-   0        0        0     1906 2023-06-23 11:45:07.000000 notion-pinecone-0.0.8/NotionPinecone/utils.py
--rw-rw-rw-   0        0        0      364 2023-06-23 11:52:05.867739 notion-pinecone-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-06-23 10:50:41.000000 notion-pinecone-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 11:52:05.866741 notion-pinecone-0.0.8/notion_pinecone.egg-info/
--rw-rw-rw-   0        0        0      364 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/top_level.txt
--rwxrwxrwx   0        0        0      165 2023-06-23 11:31:42.000000 notion-pinecone-0.0.8/pypi_upload.bat
--rw-rw-rw-   0        0        0       89 2023-06-23 10:56:22.000000 notion-pinecone-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 11:52:05.867739 notion-pinecone-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-06-23 11:52:04.000000 notion-pinecone-0.0.8/setup.py
+drwxr-xr-x   0 felixzhu   (501) staff       (20)        0 2023-06-23 12:05:45.267457 notion-pinecone-0.0.9/
+-rw-r--r--   0 felixzhu   (501) staff       (20)      293 2023-06-23 12:05:28.000000 notion-pinecone-0.0.9/.bumpversion.cfg
+-rw-r--r--   0 felixzhu   (501) staff       (20)       68 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/.gitignore
+-rw-r--r--   0 felixzhu   (501) staff       (20)     1067 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/LICENSE
+drwxr-xr-x   0 felixzhu   (501) staff       (20)        0 2023-06-23 12:05:45.261957 notion-pinecone-0.0.9/NotionPinecone/
+-rw-r--r--   0 felixzhu   (501) staff       (20)      139 2023-06-23 12:05:28.000000 notion-pinecone-0.0.9/NotionPinecone/__init__.py
+-rw-r--r--   0 felixzhu   (501) staff       (20)     3437 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/NotionPinecone/embedding.py
+-rw-r--r--   0 felixzhu   (501) staff       (20)     4504 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/NotionPinecone/notion.py
+-rw-r--r--   0 felixzhu   (501) staff       (20)     4193 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/NotionPinecone/pinecone.py
+-rw-r--r--   0 felixzhu   (501) staff       (20)     1838 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/NotionPinecone/utils.py
+-rw-r--r--   0 felixzhu   (501) staff       (20)      354 2023-06-23 12:05:45.266779 notion-pinecone-0.0.9/PKG-INFO
+-rw-r--r--   0 felixzhu   (501) staff       (20)       79 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/README.md
+drwxr-xr-x   0 felixzhu   (501) staff       (20)        0 2023-06-23 12:05:45.265708 notion-pinecone-0.0.9/notion_pinecone.egg-info/
+-rw-r--r--   0 felixzhu   (501) staff       (20)      354 2023-06-23 12:05:45.000000 notion-pinecone-0.0.9/notion_pinecone.egg-info/PKG-INFO
+-rw-r--r--   0 felixzhu   (501) staff       (20)      427 2023-06-23 12:05:45.000000 notion-pinecone-0.0.9/notion_pinecone.egg-info/SOURCES.txt
+-rw-r--r--   0 felixzhu   (501) staff       (20)        1 2023-06-23 12:05:45.000000 notion-pinecone-0.0.9/notion_pinecone.egg-info/dependency_links.txt
+-rw-r--r--   0 felixzhu   (501) staff       (20)       48 2023-06-23 12:05:45.000000 notion-pinecone-0.0.9/notion_pinecone.egg-info/requires.txt
+-rw-r--r--   0 felixzhu   (501) staff       (20)       15 2023-06-23 12:05:45.000000 notion-pinecone-0.0.9/notion_pinecone.egg-info/top_level.txt
+-rw-r--r--   0 felixzhu   (501) staff       (20)      157 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/pypi_upload.bat
+-rw-r--r--   0 felixzhu   (501) staff       (20)      139 2023-06-23 12:04:51.000000 notion-pinecone-0.0.9/pypi_upload.sh
+-rw-r--r--   0 felixzhu   (501) staff       (20)       82 2023-06-23 12:02:39.000000 notion-pinecone-0.0.9/requirements.txt
+-rw-r--r--   0 felixzhu   (501) staff       (20)       38 2023-06-23 12:05:45.267724 notion-pinecone-0.0.9/setup.cfg
+-rw-r--r--   0 felixzhu   (501) staff       (20)      596 2023-06-23 12:05:28.000000 notion-pinecone-0.0.9/setup.py
```

### Comparing `notion-pinecone-0.0.8/LICENSE` & `notion-pinecone-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 felixzhu17
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 felixzhu17
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `notion-pinecone-0.0.8/NotionPinecone/pinecone.py` & `notion-pinecone-0.0.9/NotionPinecone/pinecone.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import pinecone
-import os
-from langchain.vectorstores import Pinecone
-from tqdm import tqdm
-from langchain.chat_models import ChatOpenAI
-from langchain.chains import RetrievalQAWithSourcesChain
-from .utils import *
-
-LLM_MODEL = "gpt-3.5-turbo"
-
-class PineconeVectorStore(Pinecone, pinecone.GRPCIndex):
-    """
-    A class that inherits from Pinecone and GRPCIndex to manage Pinecone vector stores.
-
-    Attributes:
-        database_name (str): Name of the Pinecone database.
-        embedder (obj): An object of a class handling embeddings.
-        metadata_text_field (str): Name of the field that holds text data.
-        openai_api_key (str): The key for the OpenAI API.
-        pinecone_api_key (str): The key for the Pinecone API.
-        pinecone_environment (str): The Pinecone environment to be used.
-        llm_model (str): The model to be used for language learning.
-    """
-
-    def __init__(
-        self,
-        database_name,
-        embedder,
-        metadata_text_field="text",
-        openai_api_key = None,
-        pinecone_api_key=None,
-        pinecone_environment=None,
-        llm_model = LLM_MODEL
-    ):
-        """The constructor for PineconeVectorStore class."""
-        self.database_name = database_name
-        self.embedder = embedder
-        self.metadata_text_field = metadata_text_field
-        self.openai_api_key = get_env_var("OPENAI_API_KEY", openai_api_key)
-        self.pinecone_api_key = get_env_var("PINECONE_API_KEY", pinecone_api_key)
-        self.pinecone_environment = get_env_var("PINECONE_ENVIRONMENT", pinecone_environment)
-        self.llm_model = llm_model
-        pinecone.init(
-            api_key=self.pinecone_api_key, environment=self.pinecone_environment
-        )
-        pinecone.GRPCIndex.__init__(self, self.database_name)
-        Pinecone.__init__(
-            self,
-            pinecone.Index(self.database_name),
-            self.embedder.embed,
-            self.metadata_text_field,
-        )
-
-    def create_database(self):
-        """Creates a Pinecone database if it doesn't already exist."""
-        if self.database_name not in pinecone.list_indexes():
-            pinecone.create_index(
-                name=self.database_name,
-                metric="cosine",
-                dimension=self.embedder.dimensions,
-            )
-
-    def upload_in_batches(self, ids, embeddings, metadata, batch_size=100):
-        """
-        Uploads data to Pinecone in batches.
-
-        Args:
-            ids (list): The list of IDs.
-            embeddings (list): The list of embeddings.
-            metadata (list): The list of metadata.
-            batch_size (int, optional): The size of each batch. Defaults to 100.
-        """
-        num_batches = len(ids) // batch_size + (len(ids) % batch_size != 0)
-
-        for i in tqdm(range(num_batches)):
-            batch_start = i * batch_size
-            batch_end = min((i + 1) * batch_size, len(ids))
-
-            ids_batch = ids[batch_start:batch_end]
-            embeddings_batch = embeddings[batch_start:batch_end]
-            metadata_batch = metadata[batch_start:batch_end]
-
-            self.upsert(vectors=zip(ids_batch, embeddings_batch, metadata_batch))
-
-    @property
-    def llm(self):
-        """
-        Property that returns a ChatOpenAI object with the specified API key and model.
-
-        Returns:
-            ChatOpenAI: A ChatOpenAI object.
-        """
-        return ChatOpenAI(
-            openai_api_key=self.openai_api_key,
-            model_name=self.llm_model,
-            temperature=0.0
-        )
-
-    @property
-    def question_answer(self):
-        """
-        Property that returns a RetrievalQAWithSourcesChain object.
-
-        Returns:
-            RetrievalQAWithSourcesChain: A RetrievalQAWithSourcesChain object.
-        """
-        return RetrievalQAWithSourcesChain.from_chain_type(
-            llm=self.llm,
-            chain_type="stuff",
-            retriever=self.as_retriever()
-        )
-
-    def ask(self, query):
-        """
-        Ask a question and get a response.
-
-        Args:
-            query (str): The query to ask.
-
-        Returns:
-            str: The response to the query.
-        """
-        return self.question_answer(query)
+import pinecone
+import os
+from langchain.vectorstores import Pinecone
+from tqdm import tqdm
+from langchain.chat_models import ChatOpenAI
+from langchain.chains import RetrievalQAWithSourcesChain
+from .utils import *
+
+LLM_MODEL = "gpt-3.5-turbo"
+
+class PineconeVectorStore(Pinecone, pinecone.GRPCIndex):
+    """
+    A class that inherits from Pinecone and GRPCIndex to manage Pinecone vector stores.
+
+    Attributes:
+        database_name (str): Name of the Pinecone database.
+        embedder (obj): An object of a class handling embeddings.
+        metadata_text_field (str): Name of the field that holds text data.
+        openai_api_key (str): The key for the OpenAI API.
+        pinecone_api_key (str): The key for the Pinecone API.
+        pinecone_environment (str): The Pinecone environment to be used.
+        llm_model (str): The model to be used for language learning.
+    """
+
+    def __init__(
+        self,
+        database_name,
+        embedder,
+        metadata_text_field="text",
+        openai_api_key = None,
+        pinecone_api_key=None,
+        pinecone_environment=None,
+        llm_model = LLM_MODEL
+    ):
+        """The constructor for PineconeVectorStore class."""
+        self.database_name = database_name
+        self.embedder = embedder
+        self.metadata_text_field = metadata_text_field
+        self.openai_api_key = get_env_var("OPENAI_API_KEY", openai_api_key)
+        self.pinecone_api_key = get_env_var("PINECONE_API_KEY", pinecone_api_key)
+        self.pinecone_environment = get_env_var("PINECONE_ENVIRONMENT", pinecone_environment)
+        self.llm_model = llm_model
+        pinecone.init(
+            api_key=self.pinecone_api_key, environment=self.pinecone_environment
+        )
+        pinecone.GRPCIndex.__init__(self, self.database_name)
+        Pinecone.__init__(
+            self,
+            pinecone.Index(self.database_name),
+            self.embedder.embed,
+            self.metadata_text_field,
+        )
+
+    def create_database(self):
+        """Creates a Pinecone database if it doesn't already exist."""
+        if self.database_name not in pinecone.list_indexes():
+            pinecone.create_index(
+                name=self.database_name,
+                metric="cosine",
+                dimension=self.embedder.dimensions,
+            )
+
+    def upload_in_batches(self, ids, embeddings, metadata, batch_size=100):
+        """
+        Uploads data to Pinecone in batches.
+
+        Args:
+            ids (list): The list of IDs.
+            embeddings (list): The list of embeddings.
+            metadata (list): The list of metadata.
+            batch_size (int, optional): The size of each batch. Defaults to 100.
+        """
+        num_batches = len(ids) // batch_size + (len(ids) % batch_size != 0)
+
+        for i in tqdm(range(num_batches)):
+            batch_start = i * batch_size
+            batch_end = min((i + 1) * batch_size, len(ids))
+
+            ids_batch = ids[batch_start:batch_end]
+            embeddings_batch = embeddings[batch_start:batch_end]
+            metadata_batch = metadata[batch_start:batch_end]
+
+            self.upsert(vectors=zip(ids_batch, embeddings_batch, metadata_batch))
+
+    @property
+    def llm(self):
+        """
+        Property that returns a ChatOpenAI object with the specified API key and model.
+
+        Returns:
+            ChatOpenAI: A ChatOpenAI object.
+        """
+        return ChatOpenAI(
+            openai_api_key=self.openai_api_key,
+            model_name=self.llm_model,
+            temperature=0.0
+        )
+
+    @property
+    def question_answer(self):
+        """
+        Property that returns a RetrievalQAWithSourcesChain object.
+
+        Returns:
+            RetrievalQAWithSourcesChain: A RetrievalQAWithSourcesChain object.
+        """
+        return RetrievalQAWithSourcesChain.from_chain_type(
+            llm=self.llm,
+            chain_type="stuff",
+            retriever=self.as_retriever()
+        )
+
+    def ask(self, query):
+        """
+        Ask a question and get a response.
+
+        Args:
+            query (str): The query to ask.
+
+        Returns:
+            str: The response to the query.
+        """
+        return self.question_answer(query)
```

### Comparing `notion-pinecone-0.0.8/NotionPinecone/utils.py` & `notion-pinecone-0.0.9/NotionPinecone/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import hashlib
-from tqdm import tqdm
-import os
-
-def get_env_var(key, var=None):
-    """Retrieve an environment variable or return a given default value.
-
-    Raises:
-        EnvironmentError: If the environment variable doesn't exist and no default value is provided.
-
-    Args:
-        key (str): The environment variable key.
-        var (str, optional): The default value to return if the environment variable is not set.
-
-    Returns:
-        str: The value of the environment variable or the default value.
-    """
-    var = var or os.getenv(key)
-    if var is None:
-        raise EnvironmentError(f"Environment variable {key} is not set")
-    return var
-
-
-def chunk_data_sources(data, sources, text_split_func):
-    """
-    Splits data into chunks and associates each chunk with its source.
-
-    Args:
-        data (list): The list of data to be chunked.
-        sources (list): The list of sources for each data item.
-        text_split_func (callable): A function that splits a text into chunks.
-
-    Returns:
-        list, list: Lists of chunks and their corresponding metadata.
-    """
-    docs = []
-    metadatas = []
-    for i, d in tqdm(enumerate(data)):
-        splits = text_split_func(d)
-        docs.extend(splits)
-        metadatas.extend([{"text": split, "source": sources[i]} for split in splits])
-    return docs, metadatas
-
-
-def hash(text):
-    """
-    Computes the SHA-256 hash of a text.
-
-    Args:
-        text (str): The text to be hashed.
-
-    Returns:
-        str: The hash of the text.
-    """
-    return hashlib.sha256(text.encode()).hexdigest()
-
-
-def hash_docs(docs):
-    """
-    Computes the hash of each document in a list.
-
-    Args:
-        docs (list): The list of documents to be hashed.
-
-    Returns:
-        list: The list of hashes for each document.
-    """
-    return [hash(doc) for doc in docs]
+import hashlib
+from tqdm import tqdm
+import os
+
+def get_env_var(key, var=None):
+    """Retrieve an environment variable or return a given default value.
+
+    Raises:
+        EnvironmentError: If the environment variable doesn't exist and no default value is provided.
+
+    Args:
+        key (str): The environment variable key.
+        var (str, optional): The default value to return if the environment variable is not set.
+
+    Returns:
+        str: The value of the environment variable or the default value.
+    """
+    var = var or os.getenv(key)
+    if var is None:
+        raise EnvironmentError(f"Environment variable {key} is not set")
+    return var
+
+
+def chunk_data_sources(data, sources, text_split_func):
+    """
+    Splits data into chunks and associates each chunk with its source.
+
+    Args:
+        data (list): The list of data to be chunked.
+        sources (list): The list of sources for each data item.
+        text_split_func (callable): A function that splits a text into chunks.
+
+    Returns:
+        list, list: Lists of chunks and their corresponding metadata.
+    """
+    docs = []
+    metadatas = []
+    for i, d in tqdm(enumerate(data)):
+        splits = text_split_func(d)
+        docs.extend(splits)
+        metadatas.extend([{"text": split, "source": sources[i]} for split in splits])
+    return docs, metadatas
+
+
+def hash(text):
+    """
+    Computes the SHA-256 hash of a text.
+
+    Args:
+        text (str): The text to be hashed.
+
+    Returns:
+        str: The hash of the text.
+    """
+    return hashlib.sha256(text.encode()).hexdigest()
+
+
+def hash_docs(docs):
+    """
+    Computes the hash of each document in a list.
+
+    Args:
+        docs (list): The list of documents to be hashed.
+
+    Returns:
+        list: The list of hashes for each document.
+    """
+    return [hash(doc) for doc in docs]
```

