# Comparing `tmp/pystructurizr-0.1.1.tar.gz` & `tmp/pystructurizr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructurizr-0.1.1.tar", last modified: Sun Jun 18 09:58:37 2023, max compression
+gzip compressed data, was "pystructurizr-0.1.2.tar", last modified: Fri Jun 23 21:02:17 2023, max compression
```

## Comparing `pystructurizr-0.1.1.tar` & `pystructurizr-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.675823 pystructurizr-0.1.1/
--rw-r--r--   0 niels      (501) staff       (20)     1091 2023-06-15 21:03:41.000000 pystructurizr-0.1.1/LICENSE.txt
--rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-18 09:58:37.675407 pystructurizr-0.1.1/PKG-INFO
--rw-r--r--   0 niels      (501) staff       (20)     3417 2023-06-15 21:10:05.000000 pystructurizr-0.1.1/README.md
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.664757 pystructurizr-0.1.1/example/
--rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:48:57.000000 pystructurizr-0.1.1/example/__init__.py
--rw-r--r--   0 niels      (501) staff       (20)     2492 2023-06-18 09:38:04.000000 pystructurizr-0.1.1/example/analysissystem.py
--rw-r--r--   0 niels      (501) staff       (20)      286 2023-06-18 09:39:00.000000 pystructurizr-0.1.1/example/analysisystem_containerview.py
--rw-r--r--   0 niels      (501) staff       (20)      197 2023-06-18 09:39:15.000000 pystructurizr-0.1.1/example/chatserver_componentview.py
--rw-r--r--   0 niels      (501) staff       (20)     1060 2023-06-17 18:06:20.000000 pystructurizr-0.1.1/example/chatsystem.py
--rw-r--r--   0 niels      (501) staff       (20)      194 2023-06-18 09:39:26.000000 pystructurizr-0.1.1/example/chatsystem_containerview.py
--rw-r--r--   0 niels      (501) staff       (20)      163 2023-06-11 13:15:48.000000 pystructurizr-0.1.1/example/systemlandscapeview.py
--rw-r--r--   0 niels      (501) staff       (20)      315 2023-06-17 10:47:22.000000 pystructurizr-0.1.1/example/users.py
--rw-r--r--   0 niels      (501) staff       (20)      606 2023-06-17 18:12:09.000000 pystructurizr-0.1.1/example/workspace.py
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.670364 pystructurizr-0.1.1/pystructurizr/
--rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:49:07.000000 pystructurizr-0.1.1/pystructurizr/__init__.py
--rw-r--r--   0 niels      (501) staff       (20)     3469 2023-06-18 09:28:43.000000 pystructurizr-0.1.1/pystructurizr/cli.py
--rw-r--r--   0 niels      (501) staff       (20)     1937 2023-06-18 09:29:38.000000 pystructurizr-0.1.1/pystructurizr/cli_helper.py
--rw-r--r--   0 niels      (501) staff       (20)     2251 2023-06-17 20:24:22.000000 pystructurizr-0.1.1/pystructurizr/cli_watcher.py
--rw-r--r--   0 niels      (501) staff       (20)     2516 2023-06-17 20:29:47.000000 pystructurizr-0.1.1/pystructurizr/cloudstorage.py
--rw-r--r--   0 niels      (501) staff       (20)    12123 2023-06-17 20:41:33.000000 pystructurizr-0.1.1/pystructurizr/dsl.py
--rw-r--r--   0 niels      (501) staff       (20)      249 2023-06-17 11:06:39.000000 pystructurizr-0.1.1/pystructurizr/index.html
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.673808 pystructurizr-0.1.1/pystructurizr.egg-info/
--rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/PKG-INFO
--rw-r--r--   0 niels      (501) staff       (20)      699 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/SOURCES.txt
--rw-r--r--   0 niels      (501) staff       (20)        1 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/dependency_links.txt
--rw-r--r--   0 niels      (501) staff       (20)       57 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/entry_points.txt
--rw-r--r--   0 niels      (501) staff       (20)       80 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/requires.txt
--rw-r--r--   0 niels      (501) staff       (20)       22 2023-06-18 09:58:37.000000 pystructurizr-0.1.1/pystructurizr.egg-info/top_level.txt
--rw-r--r--   0 niels      (501) staff       (20)       38 2023-06-18 09:58:37.675961 pystructurizr-0.1.1/setup.cfg
--rw-r--r--   0 niels      (501) staff       (20)     1271 2023-06-18 09:55:27.000000 pystructurizr-0.1.1/setup.py
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-18 09:58:37.674396 pystructurizr-0.1.1/test/
--rw-r--r--   0 niels      (501) staff       (20)      675 2023-06-17 20:47:58.000000 pystructurizr-0.1.1/test/test_cli.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.039086 pystructurizr-0.1.2/
+-rw-r--r--   0 niels      (501) staff       (20)     1091 2023-06-15 21:03:41.000000 pystructurizr-0.1.2/LICENSE.txt
+-rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-23 21:02:17.038572 pystructurizr-0.1.2/PKG-INFO
+-rw-r--r--   0 niels      (501) staff       (20)     3417 2023-06-15 21:10:05.000000 pystructurizr-0.1.2/README.md
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.026063 pystructurizr-0.1.2/example/
+-rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:48:57.000000 pystructurizr-0.1.2/example/__init__.py
+-rw-r--r--   0 niels      (501) staff       (20)     2492 2023-06-18 09:38:04.000000 pystructurizr-0.1.2/example/analysissystem.py
+-rw-r--r--   0 niels      (501) staff       (20)      286 2023-06-18 09:39:00.000000 pystructurizr-0.1.2/example/analysisystem_containerview.py
+-rw-r--r--   0 niels      (501) staff       (20)      197 2023-06-18 09:39:15.000000 pystructurizr-0.1.2/example/chatserver_componentview.py
+-rw-r--r--   0 niels      (501) staff       (20)     1060 2023-06-17 18:06:20.000000 pystructurizr-0.1.2/example/chatsystem.py
+-rw-r--r--   0 niels      (501) staff       (20)      194 2023-06-18 09:39:26.000000 pystructurizr-0.1.2/example/chatsystem_containerview.py
+-rw-r--r--   0 niels      (501) staff       (20)      163 2023-06-11 13:15:48.000000 pystructurizr-0.1.2/example/systemlandscapeview.py
+-rw-r--r--   0 niels      (501) staff       (20)      315 2023-06-17 10:47:22.000000 pystructurizr-0.1.2/example/users.py
+-rw-r--r--   0 niels      (501) staff       (20)      606 2023-06-17 18:12:09.000000 pystructurizr-0.1.2/example/workspace.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.030977 pystructurizr-0.1.2/pystructurizr/
+-rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:49:07.000000 pystructurizr-0.1.2/pystructurizr/__init__.py
+-rw-r--r--   0 niels      (501) staff       (20)     3465 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/cli.py
+-rw-r--r--   0 niels      (501) staff       (20)     1323 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/cli_helper.py
+-rw-r--r--   0 niels      (501) staff       (20)     2251 2023-06-17 20:24:22.000000 pystructurizr-0.1.2/pystructurizr/cli_watcher.py
+-rw-r--r--   0 niels      (501) staff       (20)     2516 2023-06-17 20:29:47.000000 pystructurizr-0.1.2/pystructurizr/cloudstorage.py
+-rw-r--r--   0 niels      (501) staff       (20)    12129 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/dsl.py
+-rw-r--r--   0 niels      (501) staff       (20)     1021 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/generator.py
+-rw-r--r--   0 niels      (501) staff       (20)      249 2023-06-17 11:06:39.000000 pystructurizr-0.1.2/pystructurizr/index.html
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.036479 pystructurizr-0.1.2/pystructurizr.egg-info/
+-rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/PKG-INFO
+-rw-r--r--   0 niels      (501) staff       (20)      726 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/SOURCES.txt
+-rw-r--r--   0 niels      (501) staff       (20)        1 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/dependency_links.txt
+-rw-r--r--   0 niels      (501) staff       (20)       57 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/entry_points.txt
+-rw-r--r--   0 niels      (501) staff       (20)       80 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/requires.txt
+-rw-r--r--   0 niels      (501) staff       (20)       22 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/top_level.txt
+-rw-r--r--   0 niels      (501) staff       (20)       38 2023-06-23 21:02:17.039266 pystructurizr-0.1.2/setup.cfg
+-rw-r--r--   0 niels      (501) staff       (20)     1271 2023-06-23 21:01:37.000000 pystructurizr-0.1.2/setup.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.037453 pystructurizr-0.1.2/test/
+-rw-r--r--   0 niels      (501) staff       (20)      675 2023-06-17 20:47:58.000000 pystructurizr-0.1.2/test/test_cli.py
```

### Comparing `pystructurizr-0.1.1/LICENSE.txt` & `pystructurizr-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.1/PKG-INFO` & `pystructurizr-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructurizr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python DSL inspired by Structurizr, intended for generating C4 diagrams
 Home-page: https://github.com/nielsvanspauwen/pystructurizr
 Author: Niels Vanspauwen
 Author-email: niels.vanspauwen@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pystructurizr-0.1.1/README.md` & `pystructurizr-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.1/example/analysissystem.py` & `pystructurizr-0.1.2/example/analysissystem.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.1/example/chatsystem.py` & `pystructurizr-0.1.2/example/chatsystem.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.1/example/workspace.py` & `pystructurizr-0.1.2/example/workspace.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.1/pystructurizr/cli.py` & `pystructurizr-0.1.2/pystructurizr/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,95 +2,92 @@
 import json
 import os
 import shutil
 import subprocess
 
 import click
 
-from .cli_helper import (ensure_tmp_folder_exists, generate_diagram_code,
-                         generate_diagram_code_in_child_process, generate_svg)
+from .cli_helper import (ensure_tmp_folder_exists, generate_diagram_code_in_child_process, generate_svg)
 from .cli_watcher import observe_modules
 from .cloudstorage import CloudStorage, create_cloud_storage
 
 
 @click.command()
 @click.option('--view', prompt='Your view file (e.g. example.componentview)',
               help='The view file to generate.')
 @click.option('--as-json', is_flag=True, default=False,
               help='Dumps the generated code and the imported modules as a json object')
 def dump(view, as_json):
-    diagram_code, imported_modules = generate_diagram_code(view)
+    diagram_code, imported_modules = generate_diagram_code_in_child_process(view)
     if as_json:
         print(json.dumps({
             "code": diagram_code,
             "imported_modules": list(imported_modules)
         }))
     else:
         print(diagram_code)
 
 
-
 @click.command()
 @click.option('--view', prompt='Your view file (e.g. example.componentview)',
               help='The view file to develop.')
 def dev(view):
     click.echo(f"Setting up live preview of view {view}...")
     # Prep the /tmp/pystructurizr folder
     tmp_folder = ensure_tmp_folder_exists()
     current_script_path = os.path.abspath(__file__)
     index_html = os.path.join(os.path.dirname(current_script_path), 'index.html')
     shutil.copy(index_html, f"{tmp_folder}/index.html")
 
     async def async_behavior():
         print("Generating diagram...")
-        result = generate_diagram_code_in_child_process(view)
-        await generate_svg(result['code'], tmp_folder)
-        return result['imported_modules']
+        diagram_code, imported_modules = generate_diagram_code_in_child_process(view)
+        await generate_svg(diagram_code, tmp_folder)
+        return imported_modules
 
     async def observe_loop():
         modules_to_watch = await async_behavior()
         click.echo("Launching webserver...")
         # pylint: disable=consider-using-with
         subprocess.Popen(f"httpwatcher --root {tmp_folder} --watch {tmp_folder}", shell=True)
         await observe_modules(modules_to_watch, async_behavior)
 
     asyncio.run(observe_loop())
 
 
-
 @click.command()
 @click.option('--view', prompt='Your view file (e.g. example.componentview)',
               help='The view file to generate and upload to cloud storage.')
 @click.option('--gcs-credentials', prompt='Path to json file containing Google Cloud Storage credentials', type=click.Path(exists=True),
               help='Path to the credentials.json file for Google Cloud Storage.')
 @click.option('--bucket-name', prompt='Name of the bucket on Google Cloud Storage',
               help='The name of the bucket to use on Google Cloud Storage.')
 @click.option('--object-name', prompt='Name of the object on Google Cloud Storage',
               help='The name of the object to use on Google Cloud Storage.')
 def build(view, gcs_credentials, bucket_name, object_name):
     async def async_behavior():
         # Generate diagram
-        diagram_code, _ = generate_diagram_code(view)
+        diagram_code, _ = generate_diagram_code_in_child_process(view)
         tmp_folder = ensure_tmp_folder_exists()
 
         # Generate SVG
         svg_file_path = await generate_svg(diagram_code, tmp_folder)
 
         # Upload it to the requested cloud storage provider
         cloud_storage = create_cloud_storage(CloudStorage.Provider.GCS, gcs_credentials)
         svg_file_url = cloud_storage.upload_file(svg_file_path, bucket_name, object_name)
         print(svg_file_url)
 
     asyncio.run(async_behavior())
 
 
-
 @click.group()
 def cli():
     pass
 
+
 cli.add_command(dump)
 cli.add_command(dev)
 cli.add_command(build)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `pystructurizr-0.1.1/pystructurizr/cli_watcher.py` & `pystructurizr-0.1.2/pystructurizr/cli_watcher.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.1/pystructurizr/cloudstorage.py` & `pystructurizr-0.1.2/pystructurizr/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.1/pystructurizr/dsl.py` & `pystructurizr-0.1.2/pystructurizr/dsl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import keyword
 import re
 from enum import Enum
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 
 # pylint: disable=too-few-public-methods
 class Identifier:
     counter = {}
 
     @staticmethod
@@ -249,15 +249,15 @@
             dumper.add(f'exclude {exclude.instname}')
         dumper.add('autoLayout')
         dumper.outdent()
         dumper.add('}')
 
 
 class Style:
-    def __init__(self, style_map: dict[str, str]):
+    def __init__(self, style_map: Dict[str, str]):
         self.map = style_map
 
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'element "{self.map["tag"]}" {{')
         dumper.indent()
         for key, value in self.map.items():
             if key == "tag":
@@ -361,10 +361,10 @@
     # pylint: disable=invalid-name
     def ComponentView(self, element: Element, name: str, description: str):
         view = View(View.Kind.COMPONENT, element, name, description)
         self.views.append(view)
         return view
 
     # pylint: disable=invalid-name
-    def Styles(self, *styles: dict[str, str]) -> None:
+    def Styles(self, *styles: Dict[str, str]) -> None:
         for style in styles:
             self.styles.append(Style(style))
```

### Comparing `pystructurizr-0.1.1/pystructurizr.egg-info/PKG-INFO` & `pystructurizr-0.1.2/pystructurizr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructurizr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python DSL inspired by Structurizr, intended for generating C4 diagrams
 Home-page: https://github.com/nielsvanspauwen/pystructurizr
 Author: Niels Vanspauwen
 Author-email: niels.vanspauwen@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pystructurizr-0.1.1/pystructurizr.egg-info/SOURCES.txt` & `pystructurizr-0.1.2/pystructurizr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 example/workspace.py
 pystructurizr/__init__.py
 pystructurizr/cli.py
 pystructurizr/cli_helper.py
 pystructurizr/cli_watcher.py
 pystructurizr/cloudstorage.py
 pystructurizr/dsl.py
+pystructurizr/generator.py
 pystructurizr/index.html
 pystructurizr.egg-info/PKG-INFO
 pystructurizr.egg-info/SOURCES.txt
 pystructurizr.egg-info/dependency_links.txt
 pystructurizr.egg-info/entry_points.txt
 pystructurizr.egg-info/requires.txt
 pystructurizr.egg-info/top_level.txt
```

### Comparing `pystructurizr-0.1.1/setup.py` & `pystructurizr-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pystructurizr',
-    version='0.1.1',
+    version='0.1.2',
     description='A Python DSL inspired by Structurizr, intended for generating C4 diagrams',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Niels Vanspauwen',
     author_email='niels.vanspauwen@gmail.com',
     license='MIT',
     url='https://github.com/nielsvanspauwen/pystructurizr',
```

### Comparing `pystructurizr-0.1.1/test/test_cli.py` & `pystructurizr-0.1.2/test/test_cli.py`

 * *Files identical despite different names*

