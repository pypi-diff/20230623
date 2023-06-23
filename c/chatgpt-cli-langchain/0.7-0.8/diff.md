# Comparing `tmp/chatgpt-cli-langchain-0.7.tar.gz` & `tmp/chatgpt-cli-langchain-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-cli-langchain-0.7.tar", last modified: Fri Jun 23 16:40:48 2023, max compression
+gzip compressed data, was "chatgpt-cli-langchain-0.8.tar", last modified: Fri Jun 23 16:44:06 2023, max compression
```

## Comparing `chatgpt-cli-langchain-0.7.tar` & `chatgpt-cli-langchain-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 16:40:48.345434 chatgpt-cli-langchain-0.7/
--rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 chatgpt-cli-langchain-0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      775 2023-06-23 16:40:48.346433 chatgpt-cli-langchain-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 chatgpt-cli-langchain-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 16:40:48.282426 chatgpt-cli-langchain-0.7/chatgpt-cli-langchain/
--rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 chatgpt-cli-langchain-0.7/chatgpt-cli-langchain/__init__.py
--rw-rw-rw-   0        0        0       55 2023-06-23 16:40:32.000000 chatgpt-cli-langchain-0.7/chatgpt-cli-langchain/__main__.py
--rw-rw-rw-   0        0        0     3993 2023-06-23 16:39:49.000000 chatgpt-cli-langchain-0.7/chatgpt-cli-langchain/chat.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:40:48.340433 chatgpt-cli-langchain-0.7/chatgpt_cli_langchain.egg-info/
--rw-rw-rw-   0        0        0      775 2023-06-23 16:40:47.000000 chatgpt-cli-langchain-0.7/chatgpt_cli_langchain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-23 16:40:48.000000 chatgpt-cli-langchain-0.7/chatgpt_cli_langchain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 16:40:47.000000 chatgpt-cli-langchain-0.7/chatgpt_cli_langchain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      359 2023-06-23 16:40:47.000000 chatgpt-cli-langchain-0.7/chatgpt_cli_langchain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-23 16:40:47.000000 chatgpt-cli-langchain-0.7/chatgpt_cli_langchain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-23 16:40:48.352427 chatgpt-cli-langchain-0.7/setup.cfg
--rw-rw-rw-   0        0        0     2081 2023-06-23 16:40:44.000000 chatgpt-cli-langchain-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:44:06.931321 chatgpt-cli-langchain-0.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 chatgpt-cli-langchain-0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      775 2023-06-23 16:44:06.933337 chatgpt-cli-langchain-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 chatgpt-cli-langchain-0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 16:44:06.873413 chatgpt-cli-langchain-0.8/chatgpt-cli-langchain/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 chatgpt-cli-langchain-0.8/chatgpt-cli-langchain/__init__.py
+-rw-rw-rw-   0        0        0       56 2023-06-23 16:42:42.000000 chatgpt-cli-langchain-0.8/chatgpt-cli-langchain/__main__.py
+-rw-rw-rw-   0        0        0     3993 2023-06-23 16:43:27.000000 chatgpt-cli-langchain-0.8/chatgpt-cli-langchain/chat.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:44:06.928317 chatgpt-cli-langchain-0.8/chatgpt_cli_langchain.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-06-23 16:44:06.000000 chatgpt-cli-langchain-0.8/chatgpt_cli_langchain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-23 16:44:06.000000 chatgpt-cli-langchain-0.8/chatgpt_cli_langchain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:44:06.000000 chatgpt-cli-langchain-0.8/chatgpt_cli_langchain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      359 2023-06-23 16:44:06.000000 chatgpt-cli-langchain-0.8/chatgpt_cli_langchain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-23 16:44:06.000000 chatgpt-cli-langchain-0.8/chatgpt_cli_langchain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-23 16:44:06.942318 chatgpt-cli-langchain-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2081 2023-06-23 16:43:59.000000 chatgpt-cli-langchain-0.8/setup.py
```

### Comparing `chatgpt-cli-langchain-0.7/LICENSE.txt` & `chatgpt-cli-langchain-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-langchain-0.7/PKG-INFO` & `chatgpt-cli-langchain-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-langchain
-Version: 0.7
+Version: 0.8
 Summary: Simple CLI interface for ChatGPT
 Home-page: https://github.com/raphael2692/chatgpt-cli-langchain
-Download-URL: https://github.com/user/reponame/archive/v_07.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_08.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `chatgpt-cli-langchain-0.7/chatgpt-cli-langchain/chat.py` & `chatgpt-cli-langchain-0.8/chatgpt-cli-langchain/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-cli-langchain-0.7/chatgpt_cli_langchain.egg-info/PKG-INFO` & `chatgpt-cli-langchain-0.8/chatgpt_cli_langchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chatgpt-cli-langchain
-Version: 0.7
+Version: 0.8
 Summary: Simple CLI interface for ChatGPT
 Home-page: https://github.com/raphael2692/chatgpt-cli-langchain
-Download-URL: https://github.com/user/reponame/archive/v_07.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_08.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `chatgpt-cli-langchain-0.7/setup.py` & `chatgpt-cli-langchain-0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'chatgpt-cli-langchain',         # How you named your package folder (MyLib)
   packages = ['chatgpt-cli-langchain'],   # Chose the same as "name"
-  version = '0.7',      # Start with a small number and increase it with every change you make
+  version = '0.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Simple CLI interface for ChatGPT',   # Give a short description about your library
   author = 'Raffaele Spataro',                   # Type in your name
   author_email = 'raffaele2692@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/raphael2692/chatgpt-cli-langchain',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/user/reponame/archive/v_07.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/user/reponame/archive/v_08.tar.gz',    # I explain this later on
   keywords = ['CHAT', 'GPT', 'CLI'],   # Keywords that define your package best
   install_requires=
         ['aiohttp', 'aiosignal', 'async-timeout', 'attrs', 'certifi', 'charset-normalizer', 'colorama', 'dataclasses-json', 'frozenlist', 'greenlet', 'idna', 'langchain', 'langchainplus-sdk', 'marshmallow', 'marshmallow-enum', 'multidict', 'mypy-extensions', 'numexpr', 'numpy', 'openai', 'openapi-schema-pydantic', 'packaging', 'pydantic', 'pyfiglet', 'PyYAML', 'requests', 'SQLAlchemy', 'tenacity', 'tqdm', 'typing-inspect', 'typing_extensions', 'urllib3', 'yarl'],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

