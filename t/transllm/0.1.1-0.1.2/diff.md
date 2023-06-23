# Comparing `tmp/transllm-0.1.1.tar.gz` & `tmp/transllm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transllm-0.1.1.tar", last modified: Fri Jun 23 09:53:32 2023, max compression
+gzip compressed data, was "transllm-0.1.2.tar", last modified: Fri Jun 23 10:22:28 2023, max compression
```

## Comparing `transllm-0.1.1.tar` & `transllm-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:53:32.921917 transllm-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      972 2023-06-23 09:53:32.920921 transllm-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-06-23 09:35:17.000000 transllm-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 09:53:32.922919 transllm-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1982 2023-06-23 09:52:59.000000 transllm-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:53:32.904725 transllm-0.1.1/transllm/
--rw-rw-rw-   0        0        0      192 2023-06-23 09:53:10.000000 transllm-0.1.1/transllm/__init__.py
--rw-rw-rw-   0        0        0     5528 2023-06-23 09:52:40.000000 transllm-0.1.1/transllm/core.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:53:32.919911 transllm-0.1.1/transllm.egg-info/
--rw-rw-rw-   0        0        0      972 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 09:53:32.000000 transllm-0.1.1/transllm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 10:22:28.879325 transllm-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-06-23 08:54:28.000000 transllm-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6166 2023-06-23 10:22:28.879325 transllm-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5227 2023-06-23 10:20:39.000000 transllm-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 10:22:28.880324 transllm-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1970 2023-06-23 10:22:11.000000 transllm-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:22:28.863659 transllm-0.1.2/transllm/
+-rw-rw-rw-   0        0        0      192 2023-06-23 10:22:14.000000 transllm-0.1.2/transllm/__init__.py
+-rw-rw-rw-   0        0        0     5528 2023-06-23 09:52:40.000000 transllm-0.1.2/transllm/core.py
+drwxrwxrwx   0        0        0        0 2023-06-23 10:22:28.877325 transllm-0.1.2/transllm.egg-info/
+-rw-rw-rw-   0        0        0     6166 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 10:22:28.000000 transllm-0.1.2/transllm.egg-info/top_level.txt
```

### Comparing `transllm-0.1.1/LICENSE` & `transllm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transllm-0.1.1/setup.py` & `transllm-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="transllm",
-    version="0.1.1",
+    version="0.1.2",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="LLMtranslator translates and generates text in multiple languages.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
@@ -43,15 +43,15 @@
         "deepl",
         "transformers",
         "googletrans",
         "bardapi",
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
```

### Comparing `transllm-0.1.1/transllm/core.py` & `transllm-0.1.2/transllm/core.py`

 * *Files identical despite different names*

