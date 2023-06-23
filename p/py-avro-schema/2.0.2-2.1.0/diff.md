# Comparing `tmp/py-avro-schema-2.0.2.tar.gz` & `tmp/py-avro-schema-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-avro-schema-2.0.2.tar", last modified: Mon Apr 10 16:03:38 2023, max compression
+gzip compressed data, was "py-avro-schema-2.1.0.tar", last modified: Fri Jun 23 11:37:52 2023, max compression
```

## Comparing `py-avro-schema-2.0.2.tar` & `py-avro-schema-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.406587 py-avro-schema-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/py_avro_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:03:38.414588 py-avro-schema-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.406587 py-avro-schema-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/src/py_avro_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33004 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/src/py_avro_schema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 16:03:38.000000 py-avro-schema-2.0.2/src/py_avro_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:03:38.410587 py-avro-schema-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_logicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 16:03:25.000000 py-avro-schema-2.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.675762 py-avro-schema-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.667762 py-avro-schema-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.671762 py-avro-schema-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-23 11:37:52.675762 py-avro-schema-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.671762 py-avro-schema-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/docs/py_avro_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:37:52.675762 py-avro-schema-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.671762 py-avro-schema-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.671762 py-avro-schema-2.1.0/src/py_avro_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/src/py_avro_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34882 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/src/py_avro_schema/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/src/py_avro_schema/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/src/py_avro_schema/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/src/py_avro_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.671762 py-avro-schema-2.1.0/src/py_avro_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-23 11:37:52.000000 py-avro-schema-2.1.0/src/py_avro_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 11:37:52.000000 py-avro-schema-2.1.0/src/py_avro_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:37:52.000000 py-avro-schema-2.1.0/src/py_avro_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-23 11:37:52.000000 py-avro-schema-2.1.0/src/py_avro_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 11:37:52.000000 py-avro-schema-2.1.0/src/py_avro_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:37:52.675762 py-avro-schema-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tests/test_logicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tests/test_plain_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-23 11:37:36.000000 py-avro-schema-2.1.0/tox.ini
```

### Comparing `py-avro-schema-2.0.2/.flake8` & `py-avro-schema-2.1.0/.flake8`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/.github/workflows/release-package.yml` & `py-avro-schema-2.1.0/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/.github/workflows/test-package.yml` & `py-avro-schema-2.1.0/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/.gitignore` & `py-avro-schema-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/LICENSE` & `py-avro-schema-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/LICENSE_HEADER.txt` & `py-avro-schema-2.1.0/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/PKG-INFO` & `py-avro-schema-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.0.2
+Version: 2.1.0
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.0.2/README.md` & `py-avro-schema-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/docs/conf.py` & `py-avro-schema-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/docs/index.rst` & `py-avro-schema-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/docs/tutorial.rst` & `py-avro-schema-2.1.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/docs/types.rst` & `py-avro-schema-2.1.0/docs/types.rst`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,56 @@
 The Avro record schema's ``doc`` attribute is populated from the Python class's docstring.
 For individual model fields, the ``doc`` attribute is taken from the Pydantic field's :attr:`description` attribute.
 To *disable* this, pass the option :attr:`py_avro_schema.Option.NO_DOC`.
 
 Recursive or repeated reference to the same Pydantic class is supported. After the first time the schema is output, any subsequent references are by name only.
 
 
+Plain Python classes
+~~~~~~~~~~~~~~~~~~~~
+
+Supports Python classes with a :meth:`__init__` where all arguments have type hints and fully define all schema fields.
+
+Avro schema: ``record``
+
+The Avro ``record`` type is a named schema.
+**py-avro-schema** uses the Python class name as the schema name.
+
+Example::
+
+    class Port:
+        """A port you can sail too"""
+
+        def __init__(self, name: str, country: str = "NLD"):
+            self.name = name
+            self.country = country.upper()
+
+Is output as:
+
+.. code-block:: json
+
+   {
+     "type": "record",
+     "name": "Port",
+     "namespace": "shipping",
+     "doc": "A port you can sail too",
+     "fields": [
+       {
+         "name": "name",
+         "type": "string"
+       },
+       {
+         "name": "country",
+         "type": "string",
+         "default": "NLD"
+       }
+     ]
+   }
+
+
 :class:`typing.Union`
 ~~~~~~~~~~~~~~~~~~~~~
 
 Avro schema: JSON array of multiple Avro schemas
 
 Union members can be any other type supported by **py-avro-schema**.
```

### Comparing `py-avro-schema-2.0.2/pyproject.toml` & `py-avro-schema-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/src/py_avro_schema/__init__.py` & `py-avro-schema-2.1.0/src/py_avro_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/src/py_avro_schema/_schemas.py` & `py-avro-schema-2.1.0/src/py_avro_schema/_schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,25 @@
 import dataclasses
 import datetime
 import decimal
 import enum
 import inspect
 import sys
 import uuid
-from typing import TYPE_CHECKING, Any, Dict, ForwardRef, List, Optional, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    ForwardRef,
+    List,
+    Optional,
+    Type,
+    Union,
+    get_type_hints,
+)
 
 import orjson
 import typeguard
 
 if TYPE_CHECKING:
     # Pydantic not necessarily required at runtime
     import pydantic  # type: ignore
@@ -825,14 +835,52 @@
         if not py_field.allow_none:
             return py_field.annotation
         else:
             # Pydantic allows setting fields to ``None`` even if there is no ``NoneType`` annotation...
             return Optional[py_field.annotation]
 
 
+class PlainClassSchema(RecordSchema):
+    """An Avro record schema for a plain Python class with typed constructor method arguments"""
+
+    @classmethod
+    def handles_type(cls, py_type: Type) -> bool:
+        """Whether this schema class can represent a given Python class"""
+        return (
+            not dataclasses.is_dataclass(py_type)  # Dataclasses are handled above
+            and not hasattr(py_type, "__fields__")  # Pydantic models too
+            and bool(get_type_hints(py_type.__init__))  # Any other class with __init__ with typed args
+        )
+
+    def __init__(self, py_type: Type, namespace: Optional[str] = None, options: Option = Option(0)):
+        """
+        An Avro record schema for a plain Python class with typed constructor method arguments
+
+        :param py_type:   The Python class to generate a schema for.
+        :param namespace: The Avro namespace to add to schemas.
+        :param options:   Schema generation options.
+        """
+        super().__init__(py_type, namespace=namespace, options=options)
+        # Extracting arguments from __init__, dropping first argument `self`.
+        self.py_fields = list(inspect.signature(py_type.__init__).parameters.values())[1:]
+        self.record_fields = [self._record_field(field) for field in self.py_fields]
+
+    def _record_field(self, py_field: inspect.Parameter) -> RecordField:
+        """Return an Avro record field object for a given Python instance attribute"""
+        default = py_field.default if py_field.default != inspect.Parameter.empty else dataclasses.MISSING
+        field_obj = RecordField(
+            py_type=py_field.annotation,
+            name=py_field.name,
+            namespace=self.namespace_override,
+            default=default,
+            options=self.options,
+        )
+        return field_obj
+
+
 def _doc_for_class(py_type: Type) -> str:
     """Return the first line of the docstring for a given class, if any"""
     doc = inspect.getdoc(py_type)
     if doc:
         # Take the first sentence
         doc = doc.split("\n\n", 1)[0].replace("\n", " ").replace("  ", " ").strip()
         return doc
```

### Comparing `py-avro-schema-2.0.2/src/py_avro_schema/_testing.py` & `py-avro-schema-2.1.0/src/py_avro_schema/_testing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/src/py_avro_schema/_typing.py` & `py-avro-schema-2.1.0/src/py_avro_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/src/py_avro_schema.egg-info/PKG-INFO` & `py-avro-schema-2.1.0/src/py_avro_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.0.2
+Version: 2.1.0
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.0.2/src/py_avro_schema.egg-info/SOURCES.txt` & `py-avro-schema-2.1.0/src/py_avro_schema.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 src/py_avro_schema.egg-info/SOURCES.txt
 src/py_avro_schema.egg-info/dependency_links.txt
 src/py_avro_schema.egg-info/requires.txt
 src/py_avro_schema.egg-info/top_level.txt
 tests/test_avro_schema.py
 tests/test_dataclass.py
 tests/test_logicals.py
+tests/test_plain_class.py
 tests/test_primitives.py
 tests/test_pydantic.py
 tests/test_typing.py
```

### Comparing `py-avro-schema-2.0.2/tests/test_avro_schema.py` & `py-avro-schema-2.1.0/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/tests/test_dataclass.py` & `py-avro-schema-2.1.0/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/tests/test_logicals.py` & `py-avro-schema-2.1.0/tests/test_logicals.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/tests/test_primitives.py` & `py-avro-schema-2.1.0/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/tests/test_pydantic.py` & `py-avro-schema-2.1.0/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/tests/test_typing.py` & `py-avro-schema-2.1.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.0.2/tox.ini` & `py-avro-schema-2.1.0/tox.ini`

 * *Files identical despite different names*

