# Comparing `tmp/bob.learn.em-3.3.0.tar.gz` & `tmp/bob.learn.em-3.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bob.learn.em-3.3.0.tar", last modified: Fri Jun 16 12:35:28 2023, max compression
+gzip compressed data, was "bob.learn.em-3.3.1b0.tar", last modified: Fri Jun 23 19:16:56 2023, max compression
```

## Comparing `bob.learn.em-3.3.0.tar` & `bob.learn.em-3.3.1b0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.363713 bob.learn.em-3.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3194 2023-06-16 12:35:28.363713 bob.learn.em-3.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-06-16 12:31:33.000000 bob.learn.em-3.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.355713 bob.learn.em-3.3.0/doc/
--rwxrwxrwx   0 root         (0) root         (0)     7217 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)    15573 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/doc/guide.rst
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3559 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/doc/py_api.rst
--rw-rw-rw-   0 root         (0) root         (0)     2426 2023-06-16 12:31:33.000000 bob.learn.em-3.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:35:28.363713 bob.learn.em-3.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.351713 bob.learn.em-3.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.355713 bob.learn.em-3.3.0/src/bob/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.359713 bob.learn.em-3.3.0/src/bob/learn/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.359713 bob.learn.em-3.3.0/src/bob/learn/em/
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    64905 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/factor_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    36780 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/gmm.py
--rw-rw-rw-   0 root         (0) root         (0)    11641 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/ivector.py
--rw-rw-rw-   0 root         (0) root         (0)    14475 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/kmeans.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/linear_scoring.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3100 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/wccn.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2023-06-12 19:12:08.000000 bob.learn.em-3.3.0/src/bob/learn/em/whitening.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.359713 bob.learn.em-3.3.0/src/bob.learn.em.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3194 2023-06-16 12:35:28.000000 bob.learn.em-3.3.0/src/bob.learn.em.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2023-06-16 12:35:28.000000 bob.learn.em-3.3.0/src/bob.learn.em.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:35:28.000000 bob.learn.em-3.3.0/src/bob.learn.em.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:35:28.000000 bob.learn.em-3.3.0/src/bob.learn.em.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      281 2023-06-16 12:35:28.000000 bob.learn.em-3.3.0/src/bob.learn.em.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-16 12:35:28.000000 bob.learn.em-3.3.0/src/bob.learn.em.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:35:28.363713 bob.learn.em-3.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-12 19:12:09.000000 bob.learn.em-3.3.0/tests/test_factor_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    35521 2023-06-12 19:12:09.000000 bob.learn.em-3.3.0/tests/test_gmm.py
--rw-rw-rw-   0 root         (0) root         (0)     9695 2023-06-12 19:12:09.000000 bob.learn.em-3.3.0/tests/test_ivector.py
--rw-rw-rw-   0 root         (0) root         (0)     6244 2023-06-12 19:12:09.000000 bob.learn.em-3.3.0/tests/test_kmeans.py
--rw-rw-rw-   0 root         (0) root         (0)     3867 2023-06-12 19:12:09.000000 bob.learn.em-3.3.0/tests/test_linear.py
--rw-rw-rw-   0 root         (0) root         (0)     7024 2023-06-12 19:12:09.000000 bob.learn.em-3.3.0/tests/test_linearscoring.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-12 19:12:09.000000 bob.learn.em-3.3.0/tests/test_picklability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.191052 bob.learn.em-3.3.1b0/
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-06-23 19:16:56.187052 bob.learn.em-3.3.1b0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.183052 bob.learn.em-3.3.1b0/doc/
+-rwxrwxrwx   0 root         (0) root         (0)     7217 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)    15573 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/doc/guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/doc/links.rst
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/doc/py_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 19:16:56.191052 bob.learn.em-3.3.1b0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.179052 bob.learn.em-3.3.1b0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.183052 bob.learn.em-3.3.1b0/src/bob/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.183052 bob.learn.em-3.3.1b0/src/bob/learn/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.187052 bob.learn.em-3.3.1b0/src/bob/learn/em/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    64905 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/factor_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    36780 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/gmm.py
+-rw-rw-rw-   0 root         (0) root         (0)    11641 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/ivector.py
+-rw-rw-rw-   0 root         (0) root         (0)    14475 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/kmeans.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/linear_scoring.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3100 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/wccn.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/src/bob/learn/em/whitening.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.183052 bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-06-23 19:16:56.000000 bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2023-06-23 19:16:56.000000 bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:16:56.000000 bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 19:16:55.000000 bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-23 19:16:56.000000 bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-23 19:16:56.000000 bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 19:16:56.187052 bob.learn.em-3.3.1b0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/tests/test_factor_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    35521 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/tests/test_gmm.py
+-rw-rw-rw-   0 root         (0) root         (0)     9695 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/tests/test_ivector.py
+-rw-rw-rw-   0 root         (0) root         (0)     6244 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/tests/test_kmeans.py
+-rw-rw-rw-   0 root         (0) root         (0)     3867 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/tests/test_linear.py
+-rw-rw-rw-   0 root         (0) root         (0)     7024 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/tests/test_linearscoring.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-23 19:12:41.000000 bob.learn.em-3.3.1b0/tests/test_picklability.py
```

### Comparing `bob.learn.em-3.3.0/LICENSE` & `bob.learn.em-3.3.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/PKG-INFO` & `bob.learn.em-3.3.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.learn.em
-Version: 3.3.0
+Version: 3.3.1b0
 Summary: Bindings for EM machines and trainers of Bob
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.learn.em/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.learn.em
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.learn.em/-/releases
 Keywords: bob,em,expectation-maximization
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 
-[![badge doc](https://img.shields.io/badge/docs-v3.3.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.learn.em/badges/v3.3.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.learn.em/commits/v3.3.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.learn.em/badges/v3.3.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.learn.em/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.learn.em/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.learn.em/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.learn.em)
 
 # Expectation Maximization Machine Learning Tools
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains routines for learning
 probabilistic models via Expectation Maximization (EM).
```

### Comparing `bob.learn.em-3.3.0/README.md` & `bob.learn.em-3.3.1b0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-[![badge doc](https://img.shields.io/badge/docs-v3.3.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.learn.em/badges/v3.3.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.learn.em/commits/v3.3.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.learn.em/badges/v3.3.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.learn.em/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.learn.em/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.learn.em/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.learn.em)
 
 # Expectation Maximization Machine Learning Tools
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains routines for learning
 probabilistic models via Expectation Maximization (EM).
```

### Comparing `bob.learn.em-3.3.0/doc/conf.py` & `bob.learn.em-3.3.1b0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/doc/guide.rst` & `bob.learn.em-3.3.1b0/doc/guide.rst`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/doc/index.rst` & `bob.learn.em-3.3.1b0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/doc/links.rst` & `bob.learn.em-3.3.1b0/doc/links.rst`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/doc/py_api.rst` & `bob.learn.em-3.3.1b0/doc/py_api.rst`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/pyproject.toml` & `bob.learn.em-3.3.1b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0.0", "wheel"]
     build-backend = "setuptools.build_meta"
 
 [project]
     name = "bob.learn.em"
-    version = "3.3.0"
+    version = "3.3.1b0"
     requires-python = ">=3.9"
     description = "Bindings for EM machines and trainers of Bob"
     dynamic = ["readme"]
     license = {text = "BSD 3-Clause License"}
     authors = [
     {name = "Andre Anjos", email = "andre.anjos@idiap.ch"},
     ]
@@ -21,40 +21,40 @@
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
     dependencies = [
-        "bob==12.0.0",
-        "dask==2023.1.0",
-        "dask-ml==2022.5.27",
-        "h5py==3.7.0",
-        "scikit-learn==1.1.2",
+        "bob",
+        "dask",
+        "dask-ml",
+        "h5py",
+        "scikit-learn",
     ]
 
 [project.urls]
-    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/sphinx/"
+    documentation = "https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/sphinx/"
     homepage = "https://pypi.org/project/bob.learn.em/"
     repository = "https://gitlab.idiap.ch/bob/bob.learn.em"
     changelog = "https://gitlab.idiap.ch/bob/bob.learn.em/-/releases"
 
 [project.optional-dependencies]
     qa = ["pre-commit"]
     doc = [
-        "sphinx==5.3.0",
-        "sphinx-rtd-theme==1.1.1",
-        "sphinx-autodoc-typehints==1.21.8",
-        "sphinxcontrib-programoutput==0.17",
-        "matplotlib==3.6.2",
+        "sphinx",
+        "sphinx_rtd_theme",
+        "sphinx-autodoc-typehints",
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
@@ -79,11 +79,7 @@
     addopts = [
         "--import-mode=append",
         "--cov-report=term-missing",
         "--cov=bob.learn.em",
     ]
     junit_logging = "all"
     junit_log_passing_tests = false
-
-[profile]
-    repository_url = "git@gitlab.idiap.ch:bob/dev-profile.git"
-    commit_hash = "ade723be1f11feddb7bece235de32cc98953dc07"
```

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/__init__.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/__init__.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/factor_analysis.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/factor_analysis.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/gmm.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/gmm.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/ivector.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/ivector.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/kmeans.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/kmeans.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/linear_scoring.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/linear_scoring.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/utils.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/utils.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/wccn.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/wccn.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob/learn/em/whitening.py` & `bob.learn.em-3.3.1b0/src/bob/learn/em/whitening.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/src/bob.learn.em.egg-info/PKG-INFO` & `bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bob.learn.em
-Version: 3.3.0
+Version: 3.3.1b0
 Summary: Bindings for EM machines and trainers of Bob
 Author-email: Andre Anjos <andre.anjos@idiap.ch>
 License: BSD 3-Clause License
-Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/sphinx/
+Project-URL: documentation, https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/sphinx/
 Project-URL: homepage, https://pypi.org/project/bob.learn.em/
 Project-URL: repository, https://gitlab.idiap.ch/bob/bob.learn.em
 Project-URL: changelog, https://gitlab.idiap.ch/bob/bob.learn.em/-/releases
 Keywords: bob,em,expectation-maximization
 Classifier: Framework :: Bob
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: qa
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 
-[![badge doc](https://img.shields.io/badge/docs-v3.3.0-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/sphinx/index.html)
-[![badge pipeline](https://gitlab.idiap.ch/bob/bob.learn.em/badges/v3.3.0/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.learn.em/commits/v3.3.0)
-[![badge coverage](https://gitlab.idiap.ch/bob/bob.learn.em/badges/v3.3.0/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/v3.3.0/coverage)
+[![badge doc](https://img.shields.io/badge/docs-latest-orange.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/sphinx/index.html)
+[![badge pipeline](https://gitlab.idiap.ch/bob/bob.learn.em/badges/master/pipeline.svg)](https://gitlab.idiap.ch/bob/bob.learn.em/commits/master)
+[![badge coverage](https://gitlab.idiap.ch/bob/bob.learn.em/badges/master/coverage.svg)](https://www.idiap.ch/software/bob/docs/bob/bob.learn.em/master/coverage)
 [![badge gitlab](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/bob/bob.learn.em)
 
 # Expectation Maximization Machine Learning Tools
 
 This package is part of the signal-processing and machine learning toolbox
 [Bob](https://www.idiap.ch/software/bob). It contains routines for learning
 probabilistic models via Expectation Maximization (EM).
```

### Comparing `bob.learn.em-3.3.0/src/bob.learn.em.egg-info/SOURCES.txt` & `bob.learn.em-3.3.1b0/src/bob.learn.em.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/tests/test_factor_analysis.py` & `bob.learn.em-3.3.1b0/tests/test_factor_analysis.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/tests/test_gmm.py` & `bob.learn.em-3.3.1b0/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/tests/test_ivector.py` & `bob.learn.em-3.3.1b0/tests/test_ivector.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/tests/test_kmeans.py` & `bob.learn.em-3.3.1b0/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/tests/test_linear.py` & `bob.learn.em-3.3.1b0/tests/test_linear.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/tests/test_linearscoring.py` & `bob.learn.em-3.3.1b0/tests/test_linearscoring.py`

 * *Files identical despite different names*

### Comparing `bob.learn.em-3.3.0/tests/test_picklability.py` & `bob.learn.em-3.3.1b0/tests/test_picklability.py`

 * *Files identical despite different names*

