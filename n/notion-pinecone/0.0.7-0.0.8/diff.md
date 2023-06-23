# Comparing `tmp/notion-pinecone-0.0.7.tar.gz` & `tmp/notion-pinecone-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\notion-pinecone-0.0.7.tar", last modified: Fri Jun 23 11:31:26 2023, max compression
+gzip compressed data, was "dist\notion-pinecone-0.0.8.tar", last modified: Fri Jun 23 11:52:05 2023, max compression
```

## Comparing `notion-pinecone-0.0.7.tar` & `notion-pinecone-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.689413 notion-pinecone-0.0.7/
--rw-rw-rw-   0        0        0      305 2023-06-23 11:31:12.000000 notion-pinecone-0.0.7/.bumpversion.cfg
--rw-rw-rw-   0        0        0       65 2023-06-23 11:01:57.000000 notion-pinecone-0.0.7/.gitignore
--rw-rw-rw-   0        0        0     1088 2023-06-23 10:50:41.000000 notion-pinecone-0.0.7/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.675413 notion-pinecone-0.0.7/NotionPinecone/
--rw-rw-rw-   0        0        0      143 2023-06-23 11:31:12.000000 notion-pinecone-0.0.7/NotionPinecone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.678412 notion-pinecone-0.0.7/NotionPinecone/__pycache__/
--rw-rw-rw-   0        0        0     2278 2023-06-23 10:32:21.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/embedding.cpython-39.pyc
--rw-rw-rw-   0        0        0     3525 2023-06-23 10:31:21.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/notion.cpython-39.pyc
--rw-rw-rw-   0        0        0     2562 2023-06-23 10:31:21.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/pinecone.cpython-39.pyc
--rw-rw-rw-   0        0        0     1027 2023-06-23 10:15:44.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-   0        0        0     3541 2023-06-23 11:12:38.000000 notion-pinecone-0.0.7/NotionPinecone/embedding.py
--rw-rw-rw-   0        0        0     4718 2023-06-23 11:14:32.000000 notion-pinecone-0.0.7/NotionPinecone/notion.py
--rw-rw-rw-   0        0        0     4283 2023-06-23 11:15:57.000000 notion-pinecone-0.0.7/NotionPinecone/pinecone.py
--rw-rw-rw-   0        0        0     1262 2023-06-23 11:16:29.000000 notion-pinecone-0.0.7/NotionPinecone/utils.py
--rw-rw-rw-   0        0        0      364 2023-06-23 11:31:26.689413 notion-pinecone-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-06-23 10:50:41.000000 notion-pinecone-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.688412 notion-pinecone-0.0.7/notion_pinecone.egg-info/
--rw-rw-rw-   0        0        0      364 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/top_level.txt
--rwxrwxrwx   0        0        0      165 2023-06-23 11:30:54.000000 notion-pinecone-0.0.7/pypi_upload.bat
--rw-rw-rw-   0        0        0       89 2023-06-23 10:56:22.000000 notion-pinecone-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 11:31:26.689413 notion-pinecone-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-06-23 11:31:12.000000 notion-pinecone-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:52:05.867739 notion-pinecone-0.0.8/
+-rw-rw-rw-   0        0        0      305 2023-06-23 11:52:04.000000 notion-pinecone-0.0.8/.bumpversion.cfg
+-rw-rw-rw-   0        0        0       74 2023-06-23 11:34:20.000000 notion-pinecone-0.0.8/.gitignore
+-rw-rw-rw-   0        0        0     1088 2023-06-23 10:50:41.000000 notion-pinecone-0.0.8/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-23 11:52:05.848738 notion-pinecone-0.0.8/NotionPinecone/
+-rw-rw-rw-   0        0        0      143 2023-06-23 11:52:04.000000 notion-pinecone-0.0.8/NotionPinecone/__init__.py
+-rw-rw-rw-   0        0        0     3566 2023-06-23 11:50:44.000000 notion-pinecone-0.0.8/NotionPinecone/embedding.py
+-rw-rw-rw-   0        0        0     4624 2023-06-23 11:50:00.000000 notion-pinecone-0.0.8/NotionPinecone/notion.py
+-rw-rw-rw-   0        0        0     4316 2023-06-23 11:49:51.000000 notion-pinecone-0.0.8/NotionPinecone/pinecone.py
+-rw-rw-rw-   0        0        0     1906 2023-06-23 11:45:07.000000 notion-pinecone-0.0.8/NotionPinecone/utils.py
+-rw-rw-rw-   0        0        0      364 2023-06-23 11:52:05.867739 notion-pinecone-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-06-23 10:50:41.000000 notion-pinecone-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 11:52:05.866741 notion-pinecone-0.0.8/notion_pinecone.egg-info/
+-rw-rw-rw-   0        0        0      364 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-23 11:52:05.000000 notion-pinecone-0.0.8/notion_pinecone.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0      165 2023-06-23 11:31:42.000000 notion-pinecone-0.0.8/pypi_upload.bat
+-rw-rw-rw-   0        0        0       89 2023-06-23 10:56:22.000000 notion-pinecone-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:52:05.867739 notion-pinecone-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-06-23 11:52:04.000000 notion-pinecone-0.0.8/setup.py
```

### Comparing `notion-pinecone-0.0.7/LICENSE` & `notion-pinecone-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.7/NotionPinecone/embedding.py` & `notion-pinecone-0.0.8/NotionPinecone/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import tiktoken
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.embeddings.openai import OpenAIEmbeddings
+from .utils import *
 
 # Overlap factor for text splitting
 OVERLAP_FACTOR = 20
 
 
 class Embedder:
     """
@@ -23,23 +24,23 @@
     def __init__(
         self,
         name,
         tokenizer,
         dimensions,
         max_tokens,
         overlap_factor=OVERLAP_FACTOR,
-        openai_api_key=os.environ.get("OPENAI_API_KEY"),
+        openai_api_key=None,
     ):
         """The constructor for Embedder class."""
         self.name = name
         self.tokenizer = tokenizer
         self.dimensions = dimensions
         self.max_tokens = max_tokens
         self.overlap_factor = overlap_factor
-        self.openai_api_key = openai_api_key
+        self.openai_api_key = get_env_var("OPENAI_API_KEY", openai_api_key)
 
     def encode(self, text):
         """
         Encodes a given text.
 
         Args:
             text (str): The text to encode.
```

### Comparing `notion-pinecone-0.0.7/NotionPinecone/notion.py` & `notion-pinecone-0.0.8/NotionPinecone/notion.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
     def __init__(
         self,
         notion_path,
         database_name,
         embedder,
         metadata_text_field="text",
-        openai_api_key = os.environ.get("OPENAI_API_KEY"),
-        pinecone_api_key=os.environ.get("PINECONE_API_KEY"),
-        pinecone_environment=os.environ.get("PINECONE_ENVIRONMENT"),
+        openai_api_key=None,
+        pinecone_api_key=None,
+        pinecone_environment=None,
         llm_model = "gpt-3.5-turbo"
     ):
         """The constructor for NotionPinecone class."""
         self.notion_path = notion_path
         self.embedder = embedder
         self.notion_file_paths = list(Path(notion_path).glob("**/*.md"))
         self.docs, self.metadata = self.extract_notion_data()
```

### Comparing `notion-pinecone-0.0.7/NotionPinecone/pinecone.py` & `notion-pinecone-0.0.8/NotionPinecone/pinecone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pinecone
 import os
 from langchain.vectorstores import Pinecone
 from tqdm import tqdm
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import RetrievalQAWithSourcesChain
+from .utils import *
 
 LLM_MODEL = "gpt-3.5-turbo"
 
 class PineconeVectorStore(Pinecone, pinecone.GRPCIndex):
     """
     A class that inherits from Pinecone and GRPCIndex to manage Pinecone vector stores.
 
@@ -22,26 +23,26 @@
     """
 
     def __init__(
         self,
         database_name,
         embedder,
         metadata_text_field="text",
-        openai_api_key = os.environ.get("OPENAI_API_KEY"),
-        pinecone_api_key=os.environ.get("PINECONE_API_KEY"),
-        pinecone_environment=os.environ.get("PINECONE_ENVIRONMENT"),
+        openai_api_key = None,
+        pinecone_api_key=None,
+        pinecone_environment=None,
         llm_model = LLM_MODEL
     ):
         """The constructor for PineconeVectorStore class."""
         self.database_name = database_name
         self.embedder = embedder
         self.metadata_text_field = metadata_text_field
-        self.openai_api_key=openai_api_key
-        self.pinecone_api_key = pinecone_api_key
-        self.pinecone_environment = pinecone_environment
+        self.openai_api_key = get_env_var("OPENAI_API_KEY", openai_api_key)
+        self.pinecone_api_key = get_env_var("PINECONE_API_KEY", pinecone_api_key)
+        self.pinecone_environment = get_env_var("PINECONE_ENVIRONMENT", pinecone_environment)
         self.llm_model = llm_model
         pinecone.init(
             api_key=self.pinecone_api_key, environment=self.pinecone_environment
         )
         pinecone.GRPCIndex.__init__(self, self.database_name)
         Pinecone.__init__(
             self,
```

### Comparing `notion-pinecone-0.0.7/setup.py` & `notion-pinecone-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="notion-pinecone",
-    version="0.0.7",
+    version="0.0.8",
     license="MIT",
     author="Felix Zhu",
     author_email="zhu.felix@outlook.com",
     description="Automated QA of Notion in Pinecone",
     long_description=long_description,
     packages=find_packages(),
     setup_requires=["setuptools_scm"],
```

