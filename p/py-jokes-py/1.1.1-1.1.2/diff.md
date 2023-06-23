# Comparing `tmp/py_jokes_py-1.1.1.tar.gz` & `tmp/py_jokes_py-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_jokes_py-1.1.1.tar", max compression
+gzip compressed data, was "py_jokes_py-1.1.2.tar", max compression
```

## Comparing `py_jokes_py-1.1.1.tar` & `py_jokes_py-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-06-22 13:17:37.956144 py_jokes_py-1.1.1/LICENSE
--rw-r--r--   0        0        0      158 2023-06-22 13:17:37.956144 py_jokes_py-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-22 13:17:37.956144 py_jokes_py-1.1.1/jokes/__init__.py
--rw-r--r--   0        0        0     4519 2023-06-22 13:34:18.699884 py_jokes_py-1.1.1/jokes/jokes.py
--rw-r--r--   0        0        0     5262 2023-06-22 13:47:46.200233 py_jokes_py-1.1.1/jokes/jokesv2.py
--rw-r--r--   0        0        0      886 2023-06-22 13:56:00.940498 py_jokes_py-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 py_jokes_py-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-22 13:17:37.956144 py_jokes_py-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1829 2023-06-23 05:56:12.179947 py_jokes_py-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 13:17:37.956144 py_jokes_py-1.1.2/jokes/__init__.py
+-rw-r--r--   0        0        0     4519 2023-06-23 05:20:38.802298 py_jokes_py-1.1.2/jokes/jokes.py
+-rw-r--r--   0        0        0     5262 2023-06-22 13:47:46.200233 py_jokes_py-1.1.2/jokes/jokesv2.py
+-rw-r--r--   0        0        0      886 2023-06-23 05:56:39.828130 py_jokes_py-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 py_jokes_py-1.1.2/PKG-INFO
```

### Comparing `py_jokes_py-1.1.1/LICENSE` & `py_jokes_py-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_jokes_py-1.1.1/jokes/jokes.py` & `py_jokes_py-1.1.2/jokes/jokes.py`

 * *Files identical despite different names*

### Comparing `py_jokes_py-1.1.1/jokes/jokesv2.py` & `py_jokes_py-1.1.2/jokes/jokesv2.py`

 * *Files identical despite different names*

### Comparing `py_jokes_py-1.1.1/pyproject.toml` & `py_jokes_py-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-jokes-py"
-version = "1.1.1"
+version = "1.1.2"
 description = "Python wrapper for jokes APIs provided by icanhazdadjokes.com and jokeapi.dev"
 authors = ["Freedom Loisa <kitakayaloisa@gmail.com>"]
 readme = "README.md"
 packages = [{include = "jokes"}]
 homepage = "https://github.com/LoisaKitakaya/Jokes"
 documentation = "https://github.com/LoisaKitakaya/Jokes#readme"
 keywords = ["python", "jokes", "api", "dad jokes"]
```

