# Comparing `tmp/embedstore-0.0.5-py3-none-any.whl.zip` & `tmp/embedstore-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11305 bytes, number of entries: 11
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 16:49 embedstore/__init__.py
--rw-r--r--  2.0 unx     2548 b- defN 23-Jun-13 16:49 embedstore/helpers/api.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 16:49 embedstore/helpers/exceptions.py
--rw-r--r--  2.0 unx     1197 b- defN 23-Jun-13 16:49 embedstore/rag/datadownloaders.py
--rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 16:49 embedstore/rag/retrievers.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 16:49 embedstore/tools/factcheck.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    16916 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      907 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/RECORD
-11 files, 24264 bytes uncompressed, 9761 bytes compressed:  59.8%
+Zip file size: 11474 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-23 15:36 embedstore/__init__.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Jun-23 15:36 embedstore/helpers/api.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-23 15:36 embedstore/helpers/exceptions.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-23 15:36 embedstore/rag/datadownloaders.py
+-rw-r--r--  2.0 unx     1343 b- defN 23-Jun-23 15:36 embedstore/rag/retrievers.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 15:36 embedstore/tools/factcheck.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-23 15:36 embedstore-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17183 b- defN 23-Jun-23 15:36 embedstore-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 15:36 embedstore-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 15:36 embedstore-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      907 b- defN 23-Jun-23 15:36 embedstore-0.0.6.dist-info/RECORD
+11 files, 24546 bytes uncompressed, 9930 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: embedstore/rag/retrievers.py
 Comment: 
 
 Filename: embedstore/tools/factcheck.py
 Comment: 
 
-Filename: embedstore-0.0.5.dist-info/LICENSE
+Filename: embedstore-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: embedstore-0.0.5.dist-info/METADATA
+Filename: embedstore-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: embedstore-0.0.5.dist-info/WHEEL
+Filename: embedstore-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: embedstore-0.0.5.dist-info/top_level.txt
+Filename: embedstore-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: embedstore-0.0.5.dist-info/RECORD
+Filename: embedstore-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedstore/__init__.py

```diff
@@ -1,4 +1,4 @@
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## embedstore/rag/retrievers.py

```diff
@@ -3,15 +3,15 @@
 
 
 class EmbedStoreRetriever:
     """
     Base class for retreiver
     """
     def _validate_dataset_id(self,dataset_id):
-        available_dataset_id = ['podcasts_01','arxiv_01']
+        available_dataset_id = ['podcasts_01','arxiv_01','wikipedia_01']
         if dataset_id not in available_dataset_id:
             raise InvalidInput(f'Invalid dataset_id : Has to be one of the following - {available_dataset_id}')
     
     def __init__(self, dataset_id, num_docs, retrieving_method="similarity_score") -> None:
         """Init params."""
         self._validate_dataset_id(dataset_id)
         self.dataset_id = dataset_id
```

## Comparing `embedstore-0.0.5.dist-info/LICENSE` & `embedstore-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedstore-0.0.5.dist-info/METADATA` & `embedstore-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedstore
-Version: 0.0.5
+Version: 0.0.6
 Summary: Retrieving the most relevant context for your LLMs
 License: MIT License
         
         Copyright (c) Buidl Labs Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,15 +40,15 @@
   <p align="center">
     Context retrieval apis to power your LLMs! <br/>
     <a href="#quick-start"><strong>Get started »</strong></a>
   </p>
   <a href="https://pepy.tech/project/embedstore" alt="Downloads">
         <img src="https://static.pepy.tech/personalized-badge/embedstore?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/month" /></a>
   <a href="https://discord.com/invite/hAnE4e5T6M">
-    <img src="https://dcbadge.vercel.app/api/server/hAnE4e5T6M?style=flat" />
+    <img src="https://img.shields.io/discord/1111412701651013713?label=discord" />
   </a>
   <a>
     <img src="https://img.shields.io/github/license/embeddingstore/embedstore"/>
   </a>
   <p align="center">
     <br />
      <a href="https://colab.research.google.com/drive/1yhBhLmiPNtc06qVnjQRLsWuQDID3_cwl?usp=sharing">Try on Google Colab</a>
@@ -64,14 +64,16 @@
 ### Installation
 You have two ways to get started:
 1. Install our python library : `pip install embedstore`
 2. Directly call the endpoint : `https://api.embedding.store/retrieve`
 
 
 ### Get API Key [here](https://api.embedding.store/register)
+**Note:** Currently we are rate-limiting all API keys to 100 requests/day
+
 Set the `EMBEDSTORE_API_KEY` as environment variable
 ```python
 import os
 os.environ["EMBEDSTORE_API_KEY"] = <YOUR API KEY> 
 ```
 Pass the API key as header if you are calling the endpoint directly. More details about the [endpoint](#using-retrieve-endpoint)
 ```python
@@ -210,15 +212,15 @@
 
 ## Datasets
 
 | Dataset             | dataset_id | Description                                                     | Status      | Filters Available                                                                                                 |
 | ------------------- | ----------------------------- | --------------------------------------------------------------- | ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Podcast Transcripts | podcasts_01                   | 30 most recent podcasts across Finance, Business and Technology | Live        | - `category` : ["Finance","Business","Technology"]                                                                                                                                                                                                                                                 | 
 | arXiv               | arxiv_01                      | 2M arxiv papers                                               | Live        | - `category` : ['Computer Science', 'Quantitative Biology', 'Economics', 'Quantitative Finance', 'Statistics', 'Electrical Engineering and Systems Science', 'Mathematics', 'Physics']<br><br>- `publish_date_start` : To filter papers published after this date (string in `%Y-%m-%dT%H:%M:%SZ`)                                                                                                            |
-| Wikipedia                | wikipedia_01                                                                                     | Launching Soon - [Subscribe](http://embedding.store/) |                                                                                                                                                                                                                                                                                                      |       
+| Wikipedia                | wikipedia_01                                                                                     | 50K popular pages (get access to the full dataset [here](https://airtable.com/shrpp2iqmEjHp6h1M))     |     Live                                                                                                                                                                                                                                                                                               |     - `category` : ['Arts and Entertainment', 'Sports', 'People', 'Science and Technology', 'Geography', 'Politics and Government', 'History'] 
 | News                | news_01                                                                                     | Launching Soon - [Subscribe](http://embedding.store/) |                                                                                                                                                                                                                                                                                                      |       
 
 
 ## Get involved
 We are early, and we want to know how you use this library and what else would you want to make the most out of it.
 
 Join us on our [discord](https://discord.gg/hAnE4e5T6M), or feel free to email us at hello@embedding.store!
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedstore Version: 0.0.5 Summary: Retrieving the
+Metadata-Version: 2.1 Name: embedstore Version: 0.0.6 Summary: Retrieving the
 most relevant context for your LLMs License: MIT License Copyright (c) Buidl
 Labs Inc. Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
@@ -18,30 +18,31 @@
 requests (>=2)
                                     [Logo]
                              **** embedstore ****
                   Context retrieval apis to power your LLMs!
                                 Get_started_Â»
                  [https://static.pepy.tech/personalized-badge/
 embedstore?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/
-month] [https://dcbadge.vercel.app/api/server/hAnE4e5T6M?style=flat] [https://
-           img.shields.io/github/license/embeddingstore/embedstore]
+  month] [https://img.shields.io/discord/1111412701651013713?label=discord]
+       [https://img.shields.io/github/license/embeddingstore/embedstore]
 
         Try_on_Google_Colab â Test_API â Subscribe_for_Early_Access
 ## Quick start ### Installation You have two ways to get started: 1. Install
 our python library : `pip install embedstore` 2. Directly call the endpoint :
 `https://api.embedding.store/retrieve` ### Get API Key [here](https://
-api.embedding.store/register) Set the `EMBEDSTORE_API_KEY` as environment
-variable ```python import os os.environ["EMBEDSTORE_API_KEY"] =  ``` Pass the
-API key as header if you are calling the endpoint directly. More details about
-the [endpoint](#using-retrieve-endpoint) ```python headers = {'API-Key': } ```
-### Retrieve context In a few lines of code, you can now start retrieving
-relevant context to get better answers from your LLM. We have already embedded
-Podcast Transcripts and Arxiv Research Papers, with new dataset drops every
-week ([full list here](#datasets)) ```python from embedstore.rag.retrievers
-import EmbedStoreRetriever # Initialize the retriever arxiv_retriever =
+api.embedding.store/register) **Note:** Currently we are rate-limiting all API
+keys to 100 requests/day Set the `EMBEDSTORE_API_KEY` as environment variable
+```python import os os.environ["EMBEDSTORE_API_KEY"] =  ``` Pass the API key as
+header if you are calling the endpoint directly. More details about the
+[endpoint](#using-retrieve-endpoint) ```python headers = {'API-Key': } ``` ###
+Retrieve context In a few lines of code, you can now start retrieving relevant
+context to get better answers from your LLM. We have already embedded Podcast
+Transcripts and Arxiv Research Papers, with new dataset drops every week ([full
+list here](#datasets)) ```python from embedstore.rag.retrievers import
+EmbedStoreRetriever # Initialize the retriever arxiv_retriever =
 EmbedStoreRetriever(dataset_id = "arxiv_01", num_docs=3) # Query the retriever
 context = arxiv_retriever.query("What is the state of the art in Autonomous
 Driving security and safety?") # Examine the retrieved context and then append
 it to the prompt before you call your LLM print(context[0]) ``` Read more
 [here](#usage) for detailed usage guidelines. ## What is this? We are building
 context retrieval apis for developers creating chatbots, copilots and search
 tools on top of LLMs. You no longer need to maintain scraping and embedding
@@ -183,13 +184,15 @@
 across Finance, Business and Technology | Live | - `category` :
 ["Finance","Business","Technology"] | | arXiv | arxiv_01 | 2M arxiv papers |
 Live | - `category` : ['Computer Science', 'Quantitative Biology', 'Economics',
 'Quantitative Finance', 'Statistics', 'Electrical Engineering and Systems
 Science', 'Mathematics', 'Physics']
 
 - `publish_date_start` : To filter papers published after this date (string in
-`%Y-%m-%dT%H:%M:%SZ`) | | Wikipedia | wikipedia_01 | Launching Soon -
-[Subscribe](http://embedding.store/) | | | News | news_01 | Launching Soon -
-[Subscribe](http://embedding.store/) | | ## Get involved We are early, and we
-want to know how you use this library and what else would you want to make the
-most out of it. Join us on our [discord](https://discord.gg/hAnE4e5T6M), or
-feel free to email us at hello@embedding.store!
+`%Y-%m-%dT%H:%M:%SZ`) | | Wikipedia | wikipedia_01 | 50K popular pages (get
+access to the full dataset [here](https://airtable.com/shrpp2iqmEjHp6h1M)) |
+Live | - `category` : ['Arts and Entertainment', 'Sports', 'People', 'Science
+and Technology', 'Geography', 'Politics and Government', 'History'] | News |
+news_01 | Launching Soon - [Subscribe](http://embedding.store/) | | ## Get
+involved We are early, and we want to know how you use this library and what
+else would you want to make the most out of it. Join us on our [discord](https:
+//discord.gg/hAnE4e5T6M), or feel free to email us at hello@embedding.store!
```

## Comparing `embedstore-0.0.5.dist-info/RECORD` & `embedstore-0.0.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-embedstore/__init__.py,sha256=7pFryrckxVKBWVmohG01PF-JBbeEbsK_-Vbwt3wxoic,79
+embedstore/__init__.py,sha256=p0kzqGWjDzLiFWmv4_FzxLfVWs5haZFrsjA-J746IgA,79
 embedstore/helpers/api.py,sha256=fpLDfwSEMhawKSxR-ZdNyLpocNC6VLrwnGnSDLdvlx0,2548
 embedstore/helpers/exceptions.py,sha256=3ZonzI11hhrIgPuO5ua1veI8MWs3RCYrKcA3OEbatX0,120
 embedstore/rag/datadownloaders.py,sha256=CqSErYPjuU3qJ9WPTHm1WKR4xo10fnEu3STCjBlcclU,1197
-embedstore/rag/retrievers.py,sha256=FCHvNonpidZH9LeJwORxyuJoDi05BkZd-a2UcFUbhUc,1328
+embedstore/rag/retrievers.py,sha256=Lzc5DOkbPiHhCogD6cvt0h9KhAbkUb6DMuSicSgwhyY,1343
 embedstore/tools/factcheck.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-embedstore-0.0.5.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
-embedstore-0.0.5.dist-info/METADATA,sha256=WL2VuxCEJQSiggaWHR9m-tb8gUq4UeZB18gku9ViiRw,16916
-embedstore-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-embedstore-0.0.5.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
-embedstore-0.0.5.dist-info/RECORD,,
+embedstore-0.0.6.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
+embedstore-0.0.6.dist-info/METADATA,sha256=wzJtJoX5T3w5gF6XDimp4etUFbt90cahcJwo70c4WnY,17183
+embedstore-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+embedstore-0.0.6.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
+embedstore-0.0.6.dist-info/RECORD,,
```

