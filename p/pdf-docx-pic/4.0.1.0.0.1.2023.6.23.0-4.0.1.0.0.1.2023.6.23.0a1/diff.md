# Comparing `tmp/pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0.tar.gz` & `tmp/pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0.tar", last modified: Fri Jun 23 04:06:25 2023, max compression
+gzip compressed data, was "pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1.tar", last modified: Fri Jun 23 04:05:34 2023, max compression
```

## Comparing `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0.tar` & `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 04:06:25.798572 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/
--rw-rw-rw-   0        0        0     1903 2023-06-23 04:06:25.798572 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-23 04:06:25.782939 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic/__init__.py
--rw-rw-rw-   0        0        0      344 2023-06-23 04:05:13.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic/check.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:06:25.798572 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1903 2023-06-23 04:06:25.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-23 04:06:25.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 04:06:25.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-06-23 04:06:25.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 04:06:25.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 04:06:25.798572 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/setup.cfg
--rw-rw-rw-   0        0        0     1951 2023-06-23 04:06:14.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 04:05:34.158181 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/
+-rw-rw-rw-   0        0        0     1905 2023-06-23 04:05:34.158181 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 04:05:34.142541 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic/__init__.py
+-rw-rw-rw-   0        0        0      344 2023-06-23 04:05:13.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic/check.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-23 04:05:34.158181 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1905 2023-06-23 04:05:34.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-23 04:05:34.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 04:05:34.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-06-23 04:05:34.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-23 04:05:34.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 04:05:34.158181 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/setup.cfg
+-rw-rw-rw-   0        0        0     1953 2023-06-23 04:05:21.000000 pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/setup.py
```

### Comparing `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/PKG-INFO` & `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf_docx_pic
-Version: 4.0.1.0.0.1.2023.6.23.0
+Version: 4.0.1.0.0.1.2023.6.23.0a1
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
```

### Comparing `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic/main.py` & `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/pdf_docx_pic.egg-info/PKG-INFO` & `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 4.0.1.0.0.1.2023.6.23.0
+Version: 4.0.1.0.0.1.2023.6.23.0a1
 Classifier: Development Status :: 4 - Beta
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
```

### Comparing `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0/setup.py` & `pdf_docx_pic-4.0.1.0.0.1.2023.6.23.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 c.check()
 
 a = open(".\\README.rst", mode='r', encoding = 'UTF-8').read()
 
 setup(
     name = "pdf_docx_pic",
-    version = "4.0.1.0.0.1.2023.6.23.0",
+    version = "4.0.1.0.0.1.2023.6.23.0a1",
     packages = find_packages(),
     python_requires = ">=2.6, <=3.12",
     classifiers = [
         "Development Status :: 4 - Beta",
         "Development Status :: 5 - Production/Stable",
         "Environment :: GPU",
         "Framework :: Jupyter :: JupyterLab :: 4",
```

