# Comparing `tmp/openai_functions-0.2.4.tar.gz` & `tmp/openai_functions-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.2.4.tar", max compression
+gzip compressed data, was "openai_functions-0.2.5.tar", max compression
```

## Comparing `openai_functions-0.2.4.tar` & `openai_functions-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     2627 2023-06-23 15:00:32.331037 openai_functions-0.2.4/README.md
--rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.4/openai_functions/__init__.py
--rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.4/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.4/openai_functions/json_type.py
--rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.4/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.4/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.2.4/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.2.4/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.4/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.2.4/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.4/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.2.4/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.2.4/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.4/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.4/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.2.4/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.2.4/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.4/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.2.4/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0     4539 2023-06-23 17:39:29.717354 openai_functions-0.2.4/openai_functions/runner.py
--rw-r--r--   0        0        0      557 2023-06-23 18:33:08.615612 openai_functions-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 openai_functions-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2627 2023-06-23 15:00:32.331037 openai_functions-0.2.5/README.md
+-rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.5/openai_functions/__init__.py
+-rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.5/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.5/openai_functions/json_type.py
+-rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.5/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.5/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.2.5/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.2.5/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.5/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.2.5/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.5/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.2.5/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.2.5/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.5/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.5/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.2.5/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.2.5/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.5/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.2.5/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.2.5/openai_functions/py.typed
+-rw-r--r--   0        0        0     4539 2023-06-23 17:39:29.717354 openai_functions-0.2.5/openai_functions/runner.py
+-rw-r--r--   0        0        0      557 2023-06-23 18:45:46.829908 openai_functions-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 openai_functions-0.2.5/PKG-INFO
```

### Comparing `openai_functions-0.2.4/README.md` & `openai_functions-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/function_wrapper.py` & `openai_functions-0.2.5/openai_functions/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/openai_types.py` & `openai_functions-0.2.5/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/abc.py` & `openai_functions-0.2.5/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/default.py` & `openai_functions-0.2.5/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/dict_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/enum_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/int_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/list_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/none_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/parsers/union_parser.py` & `openai_functions-0.2.5/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/openai_functions/runner.py` & `openai_functions-0.2.5/openai_functions/runner.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.4/pyproject.toml` & `openai_functions-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.2.4/PKG-INFO` & `openai_functions-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

