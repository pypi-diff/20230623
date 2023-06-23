# Comparing `tmp/schemander-0.0.3.tar.gz` & `tmp/schemander-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemander-0.0.3.tar", last modified: Wed Jun  7 22:23:22 2023, max compression
+gzip compressed data, was "schemander-0.0.4.tar", last modified: Fri Jun 23 18:53:22 2023, max compression
```

## Comparing `schemander-0.0.3.tar` & `schemander-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:22.509270 schemander-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-07 22:22:50.000000 schemander-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-07 22:23:22.509270 schemander-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-07 22:22:50.000000 schemander-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 22:22:50.000000 schemander-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:22.509270 schemander-0.0.3/schemander.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-06-07 22:22:50.000000 schemander-0.0.3/schemander.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 22:23:22.509270 schemander-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:53:22.589091 schemander-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-23 18:52:48.000000 schemander-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 18:53:22.589091 schemander-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 18:52:48.000000 schemander-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-23 18:52:48.000000 schemander-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:53:22.589091 schemander-0.0.4/schemander.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-06-23 18:52:48.000000 schemander-0.0.4/schemander.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:53:22.589091 schemander-0.0.4/setup.cfg
```

### Comparing `schemander-0.0.3/LICENSE` & `schemander-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `schemander-0.0.3/PKG-INFO` & `schemander-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.3
+Version: 0.0.4
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `schemander-0.0.3/README.md` & `schemander-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `schemander-0.0.3/pyproject.toml` & `schemander-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-version = "0.0.3"
+version = "0.0.4"
 name = "schemander"
 authors = [
     { name="Miguel Alejandro Salgado Zapien", email="ekiim@ekiim.xyz"},
 ]
 description = "A single file schema validator for dictionaries."
 readme="README.md"
 requires-python = ">= 3.11"
```

### Comparing `schemander-0.0.3/schemander.egg-info/PKG-INFO` & `schemander-0.0.4/schemander.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.3
+Version: 0.0.4
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `schemander-0.0.3/schemander.py` & `schemander-0.0.4/schemander.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import typing as t
 
 from datetime import (
     date,
     datetime,
     timezone,
 )
+from enum import Enum
 from functools import reduce
-from itertools import chain
 from json import JSONEncoder
-from random import choice
 from re import fullmatch
 from types import UnionType, NoneType
 from uuid import UUID
 from zoneinfo import (
     ZoneInfo,
     ZoneInfoNotFoundError,
 )
@@ -144,29 +143,32 @@
 class Phone(InternalObjectTypeString):
     object_class = phonenumbers.PhoneNumber
 
     @classmethod
     def convert(
         cls, value: str | phonenumbers.PhoneNumber
     ) -> t.Tuple[str, phonenumbers.PhoneNumber]:
+        is_string = isinstance(value, str)
+        is_phone_obj = isinstance(value, phonenumbers.PhoneNumber)
         try:
-            if not isinstance(value, str) and not isinstance(
-                value, phonenumbers.PhoneNumber
-            ):
+            if not is_string and not is_phone_obj:
                 raise TypeError
-            if isinstance(value, phonenumbers.PhoneNumber):
+            if is_phone_obj:
                 obj = value
             else:
-                obj = phonenumbers.parse(value, None)
-        except (TypeError, phonenumbers.NumberParseException):
+                obj = phonenumbers.parse(value, None, keep_raw_input=True)
+        except (TypeError, phonenumbers.NumberParseException) as e:
             raise ValueError
+
         string = phonenumbers.format_number(
             obj,
             phonenumbers.PhoneNumberFormat.E164,
         )
+        if obj.raw_input and obj.raw_input != string:
+            raise ValueError("Incorrect format for phone number.")
         return string, obj
 
 
 class RegexValidatedString(str):
     regex = ".*"
 
     def __new__(cls, string: str) -> "RegexValidatedString":
@@ -297,15 +299,19 @@
     def to_dict(self) -> JsonRoot:
         return {k: getattr(self, k) for k in self.__class__._annotations()}
 
     def to_minimal_dict(self) -> JsonRoot:
         return {k: v for k, v in self.to_dict().items() if v is not None}
 
     @classmethod
-    def from_dict(cls, data: JsonRoot) -> "Schema":
+    def from_dict(cls, data: JsonRoot | SchemaType) -> SchemaType:
+
+        if isinstance(data, Schema):
+            return data
+
         annotations = cls._annotations().keys()
         if set(data.keys()) - annotations:
             raise ValueError("Arguments outside schema were provided.")
         kwargs: dict[str, t.Any] = {
             **cls._nullable_fields(),
             **cls._default_values(),
             **{k: v for k, v in data.items() if k in annotations},
```

