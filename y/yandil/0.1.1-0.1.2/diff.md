# Comparing `tmp/yandil-0.1.1.tar.gz` & `tmp/yandil-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.1.1.tar", max compression
+gzip compressed data, was "yandil-0.1.2.tar", max compression
```

## Comparing `yandil-0.1.1.tar` & `yandil-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11358 2023-06-22 17:48:56.767189 yandil-0.1.1/README.md
--rw-r--r--   0        0        0      817 2023-06-22 17:49:49.976006 yandil-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0     8588 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/dependency.py
--rw-r--r--   0        0        0     1020 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3002 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      255 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     2364 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-22 17:48:56.767189 yandil-0.1.1/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 yandil-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-22 23:09:51.446353 yandil-0.1.2/README.md
+-rw-r--r--   0        0        0      817 2023-06-22 23:10:53.499451 yandil-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0     8588 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1020 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      257 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      255 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     2364 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 yandil-0.1.2/PKG-INFO
```

### Comparing `yandil-0.1.1/README.md` & `yandil-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/pyproject.toml` & `yandil-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.1.1"
+version = "0.1.2"
 description = "Yet ANother Dependency Injection Library"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 
@@ -30,15 +30,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.1"
+version = "0.1.2"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.1.1/src/yandil/configuration/configuration_container.py` & `yandil-0.1.2/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/container.py` & `yandil-0.1.2/src/yandil/container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/declarative/decorators.py` & `yandil-0.1.2/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/dependency.py` & `yandil-0.1.2/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/dependency_filler.py` & `yandil-0.1.2/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/discovery/class_discovery.py` & `yandil-0.1.2/src/yandil/discovery/class_discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ast import Call, ClassDef, FunctionDef, Name, parse
+from ast import Call, ClassDef, FunctionDef, Name, Subscript, parse
 from dataclasses import dataclass
 from importlib import import_module
 from os import path
 from os.path import relpath, splitext
 from typing import Iterable, Set, Type
 
 
@@ -24,17 +24,22 @@
 
     for node in module_ast.body:
         if isinstance(node, ClassDef):
             yield node
 
 
 def exclude_abstract_classes(class_nodes: Iterable[ClassDef]) -> Iterable[ClassDef]:
+    abstract_bases = {"Protocol", "Generic", "ABC"}
+
     def __is_abstract_class_node(node: ClassDef) -> bool:
         for base in node.bases:
-            if isinstance(base, Name) and base.id in {"Protocol", "Generic", "ABC"}:
+            if isinstance(base, Name) and base.id in abstract_bases:
+                return True
+
+            if isinstance(base, Subscript) and isinstance(base.value, Name) and base.value.id in abstract_bases:
                 return True
         return False
 
     for class_node in class_nodes:
         if not __is_abstract_class_node(class_node):
             yield class_node
```

### Comparing `yandil-0.1.1/src/yandil/discovery/module_discovery.py` & `yandil-0.1.2/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.1.2/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.1.2/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/src/yandil/typing_tools.py` & `yandil-0.1.2/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.1/PKG-INFO` & `yandil-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yet ANother Dependency Injection Library
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

