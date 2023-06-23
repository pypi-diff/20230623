# Comparing `tmp/monoqueue-1.0.1.tar.gz` & `tmp/monoqueue-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monoqueue-1.0.1.tar", last modified: Mon May  8 19:54:44 2023, max compression
+gzip compressed data, was "monoqueue-1.1.0.tar", last modified: Fri Jun 23 21:42:57 2023, max compression
```

## Comparing `monoqueue-1.0.1.tar` & `monoqueue-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     7747 2023-05-08 19:54:44.215310 monoqueue-1.0.1/PKG-INFO
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     6538 2023-04-30 03:14:32.000000 monoqueue-1.0.1/README.md
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     1503 2023-05-08 19:54:30.000000 monoqueue-1.0.1/pyproject.toml
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       38 2023-05-08 19:54:44.215310 monoqueue-1.0.1/setup.cfg
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/src/
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/src/monoqueue/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    10187 2023-05-08 15:53:41.000000 monoqueue-1.0.1/src/monoqueue/__init__.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      423 2023-04-27 20:42:24.000000 monoqueue-1.0.1/src/monoqueue/__main__.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2680 2023-05-06 23:47:56.000000 monoqueue-1.0.1/src/monoqueue/cli.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     3429 2023-05-08 15:53:58.000000 monoqueue-1.0.1/src/monoqueue/discourse.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2927 2023-05-08 15:54:00.000000 monoqueue-1.0.1/src/monoqueue/firefox.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2906 2023-05-08 15:54:04.000000 monoqueue-1.0.1/src/monoqueue/github.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      548 2023-04-27 20:42:24.000000 monoqueue-1.0.1/src/monoqueue/log.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     7617 2023-04-29 18:07:24.000000 monoqueue-1.0.1/src/monoqueue/parse.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2811 2023-05-06 17:41:10.000000 monoqueue-1.0.1/src/monoqueue/time.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     4409 2023-05-06 23:49:09.000000 monoqueue-1.0.1/src/monoqueue/ui.py
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/src/monoqueue.egg-info/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     7747 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/PKG-INFO
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      503 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/SOURCES.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)        1 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/dependency_links.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       42 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/entry_points.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       22 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/requires.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       10 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/top_level.txt
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/tests/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2756 2023-04-29 16:19:18.000000 monoqueue-1.0.1/tests/test_parse.py
+drwxrwxr-x   0 curtis    (1001) curtis    (1001)        0 2023-06-23 21:42:57.783710 monoqueue-1.1.0/
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     7746 2023-06-23 21:42:57.783710 monoqueue-1.1.0/PKG-INFO
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     6537 2023-06-23 18:01:14.000000 monoqueue-1.1.0/README.md
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     1503 2023-06-23 21:41:50.000000 monoqueue-1.1.0/pyproject.toml
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)       38 2023-06-23 21:42:57.783710 monoqueue-1.1.0/setup.cfg
+drwxrwxr-x   0 curtis    (1001) curtis    (1001)        0 2023-06-23 21:42:57.783710 monoqueue-1.1.0/src/
+drwxrwxr-x   0 curtis    (1001) curtis    (1001)        0 2023-06-23 21:42:57.783710 monoqueue-1.1.0/src/monoqueue/
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)    10187 2023-05-26 17:28:52.000000 monoqueue-1.1.0/src/monoqueue/__init__.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)      423 2023-05-26 17:28:52.000000 monoqueue-1.1.0/src/monoqueue/__main__.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     2680 2023-05-26 17:28:52.000000 monoqueue-1.1.0/src/monoqueue/cli.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     3438 2023-06-23 20:23:41.000000 monoqueue-1.1.0/src/monoqueue/discourse.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     3302 2023-06-23 20:27:14.000000 monoqueue-1.1.0/src/monoqueue/firefox.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     2915 2023-06-23 20:23:41.000000 monoqueue-1.1.0/src/monoqueue/github.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)      831 2023-06-23 20:25:59.000000 monoqueue-1.1.0/src/monoqueue/log.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     7617 2023-05-26 17:28:52.000000 monoqueue-1.1.0/src/monoqueue/parse.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     2811 2023-05-26 17:28:52.000000 monoqueue-1.1.0/src/monoqueue/time.py
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     4409 2023-05-26 17:28:52.000000 monoqueue-1.1.0/src/monoqueue/ui.py
+drwxrwxr-x   0 curtis    (1001) curtis    (1001)        0 2023-06-23 21:42:57.783710 monoqueue-1.1.0/src/monoqueue.egg-info/
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     7746 2023-06-23 21:42:57.000000 monoqueue-1.1.0/src/monoqueue.egg-info/PKG-INFO
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)      503 2023-06-23 21:42:57.000000 monoqueue-1.1.0/src/monoqueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)        1 2023-06-23 21:42:57.000000 monoqueue-1.1.0/src/monoqueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)       42 2023-06-23 21:42:57.000000 monoqueue-1.1.0/src/monoqueue.egg-info/entry_points.txt
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)       22 2023-06-23 21:42:57.000000 monoqueue-1.1.0/src/monoqueue.egg-info/requires.txt
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)       10 2023-06-23 21:42:57.000000 monoqueue-1.1.0/src/monoqueue.egg-info/top_level.txt
+drwxrwxr-x   0 curtis    (1001) curtis    (1001)        0 2023-06-23 21:42:57.783710 monoqueue-1.1.0/tests/
+-rw-rw-r--   0 curtis    (1001) curtis    (1001)     2756 2023-05-26 17:28:52.000000 monoqueue-1.1.0/tests/test_parse.py
```

### Comparing `monoqueue-1.0.1/PKG-INFO` & `monoqueue-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monoqueue
-Version: 1.0.1
+Version: 1.1.0
 Summary: Fight burnout. Stay organized.
 Author-email: Curtis Rueden <ctrueden@wisc.edu>
 License: The Unlicense
 Project-URL: homepage, https://github.com/ctrueden/monoqueue
 Project-URL: documentation, https://github.com/ctrueden/monoqueue/blob/main/README.md
 Project-URL: source, https://github.com/ctrueden/monoqueue
 Project-URL: download, https://pypi.org/project/monoqueue/
@@ -69,16 +69,15 @@
 ```shell
 pip install monoqueue
 ```
 
 Or from source:
 
 ```shell
-git clone https://github.com/ctrueden/monoqueue
-pip install --user -e monoqueue
+pip install --user git+https://github.com/ctrueden/monoqueue.git#egg=monoqueue
 ```
 
 And put `~/.local/bin` on your path.
 
 ## Configuration
 
 ```shell
```

### Comparing `monoqueue-1.0.1/README.md` & `monoqueue-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 ```shell
 pip install monoqueue
 ```
 
 Or from source:
 
 ```shell
-git clone https://github.com/ctrueden/monoqueue
-pip install --user -e monoqueue
+pip install --user git+https://github.com/ctrueden/monoqueue.git#egg=monoqueue
 ```
 
 And put `~/.local/bin` on your path.
 
 ## Configuration
 
 ```shell
```

### Comparing `monoqueue-1.0.1/pyproject.toml` & `monoqueue-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "monoqueue"
-version = "1.0.1"
+version = "1.1.0"
 description = "Fight burnout. Stay organized."
 license = {text = "The Unlicense"}
 authors = [{name = "Curtis Rueden", email = "ctrueden@wisc.edu"}]
 readme = "README.md"
 keywords = ["support", "queue"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `monoqueue-1.0.1/src/monoqueue/__init__.py` & `monoqueue-1.1.0/src/monoqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.1/src/monoqueue/cli.py` & `monoqueue-1.1.0/src/monoqueue/cli.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.1/src/monoqueue/discourse.py` & `monoqueue-1.1.0/src/monoqueue/discourse.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 curl -i -sS -X GET -G https://forum.image.sc/search.json \
   --data-urlencode 'q=#development tags:imagej,imagej2,fiji,scijava,scifio status:open status:unsolved' \ 
   --data-urlencode 'page=2' \
   -H "Api-Key: <your-key-here>" \
   -H "Api-Username: ctrueden" | tee image-sc-forum-search-page-2.json
 """
 
-import json, logging, sys, time
+import json, sys, time
 
 import requests
 
+from .log import log
+
 
 def update(mq, config):
     baseurl = config.get("baseurl", f"https://{config['source']}")
     username = config["username"]
     key = config["key"]
     query = config["query"]
 
@@ -91,15 +93,15 @@
             time.sleep(self._delay_per_request)
 
     def _download_page(self, url: str, query: str, page: int):
         headers = {'User-Agent': 'monoqueue'}
         if self._key: headers['Api-Key'] = f"{self._key}"
         if self._username: headers['Api-Username'] = f"{self._username}"
 
-        logging.debug("Downloading %s page %d", url, page)
+        log.debug("Downloading %s page %d", url, page)
         params = {"q": query, "page": page}
         response = requests.get(url, params=params, headers=headers)
         response.raise_for_status()
         result = response.json()
         self.topics.extend(result['topics'])
 
         gsr = result.get("grouped_search_result", {})
```

### Comparing `monoqueue-1.0.1/src/monoqueue/firefox.py` & `monoqueue-1.1.0/src/monoqueue/firefox.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 Routines to extract information from Firefox's places.sqlite database.
 """
 
 import os, shutil, sqlite3, sys, tempfile
 from pathlib import Path
 
 from . import time
+from .log import log
 
 
 def update(mq, config):
     for bookmark in bookmarks(config["folder"]):
         url = bookmark["url"]
         if not url in mq.items:
             mq.items[url] = {}
@@ -28,23 +29,35 @@
             "created": bookmark["dateAdded"],
             "updated": bookmark["lastModified"],
             "bookmark": bookmark
         })
 
 
 def bookmarks(folder_name=None):
-    firefox_config_dir = Path("~/.mozilla/firefox").expanduser()
-    places_dbs = list(firefox_config_dir.glob("*/places.sqlite"))
-
     results = []
 
-    if len(places_dbs) > 0:
-        tf = tempfile.NamedTemporaryFile(delete=False, prefix="firefox", suffix=".sqlite")
-        temp_db_path = tf.name
-        tf.close()
+    config_dirs = [
+        "~/.mozilla/firefox",
+        "~/snap/firefox/common/.mozilla/firefox",
+    ]
+    places_dbs = []
+    for config_dir in config_dirs:
+        sqlite_db_files = Path(config_dir).expanduser().glob("*/places.sqlite")
+        if log.is_debug():
+            for db_file in sqlite_db_files:
+                log.debug(f"Found Firefox sqlite DB: {db_file}")
+        places_dbs.extend(sqlite_db_files)
+
+    if len(places_dbs) == 0:
+        log.warning("No Firefox sqlite DBs found!")
+        return results
+
+    tf = tempfile.NamedTemporaryFile(delete=False, prefix="firefox", suffix=".sqlite")
+    temp_db_path = tf.name
+    tf.close()
 
     for db in places_dbs:
         # NB: make a copy to avoid locked DB in case Firefox is open.
         shutil.copyfile(db, temp_db_path)
 
         cx = sqlite3.connect(temp_db_path)
```

### Comparing `monoqueue-1.0.1/src/monoqueue/github.py` & `monoqueue-1.1.0/src/monoqueue/github.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 # github.py
 # ------------------------------------------------------------------------
 
 """
 Routines to download and organize information from GitHub.
 """
 
-import json, logging, sys, time
+import json, sys, time
 
 import requests
 
+from .log import log
+
 
 def update(mq, config):
     token = config["token"]
     query = config["query"]
 
     ghi = GitHubIssues(token=token)
     ghi._progress = mq.progress
@@ -42,15 +44,15 @@
     @staticmethod
     def _search_url(query):
         return f"https://api.github.com/search/issues?q={query}&sort=created&order=asc&per_page=100"
 
     def __init__(self, items=None, token=None):
         self._token = token
         self.issues = [] if items is None else items
-        self._delay_per_request = 6
+        self._delay_per_request = 7
         self._max_requests = 100
         self._progress = None
 
     def load(self, filepath):
         """
         Load issues from the given JSON file.
         """
@@ -76,15 +78,15 @@
             if not url: break
             time.sleep(self._delay_per_request)
 
     def _download_page(self, url, query):
         headers = {'User-Agent': 'monoqueue'}
         if self._token: headers['Authorization'] = f"token {self._token}"
 
-        logging.debug("Downloading %s", url)
+        log.debug("Downloading %s", url)
         response = requests.get(url, headers=headers)
         response.raise_for_status()
         result = response.json()
         self.issues.extend(result['items'])
 
         next_url = response.links['next']['url'] if 'next' in response.links else None
         if not next_url and result['total_count'] > 1000 and len(result['items']) > 0:
```

### Comparing `monoqueue-1.0.1/src/monoqueue/parse.py` & `monoqueue-1.1.0/src/monoqueue/parse.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.1/src/monoqueue/time.py` & `monoqueue-1.1.0/src/monoqueue/time.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.1/src/monoqueue/ui.py` & `monoqueue-1.1.0/src/monoqueue/ui.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.1/src/monoqueue.egg-info/PKG-INFO` & `monoqueue-1.1.0/src/monoqueue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monoqueue
-Version: 1.0.1
+Version: 1.1.0
 Summary: Fight burnout. Stay organized.
 Author-email: Curtis Rueden <ctrueden@wisc.edu>
 License: The Unlicense
 Project-URL: homepage, https://github.com/ctrueden/monoqueue
 Project-URL: documentation, https://github.com/ctrueden/monoqueue/blob/main/README.md
 Project-URL: source, https://github.com/ctrueden/monoqueue
 Project-URL: download, https://pypi.org/project/monoqueue/
@@ -69,16 +69,15 @@
 ```shell
 pip install monoqueue
 ```
 
 Or from source:
 
 ```shell
-git clone https://github.com/ctrueden/monoqueue
-pip install --user -e monoqueue
+pip install --user git+https://github.com/ctrueden/monoqueue.git#egg=monoqueue
 ```
 
 And put `~/.local/bin` on your path.
 
 ## Configuration
 
 ```shell
```

### Comparing `monoqueue-1.0.1/tests/test_parse.py` & `monoqueue-1.1.0/tests/test_parse.py`

 * *Files identical despite different names*

