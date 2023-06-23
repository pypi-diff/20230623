# Comparing `tmp/openai_functions-0.1.3.tar.gz` & `tmp/openai_functions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.1.3.tar", max compression
+gzip compressed data, was "openai_functions-0.2.0.tar", max compression
```

## Comparing `openai_functions-0.1.3.tar` & `openai_functions-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2362 2023-06-23 08:53:43.458199 openai_functions-0.1.3/README.md
--rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.1.3/openai_functions/__init__.py
--rw-r--r--   0        0        0     4505 2023-06-22 14:37:47.266184 openai_functions-0.1.3/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.1.3/openai_functions/json_type.py
--rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.1.3/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.1.3/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1635 2023-06-22 13:07:10.956782 openai_functions-0.1.3/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      906 2023-06-23 07:36:54.214140 openai_functions-0.1.3/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.1.3/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1527 2023-06-22 13:18:12.684665 openai_functions-0.1.3/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      708 2023-06-22 14:43:53.687930 openai_functions-0.1.3/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1131 2023-06-22 13:17:07.386935 openai_functions-0.1.3/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0      888 2023-06-23 09:05:32.391279 openai_functions-0.1.3/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.1.3/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      196 2023-06-23 07:38:49.312196 openai_functions-0.1.3/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      943 2023-06-22 13:16:15.158356 openai_functions-0.1.3/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      235 2023-06-23 09:07:12.949284 openai_functions-0.1.3/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.1.3/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0      953 2023-06-23 07:39:48.395745 openai_functions-0.1.3/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0     4539 2023-06-22 15:03:36.171643 openai_functions-0.1.3/openai_functions/runner.py
--rw-r--r--   0        0        0      384 2023-06-23 09:07:41.268567 openai_functions-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 openai_functions-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2609 2023-06-23 14:58:23.231555 openai_functions-0.2.0/README.md
+-rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.0/openai_functions/__init__.py
+-rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.0/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.0/openai_functions/json_type.py
+-rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.0/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.0/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1664 2023-06-23 13:53:35.752492 openai_functions-0.2.0/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      973 2023-06-23 13:58:56.625985 openai_functions-0.2.0/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.0/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1598 2023-06-23 13:59:51.048559 openai_functions-0.2.0/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.0/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1190 2023-06-23 14:24:46.974601 openai_functions-0.2.0/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0      917 2023-06-23 14:01:10.322393 openai_functions-0.2.0/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.0/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.0/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      989 2023-06-23 14:24:10.570207 openai_functions-0.2.0/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      687 2023-06-23 14:09:22.031628 openai_functions-0.2.0/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.0/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1269 2023-06-23 14:36:38.867041 openai_functions-0.2.0/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0     4539 2023-06-22 15:03:36.171643 openai_functions-0.2.0/openai_functions/runner.py
+-rw-r--r--   0        0        0      517 2023-06-23 14:58:56.963943 openai_functions-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 openai_functions-0.2.0/PKG-INFO
```

### Comparing `openai_functions-0.1.3/README.md` & `openai_functions-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # OpenAI functions
 
 The `openai-functions` Python project simplifies the usage of OpenAI's function calling feature. It abstracts away the complexity of parsing function signatures and docstrings by providing developers with a clean and intuitive interface.
 
+![Tests](https://github.com/rizerphe/openai-functions/actions/workflows/tests.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/badges/shields/badge.svg?branch=master)](https://coveralls.io/github/badges/shields?branch=master)
+
 ## Installation
 
 You can install `openai-functions` from PyPI using pip:
 
 ```
 pip install openai-functions
 ```
```

### Comparing `openai_functions-0.1.3/openai_functions/function_wrapper.py` & `openai_functions-0.2.0/openai_functions/function_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,22 @@
     def arguments_schema(self) -> JsonType:
         """Get the arguments schema for this function
 
         Returns:
             JsonType: The arguments schema
         """
         return {
-            name: parser.argument_schema | {"description": self.arg_docs.get(name)}
+            name: {
+                **parser.argument_schema,
+                **(
+                    {"description": self.arg_docs.get(name)}
+                    if name in self.arg_docs
+                    else {}
+                ),
+            }
             for name, parser in self.argument_parsers.items()
         }
 
     @property
     def parsed_docs(self) -> Docstring:
         """Get the parsed docs for this function
```

### Comparing `openai_functions-0.1.3/openai_functions/openai_types.py` & `openai_functions-0.2.0/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.3/openai_functions/parsers/abc.py` & `openai_functions-0.2.0/openai_functions/parsers/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Abstract base class for argument schema parsers"""
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from typing import Any, Generic, TYPE_CHECKING, Type, TypeGuard, TypeVar
+from typing import Any, Generic, TYPE_CHECKING, Type, TypeVar
+from typing_extensions import TypeGuard
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 T = TypeVar("T")
 S = TypeVar("S")
```

### Comparing `openai_functions-0.1.3/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.2.0/openai_functions/parsers/atomic_type_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Parser for atomic json types"""
 from __future__ import annotations
 from abc import abstractmethod
-from typing import Any, TYPE_CHECKING, Type, TypeGuard, TypeVar
+from typing import Any, TYPE_CHECKING, Type, TypeVar
+from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 T = TypeVar("T")
@@ -15,15 +16,15 @@
     """Parser for atomic json values"""
 
     _type: Type[T]
 
     @property
     @abstractmethod
     def schema_type_name(self) -> str:
-        ...
+        """Name of the type in the json schema"""
 
     @classmethod
     def can_parse(cls, argtype: Any) -> TypeGuard[Type[T]]:
         return argtype is cls._type
 
     @property
     def argument_schema(self) -> dict[str, JsonType]:
```

### Comparing `openai_functions-0.1.3/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.2.0/openai_functions/parsers/dataclass_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Parser for dataclass types"""
 from __future__ import annotations
 import dataclasses
-from typing import Any, ClassVar, Protocol, TYPE_CHECKING, Type, TypeGuard
+from typing import Any, ClassVar, Protocol, TYPE_CHECKING, Type
+from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
-class IsDataclass(Protocol):
+class IsDataclass(Protocol):  # pylint: disable=too-few-public-methods
     """A protocol for checking if a class is a dataclass"""
 
     __dataclass_fields__: ClassVar[dict]
 
 
 class DataclassParser(ArgSchemaParser[IsDataclass]):
     """Parser for dataclass types"""
```

### Comparing `openai_functions-0.1.3/openai_functions/parsers/default.py` & `openai_functions-0.2.0/openai_functions/parsers/default.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .bool_parser import BoolParser
 from .dataclass_parser import DataclassParser
 from .dict_parser import DictParser
 from .enum_parser import EnumParser
 from .float_parser import FloatParser
 from .int_parser import IntParser
 from .list_parser import ListParser
+from .none_parser import NoneParser
 from .str_parser import StringParser
 from .union_parser import UnionParser
 
 if TYPE_CHECKING:
     from .abc import ArgSchemaParser
 
 
@@ -20,10 +21,11 @@
     BoolParser,
     DataclassParser,
     DictParser,
     EnumParser,
     FloatParser,
     IntParser,
     ListParser,
+    NoneParser,
     StringParser,
     UnionParser,
 ]
```

### Comparing `openai_functions-0.1.3/openai_functions/parsers/dict_parser.py` & `openai_functions-0.2.0/openai_functions/parsers/dict_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 """Parser for dict types"""
 from __future__ import annotations
-import types
-from typing import Any, TYPE_CHECKING, Type, TypeGuard, TypeVar
+from typing import Any, Dict, TYPE_CHECKING, Type, TypeVar, get_args, get_origin
+from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 T = TypeVar("T")
 
 
-class DictParser(ArgSchemaParser[dict[str, T]]):
+class DictParser(ArgSchemaParser[Dict[str, T]]):
     """Parser for dict types"""
 
     @classmethod
-    def can_parse(cls, argtype: Any) -> TypeGuard[Type[dict[str, T]]]:
+    def can_parse(cls, argtype: Any) -> TypeGuard[Type[Dict[str, T]]]:
         return (
-            isinstance(argtype, types.GenericAlias)
-            and argtype.__origin__ is dict
-            and argtype.__args__[0] is str
+            get_origin(argtype)
+            in [
+                dict,
+                Dict,
+            ]
+            and get_args(argtype)[0] is str
         )
 
     @property
-    def argument_schema(self) -> dict[str, JsonType]:
+    def argument_schema(self) -> Dict[str, JsonType]:
         return {
             "type": "object",
             "additionalProperties": self.parse_rec(
-                self.argtype.__args__[1]
+                get_args(self.argtype)[1]
             ).argument_schema,
         }
 
-    def parse_value(self, value: JsonType) -> dict[str, T]:
+    def parse_value(self, value: JsonType) -> Dict[str, T]:
         if not isinstance(value, dict):
             raise TypeError(f"Expected dict, got {value}")
         return {
-            k: self.parse_rec(self.argtype.__args__[1]).parse_value(v)
+            k: self.parse_rec(get_args(self.argtype)[1]).parse_value(v)
             for k, v in value.items()
         }
```

### Comparing `openai_functions-0.1.3/openai_functions/parsers/enum_parser.py` & `openai_functions-0.2.0/openai_functions/parsers/enum_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Parser for enum types"""
 from __future__ import annotations
 import enum
-from typing import Any, TYPE_CHECKING, Type, TypeGuard, TypeVar
+from typing import Any, TYPE_CHECKING, Type, TypeVar
+from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 T = TypeVar("T", bound=enum.Enum)
```

### Comparing `openai_functions-0.1.3/openai_functions/parsers/union_parser.py` & `openai_functions-0.2.0/openai_functions/parsers/none_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-"""Parser for union types"""
+"""Parser for null types"""
 from __future__ import annotations
-import types
-from typing import Any, TYPE_CHECKING, Type, TypeGuard
+from typing import Any, TYPE_CHECKING, Type
+from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
 
 
-class UnionParser(ArgSchemaParser[types.UnionType]):
-    """Parser for union types"""
+class NoneParser(ArgSchemaParser[None]):
+    """Parser for null types"""
 
     @classmethod
-    def can_parse(cls, argtype: Any) -> TypeGuard[Type[types.UnionType]]:
-        return isinstance(argtype, types.UnionType)
+    def can_parse(cls, argtype: Any) -> TypeGuard[Type[None]]:
+        return argtype in [None, type(None)]
 
     @property
     def argument_schema(self) -> dict[str, JsonType]:
-        return {
-            "anyOf": [self.parse_rec(t).argument_schema for t in self.argtype.__args__],
-        }
-
-    def parse_value(self, value: JsonType) -> types.UnionType:
-        for single_type in self.argtype.__args__:
-            with contextlib.suppress(TypeError):
-                return self.parse_rec(single_type).parse_value(value)
-        raise TypeError(f"Expected one of {self.argtype.__args__}, got {value}")
+        return {"type": "null"}
+
+    def parse_value(self, value: JsonType) -> None:
+        if value is not None:
+            raise TypeError(f"Expected None, got {type(value)}")
```

### Comparing `openai_functions-0.1.3/openai_functions/runner.py` & `openai_functions-0.2.0/openai_functions/runner.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.1.3/PKG-INFO` & `openai_functions-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # OpenAI functions
 
 The `openai-functions` Python project simplifies the usage of OpenAI's function calling feature. It abstracts away the complexity of parsing function signatures and docstrings by providing developers with a clean and intuitive interface.
 
+![Tests](https://github.com/rizerphe/openai-functions/actions/workflows/tests.yml/badge.svg) [![Coverage Status](https://coveralls.io/repos/github/badges/shields/badge.svg?branch=master)](https://coveralls.io/github/badges/shields?branch=master)
+
 ## Installation
 
 You can install `openai-functions` from PyPI using pip:
 
 ```
 pip install openai-functions
 ```
```

