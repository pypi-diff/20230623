# Comparing `tmp/banana_dev-4.0.2.tar.gz` & `tmp/banana_dev-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banana_dev-4.0.2.tar", last modified: Fri Apr  7 03:09:55 2023, max compression
+gzip compressed data, was "banana_dev-5.0.0.tar", last modified: Fri Jun 23 20:03:39 2023, max compression
```

## Comparing `banana_dev-4.0.2.tar` & `banana_dev-5.0.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-07 03:09:55.032023 banana_dev-4.0.2/
--rw-r--r--   0 erik       (501) staff       (20)     1880 2023-04-07 03:09:55.032081 banana_dev-4.0.2/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1220 2023-04-07 03:03:29.000000 banana_dev-4.0.2/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-07 03:09:55.031354 banana_dev-4.0.2/banana_dev/
--rw-r--r--   0 erik       (501) staff       (20)       38 2022-11-04 12:23:27.000000 banana_dev-4.0.2/banana_dev/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     4193 2023-04-07 03:06:39.000000 banana_dev-4.0.2/banana_dev/generics.py
--rw-r--r--   0 erik       (501) staff       (20)      571 2023-04-07 01:40:16.000000 banana_dev-4.0.2/banana_dev/package.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-07 03:09:55.031933 banana_dev-4.0.2/banana_dev.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     1880 2023-04-07 03:09:55.000000 banana_dev-4.0.2/banana_dev.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      265 2023-04-07 03:09:55.000000 banana_dev-4.0.2/banana_dev.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-04-07 03:09:55.000000 banana_dev-4.0.2/banana_dev.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       24 2023-04-07 03:09:55.000000 banana_dev-4.0.2/banana_dev.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       11 2023-04-07 03:09:55.000000 banana_dev-4.0.2/banana_dev.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       79 2023-04-07 03:09:55.032261 banana_dev-4.0.2/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1235 2023-04-07 02:55:27.000000 banana_dev-4.0.2/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 20:03:39.643908 banana_dev-5.0.0/
+-rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-23 20:03:39.643964 banana_dev-5.0.0/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     1220 2023-04-25 00:43:43.000000 banana_dev-5.0.0/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 20:03:39.643159 banana_dev-5.0.0/banana_dev/
+-rw-r--r--   0 erik       (501) staff       (20)       26 2023-04-25 02:04:09.000000 banana_dev-5.0.0/banana_dev/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     4026 2023-06-23 18:35:30.000000 banana_dev-5.0.0/banana_dev/client.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-23 20:03:39.643817 banana_dev-5.0.0/banana_dev.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      241 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)       24 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       11 2023-06-23 20:03:39.000000 banana_dev-5.0.0/banana_dev.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       79 2023-06-23 20:03:39.644527 banana_dev-5.0.0/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1222 2023-06-23 19:58:15.000000 banana_dev-5.0.0/setup.py
```

### Comparing `banana_dev-4.0.2/PKG-INFO` & `banana_dev-5.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: banana_dev
-Version: 4.0.2
+Version: 5.0.0
 Summary: The banana package is a python client to interact with your machine learning models hosted on Banana
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: MIT
 Keywords: Banana client,API wrapper,Banana,SDK
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `banana_dev-4.0.2/README.md` & `banana_dev-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `banana_dev-4.0.2/banana_dev.egg-info/PKG-INFO` & `banana_dev-5.0.0/banana_dev.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: banana-dev
-Version: 4.0.2
+Version: 5.0.0
 Summary: The banana package is a python client to interact with your machine learning models hosted on Banana
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: MIT
 Keywords: Banana client,API wrapper,Banana,SDK
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `banana_dev-4.0.2/setup.py` & `banana_dev-5.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='banana_dev',
     packages=['banana_dev'],
-    version='4.0.2',
+    version='5.0.0',
     license='MIT',
     # Give a short description about your library
     description='The banana package is a python client to interact with your machine learning models hosted on Banana',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
@@ -20,15 +20,15 @@
     keywords=['Banana client', 'API wrapper', 'Banana', 'SDK'],
     setup_requires=['wheel'],
     install_requires=[
         "requests>=2.26.0,<3.0.0",
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

