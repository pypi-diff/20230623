# Comparing `tmp/transllm-0.1.2.tar.gz` & `tmp/transllm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transllm-0.1.2.tar", last modified: Fri Jun 23 10:22:28 2023, max compression
+gzip compressed data, was "transllm-0.1.3.tar", last modified: Fri Jun 23 10:25:25 2023, max compression
```

## Comparing `transllm-0.1.2.tar` & `transllm-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 10:22:28.879325 transllm-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6166 2023-06-23 10:22:28.879325 transllm-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5227 2023-06-23 10:20:39.000000 transllm-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 10:22:28.880324 transllm-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1970 2023-06-23 10:22:11.000000 transllm-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:22:28.863659 transllm-0.1.2/transllm/
--rw-rw-rw-   0        0        0      192 2023-06-23 10:22:14.000000 transllm-0.1.2/transllm/__init__.py
--rw-rw-rw-   0        0        0     5528 2023-06-23 09:52:40.000000 transllm-0.1.2/transllm/core.py
-drwxrwxrwx   0        0        0        0 2023-06-23 10:22:28.877325 transllm-0.1.2/transllm.egg-info/
--rw-rw-rw-   0        0        0     6166 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 10:25:25.682871 transllm-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6166 2023-06-23 10:25:25.682871 transllm-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5227 2023-06-23 10:20:39.000000 transllm-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 10:25:25.682871 transllm-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1988 2023-06-23 10:25:11.000000 transllm-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:25:25.668955 transllm-0.1.3/transllm/
+-rw-rw-rw-   0        0        0      192 2023-06-23 10:25:05.000000 transllm-0.1.3/transllm/__init__.py
+-rw-rw-rw-   0        0        0     5528 2023-06-23 09:52:40.000000 transllm-0.1.3/transllm/core.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:25:25.680870 transllm-0.1.3/transllm.egg-info/
+-rw-rw-rw-   0        0        0     6166 2023-06-23 10:25:25.000000 transllm-0.1.3/transllm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-23 10:25:25.000000 transllm-0.1.3/transllm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 10:25:25.000000 transllm-0.1.3/transllm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-23 10:25:25.000000 transllm-0.1.3/transllm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       99 2023-06-23 10:25:25.000000 transllm-0.1.3/transllm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 10:25:25.000000 transllm-0.1.3/transllm.egg-info/top_level.txt
```

### Comparing `transllm-0.1.2/LICENSE` & `transllm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transllm-0.1.2/PKG-INFO` & `transllm-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.2
+Version: 0.1.3
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.2 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.3 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `transllm-0.1.2/README.md` & `transllm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `transllm-0.1.2/setup.py` & `transllm-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="transllm",
-    version="0.1.2",
+    version="0.1.3",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="LLMtranslator translates and generates text in multiple languages.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
@@ -40,14 +40,15 @@
         "colorama",
         "httpx[http2]",
         "torch",
         "deepl",
         "transformers",
         "googletrans",
         "bardapi",
+        "openai"
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
```

### Comparing `transllm-0.1.2/transllm/core.py` & `transllm-0.1.3/transllm/core.py`

 * *Files identical despite different names*

### Comparing `transllm-0.1.2/transllm.egg-info/PKG-INFO` & `transllm-0.1.3/transllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transllm
-Version: 0.1.2
+Version: 0.1.3
 Summary: LLMtranslator translates and generates text in multiple languages.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transllm Version: 0.1.2 Summary: LLMtranslator
+Metadata-Version: 2.1 Name: transllm Version: 0.1.3 Summary: LLMtranslator
 translates and generates text in multiple languages. Home-page: https://
 github.com/dsdanielpark/hf-transllm Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Science/Research Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

