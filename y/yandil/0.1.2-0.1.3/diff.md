# Comparing `tmp/yandil-0.1.2.tar.gz` & `tmp/yandil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandil-0.1.2.tar", max compression
+gzip compressed data, was "yandil-0.1.3.tar", max compression
```

## Comparing `yandil-0.1.2.tar` & `yandil-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11358 2023-06-22 23:09:51.446353 yandil-0.1.2/README.md
--rw-r--r--   0        0        0      817 2023-06-22 23:10:53.499451 yandil-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/__init__.py
--rw-r--r--   0        0        0      148 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/argument.py
--rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/configuration/__init__.py
--rw-r--r--   0        0        0      800 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/configuration/configuration_container.py
--rw-r--r--   0        0        0      507 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/configuration/environment.py
--rw-r--r--   0        0        0     8588 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/container.py
--rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/declarative/__init__.py
--rw-r--r--   0        0        0      516 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/declarative/decorators.py
--rw-r--r--   0        0        0      799 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/dependency.py
--rw-r--r--   0        0        0     1020 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/dependency_filler.py
--rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/discovery/__init__.py
--rw-r--r--   0        0        0     3192 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/discovery/class_discovery.py
--rw-r--r--   0        0        0      883 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/discovery/module_discovery.py
--rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/abstract_class_not_allowed_error.py
--rw-r--r--   0        0        0      467 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/configuration_value_type_mismatch_error.py
--rw-r--r--   0        0        0      239 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/dependency_not_found_error.py
--rw-r--r--   0        0        0      257 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/missing_configuration_value_error.py
--rw-r--r--   0        0        0      127 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/missing_type_hint_item_type_error.py
--rw-r--r--   0        0        0      255 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/primary_dependency_already_defined_error.py
--rw-r--r--   0        0        0      243 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/errors/primary_dependency_not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/loaders/__init__.py
--rw-r--r--   0        0        0     1188 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/loaders/declarative_dependency_loader.py
--rw-r--r--   0        0        0     2364 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/loaders/self_discover_dependency_loader.py
--rw-r--r--   0        0        0     1238 2023-06-22 23:09:51.446353 yandil-0.1.2/src/yandil/typing_tools.py
--rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 yandil-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-23 15:41:24.685373 yandil-0.1.3/README.md
+-rw-r--r--   0        0        0      817 2023-06-23 15:42:23.833490 yandil-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/argument.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/configuration/__init__.py
+-rw-r--r--   0        0        0      800 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/configuration/configuration_container.py
+-rw-r--r--   0        0        0      507 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/configuration/environment.py
+-rw-r--r--   0        0        0     9192 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/container.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/declarative/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/declarative/decorators.py
+-rw-r--r--   0        0        0      799 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/dependency.py
+-rw-r--r--   0        0        0     1020 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/dependency_filler.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/discovery/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/discovery/class_discovery.py
+-rw-r--r--   0        0        0      883 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/discovery/module_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/abstract_class_not_allowed_error.py
+-rw-r--r--   0        0        0      467 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/configuration_value_type_mismatch_error.py
+-rw-r--r--   0        0        0      239 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/dependency_not_found_error.py
+-rw-r--r--   0        0        0      257 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/missing_configuration_value_error.py
+-rw-r--r--   0        0        0      127 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/missing_type_hint_item_type_error.py
+-rw-r--r--   0        0        0      255 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/primary_dependency_already_defined_error.py
+-rw-r--r--   0        0        0      243 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/errors/primary_dependency_not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/loaders/__init__.py
+-rw-r--r--   0        0        0     1188 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/loaders/declarative_dependency_loader.py
+-rw-r--r--   0        0        0     2364 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/loaders/self_discover_dependency_loader.py
+-rw-r--r--   0        0        0     1238 2023-06-23 15:41:24.689372 yandil-0.1.3/src/yandil/typing_tools.py
+-rw-r--r--   0        0        0    11689 1970-01-01 00:00:00.000000 yandil-0.1.3/PKG-INFO
```

### Comparing `yandil-0.1.2/README.md` & `yandil-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/pyproject.toml` & `yandil-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yandil"
-version = "0.1.2"
+version = "0.1.3"
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
-version = "0.1.2"
+version = "0.1.3"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `yandil-0.1.2/src/yandil/configuration/configuration_container.py` & `yandil-0.1.3/src/yandil/configuration/configuration_container.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/container.py` & `yandil-0.1.3/src/yandil/container.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,48 +47,60 @@
 
     def add(self, cls: Type, is_primary: Optional[bool] = None) -> None:
         if self.__is_abstract_class(cls):
             raise AbstractClassNotAllowedError(cls)
 
         dependency = Dependency(cls, is_primary=is_primary)
 
-        self.__update_parents_map(cls, is_primary)
+        self.__update_bases_map(cls, is_primary)
         self.__dependency_map[cls] = dependency
 
     def __setitem__(self, cls: Type[DT], value: DT) -> None:
         if self.__is_abstract_class(cls):
             cls = value.__class__
             is_primary = True
             dependency = Dependency(cls, value=value, is_resolved=True, is_primary=True)
         else:
             is_primary = None
             dependency = Dependency(cls, value=value, is_resolved=True)
 
-        self.__update_parents_map(cls, is_primary)
+        self.__update_bases_map(cls, is_primary)
         self.__dependency_map[cls] = dependency
 
     def __is_abstract_class(self, cls: Type) -> bool:
         for base in cls.__bases__:
             if base in self.__ABSTRACT_BASES:
                 return True
         return False
 
-    def __update_parents_map(self, cls: Type, is_primary: Optional[bool]) -> None:
-        for base in cls.__bases__:
-            if base in self.__EXCLUDED_BASES:
+    def __update_bases_map(
+        self, cls: Type, children_is_primary: Optional[bool], reference_class: Optional[Type] = None
+    ) -> None:
+        if reference_class is None:
+            reference_class = cls
+
+        if hasattr(reference_class, "__orig_bases__"):
+            for base in reference_class.__orig_bases__:
+                self.__add_children_to_base(cls, base, children_is_primary)
+
+        for base in reference_class.__bases__:
+            if base in self.__EXCLUDED_BASES or base in self.__ABSTRACT_BASES:
                 continue
+            self.__add_children_to_base(cls, base, children_is_primary)
+            self.__update_bases_map(cls, children_is_primary, reference_class=base)
 
-            if (
-                is_primary is True
-                and base in self.__bases_map
-                and self.__get_primary_dependency_from_base_children(self.__bases_map[base])
-            ):
-                raise PrimaryDependencyAlreadyDefinedError(base)
+    def __add_children_to_base(self, cls: Type, base: Type, children_is_primary: Optional[bool]) -> None:
+        if (
+            children_is_primary is True
+            and base in self.__bases_map
+            and self.__get_primary_dependency_from_base_children(self.__bases_map[base])
+        ):
+            raise PrimaryDependencyAlreadyDefinedError(base)
 
-            self.__bases_map[base].append(cls)
+        self.__bases_map[base].append(cls)
 
     def __getitem__(self, cls: Type[DT]) -> Optional[DT]:
         dependency = self.__dependency_map.get(cls, None)
         if dependency is None and cls in self.__bases_map:
             dependency = self.__get_dependency_from_base(cls)
 
         if dependency is not None:
```

### Comparing `yandil-0.1.2/src/yandil/declarative/decorators.py` & `yandil-0.1.3/src/yandil/declarative/decorators.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/dependency.py` & `yandil-0.1.3/src/yandil/dependency.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/dependency_filler.py` & `yandil-0.1.3/src/yandil/dependency_filler.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/discovery/class_discovery.py` & `yandil-0.1.3/src/yandil/discovery/class_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/discovery/module_discovery.py` & `yandil-0.1.3/src/yandil/discovery/module_discovery.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/loaders/declarative_dependency_loader.py` & `yandil-0.1.3/src/yandil/loaders/declarative_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/loaders/self_discover_dependency_loader.py` & `yandil-0.1.3/src/yandil/loaders/self_discover_dependency_loader.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/src/yandil/typing_tools.py` & `yandil-0.1.3/src/yandil/typing_tools.py`

 * *Files identical despite different names*

### Comparing `yandil-0.1.2/PKG-INFO` & `yandil-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yandil
-Version: 0.1.2
+Version: 0.1.3
 Summary: Yet ANother Dependency Injection Library
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

