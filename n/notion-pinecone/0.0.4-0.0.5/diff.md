# Comparing `tmp/notion-pinecone-0.0.4.tar.gz` & `tmp/notion-pinecone-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\notion-pinecone-0.0.4.tar", last modified: Fri Jun 23 11:05:41 2023, max compression
+gzip compressed data, was "dist\notion-pinecone-0.0.5.tar", last modified: Fri Jun 23 11:07:18 2023, max compression
```

## Comparing `notion-pinecone-0.0.4.tar` & `notion-pinecone-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 11:05:41.504387 notion-pinecone-0.0.4/
--rw-rw-rw-   0        0        0      305 2023-06-23 11:05:39.000000 notion-pinecone-0.0.4/.bumpversion.cfg
--rw-rw-rw-   0        0        0       65 2023-06-23 11:01:57.000000 notion-pinecone-0.0.4/.gitignore
--rw-rw-rw-   0        0        0     1088 2023-06-23 10:50:41.000000 notion-pinecone-0.0.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-23 11:05:41.492386 notion-pinecone-0.0.4/NotionPinecone/
--rw-rw-rw-   0        0        0      140 2023-06-23 11:05:39.000000 notion-pinecone-0.0.4/NotionPinecone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:05:41.495384 notion-pinecone-0.0.4/NotionPinecone/__pycache__/
--rw-rw-rw-   0        0        0     2278 2023-06-23 10:32:21.000000 notion-pinecone-0.0.4/NotionPinecone/__pycache__/embedding.cpython-39.pyc
--rw-rw-rw-   0        0        0     3525 2023-06-23 10:31:21.000000 notion-pinecone-0.0.4/NotionPinecone/__pycache__/notion.cpython-39.pyc
--rw-rw-rw-   0        0        0     2562 2023-06-23 10:31:21.000000 notion-pinecone-0.0.4/NotionPinecone/__pycache__/pinecone.cpython-39.pyc
--rw-rw-rw-   0        0        0     1027 2023-06-23 10:15:44.000000 notion-pinecone-0.0.4/NotionPinecone/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-   0        0        0     1779 2023-06-23 10:54:41.000000 notion-pinecone-0.0.4/NotionPinecone/embedding.py
--rw-rw-rw-   0        0        0     3136 2023-06-23 11:03:38.000000 notion-pinecone-0.0.4/NotionPinecone/notion.py
--rw-rw-rw-   0        0        0     2678 2023-06-23 11:01:42.000000 notion-pinecone-0.0.4/NotionPinecone/pinecone.py
--rw-rw-rw-   0        0        0      495 2023-06-23 09:59:39.000000 notion-pinecone-0.0.4/NotionPinecone/utils.py
--rw-rw-rw-   0        0        0      366 2023-06-23 11:05:41.504387 notion-pinecone-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-06-23 10:50:41.000000 notion-pinecone-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 11:05:41.503384 notion-pinecone-0.0.4/notion_pinecone.egg-info/
--rw-rw-rw-   0        0        0      366 2023-06-23 11:05:41.000000 notion-pinecone-0.0.4/notion_pinecone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-06-23 11:05:41.000000 notion-pinecone-0.0.4/notion_pinecone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 11:05:41.000000 notion-pinecone-0.0.4/notion_pinecone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-23 11:05:41.000000 notion-pinecone-0.0.4/notion_pinecone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-23 11:05:41.000000 notion-pinecone-0.0.4/notion_pinecone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       89 2023-06-23 10:56:22.000000 notion-pinecone-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 11:05:41.504387 notion-pinecone-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-06-23 11:05:39.000000 notion-pinecone-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:07:18.337371 notion-pinecone-0.0.5/
+-rw-rw-rw-   0        0        0      305 2023-06-23 11:07:16.000000 notion-pinecone-0.0.5/.bumpversion.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-23 11:01:57.000000 notion-pinecone-0.0.5/.gitignore
+-rw-rw-rw-   0        0        0     1088 2023-06-23 10:50:41.000000 notion-pinecone-0.0.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-23 11:07:18.324370 notion-pinecone-0.0.5/NotionPinecone/
+-rw-rw-rw-   0        0        0      140 2023-06-23 11:07:16.000000 notion-pinecone-0.0.5/NotionPinecone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:07:18.327370 notion-pinecone-0.0.5/NotionPinecone/__pycache__/
+-rw-rw-rw-   0        0        0     2278 2023-06-23 10:32:21.000000 notion-pinecone-0.0.5/NotionPinecone/__pycache__/embedding.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3525 2023-06-23 10:31:21.000000 notion-pinecone-0.0.5/NotionPinecone/__pycache__/notion.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2562 2023-06-23 10:31:21.000000 notion-pinecone-0.0.5/NotionPinecone/__pycache__/pinecone.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1027 2023-06-23 10:15:44.000000 notion-pinecone-0.0.5/NotionPinecone/__pycache__/utils.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1779 2023-06-23 10:54:41.000000 notion-pinecone-0.0.5/NotionPinecone/embedding.py
+-rw-rw-rw-   0        0        0     3136 2023-06-23 11:03:38.000000 notion-pinecone-0.0.5/NotionPinecone/notion.py
+-rw-rw-rw-   0        0        0     2678 2023-06-23 11:01:42.000000 notion-pinecone-0.0.5/NotionPinecone/pinecone.py
+-rw-rw-rw-   0        0        0      495 2023-06-23 09:59:39.000000 notion-pinecone-0.0.5/NotionPinecone/utils.py
+-rw-rw-rw-   0        0        0      366 2023-06-23 11:07:18.337371 notion-pinecone-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-06-23 10:50:41.000000 notion-pinecone-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 11:07:18.336372 notion-pinecone-0.0.5/notion_pinecone.egg-info/
+-rw-rw-rw-   0        0        0      366 2023-06-23 11:07:17.000000 notion-pinecone-0.0.5/notion_pinecone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-06-23 11:07:18.000000 notion-pinecone-0.0.5/notion_pinecone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:07:17.000000 notion-pinecone-0.0.5/notion_pinecone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-23 11:07:17.000000 notion-pinecone-0.0.5/notion_pinecone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-23 11:07:17.000000 notion-pinecone-0.0.5/notion_pinecone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       89 2023-06-23 10:56:22.000000 notion-pinecone-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:07:18.338373 notion-pinecone-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-06-23 11:07:16.000000 notion-pinecone-0.0.5/setup.py
```

### Comparing `notion-pinecone-0.0.4/LICENSE` & `notion-pinecone-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/NotionPinecone/__pycache__/embedding.cpython-39.pyc` & `notion-pinecone-0.0.5/NotionPinecone/__pycache__/embedding.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/NotionPinecone/__pycache__/notion.cpython-39.pyc` & `notion-pinecone-0.0.5/NotionPinecone/__pycache__/notion.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/NotionPinecone/__pycache__/pinecone.cpython-39.pyc` & `notion-pinecone-0.0.5/NotionPinecone/__pycache__/pinecone.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/NotionPinecone/__pycache__/utils.cpython-39.pyc` & `notion-pinecone-0.0.5/NotionPinecone/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/NotionPinecone/embedding.py` & `notion-pinecone-0.0.5/NotionPinecone/embedding.py`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/NotionPinecone/notion.py` & `notion-pinecone-0.0.5/NotionPinecone/notion.py`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/NotionPinecone/pinecone.py` & `notion-pinecone-0.0.5/NotionPinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/notion_pinecone.egg-info/SOURCES.txt` & `notion-pinecone-0.0.5/notion_pinecone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.4/setup.py` & `notion-pinecone-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="notion-pinecone",
-    version="0.0.4",
+    version="0.0.5",
     license="MIT",
     author="Felix Zhu",
     author_email="zhu.felix@outlook.com",
     description="Automated QA of Notion in Pinecone",
     long_description=long_description,
     packages=find_packages(),
     setup_requires=["setuptools_scm"],
```

