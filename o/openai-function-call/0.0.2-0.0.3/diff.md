# Comparing `tmp/openai_function_call-0.0.2.tar.gz` & `tmp/openai_function_call-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_call-0.0.2.tar", max compression
+gzip compressed data, was "openai_function_call-0.0.3.tar", max compression
```

## Comparing `openai_function_call-0.0.2.tar` & `openai_function_call-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-06-17 12:35:29.432156 openai_function_call-0.0.2/LICENSE
--rw-r--r--   0        0        0     3242 2023-06-23 03:49:25.348705 openai_function_call-0.0.2/README.md
--rw-r--r--   0        0        0     4155 2023-06-23 03:49:25.348966 openai_function_call-0.0.2/openai_function_call/__init__.py
--rw-r--r--   0        0        0      445 2023-06-23 03:49:25.349158 openai_function_call-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 openai_function_call-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-17 12:35:29.432156 openai_function_call-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3242 2023-06-23 03:49:25.348705 openai_function_call-0.0.3/README.md
+-rw-r--r--   0        0        0     4155 2023-06-23 03:49:25.348966 openai_function_call-0.0.3/openai_function_call/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-23 03:54:17.314715 openai_function_call-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 openai_function_call-0.0.3/PKG-INFO
```

### Comparing `openai_function_call-0.0.2/LICENSE` & `openai_function_call-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.0.2/README.md` & `openai_function_call-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.0.2/openai_function_call/__init__.py` & `openai_function_call-0.0.3/openai_function_call/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.0.2/PKG-INFO` & `openai_function_call-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-call
-Version: 0.0.2
+Version: 0.0.3
 Summary: Helper functions that allow us to improve openai's function_call ergonomics
 License: MIT
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

