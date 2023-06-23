# Comparing `tmp/geocat.comp-2023.5.0.tar.gz` & `tmp/geocat.comp-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocat.comp-2023.5.0.tar", last modified: Fri May  5 15:41:27 2023, max compression
+gzip compressed data, was "geocat.comp-2023.6.0.tar", last modified: Fri Jun 23 21:03:47 2023, max compression
```

## Comparing `geocat.comp-2023.5.0.tar` & `geocat.comp-2023.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/build_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/build_envs/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/build_envs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/build_envs/upstream-dev-environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-05 15:41:27.630870 geocat.comp-2023.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.622870 geocat.comp-2023.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/src/geocat/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/src/geocat/comp/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30249 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/climatologies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/fourier_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/gc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    54706 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/meteorology.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/src/geocat.comp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.721020 geocat.comp-2023.6.0/build_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/build_envs/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/build_envs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/build_envs/upstream-dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.721020 geocat.comp-2023.6.0/geocat/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/geocat/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/climatologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/fourier_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/gc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26716 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54706 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/meteorology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/geocat/comp/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:03:47.721020 geocat.comp-2023.6.0/geocat.comp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 21:03:47.000000 geocat.comp-2023.6.0/geocat.comp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-23 21:03:47.725020 geocat.comp-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 21:03:32.000000 geocat.comp-2023.6.0/setup.py
```

### Comparing `geocat.comp-2023.5.0/.gitignore` & `geocat.comp-2023.6.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /build/
 
 # Dask
-/src/geocat/comp/dask-worker-space/
+geocat/comp/dask-worker-space/
 
 
 # Created by https://www.gitignore.io/api/python,intellij,intellij+all,intellij+iml
 # Edit at https://www.gitignore.io/?templates=python,intellij,intellij+all,intellij+iml
 
 ### Intellij ###
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio and WebStorm
```

### Comparing `geocat.comp-2023.5.0/.pre-commit-config.yaml` & `geocat.comp-2023.6.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
--   repo: https://github.com/pre-commit/mirrors-yapf    # To format the code to conform YAPF
-    rev: v0.31.0
+-   repo: https://github.com/google/yapf    # To format the code to conform YAPF
+    rev: v0.33.0
     hooks:
       - id: yapf
         args: ['--in-place', '--recursive', '--style', 'google']
 
 -   repo: https://github.com/myint/docformatter    # To format the doc strings to conform PEP257
     rev: v1.4
     hooks:
```

### Comparing `geocat.comp-2023.5.0/CONTRIBUTING.md` & `geocat.comp-2023.6.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 contribution guidelines (such as detailed description of GeoCAT structure, forking, repository cloning,
 branching, etc.). Once you determine that a function should be contributed under this repo, please refer to the
 following contribution guidelines:
 
 # Adding new functions to the Geocat-comp repo
 
 1. For a new function or family of functions that handle similar computations, create a new Python file in
-`$GEOCATCOMP/src/geocat/comp/`.
+`$GEOCATCOMP/geocat/comp/`.
 
 2. For implementation guidelines (such as Xarray and Dask usage), please refer to:
    - Previously implemented functionality as examples,
-    e.g. [polynomial.py](https://github.com/NCAR/geocat-comp/blob/main/src/geocat/comp/polynomial.py) or others.
+    e.g. [polynomial.py](https://github.com/NCAR/geocat-comp/blob/main/geocat/comp/polynomial.py) or others.
    - [GeoCAT Contributor's Guide](https://geocat.ucar.edu/pages/contributing.html) for further information.
 
-3. In any Python script under `$GEOCATCOMP/src/geocat/comp/`, there may be user API functions, which are
+3. In any Python script under `$GEOCATCOMP/geocat/comp/`, there may be user API functions, which are
 supposed to be included in the `geocat.comp` namespace, and internal API functions, which are used by the
 user API functions as helpers, preferably starts with an underscore ("_") in their names, as well as are
 not included in the `geocat.comp` namespace.
 
-4. The user API functions should be imported in `$GEOCATCOMP/src/geocat/comp/__init__.py` to be included in
+4. The user API functions should be imported in `$GEOCATCOMP/geocat/comp/__init__.py` to be included in
 the namespace.
 
 5. For appropriate documentation, each user API and internal API function should be listed in the
 `$GEOCATCOMP/docs/user_api/index.rst` and `$GEOCATCOMP/docs/internal_api/index.rst`, respectively.
 
 # Adding unit tests
```

### Comparing `geocat.comp-2023.5.0/LICENSE` & `geocat.comp-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.5.0/PKG-INFO` & `geocat.comp-2023.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: geocat.comp
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: GeoCAT-comp is computational component of the GeoCAT project and
 Home-page: https://geocat-comp.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.11,>=3.8
+Requires-Python: <=3.11,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 | CI           | [![GitHub Workflow Status][github-ci-badge]][github-ci-link] [![GitHub Workflow Status][github-upstream-ci-badge]][github-upstream-ci-link] [![Code Coverage Status][codecov-badge]][codecov-link] |
 | :----------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 | **Docs**     |                                                                    [![Documentation Status][rtd-badge]][rtd-link]                                                                    |
 | **Package**  |                                                         [![Conda][conda-badge]][conda-link] [![PyPI][pypi-badge]][pypi-link]                                                         |
@@ -30,35 +30,14 @@
 
 GeoCAT-comp is both the whole computational component of the [GeoCAT](https://geocat.ucar.edu/)
 project and a single Github repository as described here. As the computational component of
 [GeoCAT](https://geocat.ucar.edu/), GeoCAT-comp provides implementations of computational functions for operating
 on geosciences data. Many of these functions originated in NCL and were translated into Python with the help of GeoCAT-comp;
 however, developers are welcome to come up with novel computational functions for geosciences data.
 
-Many of the computational functions in GeoCAT are implemented in a pure Python fashion. However,
-there are some others that are implemented in Fortran but wrapped up in Python. To facilitate
-contribution, the whole GeoCAT-comp structure is split into two repositories with respect to
-being pure-Python or Python with compiled codes (i.e. Fortran) implementations. Such implementation
-layers are handled within [GeoCAT-comp](https://github.com/NCAR/geocat-comp) and
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py) repositories, respectively (The
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py) repo is documented on its own).
-
-
-# GeoCAT-comp
-
-GeoCAT-comp repo does not explicitly contain or require any compiled code, making it more
-accessible to the general Python community at large. However, if
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py) is installed, then all functions contained in
-the "geocat.f2py" package are imported seamlessly into the "geocat.comp" namespace. Thus,
-GeoCAT-comp repo serves as a user API to access the entire computational toolkit even though the
-repo itself only contains pure Python code from the contributor’s perspective. Whenever prospective
-contributors want to add new computational functionality implemented as pure Python, GeoCAT-comp
-is the repo to do so. Therefore, there is no onus on contributors of pure python code to
-build/compile/test any compiled code (i.e. Fortran) at GeoCAT-comp level.
-
 
 # Documentation
 
 [GeoCAT Homepage](https://geocat.ucar.edu/)
 
 [GeoCAT Contributor's Guide](https://geocat.ucar.edu/pages/contributing.html)
 
@@ -67,23 +46,14 @@
 
 # Installation and build instructions
 
 Please see our documentation for
 [installation and build instructions](https://github.com/NCAR/geocat-comp/blob/main/INSTALLATION.md).
 
 
-# Xarray interface vs NumPy interface
-
-GeoCAT-comp provides a high-level [Xarray](http://xarray.pydata.org/en/stable/) interface under the
-`geocat.comp` namespace. However, a stripped-down NumPy interface is used under the hood to bridge
-the gap between NumPy arrays and the compiled language data structures used by
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py). These functions are accessible under the
-`geocat.comp` namespace, but are minimally documented and are
-intended primarily for internal use.
-
 # Citing GeoCAT-comp
 
 If you use this software, please cite it as described at the [GeoCAT-comp - Citation](
 https://geocat-comp.readthedocs.io/en/latest/citation.html) page.
 
 
 [github-ci-badge]: https://img.shields.io/github/actions/workflow/status/NCAR/geocat-comp/ci.yml?branch=main&label=CI&style=for-the-badge
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geocat.comp-2023.5.0/README.md` & `geocat.comp-2023.6.0/geocat.comp.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: geocat.comp
+Version: 2023.6.0
+Summary: GeoCAT-comp is computational component of the GeoCAT project and
+Home-page: https://geocat-comp.readthedocs.io
+Author: GeoCAT Team
+Author-email: geocat@ucar.edu
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: <=3.11,>=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+
 | CI           | [![GitHub Workflow Status][github-ci-badge]][github-ci-link] [![GitHub Workflow Status][github-upstream-ci-badge]][github-upstream-ci-link] [![Code Coverage Status][codecov-badge]][codecov-link] |
 | :----------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 | **Docs**     |                                                                    [![Documentation Status][rtd-badge]][rtd-link]                                                                    |
 | **Package**  |                                                         [![Conda][conda-badge]][conda-link] [![PyPI][pypi-badge]][pypi-link]                                                         |
 | **License**  |                                                                        [![License][license-badge]][repo-link]                                                                        |
 | **Citing**  |                                                                              [![DOI][doi-badge]][doi-link]                                                                            |
 
@@ -9,35 +30,14 @@
 
 GeoCAT-comp is both the whole computational component of the [GeoCAT](https://geocat.ucar.edu/)
 project and a single Github repository as described here. As the computational component of
 [GeoCAT](https://geocat.ucar.edu/), GeoCAT-comp provides implementations of computational functions for operating
 on geosciences data. Many of these functions originated in NCL and were translated into Python with the help of GeoCAT-comp;
 however, developers are welcome to come up with novel computational functions for geosciences data.
 
-Many of the computational functions in GeoCAT are implemented in a pure Python fashion. However,
-there are some others that are implemented in Fortran but wrapped up in Python. To facilitate
-contribution, the whole GeoCAT-comp structure is split into two repositories with respect to
-being pure-Python or Python with compiled codes (i.e. Fortran) implementations. Such implementation
-layers are handled within [GeoCAT-comp](https://github.com/NCAR/geocat-comp) and
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py) repositories, respectively (The
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py) repo is documented on its own).
-
-
-# GeoCAT-comp
-
-GeoCAT-comp repo does not explicitly contain or require any compiled code, making it more
-accessible to the general Python community at large. However, if
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py) is installed, then all functions contained in
-the "geocat.f2py" package are imported seamlessly into the "geocat.comp" namespace. Thus,
-GeoCAT-comp repo serves as a user API to access the entire computational toolkit even though the
-repo itself only contains pure Python code from the contributor’s perspective. Whenever prospective
-contributors want to add new computational functionality implemented as pure Python, GeoCAT-comp
-is the repo to do so. Therefore, there is no onus on contributors of pure python code to
-build/compile/test any compiled code (i.e. Fortran) at GeoCAT-comp level.
-
 
 # Documentation
 
 [GeoCAT Homepage](https://geocat.ucar.edu/)
 
 [GeoCAT Contributor's Guide](https://geocat.ucar.edu/pages/contributing.html)
 
@@ -46,23 +46,14 @@
 
 # Installation and build instructions
 
 Please see our documentation for
 [installation and build instructions](https://github.com/NCAR/geocat-comp/blob/main/INSTALLATION.md).
 
 
-# Xarray interface vs NumPy interface
-
-GeoCAT-comp provides a high-level [Xarray](http://xarray.pydata.org/en/stable/) interface under the
-`geocat.comp` namespace. However, a stripped-down NumPy interface is used under the hood to bridge
-the gap between NumPy arrays and the compiled language data structures used by
-[GeoCAT-f2py](https://github.com/NCAR/geocat-f2py). These functions are accessible under the
-`geocat.comp` namespace, but are minimally documented and are
-intended primarily for internal use.
-
 # Citing GeoCAT-comp
 
 If you use this software, please cite it as described at the [GeoCAT-comp - Citation](
 https://geocat-comp.readthedocs.io/en/latest/citation.html) page.
 
 
 [github-ci-badge]: https://img.shields.io/github/actions/workflow/status/NCAR/geocat-comp/ci.yml?branch=main&label=CI&style=for-the-badge
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geocat.comp-2023.5.0/build_envs/environment.yml` & `geocat.comp-2023.6.0/build_envs/environment.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 name: geocat_comp_build
 channels:
   - conda-forge
 dependencies:
-  - python>=3.8, <3.11  # minimum support 3.8, 3.11 not yet fully supported
+  - python>=3.9, <=3.11  # minimum support 3.9
   - cf_xarray>=0.3.1    # min version 0.3.1 for dependencies
   - cftime
   - dask
   - distributed
   - eofs
-  - geocat-f2py
   - metpy
   - numba
   - numpy<1.24  # 1.24 not yet fully compatible with numba
   - pint
   - xarray<=2023.02.0 #pin per issue #381
   - xskillscore
 # Packages listed below are for testing
```

### Comparing `geocat.comp-2023.5.0/setup.cfg` & `geocat.comp-2023.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -13,38 +13,34 @@
 license_files = file: LICENSE
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = >=3.8, <3.11
-package_dir = 
-	=src
+python_requires = >=3.9, <=3.11
 packages = 
 	geocat
 	geocat.comp
 setup_requires = 
 	setuptools_scm
 	setuptools
 	pip
-	geocat.f2py
 install_requires = 
 	cf_xarray>=0.3.1
 	cftime
 	eofs
-	geocat.f2py
 	metpy
 	scipy
 	xarray
 	xskillscore
 	packaging
 tests_require = 
 	pytest
```

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/__init__.py` & `geocat.comp-2023.6.0/geocat/comp/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,57 @@
 # move functions into geocat.comp namespace
-from .climatologies import anomaly, climatology, month_to_season, calendar_average, climatology_average, climate_anomaly
-from .fourier_filters import (fourier_band_block, fourier_band_pass,
-                              fourier_filter, fourier_high_pass,
-                              fourier_low_pass)
+from .climatologies import (
+    month_to_season,
+    calendar_average,
+    climatology_average,
+    climate_anomaly,
+)
+from .fourier_filters import (
+    fourier_band_block,
+    fourier_band_pass,
+    fourier_filter,
+    fourier_high_pass,
+    fourier_low_pass,
+)
 from .gradient import gradient, _arc_lon_wgs84, _arc_lat_wgs84, _rad_lat_wgs84
-from .interpolation import interp_hybrid_to_pressure, interp_sigma_to_hybrid, interp_multidim
-from .meteorology import (dewtemp, heat_index, relhum, relhum_ice, relhum_water,
-                          actual_saturation_vapor_pressure, max_daylight,
-                          psychrometric_constant, saturation_vapor_pressure,
-                          saturation_vapor_pressure_slope, delta_pressure,
-                          dpres_plev)
+from .interpolation import (
+    interp_hybrid_to_pressure,
+    interp_sigma_to_hybrid,
+    interp_multidim,
+)
+from .meteorology import (
+    dewtemp,
+    heat_index,
+    relhum,
+    relhum_ice,
+    relhum_water,
+    actual_saturation_vapor_pressure,
+    max_daylight,
+    psychrometric_constant,
+    saturation_vapor_pressure,
+    saturation_vapor_pressure_slope,
+    delta_pressure,
+    dpres_plev,
+)
 from .spherical import decomposition, recomposition, scale_voronoi
 from .stats import eofunc, eofunc_eofs, eofunc_pcs, eofunc_ts, pearson_r
-# bring all functions from geocat.f2py into the geocat.comp namespace
-try:
-    from geocat.f2py import *
-except ImportError:
-    pass
+from .deprecated import (
+    grid_to_triple,
+    linint1,
+    linint2,
+    linint2pts,
+    moc_globe_atl,
+    rcm2points,
+    rcm2rgrid,
+    rgrid2rcm,
+    triple_to_grid,
+)
 
 # get version from pyproject.toml
 from importlib.metadata import version as _version
+
 try:
     __version__ = _version("geocat.comp")
 except Exception:
     # Local copy or not installed with setuptools.
     # Disable minimum version checks on downstream libraries.
     __version__ = "999"
```

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/climatologies.py` & `geocat.comp-2023.6.0/geocat/comp/climatologies.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,14 @@
 import numpy as np
 import typing
 import xarray as xr
 
 _FREQUENCIES = {"day", "month", "year", "season"}
 
 
-def _find_time_invariant_vars(dset, time_coord_name):
-    if isinstance(dset, xr.Dataset):
-        return [
-            v for v in dset.variables if time_coord_name not in dset[v].dims
-        ]
-    return
-
-
 def _contains_datetime_like_objects(d_arr):
     """Check if a variable contains datetime like objects (either
     np.datetime64, or cftime.datetime)"""
     return np.issubdtype(
         d_arr.dtype,
         np.datetime64) or xr.core.common.contains_cftime_datetimes(d_arr)
 
@@ -41,28 +33,14 @@
         raise ValueError(
             f"The {time_coord_name} coordinate should be either `np.datetime64` or `cftime.datetime`"
         )
 
     return time_coord_name
 
 
-def _setup_clim_anom_input(dset, freq, time_coord_name):
-    _validate_freq(freq)
-
-    time_coord_name = _get_time_coordinate_info(dset, time_coord_name)
-    time_invariant_vars = _find_time_invariant_vars(dset, time_coord_name)
-    if time_invariant_vars:
-        data = dset.drop_vars(time_invariant_vars)
-    else:
-        data = dset
-    time_dot_freq = ".".join([time_coord_name, freq])
-
-    return data, time_invariant_vars, time_coord_name, time_dot_freq
-
-
 def _calculate_center_of_time_bounds(
         dset: typing.Union[xr.Dataset, xr.DataArray],
         time_dim: str,
         freq: str,
         calendar: str,
         start: typing.Union[str, cftime.datetime],
         end: typing.Union[str, cftime.datetime],
@@ -127,229 +105,14 @@
     """
     if np.asarray(dates).dtype == "datetime64[ns]":
         return "proleptic_gregorian"
     else:
         return np.asarray(dates).ravel()[0].calendar
 
 
-def climatology(
-        dset: typing.Union[xr.DataArray, xr.Dataset],
-        freq: str,
-        time_coord_name: str = None,
-        keep_attrs: bool = None) -> typing.Union[xr.DataArray, xr.Dataset]:
-    r""".. deprecated:: 2023.02.0 The ``climatology`` function is deprecated due to
-        inaccuracies in monthly climatology calculations and when using monthly
-        data to calculate seasonal or yearly climatologies. Use
-        `climatology_average <https://geocat-comp.readthedocs.io/en/stable/user_api/generated/geocat.comp.climatologies.climatology_average.html>`__
-        instead.
-
-    Compute climatologies for a specified time frequency.
-
-    Parameters
-    ----------
-    dset : :class:`xarray.Dataset`, :class:`xarray.DataArray`
-        The data on which to operate
-
-    freq : str
-        Climatology frequency alias. Accepted alias:
-
-        - `day`: for daily climatologies
-        - `month`: for monthly climatologies
-        - `year`: for annual climatologies
-        - `season': for seasonal climatologies
-
-    time_coord_name : str, optional
-         Name for time coordinate to use. Defaults to ``None`` and infers the name
-         from the data.
-
-    keep_attrs : bool, optional
-        If True, attrs will be copied from the original object to the new one.
-        If False, the new object will be returned without attributes.
-        Defaults to None which means the attrs will only be kept in unambiguous circumstances.
-
-    Returns
-    -------
-    computed_dset : :class:`xarray.Dataset`, :class:`xarray.DataArray`
-       The computed climatology data
-
-    Examples
-    --------
-    >>> import xarray as xr
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> import geocat.comp
-    >>> # Create toy data set
-    >>> dates = pd.date_range(start="2000/01/01",
-    ...                       freq="M",
-    ...                       periods=24)
-    >>> ts = xr.DataArray(np.arange(24).reshape(24, 1, 1),
-    ...                   dims=["time", "lat", "lon"],
-    ...                   coords={"time": dates})
-    >>> ts
-    <xarray.DataArray (time: 24, lat: 1, lon: 1)>
-    array([[[ 0]],
-        [[ 1]],
-        [[ 2]],
-    <BLANKLINE>
-        [[21]],
-        [[22]],
-        [[23]]])
-    Coordinates:
-    * time     (time) datetime64[ns] 2000-01-31 2000-02-29 ... 2001-12-31
-    Dimensions without coordinates: lat, lon
-
-    >>> # Calculate yearly climate averages
-    >>> geocat.comp.climatology(ts, 'year')
-    <xarray.DataArray (year: 2, lat: 1, lon: 1)>
-    array([[[ 5.5]],
-        [[17.5]]])
-    Coordinates:
-    * year     (year) int64 2000 2001
-    Dimensions without coordinates: lat, lon
-
-    >>> # Calculate seasonal climate averages
-    >>> geocat.comp.climatology(ts, 'season')
-    <xarray.DataArray (season: 4, lat: 1, lon: 1)>
-    array([[[10.]],
-        [[12.]],
-        [[ 9.]],
-        [[15.]]])
-    Coordinates:
-    * season   (season) object 'DJF' 'JJA' 'MAM' 'SON'
-    Dimensions without coordinates: lat, lon
-
-    See Also
-    --------
-    Related GeoCAT Functions:
-    :func:`climatology_average`
-
-    Related NCL Functions:
-    `clmDayTLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/clmDayTLL.shtml>`__,
-    `clmDayTLLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/clmDayTLLL.shtml>`__,
-    `clmMonLLLT <https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonLLLT.shtml>`__,
-    `clmMonLLT <https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonLLT.shtml>`__,
-    `clmMonTLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonTLL.shtml>`__,
-    `clmMonTLLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonTLLL.shtml>`__,
-    `month_to_season <https://www.ncl.ucar.edu/Document/Functions/Contributed/month_to_season.shtml>`__
-    """
-    data, time_invariant_vars, time_coord_name, time_dot_freq = _setup_clim_anom_input(
-        dset, freq, time_coord_name)
-
-    grouped = data.groupby(time_dot_freq)
-    # TODO: Compute weighted climatologies when `time_bounds` are available
-    clim = grouped.mean(time_coord_name, keep_attrs=keep_attrs)
-    if time_invariant_vars:
-        if keep_attrs == False:
-            return xr.concat([dset[time_invariant_vars], clim],
-                             combine_attrs='drop',
-                             dim=time_coord_name)
-        else:
-            return xr.concat([dset[time_invariant_vars], clim],
-                             dim=time_coord_name)
-    else:
-        return clim
-
-
-def anomaly(
-        dset: typing.Union[xr.DataArray, xr.Dataset],
-        freq: str,
-        time_coord_name: str = None) -> typing.Union[xr.DataArray, xr.Dataset]:
-    r""".. deprecated:: 2023.02.0 The ``anomaly`` function is deprecated due to
-        inaccuracies in monthly anomaly calculations and when using monthly
-        data to calculate seasonal or yearly anomalies. Use `climate_anomaly <https://geocat-comp.readthedocs.io/en/stable/user_api/generated/geocat.comp.climatologies.climate_anomaly.html>`__
-        instead.
-
-    Parameters
-    ----------
-    dset : :class:`xarray.Dataset`, :class:`xarray.DataArray`
-        The data on which to operate
-
-    freq : str
-        Anomaly frequency alias. Accepted alias:
-
-        - `day`: for daily anomalies
-        - `month`: for monthly anomalies
-        - `year`: for annual anomalies
-        - `season`: for seasonal anomalies
-
-    time_coord_name : str, optional
-         Name for time coordinate to use. Defaults to ``None`` and infers the name
-         from the data.
-
-    Returns
-    -------
-    computed_dset : :class:`xarray.Dataset`, :class:`xarray.DataArray`
-       The computed anomaly data
-
-    Examples
-    --------
-    >>> import xarray as xr
-    >>> import pandas as pd
-    >>> import numpy as np
-    >>> import geocat.comp
-    >>> # Create toy data
-    >>> dates = pd.date_range(start="2000/01/01",
-    ...                       freq="M",
-    ...                       dates=24)
-    >>> ts = xr.DataArray(np.arange(24).reshape(24, 1, 1),
-    ...                   dims=["time", "lat", "lon"],
-    ...                   coords={"time": dates})
-    >>> ts
-    <xarray.DataArray (time: 24, lat: 1, lon: 1)>
-    array([[[ 0]],
-        [[ 1]],
-        [[ 2]],
-    <BLANKLINE>
-        [[21]],
-        [[22]],
-        [[23]]])
-    Coordinates:
-    * time     (time) datetime64[ns] 2000-01-31 2000-02-29 ... 2001-12-31
-    Dimensions without coordinates: lat, lon
-
-    >>> # Compute seasonal anomalies
-    >>> geocat.comp.anomaly(ts, 'season')
-    <xarray.DataArray (time: 24, lat: 1, lon: 1)>
-    array([[[-10.]],
-        [[ -9.]],
-        [[ -7.]],
-    <BLANKLINE>
-        [[  6.]],
-        [[  7.]],
-        [[ 13.]]])
-    Coordinates:
-    * time     (time) datetime64[ns] 2000-01-31 2000-02-29 ... 2001-12-31
-        season   (time) <U3 'DJF' 'DJF' 'MAM' 'MAM' ... 'SON' 'SON' 'SON' 'DJF'
-    Dimensions without coordinates: lat, lon
-
-    See Also
-    --------
-    Related GeoCAT Functions:
-    :func:`climate_anomaly`
-
-    Related NCL Functions:
-    `clmDayAnomTLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/calcDayAnomTLL.shtml>`__,
-    `clmDayAnomTLLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/calcMonAnomTLLL.shtml>`__,
-    `clmMonAnomLLLT <https://www.ncl.ucar.edu/Document/Functions/Contributed/calcMonAnomLLLT.shtml>`__,
-    `clmMonAnomLLT <https://www.ncl.ucar.edu/Document/Functions/Contributed/calcMonAnomLLT.shtml>`__,
-    `clmMonAnomTLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/calcMonAnomTLL.shtml>`__,
-    `clmMonAnomTLLL <https://www.ncl.ucar.edu/Document/Functions/Contributed/calcMonAnomTLLL.shtml>`__
-    """
-
-    data, time_invariant_vars, time_coord_name, time_dot_freq = _setup_clim_anom_input(
-        dset, freq, time_coord_name)
-
-    clim = climatology(data, freq, time_coord_name)
-    anom = data.groupby(time_dot_freq) - clim
-    if time_invariant_vars:
-        return xr.merge([dset[time_invariant_vars], anom])
-    else:
-        return anom
-
-
 def climate_anomaly(
         dset: typing.Union[xr.DataArray, xr.Dataset],
         freq: str,
         time_dim: str = None,
         keep_attrs: bool = 'default') -> typing.Union[xr.DataArray, xr.Dataset]:
     """This function calculates climate anomalies by subtracting the long term
     mean of each ``freq`` period (day, month, season, or year) from each
```

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/fourier_filters.py` & `geocat.comp-2023.6.0/geocat/comp/fourier_filters.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/gc_util.py` & `geocat.comp-2023.6.0/geocat/comp/gc_util.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/gradient.py` & `geocat.comp-2023.6.0/geocat/comp/gradient.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/interpolation.py` & `geocat.comp-2023.6.0/geocat/comp/interpolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     hgt = phi_sfc * g_inv
     t0 = tstar + 0.0065 * hgt
     tplat = xr.apply_ufunc(np.minimum, 298, t0, dask='parallelized')
 
     tprime0 = xr.where((2000 <= hgt) & (hgt <= 2500),
                        0.002 * ((2500 - hgt) * t0 + ((hgt - 2000) * tplat)),
                        np.nan)
-    tprime0 = xr.where(2500 < hgt, tplat, np.nan)
+    tprime0 = xr.where(2500 < hgt, tplat, tprime0)
 
     alnp = xr.where(hgt < 2000, alpha * np.log(lev / ps),
                     R_d * (tprime0 - tstar) / phi_sfc * np.log(lev / ps))
     alnp = xr.where(tprime0 < tstar, 0, alnp)
 
     return tstar * (1 + alnp + (0.5 * (alnp**2)) + (1 / 6 * (alnp**3)))
```

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/meteorology.py` & `geocat.comp-2023.6.0/geocat/comp/meteorology.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/spherical.py` & `geocat.comp-2023.6.0/geocat/comp/spherical.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.5.0/src/geocat/comp/stats.py` & `geocat.comp-2023.6.0/geocat/comp/stats.py`

 * *Files identical despite different names*

