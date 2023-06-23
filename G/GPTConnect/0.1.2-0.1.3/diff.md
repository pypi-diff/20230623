# Comparing `tmp/GPTConnect-0.1.2.tar.gz` & `tmp/GPTConnect-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.2.tar", last modified: Fri Jun 23 13:49:56 2023, max compression
+gzip compressed data, was "GPTConnect-0.1.3.tar", last modified: Fri Jun 23 14:20:53 2023, max compression
```

## Comparing `GPTConnect-0.1.2.tar` & `GPTConnect-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:49:56.969889 GPTConnect-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-23 13:49:56.960889 GPTConnect-0.1.2/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0      131 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-06-23 13:49:56.968890 GPTConnect-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-06-23 12:40:28.000000 GPTConnect-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 13:49:56.965891 GPTConnect-0.1.2/gptconnect/
--rw-rw-rw-   0        0        0       27 2023-06-23 13:36:18.000000 GPTConnect-0.1.2/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-06-23 13:36:05.000000 GPTConnect-0.1.2/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0       42 2023-06-23 13:49:56.969889 GPTConnect-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      211 2023-06-23 13:49:52.000000 GPTConnect-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:20:53.505276 GPTConnect-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-23 14:20:53.497241 GPTConnect-0.1.3/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-06-23 14:20:53.000000 GPTConnect-0.1.3/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-23 14:20:53.000000 GPTConnect-0.1.3/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:20:53.000000 GPTConnect-0.1.3/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 14:20:53.000000 GPTConnect-0.1.3/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-06-23 14:20:53.504296 GPTConnect-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-23 14:20:28.000000 GPTConnect-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 14:20:53.501759 GPTConnect-0.1.3/gptconnect/
+-rw-rw-rw-   0        0        0       27 2023-06-23 13:36:18.000000 GPTConnect-0.1.3/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2605 2023-06-23 14:19:13.000000 GPTConnect-0.1.3/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:20:53.505276 GPTConnect-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      211 2023-06-23 14:20:28.000000 GPTConnect-0.1.3/setup.py
```

### Comparing `GPTConnect-0.1.2/README.md` & `GPTConnect-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,9 +4,12 @@
 
 ## Features
 
 - Simplified and intuitive decorator based system to define GPT functions.
 - Function groups system that allow easy integration of multiple commands at a time
 - More feautures coming soon! This package is only in early stages of development.
 
+## Install
+`pip install GPTConnect`
+
 ## Demo
 [demo.py](https://github.com/SleepyStew/gptconnect/blob/master/demo.py)
```

### Comparing `GPTConnect-0.1.2/gptconnect/gptconnect.py` & `GPTConnect-0.1.3/gptconnect/gptconnect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Union
 import openai
 import copy
 
-valid_models = ["gpt-3.5-turbo-0613", "gpt-4-32k-0613"]
+valid_models = ["gpt-3.5-turbo-0613", "gpt-4-0613", "gpt-4-32k-0613"]
 functions = []
 
 
 class GPTConnect:
     def __init__(self, token: str, model: str):
         openai.api_key = token
         if model not in valid_models:
```

