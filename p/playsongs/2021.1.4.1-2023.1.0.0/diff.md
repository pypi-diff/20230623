# Comparing `tmp/PlaySongs-2021.1.4.1.tar.gz` & `tmp/playsongs-2023.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlaySongs-2021.1.4.1.tar", max compression
+gzip compressed data, was "playsongs-2023.1.0.0.tar", max compression
```

## Comparing `PlaySongs-2021.1.4.1.tar` & `playsongs-2023.1.0.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rwxr-xr-x   0        0        0     2005 2021-03-23 05:42:02.004781 PlaySongs-2021.1.4.1/README.rst
--rwxr-xr-x   0        0        0       27 2021-03-23 05:42:02.004781 PlaySongs-2021.1.4.1/playsongs/__init__.py
--rwxr-xr-x   0        0        0     2205 2021-03-23 05:42:02.004781 PlaySongs-2021.1.4.1/playsongs/playsongs.py
--rwxr-xr-x   0        0        0      529 2021-03-23 05:42:02.004781 PlaySongs-2021.1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2822 2021-03-23 05:42:13.662526 PlaySongs-2021.1.4.1/setup.py
--rw-r--r--   0        0        0     2813 2021-03-23 05:42:13.663509 PlaySongs-2021.1.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2017 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/README.rst
+-rwxr-xr-x   0        0        0     2474 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/playsongs/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/playsongs/__main__.py
+-rwxr-xr-x   0        0        0      529 2023-06-23 10:36:44.350152 playsongs-2023.1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 playsongs-2023.1.0.0/PKG-INFO
```

### Comparing `PlaySongs-2021.1.4.1/README.rst` & `playsongs-2023.1.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -43,26 +43,30 @@
    # or
    python3 -m pip install playsongs
 
 In Python3:
 
 .. code-block:: BASH
 
-   from playsongs.playsongs import PlaySongs
+   from playsongs import PlaySongs
    PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)
 
 In BASH:
 
 .. code-block:: BASH
 
-   python3 -c "from playsongs.playsongs import PlaySongs; PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)"
+   python3 -c "from playsongs import PlaySongs; PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)"
 
 Changelog
 ---------
 
+2023.1.0.0
+
+- Cleaned-up code.
+
 2021.1.4.1
 
 - Multiprocessing bugfix. The songs should advance automatically now.
 
 2021.1.3.1
 
 - Updated README.
```

### Comparing `PlaySongs-2021.1.4.1/pyproject.toml` & `playsongs-2023.1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaySongs"
-version = "2021.1.4.1"
+version = "2023.1.0.0"
 description = "Play MP3 files from a directory."
 readme = "README.rst"
 authors = ["Ahmad Ferdaus Abd Razak <ahmad.ferdaus.abd.razak@ni.com>"]
 license = "GPL-2.0-only"
 repository = "https://github.com/fer1035/pypi-playsongs"
 keywords = ["music", "MP3"]
```

### Comparing `PlaySongs-2021.1.4.1/PKG-INFO` & `playsongs-2023.1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: playsongs
-Version: 2021.1.4.1
+Version: 2023.1.0.0
 Summary: Play MP3 files from a directory.
 Home-page: https://github.com/fer1035/pypi-playsongs
 License: GPL-2.0-only
 Keywords: music,MP3
 Author: Ahmad Ferdaus Abd Razak
 Author-email: ahmad.ferdaus.abd.razak@ni.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: playsound (>=1.2.2,<2.0.0)
 Requires-Dist: pyobjc (>=7.1,<8.0)
 Project-URL: Repository, https://github.com/fer1035/pypi-playsongs
 Description-Content-Type: text/x-rst
 
 ==============
 **PlaySongs**
@@ -64,26 +66,30 @@
    # or
    python3 -m pip install playsongs
 
 In Python3:
 
 .. code-block:: BASH
 
-   from playsongs.playsongs import PlaySongs
+   from playsongs import PlaySongs
    PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)
 
 In BASH:
 
 .. code-block:: BASH
 
-   python3 -c "from playsongs.playsongs import PlaySongs; PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)"
+   python3 -c "from playsongs import PlaySongs; PlaySongs('/home/username/Music', repeat = 10000000, shuffle = True)"
 
 Changelog
 ---------
 
+2023.1.0.0
+
+- Cleaned-up code.
+
 2021.1.4.1
 
 - Multiprocessing bugfix. The songs should advance automatically now.
 
 2021.1.3.1
 
 - Updated README.
```

