# Comparing `tmp/my-latest-hello-world-0.0.3.tar.gz` & `tmp/my-latest-hello-world-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-latest-hello-world-0.0.3.tar", last modified: Fri Jun 23 06:31:07 2023, max compression
+gzip compressed data, was "my-latest-hello-world-0.0.6.tar", last modified: Fri Jun 23 04:54:30 2023, max compression
```

## Comparing `my-latest-hello-world-0.0.3.tar` & `my-latest-hello-world-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 06:31:07.437444 my-latest-hello-world-0.0.3/
--rw-rw-rw-   0        0        0      339 2023-04-21 02:36:22.000000 my-latest-hello-world-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      235 2023-04-21 01:29:52.000000 my-latest-hello-world-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1107 2023-06-23 06:31:07.435413 my-latest-hello-world-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-04-21 01:59:55.000000 my-latest-hello-world-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-23 06:31:07.421119 my-latest-hello-world-0.0.3/hello/
--rw-rw-rw-   0        0        0      108 2023-06-23 06:30:36.000000 my-latest-hello-world-0.0.3/hello/__init__.py
--rw-rw-rw-   0        0        0      382 2023-06-23 06:14:16.000000 my-latest-hello-world-0.0.3/hello/hello.py
-drwxrwxrwx   0        0        0        0 2023-06-23 06:31:07.433126 my-latest-hello-world-0.0.3/my_latest_hello_world.egg-info/
--rw-rw-rw-   0        0        0     1107 2023-06-23 06:31:06.000000 my-latest-hello-world-0.0.3/my_latest_hello_world.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-06-23 06:31:07.000000 my-latest-hello-world-0.0.3/my_latest_hello_world.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 06:31:06.000000 my-latest-hello-world-0.0.3/my_latest_hello_world.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-23 06:31:06.000000 my-latest-hello-world-0.0.3/my_latest_hello_world.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-23 06:31:06.000000 my-latest-hello-world-0.0.3/my_latest_hello_world.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       23 2023-04-21 01:12:28.000000 my-latest-hello-world-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 06:31:07.438443 my-latest-hello-world-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1009 2023-06-23 06:30:54.000000 my-latest-hello-world-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 04:54:30.733037 my-latest-hello-world-0.0.6/
+-rw-rw-rw-   0        0        0      339 2023-04-21 02:36:22.000000 my-latest-hello-world-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      235 2023-04-21 01:29:52.000000 my-latest-hello-world-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1107 2023-06-23 04:54:30.733037 my-latest-hello-world-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-04-21 01:59:55.000000 my-latest-hello-world-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 04:54:30.717947 my-latest-hello-world-0.0.6/hello/
+-rw-rw-rw-   0        0        0       30 2023-04-21 01:11:25.000000 my-latest-hello-world-0.0.6/hello/__init__.py
+-rw-rw-rw-   0        0        0      291 2023-05-19 04:29:27.000000 my-latest-hello-world-0.0.6/hello/hello.py
+drwxrwxrwx   0        0        0        0 2023-06-23 04:54:30.731038 my-latest-hello-world-0.0.6/my_latest_hello_world.egg-info/
+-rw-rw-rw-   0        0        0     1107 2023-06-23 04:54:29.000000 my-latest-hello-world-0.0.6/my_latest_hello_world.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-06-23 04:54:30.000000 my-latest-hello-world-0.0.6/my_latest_hello_world.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 04:54:29.000000 my-latest-hello-world-0.0.6/my_latest_hello_world.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-23 04:54:29.000000 my-latest-hello-world-0.0.6/my_latest_hello_world.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-23 04:54:29.000000 my-latest-hello-world-0.0.6/my_latest_hello_world.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       23 2023-04-21 01:12:28.000000 my-latest-hello-world-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 04:54:30.734030 my-latest-hello-world-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2023-05-05 04:15:24.000000 my-latest-hello-world-0.0.6/setup.py
```

### Comparing `my-latest-hello-world-0.0.3/PKG-INFO` & `my-latest-hello-world-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-latest-hello-world
-Version: 0.0.3
+Version: 0.0.6
 Summary: A simple library to print hello world
 Author: Pragyat Singh Rana
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `my-latest-hello-world-0.0.3/my_latest_hello_world.egg-info/PKG-INFO` & `my-latest-hello-world-0.0.6/my_latest_hello_world.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-latest-hello-world
-Version: 0.0.3
+Version: 0.0.6
 Summary: A simple library to print hello world
 Author: Pragyat Singh Rana
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `my-latest-hello-world-0.0.3/setup.py` & `my-latest-hello-world-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./requirements.txt", "r", encoding="utf-8") as reqs_file:
     reqs = reqs_file.readlines()
 
 setup(
     name="my-latest-hello-world",
-    version="0.0.3",
+    version="0.0.6",
     description="A simple library to print hello world",
     long_description=open("README.rst", encoding="utf-8").read(),
     author="Pragyat Singh Rana",
     packages=find_packages(),
     install_requires=reqs,
     include_package_data=True,
     classifiers=[
```

