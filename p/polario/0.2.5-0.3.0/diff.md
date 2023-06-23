# Comparing `tmp/polario-0.2.5.tar.gz` & `tmp/polario-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polario-0.2.5.tar", max compression
+gzip compressed data, was "polario-0.3.0.tar", max compression
```

## Comparing `polario-0.2.5.tar` & `polario-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-08 13:37:04.504427 polario-0.2.5/LICENSE
--rw-r--r--   0        0        0      694 2023-06-08 13:37:04.504427 polario-0.2.5/README.md
--rw-r--r--   0        0        0      106 2023-06-08 13:37:04.508427 polario-0.2.5/polario/__init__.py
--rw-r--r--   0        0        0    11649 2023-06-08 13:37:04.508427 polario-0.2.5/polario/dataset.py
--rw-r--r--   0        0        0     1644 2023-06-08 13:37:04.508427 polario-0.2.5/polario/main.py
--rw-r--r--   0        0        0        0 2023-06-08 13:37:04.508427 polario-0.2.5/polario/py.typed
--rw-r--r--   0        0        0      999 2023-06-08 13:37:23.492444 polario-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 polario-0.2.5/setup.py
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 polario-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 11:59:46.922190 polario-0.3.0/LICENSE
+-rw-r--r--   0        0        0      931 2023-06-23 11:59:46.922190 polario-0.3.0/README.md
+-rw-r--r--   0        0        0      543 2023-06-23 11:59:46.922190 polario-0.3.0/polario/__init__.py
+-rw-r--r--   0        0        0     2040 2023-06-23 11:59:46.922190 polario-0.3.0/polario/delta_dataset.py
+-rw-r--r--   0        0        0    15375 2023-06-23 11:59:46.926190 polario-0.3.0/polario/hive_dataset.py
+-rw-r--r--   0        0        0     1644 2023-06-23 11:59:46.926190 polario-0.3.0/polario/main.py
+-rw-r--r--   0        0        0        0 2023-06-23 11:59:46.926190 polario-0.3.0/polario/py.typed
+-rw-r--r--   0        0        0     1036 2023-06-23 12:00:08.546168 polario-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 polario-0.3.0/setup.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 polario-0.3.0/PKG-INFO
```

### Comparing `polario-0.2.5/LICENSE` & `polario-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polario-0.2.5/README.md` & `polario-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,7 +24,14 @@
 
 ds.write(df)
 
 for partition_df in ds.read_partitions():
     print(partition_df)
 
 ```
+
+
+To model data storage, we use three layers: dataset, partition, fragment.
+
+Each dataset is a lexical ordered set of partitions
+Each partition is a lexical ordered set of fragments
+Each fragment is a file on disk with rows in any order
```

### Comparing `polario-0.2.5/polario/main.py` & `polario-0.3.0/polario/main.py`

 * *Files identical despite different names*

### Comparing `polario-0.2.5/pyproject.toml` & `polario-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "polario"
-version = "0.2.5"
+version = "0.3.0"
 description = "Polars IO"
 authors = ["Bram Neijt <bram@neijt.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://bneijt.github.io/polario/"
 repository = "https://github.com/bneijt/polario"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-polars = ">=0.16.8"
-fsspec = "^2023.1.0"
-pyarrow = ">=11.0.0"
-
+polars = { extras = ["fsspec"], version = ">=0.16" }
+fsspec = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "^23.1.0", allow-prereleases = true }
 mypy = "^1.0.1"
 pytest = "^7.2.1"
 pdoc = "^13.0.0"
 twine = "^4.0.2"
 isort = "^5.12.0"
 pre-commit = "^3.1.0"
 ruff = "^0.0.259"
+deltalake = "^0.10.0"
+s3fs = "^2023.6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 polario = 'polario.main:main'
@@ -41,8 +41,8 @@
 
 [tool.mypy]
 files = "polario,tests"
 ignore_missing_imports = true
 show_error_codes = true
 
 [tool.ruff]
-extend-ignore = ["E501"]
+ignore = ["E501"]
```

### Comparing `polario-0.2.5/setup.py` & `polario-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['polario']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fsspec>=2023.1.0,<2024.0.0', 'polars>=0.16.8', 'pyarrow>=11.0.0']
+['fsspec', 'polars[fsspec]>=0.16']
 
 entry_points = \
 {'console_scripts': ['polario = polario.main:main']}
 
 setup_kwargs = {
     'name': 'polario',
-    'version': '0.2.5',
+    'version': '0.3.0',
     'description': 'Polars IO',
-    'long_description': 'Polars IO utility library\n=================\n\nHelpers to make it easier to read and write Hive partitioned parquet dataset with Polars.\n\nIt is meant to be a library to deal with datasets easily, but also contains a commandline interface\nwhich allows you to inspect parquet files and datasets more easily.\n\nDataset\n=======\nExample of use of `polario.dataset.HiveDataset`\n```python\n\nfrom polario.dataset import HiveDataset\nimport polars as pl\ndf = pl.from_dicts(\n        [\n            {"p1": 1, "v": 1},\n            {"p1": 2, "v": 1},\n        ]\n    )\n\nds = HiveDataset("file:///tmp/", partition_columns=["p1"])\n\nds.write(df)\n\nfor partition_df in ds.read_partitions():\n    print(partition_df)\n\n```\n',
+    'long_description': 'Polars IO utility library\n=================\n\nHelpers to make it easier to read and write Hive partitioned parquet dataset with Polars.\n\nIt is meant to be a library to deal with datasets easily, but also contains a commandline interface\nwhich allows you to inspect parquet files and datasets more easily.\n\nDataset\n=======\nExample of use of `polario.dataset.HiveDataset`\n```python\n\nfrom polario.dataset import HiveDataset\nimport polars as pl\ndf = pl.from_dicts(\n        [\n            {"p1": 1, "v": 1},\n            {"p1": 2, "v": 1},\n        ]\n    )\n\nds = HiveDataset("file:///tmp/", partition_columns=["p1"])\n\nds.write(df)\n\nfor partition_df in ds.read_partitions():\n    print(partition_df)\n\n```\n\n\nTo model data storage, we use three layers: dataset, partition, fragment.\n\nEach dataset is a lexical ordered set of partitions\nEach partition is a lexical ordered set of fragments\nEach fragment is a file on disk with rows in any order\n',
     'author': 'Bram Neijt',
     'author_email': 'bram@neijt.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bneijt.github.io/polario/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `polario-0.2.5/PKG-INFO` & `polario-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: polario
-Version: 0.2.5
+Version: 0.3.0
 Summary: Polars IO
 Home-page: https://bneijt.github.io/polario/
 License: Apache-2.0
 Author: Bram Neijt
 Author-email: bram@neijt.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
-Requires-Dist: polars (>=0.16.8)
-Requires-Dist: pyarrow (>=11.0.0)
+Requires-Dist: fsspec
+Requires-Dist: polars[fsspec] (>=0.16)
 Project-URL: Repository, https://github.com/bneijt/polario
 Description-Content-Type: text/markdown
 
 Polars IO utility library
 =================
 
 Helpers to make it easier to read and write Hive partitioned parquet dataset with Polars.
@@ -46,7 +45,14 @@
 ds.write(df)
 
 for partition_df in ds.read_partitions():
     print(partition_df)
 
 ```
 
+
+To model data storage, we use three layers: dataset, partition, fragment.
+
+Each dataset is a lexical ordered set of partitions
+Each partition is a lexical ordered set of fragments
+Each fragment is a file on disk with rows in any order
+
```

