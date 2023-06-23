# Comparing `tmp/openplugin-client-0.1.0.tar.gz` & `tmp/openplugin-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-client-0.1.0.tar", last modified: Thu Jun 22 14:49:38 2023, max compression
+gzip compressed data, was "openplugin-client-0.2.0.tar", last modified: Fri Jun 23 04:34:41 2023, max compression
```

## Comparing `openplugin-client-0.1.0.tar` & `openplugin-client-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/openplugin/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/openplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/openplugin/openplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/openplugin/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/openplugin_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:34:41.483514 openplugin-client-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 04:34:41.483514 openplugin-client-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:34:41.479514 openplugin-client-0.2.0/openplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 04:34:31.000000 openplugin-client-0.2.0/openplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-23 04:34:31.000000 openplugin-client-0.2.0/openplugin/openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-23 04:34:31.000000 openplugin-client-0.2.0/openplugin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:34:41.483514 openplugin-client-0.2.0/openplugin_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 04:34:41.000000 openplugin-client-0.2.0/openplugin_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 04:34:41.000000 openplugin-client-0.2.0/openplugin_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 04:34:41.000000 openplugin-client-0.2.0/openplugin_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 04:34:41.000000 openplugin-client-0.2.0/openplugin_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 04:34:41.000000 openplugin-client-0.2.0/openplugin_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 04:34:41.483514 openplugin-client-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-23 04:34:31.000000 openplugin-client-0.2.0/setup.py
```

### Comparing `openplugin-client-0.1.0/PKG-INFO` & `openplugin-client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugin-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugin-client-0.1.0/openplugin_client.egg-info/PKG-INFO` & `openplugin-client-0.2.0/openplugin_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugin-client
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugin-client-0.1.0/setup.py` & `openplugin-client-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugin-client', 
-        version="0.1.0",
+        version="0.2.0",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API',
         long_description='Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API',
         packages=find_packages(),
         install_requires=[
             'pyyaml',
```

