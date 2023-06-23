# Comparing `tmp/transllm-0.1.4.tar.gz` & `tmp/transllm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transllm-0.1.4.tar", last modified: Fri Jun 23 10:38:39 2023, max compression
+gzip compressed data, was "transllm-0.1.5.tar", last modified: Fri Jun 23 10:54:59 2023, max compression
```

## Comparing `transllm-0.1.4.tar` & `transllm-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:39.377061 transllm-0.1.4/
--rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6166 2023-06-23 10:38:39.375694 transllm-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5227 2023-06-23 10:20:39.000000 transllm-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 10:38:39.377061 transllm-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2037 2023-06-23 10:38:13.000000 transllm-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:39.361607 transllm-0.1.4/transllm/
--rw-rw-rw-   0        0        0      192 2023-06-23 10:38:05.000000 transllm-0.1.4/transllm/__init__.py
--rw-rw-rw-   0        0        0     5528 2023-06-23 09:52:40.000000 transllm-0.1.4/transllm/core.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:38:39.374615 transllm-0.1.4/transllm.egg-info/
--rw-rw-rw-   0        0        0     6166 2023-06-23 10:38:39.000000 transllm-0.1.4/transllm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-23 10:38:39.000000 transllm-0.1.4/transllm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 10:38:39.000000 transllm-0.1.4/transllm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-23 10:38:39.000000 transllm-0.1.4/transllm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-06-23 10:38:39.000000 transllm-0.1.4/transllm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 10:38:39.000000 transllm-0.1.4/transllm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 10:54:59.021558 transllm-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6197 2023-06-23 10:54:59.020559 transllm-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5258 2023-06-23 10:49:39.000000 transllm-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 10:54:59.021558 transllm-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2037 2023-06-23 10:54:48.000000 transllm-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:54:58.999569 transllm-0.1.5/transllm/
+-rw-rw-rw-   0        0        0      192 2023-06-23 10:54:46.000000 transllm-0.1.5/transllm/__init__.py
+-rw-rw-rw-   0        0        0     5718 2023-06-23 10:54:29.000000 transllm-0.1.5/transllm/core.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:54:59.017557 transllm-0.1.5/transllm.egg-info/
+-rw-rw-rw-   0        0        0     6197 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 10:54:58.000000 transllm-0.1.5/transllm.egg-info/top_level.txt
```

### Comparing `transllm-0.1.4/LICENSE` & `transllm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `transllm-0.1.4/PKG-INFO` & `transllm-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.4
+Version: 0.1.5
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -30,14 +30,16 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
 > LLMtranslator translates and generates text in multiple languages.
 
+![](assets/hf-transllm.png)
+
 Through the inference module of Hugging Face, you can conveniently use the results of Hugging Face's open-source large language model. However, there are limitations in retraining or evaluating the model's performance in various languages.
 
 Therefore, this package allows you to explore the results of the Hugging Face inference module in multiple languages using various trnaslated_answer API services.
 
 Since the purpose of the Hugging Face inference module is more focused on checking the model weights easily rather than efficiency, this package emphasizes the ability to explore the results in various languages rather than efficiency.
 
 
@@ -59,15 +61,15 @@
 ```
 
 <br>
 
 <br>
 
 ## Usage 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
 
 Simple Usage
 
 - Google Trnaslator
 ```python
 from transllm import LLMtranslator
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.4 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.5 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -12,32 +12,32 @@
 Intelligence Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Development Status :: 3 - Alpha # Python Package: hf-
 transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
-> LLMtranslator translates and generates text in multiple languages. Through
-the inference module of Hugging Face, you can conveniently use the results of
-Hugging Face's open-source large language model. However, there are limitations
-in retraining or evaluating the model's performance in various languages.
-Therefore, this package allows you to explore the results of the Hugging Face
-inference module in multiple languages using various trnaslated_answer API
-services. Since the purpose of the Hugging Face inference module is more
-focused on checking the model weights easily rather than efficiency, this
-package emphasizes the ability to explore the results in various languages
-rather than efficiency.
+> LLMtranslator translates and generates text in multiple languages. ![]
+(assets/hf-transllm.png) Through the inference module of Hugging Face, you can
+conveniently use the results of Hugging Face's open-source large language
+model. However, there are limitations in retraining or evaluating the model's
+performance in various languages. Therefore, this package allows you to explore
+the results of the Hugging Face inference module in multiple languages using
+various trnaslated_answer API services. Since the purpose of the Hugging Face
+inference module is more focused on checking the model weights easily rather
+than efficiency, this package emphasizes the ability to explore the results in
+various languages rather than efficiency.
 
 ## Install ``` pip install transllm ``` If you wish to use the various features
 and CLI: ``` pip install git+https://github.com/dsdanielpark/hf-transllm.git cd
 hf-transllm python main.py ```
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) Simple Usage - Google Trnaslator
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Simple Usage - Google Trnaslator
 ```python from transllm import LLMtranslator # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
 open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
 Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
 translator='google') # Using Prompt in multi-language prompt = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
 trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
```

### Comparing `transllm-0.1.4/README.md` & `transllm-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
 > LLMtranslator translates and generates text in multiple languages.
 
+![](assets/hf-transllm.png)
+
 Through the inference module of Hugging Face, you can conveniently use the results of Hugging Face's open-source large language model. However, there are limitations in retraining or evaluating the model's performance in various languages.
 
 Therefore, this package allows you to explore the results of the Hugging Face inference module in multiple languages using various trnaslated_answer API services.
 
 Since the purpose of the Hugging Face inference module is more focused on checking the model weights easily rather than efficiency, this package emphasizes the ability to explore the results in various languages rather than efficiency.
 
 
@@ -37,15 +39,15 @@
 ```
 
 <br>
 
 <br>
 
 ## Usage 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
 
 Simple Usage
 
 - Google Trnaslator
 ```python
 from transllm import LLMtranslator
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
 Development Status :: 3 - Alpha # Python Package: hf-transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
-> LLMtranslator translates and generates text in multiple languages. Through
-the inference module of Hugging Face, you can conveniently use the results of
-Hugging Face's open-source large language model. However, there are limitations
-in retraining or evaluating the model's performance in various languages.
-Therefore, this package allows you to explore the results of the Hugging Face
-inference module in multiple languages using various trnaslated_answer API
-services. Since the purpose of the Hugging Face inference module is more
-focused on checking the model weights easily rather than efficiency, this
-package emphasizes the ability to explore the results in various languages
-rather than efficiency.
+> LLMtranslator translates and generates text in multiple languages. ![]
+(assets/hf-transllm.png) Through the inference module of Hugging Face, you can
+conveniently use the results of Hugging Face's open-source large language
+model. However, there are limitations in retraining or evaluating the model's
+performance in various languages. Therefore, this package allows you to explore
+the results of the Hugging Face inference module in multiple languages using
+various trnaslated_answer API services. Since the purpose of the Hugging Face
+inference module is more focused on checking the model weights easily rather
+than efficiency, this package emphasizes the ability to explore the results in
+various languages rather than efficiency.
 
 ## Install ``` pip install transllm ``` If you wish to use the various features
 and CLI: ``` pip install git+https://github.com/dsdanielpark/hf-transllm.git cd
 hf-transllm python main.py ```
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) Simple Usage - Google Trnaslator
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Simple Usage - Google Trnaslator
 ```python from transllm import LLMtranslator # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
 open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
 Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
 translator='google') # Using Prompt in multi-language prompt = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
 trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
```

### Comparing `transllm-0.1.4/setup.py` & `transllm-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="transllm",
-    version="0.1.4",
+    version="0.1.5",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="LLMtranslator translates and generates text in multiple languages.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
```

### Comparing `transllm-0.1.4/transllm/core.py` & `transllm-0.1.5/transllm/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,19 +76,24 @@
             text (str): The text to be translated.
             dest_lang (str): The destination language code.
 
         Returns:
             str: The translated text in the specified language.
         """
         if self.translator == "google":
-            return self.translator_obj.translate(text, dest=dest_lang).text
+            translator = self.translator_obj
+            translated = translator.translate(text, dest=dest_lang)
+            return translated.text
         elif self.translator == "deepl":
-            return self.translator_obj.translate_text(text, target_lang=dest_lang).text
+            translator = self.translator_obj
+            translated = translator.translate_text(text, target_lang=dest_lang).text
+            return translated.text
         elif self.translator == "bard":
-            translated = self.translator_obj.get_answer(f"{text}를 {dest_lang}로 번역해.")['content']
+            translator = self.translator_obj
+            translated = translator.get_answer(f"{text}를 {dest_lang}로 번역해.")['content']
             extracted_text = re.findall(r'"([^"]*)"', translated)
             return extracted_text[0]
         elif self.translator == "openai":
             response = openai.ChatCompletion.create(
                 model=self.openai_model,
                 messages=[{"role": "user", "content": f"{text}를 {dest_lang}으로 번역해"}],
             )
```

### Comparing `transllm-0.1.4/transllm.egg-info/PKG-INFO` & `transllm-0.1.5/transllm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.4
+Version: 0.1.5
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -30,14 +30,16 @@
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
 <a href="https://pypi.org/project/transllm/"><img alt="PyPI" src="https://img.shields.io/pypi/v/transllm"></a>
 </p>
 
 
 > LLMtranslator translates and generates text in multiple languages.
 
+![](assets/hf-transllm.png)
+
 Through the inference module of Hugging Face, you can conveniently use the results of Hugging Face's open-source large language model. However, there are limitations in retraining or evaluating the model's performance in various languages.
 
 Therefore, this package allows you to explore the results of the Hugging Face inference module in multiple languages using various trnaslated_answer API services.
 
 Since the purpose of the Hugging Face inference module is more focused on checking the model weights easily rather than efficiency, this package emphasizes the ability to explore the results in various languages rather than efficiency.
 
 
@@ -59,15 +61,15 @@
 ```
 
 <br>
 
 <br>
 
 ## Usage 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) 
 
 Simple Usage
 
 - Google Trnaslator
 ```python
 from transllm import LLMtranslator
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.4 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.5 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -12,32 +12,32 @@
 Intelligence Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Development Status :: 3 - Alpha # Python Package: hf-
 transllm
 [PyPI package] [Code_style:_black] [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2Fhf-
 transllm&count_bg=%23000000&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false]
 [PyPI]
-> LLMtranslator translates and generates text in multiple languages. Through
-the inference module of Hugging Face, you can conveniently use the results of
-Hugging Face's open-source large language model. However, there are limitations
-in retraining or evaluating the model's performance in various languages.
-Therefore, this package allows you to explore the results of the Hugging Face
-inference module in multiple languages using various trnaslated_answer API
-services. Since the purpose of the Hugging Face inference module is more
-focused on checking the model weights easily rather than efficiency, this
-package emphasizes the ability to explore the results in various languages
-rather than efficiency.
+> LLMtranslator translates and generates text in multiple languages. ![]
+(assets/hf-transllm.png) Through the inference module of Hugging Face, you can
+conveniently use the results of Hugging Face's open-source large language
+model. However, there are limitations in retraining or evaluating the model's
+performance in various languages. Therefore, this package allows you to explore
+the results of the Hugging Face inference module in multiple languages using
+various trnaslated_answer API services. Since the purpose of the Hugging Face
+inference module is more focused on checking the model weights easily rather
+than efficiency, this package emphasizes the ability to explore the results in
+various languages rather than efficiency.
 
 ## Install ``` pip install transllm ``` If you wish to use the various features
 and CLI: ``` pip install git+https://github.com/dsdanielpark/hf-transllm.git cd
 hf-transllm python main.py ```
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
-1zzzlTIh0kt2MdjLzvXRby1rWbHzmog8t?usp=sharing) Simple Usage - Google Trnaslator
+1117ikGEmU4FncBDl1xCC2IhPPDOr75lX?usp=sharing) Simple Usage - Google Trnaslator
 ```python from transllm import LLMtranslator # Set huggingface repository
 model_path = 'openlm-research/open_llama_3b' # model_path = 'openlm-research/
 open_llama_7b' # model_path = 'openlm-research/open_llama_13b' # Get TransLLM
 Object open_llama3b_kor = LLMtranslator(model_path, target_lang='ko',
 translator='google') # Using Prompt in multi-language prompt = "ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤"
 trnaslated_answer = open_llama3b_kor.generate(prompt) print(trnaslated_answer)
```

