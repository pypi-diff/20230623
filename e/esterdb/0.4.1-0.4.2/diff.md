# Comparing `tmp/esterdb-0.4.1.tar.gz` & `tmp/esterdb-0.4.2.tar.gz`

## Comparing `esterdb-0.4.1.tar` & `esterdb-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esterdb-0.4.1/Makefile
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 esterdb-0.4.1/esterdb/__about__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 esterdb-0.4.1/esterdb/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 esterdb-0.4.1/esterdb/_env.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 esterdb-0.4.1/esterdb/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esterdb-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 esterdb-0.4.1/tests/test_load.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 esterdb-0.4.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 esterdb-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 esterdb-0.4.1/README.md
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 esterdb-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esterdb-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esterdb-0.4.2/Makefile
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 esterdb-0.4.2/esterdb/__about__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 esterdb-0.4.2/esterdb/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 esterdb-0.4.2/esterdb/_env.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 esterdb-0.4.2/esterdb/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esterdb-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 esterdb-0.4.2/tests/test_load.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 esterdb-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 esterdb-0.4.2/LICENSE.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 esterdb-0.4.2/README.md
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 esterdb-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esterdb-0.4.2/PKG-INFO
```

### Comparing `esterdb-0.4.1/esterdb/main.py` & `esterdb-0.4.2/esterdb/main.py`

 * *Files identical despite different names*

### Comparing `esterdb-0.4.1/tests/test_load.py` & `esterdb-0.4.2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `esterdb-0.4.1/LICENSE.txt` & `esterdb-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `esterdb-0.4.1/pyproject.toml` & `esterdb-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esterdb-0.4.1/PKG-INFO` & `esterdb-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esterdb
-Version: 0.4.1
+Version: 0.4.2
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

