# Comparing `tmp/bob.io.base-5.1.0.tar.gz` & `tmp/bob.io.base-5.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.io.base-5.1.0.tar", last modified: Fri Jun 16 11:58:17 2023, max compression
+gzip compressed data, was "bob.io.base-5.1.1b0.tar", last modified: Fri Jun 23 19:05:41 2023, max compression
```

## Comparing `bob.io.base-5.1.0.tar` & `bob.io.base-5.1.1b0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.240806 bob.io.base-5.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-16 11:58:17.240806 bob.io.base-5.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-16 10:57:42.000000 bob.io.base-5.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.232806 bob.io.base-5.1.0/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.232806 bob.io.base-5.1.0/doc/img/
--rw-rw-rw-   0 root         (0) root         (0)     4286 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/doc/img/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     6266 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/doc/img/logo.png
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/doc/py_api.rst
--rw-rw-rw-   0 root         (0) root         (0)     1974 2023-06-16 10:57:42.000000 bob.io.base-5.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 11:58:17.240806 bob.io.base-5.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.228806 bob.io.base-5.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.232806 bob.io.base-5.1.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.236806 bob.io.base-5.1.0/src/bob/io/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/src/bob/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.236806 bob.io.base-5.1.0/src/bob/io/base/
--rw-rw-rw-   0 root         (0) root         (0)    12455 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/src/bob/io/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4537 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/src/bob/io/base/testing_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4529 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/src/bob/io/image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.236806 bob.io.base-5.1.0/src/bob.io.base.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-16 11:58:17.000000 bob.io.base-5.1.0/src/bob.io.base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2023-06-16 11:58:17.000000 bob.io.base-5.1.0/src/bob.io.base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 11:58:17.000000 bob.io.base-5.1.0/src/bob.io.base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-16 11:58:17.000000 bob.io.base-5.1.0/src/bob.io.base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-16 11:58:17.000000 bob.io.base-5.1.0/src/bob.io.base.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 11:58:16.000000 bob.io.base-5.1.0/src/bob.io.base.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:58:17.240806 bob.io.base-5.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 11:57:54.000000 bob.io.base-5.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/tests/test_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/tests/test_image_support.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/tests/test_io.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-12 19:03:18.000000 bob.io.base-5.1.0/tests/test_utlilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.597329 bob.io.base-5.1.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-06-23 19:05:41.597329 bob.io.base-5.1.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.593329 bob.io.base-5.1.1b0/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.593329 bob.io.base-5.1.1b0/doc/img/
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/doc/img/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/doc/img/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/doc/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/doc/py_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:05:41.597329 bob.io.base-5.1.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.589329 bob.io.base-5.1.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.593329 bob.io.base-5.1.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.597329 bob.io.base-5.1.1b0/src/bob/io/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/src/bob/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.597329 bob.io.base-5.1.1b0/src/bob/io/base/
+-rw-rw-rw-   0 root         (0) root         (0)    12455 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/src/bob/io/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4537 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/src/bob/io/base/testing_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/src/bob/io/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.597329 bob.io.base-5.1.1b0/src/bob.io.base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-06-23 19:05:41.000000 bob.io.base-5.1.1b0/src/bob.io.base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2023-06-23 19:05:41.000000 bob.io.base-5.1.1b0/src/bob.io.base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:05:41.000000 bob.io.base-5.1.1b0/src/bob.io.base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-23 19:05:41.000000 bob.io.base-5.1.1b0/src/bob.io.base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 19:05:41.000000 bob.io.base-5.1.1b0/src/bob.io.base.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:05:41.000000 bob.io.base-5.1.1b0/src/bob.io.base.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:05:41.597329 bob.io.base-5.1.1b0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 19:05:17.000000 bob.io.base-5.1.1b0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/tests/test_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/tests/test_image_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/tests/test_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-19 19:03:16.000000 bob.io.base-5.1.1b0/tests/test_utlilities.py
```

### Comparing `bob.io.base-5.1.0/LICENSE` & `bob.io.base-5.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/PKG-INFO` & `bob.io.base-5.1.1b0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.io.base
-Version: 5.1.0
+Version: 5.1.1b0
 Summary: Basic IO for Bob
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/sphinx
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/sphinx
 Project-URL: homepage, https://pypi.org/project/bob.io.base
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.io.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.io.base/-/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -17,17 +17,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![latest-docs](https://img.shields.io/badge/docs-v5.1.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/sphinx/index.html)
-[![build](https://gitlab.idiap.ch/bob/bob.io.base/badges/v5.1.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.io.base/commits/v5.1.0)
-[![coverage](https://gitlab.idiap.ch/bob/bob.io.base/badges/v5.1.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/sphinx/index.html)
+[![build](https://gitlab.idiap.ch/bob/bob.io.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.io.base/commits/master)
+[![coverage](https://gitlab.idiap.ch/bob/bob.io.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.io.base)
 
 # bob.io.base
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains Bob's basic I/O functionality.
```

### Comparing `bob.io.base-5.1.0/README.md` & `bob.io.base-5.1.1b0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-[![latest-docs](https://img.shields.io/badge/docs-v5.1.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/sphinx/index.html)
-[![build](https://gitlab.idiap.ch/bob/bob.io.base/badges/v5.1.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.io.base/commits/v5.1.0)
-[![coverage](https://gitlab.idiap.ch/bob/bob.io.base/badges/v5.1.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/sphinx/index.html)
+[![build](https://gitlab.idiap.ch/bob/bob.io.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.io.base/commits/master)
+[![coverage](https://gitlab.idiap.ch/bob/bob.io.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.io.base)
 
 # bob.io.base
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains Bob's basic I/O functionality.
```

### Comparing `bob.io.base-5.1.0/doc/img/favicon.ico` & `bob.io.base-5.1.1b0/doc/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/doc/img/logo.png` & `bob.io.base-5.1.1b0/doc/img/logo.png`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/doc/index.rst` & `bob.io.base-5.1.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/doc/install.rst` & `bob.io.base-5.1.1b0/doc/install.rst`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/doc/py_api.rst` & `bob.io.base-5.1.1b0/doc/py_api.rst`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/pyproject.toml` & `bob.io.base-5.1.1b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
 name = "bob.io.base"
-version = "5.1.0"
+version = "5.1.1b0"
 requires-python = ">=3.9"
 description = "Basic IO for Bob"
 dynamic = ["readme"]
 license = {text = "BSD 3-Clause License"}
 authors = [
   {name = "Andre Anjos", email = "andre.anjos@idiap.ch"},
 ]
@@ -17,38 +17,38 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "bob==12.0.0",
-    "h5py==3.7.0",
-    "imageio==2.24.0",
-    "numpy==1.23.5",
-    "pillow==9.4.0",
+    "bob",
+    "h5py",
+    "imageio",
+    "numpy",
+    "pillow",
 ]
 
 [project.urls]
-documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/sphinx"
+documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/sphinx"
 homepage = "https://pypi.org/project/bob.io.base"
 repository = "https://gitlab.idiap.ch/bob/bob.io.base"
 changelog = "https://gitlab.idiap.ch/bob/bob.io.base/-/releases"
 
 [project.optional-dependencies]
 qa = ["pre-commit"]
 doc = [
-    "sphinx==5.3.0",
-    "sphinx-rtd-theme==1.1.1",
-    "auto-intersphinx==1.0.2",
+    "sphinx",
+    "sphinx_rtd_theme",
+    "auto-intersphinx",
     ]
 test = [
-    "pytest==7.2.1",
-    "pytest-cov==4.0.0",
-    "coverage==7.0.5",
+    "pytest",
+    "pytest-cov",
+    "coverage",
     ]
 
 [tool.setuptools]
 zip-safe = true
 package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
@@ -74,11 +74,7 @@
     "--import-mode=append",
     "--cov-report=term-missing",
     "--cov=bob.io.base",
 ]
 junit_logging = "all"
 junit_log_passing_tests = false
 norecursedirs = ["src/*"]
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.io.base-5.1.0/src/bob/io/base/__init__.py` & `bob.io.base-5.1.1b0/src/bob/io/base/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/src/bob/io/base/testing_utils.py` & `bob.io.base-5.1.1b0/src/bob/io/base/testing_utils.py`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/src/bob/io/image.py` & `bob.io.base-5.1.1b0/src/bob/io/image.py`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/src/bob.io.base.egg-info/PKG-INFO` & `bob.io.base-5.1.1b0/src/bob.io.base.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.io.base
-Version: 5.1.0
+Version: 5.1.1b0
 Summary: Basic IO for Bob
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/sphinx
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/sphinx
 Project-URL: homepage, https://pypi.org/project/bob.io.base
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.io.base
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.io.base/-/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -17,17 +17,17 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![latest-docs](https://img.shields.io/badge/docs-v5.1.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/sphinx/index.html)
-[![build](https://gitlab.idiap.ch/bob/bob.io.base/badges/v5.1.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.io.base/commits/v5.1.0)
-[![coverage](https://gitlab.idiap.ch/bob/bob.io.base/badges/v5.1.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/v5.1.0/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/sphinx/index.html)
+[![build](https://gitlab.idiap.ch/bob/bob.io.base/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.io.base/commits/master)
+[![coverage](https://gitlab.idiap.ch/bob/bob.io.base/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.io.base/master/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.io.base)
 
 # bob.io.base
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains Bob's basic I/O functionality.
```

### Comparing `bob.io.base-5.1.0/src/bob.io.base.egg-info/SOURCES.txt` & `bob.io.base-5.1.1b0/src/bob.io.base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/tests/test_hdf5.py` & `bob.io.base-5.1.1b0/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/tests/test_image_support.py` & `bob.io.base-5.1.1b0/tests/test_image_support.py`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/tests/test_io.py` & `bob.io.base-5.1.1b0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bob.io.base-5.1.0/tests/test_utlilities.py` & `bob.io.base-5.1.1b0/tests/test_utlilities.py`

 * *Files identical despite different names*

