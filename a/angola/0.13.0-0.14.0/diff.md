# Comparing `tmp/angola-0.13.0.tar.gz` & `tmp/angola-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.13.0.tar", last modified: Fri Jun 23 04:35:40 2023, max compression
+gzip compressed data, was "angola-0.14.0.tar", last modified: Fri Jun 23 08:09:01 2023, max compression
```

## Comparing `angola-0.13.0.tar` & `angola-0.14.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.852900 angola-0.13.0/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.13.0/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.13.0/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 04:35:40.852969 angola-0.13.0/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.13.0/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-23 04:35:40.853207 angola-0.13.0/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      793 2023-06-23 04:35:13.000000 angola-0.13.0/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.847959 angola-0.13.0/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.850616 angola-0.13.0/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.13.0/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-23 04:30:25.000000 angola-0.13.0/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.13.0/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.13.0/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17512 2023-06-23 04:30:25.000000 angola-0.13.0/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.13.0/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.851390 angola-0.13.0/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       53 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-23 04:35:40.000000 angola-0.13.0/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 04:35:40.852797 angola-0.13.0/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.13.0/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.13.0/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.13.0/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.13.0/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.13.0/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.198786 angola-0.14.0/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.0/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.0/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 08:09:01.198896 angola-0.14.0/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.0/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-23 08:09:01.199170 angola-0.14.0/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      793 2023-06-23 08:06:55.000000 angola-0.14.0/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.192687 angola-0.14.0/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.196303 angola-0.14.0/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.0/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    50979 2023-06-23 08:06:55.000000 angola-0.14.0/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.0/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.0/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18566 2023-06-23 07:29:33.000000 angola-0.14.0/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.0/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.197510 angola-0.14.0/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       53 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-23 08:09:01.000000 angola-0.14.0/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-23 08:09:01.198619 angola-0.14.0/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.0/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.0/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.0/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     4793 2023-06-23 08:02:26.000000 angola-0.14.0/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.0/tests/test_query.py
```

### Comparing `angola-0.13.0/LICENSE` & `angola-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.13.0/PKG-INFO` & `angola-0.14.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.13.0
+Version: 0.14.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.13.0/README.md` & `angola-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.13.0/setup.py` & `angola-0.14.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.13.0"
+VERSION = "0.14.0"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.13.0/src/angola/database.py` & `angola-0.14.0/src/angola/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1204,20 +1204,23 @@
             item:CollectionItem
             replace_document:bool - To replace instead of updating. Replace will not merge the data.
         """
         if not item._key:
             raise MissingItemKeyError()
         try:
             if replace_document:
+                lib.dict_inspect_valid_keyname(item.to_dict())
                 return self.collection.replace(item.to_dict(), return_new=True)["new"]
             else:
                 item.timestamp('_modified_at')
+                lib.dict_inspect_valid_keyname(item.to_dict())
                 return self.collection.update(item.to_dict(), return_new=True)["new"]
         except DocumentUpdateError as due:
             item.update({"_modified_at": None})
+            lib.dict_inspect_valid_keyname(item.to_dict())
             return self.collection.insert(item.to_dict(), return_new=True)["new"]
 
     def __iter__(self):
         return self.find(filters={})
 
     def item(self, data:dict, read_only:bool=False) -> CollectionItem:
         """
```

### Comparing `angola-0.13.0/src/angola/dict_mutator.py` & `angola-0.14.0/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.13.0/src/angola/dict_query.py` & `angola-0.14.0/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.13.0/src/angola/lib.py` & `angola-0.14.0/src/angola/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,23 +48,44 @@
         
     Return: int 
     """
     return sys.getsizeof(json_dumps(obj))
 
 
 
-def collection_name_valid(name):
+def collection_name_valid(name:str) -> bool:
     """
     Valid a collection name 
     length: 2, 64
     pattern: lowercase, letters and numbers and underscore
     """
+    if not name or not isinstance(name, str):
+        return False
     pattern = re.compile(r"^[a-z][a-z0-9\_]{2,64}$")
     return bool(pattern.match(name)) 
 
+def keyname_valid(name:str) -> bool:
+    """
+    Test if a key name is valid. 
+
+    For example, it can test if a key in a dict is valid
+
+    pattern: start with letters or underscrore. Contains alphanum + _
+
+    Params:
+        name:str
+    Returns:
+        bool
+    """
+    if not name or not isinstance(name, str):
+        return False
+    pattern = re.compile(r"^[a-zA-Z\_][a-zA-Z0-9\_]*$")
+    return bool(pattern.match(name)) 
+
+
 
 def gen_xid() -> str:
     """
     Return UUID7. 32 Chars
     """
     return str(uuid7()).replace("-", "")
 
@@ -535,14 +556,32 @@
     """
     To order a list of dict, by the value in the dict
 
     list_sorted_dict(list, "name")
     """
     return sorted(l, key=itemgetter(key))
 
+def dict_inspect_valid_keyname(obj:dict) -> bool:
+    """
+    Inspect a dict valid keys
+    It goes recursively. 
+    Will raise errors if a key is invalid
+    """
+    for k, v in obj.items():
+        if isinstance(v, dict):
+            dict_inspect_valid_keyname(v)
+        elif isinstance(v, list):
+            for l in v:
+                if isinstance(l, dict):
+                    dict_inspect_valid_keyname(l)
+
+        if keyname_valid(k) is False:
+            raise NameError("INVALID_DATA_KEY_ERROR:%s" % k)
+    return True
+        
 #===
 
 def hash_string(s):
     return hashlib.sha256(s.encode('utf-8')).hexdigest()
 
 
 def calc_pagination_offset(page: int, per_page: int) -> int:
```

### Comparing `angola-0.13.0/src/angola/lib_xql.py` & `angola-0.14.0/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.13.0/src/angola.egg-info/PKG-INFO` & `angola-0.14.0/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.13.0
+Version: 0.14.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.13.0/tests/test_database.py` & `angola-0.14.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.13.0/tests/test_dict_mutator.py` & `angola-0.14.0/tests/test_dict_mutator.py`

 * *Files identical despite different names*

