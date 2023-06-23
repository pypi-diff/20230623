# Comparing `tmp/openai_functions-0.2.5.tar.gz` & `tmp/openai_functions-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.2.5.tar", max compression
+gzip compressed data, was "openai_functions-0.3.0.tar", max compression
```

## Comparing `openai_functions-0.2.5.tar` & `openai_functions-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2627 2023-06-23 15:00:32.331037 openai_functions-0.2.5/README.md
--rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.5/openai_functions/__init__.py
--rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.5/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.5/openai_functions/json_type.py
--rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.5/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.5/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.2.5/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.2.5/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.5/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.2.5/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.5/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.2.5/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.2.5/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.5/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.5/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.2.5/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.2.5/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.5/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.2.5/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.2.5/openai_functions/py.typed
--rw-r--r--   0        0        0     4539 2023-06-23 17:39:29.717354 openai_functions-0.2.5/openai_functions/runner.py
--rw-r--r--   0        0        0      557 2023-06-23 18:45:46.829908 openai_functions-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 openai_functions-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2629 2023-06-23 20:50:25.777069 openai_functions-0.3.0/README.md
+-rw-r--r--   0        0        0      308 2023-06-23 20:51:06.616455 openai_functions-0.3.0/openai_functions/__init__.py
+-rw-r--r--   0        0        0     5596 2023-06-23 19:06:11.339113 openai_functions-0.3.0/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.3.0/openai_functions/json_type.py
+-rw-r--r--   0        0        0     3372 2023-06-23 20:40:56.693784 openai_functions-0.3.0/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.3.0/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.3.0/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.3.0/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.3.0/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.3.0/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.3.0/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.3.0/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.3.0/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.3.0/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.3.0/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.3.0/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.3.0/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.3.0/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.3.0/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.3.0/openai_functions/py.typed
+-rw-r--r--   0        0        0    11932 2023-06-23 20:45:27.576270 openai_functions-0.3.0/openai_functions/runner.py
+-rw-r--r--   0        0        0      557 2023-06-23 20:48:30.033977 openai_functions-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 openai_functions-0.3.0/PKG-INFO
```

### Comparing `openai_functions-0.2.5/README.md` & `openai_functions-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 3. Define your functions using the `@runner.add_function` decorator:
 
 ```python
 class Unit(enum.Enum):
     FAHRENHEIT = "fahrenheit"
     CELSIUS = "celsius"
 
-@runner.add_function
+@runner.add_function()
 def get_current_weather(location: str, unit: Unit = Unit.FAHRENHEIT) -> dict:
     """
     Get the current weather in a given location.
 
     Args:
         location (str): The city and state, e.g., San Francisco, CA
         unit (Unit): The unit to use, e.g. fahrenheit or celsius
```

### Comparing `openai_functions-0.2.5/openai_functions/function_wrapper.py` & `openai_functions-0.3.0/openai_functions/function_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,36 @@
 class FunctionWrapper:
     """Wraps a function for jsonschema io"""
 
     def __init__(
         self,
         func: Callable[..., JsonType],
         parsers: list[Type[ArgSchemaParser]] | None = None,
+        save_return: bool = True,
+        serialize: bool = True,
+        interpret_as_response: bool = False,
     ) -> None:
+        """Initialize a FunctionWrapper
+
+        Args:
+            func (Callable[..., JsonType]): The function to wrap
+            parsers (list[Type[ArgSchemaParser]], optional): The parsers to use.
+            save_return (bool): Whether to send the return value of this
+                function to the AI. Defaults to True.
+            serialize (bool): Whether to serialize the return value of this
+                function. Defaults to True. Otherwise, the return value must be a
+                string.
+            interpret_as_response (bool): Whether to interpret the return
+                value of this function as a response of the agent. Defaults to False.
+        """
         self.func = func
         self.parsers = parsers or defargparsers
+        self.save_return = save_return
+        self.serialize = serialize
+        self.interpret_as_response = interpret_as_response
 
     @property
     def argument_parsers(self) -> OrderedDict[str, ArgSchemaParser]:
         """Get the argument parsers for this function
 
         Returns:
             OrderedDict[str, ArgSchemaParser]: The argument parsers
```

### Comparing `openai_functions-0.2.5/openai_functions/parsers/abc.py` & `openai_functions-0.3.0/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/default.py` & `openai_functions-0.3.0/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/dict_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/enum_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/int_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/list_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/none_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/openai_functions/parsers/union_parser.py` & `openai_functions-0.3.0/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.5/pyproject.toml` & `openai_functions-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.2.5"
+version = "0.3.0"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.2.5/PKG-INFO` & `openai_functions-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.2.5
+Version: 0.3.0
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -48,15 +48,15 @@
 3. Define your functions using the `@runner.add_function` decorator:
 
 ```python
 class Unit(enum.Enum):
     FAHRENHEIT = "fahrenheit"
     CELSIUS = "celsius"
 
-@runner.add_function
+@runner.add_function()
 def get_current_weather(location: str, unit: Unit = Unit.FAHRENHEIT) -> dict:
     """
     Get the current weather in a given location.
 
     Args:
         location (str): The city and state, e.g., San Francisco, CA
         unit (Unit): The unit to use, e.g. fahrenheit or celsius
```

