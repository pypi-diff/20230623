# Comparing `tmp/access_nri_intake-0.0.7.tar.gz` & `tmp/access_nri_intake-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.7.tar", last modified: Thu Jun 15 00:02:09 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.8.tar", last modified: Thu Jun 22 23:45:59 2023, max compression
```

## Comparing `access_nri_intake-0.0.7.tar` & `access_nri_intake-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.086476 access_nri_intake-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/catalog/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/catalog/translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/data/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/data/catalog.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/src/access_nri_intake/source/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/source/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/source/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.090477 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 00:02:09.000000 access_nri_intake-0.0.7/src/access_nri_intake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:02:09.094477 access_nri_intake-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/tests/test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-06-15 00:01:52.000000 access_nri_intake-0.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.174280 access_nri_intake-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/src/access_nri_intake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/src/access_nri_intake/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/catalog/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/catalog/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/src/access_nri_intake/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/data/catalog.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/src/access_nri_intake/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/source/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/source/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-22 23:45:59.000000 access_nri_intake-0.0.8/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-22 23:45:59.000000 access_nri_intake-0.0.8/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:45:59.000000 access_nri_intake-0.0.8/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 23:45:59.000000 access_nri_intake-0.0.8/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-22 23:45:59.000000 access_nri_intake-0.0.8/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 23:45:59.000000 access_nri_intake-0.0.8/src/access_nri_intake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:45:59.178280 access_nri_intake-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/tests/test_builder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-06-22 23:45:41.000000 access_nri_intake-0.0.8/versioneer.py
```

### Comparing `access_nri_intake-0.0.7/LICENSE` & `access_nri_intake-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.7/PKG-INFO` & `access_nri_intake-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.0.7
+Version: 0.0.8
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,16 @@
 ACCESS-NRI Intake Catalog
 =========================
 
 **Tools and configuration info used to manage ACCESS-NRI's intake catalog**
 
 Note, this project is under development. Things might change/break frequently and without warning.
 
+Read the `documentation here <https://access-nri-intake-catalog.readthedocs.io/en/latest/index.html>`_. 
+
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
```

### Comparing `access_nri_intake-0.0.7/README.rst` & `access_nri_intake-0.0.8/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 ACCESS-NRI Intake Catalog
 =========================
 
 **Tools and configuration info used to manage ACCESS-NRI's intake catalog**
 
 Note, this project is under development. Things might change/break frequently and without warning.
 
+Read the `documentation here <https://access-nri-intake-catalog.readthedocs.io/en/latest/index.html>`_. 
+
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
```

### Comparing `access_nri_intake-0.0.7/pyproject.toml` & `access_nri_intake-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/catalog/__init__.py` & `access_nri_intake-0.0.8/src/access_nri_intake/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/catalog/manager.py` & `access_nri_intake-0.0.8/src/access_nri_intake/catalog/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/catalog/translators.py` & `access_nri_intake-0.0.8/src/access_nri_intake/catalog/translators.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/cli.py` & `access_nri_intake-0.0.8/src/access_nri_intake/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import argparse
 import logging
 import os
 
 import jsonschema
 import yaml
+from intake import open_esm_datastore
 
 from . import __version__
 from .catalog import EXP_JSONSCHEMA, translators
 from .catalog.manager import CatalogManager
 from .source import builders
 from .utils import load_metadata_yaml, validate_against_schema
 
@@ -156,39 +157,47 @@
     metacatalog_path = os.path.join(build_base_path, version, catalog_file)
     os.makedirs(build_path, exist_ok=True)
 
     # Parse inputs to pass to CatalogManager
     parsed_sources = _parse_inputs(config_yamls, build_path)
     _check_args([parsed_source[1] for parsed_source in parsed_sources])
 
+    # Get the project storage flags
+    def _get_project(path):
+        return os.path.normpath(path).split(os.sep)[3]
+
+    project = set()
+    for method, args in parsed_sources:
+        if method == "load":
+            # This is a hack but I don't know how else to get the storage from pre-built datastores
+            esm_ds = open_esm_datastore(args["path"][0])
+            project |= set(esm_ds.df["path"].map(_get_project))
+
+        project |= {_get_project(path) for path in args["path"]}
+    storage_flags = "+".join(sorted([f"gdata/{proj}" for proj in project]))
+
     # Build the catalog
-    for (method, args) in parsed_sources:
+    for method, args in parsed_sources:
         man = CatalogManager(path=metacatalog_path)
         logger.info(f"Adding '{args['name']}' to metacatalog '{metacatalog_path}'")
         getattr(man, method)(**args).add()
 
     # Write catalog yaml file
-    storage = set()
-    for (_, args) in parsed_sources:
-        storage |= {
-            f"gdata/{os.path.normpath(path).split(os.sep)[3]}" for path in args["path"]
-        }
-
     cat = man.dfcat
     cat.name = "access_nri"
     cat.description = "ACCESS-NRI intake catalog"
     yaml_dict = yaml.safe_load(cat.yaml())
 
     yaml_dict["sources"]["access_nri"]["args"]["path"] = os.path.join(
         build_base_path, "{{version}}", catalog_file
     )
     yaml_dict["sources"]["access_nri"]["args"]["mode"] = "r"
     yaml_dict["sources"]["access_nri"]["metadata"] = {
         "version": "{{version}}",
-        "storage": "+".join(list(storage)),
+        "storage": storage_flags,
     }
     yaml_dict["sources"]["access_nri"]["parameters"] = {
         "version": {"description": "Catalog version", "type": "str", "default": version}
     }
 
     _here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(_here, "data", "catalog.yaml"), "w") as fobj:
```

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/data/catalog.yaml` & `access_nri_intake-0.0.8/src/access_nri_intake/data/catalog.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,14 @@
       mode: r
       name_column: name
       path: /g/data/xp65/public/apps/access-nri-intake-catalog/{{version}}/metacatalog.csv
       yaml_column: yaml
     description: ACCESS-NRI intake catalog
     driver: intake_dataframe_catalog.core.DfFileCatalog
     metadata:
-      storage: gdata/cj50+gdata/p73+gdata/ik11+gdata/dk92
+      storage: gdata/al33+gdata/cj50+gdata/dk92+gdata/fs38+gdata/ik11+gdata/oi10+gdata/p73+gdata/rr3
       version: '{{version}}'
     parameters:
       version:
-        default: v0.0.7
+        default: v0.0.8
         description: Catalog version
         type: str
```

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/source/__init__.py` & `access_nri_intake-0.0.8/src/access_nri_intake/source/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/source/builders.py` & `access_nri_intake-0.0.8/src/access_nri_intake/source/builders.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """ Builders for generating Intake-ESM datastores """
 
 import multiprocessing
 import re
 import traceback
-from pathlib import Path
 
-import xarray as xr
 from ecgtools.builder import INVALID_ASSET, TRACEBACK, Builder
 
 from ..utils import validate_against_schema
 from . import ESM_JSONSCHEMA, PATH_COLUMN, VARIABLE_COLUMN
-from .utils import get_timeinfo, redact_time_stamps
+from .utils import parse_access_ncfile
 
 
 class ParserError(Exception):
     pass
 
 
 class BaseBuilder(Builder):
@@ -229,41 +227,26 @@
             # configuration = match_groups[0]
             # exp_id = match_groups[1]
             realm = match_groups[2]
 
             if realm == "ice":
                 realm = "seaIce"
 
-            filename = Path(file).stem
-
-            # Get file id from filename without any time stamps
-            file_id = redact_time_stamps(filename)
-
-            with xr.open_dataset(
-                file,
-                chunks={},
-                decode_cf=False,
-                decode_times=False,
-                decode_coords=False,
-            ) as ds:
-                variable_list = []
-                variable_long_name_list = []
-                variable_standard_name_list = []
-                variable_cell_methods_list = []
-                for var in ds.data_vars:
-                    attrs = ds[var].attrs
-                    if "long_name" in attrs:
-                        variable_list.append(var)
-                        variable_long_name_list.append(attrs["long_name"])
-                    if "standard_name" in attrs:
-                        variable_standard_name_list.append(attrs["standard_name"])
-                    if "cell_methods" in attrs:
-                        variable_cell_methods_list.append(attrs["cell_methods"])
-
-                start_date, end_date, frequency = get_timeinfo(ds)
+            (
+                filename,
+                file_id,
+                _,
+                frequency,
+                start_date,
+                end_date,
+                variable_list,
+                variable_long_name_list,
+                variable_standard_name_list,
+                variable_cell_methods_list,
+            ) = parse_access_ncfile(file)
 
             info = {
                 "path": str(file),
                 "realm": realm,
                 "variable": variable_list,
                 "frequency": frequency,
                 "start_date": start_date,
@@ -332,42 +315,29 @@
             match_groups = re.match(r".*/([^/]*)/history/([^/]*)/.*\.nc", file).groups()
             exp_id = match_groups[0]
             realm = match_groups[1]
 
             realm_mapping = {"atm": "atmos", "ocn": "ocean", "ice": "seaIce"}
             realm = realm_mapping[realm]
 
-            filename = Path(file).stem
-
-            # Get file id from filename without any time stamps or exp_id
-            file_id = re.sub(exp_id, "", filename)
-            file_id = redact_time_stamps(file_id)
-
-            with xr.open_dataset(
-                file,
-                chunks={},
-                decode_cf=False,
-                decode_times=False,
-                decode_coords=False,
-            ) as ds:
-                variable_list = []
-                variable_long_name_list = []
-                variable_standard_name_list = []
-                variable_cell_methods_list = []
-                for var in ds.data_vars:
-                    attrs = ds[var].attrs
-                    if "long_name" in attrs:
-                        variable_list.append(var)
-                        variable_long_name_list.append(attrs["long_name"])
-                    if "standard_name" in attrs:
-                        variable_standard_name_list.append(attrs["standard_name"])
-                    if "cell_methods" in attrs:
-                        variable_cell_methods_list.append(attrs["cell_methods"])
+            (
+                filename,
+                file_id,
+                _,
+                frequency,
+                start_date,
+                end_date,
+                variable_list,
+                variable_long_name_list,
+                variable_standard_name_list,
+                variable_cell_methods_list,
+            ) = parse_access_ncfile(file)
 
-                start_date, end_date, frequency = get_timeinfo(ds)
+            # Remove exp_id from file id so that members can be part of the same dataset
+            file_id = re.sub(exp_id, "", file_id).strip("_")
 
             info = {
                 "path": str(file),
                 "realm": realm,
                 "variable": variable_list,
                 "frequency": frequency,
                 "start_date": start_date,
```

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.8/src/access_nri_intake/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.0.8/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-nri-intake
-Version: 0.0.7
+Version: 0.0.8
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,16 @@
 ACCESS-NRI Intake Catalog
 =========================
 
 **Tools and configuration info used to manage ACCESS-NRI's intake catalog**
 
 Note, this project is under development. Things might change/break frequently and without warning.
 
+Read the `documentation here <https://access-nri-intake-catalog.readthedocs.io/en/latest/index.html>`_. 
+
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
```

### Comparing `access_nri_intake-0.0.7/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.8/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 src/access_nri_intake/catalog/manager.py
 src/access_nri_intake/catalog/translators.py
 src/access_nri_intake/data/__init__.py
 src/access_nri_intake/data/catalog.yaml
 src/access_nri_intake/source/__init__.py
 src/access_nri_intake/source/builders.py
 src/access_nri_intake/source/utils.py
-tests/test_builders.py
+tests/test_builder_utils.py
```

### Comparing `access_nri_intake-0.0.7/tests/test_builders.py` & `access_nri_intake-0.0.8/tests/test_builder_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 import pytest
 
-from access_nri_intake.source.utils import redact_time_stamps
+from access_nri_intake.source.utils import parse_access_filename
 
 
 @pytest.mark.parametrize(
     "filename, expected",
     [
         # Example ACCESS-CM2 filenames
-        ("bz687a.pm107912_mon", "bz687a_pmXXXXXX_mon"),
-        ("bz687a.p7107912_mon", "bz687a_p7XXXXXX_mon"),
-        ("iceh_m.2014-06", "iceh_m_XXXX_XX"),
-        ("iceh.1917-05-daily", "iceh_XXXX_XX_daily"),
-        ("ocean_bgc_ann", "ocean_bgc_ann"),
-        ("ocean_daily", "ocean_daily"),
+        ("bz687a.pm107912_mon", ("bz687a_pmXXXXXX_mon", "107912", "1mon")),
+        ("bz687a.p7107912_mon", ("bz687a_p7XXXXXX_mon", "107912", "1mon")),
+        ("bz687a.p7107912_dai", ("bz687a_p7XXXXXX_dai", "107912", "1day")),
+        ("iceh_m.2014-06", ("iceh_m_XXXX_XX", "2014-06", None)),
+        ("iceh.1917-05-daily", ("iceh_XXXX_XX_daily", "1917-05", "1day")),
+        ("ocean_bgc_ann", ("ocean_bgc_ann", None, "1yr")),
+        ("ocean_daily", ("ocean_daily", None, "1day")),
         # Example ACCESS-ESM1.5 filenames
-        ("PI-GWL-B2035.pe-109904_dai", "PI_GWL_B2035_pe_XXXXXX_dai"),
-        ("PI-GWL-B2035.pa-109904_mon", "PI_GWL_B2035_pa_XXXXXX_mon"),
-        ("PI-1pct-02.pe-011802_dai.nc_dai", "PI_1pct_02_pe_XXXXXX_dai_nc_dai"),
-        ("iceh.1917-05", "iceh_XXXX_XX"),
+        (
+            "PI-GWL-B2035.pe-109904_dai",
+            ("PI_GWL_B2035_pe_XXXXXX_dai", "109904", "1day"),
+        ),
+        (
+            "PI-GWL-B2035.pa-109904_mon",
+            ("PI_GWL_B2035_pa_XXXXXX_mon", "109904", "1mon"),
+        ),
+        (
+            "PI-1pct-02.pe-011802_dai.nc_dai",
+            ("PI_1pct_02_pe_XXXXXX_dai_nc_dai", "011802", "1day"),
+        ),
+        ("iceh.1917-05", ("iceh_XXXX_XX", "1917-05", None)),
         # Example ACCESS-OM2 filenames
-        ("iceh.057-daily", "iceh_XXX_daily"),
-        ("ocean", "ocean"),
-        ("ocean_month", "ocean_month"),
-        ("ocean_daily_3d_vhrho_nt_07", "ocean_daily_3d_vhrho_nt_XX"),
+        ("iceh.057-daily", ("iceh_XXX_daily", "057", "1day")),
+        ("ocean", ("ocean", None, None)),
+        ("ocean_month", ("ocean_month", None, "1mon")),
+        ("ocean_daily_3d_vhrho_nt_07", ("ocean_daily_3d_vhrho_nt_XX", "07", "1day")),
         (
             "oceanbgc-3d-caco3-1-yearly-mean-y_2015",
-            "oceanbgc_3d_caco3_1_yearly_mean_y_XXXX",
+            ("oceanbgc_3d_caco3_1_yearly_mean_y_XXXX", "2015", "1yr"),
         ),
         (
             "oceanbgc-2d-wdet100-1-daily-mean-y_2015",
-            "oceanbgc_2d_wdet100_1_daily_mean_y_XXXX",
+            ("oceanbgc_2d_wdet100_1_daily_mean_y_XXXX", "2015", "1day"),
         ),
         (
             "ocean-3d-v-1-monthly-pow02-ym_1958_04",
-            "ocean_3d_v_1_monthly_pow02_ym_XXXX_XX",
+            ("ocean_3d_v_1_monthly_pow02_ym_XXXX_XX", "1958_04", "1mon"),
         ),
         (
             "ocean-2d-sfc_salt_flux_restore-1-monthly-mean-ym_1958_04",
-            "ocean_2d_sfc_salt_flux_restore_1_monthly_mean_ym_XXXX_XX",
+            (
+                "ocean_2d_sfc_salt_flux_restore_1_monthly_mean_ym_XXXX_XX",
+                "1958_04",
+                "1mon",
+            ),
         ),
         (
             "oceanbgc-3d-phy-1-daily-mean-3-sigfig-5-daily-ymd_2020_12_01",
-            "oceanbgc_3d_phy_1_daily_mean_3_sigfig_5_daily_ymd_XXXX_XX_XX",
+            (
+                "oceanbgc_3d_phy_1_daily_mean_3_sigfig_5_daily_ymd_XXXX_XX_XX",
+                "2020_12_01",
+                "1day",
+            ),
         ),
-        ("iceh.1985-08-31", "iceh_XXXX_XX_XX"),
+        ("iceh.1985-08-31", ("iceh_XXXX_XX_XX", "1985-08-31", None)),
     ],
 )
-def test_redact_time_stamps(filename, expected):
-    assert redact_time_stamps(filename) == expected
+def test_parse_access_filename(filename, expected):
+    assert parse_access_filename(filename) == expected
```

### Comparing `access_nri_intake-0.0.7/versioneer.py` & `access_nri_intake-0.0.8/versioneer.py`

 * *Files identical despite different names*

