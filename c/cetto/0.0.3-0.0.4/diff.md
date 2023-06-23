# Comparing `tmp/cetto-0.0.3.tar.gz` & `tmp/cetto-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cetto-0.0.3.tar", last modified: Fri Jun 23 21:37:41 2023, max compression
+gzip compressed data, was "cetto-0.0.4.tar", last modified: Fri Jun 23 21:44:16 2023, max compression
```

## Comparing `cetto-0.0.3.tar` & `cetto-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 21:37:41.545539 cetto-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 cetto-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      748 2023-06-23 21:37:41.547406 cetto-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 cetto-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 21:37:41.485933 cetto-0.0.3/cetto/
--rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 cetto-0.0.3/cetto/__init__.py
--rw-rw-rw-   0        0        0       56 2023-06-23 16:42:42.000000 cetto-0.0.3/cetto/__main__.py
--rw-rw-rw-   0        0        0     3993 2023-06-23 16:43:27.000000 cetto-0.0.3/cetto/cetto.py
-drwxrwxrwx   0        0        0        0 2023-06-23 21:37:41.543906 cetto-0.0.3/cetto.egg-info/
--rw-rw-rw-   0        0        0      748 2023-06-23 21:37:41.000000 cetto-0.0.3/cetto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-23 21:37:41.000000 cetto-0.0.3/cetto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 21:37:41.000000 cetto-0.0.3/cetto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-23 21:37:41.000000 cetto-0.0.3/cetto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      374 2023-06-23 21:37:41.000000 cetto-0.0.3/cetto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-23 21:37:41.000000 cetto-0.0.3/cetto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-23 21:37:41.551729 cetto-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2118 2023-06-23 21:37:35.000000 cetto-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:44:16.891899 cetto-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 15:47:50.000000 cetto-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      801 2023-06-23 21:44:16.892584 cetto-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-19 15:16:56.000000 cetto-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 21:44:16.832171 cetto-0.0.4/cetto/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:00:01.000000 cetto-0.0.4/cetto/__init__.py
+-rw-rw-rw-   0        0        0       56 2023-06-23 16:42:42.000000 cetto-0.0.4/cetto/__main__.py
+-rw-rw-rw-   0        0        0     4473 2023-06-23 21:43:14.000000 cetto-0.0.4/cetto/cetto.py
+drwxrwxrwx   0        0        0        0 2023-06-23 21:44:16.881205 cetto-0.0.4/cetto.egg-info/
+-rw-rw-rw-   0        0        0      801 2023-06-23 21:44:16.000000 cetto-0.0.4/cetto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-23 21:44:16.000000 cetto-0.0.4/cetto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 21:44:16.000000 cetto-0.0.4/cetto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-23 21:44:16.000000 cetto-0.0.4/cetto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      374 2023-06-23 21:44:16.000000 cetto-0.0.4/cetto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-23 21:44:16.000000 cetto-0.0.4/cetto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-23 21:44:16.893087 cetto-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2171 2023-06-23 21:44:10.000000 cetto-0.0.4/setup.py
```

### Comparing `cetto-0.0.3/LICENSE.txt` & `cetto-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cetto-0.0.3/PKG-INFO` & `cetto-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cetto
-Version: 0.0.3
-Summary: Simple CLI interface for ChatGPT
+Version: 0.0.4
+Summary: Simple CLI interface for ChatGPT Based on Langchain. Blazingly fast, easily hackable.
 Home-page: https://github.com/raphael2692/cetto
-Download-URL: https://github.com/user/reponame/archive/v_0_0_3.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_0_0_4.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cetto-0.0.3/cetto/cetto.py` & `cetto-0.0.4/cetto/cetto.py`

 * *Files 21% similar despite different names*

```diff
@@ -55,16 +55,31 @@
 Human: {human_input}
 Chatbot:
 """,
 }
 
 config = {"model_name": "gpt-3.5-turbo", "temperature": "0.5", "max_tokens": "1000"}
 
+cetto_config = os.environ.get('CETTO_CONFIG')
+cetto_templates = os.environ.get('CETTO_TEMPLATES')
+
+if cetto_config:
+    with open(
+        os.path.join(os.path.dirname(os.path.realpath(cetto_config)), "config.yaml"), "r"
+            ) as yamlfile:
+        config = yaml.safe_load(yamlfile)
+if cetto_templates:
+    with open(
+        os.path.join(os.path.dirname(os.path.realpath(__file__)), "templates.yaml"), "r"
+    ) as yamlfile:
+        templates = yaml.safe_load(yamlfile)
+
+
 def main():
-    welcome_message = pyfiglet.figlet_format("Command Line ChatGPT", font="rectangles")
+    welcome_message = pyfiglet.figlet_format("CETTO", font="rectangles")
     print(welcome_message)
 
     while True:
         try:
             templates_list = "\n".join([f"* {t}" for t in templates.keys()])
             print("system: Select one of the templates below or type 'quit' to exit:")
             print(f"\n{templates_list}\n")
```

### Comparing `cetto-0.0.3/cetto.egg-info/PKG-INFO` & `cetto-0.0.4/cetto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cetto
-Version: 0.0.3
-Summary: Simple CLI interface for ChatGPT
+Version: 0.0.4
+Summary: Simple CLI interface for ChatGPT Based on Langchain. Blazingly fast, easily hackable.
 Home-page: https://github.com/raphael2692/cetto
-Download-URL: https://github.com/user/reponame/archive/v_0_0_3.tar.gz
+Download-URL: https://github.com/user/reponame/archive/v_0_0_4.tar.gz
 Author: Raffaele Spataro
 Author-email: raffaele2692@gmail.com
 License: MIT
 Keywords: CHAT,GPT,CLI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `cetto-0.0.3/setup.py` & `cetto-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'cetto',         # How you named your package folder (MyLib)
   packages = ['cetto'],   # Chose the same as "name"
-  version = '0.0.3',      # Start with a small number and increase it with every change you make
+  version = '0.0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'Simple CLI interface for ChatGPT',   # Give a short description about your library
+  description = 'Simple CLI interface for ChatGPT Based on Langchain. Blazingly fast, easily hackable.',   # Give a short description about your library
   author = 'Raffaele Spataro',                   # Type in your name
   author_email = 'raffaele2692@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/raphael2692/cetto',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/user/reponame/archive/v_0_0_3.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/user/reponame/archive/v_0_0_4.tar.gz',    # I explain this later on
   keywords = ['CHAT', 'GPT', 'CLI'],   # Keywords that define your package best
   install_requires=
         ['beautifulsoup4', 'aiohttp', 'aiosignal', 'async-timeout', 'attrs', 'certifi', 'charset-normalizer', 'colorama', 'dataclasses-json', 'frozenlist', 'greenlet', 'idna', 'langchain', 'langchainplus-sdk', 'marshmallow', 'marshmallow-enum', 'multidict', 'mypy-extensions', 'numexpr', 'numpy', 'openai', 'openapi-schema-pydantic', 'packaging', 'pydantic', 'pyfiglet', 'PyYAML', 'requests', 'SQLAlchemy', 'tenacity', 'tqdm', 'typing-inspect', 'typing_extensions', 'urllib3', 'yarl'],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

