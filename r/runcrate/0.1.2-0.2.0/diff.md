# Comparing `tmp/runcrate-0.1.2.tar.gz` & `tmp/runcrate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runcrate-0.1.2.tar", last modified: Thu Mar 23 14:29:03 2023, max compression
+gzip compressed data, was "runcrate-0.2.0.tar", last modified: Fri Jun 23 10:29:26 2023, max compression
```

## Comparing `runcrate-0.1.2.tar` & `runcrate-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:29:03.485599 runcrate-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-23 14:28:55.000000 runcrate-0.1.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-23 14:28:55.000000 runcrate-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-03-23 14:28:55.000000 runcrate-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-23 14:28:55.000000 runcrate-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-23 14:28:55.000000 runcrate-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-23 14:29:03.485599 runcrate-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-23 14:28:55.000000 runcrate-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:29:03.485599 runcrate-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:29:03.485599 runcrate-0.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/reference/main.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 14:28:55.000000 runcrate-0.1.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 14:28:55.000000 runcrate-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-23 14:28:55.000000 runcrate-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-23 14:29:03.485599 runcrate-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-23 14:28:55.000000 runcrate-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:29:03.481599 runcrate-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:29:03.485599 runcrate-0.1.2/src/runcrate/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-23 14:28:55.000000 runcrate-0.1.2/src/runcrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-03-23 14:28:55.000000 runcrate-0.1.2/src/runcrate/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-23 14:28:55.000000 runcrate-0.1.2/src/runcrate/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-03-23 14:28:55.000000 runcrate-0.1.2/src/runcrate/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-23 14:28:55.000000 runcrate-0.1.2/src/runcrate/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-23 14:28:55.000000 runcrate-0.1.2/src/runcrate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:29:03.485599 runcrate-0.1.2/src/runcrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-23 14:29:03.000000 runcrate-0.1.2/src/runcrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-23 14:29:03.000000 runcrate-0.1.2/src/runcrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:29:03.000000 runcrate-0.1.2/src/runcrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-23 14:29:03.000000 runcrate-0.1.2/src/runcrate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:29:03.000000 runcrate-0.1.2/src/runcrate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-23 14:29:03.000000 runcrate-0.1.2/src/runcrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 14:29:03.000000 runcrate-0.1.2/src/runcrate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:26.699746 runcrate-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-23 10:29:17.000000 runcrate-0.2.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 10:29:17.000000 runcrate-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-23 10:29:17.000000 runcrate-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 10:29:17.000000 runcrate-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-23 10:29:17.000000 runcrate-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-23 10:29:26.699746 runcrate-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-23 10:29:17.000000 runcrate-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:26.695746 runcrate-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:26.695746 runcrate-0.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/reference/main.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 10:29:17.000000 runcrate-0.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 10:29:17.000000 runcrate-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 10:29:17.000000 runcrate-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-23 10:29:26.699746 runcrate-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 10:29:17.000000 runcrate-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:26.695746 runcrate-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:26.699746 runcrate-0.2.0/src/runcrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-23 10:29:17.000000 runcrate-0.2.0/src/runcrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-23 10:29:17.000000 runcrate-0.2.0/src/runcrate/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-23 10:29:17.000000 runcrate-0.2.0/src/runcrate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32086 2023-06-23 10:29:17.000000 runcrate-0.2.0/src/runcrate/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-23 10:29:17.000000 runcrate-0.2.0/src/runcrate/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-23 10:29:17.000000 runcrate-0.2.0/src/runcrate/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-23 10:29:17.000000 runcrate-0.2.0/src/runcrate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:26.699746 runcrate-0.2.0/src/runcrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-23 10:29:26.000000 runcrate-0.2.0/src/runcrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-23 10:29:26.000000 runcrate-0.2.0/src/runcrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:29:26.000000 runcrate-0.2.0/src/runcrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 10:29:26.000000 runcrate-0.2.0/src/runcrate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:29:26.000000 runcrate-0.2.0/src/runcrate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 10:29:26.000000 runcrate-0.2.0/src/runcrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 10:29:26.000000 runcrate-0.2.0/src/runcrate.egg-info/top_level.txt
```

### Comparing `runcrate-0.1.2/CONTRIBUTING.rst` & `runcrate-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `runcrate-0.1.2/LICENSE` & `runcrate-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runcrate-0.1.2/PKG-INFO` & `runcrate-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runcrate
-Version: 0.1.2
+Version: 0.2.0
 Summary: Workflow Run RO-Crate toolkit
 Home-page: https://github.com/ResearchObject/runcrate
 Author: CRS4, RO-Crate community
 Author-email: ro-crate@elixir-europe.org
 License: Apache License, version 2.0 (Apache-2.0)
 Keywords: ro-crate,workflow,provenance,CWL
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `runcrate-0.1.2/README.rst` & `runcrate-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `runcrate-0.1.2/setup.cfg` & `runcrate-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.8, <4
 install_requires = 
 	bdbag>=1.4.1
 	click~=8.1
-	cwl-utils==0.13
+	cwl-utils>=0.27
 	cwlprov==0.1.1
-	networkx==2.8
+	networkx==3.1
 	prov>=1.5.1
-	rocrate~=0.7
+	rocrate~=0.8
 
 [options.entry_points]
 console_scripts = 
 	runcrate=runcrate.cli:cli
 
 [options.packages.find]
 where = src
```

### Comparing `runcrate-0.1.2/src/runcrate/__init__.py` & `runcrate-0.2.0/src/runcrate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
```

### Comparing `runcrate-0.1.2/src/runcrate/cli.py` & `runcrate-0.2.0/src/runcrate/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from pathlib import Path
 
 import click
 
 from . import __version__
 from .convert import ProvCrateBuilder
 from .report import dump_crate_actions
+from .run import run_crate
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -83,14 +84,36 @@
 
     RO_CRATE: RO-Crate directory or zip file.
     """
     dump_crate_actions(crate)
 
 
 @cli.command()
+@click.argument(
+    "crate",
+    metavar="RO_CRATE",
+    type=click.Path(exists=True, readable=True, path_type=Path),
+)
+@click.option("--executable", help="workflow runner executable")
+@click.option("--keep-wd", help="keep working directory", is_flag=True)
+@click.option(
+    "--dry-run",
+    help="do not actually run the workflow (implies --keep-wd)",
+    is_flag=True
+)
+def run(crate, executable, keep_wd, dry_run):
+    """\
+    Run the workflow from a Workflow Run RO-Crate.
+
+    RO_CRATE: RO-Crate directory or zip file.
+    """
+    run_crate(crate, executable=executable, keep_wd=keep_wd, dry_run=dry_run)
+
+
+@cli.command()
 def version():
     """\
     Print version string and exit.
     """
     sys.stdout.write(f"{__version__}\n")
```

### Comparing `runcrate-0.1.2/src/runcrate/constants.py` & `runcrate-0.2.0/src/runcrate/constants.py`

 * *Files identical despite different names*

### Comparing `runcrate-0.1.2/src/runcrate/convert.py` & `runcrate-0.2.0/src/runcrate/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright 2022-2023 CRS4.
+# Copyright 2023 Michael R. Crusoe
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,14 +16,15 @@
 """\
 Generate a Workflow Run RO-Crate from a CWLProv RO bundle.
 """
 
 import hashlib
 import json
 import re
+from io import StringIO
 from pathlib import Path
 
 import networkx as nx
 import prov.model
 from bdbag.bdbagit import BDBag
 from cwl_utils.parser import load_document_by_yaml
 from cwlprov.prov import Entity, Provenance
@@ -33,14 +35,16 @@
 from rocrate.rocrate import ROCrate
 
 from .constants import EXTRA_TERMS, PROFILES_BASE, PROFILES_VERSION
 from .utils import as_list
 
 
 WORKFLOW_BASENAME = "packed.cwl"
+INPUTS_FILE_BASENAME = "primary-job.json"
+MANIFEST_FILE = "manifest-sha1.txt"
 
 CWL_TYPE_MAP = {
     "string": "Text",
     "int": "Integer",
     "long": "Integer",
     "float": "Float",
     "double": "Float",
@@ -64,44 +68,45 @@
         s.discard(None)
         return s.pop() if len(s) == 1 else sorted(s)
     if isinstance(cwl_type, str):
         return CWL_TYPE_MAP[cwl_type]
     if cwl_type.type == "enum":
         return "Text"  # use actionOption to represent choices?
     if cwl_type.type == "array":
-        return CWL_TYPE_MAP[cwl_type.items]
+        return convert_cwl_type(cwl_type.items)
     if cwl_type.type == "record":
         return "PropertyValue"
 
 
 def properties_from_cwl_param(cwl_p):
     def is_structured(cwl_type):
         return getattr(cwl_type, "type", None) in ("array", "record")
     additional_type = "Collection" if cwl_p.secondaryFiles else convert_cwl_type(cwl_p.type)
     properties = {
         "@type": "FormalParameter",
         "additionalType": additional_type
     }
+    if hasattr(cwl_p, "doc") and cwl_p.doc:
+        properties["description"] = cwl_p.doc
+    elif hasattr(cwl_p, "label") and cwl_p.label:
+        # name is used for the parameter's id to support reproducibility
+        properties["description"] = cwl_p.label
     if cwl_p.format:
         properties["encodingFormat"] = cwl_p.format
     if isinstance(cwl_p.type, list) and "null" in cwl_p.type:
         properties["valueRequired"] = "False"
     if is_structured(cwl_p.type):
         properties["multipleValues"] = "True"
     if hasattr(cwl_p, "default"):
-        try:
-            default_type = cwl_p.default["class"]
-        except (TypeError, KeyError):
-            if not is_structured(cwl_p.type) and cwl_p.default is not None:
-                properties["defaultValue"] = str(cwl_p.default)
-        else:
-            if default_type in ("File", "Directory"):
-                default = cwl_p.default.get("location", cwl_p.default.get("path"))
-                if default:
-                    properties["defaultValue"] = default
+        if hasattr(cwl_p.default, "class_") and cwl_p.default.class_ in ("File", "Directory"):
+            default = cwl_p.default.location or cwl_p.default.path
+            if default:
+                properties["defaultValue"] = default
+        elif not is_structured(cwl_p.type) and cwl_p.default is not None:
+            properties["defaultValue"] = str(cwl_p.default)
         # TODO: support more cases
     if getattr(cwl_p.type, "type", None) == "enum":
         properties["valuePattern"] = "|".join(_.rsplit("/", 1)[-1] for _ in cwl_p.type.symbols)
     return properties
 
 
 def get_fragment(uri):
@@ -126,20 +131,38 @@
         for o in s.out:
             out_map[o] = get_fragment(s.id)
     graph = nx.DiGraph()
     for s in cwl_wf.steps:
         fragment = get_fragment(s.id)
         graph.add_node(fragment)
         for i in s.in_:
-            source_fragment = out_map.get(i.source)
-            if source_fragment:
-                graph.add_edge(source_fragment, fragment)
+            sources = [i.source] if not isinstance(i.source, list) else i.source
+            for s in sources:
+                source_fragment = out_map.get(s)
+                if source_fragment:
+                    graph.add_edge(source_fragment, fragment)
     return graph
 
 
+def normalize_cwl_defs(cwl_defs):
+    inline_tools = {}
+    for d in cwl_defs.values():
+        if not hasattr(d, "steps") or not d.steps:
+            continue
+        for s in d.steps:
+            if hasattr(s, "run") and s.run:
+                if hasattr(s.run, "id"):
+                    tool = s.run
+                    if tool.id.startswith("_:"):  # CWL > 1.0
+                        tool.id = f"{s.id}/run"
+                    inline_tools[get_fragment(tool.id)] = tool
+                    s.run = tool.id
+    cwl_defs.update(inline_tools)
+
+
 def get_workflow(wf_path):
     """\
     Read the packed CWL workflow.
 
     Returns a dictionary where tools / workflows are mapped by their ids.
 
     Does not use load_document_by_uri, so we can hack the json to work around
@@ -150,23 +173,24 @@
         json_wf = json.load(f)
     graph = json_wf.get("$graph", [json_wf])
     # https://github.com/common-workflow-language/cwltool/pull/1506
     for n in graph:
         ns = n.pop("$namespaces", {})
         if ns:
             json_wf.setdefault("$namespaces", {}).update(ns)
-    defs = load_document_by_yaml(json_wf, wf_path.absolute().as_uri())
+    defs = load_document_by_yaml(json_wf, wf_path.absolute().as_uri(), load_all=True)
     if not isinstance(defs, list):
         defs = [defs]
     def_map = {}
     for d in defs:
         k = get_fragment(d.id)
         if k == "main":
             k = wf_path.name
         def_map[k] = d
+    normalize_cwl_defs(def_map)
     return def_map
 
 
 class ProvCrateBuilder:
 
     def __init__(self, root, workflow_name=None, license=None, readme=None):
         self.root = Path(root)
@@ -182,28 +206,39 @@
         self.roc_engine_run = None
         # avoid duplicates - not handled by ro-crate-py, see
         # https://github.com/ResearchObject/ro-crate-py/issues/132
         self.control_actions = {}
         # index collections by their main entity's id
         self.collections = {}
         self.hashes = {}
+        # map source files to destination files
+        self.file_map = {}
+        self.manifest = self._get_manifest()
 
     @staticmethod
     def _get_step_maps(cwl_defs):
         rval = {}
         for k, v in cwl_defs.items():
             if hasattr(v, "steps"):
                 graph = build_step_graph(v)
                 pos_map = {f: i for i, f in enumerate(nx.topological_sort(graph))}
                 rval[k] = {}
                 for s in v.steps:
                     f = get_fragment(s.id)
                     rval[k][f] = {"tool": get_fragment(s.run), "pos": pos_map[f]}
         return rval
 
+    def _get_manifest(self):
+        manifest = {}
+        with open(self.root / Path(MANIFEST_FILE)) as f:
+            for line in f:
+                hash_, relpath = line.strip().split(None, 1)
+                manifest[hash_] = self.root / relpath
+        return manifest
+
     def _resolve_plan(self, activity):
         job_qname = activity.plan()
         plan = activity.provenance.entity(job_qname)
         if not plan:
             m = SCATTER_JOB_PATTERN.match(str(job_qname))
             if m:
                 plan = activity.provenance.entity(m.groups()[0])
@@ -252,14 +287,15 @@
         crate.metadata.extra_terms.update(EXTRA_TERMS)
         self.add_root_metadata(crate)
         self.add_profiles(crate)
         self.add_workflow(crate)
         self.add_engine_run(crate)
         self.add_action(crate, self.workflow_run)
         self.patch_workflow_input_collection(crate)
+        self.add_inputs_file(crate)
         return crate
 
     def add_root_metadata(self, crate):
         if self.license:
             crate.root_dataset["license"] = self.license
         if self.readme:
             readme = crate.add_file(self.readme)
@@ -286,21 +322,27 @@
         })))
         crate.root_dataset["conformsTo"] = profiles
 
     def add_workflow(self, crate):
         lang_version = self.cwl_defs[WORKFLOW_BASENAME].cwlVersion
         properties = {
             "@type": ["File", "SoftwareSourceCode", "ComputationalWorkflow", "HowTo"],
-            "name": self.workflow_name or self.wf_path.name
         }
         workflow = crate.add_workflow(
             self.wf_path, self.wf_path.name, main=True, lang="cwl",
             lang_version=lang_version, gen_cwl=False, properties=properties
         )
         cwl_workflow = self.cwl_defs[workflow.id]
+        wf_name = self.wf_path.name
+        if hasattr(cwl_workflow, "label") and cwl_workflow.label:
+            wf_name = cwl_workflow.label
+        workflow["name"] = self.workflow_name or wf_name
+        if hasattr(cwl_workflow, "doc") and cwl_workflow.doc:
+            workflow["description"] = cwl_workflow.doc
+        # cannot convert "intent" to featureList: workflow is not a SoftwareApplication
         workflow["input"] = self.add_params(crate, cwl_workflow.inputs)
         workflow["output"] = self.add_params(crate, cwl_workflow.outputs)
         if hasattr(cwl_workflow, "steps"):
             for s in cwl_workflow.steps:
                 self.add_step(crate, workflow, s)
             self.add_param_connections(crate, workflow)
         return workflow
@@ -311,14 +353,18 @@
         pos = self.step_maps[get_fragment(workflow.id)][step_fragment]["pos"]
         step = crate.add(ContextEntity(crate, step_id, properties={
             "@type": "HowToStep",
             "position": str(pos),
         }))
         tool = self.add_tool(crate, workflow, cwl_step.run)
         step["workExample"] = tool
+        if hasattr(cwl_step, "label") and cwl_step.label:
+            step["name"] = cwl_step.label
+        if hasattr(cwl_step, "doc") and cwl_step.doc:
+            step["description"] = cwl_step.doc
         workflow.append_to("step", step)
 
     def add_tool(self, crate, workflow, cwl_tool):
         if isinstance(cwl_tool, str):
             tool_fragment = get_fragment(cwl_tool)
             cwl_tool = self.cwl_defs[tool_fragment]
         else:
@@ -328,18 +374,34 @@
         tool_id = f"{self.wf_path.name}#{tool_fragment}"
         tool = crate.dereference(tool_id)
         if tool:
             return tool
         properties = {"name": tool_fragment}
         if cwl_tool.doc:
             properties["description"] = cwl_tool.doc
+        if cwl_tool.label:
+            properties["name"] = cwl_tool.label
         if hasattr(cwl_tool, "steps"):
             properties["@type"] = ["SoftwareSourceCode", "ComputationalWorkflow", "HowTo"]
         else:
             properties["@type"] = "SoftwareApplication"
+        if hasattr(cwl_tool, "intent") and cwl_tool.intent:
+            properties["featureList"] = cwl_tool.intent
+        if hasattr(cwl_tool, "requirements") and cwl_tool.requirements:
+            for req in cwl_tool.requirements:
+                if req.class_ == "ResourceRequirement":
+                    ramMin = req.ramMin
+                    if ramMin:
+                        properties["memoryRequirements"] = f"{int(ramMin)} MiB"
+        if hasattr(cwl_tool, "hints") and cwl_tool.hints:
+            for req in cwl_tool.hints:
+                if hasattr(req, "class_") and req.class_ == "ResourceRequirement":
+                    ramMin = req.ramMin
+                    if ramMin:
+                        properties["memoryRequirements"] = f"{int(ramMin)} MiB"
         tool = crate.add(ContextEntity(crate, tool_id, properties=properties))
         tool["input"] = self.add_params(crate, cwl_tool.inputs)
         tool["output"] = self.add_params(crate, cwl_tool.outputs)
         workflow.append_to("hasPart", tool)
         if hasattr(cwl_tool, "steps"):
             tool["programmingLanguage"] = workflow["programmingLanguage"]
             for s in cwl_tool.steps:
@@ -520,19 +582,24 @@
                 self.collections[main_entity.id] = action_p
             return action_p
         if "wf4ever:File" in type_names:
             hash_ = self.hashes[prov_param.id.localpart]
             dest = Path(parent.id if parent else "") / hash_
             action_p = crate.dereference(dest.as_posix())
             if not action_p:
-                source = self.root / Path("data") / hash_[:2] / hash_
+                source = self.manifest[hash_]
                 action_p = crate.add_file(source, dest, properties={
                     "sha1": hash_,
                 })
                 self._set_alternate_name(prov_param, action_p, parent=parent)
+                try:
+                    source_k = str(source.resolve(strict=False))
+                except RuntimeError:
+                    source_k = str(source)
+                self.file_map[source_k] = dest
             return action_p
         if "ro:Folder" in type_names:
             hash_ = self.hashes[prov_param.id.localpart]
             dest = Path(parent.id if parent else "") / hash_
             action_p = crate.dereference(dest.as_posix())
             if not action_p:
                 action_p = crate.add_directory(dest_path=dest)
@@ -574,30 +641,40 @@
                 o_name = get_fragment(o)
                 out_map[o_name] = o_name.replace(step_name, tool_name)
         for step in wf_def.steps:
             step_name = get_fragment(step.id)
             ro_step = crate.get(f"{self.wf_path.name}#{step_name}")
             tool_name = step_map[step_name]["tool"]
             for mapping in getattr(step, "in_", []):
-                from_param = get_fragment(mapping.source)
+                if not mapping.source:
+                    continue
+                sources = [mapping.source] if not isinstance(
+                    mapping.source, list
+                ) else mapping.source
+                for s in sources:
+                    from_param = get_fragment(s)
+                    try:
+                        from_param = out_map[from_param]
+                    except KeyError:
+                        pass  # only needed if source is from another step
+                    to_param = get_fragment(mapping.id).replace(step_name, tool_name)
+                    connect(from_param, to_param, ro_step)
+        for out in getattr(wf_def, "outputs", []):
+            out_sources = [out.outputSource] if not isinstance(
+                out.outputSource, list
+            ) else out.outputSource
+            for out_s in out_sources:
+                from_param = get_fragment(out_s)
                 try:
                     from_param = out_map[from_param]
                 except KeyError:
-                    pass  # only needed if source is from another step
-                to_param = get_fragment(mapping.id).replace(step_name, tool_name)
-                connect(from_param, to_param, ro_step)
-        for out in getattr(wf_def, "outputs", []):
-            from_param = get_fragment(out.outputSource)
-            try:
-                from_param = out_map[from_param]
-            except KeyError:
-                # assuming this is a passthrough for a workflow input parameter
-                pass
-            to_param = get_fragment(out.id)
-            connect(from_param, to_param, workflow)
+                    # assuming this is a passthrough for a workflow input parameter
+                    pass
+                to_param = get_fragment(out.id)
+                connect(from_param, to_param, workflow)
 
     def patch_workflow_input_collection(self, crate, wf=None):
         """\
         CWLProv records secondary files only in step runs, not in the workflow
         run. Thus, when the conversion of parameter values is completed,
         workflow-level parameters with secondary files get mapped to the main
         entity of the collection alone (a File). This method fixes the mapping
@@ -605,15 +682,15 @@
         execution.
         """
         if wf is None:
             wf = crate.mainEntity
         sel = [_ for _ in crate.contextual_entities
                if "CreateAction" in as_list(_.type) and _.get("instrument") is wf]
         if not sel:
-            raise RuntimeError(f"{wf.id} has no corresponding action")
+            return  # skipped subworkflow
         wf_action = sel[0]
         connections = [_ for _ in crate.contextual_entities
                        if "ParameterConnection" in as_list(_.type)]
         for param in wf.get("input", []):
             if param.get("additionalType") == "Collection":
                 src_sel = [_ for _ in wf_action.get("object", [])
                            if param in as_list(_.get("exampleOfWork"))]
@@ -640,7 +717,38 @@
                     if len(obj["exampleOfWork"]) == 1:
                         obj["exampleOfWork"] = obj["exampleOfWork"][0]
                     if len(obj["exampleOfWork"]) == 0:
                         del obj["exampleOfWork"]
         for tool in wf.get("hasPart", []):
             if "ComputationalWorkflow" in as_list(tool.type):
                 self.patch_workflow_input_collection(crate, wf=tool)
+
+    def _map_input_data(self, data):
+        if isinstance(data, list):
+            return [self._map_input_data(_) for _ in data]
+        if isinstance(data, dict):
+            rval = {}
+            for k, v in data.items():
+                if k == "location":
+                    source = self.root / "workflow" / v
+                    try:
+                        source_k = str(source.resolve(strict=False))
+                    except RuntimeError:
+                        source_k = str(source)
+                    dest = self.file_map.get(source_k)
+                    rval[k] = str(dest) if dest else v
+                else:
+                    rval[k] = self._map_input_data(v)
+            return rval
+        return data
+
+    def add_inputs_file(self, crate):
+        path = self.root / "workflow" / INPUTS_FILE_BASENAME
+        if path.is_file():
+            with open(path) as f:
+                data = json.load(f)
+            data = self._map_input_data(data)
+            source = StringIO(json.dumps(data, indent=4))
+            crate.add_file(source, path.name, properties={
+                "name": "input object document",
+                "encodingFormat": "application/json",
+            })
```

### Comparing `runcrate-0.1.2/src/runcrate/report.py` & `runcrate-0.2.0/src/runcrate/report.py`

 * *Files identical despite different names*

### Comparing `runcrate-0.1.2/src/runcrate/utils.py` & `runcrate-0.2.0/src/runcrate/utils.py`

 * *Files identical despite different names*

### Comparing `runcrate-0.1.2/src/runcrate.egg-info/PKG-INFO` & `runcrate-0.2.0/src/runcrate.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runcrate
-Version: 0.1.2
+Version: 0.2.0
 Summary: Workflow Run RO-Crate toolkit
 Home-page: https://github.com/ResearchObject/runcrate
 Author: CRS4, RO-Crate community
 Author-email: ro-crate@elixir-europe.org
 License: Apache License, version 2.0 (Apache-2.0)
 Keywords: ro-crate,workflow,provenance,CWL
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `runcrate-0.1.2/src/runcrate.egg-info/SOURCES.txt` & `runcrate-0.2.0/src/runcrate.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/reference/index.rst
 docs/reference/main.rst
 src/runcrate/__init__.py
 src/runcrate/cli.py
 src/runcrate/constants.py
 src/runcrate/convert.py
 src/runcrate/report.py
+src/runcrate/run.py
 src/runcrate/utils.py
 src/runcrate.egg-info/PKG-INFO
 src/runcrate.egg-info/SOURCES.txt
 src/runcrate.egg-info/dependency_links.txt
 src/runcrate.egg-info/entry_points.txt
 src/runcrate.egg-info/not-zip-safe
 src/runcrate.egg-info/requires.txt
```

