# Comparing `tmp/cardiac_geometries-0.5.1.tar.gz` & `tmp/cardiac_geometries-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-0.5.1.tar", last modified: Sun Apr 30 15:36:18 2023, max compression
+gzip compressed data, was "cardiac_geometries-0.6.0.tar", last modified: Fri Jun 23 11:48:42 2023, max compression
```

## Comparing `cardiac_geometries-0.5.1.tar` & `cardiac_geometries-0.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.070199 cardiac_geometries-0.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.074199 cardiac_geometries-0.5.1/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1512 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.074199 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/
--rw-r--r--   0 root         (0) root         (0)      602 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12783 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     9594 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_slab.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/utils.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    21343 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_biv.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_lv.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_utils.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    19764 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     4187 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    14224 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)     9972 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.074199 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 15:36:05.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-30 15:36:18.000000 cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 15:36:18.078199 cardiac_geometries-0.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)     1970 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_gmsh.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-04-30 15:36:03.000000 cardiac_geometries-0.5.1/tests/test_mshr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-06-23 11:48:42.703637 cardiac_geometries-0.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.695637 cardiac_geometries-0.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/
+-rw-r--r--   0 root         (0) root         (0)      602 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/utils.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    21343 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_biv.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_lv.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    19764 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16423 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9979 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:48:32.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 11:48:42.000000 cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:48:42.699637 cardiac_geometries-0.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_gmsh.py
+-rw-r--r--   0 root         (0) root         (0)      560 2023-06-23 11:48:30.000000 cardiac_geometries-0.6.0/tests/test_mshr.py
```

### Comparing `cardiac_geometries-0.5.1/LICENSE` & `cardiac_geometries-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/PKG-INFO` & `cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cardiac_geometries
-Version: 0.5.1
+Name: cardiac-geometries
+Version: 0.6.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: gmsh
 Provides-Extra: ldrb
-Provides-Extra: plot
 Provides-Extra: pypi
 Provides-Extra: test
 Provides-Extra: viz
 License-File: LICENSE
 
 # Cardiac Geometries
```

### Comparing `cardiac_geometries-0.5.1/setup.cfg` & `cardiac_geometries-0.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardiac_geometries
-version = 0.5.1
+version = 0.6.0
 description = A python library for cardiac geometries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ComputationalPhysiology/cardiac_geometries
 author = Henrik Finsberg
 author_email = henriknf@simula.no
 license = MIT
@@ -43,23 +43,21 @@
 	jupyter-book
 	jupytext
 	sphinxcontrib-bibtex
 gmsh = 
 	gmsh
 ldrb = 
 	ldrb
-plot = 
-	fenics-plotly
-	matplotlib
 pypi = 
 	build
 test = 
 	ldrb
 	pytest
 	pytest-cov
+	pytest-mpi
 viz = 
 	h5py
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
@@ -72,16 +70,14 @@
 [aliases]
 test = pytest
 
 [tool:pytest]
 addopts = --cov=cardiac_geometries --cov-report html -v --cov-report term-missing
 testpaths = 
 	tests
-env = 
-	FENICS_PLOTLY_SHOW=0
 markers = 
 	mshr: mark a test that tests the mshr backend.
 	gmsh: mark a test that tests the mshr backend.
 
 [mypy]
 files = cardiac_geometries,tests
 ignore_missing_imports = true
```

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/__init__.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/__init__.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_gmsh/_slab.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_gmsh/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_mesh.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_biv.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_biv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/_mshr/_lv.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/_mshr/_lv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/calculus.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/cli.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_slab.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/geometry.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/geometry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 import warnings
 from enum import auto
 from enum import Enum
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import NamedTuple
@@ -19,14 +20,16 @@
 
     from .viz import dict_to_h5
     from .viz import h5_to_dict
     from .viz import h5pyfile
 except ImportError:
     pass
 
+logger = logging.getLogger(__name__)
+
 
 class MeshTypes(Enum):
     slab = auto()
     lv_ellipsoid = auto()
     biv_ellipsoid = auto()
 
 
@@ -60,15 +63,15 @@
     f0: dolfin.Function
     s0: dolfin.Function
     n0: dolfin.Function
 
 
 def load_microstructure(mesh, microstructure_path) -> Microstructure:
     # Get signature
-    with h5pyfile(microstructure_path) as h5file:
+    with h5pyfile(microstructure_path, comm=mesh.mpi_comm()) as h5file:
         signature = h5file["f0"].attrs["signature"].decode()
 
     sig = eval(signature)
     sig._quad_scheme = "default"
     V = dolfin.FunctionSpace(mesh, sig)
     f0 = dolfin.Function(V)
     s0 = dolfin.Function(V)
@@ -176,23 +179,82 @@
     if len(fg) == 1:
         return Path(folder) / fg[0], None
     if len(fg) > 2:
         print(f"Warning: Invalid fname {fname}")
     return Path(folder) / fg[0], fg[1]
 
 
-def dump_schema(path: Union[Path, str], schema: Dict[str, H5Path]) -> None:
-    Path(path).write_text(
-        json.dumps({k: v._asdict() for k, v in schema.items()}, indent=2),
-    )
+def dump_schema(path: Union[Path, str], schema: Dict[str, H5Path], comm=None) -> None:
+    data = {k: v._asdict() for k, v in schema.items()}
+    logger.debug(f"Dump {data} to {path}")
+    if comm is None:
+        comm = dolfin.MPI.comm_world
+
+    if comm.rank == 0:
+        Path(path).write_text(
+            json.dumps(data, indent=2),
+        )
+
+
+def global_check_condition(cond, comm):
+    global_cond = False
+    if comm.rank == 0:
+        global_cond = cond
+    global_cond = comm.bcast(global_cond, root=0)
+    return global_cond
+
+
+def populate_data(schema, groups, comm, path, data, signatures):
+    required_mesh_keys = extract_mesh_keys(schema)
+    for name, mesh_key in required_mesh_keys:
+        if not groups.get(mesh_key, False):
+            msg = f"Missing mesh key '{mesh_key}' for key {name} in {path}"
+            raise RuntimeError(msg)
+
+    with dolfin.HDF5File(comm, path.as_posix(), "r") as h5file:
+        # Meshes
+        for name, p in schema.items():
+            if p.is_mesh and groups.get(name, False):
+                data[name] = dolfin.Mesh(comm)
+                h5file.read(data[name], p.h5group, True)
+
+    for name, p in schema.items():
+        if p.is_meshfunction and groups.get(name, False):
+            current_mesh = data[p.mesh_key]
+            data[name] = dolfin.MeshFunction("size_t", current_mesh, p.dim)
+            continue
+
+        if p.is_function and groups.get(name, False):
+            current_mesh = data[p.mesh_key]
+            signature = signatures.get(name)
+            if signature is None:
+                continue
+            sig = eval(signature)
+            sig._quad_scheme = "default"
+            V = dolfin.FunctionSpace(current_mesh, sig)
+            data[name] = dolfin.Function(V)
+            continue
+
+    dolfin.MPI.barrier(comm)
+
+    with dolfin.HDF5File(comm, path.as_posix(), "r") as h5file:
+        # Meshfunctions
+        for name, p in schema.items():
+            if p.is_meshfunction and groups.get(name, False):
+                h5file.read(data[name], p.h5group)
+                data[name].array()[data[name].array() == 2**64 - 1] = 0
+                continue
+
+            if p.is_function and groups.get(name, False):
+                h5file.read(data[name], p.h5group)
+                continue
 
 
 class Geometry:
     def __init__(self, **kwargs):
-
         self._fields = ["schema"]
         schema = kwargs.pop("schema")
         if schema is None:
             schema = type(self).default_schema()
 
         self.schema = {}
         missing_schema_entries = []
@@ -201,25 +263,38 @@
             if s is None:
                 missing_schema_entries.append(k)
                 continue
             self._fields.append(k)
             setattr(self, k, v)
             self.schema[k] = s
 
+        self.schema = dolfin.MPI.comm_world.bcast(self.schema, root=0)
+        missing_schema_entries = dolfin.MPI.comm_world.bcast(
+            missing_schema_entries,
+            root=0,
+        )
+        self._fields = dolfin.MPI.comm_world.bcast(self._fields, root=0)
+
         if len(missing_schema_entries) > 0:
             msg = (
                 f"Missing schema entry for keys {missing_schema_entries!r}. "
                 "Objects will not be set as geometry attributes"
             )
             warnings.warn(UserWarning(msg), stacklevel=2)
 
     def __repr__(self) -> str:
         fields = ", ".join(self._fields)
         return f"{type(self).__name__}({fields})"
 
+    @property
+    def comm(self):
+        if hasattr(self, "mesh") and hasattr(self.mesh, "mpi_comm"):
+            return self.mesh.mpi_comm()
+        return dolfin.MPI.comm_world
+
     @staticmethod
     def default_schema() -> Dict[str, H5Path]:
         return {
             "mesh": H5Path(
                 h5group=H5Paths.mesh.value,
                 is_mesh=True,
                 fname=FileNames.mesh.value,
@@ -285,117 +360,109 @@
     def save(
         self,
         fname: Union[str, Path],
         schema_path: Optional[Union[str, Path]] = None,
         unlink: bool = True,
     ) -> None:
         path = Path(fname).with_suffix(".h5")
+        logger.debug(f"Save geometry to {path}")
+        dolfin.MPI.barrier(self.comm)
+        file_exist = global_check_condition(path.is_file(), self.comm)
+
         file_mode = "w"
-        if path.is_file():
+        if file_exist:
             if unlink:
-                path.unlink()
+                if self.comm.rank == 0:
+                    path.unlink()
             else:
                 file_mode = "a"
+        logger.debug(f"File already exists: {file_exist}. File mode {file_mode}")
+        dolfin.MPI.barrier(self.comm)
 
+        logger.debug("Save dolfin object")
         with dolfin.HDF5File(
-            dolfin.MPI.comm_world,
+            self.comm,
             path.as_posix(),
             file_mode,
         ) as h5file:
             for name, p in self.schema.items():
                 obj = getattr(self, name, None)
                 if obj is not None and p.is_dolfin:
                     if p.h5group == "":
                         raise RuntimeError("Cannot write object with empty path")
                     h5file.write(obj, p.h5group)
 
+        logger.debug("Save schema to h5")
         for name, p in self.schema.items():
             obj = getattr(self, name, None)
             if obj is not None and not p.is_dolfin:
                 if p.h5group == "":
                     raise RuntimeError("Cannot write object with empty path")
-                dict_to_h5(obj, path, p.h5group)
+
+                dict_to_h5(obj, path, p.h5group, comm=self.comm)
 
         if schema_path is None:
             schema_path = path.with_suffix(".json")
+        logger.debug(f"Save schema {schema_path}")
+        # dolfin.MPI.barrier(self.comm)
+        print(self.comm.rank, schema_path, self.schema)
         dump_schema(schema_path, schema=self.schema)
+        # dolfin.MPI.barrier(self.comm)
+        logger.debug(f"Geometry saved to path {path} and schema to {schema_path}")
 
     @classmethod
     def from_file(
         cls,
         fname: Union[str, Path],
         schema_path: Optional[Union[str, Path]] = None,
         schema: Optional[Dict[str, H5Path]] = None,
+        comm=None,
     ):
         path = Path(fname)
         if not path.is_file():
             msg = f"File {path} does not exist"
             raise FileNotFoundError(msg)
 
         if schema_path is not None:
             schema = load_schema(Path(schema_path))
 
         if schema is None:
             schema = cls.default_schema()
 
+        if comm is None:
+            comm = dolfin.MPI.comm_world
+
         groups = {}
         data = {}
         signatures = {}
-        with h5pyfile(path, "r") as h5file:
+        import h5py
 
-            for name, p in schema.items():
-                if p.h5group == "":
-                    continue
-                groups[name] = p.h5group in h5file
-
-                if not p.is_dolfin:
-                    if groups[name]:
-                        data[name] = h5_to_dict(h5file[p.h5group])
-                    else:
-                        data[name] = None
-
-                if p.is_function and groups[name]:
-                    signatures[name] = h5file[p.h5group].attrs["signature"].decode()
-
-        required_mesh_keys = extract_mesh_keys(schema)
-        for name, mesh_key in required_mesh_keys:
-            if not groups.get(mesh_key, False):
-                msg = f"Missing mesh key '{mesh_key}' for key {name} in {fname}"
-                raise RuntimeError(msg)
-
-        mesh = dolfin.Mesh()
-        with dolfin.HDF5File(mesh.mpi_comm(), path.as_posix(), "r") as h5file:
-
-            # Meshes
-            for name, p in schema.items():
-                if p.is_mesh and groups[name]:
-                    data[name] = dolfin.Mesh()
-
-                    h5file.read(data[name], p.h5group, True)
-
-            # Meshfunctions
-            for name, p in schema.items():
-                if p.is_meshfunction and groups[name]:
-                    current_mesh = data[p.mesh_key]
-                    data[name] = dolfin.MeshFunction("size_t", current_mesh, p.dim)
-                    h5file.read(data[name], p.h5group)
-                    data[name].array()[data[name].array() == 2**64 - 1] = 0
-                    continue
-
-                if p.is_function and groups[name]:
-                    current_mesh = data[p.mesh_key]
-                    signature = signatures.get(name)
-                    if signature is None:
+        if comm.rank == 0:
+            with h5py.File(path, "r") as h5file:
+                for name, p in schema.items():
+                    if p.h5group == "":
                         continue
-                    sig = eval(signature)
-                    sig._quad_scheme = "default"
-                    V = dolfin.FunctionSpace(current_mesh, sig)
-                    data[name] = dolfin.Function(V)
-                    h5file.read(data[name], p.h5group)
-                    continue
+                    groups[name] = p.h5group in h5file
+
+                    if not p.is_dolfin:
+                        if groups[name]:
+                            data[name] = h5_to_dict(h5file[p.h5group])
+                        else:
+                            data[name] = None
+
+                    if p.is_function and groups[name]:
+                        signatures[name] = h5file[p.h5group].attrs["signature"].decode()
+
+        dolfin.MPI.barrier(comm)
+        signatures = comm.bcast(signatures, root=0)
+        groups = comm.bcast(groups, root=0)
+        data = comm.bcast(data, root=0)
+        dolfin.MPI.barrier(comm)
+
+        populate_data(schema, groups, comm, path, data, signatures)
 
         return cls(**data, schema=schema)
 
     @classmethod
     def from_folder(cls, folder, schema: Optional[Dict[str, H5Path]] = None):
         folder = Path(folder)
```

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries/viz.py` & `cardiac_geometries-0.6.0/src/cardiac_geometries/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,47 +94,52 @@
         <DataItem Format="HDF" Dimensions="{nverts} {dim}">{h5name}:/{h5group}</DataItem>
     </Attribute>
     """,
 )
 
 
 @contextlib.contextmanager
-def h5pyfile(h5name, filemode="r"):
+def h5pyfile(h5name, filemode="r", comm=None):
     try:
         import h5py
     except ImportError:
         print("Please install h5py")
         print("python3 -m pip install h5py --no-binary=h5py")
         raise
 
-    from mpi4py import MPI
+    if comm is None:
+        comm = dolfin.MPI.comm_world
 
-    if h5py.h5.get_config().mpi and dolfin.MPI.size(dolfin.MPI.comm_world) > 1:
-        h5file = h5py.File(h5name, filemode, driver="mpio", comm=MPI.COMM_WORLD)
+    if h5py.h5.get_config().mpi and dolfin.MPI.size(comm) > 1:
+        h5file = h5py.File(h5name, filemode, driver="mpio", comm=comm)
     else:
-        if dolfin.MPI.size(dolfin.MPI.comm_world) > 1:
+        if dolfin.MPI.size(comm) > 1:
             warnings.warn("h5py is not installed with MPI support")
         h5file = h5py.File(h5name, filemode)
     yield h5file
 
     h5file.close()
 
 
-def dict_to_h5(data, h5name, h5group):
-    with h5pyfile(h5name, "a") as h5file:
-        if h5group == "":
-            group = h5file
-        else:
-            group = h5file.create_group(h5group)
-        for k, v in data.items():
-            if isinstance(v, str):
-                if dolfin.MPI.size(dolfin.MPI.comm_world) > 1:
-                    # There are some issues with writing strings in paralell
-                    continue
-            group.create_dataset(k, data=v)
+def dict_to_h5(data, h5name, h5group, comm=None):
+    if comm is None:
+        comm = dolfin.MPI.comm_world
+    if comm.rank == 0:
+        import h5py
+
+        with h5py.File(h5name, "a") as h5file:
+            if h5group == "":
+                group = h5file
+            else:
+                group = h5file.create_group(h5group)
+            for k, v in data.items():
+                group.create_dataset(k, data=v)
+
+    # Wait for root process to finish
+    dolfin.MPI.barrier(comm)
 
 
 def decode(x):
     if isinstance(x, bytes):
         return x.decode()
     elif isinstance(x, list):
         return [xi for xi in map(decode, x)]
@@ -146,19 +151,19 @@
 
     group = {}
     for key, value in h5group.items():
         if isinstance(value, h5py.Dataset):
             v = decode(value[...].tolist())
             group[key] = v
 
-        elif isinstance(value, h5py.Group):
-            group[key] = h5_to_dict(h5group[key])
+        # elif isinstance(value, h5py.Group):
+        #     group[key] = h5_to_dict(h5group[key])
 
-        else:
-            raise ValueError(f"Unknown value type {type(value)} for key {key}.")
+        # else:
+        #     raise ValueError(f"Unknown value type {type(value)} for key {key}.")
 
     return group
 
 
 def dolfin_to_hd5(obj: dolfin.Function, h5name, time="", name=None):
     """
     Save object to and HDF file.
@@ -184,15 +189,14 @@
     if value_size(obj) == 1:
         return save_scalar_function(obj, h5name, group, file_mode)
     else:
         return save_vector_function(obj, h5name, group, file_mode)
 
 
 def save_scalar_function(obj, h5name, h5group="", file_mode="w"):
-
     V = obj.function_space()
 
     dim = V.mesh().geometry().dim()
     # TODO: gather
     coords_tmp = V.tabulate_dof_coordinates()
     coords = coords_tmp.reshape((-1, dim))
     # TODO: gather
@@ -228,15 +232,14 @@
         "coords": coords,
         "degree": element.degree(),
         "type": "scalar",
     }
 
 
 def save_vector_function(obj, h5name, h5group="", file_mode="w"):
-
     V = obj.function_space()
     gs = obj.split(deepcopy=True)
 
     W = V.sub(0).collapse()
     dim = V.mesh().geometry().dim()
     # TODO: gather
     coords_tmp = W.tabulate_dof_coordinates()
@@ -245,15 +248,14 @@
     us = [g.vector().get_local() for g in gs]
     vecs = np.array(us).T
 
     coord_group = "/".join([h5group, "coordinates"])
     vector_group = "/".join([h5group, "vector"])
 
     with h5pyfile(h5name, file_mode) as h5file:
-
         if h5group in h5file:
             del h5file[h5group]
         h5file.create_dataset(coord_group, data=coords)
         h5file.create_dataset(vector_group, data=vecs)
 
     element = obj.ufl_element()
 
@@ -275,15 +277,14 @@
         "coords": coords,
         "degree": element.degree(),
         "type": "vector",
     }
 
 
 def fun_to_xdmf(fun, fname, name="function"):
-
     h5name = Path(fname).with_suffix(".h5")
     dolfin_to_hd5(fun, h5name, name=name)
 
     dim = fun.function_space().mesh().geometry().dim()
 
     if value_size(fun) == 1:
         nverts = len(fun.vector())
@@ -329,15 +330,14 @@
             return 1, base_direction[1]
         elif base_direction[0] == "-":
             return -1, base_direction[1]
     raise ValueError(f"Invalid base direction {base_direction!r}")
 
 
 def fiber_to_xdmf(fun: dolfin.Function, fname, base_direction="z"):
-
     h5name = Path(fname).with_suffix(".h5")
     dolfin_to_hd5(fun, h5name, name="fiber")
 
     sign, direction = get_sign_direction(base_direction=base_direction)
     index = {"x": 0, "y": 1, "z": 2}[direction]
 
     f = fun.split(deepcopy=True)[index]
```

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cardiac-geometries
-Version: 0.5.1
+Name: cardiac_geometries
+Version: 0.6.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: gmsh
 Provides-Extra: ldrb
-Provides-Extra: plot
 Provides-Extra: pypi
 Provides-Extra: test
 Provides-Extra: viz
 License-File: LICENSE
 
 # Cardiac Geometries
```

### Comparing `cardiac_geometries-0.5.1/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-0.6.0/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.5.1/tests/test_cli.py` & `cardiac_geometries-0.6.0/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 from pathlib import Path
 
+import pytest
 from cardiac_geometries import cli
 from cardiac_geometries.geometry import Geometry
 from click.testing import CliRunner
 
+try:
+    import dolfin
 
+    _size = dolfin.MPI.size(dolfin.MPI.comm_world)
+except ImportError:
+    _size = 0
+
+
+no_mpi = pytest.mark.skipif(_size > 1, reason="Only works in serial")
+
+
+@no_mpi
 def test_create_slab(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(cli.create_slab, ["--create-fibers", tmp_path.as_posix()])
     assert res1.exit_code == 0
     outfile = tmp_path / "geo.h5"
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
+@no_mpi
 def test_create_lv_ellipsoid(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_lv_ellipsoid,
         ["--create-fibers", tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
@@ -28,14 +41,15 @@
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
+@no_mpi
 def test_create_biv_ellipsoid(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_biv_ellipsoid,
         ["--create-fibers", tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
@@ -43,14 +57,15 @@
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
+@no_mpi
 def test_create_biv_ellipsoid_torso(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_biv_ellipsoid_torso,
         [tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
```

### Comparing `cardiac_geometries-0.5.1/tests/test_geometry.py` & `cardiac_geometries-0.6.0/tests/test_geometry.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 import dolfin
 import pytest
 from cardiac_geometries.geometry import Geometry
 from cardiac_geometries.geometry import H5Path
 from cardiac_geometries.geometry import load_schema
 
 
+no_mpi = pytest.mark.skipif(
+    dolfin.MPI.size(dolfin.MPI.comm_world) > 1,
+    reason="Only works in serial",
+)
+
+
 class ExampleData(NamedTuple):
     info: Dict[str, Any]
     mesh: dolfin.Mesh
     ffun: dolfin.MeshFunction
     f0: dolfin.Function
     info2: Dict[str, Any]
     mesh2: dolfin.Mesh
@@ -47,51 +53,61 @@
         info2=info2,
         mesh2=mesh2,
         ffun2=ffun2,
         f02=f02,
     )
 
 
-def test_load_invalid_schema(tmp_path):
+@no_mpi
+def test_load_invalid_schema(mpi_tmp_path):
     schema = {
         "mesh": dict(h5group="/mesh", is_mesh=True, invalid_key=42),
         "ffun": dict(h5group="/ffun", is_meshfunction=True, dim=2),
         "f0": dict(h5group="/f0", is_function=True),
     }
-    path = tmp_path / "schema.json"
+    path = mpi_tmp_path / "schema.json"
     path.write_text(json.dumps(schema, indent=2))
     new_schema = load_schema(path)
     for name, d in schema.items():
         for k, v in d.items():
             if k == "invalid_key":
                 continue
             assert getattr(new_schema[name], k) == v
 
 
-def test_save_load_simple(tmp_path, example_data):
+def test_save_load_simple(mpi_tmp_path, example_data):
+    # import logging
+
+    # logging.basicConfig(
+    #     level=logging.DEBUG,
+    #     format="%(process)d - %(levelname)s - %(filename)s: %(lineno)d - %(message)s",
+    # )
     schema = {
         "info": H5Path(h5group="/info", is_dolfin=False),
         "mesh": H5Path(h5group="/mesh", is_mesh=True),
         "ffun": H5Path(h5group="/ffun", is_meshfunction=True, dim=2, mesh_key="mesh"),
         "f0": H5Path(h5group="/f0", is_function=True, mesh_key="mesh"),
     }
     geo = Geometry(**example_data._asdict(), schema=schema)
-    path = tmp_path / "geo.h5"
+
+    path = mpi_tmp_path / "geo.h5"
     schema_path = path.with_suffix(".json")
     geo.save(path, schema_path=schema_path)
+
     assert path.is_file()
 
     new_geo = Geometry.from_file(path, schema_path=schema_path)
     assert new_geo.schema == geo.schema
     assert new_geo.info == geo.info
     assert (new_geo.mesh.coordinates() == geo.mesh.coordinates()).all()
-    assert (new_geo.ffun.array() == geo.ffun.array()).all()
+    # assert (new_geo.ffun.array() == geo.ffun.array()).all()
     assert (new_geo.f0.vector().get_local() == geo.f0.vector().get_local()).all()
 
 
+@no_mpi
 def test_save_load_multiple_meshes(tmp_path, example_data):
     schema = {
         "info": H5Path(h5group="/group1/info", is_dolfin=False),
         "mesh": H5Path(h5group="/group1/mesh", is_mesh=True),
         "ffun": H5Path(
             h5group="/group1/ffun",
             is_meshfunction=True,
```

### Comparing `cardiac_geometries-0.5.1/tests/test_gmsh.py` & `cardiac_geometries-0.6.0/tests/test_gmsh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from pathlib import Path
 
 import pytest
 from cardiac_geometries import gmsh
 from cardiac_geometries import has_gmsh
 
+try:
+    import dolfin
+
+    _size = dolfin.MPI.size(dolfin.MPI.comm_world)
+except ImportError:
+    _size = 0
+
+
 require_gmsh = pytest.mark.skipif(
-    not has_gmsh(),
+    not has_gmsh() or _size > 1,
     reason="gmsh is required to run the test",
 )
 
 
 @require_gmsh
 @pytest.mark.gmsh
 def test_lv_prolate_flat_base():
```

