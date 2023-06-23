# Comparing `tmp/dask-felleskomponenter-0.0.8.tar.gz` & `tmp/dask-felleskomponenter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-felleskomponenter-0.0.8.tar", last modified: Thu May  4 12:49:23 2023, max compression
+gzip compressed data, was "dask-felleskomponenter-0.0.9.tar", last modified: Thu May  4 12:54:32 2023, max compression
```

## Comparing `dask-felleskomponenter-0.0.8.tar` & `dask-felleskomponenter-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.144875 dask-felleskomponenter-0.0.8/
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1047 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/LICENSE.txt
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1700 2023-05-04 12:49:23.143855 dask-felleskomponenter-0.0.8/PKG-INFO
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1100 2023-05-04 12:44:58.000000 dask-felleskomponenter-0.0.8/README.md
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      112 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/pyproject.toml
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)       38 2023-05-04 12:49:23.145197 dask-felleskomponenter-0.0.8/setup.cfg
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      895 2023-05-04 12:42:14.000000 dask-felleskomponenter-0.0.8/setup.py
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.131232 dask-felleskomponenter-0.0.8/src/
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.134236 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/__init__.py
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.136295 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/__init__.py
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      899 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/api_client.py
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.137668 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:19:31.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/__init__.py
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     3247 2023-05-04 12:19:31.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/json_sink.py
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.139375 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/__init__.py
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1919 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/api_source.py
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      856 2023-05-04 12:19:28.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/file_source.py
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.135662 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1700 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/PKG-INFO
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      695 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/SOURCES.txt
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        1 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/dependency_links.txt
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)       29 2023-05-04 12:49:23.000000 dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/top_level.txt
-drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:49:23.142284 dask-felleskomponenter-0.0.8/src/tests/
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/tests/__init__.py
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      267 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/tests/test_api_client.py
--rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      941 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.8/src/tests/test_api_source.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.907965 dask-felleskomponenter-0.0.9/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1047 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/LICENSE.txt
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1722 2023-05-04 12:54:32.906998 dask-felleskomponenter-0.0.9/PKG-INFO
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1122 2023-05-04 12:51:18.000000 dask-felleskomponenter-0.0.9/README.md
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      112 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/pyproject.toml
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)       38 2023-05-04 12:54:32.908234 dask-felleskomponenter-0.0.9/setup.cfg
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      895 2023-05-04 12:53:52.000000 dask-felleskomponenter-0.0.9/setup.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.895223 dask-felleskomponenter-0.0.9/src/
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.897831 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/__init__.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.899923 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/common/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/common/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      899 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/common/api_client.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.901419 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sinks/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:19:31.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sinks/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     3247 2023-05-04 12:19:31.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sinks/json_sink.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.903430 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sources/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sources/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1919 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sources/api_source.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      856 2023-05-04 12:19:28.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sources/file_source.py
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.899107 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter.egg-info/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)     1722 2023-05-04 12:54:32.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter.egg-info/PKG-INFO
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      695 2023-05-04 12:54:32.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter.egg-info/SOURCES.txt
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        1 2023-05-04 12:54:32.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter.egg-info/dependency_links.txt
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)       29 2023-05-04 12:54:32.000000 dask-felleskomponenter-0.0.9/src/dask_felleskomponenter.egg-info/top_level.txt
+drwxr-xr-x   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 12:54:32.905660 dask-felleskomponenter-0.0.9/src/tests/
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)        0 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/tests/__init__.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      267 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/tests/test_api_client.py
+-rw-r--r--   0 mari.roysheim (1028602585) BEKKNO\Domain Users (1333597109)      941 2023-05-04 10:17:42.000000 dask-felleskomponenter-0.0.9/src/tests/test_api_source.py
```

### Comparing `dask-felleskomponenter-0.0.8/LICENSE.txt` & `dask-felleskomponenter-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.8/PKG-INFO` & `dask-felleskomponenter-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 Metadata-Version: 2.1
 Name: dask-felleskomponenter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Felleskomponeneter for utvikling av Apache Beam pipelines
 Home-page: https://github.com/kartverket/dask-felleskomponenter
 Author: Dataplattform@Statens Kartverk
 Author-email: dataplattform@kartverket.no
 Project-URL: Bug Tracker, https://github.com/kartverket/dask-felleskomponenter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DASK Felleskomponenter
-This is a repo where we make available apache beam components that is utilized throughout the organization. DASK felleskomponenter is still in an early stage of the development process.
+
+This is a repo where we make available apache beam components that is utilized throughout the organization. DASK
+felleskomponenter is still in an early stage of the development process.
 
 ## Structure
+
 We structure the repo in one main components that contains the following packages:
+
 - common classes
 - custom apache beam sources
 - custom apache beam transforms
 - custom apache beam sinks
 
 ## Dependencies
-You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following command
+
+You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following
+command
+
 ```bash
 pip install -r requirements.txt
 ```
 
 ## Bulding and publishing of package
+
 ### Steps
-- Remove old dist-folder 
+
+- Remove old dist-folder
 - Update version in `setup.py`, for instance `0.0.7`->`0.0.8`
-- (Run `pip install build` if you do not have this already)
+- (Run `pip install -r requirements.txt` if you haven't done that earlier)
 - Run `python3 -m build` (and wait some minutes...)
 - Verity that dist contains a package with the new version in the package name.
 - Run `python3 -m twine upload dist/*` to upload to pypi
 
 ### To upload to PyPi test
+
 Replace the last command with `python3 -m twine upload --repository testpypi dist/*`
```

### Comparing `dask-felleskomponenter-0.0.8/README.md` & `dask-felleskomponenter-0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # DASK Felleskomponenter
-This is a repo where we make available apache beam components that is utilized throughout the organization. DASK felleskomponenter is still in an early stage of the development process.
+
+This is a repo where we make available apache beam components that is utilized throughout the organization. DASK
+felleskomponenter is still in an early stage of the development process.
 
 ## Structure
+
 We structure the repo in one main components that contains the following packages:
+
 - common classes
 - custom apache beam sources
 - custom apache beam transforms
 - custom apache beam sinks
 
 ## Dependencies
-You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following command
+
+You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following
+command
+
 ```bash
 pip install -r requirements.txt
 ```
 
 ## Bulding and publishing of package
+
 ### Steps
-- Remove old dist-folder 
+
+- Remove old dist-folder
 - Update version in `setup.py`, for instance `0.0.7`->`0.0.8`
-- (Run `pip install build` if you do not have this already)
+- (Run `pip install -r requirements.txt` if you haven't done that earlier)
 - Run `python3 -m build` (and wait some minutes...)
 - Verity that dist contains a package with the new version in the package name.
 - Run `python3 -m twine upload dist/*` to upload to pypi
 
 ### To upload to PyPi test
+
 Replace the last command with `python3 -m twine upload --repository testpypi dist/*`
```

### Comparing `dask-felleskomponenter-0.0.8/setup.py` & `dask-felleskomponenter-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dask-felleskomponenter",
-    version="0.0.8",
+    version="0.0.9",
     author="Dataplattform@Statens Kartverk",
     author_email="dataplattform@kartverket.no",
     description="Felleskomponeneter for utvikling av Apache Beam pipelines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kartverket/dask-felleskomponenter",
     project_urls={
```

### Comparing `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/common/api_client.py` & `dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/common/api_client.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sinks/json_sink.py` & `dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sinks/json_sink.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/api_source.py` & `dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sources/api_source.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter/sources/file_source.py` & `dask-felleskomponenter-0.0.9/src/dask_felleskomponenter/sources/file_source.py`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/PKG-INFO` & `dask-felleskomponenter-0.0.9/src/dask_felleskomponenter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 Metadata-Version: 2.1
 Name: dask-felleskomponenter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Felleskomponeneter for utvikling av Apache Beam pipelines
 Home-page: https://github.com/kartverket/dask-felleskomponenter
 Author: Dataplattform@Statens Kartverk
 Author-email: dataplattform@kartverket.no
 Project-URL: Bug Tracker, https://github.com/kartverket/dask-felleskomponenter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DASK Felleskomponenter
-This is a repo where we make available apache beam components that is utilized throughout the organization. DASK felleskomponenter is still in an early stage of the development process.
+
+This is a repo where we make available apache beam components that is utilized throughout the organization. DASK
+felleskomponenter is still in an early stage of the development process.
 
 ## Structure
+
 We structure the repo in one main components that contains the following packages:
+
 - common classes
 - custom apache beam sources
 - custom apache beam transforms
 - custom apache beam sinks
 
 ## Dependencies
-You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following command
+
+You need to install Python3.7 and higher, and to install the dependencies of this project, please execute the following
+command
+
 ```bash
 pip install -r requirements.txt
 ```
 
 ## Bulding and publishing of package
+
 ### Steps
-- Remove old dist-folder 
+
+- Remove old dist-folder
 - Update version in `setup.py`, for instance `0.0.7`->`0.0.8`
-- (Run `pip install build` if you do not have this already)
+- (Run `pip install -r requirements.txt` if you haven't done that earlier)
 - Run `python3 -m build` (and wait some minutes...)
 - Verity that dist contains a package with the new version in the package name.
 - Run `python3 -m twine upload dist/*` to upload to pypi
 
 ### To upload to PyPi test
+
 Replace the last command with `python3 -m twine upload --repository testpypi dist/*`
```

### Comparing `dask-felleskomponenter-0.0.8/src/dask_felleskomponenter.egg-info/SOURCES.txt` & `dask-felleskomponenter-0.0.9/src/dask_felleskomponenter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-felleskomponenter-0.0.8/src/tests/test_api_source.py` & `dask-felleskomponenter-0.0.9/src/tests/test_api_source.py`

 * *Files identical despite different names*

