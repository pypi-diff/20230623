# Comparing `tmp/types-mysqlclient-2.1.5.7.tar.gz` & `tmp/types-mysqlclient-2.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-mysqlclient-2.1.5.7.tar", last modified: Mon Mar 27 18:24:44 2023, max compression
+gzip compressed data, was "types-mysqlclient-2.2.0.0.tar", last modified: Fri Jun 23 12:33:00 2023, max compression
```

## Comparing `types-mysqlclient-2.1.5.7.tar` & `types-mysqlclient-2.2.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:44.059388 types-mysqlclient-2.1.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-27 18:24:43.000000 types-mysqlclient-2.1.5.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:43.000000 types-mysqlclient-2.1.5.7/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:44.055388 types-mysqlclient-2.1.5.7/MySQLdb-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:24:43.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/_mysql.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/connections.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:44.059388 types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/CLIENT.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/CR.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/ER.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/FIELD_TYPE.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/FLAG.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/cursors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/release.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-27 18:21:24.000000 types-mysqlclient-2.1.5.7/MySQLdb-stubs/times.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:24:44.059388 types-mysqlclient-2.1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:44.059388 types-mysqlclient-2.1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-27 18:24:43.000000 types-mysqlclient-2.1.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:44.059388 types-mysqlclient-2.1.5.7/types_mysqlclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:24:44.000000 types-mysqlclient-2.1.5.7/types_mysqlclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-27 18:24:44.000000 types-mysqlclient-2.1.5.7/types_mysqlclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:44.000000 types-mysqlclient-2.1.5.7/types_mysqlclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-27 18:24:44.000000 types-mysqlclient-2.1.5.7/types_mysqlclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.121359 types-mysqlclient-2.2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/MySQLdb-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/_mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/connections.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/CLIENT.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/CR.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/ER.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/FIELD_TYPE.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/FLAG.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/cursors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/release.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/times.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:33:00.121359 types-mysqlclient-2.2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/top_level.txt
```

### Comparing `types-mysqlclient-2.1.5.7/CHANGELOG.md` & `types-mysqlclient-2.2.0.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.2.0.0 (2023-06-23)
+
+Bump mysqlclient to 2.2 (#10353)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 2.1.5.7 (2023-03-27)
 
 Add defaults for third-party stubs M-O (#9956)
 
 ## 2.1.5.6 (2023-02-26)
 
 Improve many `__(a)exit__` annotations (#9696)
```

### Comparing `types-mysqlclient-2.1.5.7/MySQLdb-stubs/__init__.pyi` & `types-mysqlclient-2.2.0.0/MySQLdb-stubs/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from _typeshed import Incomplete
 
 from MySQLdb import connections as connections, constants as constants, converters as converters, cursors as cursors
 from MySQLdb._mysql import (
     DatabaseError as DatabaseError,
     DataError as DataError,
     Error as Error,
     IntegrityError as IntegrityError,
@@ -29,23 +29,23 @@
     TimestampFromTicks as TimestampFromTicks,
 )
 
 threadsafety: int
 apilevel: str
 paramstyle: str
 
-class DBAPISet(frozenset[Any]):
+class DBAPISet(frozenset[Incomplete]):
     def __eq__(self, other): ...
 
-STRING: Any
-BINARY: Any
-NUMBER: Any
-DATE: Any
-TIME: Any
-TIMESTAMP: Any
-DATETIME: Any
-ROWID: Any
+STRING: Incomplete
+BINARY: Incomplete
+NUMBER: Incomplete
+DATE: Incomplete
+TIME: Incomplete
+TIMESTAMP: Incomplete
+DATETIME: Incomplete
+ROWID: Incomplete
 
 def Binary(x): ...
 def Connect(*args, **kwargs): ...
 
 connect = Connect
```

### Comparing `types-mysqlclient-2.1.5.7/MySQLdb-stubs/connections.pyi` & `types-mysqlclient-2.2.0.0/MySQLdb-stubs/connections.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from _typeshed import Incomplete
+from re import Pattern
 from types import TracebackType
 from typing import Any
-from typing_extensions import Self
+from typing_extensions import LiteralString, Self, TypeAlias
 
 from . import _mysql, cursors
 from ._exceptions import (
     DatabaseError as DatabaseError,
     DataError as DataError,
     Error as Error,
     IntegrityError as IntegrityError,
@@ -12,36 +14,41 @@
     InternalError as InternalError,
     NotSupportedError as NotSupportedError,
     OperationalError as OperationalError,
     ProgrammingError as ProgrammingError,
     Warning as Warning,
 )
 
-re_numeric_part: Any
+# Any kind of object that can be passed to Connection.literal().
+# The allowed types depend on the defined encoders, but the following
+# types are always allowed.
+_Literal: TypeAlias = str | bytearray | bytes | tuple[_Literal, ...] | list[_Literal] | Any
+
+re_numeric_part: Pattern[str]
 
 def numeric_part(s): ...
 
 class Connection(_mysql.connection):
     default_cursor: type[cursors.Cursor]
     cursorclass: type[cursors.BaseCursor]
-    encoders: Any
+    encoders: Incomplete
     encoding: str
-    messages: Any
+    messages: Incomplete
     def __init__(self, *args, **kwargs) -> None: ...
     def __enter__(self) -> Self: ...
     def __exit__(
         self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: TracebackType | None
     ) -> None: ...
     def autocommit(self, on: bool) -> None: ...
     def cursor(self, cursorclass: type[cursors.BaseCursor] | None = None): ...
     def query(self, query) -> None: ...
-    def literal(self, o): ...
+    def literal(self, o: _Literal) -> bytes: ...
     def begin(self) -> None: ...
     def warning_count(self): ...
-    def set_character_set(self, charset) -> None: ...
+    def set_character_set(self, charset: LiteralString, collation: LiteralString | None = None) -> None: ...
     def set_sql_mode(self, sql_mode) -> None: ...
     def show_warnings(self): ...
     Warning: type[BaseException]
     Error: type[BaseException]
     InterfaceError: type[BaseException]
     DatabaseError: type[BaseException]
     DataError: type[BaseException]
```

### Comparing `types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/CR.pyi` & `types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/CR.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.1.5.7/MySQLdb-stubs/constants/ER.pyi` & `types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/ER.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.1.5.7/MySQLdb-stubs/converters.pyi` & `types-mysqlclient-2.2.0.0/MySQLdb-stubs/converters.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import array
-from typing import Any
+from _typeshed import Incomplete
 
 from MySQLdb._exceptions import ProgrammingError as ProgrammingError
 from MySQLdb._mysql import string_literal as string_literal
 from MySQLdb.constants import FIELD_TYPE as FIELD_TYPE, FLAG as FLAG
 from MySQLdb.times import (
     Date as Date,
     Date_or_None as Date_or_None,
@@ -11,20 +11,20 @@
     DateTime_or_None as DateTime_or_None,
     DateTimeDelta2literal as DateTimeDelta2literal,
     DateTimeDeltaType as DateTimeDeltaType,
     DateTimeType as DateTimeType,
     TimeDelta_or_None as TimeDelta_or_None,
 )
 
-NoneType: Any
+NoneType: Incomplete
 ArrayType = array.array
 
 def Bool2Str(s, d): ...
 def Set2Str(s, d): ...
 def Thing2Str(s, d): ...
 def Float2Str(o, d): ...
 def None2NULL(o, d): ...
 def Thing2Literal(o, d): ...
 def Decimal2Literal(o, d): ...
 def array2Str(o, d): ...
 
-conversions: Any
+conversions: Incomplete
```

### Comparing `types-mysqlclient-2.1.5.7/MySQLdb-stubs/cursors.pyi` & `types-mysqlclient-2.2.0.0/MySQLdb-stubs/cursors.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from _typeshed import Incomplete
-from typing import Any
+from collections.abc import Iterable
+from re import Pattern
+from typing_extensions import LiteralString, TypeAlias
 
-RE_INSERT_VALUES: Any
+from .connections import _Literal
+
+_Arguments: TypeAlias = dict[str, _Literal] | dict[bytes, _Literal] | Iterable[_Literal]
+
+RE_INSERT_VALUES: Pattern[str]
 
 class BaseCursor:
     from ._exceptions import (
         DatabaseError as DatabaseError,
         DataError as DataError,
         Error as Error,
         IntegrityError as IntegrityError,
@@ -14,50 +20,51 @@
         MySQLError as MySQLError,
         NotSupportedError as NotSupportedError,
         OperationalError as OperationalError,
         ProgrammingError as ProgrammingError,
         Warning as Warning,
     )
 
-    max_stmt_length: Any
-    connection: Any
-    description: Any
-    description_flags: Any
+    max_stmt_length: Incomplete
+    connection: Incomplete
+    description: Incomplete
+    description_flags: Incomplete
     rowcount: int
     arraysize: int
-    lastrowid: Any
-    rownumber: Any
+    lastrowid: Incomplete
+    rownumber: Incomplete
     def __init__(self, connection) -> None: ...
     def close(self) -> None: ...
     def __enter__(self): ...
     def __exit__(self, *exc_info: object) -> None: ...
     def nextset(self): ...
     def setinputsizes(self, *args) -> None: ...
     def setoutputsizes(self, *args) -> None: ...
     def execute(self, query, args: Incomplete | None = None): ...
-    def executemany(self, query: str, args: list[Any]) -> int: ...
+    def mogrify(self, query: str | bytes, args: _Arguments | None = None) -> str: ...
+    def executemany(self, query: LiteralString, args: Iterable[_Arguments]) -> int | None: ...
     def callproc(self, procname, args=()): ...
     def __iter__(self): ...
 
 class CursorStoreResultMixIn:
-    rownumber: Any
+    rownumber: Incomplete
     def fetchone(self): ...
     def fetchmany(self, size: Incomplete | None = None): ...
     def fetchall(self): ...
     def scroll(self, value, mode: str = "relative") -> None: ...
     def __iter__(self): ...
 
 class CursorUseResultMixIn:
-    rownumber: Any
+    rownumber: Incomplete
     def fetchone(self): ...
     def fetchmany(self, size: Incomplete | None = None): ...
     def fetchall(self): ...
     def __iter__(self): ...
     def next(self): ...
-    __next__: Any
+    __next__ = next
 
 class CursorTupleRowsMixIn: ...
 class CursorDictRowsMixIn: ...
 class Cursor(CursorStoreResultMixIn, CursorTupleRowsMixIn, BaseCursor): ...
 class DictCursor(CursorStoreResultMixIn, CursorDictRowsMixIn, BaseCursor): ...
 class SSCursor(CursorUseResultMixIn, CursorTupleRowsMixIn, BaseCursor): ...
 class SSDictCursor(CursorUseResultMixIn, CursorDictRowsMixIn, BaseCursor): ...
```

### Comparing `types-mysqlclient-2.1.5.7/MySQLdb-stubs/times.pyi` & `types-mysqlclient-2.2.0.0/MySQLdb-stubs/times.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.1.5.7/PKG-INFO` & `types-mysqlclient-2.2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mysqlclient
-Version: 2.1.5.7
+Version: 2.2.0.0
 Summary: Typing stubs for mysqlclient
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mysqlclient.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mysqlclient`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mysqlclient. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `b10f482e36f67a9d7aae13c49a4d14cb17df97e6` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

### Comparing `types-mysqlclient-2.1.5.7/setup.py` & `types-mysqlclient-2.2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mysqlclient`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mysqlclient. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `b10f482e36f67a9d7aae13c49a4d14cb17df97e6` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.5.7",
+      version="2.2.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mysqlclient.md",
```

### Comparing `types-mysqlclient-2.1.5.7/types_mysqlclient.egg-info/PKG-INFO` & `types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mysqlclient
-Version: 2.1.5.7
+Version: 2.2.0.0
 Summary: Typing stubs for mysqlclient
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mysqlclient.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mysqlclient`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mysqlclient. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `b10f482e36f67a9d7aae13c49a4d14cb17df97e6` and was tested
+with mypy 1.3.0, pyright 1.1.314, and
+pytype 2023.6.2.
```

### Comparing `types-mysqlclient-2.1.5.7/types_mysqlclient.egg-info/SOURCES.txt` & `types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

