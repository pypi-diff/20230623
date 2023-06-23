# Comparing `tmp/prettyc-1.0.7.tar.gz` & `tmp/prettyc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyc-1.0.7.tar", last modified: Wed Jun 21 20:05:43 2023, max compression
+gzip compressed data, was "prettyc-1.0.8.tar", last modified: Fri Jun 23 12:27:59 2023, max compression
```

## Comparing `prettyc-1.0.7.tar` & `prettyc-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 20:05:43.121312 prettyc-1.0.7/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.7/LICENSE
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 20:05:43.121312 prettyc-1.0.7/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.7/README.md
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-21 20:05:43.121312 prettyc-1.0.7/prettyc.egg-info/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/SOURCES.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/dependency_links.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/entry_points.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-21 20:05:43.000000 prettyc-1.0.7/prettyc.egg-info/top_level.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)   257046 2023-06-21 20:04:47.000000 prettyc-1.0.7/prettyc.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-21 20:05:43.121312 prettyc-1.0.7/setup.cfg
--rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.7/setup.py
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-23 12:27:59.329192 prettyc-1.0.8/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.8/LICENSE
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-23 12:27:59.329192 prettyc-1.0.8/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.8/README.md
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-23 12:27:59.329192 prettyc-1.0.8/prettyc.egg-info/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-23 12:27:59.000000 prettyc-1.0.8/prettyc.egg-info/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-23 12:27:59.000000 prettyc-1.0.8/prettyc.egg-info/SOURCES.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-23 12:27:59.000000 prettyc-1.0.8/prettyc.egg-info/dependency_links.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-23 12:27:59.000000 prettyc-1.0.8/prettyc.egg-info/entry_points.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-23 12:27:59.000000 prettyc-1.0.8/prettyc.egg-info/top_level.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)   256777 2023-06-23 12:25:16.000000 prettyc-1.0.8/prettyc.py
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-23 12:27:59.329192 prettyc-1.0.8/setup.cfg
+-rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.8/setup.py
```

### Comparing `prettyc-1.0.7/LICENSE` & `prettyc-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.7/PKG-INFO` & `prettyc-1.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.7/README.md` & `prettyc-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.7/prettyc.egg-info/PKG-INFO` & `prettyc-1.0.8/prettyc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.7/prettyc.py` & `prettyc-1.0.8/prettyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import sysconfig
 import unicodedata
 import xml.etree.ElementTree
 
 # if empty, use defaults
 _valid_extensions = set([])
 
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 __verbose__ = False
 
 try:
   #  -- pylint: disable=used-before-assignment
   xrange          # Python 2
 except NameError:
   #  -- pylint: disable=redefined-builtin
@@ -317,15 +317,14 @@
     'readability/inheritance',
     'readability/multiline_comment',
     'readability/multiline_string',
     'readability/namespace',
     'readability/nolint',
     'readability/nul',
     'readability/strings',
-    'readability/todo',
     'readability/utf8',
     'runtime/casting',
     'runtime/explicit',
     'runtime/init',
     'runtime/invalid_increment',
     'runtime/member_string_references',
     'runtime/memset',
@@ -3657,25 +3656,19 @@
       if match:
         # One whitespace is correct; zero whitespace is handled elsewhere.
         leading_whitespace = match.group(1)
         if len(leading_whitespace) > 1:
           error(filename, linenum, 'whitespace/todo', 2,
                 'Too many spaces before TODO')
 
-        username = match.group(2)
-        if not username:
-          error(filename, linenum, 'readability/todo', 2,
-                'Missing username in TODO; it should look like '
-                '"// TODO(my_username): Stuff."')
-
         middle_whitespace = match.group(3)
         # Comparisons made explicit for correctness -- pylint: disable=g-explicit-bool-comparison
         if middle_whitespace != ' ' and middle_whitespace != '':
           error(filename, linenum, 'whitespace/todo', 2,
-                'TODO(my_username) should be followed by a space')
+                'TODO: should be followed by a space')
 
       # If the comment contains an alphanumeric character, there
       # should be a space somewhere between it and the // unless
       # it's a /// or //! Doxygen comment.
       if (Match(r'//[^ ]*\w', comment) and
           not Match(r'(///|//\!)(\s+|$)', comment)):
         error(filename, linenum, 'whitespace/comments', 4,
```

### Comparing `prettyc-1.0.7/setup.py` & `prettyc-1.0.8/setup.py`

 * *Files identical despite different names*

