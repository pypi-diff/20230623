# Comparing `tmp/bob.measure-6.1.0.tar.gz` & `tmp/bob.measure-6.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.measure-6.1.0.tar", last modified: Fri Jun 16 12:11:57 2023, max compression
+gzip compressed data, was "bob.measure-6.1.1b0.tar", last modified: Fri Jun 23 19:16:05 2023, max compression
```

## Comparing `bob.measure-6.1.0.tar` & `bob.measure-6.1.1b0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.381044 bob.measure-6.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-12 19:12:08.000000 bob.measure-6.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-12 19:12:08.000000 bob.measure-6.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-16 12:11:57.381044 bob.measure-6.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1151 2023-06-16 12:08:33.000000 bob.measure-6.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.373045 bob.measure-6.1.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7438 2023-06-12 19:12:08.000000 bob.measure-6.1.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)    24828 2023-06-12 19:12:08.000000 bob.measure-6.1.0/doc/guide.rst
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-12 19:12:08.000000 bob.measure-6.1.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3516 2023-06-12 19:12:08.000000 bob.measure-6.1.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-06-12 19:12:08.000000 bob.measure-6.1.0/doc/py_api.rst
--rw-rw-rw-   0 root         (0) root         (0)     2984 2023-06-16 12:08:33.000000 bob.measure-6.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:11:57.381044 bob.measure-6.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-12 19:12:08.000000 bob.measure-6.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.373045 bob.measure-6.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.373045 bob.measure-6.1.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.377045 bob.measure-6.1.0/src/bob/measure/
--rw-rw-rw-   0 root         (0) root         (0)    18523 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47813 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/_library.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     2168 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/load.py
--rw-rw-rw-   0 root         (0) root         (0)    22937 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.377045 bob.measure-6.1.0/src/bob/measure/script/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 12:11:34.000000 bob.measure-6.1.0/src/bob/measure/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/script/commands.py
--rw-rw-rw-   0 root         (0) root         (0)    41599 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/script/common_options.py
--rw-rw-rw-   0 root         (0) root         (0)    43173 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/script/figure.py
--rw-rw-rw-   0 root         (0) root         (0)     2779 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/script/gen.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/script/measure.py
--rw-rw-rw-   0 root         (0) root         (0)     5603 2023-06-12 19:12:08.000000 bob.measure-6.1.0/src/bob/measure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.377045 bob.measure-6.1.0/src/bob.measure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-16 12:11:57.000000 bob.measure-6.1.0/src/bob.measure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      864 2023-06-16 12:11:57.000000 bob.measure-6.1.0/src/bob.measure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:11:57.000000 bob.measure-6.1.0/src/bob.measure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      413 2023-06-16 12:11:57.000000 bob.measure-6.1.0/src/bob.measure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:11:57.000000 bob.measure-6.1.0/src/bob.measure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-16 12:11:57.000000 bob.measure-6.1.0/src/bob.measure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-16 12:11:57.000000 bob.measure-6.1.0/src/bob.measure.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:11:57.381044 bob.measure-6.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    19958 2023-06-12 19:12:08.000000 bob.measure-6.1.0/tests/test_error.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-12 19:12:08.000000 bob.measure-6.1.0/tests/test_load.py
--rw-rw-rw-   0 root         (0) root         (0)     7797 2023-06-12 19:12:08.000000 bob.measure-6.1.0/tests/test_script.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-06-12 19:12:08.000000 bob.measure-6.1.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.467525 bob.measure-6.1.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-23 19:16:05.467525 bob.measure-6.1.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.455525 bob.measure-6.1.1b0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7438 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)    24828 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/doc/guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3516 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/doc/py_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:16:05.471525 bob.measure-6.1.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.455525 bob.measure-6.1.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.455525 bob.measure-6.1.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.463525 bob.measure-6.1.1b0/src/bob/measure/
+-rw-rw-rw-   0 root         (0) root         (0)    18523 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47813 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/_library.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2168 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/load.py
+-rw-rw-rw-   0 root         (0) root         (0)    22937 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.467525 bob.measure-6.1.1b0/src/bob/measure/script/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:15:37.000000 bob.measure-6.1.1b0/src/bob/measure/script/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/script/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    41599 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/script/common_options.py
+-rw-rw-rw-   0 root         (0) root         (0)    43173 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/script/figure.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/script/gen.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/script/measure.py
+-rw-rw-rw-   0 root         (0) root         (0)     5603 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/src/bob/measure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.459525 bob.measure-6.1.1b0/src/bob.measure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-23 19:16:05.000000 bob.measure-6.1.1b0/src/bob.measure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      864 2023-06-23 19:16:05.000000 bob.measure-6.1.1b0/src/bob.measure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:16:05.000000 bob.measure-6.1.1b0/src/bob.measure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      413 2023-06-23 19:16:05.000000 bob.measure-6.1.1b0/src/bob.measure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:16:05.000000 bob.measure-6.1.1b0/src/bob.measure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-23 19:16:05.000000 bob.measure-6.1.1b0/src/bob.measure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 19:16:05.000000 bob.measure-6.1.1b0/src/bob.measure.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:05.467525 bob.measure-6.1.1b0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    19958 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/tests/test_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/tests/test_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     7797 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/tests/test_script.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-06-23 19:11:48.000000 bob.measure-6.1.1b0/tests/test_utils.py
```

### Comparing `bob.measure-6.1.0/LICENSE` & `bob.measure-6.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/PKG-INFO` & `bob.measure-6.1.1b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.measure
-Version: 6.1.0
+Version: 6.1.1b0
 Summary: Evaluation metrics for Bob
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.measure/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.measure
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.measure/-/releases
 Keywords: bob,pipelines
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![badge doc](https://img.shields.io/badge/docs-v6.1.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.measure/badges/v6.1.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.measure/commits/v6.1.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.measure/badges/v6.1.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.measure/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.measure/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.measure/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.measure)
 
 # Experiment Evaluation Metrics for Bob
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains common routines for
 assessing performance of machine learning experiments.
```

### Comparing `bob.measure-6.1.0/README.md` & `bob.measure-6.1.1b0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![badge doc](https://img.shields.io/badge/docs-v6.1.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.measure/badges/v6.1.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.measure/commits/v6.1.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.measure/badges/v6.1.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.measure/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.measure/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.measure/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.measure)
 
 # Experiment Evaluation Metrics for Bob
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains common routines for
 assessing performance of machine learning experiments.
```

### Comparing `bob.measure-6.1.0/doc/conf.py` & `bob.measure-6.1.1b0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/doc/guide.rst` & `bob.measure-6.1.1b0/doc/guide.rst`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/doc/index.rst` & `bob.measure-6.1.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/doc/links.rst` & `bob.measure-6.1.1b0/doc/links.rst`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/doc/py_api.rst` & `bob.measure-6.1.1b0/doc/py_api.rst`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/pyproject.toml` & `bob.measure-6.1.1b0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "bob.measure"
-    version = "6.1.0"
+    version = "6.1.1b0"
     requires-python = ">=3.9"
     description = "Evaluation metrics for Bob"
     dynamic = ["readme"]
     license = {text = "BSD 3-Clause License"}
     authors = [
     {name = "Andre Anjos", email = "andre.anjos@idiap.ch"},
     ]
@@ -21,45 +21,45 @@
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "bob.io.base==5.1.0",
-        "clapper==1.0.1",
-        "h5py==3.7.0",
-        "matplotlib==3.6.2",
-        "numba==0.56.4",
-        "numpy==1.23.5",
-        "scipy==1.10.0",
-        "tabulate==0.9.0",
+        "bob",
+        "bob.io.base",
+        "clapper",
+        "h5py",
+        "matplotlib",
+        "numba",
+        "numpy",
+        "scipy",
+        "tabulate",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/sphinx/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/sphinx/"
     homepage = "https://pypi.org/project/bob.measure/"
     repository = "https://gitlab.idiap.ch/bob/bob.measure"
     changelog = "https://gitlab.idiap.ch/bob/bob.measure/-/releases"
 
 [project.optional-dependencies]
     qa = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "auto-intersphinx==1.0.2",
-        "sphinxcontrib-programoutput==0.17",
-        "matplotlib==3.6.2",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
+        "auto-intersphinx",
+        "sphinxcontrib-programoutput",
+        "matplotlib",
         ]
     test = [
-        "pytest==7.2.1",
-        "pytest-cov==4.0.0",
-        "coverage==7.0.5",
+        "pytest",
+        "pytest-cov",
+        "coverage",
         ]
 
 [tool.setuptools]
     zip-safe = false
     package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
@@ -93,11 +93,7 @@
     addopts = [
         "--import-mode=append",
         "--cov-report=term-missing",
         "--cov=bob.measure",
     ]
     junit_logging = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.measure-6.1.0/src/bob/measure/__init__.py` & `bob.measure-6.1.1b0/src/bob/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/_library.py` & `bob.measure-6.1.1b0/src/bob/measure/_library.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/calibration.py` & `bob.measure-6.1.1b0/src/bob/measure/calibration.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/load.py` & `bob.measure-6.1.1b0/src/bob/measure/load.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/plot.py` & `bob.measure-6.1.1b0/src/bob/measure/plot.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/script/commands.py` & `bob.measure-6.1.1b0/src/bob/measure/script/commands.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/script/common_options.py` & `bob.measure-6.1.1b0/src/bob/measure/script/common_options.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/script/figure.py` & `bob.measure-6.1.1b0/src/bob/measure/script/figure.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/script/gen.py` & `bob.measure-6.1.1b0/src/bob/measure/script/gen.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob/measure/utils.py` & `bob.measure-6.1.1b0/src/bob/measure/utils.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/src/bob.measure.egg-info/PKG-INFO` & `bob.measure-6.1.1b0/src/bob.measure.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.measure
-Version: 6.1.0
+Version: 6.1.1b0
 Summary: Evaluation metrics for Bob
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.measure/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.measure
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.measure/-/releases
 Keywords: bob,pipelines
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![badge doc](https://img.shields.io/badge/docs-v6.1.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.measure/badges/v6.1.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.measure/commits/v6.1.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.measure/badges/v6.1.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/v6.1.0/coverage/)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.measure/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.measure/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.measure/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.measure/master/coverage/)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.measure)
 
 # Experiment Evaluation Metrics for Bob
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains common routines for
 assessing performance of machine learning experiments.
```

### Comparing `bob.measure-6.1.0/src/bob.measure.egg-info/SOURCES.txt` & `bob.measure-6.1.1b0/src/bob.measure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/tests/test_error.py` & `bob.measure-6.1.1b0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/tests/test_load.py` & `bob.measure-6.1.1b0/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/tests/test_script.py` & `bob.measure-6.1.1b0/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `bob.measure-6.1.0/tests/test_utils.py` & `bob.measure-6.1.1b0/tests/test_utils.py`

 * *Files identical despite different names*

