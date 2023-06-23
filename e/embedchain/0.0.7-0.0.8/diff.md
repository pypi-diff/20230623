# Comparing `tmp/embedchain-0.0.7.tar.gz` & `tmp/embedchain-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.0.7.tar", last modified: Fri Jun 23 11:54:01 2023, max compression
+gzip compressed data, was "embedchain-0.0.8.tar", last modified: Fri Jun 23 17:19:43 2023, max compression
```

## Comparing `embedchain-0.0.7.tar` & `embedchain-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.843268 embedchain-0.0.7/
--rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.7/LICENSE
--rw-r--r--   0 tj         (501) staff       (20)     6446 2023-06-23 11:54:01.843098 embedchain-0.0.7/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)     5951 2023-06-21 17:11:27.000000 embedchain-0.0.7/README.md
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.839888 embedchain-0.0.7/embedchain/
--rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/__init__.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.842050 embedchain-0.0.7/embedchain/chunkers/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/chunkers/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-23 11:36:20.000000 embedchain-0.0.7/embedchain/chunkers/base_chunker.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/chunkers/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.7/embedchain/chunkers/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/chunkers/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)     6559 2023-06-23 11:44:19.000000 embedchain-0.0.7/embedchain/embedchain.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.842777 embedchain-0.0.7/embedchain/loaders/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/loaders/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-23 11:25:48.000000 embedchain-0.0.7/embedchain/loaders/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-23 11:25:48.000000 embedchain-0.0.7/embedchain/loaders/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-23 11:25:48.000000 embedchain-0.0.7/embedchain/loaders/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.7/embedchain/utils.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 11:54:01.841049 embedchain-0.0.7/embedchain.egg-info/
--rw-r--r--   0 tj         (501) staff       (20)     6446 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/SOURCES.txt
--rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/dependency_links.txt
--rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/requires.txt
--rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-23 11:54:01.000000 embedchain-0.0.7/embedchain.egg-info/top_level.txt
--rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-23 11:54:01.843312 embedchain-0.0.7/setup.cfg
--rw-r--r--   0 tj         (501) staff       (20)      979 2023-06-23 11:52:42.000000 embedchain-0.0.7/setup.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.096723 embedchain-0.0.8/
+-rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.8/LICENSE
+-rw-r--r--   0 tj         (501) staff       (20)     7108 2023-06-23 17:19:43.096584 embedchain-0.0.8/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)     6613 2023-06-23 17:14:59.000000 embedchain-0.0.8/README.md
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.093089 embedchain-0.0.8/embedchain/
+-rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/__init__.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.095205 embedchain-0.0.8/embedchain/chunkers/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/chunkers/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-23 11:36:20.000000 embedchain-0.0.8/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-23 17:14:59.000000 embedchain-0.0.8/embedchain/chunkers/qna_pair.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.8/embedchain/chunkers/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     8154 2023-06-23 17:15:05.000000 embedchain-0.0.8/embedchain/embedchain.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.096355 embedchain-0.0.8/embedchain/loaders/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.8/embedchain/loaders/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      301 2023-06-23 17:14:59.000000 embedchain-0.0.8/embedchain/loaders/local_qna_pair.py
+-rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-23 11:25:48.000000 embedchain-0.0.8/embedchain/loaders/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-23 11:25:48.000000 embedchain-0.0.8/embedchain/loaders/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-23 11:25:48.000000 embedchain-0.0.8/embedchain/loaders/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     1162 2023-06-23 17:15:05.000000 embedchain-0.0.8/embedchain/utils.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-23 17:19:43.093796 embedchain-0.0.8/embedchain.egg-info/
+-rw-r--r--   0 tj         (501) staff       (20)     7108 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)      630 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/requires.txt
+-rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-23 17:19:43.000000 embedchain-0.0.8/embedchain.egg-info/top_level.txt
+-rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-23 17:19:43.096756 embedchain-0.0.8/setup.cfg
+-rw-r--r--   0 tj         (501) staff       (20)      979 2023-06-23 17:18:27.000000 embedchain-0.0.8/setup.py
```

### Comparing `embedchain-0.0.7/LICENSE` & `embedchain-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.7/PKG-INFO` & `embedchain-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.7
+Version: 0.0.8
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
 
 [![](https://dcbadge.vercel.app/api/server/nhvCbCtKV?style=flat)](https://discord.gg/nhvCbCtKV)
+![PyPI](https://img.shields.io/pypi/v/embedchain)
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
-You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
+You can add a single or multiple dataset using `.add` and `.add_local` function and then use `.query` function to find an answer from the added datasets.
 
-If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
+If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, as well as a question and answer pair you supply, all you need to do is add the links to the videos, pdf and blog posts and the QnA pair and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
+# Embed Online Resources
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
 
+# Embed Local Resources
+naval_chat_bot.add_local("qna_pair", ("Who is Naval Ravikant?", "Naval Ravikant is an Indian-American entrepreneur and investor."))
+
 naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
@@ -64,18 +69,22 @@
 
 ```python
 
 from embedchain import App
 
 naval_ravikant_chat_bot_app = App()
 
+# Embed Online Resources
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
+
+# Embed Local Resources
+naval_chat_bot.add_local("qna_pair", ("Who is Naval Ravikant?", "Naval Ravikant is an Indian-American entrepreneur and investor."))
 ```
 
 * If there is any other app instance in your script or app, you can change the import as
 
 ```python
 from embedchain import App as EmbedChainApp
 
@@ -117,14 +126,22 @@
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
+### QnA Pair
+
+To supply your own QnA pair, use the data_type as `qna_pair` and enter a tuple. Eg:
+
+```python
+app.add_local('qna_pair', ("Question", "Answer"))
+```
+
 ### More Formats coming soon
 
 * If you want to add any other format, please create an [issue](https://github.com/embedchain/embedchain/issues) and we will add it to the list of supported formats.
 
 # How does it work?
 
 Creating a chat bot over any dataset needs the following steps to happen
```

### Comparing `embedchain-0.0.7/README.md` & `embedchain-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # embedchain
 
 [![](https://dcbadge.vercel.app/api/server/nhvCbCtKV?style=flat)](https://discord.gg/nhvCbCtKV)
+![PyPI](https://img.shields.io/pypi/v/embedchain)
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
-You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
+You can add a single or multiple dataset using `.add` and `.add_local` function and then use `.query` function to find an answer from the added datasets.
 
-If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
+If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, as well as a question and answer pair you supply, all you need to do is add the links to the videos, pdf and blog posts and the QnA pair and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
+# Embed Online Resources
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
 
+# Embed Local Resources
+naval_chat_bot.add_local("qna_pair", ("Who is Naval Ravikant?", "Naval Ravikant is an Indian-American entrepreneur and investor."))
+
 naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
@@ -50,18 +55,22 @@
 
 ```python
 
 from embedchain import App
 
 naval_ravikant_chat_bot_app = App()
 
+# Embed Online Resources
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
+
+# Embed Local Resources
+naval_chat_bot.add_local("qna_pair", ("Who is Naval Ravikant?", "Naval Ravikant is an Indian-American entrepreneur and investor."))
 ```
 
 * If there is any other app instance in your script or app, you can change the import as
 
 ```python
 from embedchain import App as EmbedChainApp
 
@@ -103,14 +112,22 @@
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
+### QnA Pair
+
+To supply your own QnA pair, use the data_type as `qna_pair` and enter a tuple. Eg:
+
+```python
+app.add_local('qna_pair', ("Question", "Answer"))
+```
+
 ### More Formats coming soon
 
 * If you want to add any other format, please create an [issue](https://github.com/embedchain/embedchain/issues) and we will add it to the list of supported formats.
 
 # How does it work?
 
 Creating a chat bot over any dataset needs the following steps to happen
```

### Comparing `embedchain-0.0.7/embedchain/chunkers/base_chunker.py` & `embedchain-0.0.8/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.7/embedchain/embedchain.py` & `embedchain-0.0.8/embedchain/embedchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from dotenv import load_dotenv
 from langchain.docstore.document import Document
 from langchain.embeddings.openai import OpenAIEmbeddings
 
 from embedchain.loaders.youtube_video import YoutubeVideoLoader
 from embedchain.loaders.pdf_file import PdfFileLoader
 from embedchain.loaders.web_page import WebPageLoader
+from embedchain.loaders.local_qna_pair import LocalQnaPairLoader
 from embedchain.chunkers.youtube_video import YoutubeVideoChunker
 from embedchain.chunkers.pdf_file import PdfFileChunker
 from embedchain.chunkers.web_page import WebPageChunker
+from embedchain.chunkers.qna_pair import QnaPairChunker
 from embedchain.vectordb.chroma_db import ChromaDB
 
 load_dotenv()
 
 embeddings = OpenAIEmbeddings()
 
 ABS_PATH = os.getcwd()
@@ -42,15 +44,16 @@
         :param data_type: The type of the data to load.
         :return: The loader for the given data type.
         :raises ValueError: If an unsupported data type is provided.
         """
         loaders = {
             'youtube_video': YoutubeVideoLoader(),
             'pdf_file': PdfFileLoader(),
-            'web_page': WebPageLoader()
+            'web_page': WebPageLoader(),
+            'qna_pair': LocalQnaPairLoader()
         }
         if data_type in loaders:
             return loaders[data_type]
         else:
             raise ValueError(f"Unsupported data type: {data_type}")
 
     def _get_chunker(self, data_type):
@@ -60,15 +63,16 @@
         :param data_type: The type of the data to chunk.
         :return: The chunker for the given data type.
         :raises ValueError: If an unsupported data type is provided.
         """
         chunkers = {
             'youtube_video': YoutubeVideoChunker(),
             'pdf_file': PdfFileChunker(),
-            'web_page': WebPageChunker()
+            'web_page': WebPageChunker(),
+            'qna_pair': QnaPairChunker(),
         }
         if data_type in chunkers:
             return chunkers[data_type]
         else:
             raise ValueError(f"Unsupported data type: {data_type}")
 
     def add(self, data_type, url):
@@ -81,14 +85,28 @@
         :param url: The URL where the data is located.
         """
         loader = self._get_loader(data_type)
         chunker = self._get_chunker(data_type)
         self.user_asks.append([data_type, url])
         self.load_and_embed(loader, chunker, url)
 
+    def add_local(self, data_type, content):
+        """
+        Adds the data you supply to the vector db.
+        Loads the data, chunks it, create embedding for each chunk
+        and then stores the embedding to vector database.
+
+        :param data_type: The type of the data to add.
+        :param content: The local data. Refer to the `README` for formatting.
+        """
+        loader = self._get_loader(data_type)
+        chunker = self._get_chunker(data_type)
+        self.user_asks.append([data_type, content])
+        self.load_and_embed(loader, chunker, content)
+
     def load_and_embed(self, loader, chunker, url):
         """
         Loads the data from the given URL, chunks it, and adds it to the database.
 
         :param loader: The loader to use to load the data.
         :param chunker: The chunker to use to chunk the data.
         :param url: The URL where the data is located.
@@ -141,47 +159,70 @@
             model="gpt-3.5-turbo-0613",
             messages=messages,
             temperature=0,
             max_tokens=1000,
             top_p=1,
         )
         return response["choices"][0]["message"]["content"]
+    
+    def retrieve_from_database(self, input_query):
+        """
+        Queries the vector database based on the given input query.
+        Gets relevant doc based on the query
 
-    def get_answer_from_llm(self, query, context):
+        :param input_query: The query to use.
+        :return: The content of the document that matched your query.
         """
-        Gets an answer based on the given query and context by passing it
-        to an LLM.
+        result = self.collection.query(
+            query_texts=[input_query,],
+            n_results=1,
+        )
+        result_formatted = self._format_result(result)
+        content = result_formatted[0][0].page_content
+        return content
+    
+    def generate_prompt(self, input_query, context):
+        """
+        Generates a prompt based on the given query and context, ready to be passed to an LLM
 
-        :param query: The query to use.
+        :param input_query: The query to use.
         :param context: Similar documents to the query used as context.
-        :return: The answer.
+        :return: The prompt
         """
         prompt = f"""Use the following pieces of context to answer the query at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
         {context}
-        Query: {query}
+        Query: {input_query}
         Helpful Answer:
         """
+        return prompt
+
+    def get_answer_from_llm(self, prompt):
+        """
+        Gets an answer based on the given query and context by passing it
+        to an LLM.
+
+        :param query: The query to use.
+        :param context: Similar documents to the query used as context.
+        :return: The answer.
+        """
         answer = self.get_openai_answer(prompt)
         return answer
 
     def query(self, input_query):
         """
         Queries the vector database based on the given input query.
         Gets relevant doc based on the query and then passes it to an
         LLM as context to get the answer.
 
         :param input_query: The query to use.
         :return: The answer to the query.
         """
-        result = self.collection.query(
-            query_texts=[input_query,],
-            n_results=1,
-        )
-        result_formatted = self._format_result(result)
-        answer = self.get_answer_from_llm(input_query, result_formatted[0][0].page_content)
+        context = self.retrieve_from_database(input_query)
+        prompt = self.generate_prompt(input_query, context)
+        answer = self.get_answer_from_llm(prompt)
         return answer
 
 
 class App(EmbedChain):
     """
     The EmbedChain app.
     Has two functions: add and query.
```

### Comparing `embedchain-0.0.7/embedchain/loaders/pdf_file.py` & `embedchain-0.0.8/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.7/embedchain/loaders/web_page.py` & `embedchain-0.0.8/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.7/embedchain/loaders/youtube_video.py` & `embedchain-0.0.8/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.7/embedchain.egg-info/PKG-INFO` & `embedchain-0.0.8/embedchain.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.7
+Version: 0.0.8
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
 
 [![](https://dcbadge.vercel.app/api/server/nhvCbCtKV?style=flat)](https://discord.gg/nhvCbCtKV)
+![PyPI](https://img.shields.io/pypi/v/embedchain)
 
 embedchain is a framework to easily create LLM powered bots over any dataset.
 
 It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
-You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
+You can add a single or multiple dataset using `.add` and `.add_local` function and then use `.query` function to find an answer from the added datasets.
 
-If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
+If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, as well as a question and answer pair you supply, all you need to do is add the links to the videos, pdf and blog posts and the QnA pair and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
 naval_chat_bot = App()
 
+# Embed Online Resources
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
 
+# Embed Local Resources
+naval_chat_bot.add_local("qna_pair", ("Who is Naval Ravikant?", "Naval Ravikant is an Indian-American entrepreneur and investor."))
+
 naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
 # answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
@@ -64,18 +69,22 @@
 
 ```python
 
 from embedchain import App
 
 naval_ravikant_chat_bot_app = App()
 
+# Embed Online Resources
 naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
 naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
 naval_chat_bot.add("web_page", "https://nav.al/feedback")
 naval_chat_bot.add("web_page", "https://nav.al/agi")
+
+# Embed Local Resources
+naval_chat_bot.add_local("qna_pair", ("Who is Naval Ravikant?", "Naval Ravikant is an Indian-American entrepreneur and investor."))
 ```
 
 * If there is any other app instance in your script or app, you can change the import as
 
 ```python
 from embedchain import App as EmbedChainApp
 
@@ -117,14 +126,22 @@
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
+### QnA Pair
+
+To supply your own QnA pair, use the data_type as `qna_pair` and enter a tuple. Eg:
+
+```python
+app.add_local('qna_pair', ("Question", "Answer"))
+```
+
 ### More Formats coming soon
 
 * If you want to add any other format, please create an [issue](https://github.com/embedchain/embedchain/issues) and we will add it to the list of supported formats.
 
 # How does it work?
 
 Creating a chat bot over any dataset needs the following steps to happen
```

### Comparing `embedchain-0.0.7/embedchain.egg-info/SOURCES.txt` & `embedchain-0.0.8/embedchain.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,13 +8,15 @@
 embedchain.egg-info/SOURCES.txt
 embedchain.egg-info/dependency_links.txt
 embedchain.egg-info/requires.txt
 embedchain.egg-info/top_level.txt
 embedchain/chunkers/__init__.py
 embedchain/chunkers/base_chunker.py
 embedchain/chunkers/pdf_file.py
+embedchain/chunkers/qna_pair.py
 embedchain/chunkers/web_page.py
 embedchain/chunkers/youtube_video.py
 embedchain/loaders/__init__.py
+embedchain/loaders/local_qna_pair.py
 embedchain/loaders/pdf_file.py
 embedchain/loaders/web_page.py
 embedchain/loaders/youtube_video.py
```

### Comparing `embedchain-0.0.7/setup.py` & `embedchain-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="embedchain",
-    version="0.0.7",
+    version="0.0.8",
     author="Taranjeet Singh",
     author_email="reachtotj@gmail.com",
     description="embedchain is a framework to easily create LLM powered bots over any dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/embedchain/embedchain",
     packages=setuptools.find_packages(),
```

