# Comparing `tmp/dare_datasets-0.1.8.tar.gz` & `tmp/dare_datasets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dare_datasets-0.1.8.tar", max compression
+gzip compressed data, was "dare_datasets-0.1.9.tar", max compression
```

## Comparing `dare_datasets-0.1.8.tar` & `dare_datasets-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1133 2023-06-16 05:15:58.724878 dare_datasets-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.8/dare_datasets/__init__.py
--rw-r--r--   0        0        0     2483 2023-06-08 11:08:35.634718 dare_datasets-0.1.8/dare_datasets/dataset_abc.py
--rw-r--r--   0        0        0     1904 2023-06-19 13:47:34.544013 dare_datasets-0.1.8/dare_datasets/iris.py
--rw-r--r--   0        0        0     1288 2023-06-19 13:47:34.544013 dare_datasets-0.1.8/dare_datasets/qr2t_benchmark.py
--rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.8/dare_datasets/utils/__init__.py
--rw-r--r--   0        0        0      711 2023-06-19 13:47:34.552013 dare_datasets-0.1.8/dare_datasets/utils/downloader.py
--rw-r--r--   0        0        0      831 2023-06-19 13:55:21.382213 dare_datasets-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 dare_datasets-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-06-16 05:15:58.724878 dare_datasets-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.9/dare_datasets/__init__.py
+-rw-r--r--   0        0        0     2483 2023-06-08 11:08:35.634718 dare_datasets-0.1.9/dare_datasets/dataset_abc.py
+-rw-r--r--   0        0        0     1904 2023-06-19 13:47:34.544013 dare_datasets-0.1.9/dare_datasets/iris.py
+-rw-r--r--   0        0        0     1288 2023-06-19 13:47:34.544013 dare_datasets-0.1.9/dare_datasets/qr2t_benchmark.py
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.9/dare_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-19 13:47:34.552013 dare_datasets-0.1.9/dare_datasets/utils/downloader.py
+-rw-r--r--   0        0        0      831 2023-06-19 14:05:57.908931 dare_datasets-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 dare_datasets-0.1.9/PKG-INFO
```

### Comparing `dare_datasets-0.1.8/README.md` & `dare_datasets-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.8/dare_datasets/dataset_abc.py` & `dare_datasets-0.1.9/dare_datasets/dataset_abc.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.8/dare_datasets/iris.py` & `dare_datasets-0.1.9/dare_datasets/iris.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.8/dare_datasets/qr2t_benchmark.py` & `dare_datasets-0.1.9/dare_datasets/qr2t_benchmark.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.8/dare_datasets/utils/downloader.py` & `dare_datasets-0.1.9/dare_datasets/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.8/pyproject.toml` & `dare_datasets-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dare-datasets"
-version = "0.1.8"
+version = "0.1.9"
 description = "A quick and easy way to download datasets from the DARE lab."
 authors = ["MikeXydas <mikexydas@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dare_datasets"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dare_datasets-0.1.8/PKG-INFO` & `dare_datasets-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dare-datasets
-Version: 0.1.8
+Version: 0.1.9
 Summary: A quick and easy way to download datasets from the DARE lab.
 Author: MikeXydas
 Author-email: mikexydas@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

