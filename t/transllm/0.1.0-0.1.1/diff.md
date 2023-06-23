# Comparing `tmp/transllm-0.1.0.tar.gz` & `tmp/transllm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transllm-0.1.0.tar", last modified: Fri Jun 23 09:45:15 2023, max compression
+gzip compressed data, was "transllm-0.1.1.tar", last modified: Fri Jun 23 09:53:32 2023, max compression
```

## Comparing `transllm-0.1.0.tar` & `transllm-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:45:15.926426 transllm-0.1.0/
--rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      972 2023-06-23 09:45:15.925418 transllm-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-06-23 09:35:17.000000 transllm-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 09:45:15.927425 transllm-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1891 2023-06-23 09:31:20.000000 transllm-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:45:15.908032 transllm-0.1.0/transllm/
--rw-rw-rw-   0        0        0      198 2023-06-23 09:44:59.000000 transllm-0.1.0/transllm/__init__.py
--rw-rw-rw-   0        0        0     5508 2023-06-23 09:44:19.000000 transllm-0.1.0/transllm/core.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:45:15.924037 transllm-0.1.0/transllm.egg-info/
--rw-rw-rw-   0        0        0      972 2023-06-23 09:45:15.000000 transllm-0.1.0/transllm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-23 09:45:15.000000 transllm-0.1.0/transllm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:45:15.000000 transllm-0.1.0/transllm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-23 09:45:15.000000 transllm-0.1.0/transllm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-06-23 09:45:15.000000 transllm-0.1.0/transllm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 09:45:15.000000 transllm-0.1.0/transllm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 09:53:32.921917 transllm-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      972 2023-06-23 09:53:32.920921 transllm-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-06-23 09:35:17.000000 transllm-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 09:53:32.922919 transllm-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1982 2023-06-23 09:52:59.000000 transllm-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:53:32.904725 transllm-0.1.1/transllm/
+-rw-rw-rw-   0        0        0      192 2023-06-23 09:53:10.000000 transllm-0.1.1/transllm/__init__.py
+-rw-rw-rw-   0        0        0     5528 2023-06-23 09:52:40.000000 transllm-0.1.1/transllm/core.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:53:32.919911 transllm-0.1.1/transllm.egg-info/
+-rw-rw-rw-   0        0        0      972 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/top_level.txt
```

### Comparing `transllm-0.1.0/LICENSE` & `transllm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transllm-0.1.0/PKG-INFO` & `transllm-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.0
+Version: 0.1.1
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `transllm-0.1.0/setup.py` & `transllm-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,42 @@
 
 
 version = get_version()
 
 
 setup(
     name="transllm",
-    version="0.1.0",
+    version="0.1.1",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="LLMtranslator translates and generates text in multiple languages.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=["requests", "deep_translator", "colorama", "httpx[http2]", "torch", "deepl", "transformers", "googletrans", "bardapi"],
+    install_requires=[
+        "requests",
+        "deep_translator",
+        "colorama",
+        "httpx[http2]",
+        "torch",
+        "deepl",
+        "transformers",
+        "googletrans",
+        "bardapi",
+    ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     entry_points={"console_scripts": ["transllm=transllm.cli:main"]},
-)
+)
```

### Comparing `transllm-0.1.0/transllm/core.py` & `transllm-0.1.1/transllm/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import deepl
 import openai
 from transformers import LlamaTokenizer, LlamaForCausalLM
 from googletrans import Translator
 from bardapi import Bard
 import re
 
+
 class LLMtranslator:
     """
     LLMtranslator is a translation and generation model that translates sentences into different languages and generates text based on the translated input.
 
     Args:
         model_path (str): The path or name of the pre-trained LLM model.
         target_lang (str, optional): The target language for translation. Defaults to 'ko'.
@@ -33,69 +34,81 @@
         translate_to_targetlang(text):
             Translates the given text to the target language.
 
         generate(prompt):
             Generates text based on the provided prompt and returns it in the target language.
     """
 
-    def __init__(self, model_path, target_lang='ko', translator='google', torch_dtype=torch.float16, device_map='auto', deepl_api=None, bard_api=None, openai_api=None, openai_model='gpt-3.5-turbo'):
+    def __init__(
+        self,
+        model_path,
+        target_lang="ko",
+        translator="google",
+        torch_dtype=torch.float16,
+        device_map="auto",
+        deepl_api=None,
+        bard_api=None,
+        openai_api=None,
+        openai_model="gpt-3.5-turbo",
+    ):
         self.model_path = model_path
         self.target_lang = target_lang
         self.tokenizer = LlamaTokenizer.from_pretrained(model_path)
-        self.model = LlamaForCausalLM.from_pretrained(model_path, torch_dtype=torch_dtype, device_map=device_map)
+        self.model = LlamaForCausalLM.from_pretrained(
+            model_path, torch_dtype=torch_dtype, device_map=device_map
+        )
         self.translator = translator
         self.bard_api = bard_api
         self.openai_api = openai_api
         self.deepl_api = deepl_api
         self.openai_model = openai_model
-        if self.translator == 'google':
+        if self.translator == "google":
             self.translator_obj = Translator()
-        elif self.translator == 'deepl':
+        elif self.translator == "deepl":
             self.translator_obj = deepl.Translator(self.deepl_api)
-        elif self.translator == 'bard':
+        elif self.translator == "bard":
             self.translator_obj = Bard(token=self.bard_api)
-            
 
     def translate(self, text: str, dest_lang: str) -> str:
         """
         Translates the given text to the specified destination language.
 
         Args:
             text (str): The text to be translated.
             dest_lang (str): The destination language code.
 
         Returns:
             str: The translated text in the specified language.
         """
-        if self.translator == 'google':
-            return self.translator_obj.translate(text, dest=dest_lang)
-        elif self.translator == 'deepl':
-            return self.translator_obj.translate_text(text, target_lang=dest_lang)
-        elif self.translator == 'bard':
-            translated = self.translator_obj.get_answer(f'{text}를 {dest_lang}로 번역해.')
+        if self.translator == "google":
+            return self.translator_obj.translate(text, dest=dest_lang).text
+        elif self.translator == "deepl":
+            return self.translator_obj.translate_text(text, target_lang=dest_lang).text
+        elif self.translator == "bard":
+            translated = self.translator_obj.get_answer(f"{text}를 {dest_lang}로 번역해.")['content']
             extracted_text = re.findall(r'"([^"]*)"', translated)
             return extracted_text[0]
-        elif self.translator == 'openai':
+        elif self.translator == "openai":
             response = openai.ChatCompletion.create(
-                                                    model=self.openai_model,
-                                                    messages=[{"role": "user", "content": f'{text}를 {dest_lang}으로 번역해'}]
-                                                    )
+                model=self.openai_model,
+                messages=[{"role": "user", "content": f"{text}를 {dest_lang}으로 번역해"}],
+            )
             return response
 
     def translate_to_en(self, text: str) -> str:
         """
         Translates the given text to English.
 
         Args:
             text (str): The text to be translated.
 
         Returns:
             str: The translated text in English.
         """
-        return self.translate(text, 'en')
+        return self.translate(text, "en")
 
     def translate_to_targetlang(self, text: str) -> str:
         """
         Translates the given text to the target language.
 
         Args:
             text (str): The text to be translated.
```

### Comparing `transllm-0.1.0/transllm.egg-info/PKG-INFO` & `transllm-0.1.1/transllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.0
+Version: 0.1.1
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

