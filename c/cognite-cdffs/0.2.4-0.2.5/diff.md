# Comparing `tmp/cognite_cdffs-0.2.4.tar.gz` & `tmp/cognite_cdffs-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_cdffs-0.2.4.tar", max compression
+gzip compressed data, was "cognite_cdffs-0.2.5.tar", max compression
```

## Comparing `cognite_cdffs-0.2.4.tar` & `cognite_cdffs-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2423 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/README.md
--rw-r--r--   0        0        0      205 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/__init__.py
--rw-r--r--   0        0        0     3907 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/credentials.py
--rw-r--r--   0        0        0     3134 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/file_handler.py
--rw-r--r--   0        0        0    28003 2023-06-13 10:14:31.995284 cognite_cdffs-0.2.4/cognite/cdffs/spec.py
--rw-r--r--   0        0        0     1663 2023-06-13 10:14:31.999285 cognite_cdffs-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.4/setup.py
--rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2423 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/README.md
+-rw-r--r--   0        0        0      205 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/__init__.py
+-rw-r--r--   0        0        0     3907 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/credentials.py
+-rw-r--r--   0        0        0     3134 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/file_handler.py
+-rw-r--r--   0        0        0    30135 2023-06-23 07:26:50.271973 cognite_cdffs-0.2.5/cognite/cdffs/spec.py
+-rw-r--r--   0        0        0     1663 2023-06-23 07:26:50.275973 cognite_cdffs-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.5/setup.py
+-rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 cognite_cdffs-0.2.5/PKG-INFO
```

### Comparing `cognite_cdffs-0.2.4/README.md` & `cognite_cdffs-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.4/cognite/cdffs/credentials.py` & `cognite_cdffs-0.2.5/cognite/cdffs/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.4/cognite/cdffs/file_handler.py` & `cognite_cdffs-0.2.5/cognite/cdffs/file_handler.py`

 * *Files identical despite different names*

### Comparing `cognite_cdffs-0.2.4/cognite/cdffs/spec.py` & `cognite_cdffs-0.2.5/cognite/cdffs/spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,15 +196,38 @@
         for dir_name, dir_val in directories.items():
             parent_path = str(Path(dir_name).parent)
             if parent_path not in self.dircache:
                 self.dircache[parent_path] = [dir_val]
             else:
                 self.dircache[parent_path].append(dir_val)
 
-    def _ls(self, root_dir: str, external_id_prefix: str) -> None:
+    def _invalidate_dircache(self, inp_path: str) -> None:
+        # Comments about why we need to invalidate the cache.
+        # Invalidating a cache will allow the subsequent requests to hit cdf to get the list of files instead of serving
+        # them from cache as user may use different limit values for each request.
+        # Caching the results with limit will lead to produce incorrect file list to the user.
+        # Possible scenarios.
+        #    Scenario #1
+        #       User may call `ls` method with no limits at first. We will cache the results.
+        #       User may call `ls` method with no limits at first. Results will be returned from the cache.
+        #    Scenario #2
+        #       User may call `ls` method with no limits at first. We will cache the results.
+        #       User may call `ls` method with limit. Cdf will be queried to get the results.
+        #           Cache will be invalidated at this point. Any subsequent queries will hit cdf.
+        #    Scenario #3
+        #       User may call `ls` method with limit at first. We don't cache the results.
+        #           Cache will be invalidated at this point. Any subsequent queries will hit cdf.
+        #       User may call `ls` method with limit. Cdf will still be queried to get the results.
+        #           Cache will be invalidated at this point. Any subsequent queries will hit cdf.
+        #       User may call `ls` method with no limits. We will cache the results.
+        #           Any subsequent queries will be served from cache.
+        if inp_path in self.dircache:
+            del self.dircache[inp_path]
+
+    def _ls(self, root_dir: str, external_id_prefix: str, limit: int = -1) -> None:
         """List the files based on the directory & external Id prefixes extracted from path.
 
         Args:
             root_dir (str): Root directory for the file.
             external_id (str): External Id for the file.
 
         Raises:
@@ -219,15 +242,15 @@
             if root_dir not in ("/", ""):
                 list_query["directory_prefix"] = root_dir
             if external_id_prefix != "":
                 list_query["external_id_prefix"] = external_id_prefix
 
             # Get all the files that were previously cached when writing. (if applicable)
             _file_write_cache = {d_info["name"]: True for d_path in self.dircache for d_info in self.dircache[d_path]}
-            for file_met in self.cognite_client.files.list(**list_query, limit=-1):
+            for file_met in self.cognite_client.files.list(**list_query, limit=limit):
                 if not file_met.external_id:
                     # Files are expected to have a valid external id.
                     continue
                 inp_path = Path(file_met.directory if file_met.directory else "/", file_met.external_id)
                 file_name = str(inp_path).lstrip("/")
                 file_size = int(file_met.metadata.get("size", -1)) if file_met.metadata else -1
                 file_meta = {"type": "file", "name": file_name, "size": file_size}
@@ -262,38 +285,51 @@
         Returns:
             List: Returns the list of files/directories that match the path given.
 
         Raises:
             FileNotFoundError: When there are no files matching the path given.
         """
         root_dir, external_id_prefix, _ = self.split_path(path, validate_suffix=False)
+
+        # Invalidating cache when limit is used.
+        if (limit := kwargs.get("limit", -1)) != -1:
+            self._invalidate_dircache(root_dir.strip("/"))
+            self._invalidate_dircache(path.strip("/"))
+
         inp_key = str(Path(root_dir, external_id_prefix)).lstrip("/")
-        if not (
+        if limit != -1 or not (
             inp_key in self.dircache
             and inp_key in self.cdf_list_cache
             and time.time() - self.cdf_list_cache[inp_key] < self.cdf_list_expiry_time
         ):
-            self._ls(root_dir, external_id_prefix)
+            self._ls(root_dir, external_id_prefix, limit=limit)  # type: ignore
 
         inp_path = path.strip("/")
         file_list = self.dircache.get(inp_path, [])
         if not file_list:
             # It is possible that the requested path is absolute.
             file_list = [x for x in self.dircache.get(root_dir.strip("/"), []) if x["name"] == inp_path]
+
             if file_list:
                 return file_list if detail else [x["name"] for x in file_list]
 
             raise FileNotFoundError
 
         if inp_path not in self.dircache:
             self.dircache[inp_path] = [{"type": "directory", "name": inp_path}]
         elif not [x for x in self.dircache[inp_path] if x["name"] == inp_path]:
             self.dircache[inp_path].append({"type": "directory", "name": inp_path})
 
-        return self.dircache[inp_path] if detail else [x["name"] for x in self.dircache[inp_path]]
+        out_list = self.dircache[inp_path] if detail else [x["name"] for x in self.dircache[inp_path]]
+
+        # Invalidate the cache if limit is used when listing files. Same remarks as above.
+        if limit != -1 and inp_path in self.dircache:
+            del self.dircache[inp_path]
+
+        return out_list
 
     def makedirs(self, path: str, exist_ok: bool = True) -> None:
         """Create a directory at a path given.
 
         Args:
             path (str): Path to use to create a directory.
             exist_ok (bool): Flag to specify if error can be ignored when directory already exists.
```

### Comparing `cognite_cdffs-0.2.4/pyproject.toml` & `cognite_cdffs-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-cdffs"
-version = "0.2.4"
+version = "0.2.5"
 description = "File System Interface for CDF Files"
 license = "Apache-2.0"
 authors = ["Infant Alex <infant.alex@cognite.com>"]
 readme = "README.md"
 packages = [
     { include="cognite", from="." },
 ]
```

### Comparing `cognite_cdffs-0.2.4/setup.py` & `cognite_cdffs-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pydantic>=1.10.9,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'requests>=2.31.0,<3.0.0',
  'twine>=4.0.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'cognite-cdffs',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'File System Interface for CDF Files',
     'long_description': '<a href="https://cognite.com/">\n  <img alt="Cognite" src="https://raw.githubusercontent.com/cognitedata/cognite-python-docs/master/img/cognite_logo_black.png" alt="Cognite logo" title="Cognite" align="right" height="80">\n</a>\n\n[![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/badge.svg)](https://codecov.io/gh/cognitedata/cdffs)\n![PyPI](https://img.shields.io/pypi/v/cognite-cdffs)\n\n# cdffs\n\nA file system interface (`cdffs`) to allow users to work with CDF Files using the [fsspec](https://filesystem-spec.readthedocs.io/en/latest/) supported/compatible python packages (`pandas`, `xarray` etc).\n\n`fsspec` provides an abstract file system interface to work with local/cloud storages and based on the protocol name (example, `s3` or `abfs`) provided in the path, `fsspec` translates the incoming requests to storage specific implementations and send the responses back to the upstream package to work with the desired data.\n\nRefer [fsspec documentation](https://filesystem-spec.readthedocs.io/en/latest/#who-uses-fsspec) to get the list of all supported/compatible python packages.\n\n## Installation\n\n`cdffs` is available on PyPI. Install using,\n\n```shell\npip install cognite-cdffs\n```\n\n## Usage\n\nImportant steps to follow when working with CDF Files using the `fsspec` supported python packages.\n\n1) Import `cdffs` package\n```python\n  from cognite import cdffs  # noqa\n```\n\n2) Follow instructions from [Authentication](https://cdffs.readthedocs.io/en/latest/authentication.html) to authenticate.\n\n3) Read/write the files from/to CDF using `fsspec` supported packages. Example,\n\n    * Read `zarr` files using using `xarray`.\n\n    ```python\n    ds = xarray.open_zarr("cdffs://sample_data/test.zarr")\n    ```\n    * Write `zarr` files using `xarray`.\n\n    ```python\n    ds.to_zarr("cdffs://sample_data/test.zarr", storage_options={"file_metadata": metadata})\n    ```\n\nRefer [cdffs.readthedocs.io](https://cdffs.readthedocs.io) for more details.\n\n## Contributing\nWant to contribute? Check out [CONTRIBUTING](CONTRIBUTING.md).\n',
     'author': 'Infant Alex',
     'author_email': 'infant.alex@cognite.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': '.'}
 packages = \ ['cognite', 'cognite.cdffs'] package_data = \ {'': ['*']}
 install_requires = \ ['cognite-sdk>=6.4.0,<7.0.0',
 'fsspec>=2023.6.0,<2024.0.0', 'pydantic>=1.10.9,<2.0.0', 'python-
 dotenv>=1.0.0,<2.0.0', 'requests>=2.31.0,<3.0.0', 'twine>=4.0.2,<5.0.0']
-setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.4', 'description':
+setup_kwargs = { 'name': 'cognite-cdffs', 'version': '0.2.5', 'description':
 'File System Interface for CDF Files', 'long_description': '\n_[Cognite]\n\n\n
 [![GitHub](https://img.shields.io/github/license/cognitedata/cdffs)](https://
 github.com/cognitedata/cdffs/blob/main/LICENSE)\n[![Documentation Status]
 (https://readthedocs.org/projects/cdffs/badge/?version=latest)](https://
 cdffs.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black)\n[![codecov](https://codecov.io/gh/cognitedata/cdffs/branch/main/graph/
```

### Comparing `cognite_cdffs-0.2.4/PKG-INFO` & `cognite_cdffs-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-cdffs
-Version: 0.2.4
+Version: 0.2.5
 Summary: File System Interface for CDF Files
 License: Apache-2.0
 Author: Infant Alex
 Author-email: infant.alex@cognite.com
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.4 Summary: File System
+Metadata-Version: 2.1 Name: cognite-cdffs Version: 0.2.5 Summary: File System
 Interface for CDF Files License: Apache-2.0 Author: Infant Alex Author-email:
 infant.alex@cognite.com Requires-Python: >=3.9.10,<4.0.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: cognite-sdk
 (>=6.4.0,<7.0.0) Requires-Dist: fsspec (>=2023.6.0,<2024.0.0) Requires-Dist:
 pydantic (>=1.10.9,<2.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

