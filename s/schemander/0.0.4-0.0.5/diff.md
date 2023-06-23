# Comparing `tmp/schemander-0.0.4.tar.gz` & `tmp/schemander-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemander-0.0.4.tar", last modified: Fri Jun 23 18:53:22 2023, max compression
+gzip compressed data, was "schemander-0.0.5.tar", last modified: Fri Jun 23 19:08:18 2023, max compression
```

## Comparing `schemander-0.0.4.tar` & `schemander-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:53:22.589091 schemander-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-23 18:52:48.000000 schemander-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 18:53:22.589091 schemander-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 18:52:48.000000 schemander-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-23 18:52:48.000000 schemander-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:53:22.589091 schemander-0.0.4/schemander.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 18:53:22.000000 schemander-0.0.4/schemander.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-06-23 18:52:48.000000 schemander-0.0.4/schemander.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:53:22.589091 schemander-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:18.073492 schemander-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-23 19:07:40.000000 schemander-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 19:08:18.073492 schemander-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 19:07:40.000000 schemander-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-23 19:07:40.000000 schemander-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:18.073492 schemander-0.0.5/schemander.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-23 19:07:40.000000 schemander-0.0.5/schemander.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:08:18.073492 schemander-0.0.5/setup.cfg
```

### Comparing `schemander-0.0.4/LICENSE` & `schemander-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `schemander-0.0.4/PKG-INFO` & `schemander-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.4
+Version: 0.0.5
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `schemander-0.0.4/README.md` & `schemander-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `schemander-0.0.4/pyproject.toml` & `schemander-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-version = "0.0.4"
+version = "0.0.5"
 name = "schemander"
 authors = [
     { name="Miguel Alejandro Salgado Zapien", email="ekiim@ekiim.xyz"},
 ]
 description = "A single file schema validator for dictionaries."
 readme="README.md"
 requires-python = ">= 3.11"
```

### Comparing `schemander-0.0.4/schemander.egg-info/PKG-INFO` & `schemander-0.0.5/schemander.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.4
+Version: 0.0.5
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `schemander-0.0.4/schemander.py` & `schemander-0.0.5/schemander.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import phonenumbers
 
 
 JsonType = t.Union[
     None, int, float, str, bool, list["JsonType"], dict[str, "JsonType"]
 ]
 JsonRoot = dict[str, JsonType]
-SchemaType = t.TypeVar("SchemaType", bound="Schema")
 
 
 class InternalObjectTypeString(str):
     object_class: t.Type[t.Any]
     value: t.Any
 
     def __new__(cls, value: str | t.Any) -> "InternalObjectTypeString":
@@ -149,17 +148,19 @@
     ) -> t.Tuple[str, phonenumbers.PhoneNumber]:
         is_string = isinstance(value, str)
         is_phone_obj = isinstance(value, phonenumbers.PhoneNumber)
         try:
             if not is_string and not is_phone_obj:
                 raise TypeError
             if is_phone_obj:
-                obj = value
+                obj: phonenumbers.PhoneNumber = value  # type: ignore
             else:
-                obj = phonenumbers.parse(value, None, keep_raw_input=True)
+                obj = phonenumbers.parse(
+                    value, None, keep_raw_input=True  # type: ignore
+                )
         except (TypeError, phonenumbers.NumberParseException) as e:
             raise ValueError
 
         string = phonenumbers.format_number(
             obj,
             phonenumbers.PhoneNumberFormat.E164,
         )
@@ -299,16 +300,15 @@
     def to_dict(self) -> JsonRoot:
         return {k: getattr(self, k) for k in self.__class__._annotations()}
 
     def to_minimal_dict(self) -> JsonRoot:
         return {k: v for k, v in self.to_dict().items() if v is not None}
 
     @classmethod
-    def from_dict(cls, data: JsonRoot | SchemaType) -> SchemaType:
-
+    def from_dict(cls, data: t.Union[JsonRoot, "Schema"]) -> "Schema":
         if isinstance(data, Schema):
             return data
 
         annotations = cls._annotations().keys()
         if set(data.keys()) - annotations:
             raise ValueError("Arguments outside schema were provided.")
         kwargs: dict[str, t.Any] = {
```

