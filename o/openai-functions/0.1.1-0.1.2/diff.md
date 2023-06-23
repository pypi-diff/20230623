# Comparing `tmp/openai_functions-0.1.1.tar.gz` & `tmp/openai_functions-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.1.1.tar", max compression
+gzip compressed data, was "openai_functions-0.1.2.tar", max compression
```

## Comparing `openai_functions-0.1.1.tar` & `openai_functions-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       89 2023-06-23 07:07:39.689646 openai_functions-0.1.1/README.md
--rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.1.1/openai_functions/__init__.py
--rw-r--r--   0        0        0     4505 2023-06-22 14:37:47.266184 openai_functions-0.1.1/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      124 2023-06-22 12:07:42.214576 openai_functions-0.1.1/openai_functions/json_type.py
--rw-r--r--   0        0        0      646 2023-06-22 12:41:03.271719 openai_functions-0.1.1/openai_functions/openai_types.py
--rw-r--r--   0        0        0      192 2023-06-22 14:44:17.179198 openai_functions-0.1.1/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1635 2023-06-22 13:07:10.956782 openai_functions-0.1.1/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      906 2023-06-23 07:36:54.214140 openai_functions-0.1.1/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.1.1/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1527 2023-06-22 13:18:12.684665 openai_functions-0.1.1/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      708 2023-06-22 14:43:53.687930 openai_functions-0.1.1/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1131 2023-06-22 13:17:07.386935 openai_functions-0.1.1/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0      860 2023-06-22 13:19:09.965310 openai_functions-0.1.1/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.1.1/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      196 2023-06-23 07:38:49.312196 openai_functions-0.1.1/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      943 2023-06-22 13:16:15.158356 openai_functions-0.1.1/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      235 2023-06-23 07:39:20.931489 openai_functions-0.1.1/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.1.1/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0      953 2023-06-23 07:39:48.395745 openai_functions-0.1.1/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0     4539 2023-06-22 15:03:36.171643 openai_functions-0.1.1/openai_functions/runner.py
--rw-r--r--   0        0        0      385 2023-06-23 07:45:10.725811 openai_functions-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 openai_functions-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2362 2023-06-23 08:53:43.458199 openai_functions-0.1.2/README.md
+-rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.1.2/openai_functions/__init__.py
+-rw-r--r--   0        0        0     4505 2023-06-22 14:37:47.266184 openai_functions-0.1.2/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      124 2023-06-22 12:07:42.214576 openai_functions-0.1.2/openai_functions/json_type.py
+-rw-r--r--   0        0        0      646 2023-06-22 12:41:03.271719 openai_functions-0.1.2/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      192 2023-06-22 14:44:17.179198 openai_functions-0.1.2/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1635 2023-06-22 13:07:10.956782 openai_functions-0.1.2/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      906 2023-06-23 07:36:54.214140 openai_functions-0.1.2/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.1.2/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1527 2023-06-22 13:18:12.684665 openai_functions-0.1.2/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      708 2023-06-22 14:43:53.687930 openai_functions-0.1.2/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1131 2023-06-22 13:17:07.386935 openai_functions-0.1.2/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0      860 2023-06-22 13:19:09.965310 openai_functions-0.1.2/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.1.2/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      196 2023-06-23 07:38:49.312196 openai_functions-0.1.2/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      943 2023-06-22 13:16:15.158356 openai_functions-0.1.2/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      235 2023-06-23 07:39:20.931489 openai_functions-0.1.2/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.1.2/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0      953 2023-06-23 07:39:48.395745 openai_functions-0.1.2/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0     4539 2023-06-22 15:03:36.171643 openai_functions-0.1.2/openai_functions/runner.py
+-rw-r--r--   0        0        0      385 2023-06-23 08:56:07.528638 openai_functions-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 openai_functions-0.1.2/PKG-INFO
```

### Comparing `openai_functions-0.1.1/openai_functions/function_wrapper.py` & `openai_functions-0.1.2/openai_functions/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/openai_types.py` & `openai_functions-0.1.2/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/abc.py` & `openai_functions-0.1.2/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.1.2/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.1.2/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/default.py` & `openai_functions-0.1.2/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/dict_parser.py` & `openai_functions-0.1.2/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/enum_parser.py` & `openai_functions-0.1.2/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/list_parser.py` & `openai_functions-0.1.2/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/parsers/union_parser.py` & `openai_functions-0.1.2/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.1/openai_functions/runner.py` & `openai_functions-0.1.2/openai_functions/runner.py`

 * *Files identical despite different names*

