# Comparing `tmp/libcoveofds-0.8.1.tar.gz` & `tmp/libcoveofds-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcoveofds-0.8.1.tar", last modified: Fri Jun 23 15:27:59 2023, max compression
+gzip compressed data, was "libcoveofds-0.8.2.tar", last modified: Fri Jun 23 16:02:35 2023, max compression
```

## Comparing `libcoveofds-0.8.1.tar` & `libcoveofds-0.8.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       31 2023-06-07 07:23:52.000000 libcoveofds-0.8.1/MANIFEST.in
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      837 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/README.rst
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.390739 libcoveofds-0.8.1/libcove2/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-07 07:24:06.000000 libcoveofds-0.8.1/libcove2/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3742 2023-06-07 07:24:06.000000 libcoveofds-0.8.1/libcove2/common.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/libcoveofds/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/libcoveofds/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      561 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/libcoveofds/additionalfields.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5520 2023-06-13 07:34:18.000000 libcoveofds-0.8.1/libcoveofds/cli.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/libcoveofds/data/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)   215464 2023-06-23 15:26:41.000000 libcoveofds-0.8.1/libcoveofds/data/schema-0-3-0.json
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    21467 2023-06-13 07:34:18.000000 libcoveofds-0.8.1/libcoveofds/geojson.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2159 2023-05-04 15:08:13.000000 libcoveofds-0.8.1/libcoveofds/jsonschemavalidate.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    35356 2023-02-09 08:10:34.000000 libcoveofds-0.8.1/libcoveofds/python_validate.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1595 2023-06-15 10:03:03.000000 libcoveofds-0.8.1/libcoveofds/schema.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/libcoveofds.egg-info/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      513 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/SOURCES.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/dependency_links.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       52 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/entry_points.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       89 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/requires.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       21 2023-06-23 15:27:59.000000 libcoveofds-0.8.1/libcoveofds.egg-info/top_level.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       61 2023-06-23 15:27:59.394739 libcoveofds-0.8.1/setup.cfg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1075 2023-06-23 15:26:41.000000 libcoveofds-0.8.1/setup.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 16:02:35.642155 libcoveofds-0.8.2/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       31 2023-06-07 07:23:52.000000 libcoveofds-0.8.2/MANIFEST.in
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-23 16:02:35.642155 libcoveofds-0.8.2/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      837 2023-02-09 08:10:34.000000 libcoveofds-0.8.2/README.rst
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 16:02:35.638155 libcoveofds-0.8.2/libcove2/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-07 07:24:06.000000 libcoveofds-0.8.2/libcove2/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3742 2023-06-07 07:24:06.000000 libcoveofds-0.8.2/libcove2/common.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 16:02:35.638155 libcoveofds-0.8.2/libcoveofds/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-02-09 08:10:34.000000 libcoveofds-0.8.2/libcoveofds/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      561 2023-02-09 08:10:34.000000 libcoveofds-0.8.2/libcoveofds/additionalfields.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5520 2023-06-13 07:34:18.000000 libcoveofds-0.8.2/libcoveofds/cli.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 16:02:35.642155 libcoveofds-0.8.2/libcoveofds/data/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)   179161 2023-06-23 16:01:20.000000 libcoveofds-0.8.2/libcoveofds/data/schema-0-3-0-network-only.json
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)   215464 2023-06-23 15:26:41.000000 libcoveofds-0.8.2/libcoveofds/data/schema-0-3-0.json
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    21467 2023-06-13 07:34:18.000000 libcoveofds-0.8.2/libcoveofds/geojson.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2159 2023-05-04 15:08:13.000000 libcoveofds-0.8.2/libcoveofds/jsonschemavalidate.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    35356 2023-02-09 08:10:34.000000 libcoveofds-0.8.2/libcoveofds/python_validate.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1702 2023-06-23 16:01:20.000000 libcoveofds-0.8.2/libcoveofds/schema.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-23 16:02:35.642155 libcoveofds-0.8.2/libcoveofds.egg-info/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      652 2023-06-23 16:02:35.000000 libcoveofds-0.8.2/libcoveofds.egg-info/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      561 2023-06-23 16:02:35.000000 libcoveofds-0.8.2/libcoveofds.egg-info/SOURCES.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2023-06-23 16:02:35.000000 libcoveofds-0.8.2/libcoveofds.egg-info/dependency_links.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       52 2023-06-23 16:02:35.000000 libcoveofds-0.8.2/libcoveofds.egg-info/entry_points.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       89 2023-06-23 16:02:35.000000 libcoveofds-0.8.2/libcoveofds.egg-info/requires.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       21 2023-06-23 16:02:35.000000 libcoveofds-0.8.2/libcoveofds.egg-info/top_level.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       61 2023-06-23 16:02:35.642155 libcoveofds-0.8.2/setup.cfg
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1075 2023-06-23 16:01:20.000000 libcoveofds-0.8.2/setup.py
```

### Comparing `libcoveofds-0.8.1/PKG-INFO` & `libcoveofds-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcoveofds
-Version: 0.8.1
+Version: 0.8.2
 Summary: A data review library
 Home-page: https://github.com/Open-Telecoms-Data/lib-cove-ofds
 Author: Open Data Services
 Author-email: code@opendataservices.coop
 License: UNKNOWN
 Project-URL: Documentation, https://libcoveofds.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues
```

### Comparing `libcoveofds-0.8.1/README.rst` & `libcoveofds-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcove2/common.py` & `libcoveofds-0.8.2/libcove2/common.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcoveofds/additionalfields.py` & `libcoveofds-0.8.2/libcoveofds/additionalfields.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcoveofds/cli.py` & `libcoveofds-0.8.2/libcoveofds/cli.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcoveofds/data/schema-0-3-0.json` & `libcoveofds-0.8.2/libcoveofds/data/schema-0-3-0.json`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcoveofds/geojson.py` & `libcoveofds-0.8.2/libcoveofds/geojson.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcoveofds/jsonschemavalidate.py` & `libcoveofds-0.8.2/libcoveofds/jsonschemavalidate.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcoveofds/python_validate.py` & `libcoveofds-0.8.2/libcoveofds/python_validate.py`

 * *Files identical despite different names*

### Comparing `libcoveofds-0.8.1/libcoveofds/schema.py` & `libcoveofds-0.8.2/libcoveofds/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 _schema_folder = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data")
 
 
 class OFDSSchema:
     """Represents and provides information about the schema."""
 
     package_schema_url: str = os.path.join(_schema_folder, "schema-0-3-0.json")
+    network_schema_url: str = os.path.join(
+        _schema_folder, "schema-0-3-0-network-only.json"
+    )
 
     def get_package_schema(self):
         with open(self.package_schema_url) as fp:
             return json.load(fp)
 
     def get_link_rels_for_external_nodes(self) -> list:
         return [
```

### Comparing `libcoveofds-0.8.1/libcoveofds.egg-info/PKG-INFO` & `libcoveofds-0.8.2/libcoveofds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcoveofds
-Version: 0.8.1
+Version: 0.8.2
 Summary: A data review library
 Home-page: https://github.com/Open-Telecoms-Data/lib-cove-ofds
 Author: Open Data Services
 Author-email: code@opendataservices.coop
 License: UNKNOWN
 Project-URL: Documentation, https://libcoveofds.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues
```

### Comparing `libcoveofds-0.8.1/setup.py` & `libcoveofds-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="libcoveofds",
-    version="0.8.1",
+    version="0.8.2",
     author="Open Data Services",
     author_email="code@opendataservices.coop",
     url="https://github.com/Open-Telecoms-Data/lib-cove-ofds",
     project_urls={
         "Documentation": "https://libcoveofds.readthedocs.io/en/latest/",
         "Issues": "https://github.com/Open-Telecoms-Data/lib-cove-ofds/issues",
         "Source": "https://github.com/Open-Telecoms-Data/lib-cove-ofds",
```

