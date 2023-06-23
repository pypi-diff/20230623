# Comparing `tmp/cushy-storage-1.2.0.tar.gz` & `tmp/cushy-storage-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-tgf6cdtv/cushy-storage-1.2.0.tar", last modified: Thu Jun 22 12:27:26 2023, max compression
+gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-xxrzkse5/cushy-storage-1.2.1.tar", last modified: Thu Jun 22 13:21:31 2023, max compression
```

## Comparing `cushy-storage-1.2.0.tar` & `cushy-storage-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/cushy_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/cushy_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/cushy_storage/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/cushy_storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/cushy_storage/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/cushy_storage/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/cushy_storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/cushy_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/cushy_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/cushy_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/cushy_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/cushy_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:27:26.000000 cushy-storage-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/tests/test_base_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/tests/test_cushy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/tests/test_dict_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-22 12:27:09.000000 cushy-storage-1.2.0/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/cushy_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/cushy_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/cushy_storage/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/cushy_storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/cushy_storage/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/cushy_storage/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/cushy_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/cushy_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/cushy_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/cushy_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/cushy_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/cushy_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:21:31.000000 cushy-storage-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/tests/test_base_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/tests/test_cushy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/tests/test_dict_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-22 13:21:16.000000 cushy-storage-1.2.1/tests/test_orm.py
```

### Comparing `cushy-storage-1.2.0/LICENSE` & `cushy-storage-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/PKG-INFO` & `cushy-storage-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.2.0
+Version: 1.2.1
 Summary: A data local persistence ORM framework
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,ORM,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cushy-storage-1.2.0/README.md` & `cushy-storage-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/cushy_storage/__init__.py` & `cushy-storage-1.2.1/cushy_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/cushy_storage/_core.py` & `cushy-storage-1.2.1/cushy_storage/_core.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/cushy_storage/base.py` & `cushy-storage-1.2.1/cushy_storage/base.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/cushy_storage/logger.py` & `cushy-storage-1.2.1/cushy_storage/logger.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/cushy_storage/orm.py` & `cushy-storage-1.2.1/cushy_storage/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,21 @@
 def _get_class_name(class_name_or_obj: Union[str, type(BaseORMModel)]) -> str:
     class_name: str = class_name_or_obj
     if isinstance(class_name_or_obj, type(BaseORMModel)):
         class_name = class_name_or_obj.__name__
     return class_name
 
 
+def _get_obj_name(obj: Union[BaseORMModel, QuerySet, List[BaseORMModel]]) -> str:
+    if isinstance(obj, BaseORMModel) or isinstance(obj, QuerySet):
+        return obj.__name__
+    elif isinstance(obj, List):
+        return obj[0].__name__
+
+
 class ORMMixin(ABC):
     def _get_original_data_from_cache(
         self, class_name_or_obj: Union[str, type(BaseORMModel)]
     ) -> List[BaseORMModel]:
         class_name = _get_class_name(class_name_or_obj)
         if class_name not in self:
             self.__setitem__(class_name, [])
@@ -153,54 +160,59 @@
         original_result = self._get_original_data_from_cache(class_name_or_obj)
         if len(original_result) != 0:
             queryset = QuerySet(original_result)
             queryset = queryset.remove_duplicates()
             self.set(queryset)
 
     def add(self, obj: Union[BaseORMModel, QuerySet, List[BaseORMModel]]) -> QuerySet:
-        obj_name = obj.__name__ if not isinstance(obj, list) else obj[0].__name__
-        original_result = self._get_original_data_from_cache(obj_name)
+        obj_name = _get_obj_name(obj)
+        original_result: List[BaseORMModel] = self._get_original_data_from_cache(
+            obj_name
+        )
 
         if isinstance(obj, BaseORMModel):
             original_result.append(obj)
         elif isinstance(obj, QuerySet):
             original_result += obj.all()
         else:
             original_result += obj
 
         self[obj_name] = original_result
         return QuerySet(self[obj_name])
 
-    def delete(self, obj: Union[List[BaseORMModel], BaseORMModel]):
+    def delete(self, obj: Union[List[BaseORMModel], QuerySet, BaseORMModel]):
         """delete obj by obj.__unique_id__"""
+        obj_name = _get_obj_name(obj)
         original_result: List[BaseORMModel] = self._get_original_data_from_cache(
-            obj.__name__
+            obj_name
         )
         copy_result: List[BaseORMModel] = original_result.copy()
 
         if isinstance(obj, BaseORMModel):
             obj = [obj]
+        elif isinstance(obj, QuerySet):
+            obj = obj.all()
         if len(obj) == 0:
             return
 
         for cache_obj_item in original_result:
             for input_obj_item in obj:
                 if cache_obj_item.__unique_id__ == input_obj_item.__unique_id__:
                     copy_result.remove(cache_obj_item)
-        return self.__setitem__(obj[0].__name__, copy_result)
+        return self.__setitem__(obj_name, copy_result)
 
     def set(self, obj: Union[BaseORMModel, QuerySet, List[BaseORMModel]]):
-        if isinstance(obj, QuerySet):
-            obj = obj.all()
-        elif isinstance(obj, BaseORMModel):
+        obj_name = _get_obj_name(obj)
+        if isinstance(obj, BaseORMModel):
             obj = [obj]
-
+        elif isinstance(obj, QuerySet):
+            obj = obj.all()
         if len(obj) == 0:
             return
-        return self.__setitem__(obj[0].__name__, obj)
+        return self.__setitem__(obj_name, obj)
 
     def update_obj(self, obj: BaseORMModel):
         original_result: List[BaseORMModel] = self._get_original_data_from_cache(
             obj.__name__
         )
         copy_result: List[BaseORMModel] = original_result.copy()
```

### Comparing `cushy-storage-1.2.0/cushy_storage/utils.py` & `cushy-storage-1.2.1/cushy_storage/utils.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/cushy_storage.egg-info/PKG-INFO` & `cushy-storage-1.2.1/cushy_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.2.0
+Version: 1.2.1
 Summary: A data local persistence ORM framework
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,ORM,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cushy-storage-1.2.0/setup.py` & `cushy-storage-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="cushy-storage",
-    version="1.2.0",
+    version="1.2.1",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A data local persistence ORM framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/cushy-storage",
     packages=setuptools.find_packages(),
```

### Comparing `cushy-storage-1.2.0/tests/test_base_dict.py` & `cushy-storage-1.2.1/tests/test_base_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/tests/test_cushy_dict.py` & `cushy-storage-1.2.1/tests/test_cushy_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/tests/test_dict_cache.py` & `cushy-storage-1.2.1/tests/test_dict_cache.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.2.0/tests/test_orm.py` & `cushy-storage-1.2.1/tests/test_orm.py`

 * *Files identical despite different names*

