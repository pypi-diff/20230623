# Comparing `tmp/disklru-1.0.6.tar.gz` & `tmp/disklru-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disklru-1.0.6.tar", last modified: Thu May 25 02:16:44 2023, max compression
+gzip compressed data, was "disklru-1.0.7.tar", last modified: Fri Jun 23 18:13:19 2023, max compression
```

## Comparing `disklru-1.0.6.tar` & `disklru-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.925649 disklru-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.881650 disklru-1.0.6/.github/
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.903648 disklru-1.0.6/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      800 2023-05-25 00:48:35.000000 disklru-1.0.6/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     1914 2023-05-25 00:48:35.000000 disklru-1.0.6/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.907649 disklru-1.0.6/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-25 00:48:35.000000 disklru-1.0.6/.vscode/launch.json
--rw-rw-rw-   0        0        0      819 2023-05-25 00:48:35.000000 disklru-1.0.6/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-25 00:48:35.000000 disklru-1.0.6/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-25 00:48:35.000000 disklru-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      102 2023-05-25 00:48:35.000000 disklru-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2764 2023-05-25 02:16:44.924648 disklru-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2023-05-25 00:48:35.000000 disklru-1.0.6/README.md
--rw-rw-rw-   0        0        0      400 2023-05-25 00:48:35.000000 disklru-1.0.6/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-25 00:48:35.000000 disklru-1.0.6/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-25 00:48:35.000000 disklru-1.0.6/make_venv.py
--rw-rw-rw-   0        0        0      712 2023-05-25 02:16:25.000000 disklru-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-05-25 00:48:35.000000 disklru-1.0.6/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 02:16:44.926649 disklru-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-05-25 00:48:35.000000 disklru-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.883649 disklru-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.909649 disklru-1.0.6/src/disklru/
--rw-rw-rw-   0        0        0       92 2023-05-25 00:48:35.000000 disklru-1.0.6/src/disklru/__init__.py
--rw-rw-rw-   0        0        0     3641 2023-05-25 00:48:35.000000 disklru-1.0.6/src/disklru/disklru.py
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.922649 disklru-1.0.6/src/disklru.egg-info/
--rw-rw-rw-   0        0        0     2764 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 02:16:44.000000 disklru-1.0.6/src/disklru.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 02:16:44.923649 disklru-1.0.6/tests/
--rw-rw-rw-   0        0        0     3163 2023-05-25 00:48:35.000000 disklru-1.0.6/tests/test_disklru.py
--rw-rw-rw-   0        0        0      498 2023-05-25 00:48:35.000000 disklru-1.0.6/tox.ini
--rw-rw-rw-   0        0        0      312 2023-05-25 02:15:29.000000 disklru-1.0.6/upload_package.sh
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.765107 disklru-1.0.7/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.759697 disklru-1.0.7/.github/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.763040 disklru-1.0.7/.github/workflows/
+-rw-r--r--   0 niteris    (501) staff       (20)      855 2023-05-18 22:37:02.000000 disklru-1.0.7/.github/workflows/lint.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      801 2023-05-18 22:37:02.000000 disklru-1.0.7/.github/workflows/push_macos.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      803 2023-05-18 22:37:02.000000 disklru-1.0.7/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      800 2023-05-18 22:37:02.000000 disklru-1.0.7/.github/workflows/push_win.yml
+-rw-r--r--   0 niteris    (501) staff       (20)     1914 2023-05-18 22:37:02.000000 disklru-1.0.7/.gitignore
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.763494 disklru-1.0.7/.vscode/
+-rw-r--r--   0 niteris    (501) staff       (20)     1354 2023-05-18 22:37:02.000000 disklru-1.0.7/.vscode/launch.json
+-rw-r--r--   0 niteris    (501) staff       (20)      819 2023-05-18 22:37:02.000000 disklru-1.0.7/.vscode/settings.json
+-rw-r--r--   0 niteris    (501) staff       (20)     1109 2023-05-18 22:37:02.000000 disklru-1.0.7/.vscode/tasks.json
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2023-05-18 22:37:02.000000 disklru-1.0.7/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)      102 2023-05-18 22:37:02.000000 disklru-1.0.7/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     2694 2023-06-23 18:13:19.764964 disklru-1.0.7/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)     2045 2023-06-23 18:11:38.000000 disklru-1.0.7/README.md
+-rwxr-xr-x   0 niteris    (501) staff       (20)      400 2023-05-19 00:59:49.000000 disklru-1.0.7/activate.sh
+-rwxr-xr-x   0 niteris    (501) staff       (20)      435 2023-05-18 22:37:02.000000 disklru-1.0.7/lint.sh
+-rw-r--r--   0 niteris    (501) staff       (20)     2138 2023-05-18 22:37:02.000000 disklru-1.0.7/make_venv.py
+-rw-r--r--   0 niteris    (501) staff       (20)      727 2023-06-23 18:13:07.000000 disklru-1.0.7/pyproject.toml
+-rw-r--r--   0 niteris    (501) staff       (20)       47 2023-05-19 01:11:14.000000 disklru-1.0.7/requirements.testing.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-06-23 18:13:19.765145 disklru-1.0.7/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     1090 2023-05-18 22:37:02.000000 disklru-1.0.7/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.759943 disklru-1.0.7/src/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.763808 disklru-1.0.7/src/disklru/
+-rw-r--r--   0 niteris    (501) staff       (20)       92 2023-05-19 01:11:14.000000 disklru-1.0.7/src/disklru/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3654 2023-06-23 18:12:02.000000 disklru-1.0.7/src/disklru/disklru.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.764516 disklru-1.0.7/src/disklru.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     2694 2023-06-23 18:13:19.000000 disklru-1.0.7/src/disklru.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      543 2023-06-23 18:13:19.000000 disklru-1.0.7/src/disklru.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-06-23 18:13:19.000000 disklru-1.0.7/src/disklru.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        8 2023-06-23 18:13:19.000000 disklru-1.0.7/src/disklru.egg-info/top_level.txt
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-23 18:13:19.764634 disklru-1.0.7/tests/
+-rw-r--r--   0 niteris    (501) staff       (20)     3163 2023-05-19 01:11:27.000000 disklru-1.0.7/tests/test_disklru.py
+-rw-r--r--   0 niteris    (501) staff       (20)      498 2023-05-19 01:11:14.000000 disklru-1.0.7/tox.ini
+-rwxr-xr-x   0 niteris    (501) staff       (20)      312 2023-06-23 18:11:38.000000 disklru-1.0.7/upload_package.sh
```

### Comparing `disklru-1.0.6/.github/workflows/lint.yml` & `disklru-1.0.7/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/.github/workflows/push_macos.yml` & `disklru-1.0.7/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/.github/workflows/push_ubuntu.yml` & `disklru-1.0.7/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/.github/workflows/push_win.yml` & `disklru-1.0.7/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/.gitignore` & `disklru-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/.vscode/launch.json` & `disklru-1.0.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/.vscode/settings.json` & `disklru-1.0.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/.vscode/tasks.json` & `disklru-1.0.7/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/LICENSE` & `disklru-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/PKG-INFO` & `disklru-1.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-Metadata-Version: 2.1
-Name: disklru
-Version: 1.0.6
-Summary: Creates a python disk LRU / cache - great for apps that want to save data
-Home-page: https://github.com/zackees/disklru
-Maintainer: Zachary Vorhies
-License: BSD 3-Clause License
-Keywords: template-python-cmd
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# disklru
-
-`pip install disklru`
-
-Creates a disk based lru (least recently used) cache, backed by sqlite, that you can use in your apps.
-
-Zero dependency package. Only relies on the python standard lib. Cross platform tests.
-
-[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
-
-[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
-[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
-[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
-
-
-# Usage
-
-```python
-from disklru import DiskLRUCache
-
-LRU_CACHE_FILE = "cache.db"
-MAX_ENTRIES = 4
-cache = DiskLRUCache(LRU_CACHE_FILE, MAX_ENTRIES)
-cache.put("key", "value")
-assert cache.get("key1") == "val"
-cache.clear()
-```
-
-# API
-
-```python
-class DiskLRUCache:
-    """Disk-based LRU cache using SQLite."""
-
-    def get(self, key: str) -> str | None:
-        """Returns the value associated with the given key, or None if the key is not in the cache."""
-
-    def get_json(self, key: str) -> Any:
-        """Returns the value associated with the given key, or None if the key is not in the cache."""
-
-    def put(self, key: str, value: str) -> None:
-        """Sets the value associated with the given key."""
-
-    def put_json(self, key: str, val: Any) -> None:
-        """Sets the value associated with the given key."""
-
-    def delete(self, key) -> None:
-        """Deletes the given key from the cache."""
-
-    def purge(self, timestamp) -> None:
-        """Purges all elements less than the timestamp."""
-
-    def clear(self) -> None:
-        """Clears the cache."""
-
-    def __del__(self) -> None:
-        """Destructor."""
-        self.close()
-
-    def close(self) -> None:
-        """Closes the connection to the database."""
-```
-
-# Development
-
-### Windows
-
-This environment requires you to use `git-bash`.
-
-### Linting
-
-Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
+Metadata-Version: 2.1
+Name: disklru
+Version: 1.0.7
+Summary: Creates a python disk LRU / cache - great for apps that want to save data
+Home-page: https://github.com/zackees/disklru
+Maintainer: Zachary Vorhies
+License: BSD 3-Clause License
+Keywords: disk lru cache least recently used
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# disklru
+
+`pip install disklru`
+
+Creates a disk based lru (least recently used) cache, backed by sqlite, that you can use in your apps.
+
+Zero dependency package. Only relies on the python standard lib. Cross platform tests.
+
+[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
+
+[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
+[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
+[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
+
+
+# Usage
+
+```python
+from disklru import DiskLRUCache
+
+LRU_CACHE_FILE = "cache.db"
+MAX_ENTRIES = 4
+cache = DiskLRUCache(LRU_CACHE_FILE, MAX_ENTRIES)
+cache.put("key", "value")
+assert cache.get("key1") == "val"
+cache.clear()
+```
+
+# API
+
+```python
+class DiskLRUCache:
+    """Disk-based LRU cache using SQLite."""
+
+    def get(self, key: str) -> str | None:
+        """Returns the value associated with the given key, or None if the key is not in the cache."""
+
+    def get_json(self, key: str) -> Any:
+        """Returns the value associated with the given key, or None if the key is not in the cache."""
+
+    def put(self, key: str, value: str) -> None:
+        """Sets the value associated with the given key."""
+
+    def put_json(self, key: str, val: Any) -> None:
+        """Sets the value associated with the given key."""
+
+    def delete(self, key) -> None:
+        """Deletes the given key from the cache."""
+
+    def purge(self, timestamp) -> None:
+        """Purges all elements less than the timestamp."""
+
+    def clear(self) -> None:
+        """Clears the cache."""
+
+    def __del__(self) -> None:
+        """Destructor."""
+        self.close()
+
+    def close(self) -> None:
+        """Closes the connection to the database."""
+```
+
+# Development
+
+### Windows
+
+This environment requires you to use `git-bash`.
+
+### Linting
+
+Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
```

### Comparing `disklru-1.0.6/README.md` & `disklru-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/make_venv.py` & `disklru-1.0.7/make_venv.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/pyproject.toml` & `disklru-1.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "disklru"
 description = "Creates a python disk LRU / cache - great for apps that want to save data"
 requires-python = ">=3.7"
-keywords = ["template-python-cmd"]
+keywords = ["disk lru cache least recently used"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
 ]
 # Change this with the version number bump.
 # Also make the change in zcmds/version.py
-version = "1.0.6"
+version = "1.0.7"
 
 [tool.ruff]
 line-length = 200
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
```

### Comparing `disklru-1.0.6/setup.py` & `disklru-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/src/disklru/disklru.py` & `disklru-1.0.7/src/disklru/disklru.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Disk-based LRU cache using SQLite.
 """
 
 import json
 import os
 import sqlite3
 from datetime import datetime
-from typing import Any
+from typing import Any, Optional
 
 # pylint: disable=line-too-long
 
 
 class DiskLRUCache:
     """Disk-based LRU cache using SQLite."""
 
@@ -32,15 +32,15 @@
         self.cursor.execute(
             "CREATE INDEX IF NOT EXISTS idx_timestamp ON cache (timestamp);"
         )
         self.cursor.execute("CREATE INDEX IF NOT EXISTS idx_key ON cache (key);")
         self.conn.commit()
         self.max_size = max_size
 
-    def get(self, key: str) -> str | None:
+    def get(self, key: str) -> Optional[str]:
         """Returns the value associated with the given key, or None if the key is not in the cache."""
         assert not self.closed
         self.cursor.execute("SELECT value FROM cache WHERE key=?", (key,))
         result = self.cursor.fetchone()
         if result is not None:
             self.cursor.execute(
                 "UPDATE cache SET timestamp=? WHERE key=?",
```

### Comparing `disklru-1.0.6/src/disklru.egg-info/PKG-INFO` & `disklru-1.0.7/src/disklru.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-Metadata-Version: 2.1
-Name: disklru
-Version: 1.0.6
-Summary: Creates a python disk LRU / cache - great for apps that want to save data
-Home-page: https://github.com/zackees/disklru
-Maintainer: Zachary Vorhies
-License: BSD 3-Clause License
-Keywords: template-python-cmd
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# disklru
-
-`pip install disklru`
-
-Creates a disk based lru (least recently used) cache, backed by sqlite, that you can use in your apps.
-
-Zero dependency package. Only relies on the python standard lib. Cross platform tests.
-
-[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
-
-[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
-[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
-[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
-
-
-# Usage
-
-```python
-from disklru import DiskLRUCache
-
-LRU_CACHE_FILE = "cache.db"
-MAX_ENTRIES = 4
-cache = DiskLRUCache(LRU_CACHE_FILE, MAX_ENTRIES)
-cache.put("key", "value")
-assert cache.get("key1") == "val"
-cache.clear()
-```
-
-# API
-
-```python
-class DiskLRUCache:
-    """Disk-based LRU cache using SQLite."""
-
-    def get(self, key: str) -> str | None:
-        """Returns the value associated with the given key, or None if the key is not in the cache."""
-
-    def get_json(self, key: str) -> Any:
-        """Returns the value associated with the given key, or None if the key is not in the cache."""
-
-    def put(self, key: str, value: str) -> None:
-        """Sets the value associated with the given key."""
-
-    def put_json(self, key: str, val: Any) -> None:
-        """Sets the value associated with the given key."""
-
-    def delete(self, key) -> None:
-        """Deletes the given key from the cache."""
-
-    def purge(self, timestamp) -> None:
-        """Purges all elements less than the timestamp."""
-
-    def clear(self) -> None:
-        """Clears the cache."""
-
-    def __del__(self) -> None:
-        """Destructor."""
-        self.close()
-
-    def close(self) -> None:
-        """Closes the connection to the database."""
-```
-
-# Development
-
-### Windows
-
-This environment requires you to use `git-bash`.
-
-### Linting
-
-Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
+Metadata-Version: 2.1
+Name: disklru
+Version: 1.0.7
+Summary: Creates a python disk LRU / cache - great for apps that want to save data
+Home-page: https://github.com/zackees/disklru
+Maintainer: Zachary Vorhies
+License: BSD 3-Clause License
+Keywords: disk lru cache least recently used
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# disklru
+
+`pip install disklru`
+
+Creates a disk based lru (least recently used) cache, backed by sqlite, that you can use in your apps.
+
+Zero dependency package. Only relies on the python standard lib. Cross platform tests.
+
+[![Linting](https://github.com/zackees/disklru/actions/workflows/lint.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/lint.yml)
+
+[![MacOS_Tests](https://github.com/zackees/disklru/actions/workflows/push_macos.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_macos.yml)
+[![Ubuntu_Tests](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_ubuntu.yml)
+[![Win_Tests](https://github.com/zackees/disklru/actions/workflows/push_win.yml/badge.svg)](https://github.com/zackees/disklru/actions/workflows/push_win.yml)
+
+
+# Usage
+
+```python
+from disklru import DiskLRUCache
+
+LRU_CACHE_FILE = "cache.db"
+MAX_ENTRIES = 4
+cache = DiskLRUCache(LRU_CACHE_FILE, MAX_ENTRIES)
+cache.put("key", "value")
+assert cache.get("key1") == "val"
+cache.clear()
+```
+
+# API
+
+```python
+class DiskLRUCache:
+    """Disk-based LRU cache using SQLite."""
+
+    def get(self, key: str) -> str | None:
+        """Returns the value associated with the given key, or None if the key is not in the cache."""
+
+    def get_json(self, key: str) -> Any:
+        """Returns the value associated with the given key, or None if the key is not in the cache."""
+
+    def put(self, key: str, value: str) -> None:
+        """Sets the value associated with the given key."""
+
+    def put_json(self, key: str, val: Any) -> None:
+        """Sets the value associated with the given key."""
+
+    def delete(self, key) -> None:
+        """Deletes the given key from the cache."""
+
+    def purge(self, timestamp) -> None:
+        """Purges all elements less than the timestamp."""
+
+    def clear(self) -> None:
+        """Clears the cache."""
+
+    def __del__(self) -> None:
+        """Destructor."""
+        self.close()
+
+    def close(self) -> None:
+        """Closes the connection to the database."""
+```
+
+# Development
+
+### Windows
+
+This environment requires you to use `git-bash`.
+
+### Linting
+
+Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
```

### Comparing `disklru-1.0.6/src/disklru.egg-info/SOURCES.txt` & `disklru-1.0.7/src/disklru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disklru-1.0.6/tests/test_disklru.py` & `disklru-1.0.7/tests/test_disklru.py`

 * *Files identical despite different names*

