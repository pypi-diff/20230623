# Comparing `tmp/notion-pinecone-0.0.6.tar.gz` & `tmp/notion-pinecone-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\notion-pinecone-0.0.6.tar", last modified: Fri Jun 23 11:19:09 2023, max compression
+gzip compressed data, was "dist\notion-pinecone-0.0.7.tar", last modified: Fri Jun 23 11:31:26 2023, max compression
```

## Comparing `notion-pinecone-0.0.6.tar` & `notion-pinecone-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 11:19:09.875176 notion-pinecone-0.0.6/
--rw-rw-rw-   0        0        0      305 2023-06-23 11:19:07.000000 notion-pinecone-0.0.6/.bumpversion.cfg
--rw-rw-rw-   0        0        0       65 2023-06-23 11:01:57.000000 notion-pinecone-0.0.6/.gitignore
--rw-rw-rw-   0        0        0     1088 2023-06-23 10:50:41.000000 notion-pinecone-0.0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-23 11:19:09.857178 notion-pinecone-0.0.6/NotionPinecone/
--rw-rw-rw-   0        0        0      140 2023-06-23 11:19:07.000000 notion-pinecone-0.0.6/NotionPinecone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:19:09.860175 notion-pinecone-0.0.6/NotionPinecone/__pycache__/
--rw-rw-rw-   0        0        0     2278 2023-06-23 10:32:21.000000 notion-pinecone-0.0.6/NotionPinecone/__pycache__/embedding.cpython-39.pyc
--rw-rw-rw-   0        0        0     3525 2023-06-23 10:31:21.000000 notion-pinecone-0.0.6/NotionPinecone/__pycache__/notion.cpython-39.pyc
--rw-rw-rw-   0        0        0     2562 2023-06-23 10:31:21.000000 notion-pinecone-0.0.6/NotionPinecone/__pycache__/pinecone.cpython-39.pyc
--rw-rw-rw-   0        0        0     1027 2023-06-23 10:15:44.000000 notion-pinecone-0.0.6/NotionPinecone/__pycache__/utils.cpython-39.pyc
--rw-rw-rw-   0        0        0     3541 2023-06-23 11:12:38.000000 notion-pinecone-0.0.6/NotionPinecone/embedding.py
--rw-rw-rw-   0        0        0     4718 2023-06-23 11:14:32.000000 notion-pinecone-0.0.6/NotionPinecone/notion.py
--rw-rw-rw-   0        0        0     4283 2023-06-23 11:15:57.000000 notion-pinecone-0.0.6/NotionPinecone/pinecone.py
--rw-rw-rw-   0        0        0     1262 2023-06-23 11:16:29.000000 notion-pinecone-0.0.6/NotionPinecone/utils.py
--rw-rw-rw-   0        0        0      364 2023-06-23 11:19:09.874175 notion-pinecone-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-06-23 10:50:41.000000 notion-pinecone-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 11:19:09.873176 notion-pinecone-0.0.6/notion_pinecone.egg-info/
--rw-rw-rw-   0        0        0      364 2023-06-23 11:19:09.000000 notion-pinecone-0.0.6/notion_pinecone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-06-23 11:19:09.000000 notion-pinecone-0.0.6/notion_pinecone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 11:19:09.000000 notion-pinecone-0.0.6/notion_pinecone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-23 11:19:09.000000 notion-pinecone-0.0.6/notion_pinecone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-23 11:19:09.000000 notion-pinecone-0.0.6/notion_pinecone.egg-info/top_level.txt
--rwxrwxrwx   0        0        0      119 2023-06-23 11:07:13.000000 notion-pinecone-0.0.6/pypi_upload.bat
--rw-rw-rw-   0        0        0       89 2023-06-23 10:56:22.000000 notion-pinecone-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 11:19:09.875176 notion-pinecone-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-06-23 11:19:07.000000 notion-pinecone-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.689413 notion-pinecone-0.0.7/
+-rw-rw-rw-   0        0        0      305 2023-06-23 11:31:12.000000 notion-pinecone-0.0.7/.bumpversion.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-23 11:01:57.000000 notion-pinecone-0.0.7/.gitignore
+-rw-rw-rw-   0        0        0     1088 2023-06-23 10:50:41.000000 notion-pinecone-0.0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.675413 notion-pinecone-0.0.7/NotionPinecone/
+-rw-rw-rw-   0        0        0      143 2023-06-23 11:31:12.000000 notion-pinecone-0.0.7/NotionPinecone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.678412 notion-pinecone-0.0.7/NotionPinecone/__pycache__/
+-rw-rw-rw-   0        0        0     2278 2023-06-23 10:32:21.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/embedding.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3525 2023-06-23 10:31:21.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/notion.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2562 2023-06-23 10:31:21.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/pinecone.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1027 2023-06-23 10:15:44.000000 notion-pinecone-0.0.7/NotionPinecone/__pycache__/utils.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3541 2023-06-23 11:12:38.000000 notion-pinecone-0.0.7/NotionPinecone/embedding.py
+-rw-rw-rw-   0        0        0     4718 2023-06-23 11:14:32.000000 notion-pinecone-0.0.7/NotionPinecone/notion.py
+-rw-rw-rw-   0        0        0     4283 2023-06-23 11:15:57.000000 notion-pinecone-0.0.7/NotionPinecone/pinecone.py
+-rw-rw-rw-   0        0        0     1262 2023-06-23 11:16:29.000000 notion-pinecone-0.0.7/NotionPinecone/utils.py
+-rw-rw-rw-   0        0        0      364 2023-06-23 11:31:26.689413 notion-pinecone-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-06-23 10:50:41.000000 notion-pinecone-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 11:31:26.688412 notion-pinecone-0.0.7/notion_pinecone.egg-info/
+-rw-rw-rw-   0        0        0      364 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-23 11:31:26.000000 notion-pinecone-0.0.7/notion_pinecone.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0      165 2023-06-23 11:30:54.000000 notion-pinecone-0.0.7/pypi_upload.bat
+-rw-rw-rw-   0        0        0       89 2023-06-23 10:56:22.000000 notion-pinecone-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:31:26.689413 notion-pinecone-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-06-23 11:31:12.000000 notion-pinecone-0.0.7/setup.py
```

### Comparing `notion-pinecone-0.0.6/LICENSE` & `notion-pinecone-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/__pycache__/embedding.cpython-39.pyc` & `notion-pinecone-0.0.7/NotionPinecone/__pycache__/embedding.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/__pycache__/notion.cpython-39.pyc` & `notion-pinecone-0.0.7/NotionPinecone/__pycache__/notion.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/__pycache__/pinecone.cpython-39.pyc` & `notion-pinecone-0.0.7/NotionPinecone/__pycache__/pinecone.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/__pycache__/utils.cpython-39.pyc` & `notion-pinecone-0.0.7/NotionPinecone/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/embedding.py` & `notion-pinecone-0.0.7/NotionPinecone/embedding.py`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/notion.py` & `notion-pinecone-0.0.7/NotionPinecone/notion.py`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/pinecone.py` & `notion-pinecone-0.0.7/NotionPinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/NotionPinecone/utils.py` & `notion-pinecone-0.0.7/NotionPinecone/utils.py`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/notion_pinecone.egg-info/SOURCES.txt` & `notion-pinecone-0.0.7/notion_pinecone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notion-pinecone-0.0.6/setup.py` & `notion-pinecone-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="notion-pinecone",
-    version="0.0.6",
+    version="0.0.7",
     license="MIT",
     author="Felix Zhu",
     author_email="zhu.felix@outlook.com",
     description="Automated QA of Notion in Pinecone",
     long_description=long_description,
     packages=find_packages(),
     setup_requires=["setuptools_scm"],
```

