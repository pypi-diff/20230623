# Comparing `tmp/re2shield-0.1.5.tar.gz` & `tmp/re2shield-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re2shield-0.1.5.tar", last modified: Wed Jun 21 02:39:11 2023, max compression
+gzip compressed data, was "re2shield-0.1.6.tar", last modified: Fri Jun 23 02:28:04 2023, max compression
```

## Comparing `re2shield-0.1.5.tar` & `re2shield-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:39:11.965300 re2shield-0.1.5/
--rw-r--r--   0 root         (0) root         (0)     5263 2023-06-21 02:39:11.965300 re2shield-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4029 2023-06-21 02:39:10.000000 re2shield-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:39:11.964300 re2shield-0.1.5/re2shield/
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.5/re2shield/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2317 2023-06-21 02:37:21.000000 re2shield-0.1.5/re2shield/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:39:11.965300 re2shield-0.1.5/re2shield.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5263 2023-06-21 02:39:11.000000 re2shield-0.1.5/re2shield.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      259 2023-06-21 02:39:11.000000 re2shield-0.1.5/re2shield.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 02:39:11.000000 re2shield-0.1.5/re2shield.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-21 02:39:11.000000 re2shield-0.1.5/re2shield.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-21 02:39:11.000000 re2shield-0.1.5/re2shield.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 02:39:11.965300 re2shield-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      859 2023-06-21 02:29:25.000000 re2shield-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:39:11.965300 re2shield-0.1.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-21 02:33:56.000000 re2shield-0.1.5/tests/test_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 02:28:04.160641 re2shield-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)     5228 2023-06-23 02:28:04.160641 re2shield-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-06-23 02:27:01.000000 re2shield-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 02:28:04.159641 re2shield-0.1.6/re2shield/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:41:51.000000 re2shield-0.1.6/re2shield/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-06-23 02:11:42.000000 re2shield-0.1.6/re2shield/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 02:28:04.160641 re2shield-0.1.6/re2shield.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5228 2023-06-23 02:28:04.000000 re2shield-0.1.6/re2shield.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      259 2023-06-23 02:28:04.000000 re2shield-0.1.6/re2shield.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 02:28:04.000000 re2shield-0.1.6/re2shield.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 02:28:04.000000 re2shield-0.1.6/re2shield.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 02:28:04.000000 re2shield-0.1.6/re2shield.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 02:28:04.160641 re2shield-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      859 2023-06-23 02:05:22.000000 re2shield-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 02:28:04.160641 re2shield-0.1.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 07:41:51.000000 re2shield-0.1.6/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-23 02:24:23.000000 re2shield-0.1.6/tests/test_core.py
```

### Comparing `re2shield-0.1.5/PKG-INFO` & `re2shield-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,46 +36,45 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.5
-        - Reverted the change that automatically assigned IDs to patterns. Now the compile method requires both a list of regular expressions and a list of corresponding IDs, allowing users to specify the ID for each pattern.
-        - Improved the compile method to check for ID duplication among both new and existing patterns in the database. If a duplicate ID is found and overwrite is False, a ValueError is raised.
+        ### Version 0.1.6
+        - The __str__ method has been updated. Now, it returns a string that includes the version of the Re2Shield object and the number of patterns in the database. If the database has not been compiled, the number of patterns is displayed as 0. With this change, it is guaranteed that a string is always returned when printing the Re2Shield object as a string.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
         
         ```python
         import re2shield
         
         if __name__ == "__main__":
             db = re2shield.Database()
-        
+            print(db)
             # Load patterns from file
             try:
-                db = re2shield.load('patterns.pkl')
+                db = re2shield.load('patterns.db')
                 print(db)  # Prints the number of patterns in the database
             except FileNotFoundError:
                 # If pattern file doesn't exist, compile the patterns
                 patterns = [
                     (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
                     (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
                     (r'\d+', 3)
                 ]
         
                 expressions, ids = zip(*patterns)
                 db.compile(expressions=expressions, ids=ids, overwrite=False)
-                print(db)  # Prints the number of patterns in the database
-                db.dump('patterns.pkl')
+                print(db)  # Prints the number of patterns in the database and version
+                db.dump('patterns.db')
         
             # Find patterns in text
             def match_handler(id, from_, to, flags, context):
                 print(f"Match found for pattern {id} from {from_} to {to}: {context}")
         
             db.scan('test@ex12ample12.com', match_handler)
         ```
```

### Comparing `re2shield-0.1.5/README.md` & `re2shield-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -28,46 +28,45 @@
 ```shell
 git clone https://github.com/Npc-coder/re2shield.git
 cd re2shield
 pip install .
 ```
 
 ## Updates
-### Version 0.1.5
-- Reverted the change that automatically assigned IDs to patterns. Now the compile method requires both a list of regular expressions and a list of corresponding IDs, allowing users to specify the ID for each pattern.
-- Improved the compile method to check for ID duplication among both new and existing patterns in the database. If a duplicate ID is found and overwrite is False, a ValueError is raised.
+### Version 0.1.6
+- The __str__ method has been updated. Now, it returns a string that includes the version of the Re2Shield object and the number of patterns in the database. If the database has not been compiled, the number of patterns is displayed as 0. With this change, it is guaranteed that a string is always returned when printing the Re2Shield object as a string.
 
 Please refer to the [Usage](#usage) section for examples of how to use these new features.
 
 ## Usage
 ### Importing the Library
 Here is a simple example demonstrating how to use re2shield:
 
 ```python
 import re2shield
 
 if __name__ == "__main__":
     db = re2shield.Database()
-
+    print(db)
     # Load patterns from file
     try:
-        db = re2shield.load('patterns.pkl')
+        db = re2shield.load('patterns.db')
         print(db)  # Prints the number of patterns in the database
     except FileNotFoundError:
         # If pattern file doesn't exist, compile the patterns
         patterns = [
             (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
             (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
             (r'\d+', 3)
         ]
 
         expressions, ids = zip(*patterns)
         db.compile(expressions=expressions, ids=ids, overwrite=False)
-        print(db)  # Prints the number of patterns in the database
-        db.dump('patterns.pkl')
+        print(db)  # Prints the number of patterns in the database and version
+        db.dump('patterns.db')
 
     # Find patterns in text
     def match_handler(id, from_, to, flags, context):
         print(f"Match found for pattern {id} from {from_} to {to}: {context}")
 
     db.scan('test@ex12ample12.com', match_handler)
 ```
```

### Comparing `re2shield-0.1.5/re2shield/core.py` & `re2shield-0.1.6/re2shield/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 
     def count_patterns(self):
         return len(self.re2_patterns)
 
 class Re2Shield:
     def __init__(self):
         self.db = None
+        self.version = None
 
     def __str__(self):
-        if self.db is not None:
-            return f"Re2Shield Database with {self.db.count_patterns()} patterns."
-        else:
-            return "Re2Shield Database is not compiled."
+        message = {
+            "version": self.version,
+            "pattern_counts": self.db.count_patterns() if self.db is not None else 0
+        }
+        return str(message)
 
     def compile(self, expressions, ids, overwrite=False):
         if len(expressions) != len(ids):
             raise ValueError("All parameters should have the same length")
 
         re2_patterns = {}
         raw_patterns = {}
```

### Comparing `re2shield-0.1.5/re2shield.egg-info/PKG-INFO` & `re2shield-0.1.6/re2shield.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re2shield
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.
 Home-page: https://github.com/Npc-coder/re2shield
 Author: mkCha
 Author-email: dxsaq0@gmail.com
 License: UNKNOWN
 Description: # re2shield
         `re2shield` is a Python library that provides a shield for working with regular expressions using the `re2` module. 
@@ -36,46 +36,45 @@
         ```shell
         git clone https://github.com/Npc-coder/re2shield.git
         cd re2shield
         pip install .
         ```
         
         ## Updates
-        ### Version 0.1.5
-        - Reverted the change that automatically assigned IDs to patterns. Now the compile method requires both a list of regular expressions and a list of corresponding IDs, allowing users to specify the ID for each pattern.
-        - Improved the compile method to check for ID duplication among both new and existing patterns in the database. If a duplicate ID is found and overwrite is False, a ValueError is raised.
+        ### Version 0.1.6
+        - The __str__ method has been updated. Now, it returns a string that includes the version of the Re2Shield object and the number of patterns in the database. If the database has not been compiled, the number of patterns is displayed as 0. With this change, it is guaranteed that a string is always returned when printing the Re2Shield object as a string.
         
         Please refer to the [Usage](#usage) section for examples of how to use these new features.
         
         ## Usage
         ### Importing the Library
         Here is a simple example demonstrating how to use re2shield:
         
         ```python
         import re2shield
         
         if __name__ == "__main__":
             db = re2shield.Database()
-        
+            print(db)
             # Load patterns from file
             try:
-                db = re2shield.load('patterns.pkl')
+                db = re2shield.load('patterns.db')
                 print(db)  # Prints the number of patterns in the database
             except FileNotFoundError:
                 # If pattern file doesn't exist, compile the patterns
                 patterns = [
                     (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
                     (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
                     (r'\d+', 3)
                 ]
         
                 expressions, ids = zip(*patterns)
                 db.compile(expressions=expressions, ids=ids, overwrite=False)
-                print(db)  # Prints the number of patterns in the database
-                db.dump('patterns.pkl')
+                print(db)  # Prints the number of patterns in the database and version
+                db.dump('patterns.db')
         
             # Find patterns in text
             def match_handler(id, from_, to, flags, context):
                 print(f"Match found for pattern {id} from {from_} to {to}: {context}")
         
             db.scan('test@ex12ample12.com', match_handler)
         ```
```

### Comparing `re2shield-0.1.5/setup.py` & `re2shield-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='re2shield',
-    version='0.1.5',
+    version='0.1.6',
     url='https://github.com/Npc-coder/re2shield',  # Replace with your own GitHub project URL
     author='mkCha',
     author_email='dxsaq0@gmail.com',
     description='A Python library that provides a convenient interface for compiling and matching regular expression patterns using the re2 library.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `re2shield-0.1.5/tests/test_core.py` & `re2shield-0.1.6/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import re2shield
 
 if __name__ == "__main__":
     db = re2shield.Database()
-
+    print(db)
     # Load patterns from file
     try:
         db = re2shield.load('patterns.db')
         print(db)  # Prints the number of patterns in the database
     except FileNotFoundError:
         # If pattern file doesn't exist, compile the patterns
         patterns = [
             (r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', 1),
             (r'\b\d{3}[-.\s]??\d{3}[-.\s]??\d{4}\b', 2),
             (r'\d+', 3)
         ]
 
         expressions, ids = zip(*patterns)
         db.compile(expressions=expressions, ids=ids, overwrite=False)
-        print(db)  # Prints the number of patterns in the database
+        print(db)  # Prints the number of patterns in the database and version
         db.dump('patterns.db')
 
     # Find patterns in text
     def match_handler(id, from_, to, flags, context):
         print(f"Match found for pattern {id} from {from_} to {to}: {context}")
 
     db.scan('test@ex12ample12.com', match_handler)
```

