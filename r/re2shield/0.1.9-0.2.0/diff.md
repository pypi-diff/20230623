# Comparing `tmp/re2shield-0.1.9.tar.gz` & `tmp/re2shield-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re2shield-0.1.9.tar", last modified: Fri Jun 23 05:32:22 2023, max compression
+gzip compressed data, was "re2shield-0.2.0.tar", last modified: Fri Jun 23 05:39:28 2023, max compression
```

## Comparing `re2shield-0.1.9.tar` & `re2shield-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.571397 re2shield-0.1.9/
--rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:32:22.571397 re2shield-0.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3723 2023-06-23 05:31:56.000000 re2shield-0.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.570397 re2shield-0.1.9/re2shield/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.9/re2shield/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2473 2023-06-23 05:30:27.000000 re2shield-0.1.9/re2shield/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.571397 re2shield-0.1.9/re2shield.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 05:32:22.000000 re2shield-0.1.9/re2shield.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:32:22.571397 re2shield-0.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 05:31:46.000000 re2shield-0.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:32:22.571397 re2shield-0.1.9/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.9/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 04:23:35.000000 re2shield-0.1.9/tests/test_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.187744 re2shield-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:39:28.186744 re2shield-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-06-23 05:39:22.000000 re2shield-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.186744 re2shield-0.2.0/re2shield/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.2.0/re2shield/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-06-23 05:39:11.000000 re2shield-0.2.0/re2shield/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.186744 re2shield-0.2.0/re2shield.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4957 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 05:39:28.000000 re2shield-0.2.0/re2shield.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:39:28.187744 re2shield-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 05:39:25.000000 re2shield-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:39:28.186744 re2shield-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.2.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 04:23:35.000000 re2shield-0.2.0/tests/test_core.py
```

### Comparing `re2shield-0.1.9/PKG-INFO` & `re2shield-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,15 +36,15 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.9
+        ### Version 0.2.0
         - Bug Fix
             - Fixed a bug where pattern compile were not being overwrite.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
```

### Comparing `re2shield-0.1.9/README.md` & `re2shield-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```shell
 git clone https://github.com/Npc-coder/re2shield.git
 cd re2shield
 pip install .
 ```
 
 ## Updates
-### Version 0.1.9
+### Version 0.2.0
 - Bug Fix
     - Fixed a bug where pattern compile were not being overwrite.
 
 Please refer to the [Usage](#usage) section for examples of how to use these new features.
 
 ## Usage
 ### Importing the Library
```

### Comparing `re2shield-0.1.9/re2shield/core.py` & `re2shield-0.2.0/re2shield/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,27 @@
 
     def compile(self, expressions, ids, overwrite=False):
         if len(expressions) != len(ids):
             raise ValueError("All parameters should have the same length")
 
         re2_patterns = {}
         raw_patterns = {}
-        if not overwrite:
+        if not overwrite and self.db is not None:
             re2_patterns = self.db.re2_patterns.copy()
             raw_patterns = self.db.raw_patterns.copy()
 
         for id, expr in zip(ids, expressions):
             if id in re2_patterns:
                 raise ValueError(f"ID {id} already exists in the database. To overwrite, set overwrite=True.")
             re2_patterns[id] = re2.compile(expr)
             raw_patterns[id] = expr
 
         self.db = Re2ShieldDatabase(re2_patterns, raw_patterns)
+        self.pattern_counts = self.db.count_patterns()  # Update pattern_counts after compiling
+
 
     def dump(self, file_path):
         if self.db is not None:
             with open(file_path, 'wb') as f:
                 pickle.dump((self.version, self.db.raw_patterns, self.db.count_patterns()), f)
         else:
             raise ValueError("No compiled database found. Please compile patterns first.")
```

### Comparing `re2shield-0.1.9/re2shield.egg-info/PKG-INFO` & `re2shield-0.2.0/re2shield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,15 +36,15 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.9
+        ### Version 0.2.0
         - Bug Fix
             - Fixed a bug where pattern compile were not being overwrite.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
```

### Comparing `re2shield-0.1.9/setup.py` & `re2shield-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='re2shield',
-    version='0.1.9',
+    version='0.2.0',
     url='https://github.com/Npc-coder/re2shield',  # Replace with your own GitHub project URL
     author='mkCha',
     author_email='dxsaq0@gmail.com',
     description='A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `re2shield-0.1.9/tests/test_core.py` & `re2shield-0.2.0/tests/test_core.py`

 * *Files identical despite different names*

