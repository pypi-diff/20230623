# Comparing `tmp/playsongs-2023.1.0.0.tar.gz` & `tmp/playsongs-2023.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playsongs-2023.1.0.0.tar", max compression
+gzip compressed data, was "playsongs-2023.1.0.1.tar", max compression
```

## Comparing `playsongs-2023.1.0.0.tar` & `playsongs-2023.1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     2017 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/README.rst
--rwxr-xr-x   0        0        0     2474 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/playsongs/__init__.py
--rw-r--r--   0        0        0      103 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/playsongs/__main__.py
--rwxr-xr-x   0        0        0      529 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 playsongs-2023.1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2061 2023-06-23 10:47:59.520335 playsongs-2023.1.0.1/README.rst
+-rwxr-xr-x   0        0        0     2474 2023-06-23 10:47:59.520335 playsongs-2023.1.0.1/playsongs/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-23 10:47:59.520335 playsongs-2023.1.0.1/playsongs/__main__.py
+-rwxr-xr-x   0        0        0      529 2023-06-23 10:47:59.520335 playsongs-2023.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 playsongs-2023.1.0.1/PKG-INFO
```

### Comparing `playsongs-2023.1.0.0/README.rst` & `playsongs-2023.1.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 .. code-block:: BASH
 
    python3 -c "from playsongs import PlaySongs; PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)"
 
 Changelog
 ---------
 
+2023.1.0.1
+
+- Fixed outdated dependencies.
+
 2023.1.0.0
 
 - Cleaned-up code.
 
 2021.1.4.1
 
 - Multiprocessing bugfix. The songs should advance automatically now.
```

### Comparing `playsongs-2023.1.0.0/playsongs/__init__.py` & `playsongs-2023.1.0.1/playsongs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 import random
 import multiprocessing
 from playsound import playsound
 
 
-__version__ = '2023.1.0.0'
+__version__ = '2023.1.0.1'
 
 
 def PlaySongs(path: str, repeat: int = 0, shuffle: bool = False) -> str:
     """
     Play MP3 files from a directory.
 
     return str
```

### Comparing `playsongs-2023.1.0.0/pyproject.toml` & `playsongs-2023.1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "PlaySongs"
-version = "2023.1.0.0"
+version = "2023.1.0.1"
 description = "Play MP3 files from a directory."
 readme = "README.rst"
 authors = ["Ahmad Ferdaus Abd Razak <ahmad.ferdaus.abd.razak@ni.com>"]
 license = "GPL-2.0-only"
 repository = "https://github.com/fer1035/pypi-playsongs"
 keywords = ["music", "MP3"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-playsound = "^1.2.2"
-pyobjc = "^7.1"
+python = "^3.8"
+playsound = "^1.3.0"
+pyobjc = "^9.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^7.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `playsongs-2023.1.0.0/PKG-INFO` & `playsongs-2023.1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: playsongs
-Version: 2023.1.0.0
+Version: 2023.1.0.1
 Summary: Play MP3 files from a directory.
 Home-page: https://github.com/fer1035/pypi-playsongs
 License: GPL-2.0-only
 Keywords: music,MP3
 Author: Ahmad Ferdaus Abd Razak
 Author-email: ahmad.ferdaus.abd.razak@ni.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: playsound (>=1.2.2,<2.0.0)
-Requires-Dist: pyobjc (>=7.1,<8.0)
+Requires-Dist: playsound (>=1.3.0,<2.0.0)
+Requires-Dist: pyobjc (>=9.0,<10.0)
 Project-URL: Repository, https://github.com/fer1035/pypi-playsongs
 Description-Content-Type: text/x-rst
 
 ==============
 **PlaySongs**
 ==============
 
@@ -78,14 +76,18 @@
 .. code-block:: BASH
 
    python3 -c "from playsongs import PlaySongs; PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)"
 
 Changelog
 ---------
 
+2023.1.0.1
+
+- Fixed outdated dependencies.
+
 2023.1.0.0
 
 - Cleaned-up code.
 
 2021.1.4.1
 
 - Multiprocessing bugfix. The songs should advance automatically now.
```

