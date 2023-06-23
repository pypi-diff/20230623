# Comparing `tmp/chatgpt-cli-langchain-0.2.tar.gz` & `tmp/chatgpt-cli-langchain-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-cli-langchain-0.2.tar", last modified: Fri Jun 23 16:00:48 2023, max compression
+gzip compressed data, was "chatgpt-cli-langchain-0.3.tar", last modified: Fri Jun 23 16:07:45 2023, max compression
```

## Comparing `chatgpt-cli-langchain-0.2.tar` & `chatgpt-cli-langchain-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 16:00:48.052349 chatgpt-cli-langchain-0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 chatgpt-cli-langchain-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      775 2023-06-23 16:00:48.054354 chatgpt-cli-langchain-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 chatgpt-cli-langchain-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 16:00:47.980343 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/
--rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/__init__.py
--rw-rw-rw-   0        0        0       64 2023-06-23 15:58:35.000000 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/__main__.py
--rw-rw-rw-   0        0        0     2849 2023-06-23 15:37:07.000000 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/chat.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:00:48.049343 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/
--rw-rw-rw-   0        0        0      775 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      359 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-23 16:00:48.078345 chatgpt-cli-langchain-0.2/setup.cfg
--rw-rw-rw-   0        0        0     2081 2023-06-23 16:00:42.000000 chatgpt-cli-langchain-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:07:45.089784 chatgpt-cli-langchain-0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 chatgpt-cli-langchain-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      775 2023-06-23 16:07:45.090785 chatgpt-cli-langchain-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 chatgpt-cli-langchain-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 16:07:45.039783 chatgpt-cli-langchain-0.3/chatgpt-cli-langchain/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 chatgpt-cli-langchain-0.3/chatgpt-cli-langchain/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-06-23 15:58:35.000000 chatgpt-cli-langchain-0.3/chatgpt-cli-langchain/__main__.py
+-rw-rw-rw-   0        0        0     2849 2023-06-23 16:06:27.000000 chatgpt-cli-langchain-0.3/chatgpt-cli-langchain/chat.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:07:45.087783 chatgpt-cli-langchain-0.3/chatgpt_cli_langchain.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-06-23 16:07:44.000000 chatgpt-cli-langchain-0.3/chatgpt_cli_langchain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-23 16:07:44.000000 chatgpt-cli-langchain-0.3/chatgpt_cli_langchain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:07:44.000000 chatgpt-cli-langchain-0.3/chatgpt_cli_langchain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      359 2023-06-23 16:07:44.000000 chatgpt-cli-langchain-0.3/chatgpt_cli_langchain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-23 16:07:44.000000 chatgpt-cli-langchain-0.3/chatgpt_cli_langchain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-23 16:07:45.095780 chatgpt-cli-langchain-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2081 2023-06-23 16:07:40.000000 chatgpt-cli-langchain-0.3/setup.py
```

### Comparing `chatgpt-cli-langchain-0.2/LICENSE.txt` & `chatgpt-cli-langchain-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/chat.py` & `chatgpt-cli-langchain-0.3/chatgpt-cli-langchain/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-langchain-0.2/setup.py` & `chatgpt-cli-langchain-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'chatgpt-cli-langchain',         # How you named your package folder (MyLib)
   packages = ['chatgpt-cli-langchain'],   # Chose the same as "name"
-  version = '0.2',      # Start with a small number and increase it with every change you make
+  version = '0.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Simple CLI interface for ChatGPT',   # Give a short description about your library
   author = 'Raffaele Spataro',                   # Type in your name
   author_email = 'raffaele2692@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/raphael2692/chatgpt-cli-langchain',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_02.tar.gz',    # I explain this later on
   keywords = ['CHAT', 'GPT', 'CLI'],   # Keywords that define your package best
```

