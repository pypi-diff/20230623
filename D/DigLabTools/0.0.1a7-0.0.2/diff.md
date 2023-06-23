# Comparing `tmp/DigLabTools-0.0.1a7.tar.gz` & `tmp/DigLabTools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DigLabTools-0.0.1a7.tar", last modified: Tue May 24 11:10:47 2022, max compression
+gzip compressed data, was "DigLabTools-0.0.2.tar", last modified: Fri Jun 23 13:49:20 2023, max compression
```

## Comparing `DigLabTools-0.0.1a7.tar` & `DigLabTools-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 11:10:47.560124 DigLabTools-0.0.1a7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 11:10:47.556124 DigLabTools-0.0.1a7/DigLabTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-05-24 11:10:47.000000 DigLabTools-0.0.1a7/DigLabTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-05-24 11:10:47.000000 DigLabTools-0.0.1a7/DigLabTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-24 11:10:47.000000 DigLabTools-0.0.1a7/DigLabTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-05-24 11:10:47.000000 DigLabTools-0.0.1a7/DigLabTools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-24 11:10:47.000000 DigLabTools-0.0.1a7/DigLabTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-24 11:10:47.000000 DigLabTools-0.0.1a7/DigLabTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-05-24 11:10:47.560124 DigLabTools-0.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 11:10:47.560124 DigLabTools-0.0.1a7/redcap_bridge/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     8929 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/project_building.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/project_control.py
--rw-r--r--   0 runner    (1001) docker     (121)     5011 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/project_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8754 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/server_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 11:10:47.560124 DigLabTools-0.0.1a7/redcap_bridge/template_parts/
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/template_parts/_provenance.csv
--rw-r--r--   0 runner    (1001) docker     (121)    16758 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/template_parts/array_sua_units.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/template_parts/eyelink.csv
--rw-r--r--   0 runner    (1001) docker     (121)     5214 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/template_parts/general.csv
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/template_parts/kinarm.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 11:10:47.560124 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/check_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_project_building.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_project_control.py
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_project_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_server_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/redcap_bridge/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-24 11:10:47.560124 DigLabTools-0.0.1a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-05-24 11:10:35.000000 DigLabTools-0.0.1a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.950009 DigLabTools-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.942009 DigLabTools-0.0.2/DigLabTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-23 13:49:20.000000 DigLabTools-0.0.2/DigLabTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-23 13:49:20.000000 DigLabTools-0.0.2/DigLabTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:49:20.000000 DigLabTools-0.0.2/DigLabTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 13:49:20.000000 DigLabTools-0.0.2/DigLabTools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 13:49:20.000000 DigLabTools-0.0.2/DigLabTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 13:49:20.000000 DigLabTools-0.0.2/DigLabTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-23 13:49:20.950009 DigLabTools-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.942009 DigLabTools-0.0.2/diglab_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/diglab_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/diglab_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/diglab_utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/diglab_utils/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/diglab_utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.942009 DigLabTools-0.0.2/elab_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/project_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/project_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/project_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/server_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.946009 DigLabTools-0.0.2/elab_bridge/template_parts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/template_parts/2photon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/template_parts/eyelink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/template_parts/general.json
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/template_parts/kinarm.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/template_parts/rodent_ephys.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.946009 DigLabTools-0.0.2/elab_bridge/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/tests/test_project_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/tests/test_project_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/tests/test_project_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/elab_bridge/tests/test_server_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.946009 DigLabTools-0.0.2/redcap_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/project_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/project_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/project_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/server_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.950009 DigLabTools-0.0.2/redcap_bridge/template_parts/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/template_parts/_provenance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/template_parts/array_sua_units.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/template_parts/eyelink.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/template_parts/general.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/template_parts/kinarm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    36241 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/template_parts/patch_general.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:20.950009 DigLabTools-0.0.2/redcap_bridge/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/check_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/test_project_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/test_project_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/test_project_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/test_server_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/redcap_bridge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:49:20.950009 DigLabTools-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-23 13:49:09.000000 DigLabTools-0.0.2/setup.py
```

### Comparing `DigLabTools-0.0.1a7/LICENSE` & `DigLabTools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/cli.py` & `DigLabTools-0.0.2/redcap_bridge/cli.py`

 * *Files identical despite different names*

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/project_building.py` & `DigLabTools-0.0.2/redcap_bridge/project_building.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 import numpy as np
 import pandas as pd
 
 import redcap_bridge
 from redcap_bridge.project_validation import \
     validate_project_against_template_parts
-from redcap_bridge.utils import map_header_json_to_csv, get_repo_state
+from redcap_bridge.utils import map_header_json_to_csv
+from diglab_utils.provenance import get_repo_state
 
-redcap_bridge_dir = pathlib.Path(redcap_bridge.__file__).parent
-template_dir = redcap_bridge_dir / 'template_parts'
+diglabtools_dir = pathlib.Path(redcap_bridge.__file__).parents[1]
+template_dir = diglabtools_dir / 'redcap_bridge'/ 'template_parts'
 
 
 def build_project(project_csv, output_file=None, include_provenance=True):
     """
     Build a complete RedCap Instrument CSV from a set of template_parts and a
     project csv file.
 
@@ -67,16 +68,16 @@
                     output.extend(f_include.readlines())
             else:
                 output.append(line)
 
         if include_provenance:
 
             # collect provenance infos
-            diglabtools_hash, diglabtools_state = get_repo_state(redcap_bridge_dir.parent)
-            diglabtools_version = open(redcap_bridge_dir / 'VERSION').read().strip()
+            diglabtools_hash, diglabtools_state = get_repo_state(diglabtools_dir.parent)
+            diglabtools_version = open(diglabtools_dir / 'VERSION').read().strip()
             project_conf_repo_hash, project_conf_repo_state = get_repo_state(project_csv)
 
             if not diglabtools_state:
                 warnings.warn('DigLabTools repository is in non-clean state.')
             if project_conf_repo_state is None:
                 warnings.warn('Project configuration is not part of a version control repository.')
             elif not project_conf_repo_state:
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/project_control.py` & `DigLabTools-0.0.2/redcap_bridge/project_control.py`

 * *Files identical despite different names*

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/project_validation.py` & `DigLabTools-0.0.2/redcap_bridge/project_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pathlib
 
 import pandas as pd
+import warnings
 
 import redcap_bridge
 from redcap_bridge.utils import map_header_json_to_csv
 
 index_column_header = 'Variable / Field Name'
 
 template_dir = pathlib.Path(redcap_bridge.__file__).parent / 'template_parts'
@@ -30,16 +31,15 @@
     df_project = pd.read_csv(project)
     # unify column names to conform to csv style
     df_project = df_project.rename(columns=map_header_json_to_csv)
     df_project.index = df_project[index_column_header]
     dfs_templates = []
 
     if not templates:
-        raise ValueError(
-            'No template_parts to validate against were specified.')
+        warnings.warn('No template selected list is empty')
 
     for template in templates:
         df_template = pd.read_csv((template_dir / template).with_suffix('.csv'))
         df_template.index = df_template[index_column_header]
         dfs_templates.append(df_template)
 
     # compare content of template_parts and project
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/server_interface.py` & `DigLabTools-0.0.2/redcap_bridge/server_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,16 @@
    Parameters
    ----------
    csv_file: str
        Path to the csv file to be used as data dictionary
    server_config_json: str
        Path to the json file containing the redcap url and api token
 
-    Returns:
-    ----------
-
-    Returns:
+    Returns
+    -------
         (int): The number of uploaded fields
     """
 
     df = pd.read_csv(csv_file, dtype=str)
     df.rename(columns=map_header_csv_to_json, inplace=True)
 
     # Upload csv using pycap
@@ -116,18 +114,16 @@
    Parameters
    ----------
    csv_file: str
        Path to the csv file to be used as records
    server_config_json: str
        Path to the json file containing the redcap url and api token
 
-    Returns:
-    ----------
-
-    Returns:
+    Returns
+    -------
         (int): Number of uploaded records
     """
 
     df = pd.read_csv(csv_file, dtype=str)
     df.rename(columns=map_header_csv_to_json, inplace=True)
 
     # Upload csv using pycap
@@ -141,21 +137,18 @@
 
     n = redproj.import_records(df, import_format='df', return_format_type='json')
     return n['count']
 
 
 def get_json_csv_header_mapping(server_config_json):
     """
-    Retruns
-    ----------
+    Returns
+    -------
     dict: 
         Mapping of json to csv headers
-
-    Returns:
-        dict: Mapping of json to csv headers
     """
 
     # TODO: This function should replace utils.py/map_header_json_to_csv
     raise NotImplementedError()
 
 
 def check_external_modules(server_config_json):
@@ -221,17 +214,14 @@
     Setting project specific settings on server
 
     Parameters
     ----------
     server_config_json: str
         Path to the json file containing the redcap url, api token and required external modules
 
-    Returns
-    -------
-        bool: True if required external modules are present
     """
 
     redproj = get_redcap_project(server_config_json)
     proj_json = redproj.export_project_info(format_type='json')
 
     config = json.load(open(server_config_json, 'r'))
 
@@ -239,49 +229,14 @@
     # setting project info requires a SUPER API token - not for standard usage
     if not proj_json['surveys_enabled']:
         warnings.warn(f'Surveys are not enabled for project {proj_json["project_title"]} '
                       f'(project_id {proj_json["project_id"]}). Visit the RedCap webinterface and '
                       f'enable surveys to be able to collect data via the survey URL')
 
 
-def check_external_modules(server_config_json):
-    """
-    Download records from the redcap server.
-
-    Parameters
-    ----------
-    server_config_json: str
-        Path to the json file containing the redcap url, api token and required external modules
-
-    Returns
-    -------
-        bool: True if required external modules are present
-
-    """
-    config = json.load(open(server_config_json, 'r'))
-
-    if 'external_modules' not in config:
-        warnings.warn('No external_modules defined in project configuration')
-        return True
-
-    proj_json = json.load(open(server_config_json, 'r'))
-
-    missing_modules = []
-
-    for ext_mod in config['external_modules']:
-        if ext_mod not in proj_json['external_modules']:
-            missing_modules.append(ext_mod)
-
-    if missing_modules:
-        warnings.warn(f'Project on server is missing external modules: {missing_modules}')
-        return False
-    else:
-        return True
-
-
 def get_redcap_project(server_config_json):
     """
     Initialize a pycap project based on the provided server configuration
     :param server_config_json: json file containing the api_url and api_token
     :return: pycap project
     """
     config = json.load(open(server_config_json, 'r'))
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/template_parts/_provenance.csv` & `DigLabTools-0.0.2/redcap_bridge/template_parts/_provenance.csv`

 * *Files identical despite different names*

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/template_parts/array_sua_units.csv` & `DigLabTools-0.0.2/redcap_bridge/template_parts/array_sua_units.csv`

 * *Files identical despite different names*

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/template_parts/eyelink.csv` & `DigLabTools-0.0.2/redcap_bridge/template_parts/eyelink.csv`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Variable / Field Name,Form Name,Section Header,Field Type,Field Label,"Choices, Calculations, OR Slider Labels",Field Note,Text Validation Type OR Show Slider Number,Text Validation Min,Text Validation Max,Identifier?,Branching Logic (Show field only if...),Required Field?,Custom Alignment,Question Number (surveys only),Matrix Group Name,Matrix Ranking?,Field Annotation
 eyelink_form_version,diglabform,,descriptive,Eyelink Form Version 0.0.1b,,,,,,,,,,,,,@HIDDEN
 eyelink_recorded_eye,diglabform,,dropdown,Recorded Eye,"left, Left | right, Right | both, Both | none, None",,,,,,,,,,,,
 eyelink_offset_x,diglabform,,text,Offset X,,,,,,,,y,,,,,
 eyelink_offset_y,diglabform,,text,Offset Y,,,,,,,,y,,,,,
 eyelink_gain_x,diglabform,,text,Gain X,,,,,,,,y,,,,,
 eyelink_gain_y,diglabform,,text,Gain Y,,,,,,,,y,,,,,
+eyelink_pupil_detection_threshold,diglabform,,text,Pupil detection threshold,,,number,,,,,y,,,,,
+eyelink_cornea_detection_threshold,diglabform,,text,Cornea detection threshold,,,number,,,,,y,,,,,
 data_quality_eye,diglabform,,radio,Eye movement data quality,"very_good, Very good | good, Good | bad_calibration, Bad calibration | noisy, Noisy | no_data, No data",,,,,,,y,,,,,
 eye_screen_distance,diglabform,,descriptive,Eye Screen Distance,,,,,,,,,,,,,
 eye_screen_distance_x,diglabform,,text,X,,in cm,number,,,,,y,,,,,
 eye_screen_distance_y,diglabform,,text,Y,,in cm,number,,,,,y,,,,,
 eye_screen_distance_z,diglabform,,text,Z,,in cm,number,,,,,y,,,,,
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/template_parts/general.csv` & `DigLabTools-0.0.2/redcap_bridge/template_parts/general.csv`

 * *Files identical despite different names*

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/template_parts/kinarm.csv` & `DigLabTools-0.0.2/redcap_bridge/template_parts/kinarm.csv`

 * *Files identical despite different names*

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/test_redcap/check_connectivity.py` & `DigLabTools-0.0.2/redcap_bridge/tests/check_connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import redcap_bridge
 from redcap_bridge.server_interface import download_project_settings
 from pathlib import Path
 
 
 def check_connectivity():
     print(f'RCB location: {Path(redcap_bridge.__file__).parent}')
-    test_project = Path(redcap_bridge.__file__).parent / 'test_redcap' / 'testfiles' / 'TestProject' / 'project.json'
+    test_project = Path(redcap_bridge.__file__).parent / 'tests' / 'testfiles_redcap' / 'TestProject' / 'project.json'
 
     res = download_project_settings(test_project)
     if not res['project_id']:
         raise ValueError('Unsuccessful download')
 
 
 if __name__ == '__main__':
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_cli.py` & `DigLabTools-0.0.2/redcap_bridge/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import subprocess
 import pathlib
 
 from redcap_bridge.server_interface import upload_datadict, upload_records
-from redcap_bridge.test_redcap.test_utils import (test_directory, initialize_test_dir)
-from redcap_bridge.test_redcap.test_server_interface import SERVER_CONFIG_YAML
+from redcap_bridge.tests.test_utils import (test_directory, initialize_test_dir)
+from redcap_bridge.tests.test_server_interface import SERVER_CONFIG_YAML
 
-project_dir = test_directory / 'testfiles' / 'TestProject'
+project_dir = test_directory / 'testfiles_redcap' / 'TestProject'
 
 
 def test_installed(initialize_test_dir):
     """
     Check that RedCapBridge was installed successfully
     """
     result = subprocess.run(['RedCapBridge', '--help'], stdout=subprocess.PIPE)
@@ -18,17 +18,17 @@
 
 def test_download(initialize_test_dir):
     """
     Check that download option works for Test Project
     """
 
     # Set up project on server
-    metadata_csv = test_directory / 'testfiles' / 'metadata.csv'
+    metadata_csv = test_directory / 'testfiles_redcap' / 'metadata.csv'
     upload_datadict(metadata_csv, SERVER_CONFIG_YAML)
-    records_csv = test_directory / 'testfiles' / 'record.csv'
+    records_csv = test_directory / 'testfiles_redcap' / 'record.csv'
     upload_records(records_csv, SERVER_CONFIG_YAML)
 
     output_file = test_directory / 'cli_download_test.csv'
 
     # download with default arguments
     result = subprocess.run(['RedCapBridge', 'download', output_file, SERVER_CONFIG_YAML],
                             stdout=subprocess.PIPE)
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_project_building.py` & `DigLabTools-0.0.2/redcap_bridge/tests/test_project_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 
 import pandas as pd
 
 from redcap_bridge.project_building import (build_project, customize_project,
                                             extract_customization)
-from redcap_bridge.test_redcap.test_utils import (test_directory,
-                                                  initialize_test_dir)
-
-project_dir = test_directory / 'testfiles' / 'TestProject'
+from redcap_bridge.tests.test_utils import (test_directory,
+                                            initialize_test_dir)
 
+project_dir = test_directory / 'testfiles_redcap' / 'TestProject'
 
 def test_build_and_customize_project(initialize_test_dir):
     """
     Test building and customizing a project based on its project specifications
     """
     # Running test project build
     build_project(project_dir / 'structure.csv',
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_project_control.py` & `DigLabTools-0.0.2/redcap_bridge/tests/test_project_control.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import pytest
 from redcap_bridge.project_control import setup_project
-from redcap_bridge.test_redcap.test_utils import (test_directory,
-                                                  initialize_test_dir)
+from redcap_bridge.tests.test_utils import (test_directory,
+                                            initialize_test_dir)
 
 def test_setup_project(initialize_test_dir):
     """
     Test building a complete project from its specifications and uploading it
     to the server
     """
     working_dir = test_directory / 'working_dir'
     working_dir.mkdir(exist_ok=True)
 
-    setup_project(test_directory / 'testfiles' / 'TestProject',
+    setup_project(test_directory / 'testfiles_redcap' / 'TestProject',
                   working_dir=working_dir)
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_project_validation.py` & `DigLabTools-0.0.2/redcap_bridge/tests/test_project_validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
 
 import pytest
 
 from redcap_bridge.project_building import build_project, customize_project
 from redcap_bridge.project_validation import \
     validate_project_against_template_parts, validate_record_against_template
-from redcap_bridge.test_redcap.test_utils import (test_directory,
-                                                  initialize_test_dir)
-
-project_dir = test_directory / 'testfiles' / 'TestProject'
+from redcap_bridge.tests.test_utils import (test_directory,
+                                            initialize_test_dir)
 
+project_dir = test_directory / 'testfiles_redcap' / 'TestProject'
 
 @pytest.fixture
 def setup_project_csvs():
     # pre-build project csvs based on project definition
     build_project(project_dir / 'structure.csv',
                   project_dir / 'build.csv')
     customize_project(project_dir / 'build.csv',
@@ -29,13 +28,19 @@
 
     validate_project_against_template_parts(project_dir / 'customized.csv',
                                             *template_parts)
 
 
 def test_validate_record_against_template(initialize_test_dir,
                                           setup_project_csvs):
-    record_csv = test_directory / 'testfiles' / 'record.csv'
+    record_csv = test_directory / 'testfiles_redcap' / 'record.csv'
 
     # validate against provided project metadata and constructed metadata
     validate_record_against_template(record_csv,
-                                     test_directory / 'testfiles' / 'metadata.csv')
+                                     test_directory / 'testfiles_redcap' / 'metadata.csv')
     validate_record_against_template(record_csv, project_dir / 'customized.csv')
+
+
+def test_validate_project_without_template(initialize_test_dir,
+                                           setup_project_csvs):
+    # test with an empty list of template parts
+    validate_project_against_template_parts(project_dir / 'customized.csv')
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_server_interface.py` & `DigLabTools-0.0.2/redcap_bridge/tests/test_server_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+
 import pandas as pd
 import pytest
 
 from redcap_bridge.server_interface import (upload_datadict, download_records, download_datadict,
                                             check_external_modules, get_redcap_project,
                                             upload_records, download_project_settings,
                                             configure_project_settings)
 
-from redcap_bridge.test_redcap.test_utils import (test_directory, initialize_test_dir)
+from redcap_bridge.tests.test_utils import (test_directory, initialize_test_dir)
 from redcap_bridge.utils import map_header_csv_to_json
 
-SERVER_CONFIG_YAML = (test_directory / 'testfiles' / 'TestProject' / 'project.json').resolve()
+SERVER_CONFIG_YAML = (test_directory / 'testfiles_redcap' / 'TestProject' / 'project.json').resolve()
 
 
 @pytest.fixture
 def clean_server(initialize_test_dir):
     """
     Put testing server in a defined state: only minimal metadata (instruments)
     and records present
@@ -28,92 +29,94 @@
     # first initialize in lazy mode to configure metadata even if server status
     # is corrupted
     redproj = get_redcap_project(SERVER_CONFIG_YAML)
 
     default_datadict = pd.DataFrame(data=[['record_id', 'my_first_instrument',
                                            'text', 'Record ID'] + [''] * 14],
                                     columns=map_header_csv_to_json)
-    redproj.import_metadata(default_datadict, import_format='csv')
+    redproj.import_metadata(default_datadict, import_format='df')
 
     # second initialize in non-lazy mode to configure records
     redproj = get_redcap_project(SERVER_CONFIG_YAML)
     default_records = pd.DataFrame(columns=['record_id',
                                             'my_first_instrument_complete'])
     redproj.import_records(default_records,
-                           import_format='csv', return_format_type='json',
+                           import_format='df', return_format_type='json',
                            overwrite="overwrite")
 
 
 def test_upload_datadict(clean_server, initialize_test_dir):
     """
     Test uploading a survey definition (datadict) csv to the server
     """
     # uploading metadata csv files from testfile dataset and compare to
     # return value of upload
-    metadata_csv = test_directory / 'testfiles' / 'metadata.csv'
+    metadata_csv = test_directory / 'testfiles_redcap' / 'metadata.csv'
     res = upload_datadict(metadata_csv, SERVER_CONFIG_YAML)
 
     # count number of non-empty lines in original csv
     with open(metadata_csv) as f:
         lines = f.readlines()
         exp = len(lines) - 1  # header row does not generate a record
 
     assert exp == res
 
 
 def test_upload_records(clean_server, initialize_test_dir):
     """
     Test upload of records to the server
     """
-    upload_datadict(test_directory / 'testfiles' / 'metadata.csv', SERVER_CONFIG_YAML)
-    res = upload_records(test_directory / 'testfiles' / 'record.csv', SERVER_CONFIG_YAML)
+    upload_datadict(test_directory / 'testfiles_redcap' / 'metadata.csv', SERVER_CONFIG_YAML)
+    res = upload_records(test_directory / 'testfiles_redcap' / 'record.csv', SERVER_CONFIG_YAML)
 
     # test record.csv contains 2 records
     assert res == 2
 
 
 def test_download_records(clean_server, initialize_test_dir):
     """
     Download datadict from server and compare to previously uploaded datadict
     """
     # uploading metadata csv files from testfile dataset and compare to
     # return value of upload
-    original_record_csv = test_directory / 'testfiles' / 'record.csv'
-    upload_datadict(test_directory / 'testfiles' / 'metadata.csv', SERVER_CONFIG_YAML)
-    upload_records(test_directory / 'testfiles' / 'record.csv', SERVER_CONFIG_YAML)
+    original_record_csv = test_directory / 'testfiles_redcap' / 'record.csv'
+    upload_datadict(test_directory / 'testfiles_redcap' / 'metadata.csv', SERVER_CONFIG_YAML)
+    upload_records(test_directory / 'testfiles_redcap' / 'record.csv', SERVER_CONFIG_YAML)
 
-    downloaded_record_csv = test_directory / 'testfiles' / 'record_downloaded.csv'
+    downloaded_record_csv = test_directory / 'testfiles_redcap' / 'record_downloaded.csv'
     download_records(downloaded_record_csv, SERVER_CONFIG_YAML)
 
     import csv
     original_reader = csv.reader(open(original_record_csv))
     download_reader = csv.reader(open(downloaded_record_csv))
 
     # comparing headers
     original_header = original_reader.__next__()
     downloaded_header = download_reader.__next__()
     for i, oh in enumerate(original_header):
+        # uploading of records can fail if the record cache on the server is not clean
+        # in this case reset the record cache on the webinterface of redcap
         assert oh in downloaded_header, f'{oh} not in downloaded header'
 
     # compare content
     for oline, dline in zip(original_reader, download_reader):
         assert oline == dline
 
 
 def test_download_datadict(clean_server, initialize_test_dir):
     """
     Download datadict from server and compare to previously uploaded datadict
     """
     # uploading metadata csv files from testfile dataset and compare to
     # return value of upload
-    original_metadata_csv = test_directory / 'testfiles' / 'metadata.csv'
+    original_metadata_csv = test_directory / 'testfiles_redcap' / 'metadata.csv'
     upload_datadict(original_metadata_csv, SERVER_CONFIG_YAML)
 
 
-    downloaded_metadata_csv = test_directory / 'testfiles' / 'metadata_downloaded.csv'
+    downloaded_metadata_csv = test_directory / 'testfiles_redcap' / 'metadata_downloaded.csv'
     download_datadict(downloaded_metadata_csv, SERVER_CONFIG_YAML)
 
 
     import csv
     original_reader = csv.reader(open(original_metadata_csv))
     download_reader = csv.reader(open(downloaded_metadata_csv))
 
@@ -155,12 +158,20 @@
     configure_project_settings(SERVER_CONFIG_YAML)
 
     # confirm project settings on server are consistent with project configuration
     proj_settings = download_project_settings(SERVER_CONFIG_YAML)
     assert proj_settings['surveys_enabled']
     assert len(proj_settings['external_modules'])
 
+    # no repeating instruments set at this time as no records were imported
+    # redproj = get_redcap_project(SERVER_CONFIG_YAML)
+    # rep_inst_settings = redproj.export_repeating_instruments_events()
+    # assert len(rep_inst_settings) == 1
+    # assert "form_name" in rep_inst_settings[0]
+    # assert "custom_form_label" in rep_inst_settings[0]
+
     redproj = get_redcap_project(SERVER_CONFIG_YAML)
-    rep_inst_settings = redproj.export_repeating_instruments_events()
-    assert len(rep_inst_settings) == 1
-    assert "form_name" in rep_inst_settings[0]
-    assert "custom_form_label" in rep_inst_settings[0]
+    metadata = redproj.export_metadata()
+    records = redproj.export_records()
+    assert 'field_name' in metadata[0]
+    assert 'record_id' in records[0]
+
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/test_redcap/test_utils.py` & `DigLabTools-0.0.2/diglab_utils/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,15 @@
+import shutil
 import os
 import pathlib
-import shutil
 import tempfile
-
 import pytest
 
-from redcap_bridge.utils import compress_record
 test_directory = pathlib.Path(tempfile.gettempdir()) / 'diglabtools_testfiles'
-project_dir = test_directory / 'testfiles' / 'TestProject'
-
+project_dir = test_directory / 'testfiles_redcap' / 'TestProject'
 
 @pytest.fixture
 def initialize_test_dir(clean=True):
     """
     Create main test folder if required and add test files
 
     Parameters
@@ -27,23 +24,14 @@
     """
     if clean and os.path.exists(test_directory):
         shutil.rmtree(test_directory)
     if not os.path.exists(test_directory):
         os.mkdir(test_directory)
 
     # initialize test files
-    packaged_testfolder = pathlib.Path(__file__).parent / 'testfiles'
-    shutil.copytree(packaged_testfolder, test_directory / 'testfiles')
-    return test_directory
-
-
-def test_compressedCSV(initialize_test_dir):
-
-    test_dir = test_directory / 'testfiles' / 'compression_test'
-
-    compress_record(test_dir / 'original_record.csv', test_dir / 'compressed_record.csv')
-    with open(test_dir / 'compressed_record.csv') as comp_file:
-        with open(test_dir / 'expected_record.csv') as exp_file:
-            res = comp_file.read()
-            exp = exp_file.read()
-
-            assert res == exp
+    packaged_testfolders = [
+        pathlib.Path(__file__).parents[1] / 'redcap_bridge' / 'tests' /'testfiles_redcap',
+        pathlib.Path(__file__).parents[1] / 'elab_bridge' / 'tests' / 'testfiles_elab',
+        pathlib.Path(__file__).parents[1] / 'diglab_utils' / 'tests' / 'testfiles_diglab_utils']
+    for server, packaged_testfolder in zip(['redcap', 'elab', 'diglab_utils'], packaged_testfolders):
+        shutil.copytree(packaged_testfolder, test_directory / packaged_testfolder.name)
+    return test_directory
```

### Comparing `DigLabTools-0.0.1a7/redcap_bridge/utils.py` & `DigLabTools-0.0.2/redcap_bridge/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-import git
-import pathlib
 import pandas as pd
-import re as re
 import warnings
 
 # TODO: This can be extracted via the RedCap API
 header_json = ['field_name', 'form_name', 'section_header', 'field_type',
                'field_label', 'select_choices_or_calculations', 'field_note',
                'text_validation_type_or_show_slider_number',
                'text_validation_min', 'text_validation_max', 'identifier',
@@ -23,52 +20,14 @@
 
 map_header_json_to_csv = {json: csv for json, csv in zip(header_json,
                                                          header_csv)}
 map_header_csv_to_json = {csv: json for csv, json in zip(header_csv,
                                                          header_json)}
 
 
-def get_repo_state(path):
-    """
-    Extract the latest commit hash of a git repository
-
-    Args:
-        path: Path to the git repository
-
-    Returns:
-        2-tuple (str, bool)
-            latest commit id
-            repo status: True if repository is in a clean state
-
-    Raises:
-        ValueError: if path is not part of a git repository
-    """
-
-    repo_root = None
-    # find repository root folder
-    path = pathlib.Path(path)
-    for parent in [path] + list(path.parents):
-        if (parent / '.git').exists():
-            repo_root = parent
-            break
-
-    if repo_root is None:
-        return '', None
-
-    repo = git.Repo.init(str(repo_root))
-    clean = not repo.is_dirty()
-    try:
-        commit_hash = repo.head.commit.hexsha
-    except ValueError as e:
-        commit_hash = ''
-        clean = False
-
-    return commit_hash, clean
-
-
 def compress_record(csv_file, compressed_file=None):
     warnings.warn(f'Compressing {csv_file} does not preserve all original information.'
                   f'This operation is potentially irreversible.')
 
     df = pd.read_csv(csv_file, na_filter=False, dtype='str')
 
     # compressing embedded fields
@@ -109,7 +68,16 @@
         # remove sub-columns (that are now shifted by 1)
         df.drop(df.columns[sub_indexes + 1], axis='columns', inplace=True)
 
     if compressed_file is None:
         return df
     else:
         df.to_csv(compressed_file, index=False)
+
+
+def remove_columns(csv_file, compressed_file=None):
+    df = pd.read_csv(csv_file, na_filter=False, dtype='str')
+
+
+def exportCSVtoXLS(csv_file, compressed_file=None):
+    read_file = pd.read_csv(csv_file, na_filter=False, dtype='str')
+    read_file.to_excel(r'Path', index=None, header=True)
```

### Comparing `DigLabTools-0.0.1a7/setup.py` & `DigLabTools-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 import json
 
 from setuptools import setup, find_packages
 import os
 
 # Extract central version information
-with open(os.path.join(os.path.dirname(__file__), "redcap_bridge/VERSION")) as version_file:
+with open(os.path.join(os.path.dirname(__file__), "VERSION")) as version_file:
     version = version_file.read().strip()
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 with open('README.md') as f:
     long_description = f.read()
@@ -19,25 +19,26 @@
     name="DigLabTools",
     version=version,
     packages=find_packages(),
     package_data={
         # If any package contains *.json or *.csv files, include them:
         "": ["*.json", '*.csv', '*.zip'],
     },
-    data_files=[('DigLabTools', ['redcap_bridge/VERSION', 'README.md', 'requirements.txt'])],
-    author="Julia Sprenger, Jeremy Garcia",
+    data_files=[('DigLabTools', ['VERSION', 'README.md', 'requirements.txt'])],
+    author="Julia Sprenger, Jeremy Garcia, Killian Rochet",
     description="Tools to interact with the DigLab metadata collection standard",
     long_description_content_type="text/markdown",
     long_description=long_description,
     license='MIT',
     install_requires=requires,
     include_package_data=True,
     python_requires='>=3.8',
     extras_require={
         'test': ['pytest']
     },
     entry_points={
         "console_scripts": [
             "RedCapBridge=redcap_bridge.cli:main",
+            "ElabBridge=elab_bridge.cli:main"
         ],
     }
 )
```

