# Comparing `tmp/openai_functions-0.2.3.tar.gz` & `tmp/openai_functions-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.2.3.tar", max compression
+gzip compressed data, was "openai_functions-0.2.4.tar", max compression
```

## Comparing `openai_functions-0.2.3.tar` & `openai_functions-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2627 2023-06-23 15:00:32.331037 openai_functions-0.2.3/README.md
--rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.3/openai_functions/__init__.py
--rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.3/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.3/openai_functions/json_type.py
--rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.3/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.3/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1664 2023-06-23 13:53:35.752492 openai_functions-0.2.3/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      973 2023-06-23 13:58:56.625985 openai_functions-0.2.3/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.3/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1637 2023-06-23 15:22:05.255725 openai_functions-0.2.3/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.3/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1190 2023-06-23 14:24:46.974601 openai_functions-0.2.3/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1063 2023-06-23 16:06:00.970426 openai_functions-0.2.3/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.3/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.3/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      989 2023-06-23 14:24:10.570207 openai_functions-0.2.3/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      687 2023-06-23 14:09:22.031628 openai_functions-0.2.3/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.3/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1269 2023-06-23 14:36:38.867041 openai_functions-0.2.3/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0     4539 2023-06-22 15:03:36.171643 openai_functions-0.2.3/openai_functions/runner.py
--rw-r--r--   0        0        0      557 2023-06-23 16:06:47.934280 openai_functions-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 openai_functions-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2627 2023-06-23 15:00:32.331037 openai_functions-0.2.4/README.md
+-rw-r--r--   0        0        0      263 2023-06-22 14:38:41.406626 openai_functions-0.2.4/openai_functions/__init__.py
+-rw-r--r--   0        0        0     4670 2023-06-23 14:29:15.130502 openai_functions-0.2.4/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.2.4/openai_functions/json_type.py
+-rw-r--r--   0        0        0      681 2023-06-23 09:03:28.062037 openai_functions-0.2.4/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.2.4/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.2.4/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.2.4/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.2.4/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.2.4/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.2.4/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.2.4/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.2.4/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.2.4/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.2.4/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.2.4/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.2.4/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.2.4/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.2.4/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0     4539 2023-06-23 17:39:29.717354 openai_functions-0.2.4/openai_functions/runner.py
+-rw-r--r--   0        0        0      557 2023-06-23 18:33:08.615612 openai_functions-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 openai_functions-0.2.4/PKG-INFO
```

### Comparing `openai_functions-0.2.3/README.md` & `openai_functions-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.3/openai_functions/function_wrapper.py` & `openai_functions-0.2.4/openai_functions/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.3/openai_functions/openai_types.py` & `openai_functions-0.2.4/openai_functions/openai_types.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.3/openai_functions/parsers/abc.py` & `openai_functions-0.2.4/openai_functions/parsers/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Abstract base class for argument schema parsers"""
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import Any, Generic, TYPE_CHECKING, Type, TypeVar
-from typing_extensions import TypeGuard
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 T = TypeVar("T")
 S = TypeVar("S")
 
 
 class ArgSchemaParser(ABC, Generic[T]):
     """A parser for a specific argument type"""
```

### Comparing `openai_functions-0.2.3/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/atomic_type_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Parser for atomic json types"""
 from __future__ import annotations
 from abc import abstractmethod
 from typing import Any, TYPE_CHECKING, Type, TypeVar
-from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 T = TypeVar("T")
 
 
 class AtomicParser(ArgSchemaParser[T]):
     """Parser for atomic json values"""
```

### Comparing `openai_functions-0.2.3/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/dataclass_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Parser for dataclass types"""
 from __future__ import annotations
 import dataclasses
 from typing import Any, ClassVar, Protocol, TYPE_CHECKING, Type
-from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 
 class IsDataclass(Protocol):  # pylint: disable=too-few-public-methods
     """A protocol for checking if a class is a dataclass"""
 
     __dataclass_fields__: ClassVar[dict]
```

### Comparing `openai_functions-0.2.3/openai_functions/parsers/default.py` & `openai_functions-0.2.4/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.3/openai_functions/parsers/dict_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/dict_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Parser for dict types"""
 from __future__ import annotations
 from typing import Any, Dict, TYPE_CHECKING, Type, TypeVar, get_args, get_origin
-from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 T = TypeVar("T")
 
 
 class DictParser(ArgSchemaParser[Dict[str, T]]):
     """Parser for dict types"""
```

### Comparing `openai_functions-0.2.3/openai_functions/parsers/enum_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/enum_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Parser for enum types"""
 from __future__ import annotations
 import enum
 from typing import Any, TYPE_CHECKING, Type, TypeVar
-from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 T = TypeVar("T", bound=enum.Enum)
 
 
 class EnumParser(ArgSchemaParser[T]):
     """Parser for enum types"""
```

### Comparing `openai_functions-0.2.3/openai_functions/parsers/int_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.3/openai_functions/parsers/list_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/list_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Parser for list types"""
 from __future__ import annotations
 from typing import Any, List, TYPE_CHECKING, Type, TypeVar, get_args, get_origin
-from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 T = TypeVar("T")
 
 
 class ListParser(ArgSchemaParser[List[T]]):
     """Parser for list types"""
```

### Comparing `openai_functions-0.2.3/openai_functions/parsers/none_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/none_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Parser for null types"""
 from __future__ import annotations
 from typing import Any, TYPE_CHECKING, Type
-from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 
 class NoneParser(ArgSchemaParser[None]):
     """Parser for null types"""
 
     @classmethod
     def can_parse(cls, argtype: Any) -> TypeGuard[Type[None]]:
```

### Comparing `openai_functions-0.2.3/openai_functions/parsers/union_parser.py` & `openai_functions-0.2.4/openai_functions/parsers/union_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Parser for union types"""
 from __future__ import annotations
 import contextlib
-from typing_extensions import TypeGuard
 
 from .abc import ArgSchemaParser
 
 try:
     from types import UnionType
     from typing import Any, TYPE_CHECKING, Type, Union, get_args, get_origin
 except ImportError:
@@ -18,14 +17,15 @@
         get_args,
         get_origin,
         _GenericAlias as UnionType,
     )
 
 if TYPE_CHECKING:
     from ..json_type import JsonType
+    from typing_extensions import TypeGuard
 
 
 class UnionParser(ArgSchemaParser[UnionType]):
     """Parser for union types"""
 
     @classmethod
     def can_parse(cls, argtype: Any) -> TypeGuard[Type[UnionType]]:
```

### Comparing `openai_functions-0.2.3/openai_functions/runner.py` & `openai_functions-0.2.4/openai_functions/runner.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.2.3/pyproject.toml` & `openai_functions-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.2.3/PKG-INFO` & `openai_functions-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

