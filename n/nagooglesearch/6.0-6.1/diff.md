# Comparing `tmp/nagooglesearch-6.0.tar.gz` & `tmp/nagooglesearch-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagooglesearch-6.0.tar", last modified: Sun Apr  9 10:51:57 2023, max compression
+gzip compressed data, was "nagooglesearch-6.1.tar", last modified: Fri Jun 23 16:56:15 2023, max compression
```

## Comparing `nagooglesearch-6.0.tar` & `nagooglesearch-6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:51:57.568112 nagooglesearch-6.0/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-08 21:37:17.000000 nagooglesearch-6.0/LICENSE
--rwxrwx---   0 root         (0) root         (0)       67 2023-04-08 21:37:17.000000 nagooglesearch-6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4207 2023-04-09 10:51:57.568112 nagooglesearch-6.0/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     3938 2023-04-08 21:42:54.000000 nagooglesearch-6.0/README.md
--rwxrwx---   0 root         (0) root         (0)      729 2023-04-08 21:43:00.000000 nagooglesearch-6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 10:51:57.568112 nagooglesearch-6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:51:57.564110 nagooglesearch-6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:51:57.564110 nagooglesearch-6.0/src/nagooglesearch/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-08 21:37:17.000000 nagooglesearch-6.0/src/nagooglesearch/__init__.py
--rwxrwx---   0 root         (0) root         (0)     7524 2023-04-09 10:32:21.000000 nagooglesearch-6.0/src/nagooglesearch/nagooglesearch.py
--rwxrwx---   0 root         (0) root         (0)    11269 2023-04-08 21:37:17.000000 nagooglesearch-6.0/src/nagooglesearch/user_agents.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:51:57.568112 nagooglesearch-6.0/src/nagooglesearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4207 2023-04-09 10:51:57.000000 nagooglesearch-6.0/src/nagooglesearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-09 10:51:57.000000 nagooglesearch-6.0/src/nagooglesearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 10:51:57.000000 nagooglesearch-6.0/src/nagooglesearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-09 10:51:57.000000 nagooglesearch-6.0/src/nagooglesearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-09 10:51:57.000000 nagooglesearch-6.0/src/nagooglesearch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:56:15.856094 nagooglesearch-6.1/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-06-19 21:16:29.000000 nagooglesearch-6.1/LICENSE
+-rwxrwx---   0 root         (0) root         (0)       67 2023-06-19 21:16:29.000000 nagooglesearch-6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-06-23 16:56:15.856094 nagooglesearch-6.1/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)     3937 2023-06-23 16:52:18.000000 nagooglesearch-6.1/README.md
+-rwxrwx---   0 root         (0) root         (0)      729 2023-06-23 16:36:16.000000 nagooglesearch-6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 16:56:15.856094 nagooglesearch-6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:56:15.856094 nagooglesearch-6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:56:15.856094 nagooglesearch-6.1/src/nagooglesearch/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-06-19 21:16:29.000000 nagooglesearch-6.1/src/nagooglesearch/__init__.py
+-rwxrwx---   0 root         (0) root         (0)     7582 2023-06-23 16:52:34.000000 nagooglesearch-6.1/src/nagooglesearch/nagooglesearch.py
+-rwxrwx---   0 root         (0) root         (0)    11269 2023-06-19 21:16:29.000000 nagooglesearch-6.1/src/nagooglesearch/user_agents.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:56:15.856094 nagooglesearch-6.1/src/nagooglesearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-06-23 16:56:15.000000 nagooglesearch-6.1/src/nagooglesearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-23 16:56:15.000000 nagooglesearch-6.1/src/nagooglesearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 16:56:15.000000 nagooglesearch-6.1/src/nagooglesearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-23 16:56:15.000000 nagooglesearch-6.1/src/nagooglesearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-23 16:56:15.000000 nagooglesearch-6.1/src/nagooglesearch.egg-info/top_level.txt
```

### Comparing `nagooglesearch-6.0/LICENSE` & `nagooglesearch-6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nagooglesearch-6.0/PKG-INFO` & `nagooglesearch-6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagooglesearch
-Version: 6.0
+Version: 6.1
 Summary: Not another Google searching tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/nagooglesearch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -34,15 +34,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/nagooglesearch && cd nagooglesearch
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/nagooglesearch-6.0-py3-none-any.whl
+python3 -m pip install dist/nagooglesearch-6.1-py3-none-any.whl
 ```
 
 ## Usage
 
 Default values:
 
 ```python
@@ -100,17 +100,19 @@
 	min_sleep = 15, # minimum sleep between page requests
 	max_sleep = 30, # maximum sleep between page requests
 	verbose = False # debug output
 )
 
 urls = client.search()
 
-if "429_TOO_MANY_REQUESTS" in urls:
+const = client.get_rate_limit()
+
+if const in urls:
+	urls.pop(urls.index(const))
 	print("[ HTTP 429 Too Many Requests ]")
-	urls.pop(urls.index("429_TOO_MANY_REQUESTS"))
 	# do something
 
 for url in urls:
 	print(url)
 	# do something
 ```
```

### Comparing `nagooglesearch-6.0/README.md` & `nagooglesearch-6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/nagooglesearch && cd nagooglesearch
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/nagooglesearch-6.0-py3-none-any.whl
+python3 -m pip install dist/nagooglesearch-6.1-py3-none-any.whl
 ```
 
 ## Usage
 
 Default values:
 
 ```python
@@ -87,17 +87,19 @@
 	min_sleep = 15, # minimum sleep between page requests
 	max_sleep = 30, # maximum sleep between page requests
 	verbose = False # debug output
 )
 
 urls = client.search()
 
-if "429_TOO_MANY_REQUESTS" in urls:
+const = client.get_rate_limit()
+
+if const in urls:
+	urls.pop(urls.index(const))
 	print("[ HTTP 429 Too Many Requests ]")
-	urls.pop(urls.index("429_TOO_MANY_REQUESTS"))
 	# do something
 
 for url in urls:
 	print(url)
 	# do something
 ```
```

### Comparing `nagooglesearch-6.0/pyproject.toml` & `nagooglesearch-6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nagooglesearch"
-version = "6.0"
+version = "6.1"
 authors = [{ name = "Ivan Sincek" }]
 description = "Not another Google searching tool."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `nagooglesearch-6.0/src/nagooglesearch/nagooglesearch.py` & `nagooglesearch-6.1/src/nagooglesearch/nagooglesearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 		self.__pagination = {"start": 0, "num": 10}
 		self.__urls = self.__get_urls(tld, parameters, homepage_parameters)
 		self.__session = None
 		self.__proxies = self.__get_proxies(proxy)
 		self.__headers = self.__get_headers(user_agent)
 		self.__rate_limit = "429_TOO_MANY_REQUESTS"
 
+	def get_rate_limit(self):
+		return self.__rate_limit
+
 	def __jdump(self, data):
 		return json.dumps(data, indent = 4, ensure_ascii = False)
 
 	def __debug(self, title, text, json = False):
 		if self.__verbose:
 			print(("{0}: {1}").format(title, self.__jdump(text) if json else text))
```

### Comparing `nagooglesearch-6.0/src/nagooglesearch/user_agents.txt` & `nagooglesearch-6.1/src/nagooglesearch/user_agents.txt`

 * *Files identical despite different names*

### Comparing `nagooglesearch-6.0/src/nagooglesearch.egg-info/PKG-INFO` & `nagooglesearch-6.1/src/nagooglesearch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagooglesearch
-Version: 6.0
+Version: 6.1
 Summary: Not another Google searching tool.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/nagooglesearch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -34,15 +34,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/nagooglesearch && cd nagooglesearch
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/nagooglesearch-6.0-py3-none-any.whl
+python3 -m pip install dist/nagooglesearch-6.1-py3-none-any.whl
 ```
 
 ## Usage
 
 Default values:
 
 ```python
@@ -100,17 +100,19 @@
 	min_sleep = 15, # minimum sleep between page requests
 	max_sleep = 30, # maximum sleep between page requests
 	verbose = False # debug output
 )
 
 urls = client.search()
 
-if "429_TOO_MANY_REQUESTS" in urls:
+const = client.get_rate_limit()
+
+if const in urls:
+	urls.pop(urls.index(const))
 	print("[ HTTP 429 Too Many Requests ]")
-	urls.pop(urls.index("429_TOO_MANY_REQUESTS"))
 	# do something
 
 for url in urls:
 	print(url)
 	# do something
 ```
```

