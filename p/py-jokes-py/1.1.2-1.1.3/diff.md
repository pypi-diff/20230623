# Comparing `tmp/py_jokes_py-1.1.2.tar.gz` & `tmp/py_jokes_py-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_jokes_py-1.1.2.tar", max compression
+gzip compressed data, was "py_jokes_py-1.1.3.tar", max compression
```

## Comparing `py_jokes_py-1.1.2.tar` & `py_jokes_py-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-06-22 13:17:37.956144 py_jokes_py-1.1.2/LICENSE
--rw-r--r--   0        0        0     1829 2023-06-23 05:56:12.179947 py_jokes_py-1.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-22 13:17:37.956144 py_jokes_py-1.1.2/jokes/__init__.py
--rw-r--r--   0        0        0     4519 2023-06-23 05:20:38.802298 py_jokes_py-1.1.2/jokes/jokes.py
--rw-r--r--   0        0        0     5262 2023-06-22 13:47:46.200233 py_jokes_py-1.1.2/jokes/jokesv2.py
--rw-r--r--   0        0        0      886 2023-06-23 05:56:39.828130 py_jokes_py-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 py_jokes_py-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-22 13:17:37.956144 py_jokes_py-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2149 2023-06-23 06:41:41.483328 py_jokes_py-1.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 13:17:37.956144 py_jokes_py-1.1.3/jokes/__init__.py
+-rw-r--r--   0        0        0     4519 2023-06-23 05:20:38.802298 py_jokes_py-1.1.3/jokes/jokes.py
+-rw-r--r--   0        0        0     5262 2023-06-22 13:47:46.200233 py_jokes_py-1.1.3/jokes/jokesv2.py
+-rw-r--r--   0        0        0      886 2023-06-23 06:56:06.932403 py_jokes_py-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 py_jokes_py-1.1.3/PKG-INFO
```

### Comparing `py_jokes_py-1.1.2/LICENSE` & `py_jokes_py-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_jokes_py-1.1.2/jokes/jokes.py` & `py_jokes_py-1.1.3/jokes/jokes.py`

 * *Files identical despite different names*

### Comparing `py_jokes_py-1.1.2/jokes/jokesv2.py` & `py_jokes_py-1.1.3/jokes/jokesv2.py`

 * *Files identical despite different names*

### Comparing `py_jokes_py-1.1.2/pyproject.toml` & `py_jokes_py-1.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-jokes-py"
-version = "1.1.2"
+version = "1.1.3"
 description = "Python wrapper for jokes APIs provided by icanhazdadjokes.com and jokeapi.dev"
 authors = ["Freedom Loisa <kitakayaloisa@gmail.com>"]
 readme = "README.md"
 packages = [{include = "jokes"}]
 homepage = "https://github.com/LoisaKitakaya/Jokes"
 documentation = "https://github.com/LoisaKitakaya/Jokes#readme"
 keywords = ["python", "jokes", "api", "dad jokes"]
```

### Comparing `py_jokes_py-1.1.2/PKG-INFO` & `py_jokes_py-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jokes-py
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python wrapper for jokes APIs provided by icanhazdadjokes.com and jokeapi.dev
 Home-page: https://github.com/LoisaKitakaya/Jokes
 Keywords: python,jokes,api,dad jokes
 Author: Freedom Loisa
 Author-email: kitakayaloisa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -91,12 +91,24 @@
 
 ## Example
 
 Here is a simple implementation of this package. Check it out:
 
 - [jokes_cli](https://github.com/LoisaKitakaya/jokes_cli)
 
+## Contribution
+
+If you want to contribute to this project, here are some few steps you can follow:
+
+- Fork this project's repository
+- Clone it to your local machine
+- Make the changes you want to make or add the features you want to add
+- Write tests for the new features
+- Make a pull request
+
+That's just about it.
+
 ## Issues
 
 For any issus encountered while using this package, feel free to submit a new issue [here](https://github.com/LoisaKitakaya/Jokes/issues).
 
 Enjoy! 🤪
```

