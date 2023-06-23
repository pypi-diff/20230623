# Comparing `tmp/omero-parade-0.2.dev1.tar.gz` & `tmp/omero-parade-0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omero-parade-0.2.dev1.tar", last modified: Wed Nov 27 16:50:58 2019, max compression
+gzip compressed data, was "dist/omero-parade-0.2.dev2.tar", last modified: Thu Dec  5 10:50:22 2019, max compression
```

## Comparing `omero-parade-0.2.dev1.tar` & `omero-parade-0.2.dev2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     8684 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    34519 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/table_filters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5505 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/table_filters/data_providers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4387 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/table_filters/omero_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/table_filters/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10081 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/css/parade.css
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2852 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/images/icon_layout.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/images/table_layout.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     2868 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/images/plot_layout.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/js/
--rw-rw-r--   0 travis    (2000) travis    (2000)  1316277 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/js/bundle.js.map
--rw-rw-r--   0 travis    (2000) travis    (2000)   297092 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/static/omero_parade/js/bundle.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     4203 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/data_providers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1731 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/templates/omero_parade/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/templates/omero_parade/init.js.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      898 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/templates/omero_parade/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade/annotation_filters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7998 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/annotation_filters/omero_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/annotation_filters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3612 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/omero_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3597 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/parade_settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      868 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6159 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/omero_parade/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5886 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2019-11-27 16:44:12.000000 omero-parade-0.2.dev1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8684 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1097 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-11-27 16:50:58.000000 omero-parade-0.2.dev1/omero_parade.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8684 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34519 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/table_filters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5505 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/table_filters/data_providers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4387 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/table_filters/omero_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/table_filters/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/css/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10081 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/css/parade.css
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2852 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/images/icon_layout.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/images/table_layout.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2868 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/images/plot_layout.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/js/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1316277 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/js/bundle.js.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)   297092 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/static/omero_parade/js/bundle.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4203 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/data_providers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1731 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/templates/omero_parade/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/templates/omero_parade/init.js.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      898 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/templates/omero_parade/index.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade/annotation_filters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8004 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/annotation_filters/omero_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/annotation_filters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3612 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/omero_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3597 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/parade_settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      868 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6159 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/omero_parade/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5886 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2019-12-05 10:44:01.000000 omero-parade-0.2.dev2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8684 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1097 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-12-05 10:50:22.000000 omero-parade-0.2.dev2/omero_parade.egg-info/requires.txt
```

### Comparing `omero-parade-0.2.dev1/PKG-INFO` & `omero-parade-0.2.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: omero-parade
-Version: 0.2.dev1
+Version: 0.2.dev2
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-parade
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-parade/archive/v0.2.dev1.tar.gz
+Download-URL: https://github.com/ome/omero-parade/archive/v0.2.dev2.tar.gz
 Description: .. image:: https://travis-ci.org/ome/omero-parade.svg?branch=master
             :target: https://travis-ci.org/ome/omero-parade
         
         .. image:: https://badge.fury.io/py/omero-parade.svg
             :target: https://badge.fury.io/py/omero-parade
         
         OMERO.parade
```

### Comparing `omero-parade-0.2.dev1/LICENSE` & `omero-parade-0.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/table_filters/data_providers.py` & `omero-parade-0.2.dev2/omero_parade/table_filters/data_providers.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/table_filters/omero_filters.py` & `omero-parade-0.2.dev2/omero_parade/table_filters/omero_filters.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/static/omero_parade/css/parade.css` & `omero-parade-0.2.dev2/omero_parade/static/omero_parade/css/parade.css`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/static/omero_parade/images/icon_layout.png` & `omero-parade-0.2.dev2/omero_parade/static/omero_parade/images/icon_layout.png`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/static/omero_parade/images/table_layout.png` & `omero-parade-0.2.dev2/omero_parade/static/omero_parade/images/table_layout.png`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/static/omero_parade/images/plot_layout.png` & `omero-parade-0.2.dev2/omero_parade/static/omero_parade/images/plot_layout.png`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/static/omero_parade/js/bundle.js.map` & `omero-parade-0.2.dev2/omero_parade/static/omero_parade/js/bundle.js.map`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/static/omero_parade/js/bundle.js` & `omero-parade-0.2.dev2/omero_parade/static/omero_parade/js/bundle.js`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/data_providers.py` & `omero-parade-0.2.dev2/omero_parade/data_providers.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/urls.py` & `omero-parade-0.2.dev2/omero_parade/urls.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/templates/omero_parade/init.js.html` & `omero-parade-0.2.dev2/omero_parade/templates/omero_parade/init.js.html`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/templates/omero_parade/index.html` & `omero-parade-0.2.dev2/omero_parade/templates/omero_parade/index.html`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/annotation_filters/omero_filters.py` & `omero-parade-0.2.dev2/omero_parade/annotation_filters/omero_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         return (params.query === '' || match);
     }
     return false;
 })
         """ % (json.dumps(map_values), key_placeholder, js_object_attr,
                js_object_attr)
 
-        keys = map_values.keys()
+        keys = list(map_values.keys())
         keys.sort(key=lambda x: x.lower())
 
         filter_params = [{'name': 'key',
                           'type': 'text',
                           'values': [key_placeholder] + keys,
                           'default': key_placeholder},
                          {'name': 'query',
```

### Comparing `omero-parade-0.2.dev1/omero_parade/omero_filters.py` & `omero-parade-0.2.dev2/omero_parade/omero_filters.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/utils.py` & `omero-parade-0.2.dev2/omero_parade/utils.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/parade_settings.py` & `omero-parade-0.2.dev2/omero_parade/parade_settings.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/apps.py` & `omero-parade-0.2.dev2/omero_parade/apps.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/omero_parade/views.py` & `omero-parade-0.2.dev2/omero_parade/views.py`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/README.rst` & `omero-parade-0.2.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `omero-parade-0.2.dev1/setup.py` & `omero-parade-0.2.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import os
 import setuptools.command.install
 import setuptools.command.develop
 import setuptools.command.sdist
 from distutils.core import Command
 from setuptools import setup, find_packages
 
-VERSION = "0.2.dev1"
+VERSION = "0.2.dev2"
 
 DESCRIPTION = "A Python plugin for OMERO.web"
 AUTHOR = "The Open Microscopy Team"
 LICENSE = "AGPL-3.0"
 HOMEPAGE = "https://github.com/ome/omero-parade"
```

### Comparing `omero-parade-0.2.dev1/omero_parade.egg-info/PKG-INFO` & `omero-parade-0.2.dev2/omero_parade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: omero-parade
-Version: 0.2.dev1
+Version: 0.2.dev2
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-parade
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-parade/archive/v0.2.dev1.tar.gz
+Download-URL: https://github.com/ome/omero-parade/archive/v0.2.dev2.tar.gz
 Description: .. image:: https://travis-ci.org/ome/omero-parade.svg?branch=master
             :target: https://travis-ci.org/ome/omero-parade
         
         .. image:: https://badge.fury.io/py/omero-parade.svg
             :target: https://badge.fury.io/py/omero-parade
         
         OMERO.parade
```

### Comparing `omero-parade-0.2.dev1/omero_parade.egg-info/SOURCES.txt` & `omero-parade-0.2.dev2/omero_parade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

