# Comparing `tmp/createai-0.1.1.tar.gz` & `tmp/createai-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "createai-0.1.1.tar", last modified: Tue May 16 10:14:33 2023, max compression
+gzip compressed data, was "createai-0.1.2.1.tar", last modified: Fri Jun 23 11:49:14 2023, max compression
```

## Comparing `createai-0.1.1.tar` & `createai-0.1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 10:14:33.701328 createai-0.1.1/
--rw-rw-rw-   0        0        0     1095 2023-05-14 12:09:53.000000 createai-0.1.1/LICENCE
--rw-rw-rw-   0        0        0       48 2023-05-16 10:14:33.000000 createai-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1803 2023-05-16 10:14:33.701328 createai-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1358 2023-05-16 10:13:14.000000 createai-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 10:14:33.699327 createai-0.1.1/createai.egg-info/
--rw-rw-rw-   0        0        0     1803 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 10:14:33.703327 createai-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-16 10:14:33.000000 createai-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:49:14.472135 createai-0.1.2.1/
+-rw-rw-rw-   0        0        0     1095 2023-05-14 12:09:53.000000 createai-0.1.2.1/LICENCE
+-rw-rw-rw-   0        0        0       48 2023-06-23 11:49:12.000000 createai-0.1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1952 2023-06-23 11:49:14.473144 createai-0.1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1505 2023-06-18 14:35:03.000000 createai-0.1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 11:49:14.469144 createai-0.1.2.1/createai.egg-info/
+-rw-rw-rw-   0        0        0     1952 2023-06-23 11:49:13.000000 createai-0.1.2.1/createai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-23 11:49:14.000000 createai-0.1.2.1/createai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:49:13.000000 createai-0.1.2.1/createai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-23 11:49:13.000000 createai-0.1.2.1/createai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:49:14.475141 createai-0.1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-06-23 11:49:12.000000 createai-0.1.2.1/setup.py
```

### Comparing `createai-0.1.1/LICENCE` & `createai-0.1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `createai-0.1.1/PKG-INFO` & `createai-0.1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: createai
-Version: 0.1.1
+Version: 0.1.2.1
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
-# CreateAI v0.1.1
+# CreateAI v0.1.2.1
 It's easy tool to create ai in python easy and fast.
-You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
+You can look at source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
+
+# WARNING!
+On my PC python can't find this module.
+I am using source code from github.
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
 
 ## Authors
 
  - [@R0fael](https://www.github.com/R0fael) - main programmer
 
 ## Features
- - Custom function activations - Errors
+ - Custom function activations
  - Neuron creating in one line of code
  - absolutly open sourse
 
 ## Installation
 
 Installing project with pip
 
@@ -76,12 +80,16 @@
 
 ## Change log
 
 -0.1.0 - first version
 
 -0.1.1 - speed up and little bug fix
 
+-0.1.2 - without numpy - error
+
+-0.1.2.1 - big bugfix
+
 ## Plans
 
--0.1.2 - More metods of learning
+-0.1.3 - More metods of learning
 
--0.1.3 - Multi neurons update
+-0.1.4 - Multi neurons update
```

### Comparing `createai-0.1.1/README.md` & `createai-0.1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 
-# CreateAI v0.1.1
+# CreateAI v0.1.2.1
 It's easy tool to create ai in python easy and fast.
-You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
+You can look at source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
+
+# WARNING!
+On my PC python can't find this module.
+I am using source code from github.
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
 
 ## Authors
 
  - [@R0fael](https://www.github.com/R0fael) - main programmer
 
 ## Features
- - Custom function activations - Errors
+ - Custom function activations
  - Neuron creating in one line of code
  - absolutly open sourse
 
 ## Installation
 
 Installing project with pip
 
@@ -62,12 +66,16 @@
 
 ## Change log
 
 -0.1.0 - first version
 
 -0.1.1 - speed up and little bug fix
 
+-0.1.2 - without numpy - error
+
+-0.1.2.1 - big bugfix
+
 ## Plans
 
--0.1.2 - More metods of learning
+-0.1.3 - More metods of learning
 
--0.1.3 - Multi neurons update
+-0.1.4 - Multi neurons update
```

### Comparing `createai-0.1.1/createai.egg-info/PKG-INFO` & `createai-0.1.2.1/createai.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: createai
-Version: 0.1.1
+Version: 0.1.2.1
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
-# CreateAI v0.1.1
+# CreateAI v0.1.2.1
 It's easy tool to create ai in python easy and fast.
-You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
+You can look at source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
+
+# WARNING!
+On my PC python can't find this module.
+I am using source code from github.
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
  - your motivation
  - your brain
 
 ## Authors
 
  - [@R0fael](https://www.github.com/R0fael) - main programmer
 
 ## Features
- - Custom function activations - Errors
+ - Custom function activations
  - Neuron creating in one line of code
  - absolutly open sourse
 
 ## Installation
 
 Installing project with pip
 
@@ -76,12 +80,16 @@
 
 ## Change log
 
 -0.1.0 - first version
 
 -0.1.1 - speed up and little bug fix
 
+-0.1.2 - without numpy - error
+
+-0.1.2.1 - big bugfix
+
 ## Plans
 
--0.1.2 - More metods of learning
+-0.1.3 - More metods of learning
 
--0.1.3 - Multi neurons update
+-0.1.4 - Multi neurons update
```

### Comparing `createai-0.1.1/setup.py` & `createai-0.1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'C:\MyUse\code\python\EasyPack\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='createai',
-	version='0.1.1',
+	version='0.1.2.1',
 	author='R0fael',
 	author_email='roslobodchikov@gmail.com',
 	description='Easy tool for creating AI in python',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/R0fael/CreateAI',
 	packages=['C:\MyUse\code\python\EasyPack\createai'],
```

