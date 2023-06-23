# Comparing `tmp/me_gpt-0.0.7.tar.gz` & `tmp/me_gpt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\me_gpt-0.0.7.tar", last modified: Fri Jun 23 20:43:59 2023, max compression
+gzip compressed data, was "dist\me_gpt-0.0.8.tar", last modified: Fri Jun 23 20:54:41 2023, max compression
```

## Comparing `me_gpt-0.0.7.tar` & `me_gpt-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 20:43:59.037295 me_gpt-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-06-22 15:12:34.000000 me_gpt-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3560 2023-06-23 20:43:59.035295 me_gpt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3003 2023-06-23 20:42:29.000000 me_gpt-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 20:43:59.022295 me_gpt-0.0.7/me_gpt/
--rw-rw-rw-   0        0        0       62 2023-06-23 19:59:41.000000 me_gpt-0.0.7/me_gpt/__init__.py
--rw-rw-rw-   0        0        0     9823 2023-06-23 20:37:27.000000 me_gpt-0.0.7/me_gpt/ai.py
--rw-rw-rw-   0        0        0     4841 2023-06-23 19:59:21.000000 me_gpt-0.0.7/me_gpt/db.py
--rw-rw-rw-   0        0        0      416 2023-06-23 20:00:05.000000 me_gpt-0.0.7/me_gpt/example.py
--rw-rw-rw-   0        0        0     1509 2023-06-23 19:58:17.000000 me_gpt-0.0.7/me_gpt/similarity.py
-drwxrwxrwx   0        0        0        0 2023-06-23 20:43:59.033298 me_gpt-0.0.7/me_gpt.egg-info/
--rw-rw-rw-   0        0        0     3560 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 20:43:59.037295 me_gpt-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-06-23 20:40:42.000000 me_gpt-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:54:41.636569 me_gpt-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-22 15:12:34.000000 me_gpt-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3576 2023-06-23 20:54:41.635569 me_gpt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3019 2023-06-23 20:51:43.000000 me_gpt-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 20:54:41.622569 me_gpt-0.0.8/me_gpt/
+-rw-rw-rw-   0        0        0       63 2023-06-23 20:51:59.000000 me_gpt-0.0.8/me_gpt/__init__.py
+-rw-rw-rw-   0        0        0     9824 2023-06-23 20:53:00.000000 me_gpt-0.0.8/me_gpt/ai.py
+-rw-rw-rw-   0        0        0     4842 2023-06-23 20:52:46.000000 me_gpt-0.0.8/me_gpt/db.py
+-rw-rw-rw-   0        0        0      414 2023-06-23 20:53:39.000000 me_gpt-0.0.8/me_gpt/example.py
+-rw-rw-rw-   0        0        0     1509 2023-06-23 19:58:17.000000 me_gpt-0.0.8/me_gpt/similarity.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:54:41.632570 me_gpt-0.0.8/me_gpt.egg-info/
+-rw-rw-rw-   0        0        0     3576 2023-06-23 20:54:41.000000 me_gpt-0.0.8/me_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-23 20:54:41.000000 me_gpt-0.0.8/me_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:54:41.000000 me_gpt-0.0.8/me_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-23 20:54:41.000000 me_gpt-0.0.8/me_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 20:54:41.000000 me_gpt-0.0.8/me_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:54:41.636569 me_gpt-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-06-23 20:54:19.000000 me_gpt-0.0.8/setup.py
```

### Comparing `me_gpt-0.0.7/LICENSE` & `me_gpt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `me_gpt-0.0.7/PKG-INFO` & `me_gpt-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_gpt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to clone yourself with the help of GPT
 Author: Daniel J. McDonald
 Author-email: <daniel@danielmcdonald.dev>
 Keywords: python,gpt,openai,ai,chatbot,clone
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -44,21 +44,21 @@
 
 # initial questions to help your clone get started:
 initial_questions()
 
 # have your clone ask you more questions:
 more_questions(number_of_questions=3)
 
-# chat with your clone:
-chat_with_clone()
-
 # ask your clone a question and any instructions you'd like to give:
 question = "What is your Name?"
 instructions = "Give your answer with a pirate accent."
 print(prompt_memory(question, instructions))
+
+# chat with your clone in the terminal:
+chat_with_clone()
 ```
 
 ## Key Features:
 
 1. Memory Storage: Store memories, experiences, and information in a local vector database with ease. Capture the essence of your persona and knowledge, creating a treasure trove of data for Chat GPT to tap into.
 
 2. Self-Cloning Capability: Empower Chat GPT to clone your personality and knowledge using the memories stored in the vector database. Witness the remarkable transformation as Chat GPT adapts to your unique style, preferences, and expertise.
```

### Comparing `me_gpt-0.0.7/README.md` & `me_gpt-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 
 # initial questions to help your clone get started:
 initial_questions()
 
 # have your clone ask you more questions:
 more_questions(number_of_questions=3)
 
-# chat with your clone:
-chat_with_clone()
-
 # ask your clone a question and any instructions you'd like to give:
 question = "What is your Name?"
 instructions = "Give your answer with a pirate accent."
 print(prompt_memory(question, instructions))
+
+# chat with your clone in the terminal:
+chat_with_clone()
 ```
 
 ## Key Features:
 
 1. Memory Storage: Store memories, experiences, and information in a local vector database with ease. Capture the essence of your persona and knowledge, creating a treasure trove of data for Chat GPT to tap into.
 
 2. Self-Cloning Capability: Empower Chat GPT to clone your personality and knowledge using the memories stored in the vector database. Witness the remarkable transformation as Chat GPT adapts to your unique style, preferences, and expertise.
```

### Comparing `me_gpt-0.0.7/me_gpt/ai.py` & `me_gpt-0.0.8/me_gpt/ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import openai
 from dotenv import load_dotenv
 import re
 import os
 import uuid
 import json
-from db import DB
+from .db import DB
 
 
 # load the .env file:
 load_dotenv()
 OPEN_AI_API_KEY = os.getenv("OPEN_AI_API_KEY")
```

### Comparing `me_gpt-0.0.7/me_gpt/db.py` & `me_gpt-0.0.8/me_gpt/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle
 import numpy as np
 import gzip
 import openai
-from similarity import cosine_similarity, euclidean_metric, derridaean_similarity, adams_similarity, SVM_ranking_algorithm_sort
+from .similarity import cosine_similarity, euclidean_metric, derridaean_similarity, adams_similarity, SVM_ranking_algorithm_sort
 
 def get_embedding(documents, key=None, model="text-embedding-ada-002"):
     """Default embedding function that uses OpenAI Embeddings."""
     if isinstance(documents, list):
         if isinstance(documents[0], dict):
             texts = []
             if isinstance(key, str):
```

### Comparing `me_gpt-0.0.7/me_gpt/similarity.py` & `me_gpt-0.0.8/me_gpt/similarity.py`

 * *Files identical despite different names*

### Comparing `me_gpt-0.0.7/me_gpt.egg-info/PKG-INFO` & `me_gpt-0.0.8/me_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-gpt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to clone yourself with the help of GPT
 Author: Daniel J. McDonald
 Author-email: <daniel@danielmcdonald.dev>
 Keywords: python,gpt,openai,ai,chatbot,clone
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -44,21 +44,21 @@
 
 # initial questions to help your clone get started:
 initial_questions()
 
 # have your clone ask you more questions:
 more_questions(number_of_questions=3)
 
-# chat with your clone:
-chat_with_clone()
-
 # ask your clone a question and any instructions you'd like to give:
 question = "What is your Name?"
 instructions = "Give your answer with a pirate accent."
 print(prompt_memory(question, instructions))
+
+# chat with your clone in the terminal:
+chat_with_clone()
 ```
 
 ## Key Features:
 
 1. Memory Storage: Store memories, experiences, and information in a local vector database with ease. Capture the essence of your persona and knowledge, creating a treasure trove of data for Chat GPT to tap into.
 
 2. Self-Cloning Capability: Empower Chat GPT to clone your personality and knowledge using the memories stored in the vector database. Witness the remarkable transformation as Chat GPT adapts to your unique style, preferences, and expertise.
```

### Comparing `me_gpt-0.0.7/setup.py` & `me_gpt-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A python package to clone yourself with the help of GPT'
 LONG_DESCRIPTION = 'A python package to clone yourself with the help of GPT'
 
 # Setting up
 setup(
     name="me_gpt",
     version=VERSION,
     author="Daniel J. McDonald",
     author_email="<daniel@danielmcdonald.dev>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['openai', 'python-dotenv'],
+    install_requires=['openai', 'python-dotenv', 'numpy'],
     keywords=['python', 'gpt', 'openai', 'ai', 'chatbot', 'clone'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ]
```

