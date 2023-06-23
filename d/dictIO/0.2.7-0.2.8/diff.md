# Comparing `tmp/dictIO-0.2.7.tar.gz` & `tmp/dictIO-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictIO-0.2.7.tar", last modified: Thu May  4 12:12:35 2023, max compression
+gzip compressed data, was "dictIO-0.2.8.tar", last modified: Fri Jun 23 16:47:40 2023, max compression
```

## Comparing `dictIO-0.2.7.tar` & `dictIO-0.2.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 12:12:17.000000 dictIO-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 12:12:17.000000 dictIO-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-04 12:12:35.847202 dictIO-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-04 12:12:17.000000 dictIO-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-04 12:12:17.000000 dictIO-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-04 12:12:35.851202 dictIO-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.839202 dictIO-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.843202 dictIO-0.2.7/src/dictIO/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/src/dictIO/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/cli/dictParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23370 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/cppDict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/dictParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/dictReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/dictWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    69630 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/src/dictIO/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-04 12:12:17.000000 dictIO-0.2.7/src/dictIO/utils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.843202 dictIO-0.2.7/src/dictIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 12:12:35.000000 dictIO-0.2.7/src/dictIO.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:12:35.847202 dictIO-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dictParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    22497 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dictReader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_dictWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22074 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    55082 2023-05-04 12:12:17.000000 dictIO-0.2.7/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:40.291132 dictIO-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-23 16:47:24.000000 dictIO-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 16:47:24.000000 dictIO-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-23 16:47:40.291132 dictIO-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-23 16:47:24.000000 dictIO-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-23 16:47:24.000000 dictIO-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-23 16:47:40.291132 dictIO-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:40.283132 dictIO-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:40.287132 dictIO-0.2.8/src/dictIO/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:40.287132 dictIO-0.2.8/src/dictIO/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/cli/dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23420 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/cppDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/dictReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/dictWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69630 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:40.287132 dictIO-0.2.8/src/dictIO/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/utils/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-23 16:47:24.000000 dictIO-0.2.8/src/dictIO/utils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:40.287132 dictIO-0.2.8/src/dictIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-23 16:47:40.000000 dictIO-0.2.8/src/dictIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-23 16:47:40.000000 dictIO-0.2.8/src/dictIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:47:40.000000 dictIO-0.2.8/src/dictIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 16:47:40.000000 dictIO-0.2.8/src/dictIO.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 16:47:40.000000 dictIO-0.2.8/src/dictIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 16:47:40.000000 dictIO-0.2.8/src/dictIO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:47:40.291132 dictIO-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-23 16:47:24.000000 dictIO-0.2.8/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-23 16:47:24.000000 dictIO-0.2.8/tests/test_dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22535 2023-06-23 16:47:24.000000 dictIO-0.2.8/tests/test_dictReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-06-23 16:47:24.000000 dictIO-0.2.8/tests/test_dictWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22074 2023-06-23 16:47:24.000000 dictIO-0.2.8/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55255 2023-06-23 16:47:24.000000 dictIO-0.2.8/tests/test_parser.py
```

### Comparing `dictIO-0.2.7/LICENSE` & `dictIO-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/PKG-INFO` & `dictIO-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictIO
-Version: 0.2.7
+Version: 0.2.8
 Summary: Read, write and manipulate dictionary text files.
 Home-page: https://dnv-opensource.github.io/dictIO/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
```

### Comparing `dictIO-0.2.7/README.md` & `dictIO-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/pyproject.toml` & `dictIO-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/setup.cfg` & `dictIO-0.2.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dictIO
-version = 0.2.7
+version = 0.2.8
 summary = Read, write and manipulate dictionary text files.
 description = Python package to read, write and manipulate dictionary text files. Supports dictIOs dict file format, as well as JSON, XML and OpenFOAM.
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://dnv-opensource.github.io/dictIO/README.html
 project_urls = 
 	GitHub = https://github.com/dnv-opensource/dictIO
```

### Comparing `dictIO-0.2.7/src/dictIO/__init__.py` & `dictIO-0.2.8/src/dictIO/__init__.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/cli/dictParser.py` & `dictIO-0.2.8/src/dictIO/cli/dictParser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/cppDict.py` & `dictIO-0.2.8/src/dictIO/cppDict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pyright: reportIncompatibleMethodOverride=false
 import contextlib
 import logging
 import os
 import re
 from collections import UserDict
 from pathlib import Path
 from typing import (
```

### Comparing `dictIO-0.2.7/src/dictIO/dictParser.py` & `dictIO-0.2.8/src/dictIO/dictParser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/dictReader.py` & `dictIO-0.2.8/src/dictIO/dictReader.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/dictWriter.py` & `dictIO-0.2.8/src/dictIO/dictWriter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/formatter.py` & `dictIO-0.2.8/src/dictIO/formatter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/parser.py` & `dictIO-0.2.8/src/dictIO/parser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/utils/counter.py` & `dictIO-0.2.8/src/dictIO/utils/counter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/utils/logging.py` & `dictIO-0.2.8/src/dictIO/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/utils/path.py` & `dictIO-0.2.8/src/dictIO/utils/path.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO/utils/strings.py` & `dictIO-0.2.8/src/dictIO/utils/strings.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/src/dictIO.egg-info/PKG-INFO` & `dictIO-0.2.8/src/dictIO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictIO
-Version: 0.2.7
+Version: 0.2.8
 Summary: Read, write and manipulate dictionary text files.
 Home-page: https://dnv-opensource.github.io/dictIO/README.html
 Author: Frank Lumpitzsch
 Author-email: "Frank Lumpitzsch" <frank.lumpitzsch@dnv.com>
 Maintainer: Claas Rostock
 Maintainer-email: "Claas Rostock" <claas.rostock@dnv.com>
 License: MIT
```

### Comparing `dictIO-0.2.7/src/dictIO.egg-info/SOURCES.txt` & `dictIO-0.2.8/src/dictIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/tests/test_dict.py` & `dictIO-0.2.8/tests/test_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 def test_init_with_file():  # sourcery skip: avoid-builtin-shadow
     dict = CppDict("someDict")
     assert dict.path == Path.cwd()
     assert dict.source_file == Path.cwd() / "someDict"
 
 
 def test_find_global_key():
+    # sourcery skip: no-loop-in-tests
     # Prepare
     str_in_1 = "PLACEHOLDER000001"
     str_in_2 = "PLACEHOLDER000002"
     str_in_3 = "PLACEHOLDER000003"
     not_a_str_1 = 1234
     not_a_str_2 = 1.23
     not_a_str_3 = False
@@ -205,14 +206,15 @@
     assert dict_out[keydld][keyld][0][key_3] == str_out_3
     assert dict_out[keyldl][0][keyl][0] == str_out_1
     assert dict_out[keyldl][0][keyl][1] == str_out_2
     assert dict_out[keyldl][0][keyl][2] == str_out_3
 
 
 def test_order_keys():  # sourcery skip: avoid-builtin-shadow
+    # sourcery skip: no-loop-in-tests
     # Prepare
     str_1 = "string 1"
     str_2 = "string 2"
     str_3 = "string 3"
     not_a_str_1 = 1234
     not_a_str_2 = 1.23
     not_a_str_3 = False
```

### Comparing `dictIO-0.2.7/tests/test_dictParser.py` & `dictIO-0.2.8/tests/test_dictParser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/tests/test_dictReader.py` & `dictIO-0.2.8/tests/test_dictReader.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,15 @@
     assert dict["keyK"] == [2.7, 8.1]
     assert dict["keyL"] == [[0.3, 0.9], [2.7, 8.1]]
     assert dict["keyM"] == 9.0
     assert dict["keyN"] == 7.0
 
 
 def test_compare_expressions_in_dict_format_with_expressions_in_json_format():
+    # sourcery skip: no-loop-in-tests
     # Prepare
     source_file_dict = Path("test_dictReader_dict")
     source_file_json = Path("test_dictReader_json.json")
     # Execute
     dict_dict = DictReader.read(source_file_dict)
     dict_json = DictReader.read(source_file_json)
     # Assert
```

### Comparing `dictIO-0.2.7/tests/test_dictWriter.py` & `dictIO-0.2.8/tests/test_dictWriter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/tests/test_formatter.py` & `dictIO-0.2.8/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.2.7/tests/test_parser.py` & `dictIO-0.2.8/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyright: reportPrivateUsage=false
 import re
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict
+from typing import Dict, List, Tuple
 
 import pytest
 from pytest import LogCaptureFixture
 
 from dictIO import CppDict, CppParser, Parser, XmlParser
 from dictIO.utils.counter import BorgCounter
 from dictIO.utils.strings import string_diff
@@ -338,14 +338,15 @@
         assert target_dict.path == source_file.parent
         assert target_dict.name == source_file.name
 
 
 class TestCppParser:
     def test_extract_line_comments(self):
         # sourcery skip: avoid-builtin-shadow
+        # sourcery skip: no-loop-in-tests
         # Prepare
         dict = CppDict()
         parser = CppParser()
         line1 = "a line with no line comment\n"
         line2 = "//a line comment\n"
         line3 = "a line with //an inline comment\n"
         line4 = "a line with no line comment\n"
@@ -359,14 +360,15 @@
             assert re.search(r"//", line) is None
         assert len(dict.line_comments) == 2
         for line in dict.line_comments.values():
             assert re.search("//", str(line)) is not None
 
     def test_extract_includes(self):
         # sourcery skip: avoid-builtin-shadow
+        # sourcery skip: no-loop-in-tests
         # Prepare
         dict = CppDict()
         parser = CppParser()
         line1 = "a line with no include directive\n"
         line2 = "#include testDict\n"
         line3 = "#include 'testDict'\n"
         line4 = '#include "testDict"\n'
@@ -595,14 +597,15 @@
         assert list(dict.expressions.values())[7]["expression"] == "$varName1[0]"
 
         assert list(dict.expressions.values())[8]["name"][:10] == "EXPRESSION"
         assert list(dict.expressions.values())[8]["expression"] == "$varName1[1][2]"
 
     def test_separate_delimiters(self):
         # sourcery skip: avoid-builtin-shadow
+        # sourcery skip: no-loop-in-tests
         # Prepare
         dict = CppDict()
         parser = CppParser()
         text_block_in = (
             "This is a text block\n"
             "with multiple lines. Within this text block there are distinct chars that shall be identified as delimiters.\n"
             "All chars that shall be identified delimiters are passed to _separate_delimiters as a list of chars.\n"
@@ -651,16 +654,16 @@
         dict = CppDict()
         parser = CppParser()
         text_block = (
             "level0 { level1 { level2 { level3 } level2 } level1 } level0\n"
             "level0 [ level1 [ level2 [ level3 ] level2 ] level1 ] level0\n"
             "level0 ( level1 ( level2 ( level3 ) level2 ) level1 ) level0"
         )
-        tokens = re.split(r"\s", text_block)
-        tokens_in = [(0, token) for token in tokens]
+        tokens: List[str] = re.split(r"\s", text_block)
+        tokens_in: List[Tuple[int, str]] = [(0, token) for token in tokens]
         levels_expected = [0, 0, 1, 1, 2, 2, 3, 2, 2, 1, 1, 0, 0] * 3
         tokens_expected = list(zip(levels_expected, tokens))
         dict.tokens = tokens_in
         # Execute
         parser._determine_token_hierarchy(dict)
         # Assert
         assert dict.tokens == tokens_expected
```

