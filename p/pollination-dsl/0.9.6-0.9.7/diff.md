# Comparing `tmp/pollination-dsl-0.9.6.tar.gz` & `tmp/pollination-dsl-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-dsl-0.9.6.tar", last modified: Sun Feb  7 19:24:43 2021, max compression
+gzip compressed data, was "dist/pollination-dsl-0.9.7.tar", last modified: Sat Feb 13 03:17:18 2021, max compression
```

## Comparing `pollination-dsl-0.9.6.tar` & `pollination-dsl-0.9.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12047 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9399 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)      191 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/docs/_build/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     6564 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl/alias/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10643 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/alias/inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9486 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/alias/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8887 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    11785 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl/dag/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4251 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/dag/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6828 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/dag/inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7600 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/dag/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11192 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/dag/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl/function/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5921 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/function/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5214 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/function/inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4993 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/function/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/pollination_dsl/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12047 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      997 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/pollination_dsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-02-07 19:24:43.000000 pollination-dsl-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-02-07 19:22:03.000000 pollination-dsl-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12047 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9399 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/docs/_build/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6564 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl/alias/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10643 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/alias/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9486 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/alias/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8887 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11988 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/common.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl/dag/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4551 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/dag/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6828 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/dag/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7600 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/dag/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11192 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/dag/task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl/function/
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5921 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/function/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5214 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/function/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4993 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/function/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/pollination_dsl/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12047 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/pollination_dsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-02-13 03:17:18.000000 pollination-dsl-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-02-13 03:16:12.000000 pollination-dsl-0.9.7/setup.py
```

### Comparing `pollination-dsl-0.9.6/.github/workflows/ci.yaml` & `pollination-dsl-0.9.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/LICENSE` & `pollination-dsl-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/PKG-INFO` & `pollination-dsl-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-dsl
-Version: 0.9.6
+Version: 0.9.7
 Summary: A Python DSL to create Pollination recipes and plugins.
 Home-page: https://github.com/pollination/pollination-dsl
 Author: Pollination
 Author-email: info@pollination.cloud
 License: UNKNOWN
 Description: # pollination-dsl
         A Python Domain Specific Language (DSL) to create Pollination Plugins and Recipes.
```

### Comparing `pollination-dsl-0.9.6/README.md` & `pollination-dsl-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/docs/conf.py` & `pollination-dsl-0.9.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/alias/inputs.py` & `pollination-dsl-0.9.7/pollination_dsl/alias/inputs.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/alias/outputs.py` & `pollination-dsl-0.9.7/pollination_dsl/alias/outputs.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/cli.py` & `pollination-dsl-0.9.7/pollination_dsl/cli.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/common.py` & `pollination-dsl-0.9.7/pollination_dsl/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 from typing import NamedTuple, Dict, List
-import importlib
 from collections import namedtuple
 import importlib_metadata
 import re
 import pkg_resources
 import warnings
 import subprocess
 import sys
@@ -128,28 +127,30 @@
         )
         image_id = f'ladybugtools/{dependency}:latest'
 
     return image_id
 
 
 def _get_package_readme(package_name: str) -> str:
-    package_data = importlib_metadata.metadata(package_name.replace('-', '_'))
+    package_name = name_to_pollination(package_name).replace('-', '_')
+    package_data = importlib_metadata.metadata(package_name)
     long_description = package_data.get_payload()
     if not long_description.strip():
         content = package_data.get('Description')
         long_description = []
         for line in content.split('\n'):
             long_description.append(re.sub('^        ', '', line))
         long_description = '\n'.join(long_description)
     return long_description
 
 
 def _get_package_owner(package_name: str) -> str:
     """Author field is used for package owner."""
-    package_data = importlib_metadata.metadata(package_name.replace('-', '_'))
+    package_name = name_to_pollination(package_name).replace('-', '_')
+    package_data = importlib_metadata.metadata(package_name)
     owner = package_data.get('Author')
     assert owner, \
         'You must set the author of the package in setup.py to Pollination account owner'
     # ensure there is only one author
     owner = owner.strip()
     assert len(owner.split(',')) == 1, \
         'A Pollination package can only have one author. Use maintainer field for ' \
@@ -233,15 +234,16 @@
         # development version like 0.1.dev1+gf910655.d20210207
         version = f'{x}.{y}.0'
 
     return version
 
 
 def _get_package_data(package_name: str) -> Dict:
-
+    """Get package data as a dictionary."""
+    package_name = name_to_pollination(package_name).replace('-', '_')
     package_data = importlib_metadata.metadata(package_name)
 
     data = {
         'name': package_data.get('Name').replace('pollination-', ''),
         'description': package_data.get('Summary'),
         'home': package_data.get('Home-page'),
         'tag': _get_package_version(package_data),
```

### Comparing `pollination-dsl-0.9.6/pollination_dsl/dag/base.py` & `pollination-dsl-0.9.7/pollination_dsl/dag/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """DAG dependencies.
 
         Dependencies are plugins or other recipes.
         """
         cls = self.__class__
         dag_package = self._package
         dependencies = {'plugin': [], 'recipe': [], 'dag': []}
-        for method_name, method in inspect.getmembers(cls):
+        for _, method in inspect.getmembers(cls):
             # try to get decorator
             qb_dec = getattr(method, '__decorator__', None)
             if qb_dec == 'task':
                 # get template
                 tt = method.__task_template__
                 if tt.__decorator__ == 'dag':
                     if tt._package == dag_package:
@@ -118,8 +118,16 @@
                         # dependency is another plugin
                         if tt._package not in dependencies['recipe']:
                             dependencies['recipe'].append(tt._package)
                 elif tt.__decorator__ == 'function':
                     if tt._package not in dependencies['plugin']:
                         dependencies['plugin'].append(tt._package)
 
+        # add dependencies of dag dependencies
+        for dag in dependencies['dag']:
+            deps = dag._dependencies
+            for key, sub_deps in deps.items():
+                for v in sub_deps:
+                    if v not in dependencies[key]:
+                        dependencies[key].append(v)
+
         return dependencies
```

### Comparing `pollination-dsl-0.9.6/pollination_dsl/dag/inputs.py` & `pollination-dsl-0.9.7/pollination_dsl/dag/inputs.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/dag/outputs.py` & `pollination-dsl-0.9.7/pollination_dsl/dag/outputs.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/dag/task.py` & `pollination-dsl-0.9.7/pollination_dsl/dag/task.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/function/base.py` & `pollination-dsl-0.9.7/pollination_dsl/function/base.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/function/inputs.py` & `pollination-dsl-0.9.7/pollination_dsl/function/inputs.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/function/outputs.py` & `pollination-dsl-0.9.7/pollination_dsl/function/outputs.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl/package.py` & `pollination-dsl-0.9.7/pollination_dsl/package.py`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/pollination_dsl.egg-info/PKG-INFO` & `pollination-dsl-0.9.7/pollination_dsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-dsl
-Version: 0.9.6
+Version: 0.9.7
 Summary: A Python DSL to create Pollination recipes and plugins.
 Home-page: https://github.com/pollination/pollination-dsl
 Author: Pollination
 Author-email: info@pollination.cloud
 License: UNKNOWN
 Description: # pollination-dsl
         A Python Domain Specific Language (DSL) to create Pollination Plugins and Recipes.
```

### Comparing `pollination-dsl-0.9.6/pollination_dsl.egg-info/SOURCES.txt` & `pollination-dsl-0.9.7/pollination_dsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-dsl-0.9.6/setup.py` & `pollination-dsl-0.9.7/setup.py`

 * *Files identical despite different names*

