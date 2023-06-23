# Comparing `tmp/re2shield-0.1.7.tar.gz` & `tmp/re2shield-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re2shield-0.1.7.tar", last modified: Fri Jun 23 04:23:52 2023, max compression
+gzip compressed data, was "re2shield-0.1.8.tar", last modified: Fri Jun 23 05:02:18 2023, max compression
```

## Comparing `re2shield-0.1.7.tar` & `re2shield-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 04:23:52.064174 re2shield-0.1.7/
--rw-r--r--   0 root         (0) root         (0)     4981 2023-06-23 04:23:52.064174 re2shield-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3747 2023-06-23 04:10:01.000000 re2shield-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 04:23:52.063174 re2shield-0.1.7/re2shield/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.7/re2shield/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-06-23 04:22:38.000000 re2shield-0.1.7/re2shield/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 04:23:52.064174 re2shield-0.1.7/re2shield.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4981 2023-06-23 04:23:52.000000 re2shield-0.1.7/re2shield.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 04:23:52.000000 re2shield-0.1.7/re2shield.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 04:23:52.000000 re2shield-0.1.7/re2shield.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 04:23:52.000000 re2shield-0.1.7/re2shield.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 04:23:52.000000 re2shield-0.1.7/re2shield.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 04:23:52.064174 re2shield-0.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 04:10:29.000000 re2shield-0.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 04:23:52.064174 re2shield-0.1.7/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 04:23:35.000000 re2shield-0.1.7/tests/test_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-06-23 05:02:18.428336 re2shield-0.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-06-23 04:59:33.000000 re2shield-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/re2shield/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.8/re2shield/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-06-23 05:01:27.000000 re2shield-0.1.8/re2shield/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/re2shield.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:02:18.428336 re2shield-0.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 04:59:20.000000 re2shield-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 04:23:35.000000 re2shield-0.1.8/tests/test_core.py
```

### Comparing `re2shield-0.1.7/PKG-INFO` & `re2shield-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,17 +36,17 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.7
+        ### Version 0.1.8
         - Bug Fix
-            - Fixed a bug where the version and pattern count were not being displayed correctly.
+            - Fixed a bug where pattern count were not being displayed correctly.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
```

### Comparing `re2shield-0.1.7/README.md` & `re2shield-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 ```shell
 git clone https://github.com/Npc-coder/re2shield.git
 cd re2shield
 pip install .
 ```
 
 ## Updates
-### Version 0.1.7
+### Version 0.1.8
 - Bug Fix
-    - Fixed a bug where the version and pattern count were not being displayed correctly.
+    - Fixed a bug where pattern count were not being displayed correctly.
 
 Please refer to the [Usage](#usage) section for examples of how to use these new features.
 
 ## Usage
 ### Importing the Library
 Here is a simple example demonstrating how to use re2shield:
```

### Comparing `re2shield-0.1.7/re2shield/core.py` & `re2shield-0.1.8/re2shield/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 class Re2Shield:
     def __init__(self, version=None, pattern_counts=0):
         self.db = None
         self.version = version
         self.pattern_counts = pattern_counts
 
     def __str__(self):
-        self.pattern_counts = self.db.count_patterns() if self.db is not None else 0
         message = {
             "version": self.version,
             "pattern_counts": self.pattern_counts
         }
         return str(message)
 
     def compile(self, expressions, ids, overwrite=False):
@@ -46,26 +45,26 @@
             raw_patterns[id] = expr
 
         self.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
 
     def dump(self, file_path):
         if self.db is not None:
             with open(file_path, 'wb') as f:
-                pickle.dump((self.version, self.db.raw_patterns), f)
+                pickle.dump((self.version, self.db.raw_patterns, self.db.count_patterns()), f)
         else:
             raise ValueError("No compiled database found. Please compile patterns first.")
 
     def scan(self, text, callback):
         if self.db is not None:
             self.db.findall(text, callback)
         else:
             raise ValueError("No compiled database found. Please compile patterns first.")
 
 Database = Re2Shield
 
 def load(file_path):
     with open(file_path, 'rb') as f:
-        version, raw_patterns = pickle.load(f)
+        version, raw_patterns, pattern_counts = pickle.load(f)
         re2_patterns = {id: re2.compile(expr) for id, expr in raw_patterns.items()}
-    re2_shield = Re2Shield(version=version)
+    re2_shield = Re2Shield(version=version, pattern_counts=pattern_counts)
     re2_shield.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
     return re2_shield
```

### Comparing `re2shield-0.1.7/re2shield.egg-info/PKG-INFO` & `re2shield-0.1.8/re2shield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,17 +36,17 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.7
+        ### Version 0.1.8
         - Bug Fix
-            - Fixed a bug where the version and pattern count were not being displayed correctly.
+            - Fixed a bug where pattern count were not being displayed correctly.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
```

### Comparing `re2shield-0.1.7/setup.py` & `re2shield-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='re2shield',
-    version='0.1.7',
+    version='0.1.8',
     url='https://github.com/Npc-coder/re2shield',  # Replace with your own GitHub project URL
     author='mkCha',
     author_email='dxsaq0@gmail.com',
     description='A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `re2shield-0.1.7/tests/test_core.py` & `re2shield-0.1.8/tests/test_core.py`

 * *Files identical despite different names*

