# Comparing `tmp/pythogen-0.1.8.tar.gz` & `tmp/pythogen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.1.8.tar", max compression
+gzip compressed data, was "pythogen-0.1.9.tar", max compression
```

## Comparing `pythogen-0.1.8.tar` & `pythogen-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-03-10 11:50:46.375757 pythogen-0.1.8/LICENSE
--rw-r--r--   0        0        0     2830 2023-03-10 11:50:46.375757 pythogen-0.1.8/README.md
--rw-r--r--   0        0        0     1381 2023-03-10 11:50:46.379757 pythogen-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 11:50:46.379757 pythogen-0.1.8/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1445 2023-03-10 11:50:46.379757 pythogen-0.1.8/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7247 2023-03-10 11:50:46.379757 pythogen-0.1.8/pythogen/models.py
--rw-r--r--   0        0        0     2363 2023-03-10 11:50:46.379757 pythogen-0.1.8/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-03-10 11:50:46.379757 pythogen-0.1.8/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3296 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/document.py
--rw-r--r--   0        0        0      601 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3177 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2156 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2461 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1098 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3203 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1834 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/response.py
--rw-r--r--   0        0        0    13999 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0     8582 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/settings.py
--rw-r--r--   0        0        0     4759 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0     9165 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      337 2023-03-10 11:50:46.383758 pythogen-0.1.8/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 pythogen-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-21 14:52:33.982397 pythogen-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2830 2023-03-21 14:52:33.982397 pythogen-0.1.9/README.md
+-rw-r--r--   0        0        0     1381 2023-03-21 14:52:33.986397 pythogen-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1445 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/entrypoint.py
+-rw-r--r--   0        0        0     7247 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/models.py
+-rw-r--r--   0        0        0     2363 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3296 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      601 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3177 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2156 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2461 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1098 2023-03-21 14:52:33.986397 pythogen-0.1.9/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3203 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1834 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    15724 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0     9193 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/renderer.py
+-rw-r--r--   0        0        0      172 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/settings.py
+-rw-r--r--   0        0        0     4759 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/client/httpx-method.j2
+-rw-r--r--   0        0        0     1668 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/client/httpx-request-metrics.j2
+-rw-r--r--   0        0        0     9165 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/httpx.j2
+-rw-r--r--   0        0        0       33 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/init-py.j2
+-rw-r--r--   0        0        0      337 2023-03-21 14:52:33.990397 pythogen-0.1.9/pythogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 pythogen-0.1.9/PKG-INFO
```

### Comparing `pythogen-0.1.8/LICENSE` & `pythogen-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/README.md` & `pythogen-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pyproject.toml` & `pythogen-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.1.8"
+version = "0.1.9"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
```

### Comparing `pythogen-0.1.8/pythogen/entrypoint.py` & `pythogen-0.1.9/pythogen/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/models.py` & `pythogen-0.1.9/pythogen/models.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/packager.py` & `pythogen-0.1.9/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/document.py` & `pythogen-0.1.9/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.1.9/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/operations.py` & `pythogen-0.1.9/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/parameters.py` & `pythogen-0.1.9/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/paths.py` & `pythogen-0.1.9/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/references.py` & `pythogen-0.1.9/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/request_body.py` & `pythogen-0.1.9/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/response.py` & `pythogen-0.1.9/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/parsers/schemas.py` & `pythogen-0.1.9/pythogen/parsers/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -311,14 +311,51 @@
     ) -> Union[Optional[models.SchemaObject], List[models.SchemaObject]]:
         items_schema_data = data.get('items')
         if items_schema_data:
             if items_schema_data.get('$ref', None):
                 resolved_ref = self._ref_resolver.resolve(items_schema_data['$ref'])
                 schema = self.parse_item(resolved_ref.ref_id, resolved_ref.ref_data, from_depth_level=True)
                 return schema
+            elif items_schema_data.get('anyOf'):
+                items = []
+                for any_ref_item in items_schema_data['anyOf']:
+                    ref = any_ref_item.get('$ref', None)
+                    any_ref_any_type = any_ref_item.get('type')
+                    if ref:
+                        resolved_ref = self._ref_resolver.resolve(ref)
+                        ref_schema = self.parse_item(resolved_ref.ref_id, resolved_ref.ref_data, from_depth_level=True)
+                        items.append(ref_schema)
+                    elif any_ref_any_type in PRIMITIVE_TYPES:
+                        items.append(
+                            models.SchemaObject(
+                                id='',
+                                type=models.Type(any_ref_any_type),
+                                enum=None,
+                                properties=[],
+                                title=None,
+                                format=None,
+                                items=None,
+                                required=None,
+                            )
+                        )
+                    else:
+                        items_schema_id = f'<inline+{models.SchemaObject.__name__}>'
+                        schema = self.parse_item(items_schema_id, items_schema_data)
+                        self._inline_schema_aggregator.add(items_schema_id, schema)
+
+                return models.SchemaObject(
+                    id='',
+                    type=models.Type.any_of,
+                    enum=None,
+                    properties=[],
+                    title=None,
+                    format=None,
+                    items=items,
+                    required=None,
+                )
             else:
                 parent_raw_type = data.get('type')
                 if parent_raw_type == 'array':
                     items_schema_id = f'{parent_schema_id}Item'
                 else:
                     items_schema_id = f'<inline+{models.SchemaObject.__name__}>'
                 schema = self.parse_item(items_schema_id, items_schema_data)
```

### Comparing `pythogen-0.1.8/pythogen/renderer.py` & `pythogen-0.1.9/pythogen/renderer.py`

 * *Files 7% similar despite different names*

```diff
@@ -222,16 +222,33 @@
             representation = primitive_type_mapping[schema.type]
 
     elif schema.type == models.Type.object and schema.id != '<inline+SchemaObject>':
         representation = classname(schema.id)
 
     elif schema.type == models.Type.array and schema.items:
         if schema.items.type is models.Type.any_of:  # type: ignore
-            items = [classname(item.id) for item in schema.items.items]  # type: ignore
-            representation = f'List[Union{items}]'
+            class_items = []
+            primitive_items = []
+            for item in schema.items.items:  # type: ignore
+                if item.id:
+                    class_items.append(classname(item.id))
+                else:
+                    primitive_items.append(primitive_type_mapping[item.type])
+
+            class_items_str = ', '.join([f'{class_item}' for class_item in class_items])
+            primitives_items_str = ', '.join(primitive_items)
+
+            items = []
+            if class_items_str:
+                items.append(class_items_str)
+            if primitives_items_str:
+                items.append(primitives_items_str)
+
+            items_str = ', '.join(items)
+            representation = f'List[Union[{items_str}]]'
         else:
             item = j2_typerepr(schema.items)  # type: ignore
             representation = f'List[{item}]'
 
     elif schema.type == models.Type.any_of:
         representation = classname(schema.id)
```

### Comparing `pythogen-0.1.8/pythogen/templates/client/httpx-method.j2` & `pythogen-0.1.9/pythogen/templates/client/httpx-method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.1.9/pythogen/templates/client/httpx-request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/pythogen/templates/httpx.j2` & `pythogen-0.1.9/pythogen/templates/httpx.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.1.8/PKG-INFO` & `pythogen-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.1.8
+Version: 0.1.9
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.7,<4.0
```

