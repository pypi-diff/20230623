# Comparing `tmp/padawan-0.7.tar.gz` & `tmp/padawan-0.8.tar.gz`

## Comparing `padawan-0.7.tar` & `padawan-0.8.tar`

### file list

```diff
@@ -1,45 +1,43 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.7/.readthedocs.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/README.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.7/docs/Makefile
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 padawan-0.7/docs/api.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.7/docs/conf.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.7/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.7/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.7/docs/requirements.txt
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/__init__.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/collated_dataset.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/concatenated_dataset.py
--rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/dataset.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/in_memory_dataset.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/joined_dataset.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/json_io.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/mapped_dataset.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/metadata.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/ordering.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/parallelize.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/persisted_dataset.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/reindexed_dataset.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/renamed_dataset.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/repartitioned_dataset.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/sliced_dataset.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 padawan-0.7/tests/fixtures.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_collate.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_concat.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_from_polars.py
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_io.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_join.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_map.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_rename.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_repartition.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_slice.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.7/tests/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.7/.gitignore
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.7/LICENSE
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.7/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 padawan-0.7/pyproject.toml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 padawan-0.7/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.8/.readthedocs.yml
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 padawan-0.8/data/sample.parquet/part0.parquet
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 padawan-0.8/data/sample.parquet/part24.parquet
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 padawan-0.8/data/sample.parquet/part48.parquet
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 padawan-0.8/data/sample.parquet/part72.parquet
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.8/docs/Makefile
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 padawan-0.8/docs/api.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.8/docs/conf.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.8/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.8/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.8/docs/requirements.txt
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/__init__.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/collated_dataset.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/concatenated_dataset.py
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/dataset.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/in_memory_dataset.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/joined_dataset.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/json_io.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/mapped_dataset.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/metadata.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/ordering.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/parallelize.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/persisted_dataset.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/reindexed_dataset.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/renamed_dataset.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/repartitioned_dataset.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.8/src/padawan/sliced_dataset.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 padawan-0.8/tests/fixtures.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_collate.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_concat.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_from_polars.py
+-rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_io.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_join.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_map.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_rename.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_repartition.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.8/tests/test_slice.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.8/tests/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.8/.gitignore
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.8/LICENSE
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.8/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 padawan-0.8/pyproject.toml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 padawan-0.8/PKG-INFO
```

### Comparing `padawan-0.7/docs/Makefile` & `padawan-0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `padawan-0.7/docs/conf.py` & `padawan-0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/docs/index.rst` & `padawan-0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `padawan-0.7/docs/make.bat` & `padawan-0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/__init__.py` & `padawan-0.8/src/padawan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7'
+__version__ = '0.8'
 
 __all__ = [
     'scan_parquet',
     'from_polars',
     'concat',
 ]
```

### Comparing `padawan-0.7/src/padawan/collated_dataset.py` & `padawan-0.8/src/padawan/collated_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/concatenated_dataset.py` & `padawan-0.8/src/padawan/concatenated_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/dataset.py` & `padawan-0.8/src/padawan/dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/in_memory_dataset.py` & `padawan-0.8/src/padawan/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/joined_dataset.py` & `padawan-0.8/src/padawan/joined_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,21 +29,32 @@
 
         self._left = left
         self._right = right
 
         divisions = left.lower_bounds + right.lower_bounds
         divisions = sorted(set(divisions), key=lex_key)
 
+        schema = None
+        if left.known_schema and right.known_schema:
+            index_columns = left.index_columns
+            schema = left.schema
+            for c, t in right.schema.items():
+                if c in index_columns:
+                    continue
+                if c in schema:
+                    raise ValueError(f'Duplicate column {repr(c)} in join.')
+                schema[c] = t
+
         super().__init__(
             npartitions=len(divisions) + 1,
             index_columns=left.index_columns,
             sizes=None,
             lower_bounds=None,
             upper_bounds=None,
-            schema=None,
+            schema=schema,
         )
         self._divisions = [None] + divisions + [None]
         self._how = how
 
     def _get_partition(self, partition_index):
         lb = self._divisions[partition_index]
         ub = self._divisions[partition_index + 1]
```

### Comparing `padawan-0.7/src/padawan/json_io.py` & `padawan-0.8/src/padawan/json_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/mapped_dataset.py` & `padawan-0.8/src/padawan/mapped_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     def __init__(
             self,
             other,
             func,
             extra_args=None,
             shared_args=None,
             index_columns=None,
+            schema=None,
             preserves='none',
     ):
         if not isinstance(other, Dataset):
             raise ValueError('other must be an instance of padawan.Dataset')
         self._other = other
         self._func = func
 
@@ -50,15 +51,15 @@
 
         super().__init__(
             npartitions=len(other),
             index_columns=index_columns,
             sizes=sizes,
             lower_bounds=lower_bounds,
             upper_bounds=upper_bounds,
-            schema=None,
+            schema=schema,
         )
 
     def _get_partition(self, partition_index):
         if self._extra_args is None:
             return self._func(
                 self._other[partition_index],
                 *self._shared_args).lazy()
@@ -70,14 +71,15 @@
 
 def _map(
         self,
         func,
         extra_args=None,
         shared_args=None,
         index_columns=None,
+        schema=None,
         preserves='none',
 ):
     """Apply a function to all partitions.
 
     Args:
       func (callable): The function to apply. It should return a
         ``polars.DataFrame`` or ``polars.LazyFrame`` and support the following
@@ -101,14 +103,16 @@
         extra arguments to *every* call of `func`. Defaults to ``None``, in
         which case no shared arguments are passed.
       index_columns (tuple of str, optional): The new index columns to use
         after `func` is applied. (Note that `func` may change the schema of the
         dataset, so the old index columns might not exist anymore after `func`
         is applied.) Defaults to ``None``, in which case the old index columns
         are used.
+      schema (dict, optional): The schema of the dataset after the map. Defaults
+        to ``None``, in which case the schema will be unknown.
       preserves (str, optional): Specifies which part of the metadata is
         preserved by `func`. Possible values are:
 
           ``'none'``
             No metadata is preserved.
           ``'sizes'``
             Partition sizes (number of rows) are preserved.
@@ -129,11 +133,12 @@
     """
     return MappedDataset(
         self,
         func,
         extra_args=extra_args,
         shared_args=shared_args,
         index_columns=index_columns,
+        schema=schema,
         preserves=preserves,
     )
 Dataset.map = _map
```

### Comparing `padawan-0.7/src/padawan/metadata.py` & `padawan-0.8/src/padawan/metadata.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/ordering.py` & `padawan-0.8/src/padawan/ordering.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/parallelize.py` & `padawan-0.8/src/padawan/parallelize.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/persisted_dataset.py` & `padawan-0.8/src/padawan/persisted_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/reindexed_dataset.py` & `padawan-0.8/src/padawan/reindexed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/renamed_dataset.py` & `padawan-0.8/src/padawan/renamed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/repartitioned_dataset.py` & `padawan-0.8/src/padawan/repartitioned_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/src/padawan/sliced_dataset.py` & `padawan-0.8/src/padawan/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/fixtures.py` & `padawan-0.8/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_collate.py` & `padawan-0.8/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_concat.py` & `padawan-0.8/tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_from_polars.py` & `padawan-0.8/tests/test_from_polars.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_io.py` & `padawan-0.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_join.py` & `padawan-0.8/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_map.py` & `padawan-0.8/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_rename.py` & `padawan-0.8/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_repartition.py` & `padawan-0.8/tests/test_repartition.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/tests/test_slice.py` & `padawan-0.8/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `padawan-0.7/LICENSE` & `padawan-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `padawan-0.7/README.md` & `padawan-0.8/README.md`

 * *Files identical despite different names*

### Comparing `padawan-0.7/pyproject.toml` & `padawan-0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "padawan"
-version = "0.7"
+version = "0.8"
 authors = [
   { name="Martin Wiebusch" },
 ]
 description = "Wrangle partitioned data with polars."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `padawan-0.7/PKG-INFO` & `padawan-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: padawan
-Version: 0.7
+Version: 0.8
 Summary: Wrangle partitioned data with polars.
 Project-URL: Homepage, https://github.com/mwiebusch78/padawan
 Project-URL: Bug Tracker, https://github.com/mwiebusch78/padawan/issues
 Project-URL: Documentation, https://padawan.readthedocs.io/en/latest/
 Author: Martin Wiebusch
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

