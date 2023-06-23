# Comparing `tmp/re2shield-0.1.8.tar.gz` & `tmp/re2shield-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re2shield-0.1.8.tar", last modified: Fri Jun 23 05:02:18 2023, max compression
+gzip compressed data, was "re2shield-0.1.9.tar", last modified: Fri Jun 23 05:32:22 2023, max compression
```

## Comparing `re2shield-0.1.8.tar` & `re2shield-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     4965 2023-06-23 05:02:18.428336 re2shield-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3731 2023-06-23 04:59:33.000000 re2shield-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/re2shield/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.8/re2shield/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-06-23 05:01:27.000000 re2shield-0.1.8/re2shield/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/re2shield.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4965 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 05:02:18.000000 re2shield-0.1.8/re2shield.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:02:18.428336 re2shield-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 04:59:20.000000 re2shield-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:02:18.428336 re2shield-0.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 04:23:35.000000 re2shield-0.1.8/tests/test_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.571397 re2shield-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:32:22.571397 re2shield-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-06-23 05:31:56.000000 re2shield-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.570397 re2shield-0.1.9/re2shield/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.9/re2shield/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-23 05:30:27.000000 re2shield-0.1.9/re2shield/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.571397 re2shield-0.1.9/re2shield.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:32:22.571397 re2shield-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 05:31:46.000000 re2shield-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.571397 re2shield-0.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 04:23:35.000000 re2shield-0.1.9/tests/test_core.py
```

### Comparing `re2shield-0.1.8/PKG-INFO` & `re2shield-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.8
+Version: 0.1.9
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
-        ### Version 0.1.8
+        ### Version 0.1.9
         - Bug Fix
-            - Fixed a bug where pattern count were not being displayed correctly.
+            - Fixed a bug where pattern compile were not being overwrite.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
```

### Comparing `re2shield-0.1.8/README.md` & `re2shield-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 ```shell
 git clone https://github.com/Npc-coder/re2shield.git
 cd re2shield
 pip install .
 ```
 
 ## Updates
-### Version 0.1.8
+### Version 0.1.9
 - Bug Fix
-    - Fixed a bug where pattern count were not being displayed correctly.
+    - Fixed a bug where pattern compile were not being overwrite.
 
 Please refer to the [Usage](#usage) section for examples of how to use these new features.
 
 ## Usage
 ### Importing the Library
 Here is a simple example demonstrating how to use re2shield:
```

### Comparing `re2shield-0.1.8/re2shield/core.py` & `re2shield-0.1.9/re2shield/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def compile(self, expressions, ids, overwrite=False):
         if len(expressions) != len(ids):
             raise ValueError("All parameters should have the same length")
 
         re2_patterns = {}
         raw_patterns = {}
-        if not overwrite and self.db is not None:
+        if not overwrite:
             re2_patterns = self.db.re2_patterns.copy()
             raw_patterns = self.db.raw_patterns.copy()
 
         for id, expr in zip(ids, expressions):
             if id in re2_patterns:
                 raise ValueError(f"ID {id} already exists in the database. To overwrite, set overwrite=True.")
             re2_patterns[id] = re2.compile(expr)
```

### Comparing `re2shield-0.1.8/re2shield.egg-info/PKG-INFO` & `re2shield-0.1.9/re2shield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.8
+Version: 0.1.9
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
-        ### Version 0.1.8
+        ### Version 0.1.9
         - Bug Fix
-            - Fixed a bug where pattern count were not being displayed correctly.
+            - Fixed a bug where pattern compile were not being overwrite.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
```

### Comparing `re2shield-0.1.8/setup.py` & `re2shield-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='re2shield',
-    version='0.1.8',
+    version='0.1.9',
     url='https://github.com/Npc-coder/re2shield',  # Replace with your own GitHub project URL
     author='mkCha',
     author_email='dxsaq0@gmail.com',
     description='A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `re2shield-0.1.8/tests/test_core.py` & `re2shield-0.1.9/tests/test_core.py`

 * *Files identical despite different names*

