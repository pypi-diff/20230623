# Comparing `tmp/openai_functions-0.2.2.tar.gz` & `tmp/openai_functions-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.2.2.tar", max compression
+gzip compressed data, was "openai_functions-0.2.3.tar", max compression
```

## Comparing `openai_functions-0.2.2.tar` & `openai_functions-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2627 2023-06-23 15:00:32.331037 openai_functions-0.2.2/README.md
--rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.2/openai_functions/__init__.py
--rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.2/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.2/openai_functions/json_type.py
--rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.2/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.2/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1664 2023-06-23 13:53:35.752492 openai_functions-0.2.2/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      973 2023-06-23 13:58:56.625985 openai_functions-0.2.2/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.2/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1637 2023-06-23 15:22:05.255725 openai_functions-0.2.2/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.2/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1190 2023-06-23 14:24:46.974601 openai_functions-0.2.2/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1042 2023-06-23 15:34:43.820700 openai_functions-0.2.2/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.2/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.2/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      989 2023-06-23 14:24:10.570207 openai_functions-0.2.2/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      687 2023-06-23 14:09:22.031628 openai_functions-0.2.2/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.2/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1269 2023-06-23 14:36:38.867041 openai_functions-0.2.2/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0     4539 2023-06-22 15:03:36.171643 openai_functions-0.2.2/openai_functions/runner.py
--rw-r--r--   0        0        0      557 2023-06-23 15:38:54.356483 openai_functions-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 openai_functions-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2627 2023-06-23 15:00:32.331037 openai_functions-0.2.3/README.md
+-rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.3/openai_functions/__init__.py
+-rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.3/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.3/openai_functions/json_type.py
+-rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.3/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.3/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1664 2023-06-23 13:53:35.752492 openai_functions-0.2.3/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      973 2023-06-23 13:58:56.625985 openai_functions-0.2.3/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.3/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1637 2023-06-23 15:22:05.255725 openai_functions-0.2.3/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.3/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1190 2023-06-23 14:24:46.974601 openai_functions-0.2.3/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1063 2023-06-23 16:06:00.970426 openai_functions-0.2.3/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.3/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.3/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      989 2023-06-23 14:24:10.570207 openai_functions-0.2.3/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      687 2023-06-23 14:09:22.031628 openai_functions-0.2.3/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.3/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1269 2023-06-23 14:36:38.867041 openai_functions-0.2.3/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0     4539 2023-06-22 15:03:36.171643 openai_functions-0.2.3/openai_functions/runner.py
+-rw-r--r--   0        0        0      557 2023-06-23 16:06:47.934280 openai_functions-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 openai_functions-0.2.3/PKG-INFO
```

### Comparing `openai_functions-0.2.2/README.md` & `openai_functions-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/function_wrapper.py` & `openai_functions-0.2.3/openai_functions/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/openai_types.py` & `openai_functions-0.2.3/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/abc.py` & `openai_functions-0.2.3/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/default.py` & `openai_functions-0.2.3/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/dict_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/enum_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/enum_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def can_parse(cls, argtype: Any) -> TypeGuard[Type[T]]:
         if not isinstance(argtype, type):
             return False
         return issubclass(argtype, enum.Enum)
 
     @property
     def argument_schema(self) -> dict[str, JsonType]:
-        schema = {
+        schema: dict[str, JsonType] = {
             "type": "string",
             "enum": [e.name for e in self.argtype],
         }
         if self.argtype.__doc__ is not None:
             schema["description"] = self.argtype.__doc__
         return schema
```

### Comparing `openai_functions-0.2.2/openai_functions/parsers/int_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/list_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/none_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/parsers/union_parser.py` & `openai_functions-0.2.3/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/openai_functions/runner.py` & `openai_functions-0.2.3/openai_functions/runner.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.2/pyproject.toml` & `openai_functions-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.2.2/PKG-INFO` & `openai_functions-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

