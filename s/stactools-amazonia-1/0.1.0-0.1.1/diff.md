# Comparing `tmp/stactools-amazonia-1-0.1.0.tar.gz` & `tmp/stactools-amazonia-1-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-amazonia-1-0.1.0.tar", last modified: Tue Jun  6 18:49:07 2023, max compression
+gzip compressed data, was "stactools-amazonia-1-0.1.1.tar", last modified: Fri Jun 23 20:51:01 2023, max compression
```

## Comparing `stactools-amazonia-1-0.1.0.tar` & `stactools-amazonia-1-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:49:07.714180 stactools-amazonia-1-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-06 18:49:07.714180 stactools-amazonia-1-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-06 18:49:07.714180 stactools-amazonia-1-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:49:07.710180 stactools-amazonia-1-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:49:07.710180 stactools-amazonia-1-0.1.0/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:49:07.710180 stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:49:07.714180 stactools-amazonia-1-0.1.0/src/stactools_amazonia_1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-06 18:49:07.000000 stactools-amazonia-1-0.1.0/src/stactools_amazonia_1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-06 18:49:07.000000 stactools-amazonia-1-0.1.0/src/stactools_amazonia_1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:49:07.000000 stactools-amazonia-1-0.1.0/src/stactools_amazonia_1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 18:49:07.000000 stactools-amazonia-1-0.1.0/src/stactools_amazonia_1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 18:49:07.000000 stactools-amazonia-1-0.1.0/src/stactools_amazonia_1.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:49:07.714180 stactools-amazonia-1-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-06 18:48:46.000000 stactools-amazonia-1-0.1.0/tests/test_stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.697386 stactools-amazonia-1-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.697386 stactools-amazonia-1-0.1.1/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 20:51:01.000000 stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:51:01.701386 stactools-amazonia-1-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-23 20:50:42.000000 stactools-amazonia-1-0.1.1/tests/test_stac.py
```

### Comparing `stactools-amazonia-1-0.1.0/LICENSE` & `stactools-amazonia-1-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.0/PKG-INFO` & `stactools-amazonia-1-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-amazonia-1
-Version: 0.1.0
+Version: 0.1.1
 Summary: Amazonia-1 on AWS stactools package
 Home-page: https://github.com/stactools-packages/amazonia-1
 Author: Frederico Liporace
 Author-email: liporace@amskepler.com
 Project-URL: Issues, https://github.com/stactools-packages/amazonia-1/issues
 Keywords: stactools,pystac,catalog,STAC,Amazonia-1
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-amazonia-1-0.1.0/README.md` & `stactools-amazonia-1-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.0/setup.cfg` & `stactools-amazonia-1-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/commands.py` & `stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/constants.py` & `stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.0/src/stactools/amazonia_1/stac.py` & `stactools-amazonia-1-0.1.1/src/stactools/amazonia_1/stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 )
 from pystac.extensions.eo import Band, EOExtension
 from pystac.extensions.item_assets import AssetDefinition, ItemAssetsExtension
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.sat import OrbitState, SatExtension
 from pystac.extensions.view import ViewExtension
 from pystac.summaries import Summaries
+from stactools.core.io import read_text
 
 from stactools.amazonia_1.constants import (
     BASE_CAMERA,
     BASE_COLLECTION,
     CBERS_AM_MISSIONS,
     TIF_XML_REGEX,
 )
@@ -71,39 +72,38 @@
 
 
 @typing.no_type_check
 def _get_keys_from_cbers_am(cb_am_metadata: str) -> Dict[str, Any]:
     """Extract keys from Amazonia-1 INPE's metadata.
 
     Args:
-        cb_am_metadata: CBERS/AM metadata file location
+        cb_am_metadata: CBERS/AM metadata HREF
 
     Returns:
         Item: STAC Item object
     """
 
     nsp = {"x": "http://www.gisplan.com.br/xmlsat"}
     metadata = {}
 
     match = TIF_XML_REGEX.match(cb_am_metadata.split("/")[-1])
     assert match, f"Can't match {cb_am_metadata}"
 
-    tree = ET.parse(cb_am_metadata)
-    original_root = tree.getroot()
+    tree = ET.fromstring(text=read_text(href=cb_am_metadata))
 
     # satellite node information, checking for CBERS-04A/AMAZONIA1 WFI
     # special case
-    left_root = original_root.find("x:leftCamera", nsp)
+    left_root = tree.find("x:leftCamera", nsp)
     if left_root:
-        right_root = original_root.find("x:rightCamera", nsp)
+        right_root = tree.find("x:rightCamera", nsp)
         # We use the left camera for fields that are not camera
         # specific or are not used for STAC fields computation
         root = left_root
     else:
-        root = original_root
+        root = tree
 
     satellite = root.find("x:satellite", nsp)
 
     metadata["mission"] = satellite.find("x:name", nsp).text
     metadata["number"] = satellite.find("x:number", nsp).text
     metadata["sensor"] = satellite.find("x:instrument", nsp).text
     metadata["collection"] = _build_collection_name(
```

### Comparing `stactools-amazonia-1-0.1.0/src/stactools_amazonia_1.egg-info/PKG-INFO` & `stactools-amazonia-1-0.1.1/src/stactools_amazonia_1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-amazonia-1
-Version: 0.1.0
+Version: 0.1.1
 Summary: Amazonia-1 on AWS stactools package
 Home-page: https://github.com/stactools-packages/amazonia-1
 Author: Frederico Liporace
 Author-email: liporace@amskepler.com
 Project-URL: Issues, https://github.com/stactools-packages/amazonia-1/issues
 Keywords: stactools,pystac,catalog,STAC,Amazonia-1
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-amazonia-1-0.1.0/tests/test_commands.py` & `stactools-amazonia-1-0.1.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stactools-amazonia-1-0.1.0/tests/test_stac.py` & `stactools-amazonia-1-0.1.1/tests/test_stac.py`

 * *Files identical despite different names*

