# Comparing `tmp/miniirc_matrix-0.0.8.tar.gz` & `tmp/miniirc_matrix-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniirc_matrix-0.0.8.tar", last modified: Thu Nov 17 20:36:41 2022, max compression
+gzip compressed data, was "miniirc_matrix-0.0.9.tar", last modified: Sun Dec 25 22:22:38 2022, max compression
```

## Comparing `miniirc_matrix-0.0.8.tar` & `miniirc_matrix-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 20:36:41.949710 miniirc_matrix-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2022-11-17 20:36:22.000000 miniirc_matrix-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2022-11-17 20:36:41.949710 miniirc_matrix-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2022-11-17 20:36:22.000000 miniirc_matrix-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-17 20:36:41.949710 miniirc_matrix-0.0.8/miniirc_matrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2022-11-17 20:36:41.000000 miniirc_matrix-0.0.8/miniirc_matrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      236 2022-11-17 20:36:41.000000 miniirc_matrix-0.0.8/miniirc_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-17 20:36:41.000000 miniirc_matrix-0.0.8/miniirc_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-17 20:36:41.000000 miniirc_matrix-0.0.8/miniirc_matrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-17 20:36:41.000000 miniirc_matrix-0.0.8/miniirc_matrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    27686 2022-11-17 20:36:22.000000 miniirc_matrix-0.0.8/miniirc_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-17 20:36:41.949710 miniirc_matrix-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      784 2022-11-17 20:36:22.000000 miniirc_matrix-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 22:22:38.749647 miniirc_matrix-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2022-12-25 22:22:24.000000 miniirc_matrix-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2022-12-25 22:22:38.749647 miniirc_matrix-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2022-12-25 22:22:24.000000 miniirc_matrix-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 22:22:38.749647 miniirc_matrix-0.0.9/miniirc_matrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2022-12-25 22:22:38.000000 miniirc_matrix-0.0.9/miniirc_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-25 22:22:38.000000 miniirc_matrix-0.0.9/miniirc_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-25 22:22:38.000000 miniirc_matrix-0.0.9/miniirc_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-25 22:22:38.000000 miniirc_matrix-0.0.9/miniirc_matrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-25 22:22:38.000000 miniirc_matrix-0.0.9/miniirc_matrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27720 2022-12-25 22:22:24.000000 miniirc_matrix-0.0.9/miniirc_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-25 22:22:38.749647 miniirc_matrix-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2022-12-25 22:22:24.000000 miniirc_matrix-0.0.9/setup.py
```

### Comparing `miniirc_matrix-0.0.8/LICENSE.md` & `miniirc_matrix-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniirc_matrix-0.0.8/PKG-INFO` & `miniirc_matrix-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniirc_matrix
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Matrix wrapper for miniirc.
 Author: luk3yx
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miniirc_matrix-0.0.8/README.md` & `miniirc_matrix-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `miniirc_matrix-0.0.8/miniirc_matrix.egg-info/PKG-INFO` & `miniirc_matrix-0.0.9/miniirc_matrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniirc-matrix
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Matrix wrapper for miniirc.
 Author: luk3yx
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miniirc_matrix-0.0.8/miniirc_matrix.py` & `miniirc_matrix-0.0.9/miniirc_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # Copyright © 2021 by luk3yx
 #
 
 from __future__ import annotations
 from collections.abc import Callable
 from typing import Any, Optional, TypeVar, overload
 from urllib.parse import quote as _url_quote, urlparse as _urlparse
-import functools, html.parser, itertools, json, math, re, threading, time, uuid
+import functools, html.parser, itertools, json, math, re, time, uuid
 import miniirc, requests, traceback  # type: ignore
 
 
-ver = (0, 0, 8)
+ver = (0, 0, 9)
 __version__ = '.'.join(map(str, ver))
 
 
 def _room_processor(*event_names: str):
     def _make_wrapper(f: Callable[[Matrix, str, dict[str, Any]], None]
                       ) -> Callable[[Matrix, dict[str, Any]], None]:
         @functools.wraps(f)
@@ -253,15 +253,17 @@
             raise _UnknownTagError(tag)
 
     def handle_endtag(self, tag: str) -> None:
         if self.in_reply:
             if tag in ('mx-reply', 'script'):
                 self.in_reply -= 1
             return
-        if tag in self.irc_codes:
+        if tag == 'br':
+            return
+        elif tag in self.irc_codes:
             self.text.append(self.irc_codes[tag])
         elif tag != 'font':
             raise _UnknownTagError(tag)
 
     def handle_data(self, data: str) -> None:
         if not self.in_reply:
             self.text.append(data)
```

### Comparing `miniirc_matrix-0.0.8/setup.py` & `miniirc_matrix-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 
 import pathlib
 from setuptools import setup
 
 setup(
     name='miniirc_matrix',
-    version='0.0.8',
+    version='0.0.9',
     py_modules=['miniirc_matrix'],
     author='luk3yx',
     description='A Matrix wrapper for miniirc.',
     license='MIT',
 
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
```

