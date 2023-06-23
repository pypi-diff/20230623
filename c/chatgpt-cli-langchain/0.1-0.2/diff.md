# Comparing `tmp/chatgpt-cli-langchain-0.1.tar.gz` & `tmp/chatgpt-cli-langchain-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-cli-langchain-0.1.tar", last modified: Fri Jun 23 15:52:42 2023, max compression
+gzip compressed data, was "chatgpt-cli-langchain-0.2.tar", last modified: Fri Jun 23 16:00:48 2023, max compression
```

## Comparing `chatgpt-cli-langchain-0.1.tar` & `chatgpt-cli-langchain-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 15:52:42.314163 chatgpt-cli-langchain-0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 chatgpt-cli-langchain-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      775 2023-06-23 15:52:42.315164 chatgpt-cli-langchain-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 chatgpt-cli-langchain-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 15:52:42.205165 chatgpt-cli-langchain-0.1/chatgpt-cli-langchain/
--rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 chatgpt-cli-langchain-0.1/chatgpt-cli-langchain/__init__.py
--rw-rw-rw-   0        0        0     2849 2023-06-23 15:37:07.000000 chatgpt-cli-langchain-0.1/chatgpt-cli-langchain/chat.py
-drwxrwxrwx   0        0        0        0 2023-06-23 15:52:42.311166 chatgpt-cli-langchain-0.1/chatgpt_cli_langchain.egg-info/
--rw-rw-rw-   0        0        0      775 2023-06-23 15:52:41.000000 chatgpt-cli-langchain-0.1/chatgpt_cli_langchain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-23 15:52:42.000000 chatgpt-cli-langchain-0.1/chatgpt_cli_langchain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 15:52:41.000000 chatgpt-cli-langchain-0.1/chatgpt_cli_langchain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      359 2023-06-23 15:52:41.000000 chatgpt-cli-langchain-0.1/chatgpt_cli_langchain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-23 15:52:41.000000 chatgpt-cli-langchain-0.1/chatgpt_cli_langchain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-23 15:52:42.333165 chatgpt-cli-langchain-0.1/setup.cfg
--rw-rw-rw-   0        0        0     2081 2023-06-23 15:52:35.000000 chatgpt-cli-langchain-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:00:48.052349 chatgpt-cli-langchain-0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 chatgpt-cli-langchain-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      775 2023-06-23 16:00:48.054354 chatgpt-cli-langchain-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 chatgpt-cli-langchain-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 16:00:47.980343 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-06-23 15:58:35.000000 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/__main__.py
+-rw-rw-rw-   0        0        0     2849 2023-06-23 15:37:07.000000 chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/chat.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:00:48.049343 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      359 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-23 16:00:47.000000 chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-23 16:00:48.078345 chatgpt-cli-langchain-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2081 2023-06-23 16:00:42.000000 chatgpt-cli-langchain-0.2/setup.py
```

### Comparing `chatgpt-cli-langchain-0.1/LICENSE.txt` & `chatgpt-cli-langchain-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-langchain-0.1/PKG-INFO` & `chatgpt-cli-langchain-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-langchain
-Version: 0.1
+Version: 0.2
 Summary: Simple CLI interface for ChatGPT
 Home-page: https://github.com/raphael2692/chatgpt-cli-langchain
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_02.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `chatgpt-cli-langchain-0.1/chatgpt-cli-langchain/chat.py` & `chatgpt-cli-langchain-0.2/chatgpt-cli-langchain/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-langchain-0.1/chatgpt_cli_langchain.egg-info/PKG-INFO` & `chatgpt-cli-langchain-0.2/chatgpt_cli_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-langchain
-Version: 0.1
+Version: 0.2
 Summary: Simple CLI interface for ChatGPT
 Home-page: https://github.com/raphael2692/chatgpt-cli-langchain
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_02.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `chatgpt-cli-langchain-0.1/setup.py` & `chatgpt-cli-langchain-0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'chatgpt-cli-langchain',         # How you named your package folder (MyLib)
   packages = ['chatgpt-cli-langchain'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Simple CLI interface for ChatGPT',   # Give a short description about your library
   author = 'Raffaele Spataro',                   # Type in your name
   author_email = 'raffaele2692@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/raphael2692/chatgpt-cli-langchain',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/user/reponame/archive/v_02.tar.gz',    # I explain this later on
   keywords = ['CHAT', 'GPT', 'CLI'],   # Keywords that define your package best
   install_requires=
         ['aiohttp', 'aiosignal', 'async-timeout', 'attrs', 'certifi', 'charset-normalizer', 'colorama', 'dataclasses-json', 'frozenlist', 'greenlet', 'idna', 'langchain', 'langchainplus-sdk', 'marshmallow', 'marshmallow-enum', 'multidict', 'mypy-extensions', 'numexpr', 'numpy', 'openai', 'openapi-schema-pydantic', 'packaging', 'pydantic', 'pyfiglet', 'PyYAML', 'requests', 'SQLAlchemy', 'tenacity', 'tqdm', 'typing-inspect', 'typing_extensions', 'urllib3', 'yarl'],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

