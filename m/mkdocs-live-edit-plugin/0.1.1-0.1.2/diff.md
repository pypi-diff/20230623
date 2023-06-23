# Comparing `tmp/mkdocs-live-edit-plugin-0.1.1.tar.gz` & `tmp/mkdocs-live-edit-plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-live-edit-plugin-0.1.1.tar", last modified: Fri Jun 23 19:01:30 2023, max compression
+gzip compressed data, was "mkdocs-live-edit-plugin-0.1.2.tar", last modified: Fri Jun 23 19:07:35 2023, max compression
```

## Comparing `mkdocs-live-edit-plugin-0.1.1.tar` & `mkdocs-live-edit-plugin-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:01:30.909750 mkdocs-live-edit-plugin-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-23 19:01:20.000000 mkdocs-live-edit-plugin-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 19:01:20.000000 mkdocs-live-edit-plugin-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-23 19:01:30.909750 mkdocs-live-edit-plugin-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-23 19:01:20.000000 mkdocs-live-edit-plugin-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:01:30.905750 mkdocs-live-edit-plugin-0.1.1/live/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:01:20.000000 mkdocs-live-edit-plugin-0.1.1/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-06-23 19:01:20.000000 mkdocs-live-edit-plugin-0.1.1/live/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:01:30.909750 mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-23 19:01:30.000000 mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-23 19:01:30.000000 mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:01:30.000000 mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 19:01:30.000000 mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 19:01:30.000000 mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 19:01:30.000000 mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:01:30.909750 mkdocs-live-edit-plugin-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-23 19:01:20.000000 mkdocs-live-edit-plugin-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:07:35.220212 mkdocs-live-edit-plugin-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-23 19:07:35.220212 mkdocs-live-edit-plugin-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:07:35.220212 mkdocs-live-edit-plugin-0.1.2/live/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/live/live-edit.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/live/live-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/live/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:07:35.220212 mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-23 19:07:35.000000 mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-23 19:07:35.000000 mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:07:35.000000 mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 19:07:35.000000 mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 19:07:35.000000 mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 19:07:35.000000 mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:07:35.220212 mkdocs-live-edit-plugin-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-23 19:07:27.000000 mkdocs-live-edit-plugin-0.1.2/setup.py
```

### Comparing `mkdocs-live-edit-plugin-0.1.1/LICENSE.md` & `mkdocs-live-edit-plugin-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-live-edit-plugin-0.1.1/PKG-INFO` & `mkdocs-live-edit-plugin-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-live-edit-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: An MkDocs plugin that allows editing pages directly from the browser.
 Home-page: https://github.com/eddyluten/mkdocs-live-edit-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown editing authoring wiki server
 Classifier: License :: OSI Approved :: MIT License
@@ -75,10 +75,10 @@
 
 When you edit the contents of a file, they are sent to the server via WebSockets where the plugin writes the contents to disk. Here, MkDocs picks up on the change and sends a reload signal back to the browser -- this is the same live-reload mechanism that picks up on changes you make via a text editor.
 
 A similar mechanism is in place for other operations like renaming and deleting.
 
 ## Changelog
 
-### 0.1.0 / 0.1.1
+### 0.1.0
 
 Initial release with editing, renaming, and deletion logic in place.
```

### Comparing `mkdocs-live-edit-plugin-0.1.1/README.md` & `mkdocs-live-edit-plugin-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,10 +58,10 @@
 
 When you edit the contents of a file, they are sent to the server via WebSockets where the plugin writes the contents to disk. Here, MkDocs picks up on the change and sends a reload signal back to the browser -- this is the same live-reload mechanism that picks up on changes you make via a text editor.
 
 A similar mechanism is in place for other operations like renaming and deleting.
 
 ## Changelog
 
-### 0.1.0 / 0.1.1
+### 0.1.0
 
 Initial release with editing, renaming, and deletion logic in place.
```

### Comparing `mkdocs-live-edit-plugin-0.1.1/live/plugin.py` & `mkdocs-live-edit-plugin-0.1.2/live/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-live-edit-plugin-0.1.1/mkdocs_live_edit_plugin.egg-info/PKG-INFO` & `mkdocs-live-edit-plugin-0.1.2/mkdocs_live_edit_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-live-edit-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: An MkDocs plugin that allows editing pages directly from the browser.
 Home-page: https://github.com/eddyluten/mkdocs-live-edit-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown editing authoring wiki server
 Classifier: License :: OSI Approved :: MIT License
@@ -75,10 +75,10 @@
 
 When you edit the contents of a file, they are sent to the server via WebSockets where the plugin writes the contents to disk. Here, MkDocs picks up on the change and sends a reload signal back to the browser -- this is the same live-reload mechanism that picks up on changes you make via a text editor.
 
 A similar mechanism is in place for other operations like renaming and deleting.
 
 ## Changelog
 
-### 0.1.0 / 0.1.1
+### 0.1.0
 
 Initial release with editing, renaming, and deletion logic in place.
```

### Comparing `mkdocs-live-edit-plugin-0.1.1/setup.py` & `mkdocs-live-edit-plugin-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mkdocs-live-edit-plugin',
-    version='0.1.1',
-    description=
-    'An MkDocs plugin that allows editing pages directly from the browser.',
+    version='0.1.2',
+    description='An MkDocs plugin that allows editing pages directly from the browser.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown editing authoring wiki server',
     url='https://github.com/eddyluten/mkdocs-live-edit-plugin',
     author='Eddy Luten',
     author_email='eddyluten@gmail.com',
     license='MIT',
@@ -28,9 +27,10 @@
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     packages=find_packages(exclude=['*.tests']),
     entry_points={
         'mkdocs.plugins': ['live-edit = live.plugin:LiveEditPlugin']
     },
+    data_files=[('live', ['live/live-edit.js', 'live/live-edit.css'])],
     include_package_data=True,
 )
```

