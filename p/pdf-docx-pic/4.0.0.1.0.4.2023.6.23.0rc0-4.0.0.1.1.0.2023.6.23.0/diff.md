# Comparing `tmp/pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0.tar.gz` & `tmp/pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0.tar", last modified: Fri Jun 23 03:48:56 2023, max compression
+gzip compressed data, was "pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0.tar", last modified: Fri Jun 23 03:55:20 2023, max compression
```

## Comparing `pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0.tar` & `pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 03:48:56.704322 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/
--rw-rw-rw-   0        0        0     1874 2023-06-23 03:48:56.704322 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-23 03:48:56.688705 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-23 03:48:56.704322 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1874 2023-06-23 03:48:56.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-23 03:48:56.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 03:48:56.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-06-23 03:48:56.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 03:48:56.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf_docx_pic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 03:48:56.704322 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/setup.cfg
--rw-rw-rw-   0        0        0     1869 2023-06-23 03:48:45.000000 pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:55:20.663298 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/
+-rw-rw-rw-   0        0        0     1903 2023-06-23 03:55:20.663298 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 03:55:20.647665 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-23 03:55:20.663298 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1903 2023-06-23 03:55:20.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-23 03:55:20.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 03:55:20.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-06-23 03:55:20.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-23 03:55:20.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf_docx_pic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 03:55:20.663298 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-06-23 03:55:08.000000 pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/setup.py
```

### Comparing `pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/PKG-INFO` & `pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf_docx_pic
-Version: 4.0.0.1.0.4.2023.6.23.0rc0
+Version: 4.0.0.1.1.0.2023.6.23.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
+Requires-Python: >=2.6, <=3.12
 
 请注意
 
 最新版本3.1.2.2023.6.19.16.57.42支持2.6, 2.7, 3.3, 3.4, 3.5, 3.6, 3.12
 
 但我们不确定依赖库是否存在。
```

### Comparing `pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf-docx-pic/main.py` & `pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf-docx-pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/pdf_docx_pic.egg-info/PKG-INFO` & `pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 4.0.0.1.0.4.2023.6.23.0rc0
+Version: 4.0.0.1.1.0.2023.6.23.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
+Requires-Python: >=2.6, <=3.12
 
 请注意
 
 最新版本3.1.2.2023.6.19.16.57.42支持2.6, 2.7, 3.3, 3.4, 3.5, 3.6, 3.12
 
 但我们不确定依赖库是否存在。
```

### Comparing `pdf_docx_pic-4.0.0.1.0.4.2023.6.23.0rc0/setup.py` & `pdf_docx_pic-4.0.0.1.1.0.2023.6.23.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import *
 
 a = open(".\\README.rst", mode='r', encoding = 'UTF-8').read()
 
 setup(
     name = "pdf_docx_pic",
-    version = "4.0.0.1.0.4.2023.6.23.0rc0",
+    version = "4.0.0.1.1.0.2023.6.23.0",
     packages = find_packages(),
+    python_requires = ">=2.6, <=3.12",
     classifiers = [
         "Development Status :: 4 - Beta",
         "Development Status :: 5 - Production/Stable",
         "Environment :: GPU",
         "Framework :: Jupyter :: JupyterLab :: 4",
         "Framework :: Django :: 4.2",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
```

