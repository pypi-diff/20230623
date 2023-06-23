# Comparing `tmp/angola-0.14.0.tar.gz` & `tmp/angola-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.14.0.tar", last modified: Fri Jun 23 08:09:01 2023, max compression
+gzip compressed data, was "angola-0.14.1.tar", last modified: Fri Jun 23 19:27:46 2023, max compression
```

## Comparing `angola-0.14.0.tar` & `angola-0.14.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.198786 angola-0.14.0/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.0/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.0/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 08:09:01.198896 angola-0.14.0/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.0/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-23 08:09:01.199170 angola-0.14.0/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      793 2023-06-23 08:06:55.000000 angola-0.14.0/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.192687 angola-0.14.0/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.196303 angola-0.14.0/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.0/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    50979 2023-06-23 08:06:55.000000 angola-0.14.0/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.0/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.0/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    18566 2023-06-23 07:29:33.000000 angola-0.14.0/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.0/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.197510 angola-0.14.0/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       53 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.198619 angola-0.14.0/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.0/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.0/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.0/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     4793 2023-06-23 08:02:26.000000 angola-0.14.0/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.0/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 19:27:46.518824 angola-0.14.1/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.1/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.1/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 19:27:46.518920 angola-0.14.1/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.1/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-23 19:27:46.519182 angola-0.14.1/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      793 2023-06-23 15:01:11.000000 angola-0.14.1/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 19:27:46.512666 angola-0.14.1/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 19:27:46.516212 angola-0.14.1/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.1/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    50979 2023-06-23 08:06:55.000000 angola-0.14.1/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.1/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.1/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18586 2023-06-23 14:59:38.000000 angola-0.14.1/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.1/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 19:27:46.517346 angola-0.14.1/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 19:27:46.000000 angola-0.14.1/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-23 19:27:46.000000 angola-0.14.1/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-23 19:27:46.000000 angola-0.14.1/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       53 2023-06-23 19:27:46.000000 angola-0.14.1/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-23 19:27:46.000000 angola-0.14.1/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 19:27:46.518725 angola-0.14.1/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.1/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.1/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.1/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     4792 2023-06-23 14:59:38.000000 angola-0.14.1/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.1/tests/test_query.py
```

### Comparing `angola-0.14.0/LICENSE` & `angola-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/PKG-INFO` & `angola-0.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.0
+Version: 0.14.1
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.0/README.md` & `angola-0.14.1/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/setup.py` & `angola-0.14.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.14.0"
+VERSION = "0.14.1"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.14.0/src/angola/database.py` & `angola-0.14.1/src/angola/database.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/src/angola/dict_mutator.py` & `angola-0.14.1/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/src/angola/dict_query.py` & `angola-0.14.1/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/src/angola/lib.py` & `angola-0.14.1/src/angola/lib.py`

 * *Files identical despite different names*

```diff
@@ -65,24 +65,24 @@
 
 def keyname_valid(name:str) -> bool:
     """
     Test if a key name is valid. 
 
     For example, it can test if a key in a dict is valid
 
-    pattern: start with letters or underscrore. Contains alphanum + _
+    pattern: start with letters or underscrore. Contains alphanum + underscore + hyphen
 
     Params:
         name:str
     Returns:
         bool
     """
     if not name or not isinstance(name, str):
         return False
-    pattern = re.compile(r"^[a-zA-Z\_][a-zA-Z0-9\_]*$")
+    pattern = re.compile(r"^[a-zA-Z\_][a-zA-Z0-9\_\-]*$")
     return bool(pattern.match(name)) 
 
 
 
 def gen_xid() -> str:
     """
     Return UUID7. 32 Chars
```

### Comparing `angola-0.14.0/src/angola/lib_xql.py` & `angola-0.14.1/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/src/angola.egg-info/PKG-INFO` & `angola-0.14.1/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.0
+Version: 0.14.1
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.0/tests/test_database.py` & `angola-0.14.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/tests/test_dict_mutator.py` & `angola-0.14.1/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.0/tests/test_lib.py` & `angola-0.14.1/tests/test_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 
 def test_keyname_valid():
     n = [
         ("a", True), ("ab", True), ("abC", True), ("hello", True), ("World", True), 
         ("WORDL", True), ("WORLD1", True), ("woRld7_", True), ("somethin_g", True), 
         ("_under", True), ("__double", True),
-        ("", False), ("0", False), ("0Boom", False),("-something", False), ("somet-hing", False),
+        ("", False), ("0", False), ("0Boom", False),("-something", False), ("somet-hing", True),
         (0, False), (None, False), (True, False), (False, False)
     ]
     for k in n: 
         assert lib.keyname_valid(k[0]) is k[1]
 
 def test_dict_inspect_valid_keyname():
     d = {
```

