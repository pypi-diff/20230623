# Comparing `tmp/idms-0.1.8.tar.gz` & `tmp/idms-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/idms-0.1.8.tar", last modified: Thu Dec 10 15:48:40 2020, max compression
+gzip compressed data, was "idms-0.1.9.tar", last modified: Thu Jul  1 09:29:19 2021, max compression
```

## Comparing `idms-0.1.8.tar` & `idms-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 15:48:40.749848 idms-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1079 2020-12-10 15:48:29.000000 idms-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)      157 2020-12-10 15:48:29.000000 idms-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2873 2020-12-10 15:48:40.749848 idms-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1465 2020-12-10 15:48:29.000000 idms-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 15:48:40.745847 idms-0.1.8/data/
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-10 15:48:29.000000 idms-0.1.8/data/data_file
--rw-r--r--   0 runner    (1001) docker     (116)      230 2020-12-10 15:48:29.000000 idms-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       78 2020-12-10 15:48:40.749848 idms-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     8639 2020-12-10 15:48:29.000000 idms-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 15:48:40.741846 idms-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 15:48:40.745847 idms-0.1.8/src/idms/
--rw-r--r--   0 runner    (1001) docker     (116)       13 2020-12-10 15:48:29.000000 idms-0.1.8/src/idms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 15:48:40.749848 idms-0.1.8/src/idms/api/
--rw-r--r--   0 runner    (1001) docker     (116)       13 2020-12-10 15:48:29.000000 idms-0.1.8/src/idms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10113 2020-12-10 15:48:29.000000 idms-0.1.8/src/idms/api/contentserver.py
--rw-r--r--   0 runner    (1001) docker     (116)      569 2020-12-10 15:48:29.000000 idms-0.1.8/src/idms/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 15:48:40.745847 idms-0.1.8/src/idms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2873 2020-12-10 15:48:40.000000 idms-0.1.8/src/idms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      446 2020-12-10 15:48:40.000000 idms-0.1.8/src/idms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-10 15:48:40.000000 idms-0.1.8/src/idms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       40 2020-12-10 15:48:40.000000 idms-0.1.8/src/idms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      101 2020-12-10 15:48:40.000000 idms-0.1.8/src/idms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2020-12-10 15:48:40.000000 idms-0.1.8/src/idms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-10 15:48:40.749848 idms-0.1.8/src/sample/
--rw-r--r--   0 runner    (1001) docker     (116)      111 2020-12-10 15:48:29.000000 idms-0.1.8/src/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-10 15:48:29.000000 idms-0.1.8/src/sample/package_data.dat
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-10 15:48:29.000000 idms-0.1.8/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.047413 idms-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-07-01 09:29:11.000000 idms-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-07-01 09:29:11.000000 idms-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2925 2021-07-01 09:29:19.047413 idms-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-07-01 09:29:11.000000 idms-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-01 09:29:11.000000 idms-0.1.9/data/data_file
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-07-01 09:29:11.000000 idms-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-07-01 09:29:19.047413 idms-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     8639 2021-07-01 09:29:11.000000 idms-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/idms/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/idms/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10185 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/api/contentserver.py
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/idms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2925 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.047413 idms-0.1.9/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-07-01 09:29:11.000000 idms-0.1.9/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-01 09:29:11.000000 idms-0.1.9/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-07-01 09:29:11.000000 idms-0.1.9/src/sample/simple.py
```

### Comparing `idms-0.1.8/LICENSE.txt` & `idms-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idms-0.1.8/PKG-INFO` & `idms-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/pypa/idms
 Author: Daniel Overdevest
 Author-email: d.overdevest@pzh.nl
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
@@ -48,14 +48,17 @@
         # Export results to Excel
         df.to_excel("searchresults.xlsx")
         ```
         
         # Development
         Package is hosted on GitHub. After each change increase version number and create a new Release on GitHub. The pipeline will trigger a release to PyPi (see status batch above).
         
+        ## Collaborate?
+        Send a PR!
+        
         # Disclaimer
         The developers of this package are not affiliated with OpenText.
 Keywords: idms,contentserver,restapi,searchapi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `idms-0.1.8/README.md` & `idms-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,9 +38,12 @@
 # Export results to Excel
 df.to_excel("searchresults.xlsx")
 ```
 
 # Development
 Package is hosted on GitHub. After each change increase version number and create a new Release on GitHub. The pipeline will trigger a release to PyPi (see status batch above).
 
+## Collaborate?
+Send a PR!
+
 # Disclaimer
 The developers of this package are not affiliated with OpenText.
```

### Comparing `idms-0.1.8/setup.py` & `idms-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.8',  # Required
+    version='0.1.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python class to talk to idms REST and Search API, better known as iDMS.',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `idms-0.1.8/src/idms/api/contentserver.py` & `idms-0.1.9/src/idms/api/contentserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                               'properties.owner', 
                               'properties.create_user_id', 
                               'properties.name', 
                               'properties.description', 
                               'properties.type', 
                               'properties.type_name',
                               'properties.summary',
+                              'properties.description_multilingual.nl',
                               'regions.OTLocation',
                               'systemattributes.Dossiernummer']
 
         self.debugJson = False
 
         if ticket:
             self.ticket = ticket
```

### Comparing `idms-0.1.8/src/idms/functions.py` & `idms-0.1.9/src/idms/functions.py`

 * *Files identical despite different names*

### Comparing `idms-0.1.8/src/idms.egg-info/PKG-INFO` & `idms-0.1.9/src/idms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/pypa/idms
 Author: Daniel Overdevest
 Author-email: d.overdevest@pzh.nl
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
@@ -48,14 +48,17 @@
         # Export results to Excel
         df.to_excel("searchresults.xlsx")
         ```
         
         # Development
         Package is hosted on GitHub. After each change increase version number and create a new Release on GitHub. The pipeline will trigger a release to PyPi (see status batch above).
         
+        ## Collaborate?
+        Send a PR!
+        
         # Disclaimer
         The developers of this package are not affiliated with OpenText.
 Keywords: idms,contentserver,restapi,searchapi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

