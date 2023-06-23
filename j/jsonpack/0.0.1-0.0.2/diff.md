# Comparing `tmp/jsonpack-0.0.1.tar.gz` & `tmp/jsonpack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonpack-0.0.1.tar", last modified: Wed Jun 14 18:57:40 2023, max compression
+gzip compressed data, was "jsonpack-0.0.2.tar", last modified: Fri Jun 23 20:09:36 2023, max compression
```

## Comparing `jsonpack-0.0.1.tar` & `jsonpack-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 18:57:40.355902 jsonpack-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-08 19:11:57.000000 jsonpack-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1383 2023-06-14 18:57:40.355902 jsonpack-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      675 2023-06-08 19:18:23.000000 jsonpack-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 18:57:40.348818 jsonpack-0.0.1/jsonpack/
--rw-rw-rw-   0        0        0    49747 2023-06-08 19:46:06.000000 jsonpack-0.0.1/jsonpack/__init__.py
--rw-rw-rw-   0        0        0       33 2023-06-05 16:58:37.000000 jsonpack-0.0.1/jsonpack/exceptions.py
--rw-rw-rw-   0        0        0     6053 2023-06-06 23:24:58.000000 jsonpack-0.0.1/jsonpack/node.py
--rw-rw-rw-   0        0        0     3532 2023-06-06 23:40:21.000000 jsonpack-0.0.1/jsonpack/util.py
-drwxrwxrwx   0        0        0        0 2023-06-14 18:57:40.354903 jsonpack-0.0.1/jsonpack.egg-info/
--rw-rw-rw-   0        0        0     1383 2023-06-14 18:57:40.000000 jsonpack-0.0.1/jsonpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-06-14 18:57:40.000000 jsonpack-0.0.1/jsonpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 18:57:40.000000 jsonpack-0.0.1/jsonpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 18:57:40.000000 jsonpack-0.0.1/jsonpack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-14 18:57:40.356903 jsonpack-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1119 2023-06-08 19:51:57.000000 jsonpack-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:09:36.518267 jsonpack-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-08 19:11:57.000000 jsonpack-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1603 2023-06-23 20:09:36.519268 jsonpack-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      885 2023-06-17 06:56:08.000000 jsonpack-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 20:09:36.489268 jsonpack-0.0.2/jsonpack/
+-rw-rw-rw-   0        0        0    64422 2023-06-23 20:08:58.000000 jsonpack-0.0.2/jsonpack/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-06-05 16:58:37.000000 jsonpack-0.0.2/jsonpack/exceptions.py
+-rw-rw-rw-   0        0        0     6098 2023-06-23 15:08:46.000000 jsonpack-0.0.2/jsonpack/node.py
+-rw-rw-rw-   0        0        0     5133 2023-06-23 16:36:55.000000 jsonpack-0.0.2/jsonpack/util.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:09:36.518267 jsonpack-0.0.2/jsonpack.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-06-23 20:09:36.000000 jsonpack-0.0.2/jsonpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-23 20:09:36.000000 jsonpack-0.0.2/jsonpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:09:36.000000 jsonpack-0.0.2/jsonpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 20:09:36.000000 jsonpack-0.0.2/jsonpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 20:09:36.000000 jsonpack-0.0.2/jsonpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-23 20:09:36.519268 jsonpack-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1143 2023-06-23 20:08:50.000000 jsonpack-0.0.2/setup.py
```

### Comparing `jsonpack-0.0.1/LICENSE` & `jsonpack-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpack-0.0.1/PKG-INFO` & `jsonpack-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: jsonpack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Easily create JSON packs for your Python Application.
 Home-page: https://github.com/legopitstop/jsonpack
 Author: Legopitstop
 Author-email: officiallegopitstop@gmail.com
 License: MIT
-Keywords: json,pack,manifest,scripts,events,components,Pillow
+Keywords: json,pack,manifest,scripts,events,components,Pillow,schemaser
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jsonpack
 This library allows you to create packs using JSON files to configure your Python Application.
 
+## Install
+```
+pip install jsonpack
+```
+
 ## Features
 - Supports JSON, YAML, ZIP and most image formats
 - Includes the loading of Python files from packs to easily expand your app's features
 - Easily reload all packs without having to restart your application.
 - JSON and YAML validation to make sure your file is properly configured.
 
 See the docs for more information.
 
 ## Optional Dependencies
 |Name|Required|Description|
 |--|--|--|
 |[Pillow](https://pypi.org/project/Pillow/) | No | For image/* mimetypes |
 |[PyYAML](https://pypi.org/project/PyYAML/) | No | For application/yaml mimetype |
+|[opencv-python](https://pypi.org/project/opencv-python/) | No | For video/* mimetype |
+|[pygame](https://pypi.org/project/pygame/) | No | For audio/* mimetype |
```

### Comparing `jsonpack-0.0.1/README.md` & `jsonpack-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # jsonpack
 This library allows you to create packs using JSON files to configure your Python Application.
 
+## Install
+```
+pip install jsonpack
+```
+
 ## Features
 - Supports JSON, YAML, ZIP and most image formats
 - Includes the loading of Python files from packs to easily expand your app's features
 - Easily reload all packs without having to restart your application.
 - JSON and YAML validation to make sure your file is properly configured.
 
 See the docs for more information.
 
 ## Optional Dependencies
 |Name|Required|Description|
 |--|--|--|
 |[Pillow](https://pypi.org/project/Pillow/) | No | For image/* mimetypes |
 |[PyYAML](https://pypi.org/project/PyYAML/) | No | For application/yaml mimetype |
+|[opencv-python](https://pypi.org/project/opencv-python/) | No | For video/* mimetype |
+|[pygame](https://pypi.org/project/pygame/) | No | For audio/* mimetype |
```

### Comparing `jsonpack-0.0.1/jsonpack/node.py` & `jsonpack-0.0.2/jsonpack/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import jsonpack
+import asyncio
 
 class NodeProxy:
     def __init__(self, layer: dict):
         self.__dict__.update(layer)
 
     def __len__(self) -> int:
         return len(self.__dict__)
@@ -21,15 +22,15 @@
     """
     Helper class used for creating nodes.
 
     Methods
     ---
     to_dict, from_dict, on_load, on_unload, __str__
     """
-    traits = {}
+    traits = []
     __slots__ = []
     __file__ = None
 
     def __init__(self):
         self._app = None
 
     def to_dict(self):
@@ -112,29 +113,29 @@
         Argumnets
         ---
         `name` - Name of the component to get.
         """
         res = self._components.get(name)
         if res is not None: return NodeProxy(res)
 
-    def trigger_component(self, name:str, **extra):
+    async def trigger_component(self, name:str, **extra):
         """
         Returns the result of the component function when called.
 
         Arguments
         ---
         `name` - Name of the component to call.
 
         **extra - Extra arguments to pass to the component.
         """
         node = self._app.get_node(self)
         com = node.__components__.get(name)
         kw = self._components.get(name)
         if com is not None and kw is not None:
-            return com.call(kw, extra)
+            return await com.call(kw, extra)
             
 class Eventable(object):
     """
     Helper class used for creating nodes with dynamic events.
 
     Arguments
     ---
@@ -214,16 +215,16 @@
         """
         Runs this event from the name.
 
         Arguments
         ---
         `name` - Name of the event to run.
         """
-        res = self.event(name)
+        res = self.get_event(name)
         if res is not None:
             for k, v in res.__dict__.items():
                 event:jsonpack._event = self._app.events.get(k)
                 if event is not None:
-                    event.call(v)
+                    asyncio.run(event.call(v))
         else:
             jsonpack.logger.warning(f"'{self.__file__}': Event '{name}' does not exist!")
         return self
```

### Comparing `jsonpack-0.0.1/jsonpack.egg-info/PKG-INFO` & `jsonpack-0.0.2/jsonpack.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: jsonpack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Easily create JSON packs for your Python Application.
 Home-page: https://github.com/legopitstop/jsonpack
 Author: Legopitstop
 Author-email: officiallegopitstop@gmail.com
 License: MIT
-Keywords: json,pack,manifest,scripts,events,components,Pillow
+Keywords: json,pack,manifest,scripts,events,components,Pillow,schemaser
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jsonpack
 This library allows you to create packs using JSON files to configure your Python Application.
 
+## Install
+```
+pip install jsonpack
+```
+
 ## Features
 - Supports JSON, YAML, ZIP and most image formats
 - Includes the loading of Python files from packs to easily expand your app's features
 - Easily reload all packs without having to restart your application.
 - JSON and YAML validation to make sure your file is properly configured.
 
 See the docs for more information.
 
 ## Optional Dependencies
 |Name|Required|Description|
 |--|--|--|
 |[Pillow](https://pypi.org/project/Pillow/) | No | For image/* mimetypes |
 |[PyYAML](https://pypi.org/project/PyYAML/) | No | For application/yaml mimetype |
+|[opencv-python](https://pypi.org/project/opencv-python/) | No | For video/* mimetype |
+|[pygame](https://pypi.org/project/pygame/) | No | For audio/* mimetype |
```

### Comparing `jsonpack-0.0.1/setup.py` & `jsonpack-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open('README.md') as f:
     long_description = f.read()
 
-required_modules = []
+required_modules = ['schemaser']
 
 setuptools.setup(
     name='jsonpack',
-    version='0.0.1',
+    version='0.0.2',
     author='Legopitstop',
     description='Easily create JSON packs for your Python Application.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/legopitstop/jsonpack',
     packages=setuptools.find_packages(),
     install_requires=required_modules,
     license='MIT',
-    keywords=['json', 'pack', 'manifest', 'scripts', 'events', 'components', 'Pillow'],
+    keywords=['json', 'pack', 'manifest', 'scripts', 'events', 'components', 'Pillow', 'schemaser'],
     author_email='officiallegopitstop@gmail.com',
     classifiers=[
         'Development Status :: 4 - Beta', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
```

