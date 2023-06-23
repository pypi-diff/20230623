# Comparing `tmp/me_gpt-0.0.6.tar.gz` & `tmp/me_gpt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\me_gpt-0.0.6.tar", last modified: Thu Jun 22 20:07:33 2023, max compression
+gzip compressed data, was "dist\me_gpt-0.0.7.tar", last modified: Fri Jun 23 20:43:59 2023, max compression
```

## Comparing `me_gpt-0.0.6.tar` & `me_gpt-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 20:07:33.672545 me_gpt-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-06-22 15:12:34.000000 me_gpt-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2071 2023-06-22 20:07:33.671543 me_gpt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1539 2023-06-22 20:04:21.000000 me_gpt-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 20:07:33.654543 me_gpt-0.0.6/me_gpt/
--rw-rw-rw-   0        0        0       36 2023-06-22 19:38:51.000000 me_gpt-0.0.6/me_gpt/__init__.py
--rw-rw-rw-   0        0        0     7559 2023-06-22 19:50:45.000000 me_gpt-0.0.6/me_gpt/ai.py
--rw-rw-rw-   0        0        0     1735 2023-06-22 19:31:39.000000 me_gpt-0.0.6/me_gpt/db.py
--rw-rw-rw-   0        0        0      144 2023-06-22 19:32:53.000000 me_gpt-0.0.6/me_gpt/main.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:07:33.668543 me_gpt-0.0.6/me_gpt.egg-info/
--rw-rw-rw-   0        0        0     2071 2023-06-22 20:07:33.000000 me_gpt-0.0.6/me_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-22 20:07:33.000000 me_gpt-0.0.6/me_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 20:07:33.000000 me_gpt-0.0.6/me_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-22 20:07:33.000000 me_gpt-0.0.6/me_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 20:07:33.000000 me_gpt-0.0.6/me_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 20:07:33.672545 me_gpt-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-06-22 20:07:02.000000 me_gpt-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:43:59.037295 me_gpt-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-22 15:12:34.000000 me_gpt-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3560 2023-06-23 20:43:59.035295 me_gpt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3003 2023-06-23 20:42:29.000000 me_gpt-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 20:43:59.022295 me_gpt-0.0.7/me_gpt/
+-rw-rw-rw-   0        0        0       62 2023-06-23 19:59:41.000000 me_gpt-0.0.7/me_gpt/__init__.py
+-rw-rw-rw-   0        0        0     9823 2023-06-23 20:37:27.000000 me_gpt-0.0.7/me_gpt/ai.py
+-rw-rw-rw-   0        0        0     4841 2023-06-23 19:59:21.000000 me_gpt-0.0.7/me_gpt/db.py
+-rw-rw-rw-   0        0        0      416 2023-06-23 20:00:05.000000 me_gpt-0.0.7/me_gpt/example.py
+-rw-rw-rw-   0        0        0     1509 2023-06-23 19:58:17.000000 me_gpt-0.0.7/me_gpt/similarity.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:43:59.033298 me_gpt-0.0.7/me_gpt.egg-info/
+-rw-rw-rw-   0        0        0     3560 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 20:43:58.000000 me_gpt-0.0.7/me_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:43:59.037295 me_gpt-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-06-23 20:40:42.000000 me_gpt-0.0.7/setup.py
```

### Comparing `me_gpt-0.0.6/LICENSE` & `me_gpt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `me_gpt-0.0.6/setup.py` & `me_gpt-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A python package to clone yourself with the help of GPT'
 LONG_DESCRIPTION = 'A python package to clone yourself with the help of GPT'
 
 # Setting up
 setup(
     name="me_gpt",
     version=VERSION,
     author="Daniel J. McDonald",
     author_email="<daniel@danielmcdonald.dev>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['openai', 'python-dotenv'],
-    keywords=['python', 'gpt', 'openai', 'ai', 'chatbot', 'clone', 'me'],
+    keywords=['python', 'gpt', 'openai', 'ai', 'chatbot', 'clone'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ]
 )
```

