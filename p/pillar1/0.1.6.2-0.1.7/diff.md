# Comparing `tmp/pillar1-0.1.6.2.tar.gz` & `tmp/pillar1-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.6.2.tar", last modified: Tue Jun 20 23:48:14 2023, max compression
+gzip compressed data, was "pillar1-0.1.7.tar", last modified: Fri Jun 23 13:36:45 2023, max compression
```

## Comparing `pillar1-0.1.6.2.tar` & `pillar1-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:48:14.386813 pillar1-0.1.6.2/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:48:14.386678 pillar1-0.1.6.2/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.6.2/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:48:14.385925 pillar1-0.1.6.2/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.6.2/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3047 2023-06-20 23:48:06.000000 pillar1-0.1.6.2/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 23:48:14.386490 pillar1-0.1.6.2/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 23:48:14.000000 pillar1-0.1.6.2/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 23:48:14.386856 pillar1-0.1.6.2/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 23:48:12.000000 pillar1-0.1.6.2/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:36:45.276310 pillar1-0.1.7/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-23 13:36:45.276177 pillar1-0.1.7/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:36:45.275278 pillar1-0.1.7/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3675 2023-06-23 13:33:48.000000 pillar1-0.1.7/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 13:36:45.275899 pillar1-0.1.7/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      202 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 13:36:45.000000 pillar1-0.1.7/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 13:36:45.276355 pillar1-0.1.7/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      619 2023-06-23 13:36:35.000000 pillar1-0.1.7/setup.py
```

### Comparing `pillar1-0.1.6.2/PKG-INFO` & `pillar1-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.6.2
+Version: 0.1.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.6.2/README.md` & `pillar1-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.6.2/pillar1/pillar1.py` & `pillar1-0.1.7/pillar1/pillar1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 import json
 import boto3
 import ipywidgets as widgets
 from IPython.display import display
 from pyspark.sql import SparkSession
+import constants as cn
+
+MODELS_META = {
+    'pillar1-f40b-instruct': {
+        'context': '',
+        'stop_token': '<|endoftext|>'
+    },
+    'starcoder-beta': {
+        'context': cn.STARCODER_BETA,
+        'prepend': '<|user|>',
+        'append': '(only return DataBricks-compatible SQL code)<|end|>',
+        'stop_token': '<|end|>'
+    }
+}
 
 
 class Model:
-    def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 200):
+    def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 200, verbose: bool = False):
         self.end_point = end_point
         self.prompt = None
         self.result = None
         self.cleaned_code = ''
         self.response = None
         self.max_new_tokens = max_new_tokens
+        self.verbose = verbose
 
         self.client = boto3.client(
             'sagemaker-runtime',
             aws_access_key_id=user_name,
             aws_secret_access_key=password,
             region_name='us-west-2'
         )
@@ -42,40 +57,44 @@
                 "parameters": {
                     "do_sample": True,
                     "top_p": 0.7,
                     "temperature": 0.7,
                     "top_k": 50,
                     "max_new_tokens": self.max_new_tokens,
                     "repetition_penalty": 1.03,
-                    "stop": ["<|endoftext|>"]
+                    "stop": [MODELS_META[self.end_point].get('stop_token')]
                 }
             }
 
+            if self.verbose:
+                print(f"Submit payload: {payload}")
+
             response = self.client.invoke_endpoint(
                 EndpointName=self.end_point,
                 ContentType='application/json',
                 Body=json.dumps(payload)
             )
 
             self.response = json.loads(response['Body'].read())[0]['generated_text']
             self.code()
 
         if prompt:
             self.prompt = prompt
             submit_request(self.prompt)
         else:
-            textarea_bg = widgets.Textarea(description='Provide any necessary background:', layout=widgets.Layout(width='80%', height='200px'),
-                                           style={'description_width': 'initial'})
+            # textarea_bg = widgets.Textarea(description='Provide any necessary background:', layout=widgets.Layout(width='80%', height='200px'),
+            #                                style={'description_width': 'initial'})
             input_text = widgets.Text(description='What SQL are you looking for:', layout=widgets.Layout(width='80%'), style={'description_width': 'initial'})
             button = widgets.Button(description='Submit')
-            display(textarea_bg)
+            # display(textarea_bg)
             display(input_text)
             display(button)
 
             # Define button click event
             def submit_button(b):
-                prompt = f"Given this background:\n\"{textarea_bg.value}\"\n\nAnswer this question: \"{input_text.value}\"; only provide the SQL code and nothing else:"
+                prompt = f"{MODELS_META[self.end_point].get('prepend', '')}Given this background:\n\"{MODELS_META[self.end_point].get('context', '')}\"\n\nAnswer this question: " \
+                         f"\"{input_text.value}\" {MODELS_META[self.end_point].get('append', '')}"
                 self.prompt = prompt
                 submit_request(prompt)
 
             # Bind button click event to function
             button.on_click(submit_button)
```

### Comparing `pillar1-0.1.6.2/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.7/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.6.2
+Version: 0.1.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.6.2/setup.py` & `pillar1-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.6.2',
+    version='0.1.7',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

