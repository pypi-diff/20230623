# Comparing `tmp/byu_pytest_utils-0.7.1.tar.gz` & `tmp/byu_pytest_utils-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byu_pytest_utils-0.7.1.tar", max compression
+gzip compressed data, was "byu_pytest_utils-0.7.2.tar", max compression
```

## Comparing `byu_pytest_utils-0.7.1.tar` & `byu_pytest_utils-0.7.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1195 2023-06-16 19:58:44.944894 byu_pytest_utils-0.7.1/byu_pytest_utils/__init__.py
--rw-r--r--   0        0        0      611 2023-06-16 19:58:44.958391 byu_pytest_utils-0.7.1/byu_pytest_utils/cpp_utils.py
--rw-r--r--   0        0        0     1168 2023-06-16 19:58:44.971739 byu_pytest_utils-0.7.1/byu_pytest_utils/decorators.py
--rw-r--r--   0        0        0    17927 2023-06-22 20:04:44.736000 byu_pytest_utils-0.7.1/byu_pytest_utils/dialog.py
--rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.7.1/byu_pytest_utils/edit_dist.py
--rw-r--r--   0        0        0     3636 2023-06-22 20:04:44.765627 byu_pytest_utils-0.7.1/byu_pytest_utils/pytest_plugin.py
--rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.7.1/byu_pytest_utils/utils.py
--rw-r--r--   0        0        0      562 2023-06-22 20:04:44.774571 byu_pytest_utils-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1195 2023-06-16 19:58:44.944894 byu_pytest_utils-0.7.2/byu_pytest_utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-16 19:58:44.958391 byu_pytest_utils-0.7.2/byu_pytest_utils/cpp_utils.py
+-rw-r--r--   0        0        0     1168 2023-06-16 19:58:44.971739 byu_pytest_utils-0.7.2/byu_pytest_utils/decorators.py
+-rw-r--r--   0        0        0    17927 2023-06-22 20:04:44.736000 byu_pytest_utils-0.7.2/byu_pytest_utils/dialog.py
+-rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.7.2/byu_pytest_utils/edit_dist.py
+-rw-r--r--   0        0        0     3708 2023-06-23 18:33:47.968688 byu_pytest_utils-0.7.2/byu_pytest_utils/pytest_plugin.py
+-rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.7.2/byu_pytest_utils/utils.py
+-rw-r--r--   0        0        0      562 2023-06-23 18:33:47.974614 byu_pytest_utils-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.7.2/PKG-INFO
```

### Comparing `byu_pytest_utils-0.7.1/byu_pytest_utils/__init__.py` & `byu_pytest_utils-0.7.2/byu_pytest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.1/byu_pytest_utils/cpp_utils.py` & `byu_pytest_utils-0.7.2/byu_pytest_utils/cpp_utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.1/byu_pytest_utils/decorators.py` & `byu_pytest_utils-0.7.2/byu_pytest_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.1/byu_pytest_utils/dialog.py` & `byu_pytest_utils-0.7.2/byu_pytest_utils/dialog.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.1/byu_pytest_utils/edit_dist.py` & `byu_pytest_utils-0.7.2/byu_pytest_utils/edit_dist.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.1/byu_pytest_utils/pytest_plugin.py` & `byu_pytest_utils-0.7.2/byu_pytest_utils/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
             stats['max_score'] *= getattr(metafunc.function, 'max_score', 0)
             stats['score'] *= getattr(metafunc.function, 'max_score', 0)
             test_name = f'{metafunc.function.__module__}.py::{metafunc.function.__name__}[{group_name}]'
             test_group_stats[test_name] = stats
 
         metafunc.parametrize('group_name', group_stats.keys())
     else:
-        test_group_stats[metafunc.definition.name] = {
+        test_name = f'{metafunc.function.__module__}.py::{metafunc.function.__name__}'
+        test_group_stats[test_name] = {
             'max_score': getattr(metafunc.function, 'max_score', 0)
         }
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item):
     x = yield
```

### Comparing `byu_pytest_utils-0.7.1/byu_pytest_utils/utils.py` & `byu_pytest_utils-0.7.2/byu_pytest_utils/utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.1/pyproject.toml` & `byu_pytest_utils-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byu_pytest_utils"
-version = "0.7.1"
+version = "0.7.2"
 description = "A few utilities for pytest to help with integration into gradescope"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Daniel Zappala <daniel.zappala@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `byu_pytest_utils-0.7.1/PKG-INFO` & `byu_pytest_utils-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byu-pytest-utils
-Version: 0.7.1
+Version: 0.7.2
 Summary: A few utilities for pytest to help with integration into gradescope
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
```

