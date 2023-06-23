# Comparing `tmp/text2text-1.0.9.tar.gz` & `tmp/text2text-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.0.9.tar", last modified: Tue Jun 20 14:39:49 2023, max compression
+gzip compressed data, was "text2text-1.1.0.tar", last modified: Fri Jun 23 14:33:45 2023, max compression
```

## Comparing `text2text-1.0.9.tar` & `text2text-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.415699 text2text-1.0.9/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-20 14:28:32.000000 text2text-1.0.9/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60412 2023-06-20 14:39:49.414699 text2text-1.0.9/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59598 2023-06-20 14:37:55.000000 text2text-1.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 14:39:49.415699 text2text-1.0.9/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-20 14:38:43.000000 text2text-1.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.411698 text2text-1.0.9/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-06-20 14:34:46.000000 text2text-1.0.9/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.413699 text2text-1.0.9/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.414699 text2text-1.0.9/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-20 14:30:51.000000 text2text-1.0.9/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 14:28:32.000000 text2text-1.0.9/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:39:49.412699 text2text-1.0.9/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60412 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 14:39:49.000000 text2text-1.0.9/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.973021 text2text-1.1.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-23 14:21:46.000000 text2text-1.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    60408 2023-06-23 14:33:45.973021 text2text-1.1.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59594 2023-06-23 14:27:03.000000 text2text-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 14:33:45.973021 text2text-1.1.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-23 14:25:29.000000 text2text-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.970021 text2text-1.1.0/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-06-23 14:22:43.000000 text2text-1.1.0/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.971021 text2text-1.1.0/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.973021 text2text-1.1.0/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.971021 text2text-1.1.0/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60408 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.0.9/LICENSE.txt` & `text2text-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/PKG-INFO` & `text2text-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.9
+Version: 1.1.0
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements
 ```
 pip install -qq -U text2text
 ```
-* [Examples](#examples) can run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
+* [Examples](#examples) run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
```

### Comparing `text2text-1.0.9/README.md` & `text2text-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements
 ```
 pip install -qq -U text2text
 ```
-* [Examples](#examples) can run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
+* [Examples](#examples) run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
```

### Comparing `text2text-1.0.9/setup.py` & `text2text-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.0.9",
+  version="1.1.0",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.0.9/text2text/__init__.py` & `text2text-1.1.0/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/abstractor.py` & `text2text-1.1.0/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/answerer.py` & `text2text-1.1.0/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/assistant.py` & `text2text-1.1.0/text2text/assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import text2text as t2t
 from transformers import AutoTokenizer
 from auto_gptq import AutoGPTQForCausalLM
 
 class Assistant(t2t.Transformer):
 
   def __init__(self, **kwargs):
-    model_name_or_path = "TheBloke/vicuna-13b-v1.3-GPTQ"
-    model_basename = "vicuna-13b-v1.3-GPTQ-4bit-128g.no-act.order"
+    model_name_or_path = kwargs.get("model_name_or_path", "TheBloke/vicuna-13b-v1.3-GPTQ")
+    model_basename = kwargs.get("model_basename", "vicuna-13b-v1.3-GPTQ-4bit-128g.no-act.order")
 
     self.__class__.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, use_fast=True)
 
     self.__class__.model = AutoGPTQForCausalLM.from_quantized(model_name_or_path,
       model_basename=model_basename,
       use_safetensors=True,
       trust_remote_code=False,
```

### Comparing `text2text-1.0.9/text2text/biunilm/loader_utils.py` & `text2text-1.1.0/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/biunilm/seq2seq_loader.py` & `text2text-1.1.0/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/bm25er.py` & `text2text-1.1.0/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/counter.py` & `text2text-1.1.0/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/fitter.py` & `text2text-1.1.0/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/handler.py` & `text2text-1.1.0/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/identifier.py` & `text2text-1.1.0/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/indexer.py` & `text2text-1.1.0/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/measurer.py` & `text2text-1.1.0/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.1.0/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.1.0/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.1.0/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.1.0/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.1.0/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/questioner.py` & `text2text-1.1.0/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/responder.py` & `text2text-1.1.0/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/searcher.py` & `text2text-1.1.0/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/server.py` & `text2text-1.1.0/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/summarizer.py` & `text2text-1.1.0/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/tfidfer.py` & `text2text-1.1.0/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/tokenizer.py` & `text2text-1.1.0/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/transformer.py` & `text2text-1.1.0/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/translator.py` & `text2text-1.1.0/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text/vectorizer.py` & `text2text-1.1.0/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.0.9/text2text.egg-info/PKG-INFO` & `text2text-1.1.0/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.0.9
+Version: 1.1.0
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
 
 ## Installation Requirements
 ```
 pip install -qq -U text2text
 ```
-* [Examples](#examples) can run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
+* [Examples](#examples) run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
 [Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 Language Model Setting | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
```

### Comparing `text2text-1.0.9/text2text.egg-info/SOURCES.txt` & `text2text-1.1.0/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

