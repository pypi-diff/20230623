# Comparing `tmp/pypfb-0.5.8.tar.gz` & `tmp/pypfb-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypfb-0.5.8.tar", last modified: Wed Feb 24 18:26:18 2021, max compression
+gzip compressed data, was "pypfb-0.5.9.tar", max compression
```

## Comparing `pypfb-0.5.8.tar` & `pypfb-0.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11358 2021-02-24 18:24:58.492251 pypfb-0.5.8/LICENSE
--rw-r--r--   0        0        0     1133 2021-02-24 18:24:58.492251 pypfb-0.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/__init__.py
--rw-r--r--   0        0        0     5385 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/base.py
--rw-r--r--   0        0        0     1406 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/cli.py
--rw-r--r--   0        0        0        0 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/commands/__init__.py
--rw-r--r--   0        0        0     1785 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/commands/add.py
--rw-r--r--   0        0        0      689 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/commands/etl.py
--rw-r--r--   0        0        0     5132 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/commands/import.py
--rw-r--r--   0        0        0     2256 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/commands/rename.py
--rw-r--r--   0        0        0     3262 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/commands/show.py
--rw-r--r--   0        0        0        0 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/etl/__init__.py
--rw-r--r--   0        0        0     7447 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/etl/etl.py
--rw-r--r--   0        0        0        0 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/exporters/__init__.py
--rw-r--r--   0        0        0     4472 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/exporters/gremlin.py
--rw-r--r--   0        0        0     4846 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/exporters/tsv.py
--rw-r--r--   0        0        0        0 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/importers/__init__.py
--rw-r--r--   0        0        0     9853 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/importers/gen3dict.py
--rw-r--r--   0        0        0     3392 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/importers/json.py
--rw-r--r--   0        0        0     4028 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/importers/tsv.py
--rw-r--r--   0        0        0     1320 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/reader.py
--rw-r--r--   0        0        0    12519 2021-02-24 18:24:58.492251 pypfb-0.5.8/src/pfb/writer.py
--rw-r--r--   0        0        0     1665 2021-02-24 18:26:18.484396 pypfb-0.5.8/setup.py
--rw-r--r--   0        0        0      804 2021-02-24 18:26:18.484751 pypfb-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-05-05 21:09:49.757073 pypfb-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1113 2021-05-05 21:09:49.761073 pypfb-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/__init__.py
+-rw-r--r--   0        0        0     5390 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/base.py
+-rw-r--r--   0        0        0     1406 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/cli.py
+-rw-r--r--   0        0        0        0 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/commands/__init__.py
+-rw-r--r--   0        0        0     1785 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/commands/add.py
+-rw-r--r--   0        0        0      689 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/commands/etl.py
+-rw-r--r--   0        0        0     5132 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/commands/import.py
+-rw-r--r--   0        0        0     2256 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/commands/rename.py
+-rw-r--r--   0        0        0     3262 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/commands/show.py
+-rw-r--r--   0        0        0        0 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/etl/__init__.py
+-rw-r--r--   0        0        0     7447 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/etl/etl.py
+-rw-r--r--   0        0        0        0 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/exporters/__init__.py
+-rw-r--r--   0        0        0     4472 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/exporters/gremlin.py
+-rw-r--r--   0        0        0     4917 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/exporters/tsv.py
+-rw-r--r--   0        0        0        0 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/importers/__init__.py
+-rw-r--r--   0        0        0     9853 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/importers/gen3dict.py
+-rw-r--r--   0        0        0     3392 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/importers/json.py
+-rw-r--r--   0        0        0     4405 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/importers/tsv.py
+-rw-r--r--   0        0        0     1320 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/reader.py
+-rw-r--r--   0        0        0    12531 2021-05-05 21:09:49.761073 pypfb-0.5.9/src/pfb/writer.py
+-rw-r--r--   0        0        0     1638 2021-05-05 21:11:02.896333 pypfb-0.5.9/setup.py
+-rw-r--r--   0        0        0      813 2021-05-05 21:11:02.896677 pypfb-0.5.9/PKG-INFO
```

### Comparing `pypfb-0.5.8/LICENSE` & `pypfb-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/pyproject.toml` & `pypfb-0.5.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.poetry]
 name = "pypfb"
-version = "0.5.8"
+version = "0.5.9"
 description = "Python SDK for PFB format"
 authors = ["CTDS UChicago <cdis@uchicago.edu>"]
 license = "Apache-2.0"
 packages = [
     { include = "pfb", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6.1,<3.8"
+python = ">=3.6,<3.8"
 click = "^7.1.2"
 fastavro = "^1.0.0"
 python-json-logger = "^0.1.11"
 PyYAML = "^5.3.1"
 importlib_metadata = { version = "^1.3.0", python = "<3.8" }
 gdcdictionary = "^1.2.0"
-pandas = "^1.1.0"
 aiohttp = "^3.6.3"
 dictionaryutils = "^3.2.0"
 gen3 = "^4.2.0"
 
 [tool.poetry.dev-dependencies]
 codacy-coverage = "*"
 pytest = "~=3.2"
```

### Comparing `pypfb-0.5.8/src/pfb/base.py` & `pypfb-0.5.9/src/pfb/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     unicodeRep = unicodeRep.encode().decode("unicode_escape")
     return unicodeRep
 
 
 def encode_enum(enumValue):
     encodedValue = re.sub(
-        "^[0-9]|[^A-Za-z0-9]", unicode_encode, enumValue, flags=re.UNICODE
+        "^[0-9]|[^A-Za-z0-9]", unicode_encode, str(enumValue), flags=re.UNICODE
     )
     return encodedValue
 
 
 def decode_enum(enumValue):
     decodedValue = re.sub("_[a-z0-9]+_", unicode_decode, enumValue, flags=re.UNICODE)
     return decodedValue
```

### Comparing `pypfb-0.5.8/src/pfb/cli.py` & `pypfb-0.5.9/src/pfb/cli.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/commands/add.py` & `pypfb-0.5.9/src/pfb/commands/add.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/commands/etl.py` & `pypfb-0.5.9/src/pfb/commands/etl.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/commands/import.py` & `pypfb-0.5.9/src/pfb/commands/import.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/commands/rename.py` & `pypfb-0.5.9/src/pfb/commands/rename.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/commands/show.py` & `pypfb-0.5.9/src/pfb/commands/show.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/etl/etl.py` & `pypfb-0.5.9/src/pfb/etl/etl.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/exporters/gremlin.py` & `pypfb-0.5.9/src/pfb/exporters/gremlin.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/exporters/tsv.py` & `pypfb-0.5.9/src/pfb/exporters/tsv.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         bold=True,
     )
     click.secho(output, fg="white", err=True, bold=True)
 
 
 node_submitter_ids = {}
 
+
 def _to_tsv(reader, dir_path, handlers_by_name):
     project_ids = []
     num_files = 1
 
     if not os.path.exists(dir_path):
         os.mkdir(dir_path)
 
@@ -56,56 +57,46 @@
                 for (index, d) in enumerate(reader.metadata["nodes"])
                 if d["name"] == name
             )
         )
 
         obj = row["object"]
 
-
         if "submitter_id" in obj:
             node_submitter_ids[record_id] = obj["submitter_id"]
 
-        if {
-            "name": "id",
-            "type": ["null", "string"],
-        } not in fields:
+        if {"name": "id", "type": ["null", "string"],} not in fields:
             fields.append(
-                {
-                    "name": "id",
-                    "type": ["null", "string"],
-                }
+                {"name": "id", "type": ["null", "string"],}
             )
 
         obj["id"] = record_id
 
-
         for r in row["relations"]:
             parent_node = r["dst_name"]
             parent_id = r["dst_id"]
 
             for node in reader.metadata["nodes"]:
                 if node["name"] == name:
                     for link in node["links"]:
                         if link["dst"] == parent_node:
                             plural_parent = link["name"]
+                        # already in plural form
+                        elif link["name"] == parent_node:
+                            plural_parent = parent_node
             if {
                 "name": plural_parent + ".id",
                 "type": ["null", "string"],
             } not in fields:
                 fields.append(
-                    {
-                        "name": plural_parent + ".id",
-                        "type": ["null", "string"],
-                    }
+                    {"name": plural_parent + ".id", "type": ["null", "string"],}
                 )
 
             obj[plural_parent + ".id"] = r["dst_id"]
-            
 
-            
             if {
                 "name": plural_parent + ".submitter_id",
                 "type": ["null", "string"],
             } not in fields:
                 fields.append(
                     {
                         "name": plural_parent + ".submitter_id",
@@ -114,20 +105,17 @@
                 )
 
             if parent_id in node_submitter_ids:
                 obj[plural_parent + ".submitter_id"] = node_submitter_ids[parent_id]
             else:
                 obj[plural_parent + ".submitter_id"] = "null"
 
-
         if "sample" in node_submitter_ids:
             print(node_submitter_ids["sample"])
 
-
-
         # get the TSV writer for this row, create one if not created
         pair = handlers_by_name.get(name)
         if pair is None:
             header_row = _make_header_row(fields)
             path = os.path.join(dir_path, name + ".tsv")
             click.secho("Creating ", fg="blue", err=True, nl=False)
             click.secho(path, fg="white", err=True)
@@ -143,15 +131,20 @@
         data_row = [name]
         for field in fields:
             if field["name"] == "project_id":
                 project_ids.append([name, obj["project_id"]])
                 data_row.append(obj[field["name"]])
             else:
                 # adding logic for multi-sample records that contain either project.submitter_id or samplie.submitter_id
-                if field["name"] == "samples.id" or field["name"] == "projects.id" or field["name"] == "samples.submitter_id" or field["name"] == "projects.submitter_id":
+                if (
+                    field["name"] == "samples.id"
+                    or field["name"] == "projects.id"
+                    or field["name"] == "samples.submitter_id"
+                    or field["name"] == "projects.submitter_id"
+                ):
                     if field["name"] not in obj:
                         continue
                 value = obj[field["name"]]
                 data_row.append(value)
 
         w.writerow(data_row)
```

### Comparing `pypfb-0.5.8/src/pfb/importers/gen3dict.py` & `pypfb-0.5.9/src/pfb/importers/gen3dict.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/importers/json.py` & `pypfb-0.5.9/src/pfb/importers/json.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/importers/tsv.py` & `pypfb-0.5.9/src/pfb/importers/tsv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import absolute_import
 
 import glob
-import pandas as pd
 import os
+import csv
 
 import click
 
 from ..base import avro_record
 from ..cli import from_command
 from ..reader import PFBReader
 
@@ -62,28 +62,47 @@
     total = len(order)
 
     for i, o in enumerate(order):
         o = os.path.basename(o).replace(".tsv", "").strip()
         click.secho("{}/{}: ".format(i + 1, total), fg="blue", nl=False, err=True)
         click.secho(o, fg="white", err=True)
 
-        tsv_data = pd.read_csv(
-            os.path.join(path, o + ".tsv"), delimiter="\t", index_col=1
+        tsv_data = list(
+            csv.DictReader(open(os.path.join(path, o + ".tsv")), delimiter="\t")
         )
-        tsv_data = tsv_data.where(pd.notnull(tsv_data), None).to_dict(orient="records")
 
         node_name = o
 
         if isinstance(tsv_data, dict):
             tsv_data = [tsv_data]
         for tsv_record in tsv_data:
+            for k, v in tsv_record.items():
+                tsv_record[k] = convert_types(v)
             record = _convert_tsv(node_name, tsv_record, program, project, link_dests)
             yield record
 
 
+def convert_types(val):
+    if val is None or val.strip() == "":
+        return None
+    if val.lower() == "false":
+        return False
+    if val.lower() == "true":
+        return True
+    try:
+        v = float(val)
+        # for fields that require type long
+        if int(v) == v:
+            v = int(v)
+        return v
+    except ValueError:
+        pass
+    return val
+
+
 def _convert_tsv(node_name, tsv_record, program, project, link_dests):
     relations = []
     try:
         node_id = tsv_record["submitter_id"]
     except KeyError:
         if node_name == "program":
             node_id = tsv_record["dbgap_accession_number"]
@@ -99,15 +118,15 @@
             v = item
             relations.append(
                 {
                     "dst_id": tsv_record[item]["submitter_id"],
                     "dst_name": link_dests[node_name][v],
                 }
             )
-        # array typeing being passed off as string
+        # array typing being passed off as string
         if (
             type(tsv_record[item]) == str
             and "[" in tsv_record[item]
             and "]" in tsv_record[item]
         ):
             arrayStrip = tsv_record[item].strip("[']")
             vals[item] = arrayStrip.split(",")
```

### Comparing `pypfb-0.5.8/src/pfb/reader.py` & `pypfb-0.5.9/src/pfb/reader.py`

 * *Files identical despite different names*

### Comparing `pypfb-0.5.8/src/pfb/writer.py` & `pypfb-0.5.9/src/pfb/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
                     name = record["name"]
                     record["object"] = (name, obj)
                     for hook in self._hooks:
                         record = hook(record)
 
                     to_update = {}
                     for field, value in list(obj.items()):
-                        if value and self.is_encode(name, field):
+                        if value is not None and self.is_encode(name, field):
                             obj[field] = encode_enum(value)
                     obj.update(to_update)
                     yield record
 
         writer(self._file_obj, make_avro_schema(self.schema), _iter())
 
     def rename_node(self, name_from, name_to):
```

### Comparing `pypfb-0.5.8/setup.py` & `pypfb-0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 ['PyYAML>=5.3.1,<6.0.0',
  'aiohttp>=3.6.3,<4.0.0',
  'click>=7.1.2,<8.0.0',
  'dictionaryutils>=3.2.0,<4.0.0',
  'fastavro>=1.0.0,<2.0.0',
  'gdcdictionary>=1.2.0,<2.0.0',
  'gen3>=4.2.0,<5.0.0',
- 'pandas>=1.1.0,<2.0.0',
  'python-json-logger>=0.1.11,<0.2.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=1.3.0,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['pfb = pfb.cli:main'],
@@ -35,26 +34,26 @@
                  'rename = pfb.commands.rename',
                  'show = pfb.commands.show',
                  'to_gremlin = pfb.exporters.gremlin',
                  'to_tsv = pfb.exporters.tsv']}
 
 setup_kwargs = {
     'name': 'pypfb',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'Python SDK for PFB format',
     'long_description': None,
     'author': 'CTDS UChicago',
     'author_email': 'cdis@uchicago.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.1,<3.8',
+    'python_requires': '>=3.6,<3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pypfb-0.5.8/PKG-INFO` & `pypfb-0.5.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pypfb
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python SDK for PFB format
 License: Apache-2.0
 Author: CTDS UChicago
 Author-email: cdis@uchicago.edu
-Requires-Python: >=3.6.1,<3.8
+Requires-Python: >=3.6,<3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: PyYAML (>=5.3.1,<6.0.0)
 Requires-Dist: aiohttp (>=3.6.3,<4.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: dictionaryutils (>=3.2.0,<4.0.0)
 Requires-Dist: fastavro (>=1.0.0,<2.0.0)
 Requires-Dist: gdcdictionary (>=1.2.0,<2.0.0)
 Requires-Dist: gen3 (>=4.2.0,<5.0.0)
 Requires-Dist: importlib_metadata (>=1.3.0,<2.0.0); python_version < "3.8"
-Requires-Dist: pandas (>=1.1.0,<2.0.0)
 Requires-Dist: python-json-logger (>=0.1.11,<0.2.0)
```

