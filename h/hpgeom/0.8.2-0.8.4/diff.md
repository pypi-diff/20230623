# Comparing `tmp/hpgeom-0.8.2.tar.gz` & `tmp/hpgeom-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpgeom-0.8.2.tar", last modified: Fri Jul 15 20:03:24 2022, max compression
+gzip compressed data, was "hpgeom-0.8.4.tar", last modified: Fri Jun 23 02:49:14 2023, max compression
```

## Comparing `hpgeom-0.8.2.tar` & `hpgeom-0.8.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 20:03:24.377038 hpgeom-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-07-15 20:03:06.000000 hpgeom-0.8.2/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 20:03:24.373038 hpgeom-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 20:03:24.373038 hpgeom-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-07-15 20:03:06.000000 hpgeom-0.8.2/.github/workflows/python-package-pr.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-07-15 20:03:06.000000 hpgeom-0.8.2/.github/workflows/python-package-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-07-15 20:03:06.000000 hpgeom-0.8.2/.github/workflows/python-package-push.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-07-15 20:03:06.000000 hpgeom-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-15 20:03:06.000000 hpgeom-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-15 20:03:06.000000 hpgeom-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3288 2022-07-15 20:03:24.377038 hpgeom-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-07-15 20:03:06.000000 hpgeom-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 20:03:24.373038 hpgeom-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-07-15 20:03:06.000000 hpgeom-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3316 2022-07-15 20:03:06.000000 hpgeom-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-07-15 20:03:06.000000 hpgeom-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-07-15 20:03:06.000000 hpgeom-0.8.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-15 20:03:06.000000 hpgeom-0.8.2/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 20:03:24.373038 hpgeom-0.8.2/hpgeom/
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    56621 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/healpix_geom.c
--rw-r--r--   0 runner    (1001) docker     (121)     5380 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/healpix_geom.h
--rw-r--r--   0 runner    (1001) docker     (121)    14916 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/healpy_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    60442 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/hpgeom.c
--rw-r--r--   0 runner    (1001) docker     (121)    13129 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/hpgeom.py
--rw-r--r--   0 runner    (1001) docker     (121)    15551 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/hpgeom_stack.c
--rw-r--r--   0 runner    (1001) docker     (121)     4706 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/hpgeom_stack.h
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/hpgeom_utils.c
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-07-15 20:03:06.000000 hpgeom-0.8.2/hpgeom/hpgeom_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 20:03:24.377038 hpgeom-0.8.2/hpgeom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3288 2022-07-15 20:03:24.000000 hpgeom-0.8.2/hpgeom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-07-15 20:03:24.000000 hpgeom-0.8.2/hpgeom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 20:03:24.000000 hpgeom-0.8.2/hpgeom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-15 20:03:24.000000 hpgeom-0.8.2/hpgeom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-15 20:03:24.000000 hpgeom-0.8.2/hpgeom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 20:03:23.000000 hpgeom-0.8.2/hpgeom.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-07-15 20:03:06.000000 hpgeom-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-15 20:03:06.000000 hpgeom-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-07-15 20:03:24.377038 hpgeom-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-07-15 20:03:06.000000 hpgeom-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 20:03:24.377038 hpgeom-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5577 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/make_benchmark_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_angle_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6162 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_angle_to_pixel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4200 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (121)    13997 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_healpy_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_max_pixel_radius.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_nest_to_ring.py
--rw-r--r--   0 runner    (1001) docker     (121)     5805 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_pixel_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_pixel_to_angle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_pixel_to_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)    13567 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_query_box.py
--rw-r--r--   0 runner    (1001) docker     (121)     7109 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_query_circle.py
--rw-r--r--   0 runner    (1001) docker     (121)    12152 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_query_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)     8751 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_query_polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_ring_to_nest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_vector_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/test_vector_to_pixel.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-07-15 20:03:06.000000 hpgeom-0.8.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:49:14.007678 hpgeom-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 02:48:58.000000 hpgeom-0.8.4/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:49:13.999678 hpgeom-0.8.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:49:13.999678 hpgeom-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-23 02:48:58.000000 hpgeom-0.8.4/.github/workflows/python-package-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-23 02:48:58.000000 hpgeom-0.8.4/.github/workflows/python-package-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-23 02:48:58.000000 hpgeom-0.8.4/.github/workflows/python-package-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-23 02:48:58.000000 hpgeom-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-23 02:48:58.000000 hpgeom-0.8.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 02:48:58.000000 hpgeom-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 02:48:58.000000 hpgeom-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-23 02:49:14.007678 hpgeom-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-23 02:48:58.000000 hpgeom-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:49:13.999678 hpgeom-0.8.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-23 02:48:58.000000 hpgeom-0.8.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-23 02:48:58.000000 hpgeom-0.8.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-23 02:48:58.000000 hpgeom-0.8.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 02:48:58.000000 hpgeom-0.8.4/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 02:48:58.000000 hpgeom-0.8.4/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:49:14.003677 hpgeom-0.8.4/hpgeom/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56621 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/healpix_geom.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/healpix_geom.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/healpy_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60442 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/hpgeom.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/hpgeom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/hpgeom_stack.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/hpgeom_stack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/hpgeom_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-23 02:48:58.000000 hpgeom-0.8.4/hpgeom/hpgeom_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:49:14.003677 hpgeom-0.8.4/hpgeom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-23 02:49:13.000000 hpgeom-0.8.4/hpgeom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-23 02:49:13.000000 hpgeom-0.8.4/hpgeom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:49:13.000000 hpgeom-0.8.4/hpgeom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 02:49:13.000000 hpgeom-0.8.4/hpgeom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 02:49:13.000000 hpgeom-0.8.4/hpgeom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:49:13.000000 hpgeom-0.8.4/hpgeom.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-23 02:48:58.000000 hpgeom-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 02:48:58.000000 hpgeom-0.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-23 02:49:14.007678 hpgeom-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-23 02:48:58.000000 hpgeom-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:49:14.007678 hpgeom-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/make_benchmark_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_angle_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_angle_to_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_healpy_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_max_pixel_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_nest_to_ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_pixel_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_pixel_to_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_pixel_to_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_query_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_query_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_query_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_query_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_ring_to_nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_vector_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/test_vector_to_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 02:48:58.000000 hpgeom-0.8.4/tests/utils.py
```

### Comparing `hpgeom-0.8.2/.github/workflows/python-package-pr.yml` & `hpgeom-0.8.4/.github/workflows/python-package-pr.yml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
         os: [ubuntu-latest, macOS-latest, windows-latest]
 
     steps:
     - uses: actions/checkout@v3
       with:
         # Need to clone everything to determine version from git.
         fetch-depth: 0
@@ -36,11 +36,14 @@
         python -m pip install --upgrade pip setuptools
         if [ "$RUNNER_OS" == "Windows" ]; then
             # healpy is not available on windows.
             python -m pip install .[test]
         else
             python -m pip install .[test,test_with_healpy]
         fi
+    - name: Run flake8
+      run: |
+        flake8
     - name: Run tests
       run: |
         cd tests
         pytest
```

### Comparing `hpgeom-0.8.2/.github/workflows/python-package-publish.yml` & `hpgeom-0.8.4/.github/workflows/python-package-publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,17 @@
           cache: "pip"
           cache-dependency-path: "setup.cfg"
 
       - name: Build and install
         run: |
           python -m pip install --upgrade pip setuptools
           python -m pip install .[test,test_with_healpy]
+      - name: Run flake8
+        run: |
+          flake8
       - name: Run tests
         run: |
           cd tests
           pytest
 
   pypi_sdist_build:
     runs-on: ubuntu-latest
@@ -55,15 +58,15 @@
       - uses: actions/upload-artifact@v3
         with:
           path: dist/*
 
   pypi_wheel_build:
     strategy:
       matrix:
-        os: ["ubuntu-latest", "macOS-10.15", "windows-2019"]
+        os: ["ubuntu-latest", "macOS-11", "windows-2019"]
     runs-on: ${{ matrix.os }}
     needs: [build_and_test]
     env:
       CIBW_BUILD: "cp3{7,8,9,10}-{manylinux_x86_64,macosx_arm64,macosx_x86_64,win_amd64}"
       CIBW_ARCHS_MACOS: "x86_64 arm64"
       CIBW_ARCHS_LINUX: "auto"
```

### Comparing `hpgeom-0.8.2/.github/workflows/python-package-push.yml` & `hpgeom-0.8.4/.github/workflows/python-package-push.yml`

 * *Files 13% similar despite different names*

```diff
@@ -31,11 +31,14 @@
         cache: "pip"
         cache-dependency-path: "setup.cfg"
 
     - name: Build and install
       run: |
         python -m pip install --upgrade pip setuptools
         python -m pip install .[test,test_with_healpy]
+    - name: Run flake8
+      run: |
+        flake8
     - name: Run tests
       run: |
         cd tests
         pytest
```

### Comparing `hpgeom-0.8.2/.gitignore` & `hpgeom-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/LICENSE` & `hpgeom-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/PKG-INFO` & `hpgeom-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpgeom
-Version: 0.8.2
+Version: 0.8.4
 Summary: HEALPix pixel lookup and geometry routines with numpy
 Home-page: https://github.com/lsstdesc/hpgeom
 Author: Eli Rykoff, Dark Energy Science Collaboration
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `hpgeom-0.8.2/README.md` & `hpgeom-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/docs/Makefile` & `hpgeom-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/docs/conf.py` & `hpgeom-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/docs/index.rst` & `hpgeom-0.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/docs/install.rst` & `hpgeom-0.8.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/healpix_geom.c` & `hpgeom-0.8.4/hpgeom/healpix_geom.c`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/healpix_geom.h` & `hpgeom-0.8.4/hpgeom/healpix_geom.h`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/healpy_compat.py` & `hpgeom-0.8.4/hpgeom/healpy_compat.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/hpgeom.c` & `hpgeom-0.8.4/hpgeom/hpgeom.c`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/hpgeom.py` & `hpgeom-0.8.4/hpgeom/hpgeom.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     if (np.any(npixel <= 0)):
         raise ValueError("Illegal npixel (must be positive)")
     nside = np.sqrt(np.atleast_1d(npixel)/12.0)
     if np.any(nside != np.floor(nside)):
         raise ValueError("Illegal npixel (it must be 12*nside*nside)")
 
     if len(nside) == 1:
-        return int(nside)
+        return int(nside[0])
     else:
         return nside.astype(np.int64)
 
 
 def nside_to_pixel_area(nside, degrees=True):
     """Return the pixel area given an nside in square degrees or square radians.
```

### Comparing `hpgeom-0.8.2/hpgeom/hpgeom_stack.c` & `hpgeom-0.8.4/hpgeom/hpgeom_stack.c`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/hpgeom_stack.h` & `hpgeom-0.8.4/hpgeom/hpgeom_stack.h`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/hpgeom_utils.c` & `hpgeom-0.8.4/hpgeom/hpgeom_utils.c`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom/hpgeom_utils.h` & `hpgeom-0.8.4/hpgeom/hpgeom_utils.h`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/hpgeom.egg-info/PKG-INFO` & `hpgeom-0.8.4/hpgeom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpgeom
-Version: 0.8.2
+Version: 0.8.4
 Summary: HEALPix pixel lookup and geometry routines with numpy
 Home-page: https://github.com/lsstdesc/hpgeom
 Author: Eli Rykoff, Dark Energy Science Collaboration
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `hpgeom-0.8.2/hpgeom.egg-info/SOURCES.txt` & `hpgeom-0.8.4/hpgeom.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .clang-format
 .gitignore
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
```

### Comparing `hpgeom-0.8.2/setup.cfg` & `hpgeom-0.8.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 	numpy
 zip_safe = True
 
 [options.extras_require]
 test = 
 	pytest
 	flake8
-	pytest-flake8
 test_with_healpy = healpy
 
 [options.packages.find]
 exclude = 
 	tests
 
 [flake8]
@@ -42,15 +41,11 @@
 ignore = E133, E226, E228, N802, N803, N806, N812, N815, N816, W503
 exclude = 
 	**/__init__.py
 	docs/conf.py
 	docs/_build/html/conf.py
 	build
 
-[tool:pytest]
-addopts = --flake8
-flake8-ignore = E133 E226 E228 N802 N803 N806 N812 N815 N816 W503
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hpgeom-0.8.2/tests/make_benchmark_table.py` & `hpgeom-0.8.4/tests/make_benchmark_table.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_angle_functions.py` & `hpgeom-0.8.4/tests/test_angle_functions.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_angle_to_pixel.py` & `hpgeom-0.8.4/tests/test_angle_to_pixel.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,26 +85,26 @@
     lon = np.random.uniform(low=0.0, high=360.0, size=100)
     lat = np.random.uniform(low=-90.0, high=90.0, size=100)
 
     pix_arr = hpgeom.angle_to_pixel(nside, lon, lat, nest=True, lonlat=True, degrees=True)
 
     pix_scalar1 = hpgeom.angle_to_pixel(nside, lon[0], lat[0], nest=True, lonlat=True, degrees=True)
 
-    assert(pix_scalar1 == pix_arr[0])
+    assert pix_scalar1 == pix_arr[0]
 
     pix_scalar2 = hpgeom.angle_to_pixel(
         nside,
         float(lon[0]),
         float(lat[0]),
         nest=True,
         lonlat=True,
         degrees=True
     )
 
-    assert(pix_scalar2 == pix_arr[0])
+    assert pix_scalar2 == pix_arr[0]
 
 
 def test_angle_to_pixel_mismatched_dims():
     """Test angle_to_pixel errors when dimensions are mismatched."""
     np.random.seed(12345)
 
     lon = np.random.uniform(low=0.0, high=360.0, size=100)
```

### Comparing `hpgeom-0.8.2/tests/test_boundaries.py` & `hpgeom-0.8.4/tests/test_boundaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         nest = True
     else:
         nest = False
 
     theta_hpgeom, phi_hpgeom = hpgeom.boundaries(nside, pix, step=step, nest=nest, lonlat=False)
     theta_healpy, phi_healpy = hp.vec2ang(hp.boundaries(nside, pix, step=step, nest=nest).T)
 
-    assert(theta_hpgeom.shape == (step*4,))
-    assert(phi_hpgeom.shape == (step*4,))
+    assert theta_hpgeom.shape == (step*4,)
+    assert phi_hpgeom.shape == (step*4,)
 
     np.testing.assert_array_almost_equal(theta_hpgeom, theta_healpy)
     np.testing.assert_array_almost_equal(phi_hpgeom, phi_healpy)
 
     lon_hpgeom, lat_hpgeom = hpgeom.boundaries(nside, pix, step=step, nest=nest, lonlat=True, degrees=True)
     lon_healpy, lat_healpy = hp.vec2ang(hp.boundaries(nside, pix, step=step, nest=nest).T, lonlat=True)
 
@@ -70,16 +70,16 @@
         pixels,
         step=step,
         nest=nest
     ).transpose([0, 2, 1]))
     theta_healpy = theta_healpy.reshape((npix, step*4))
     phi_healpy = phi_healpy.reshape((npix, step*4))
 
-    assert(theta_hpgeom.shape == (npix, step*4,))
-    assert(phi_hpgeom.shape == (npix, step*4,))
+    assert theta_hpgeom.shape == (npix, step*4,)
+    assert phi_hpgeom.shape == (npix, step*4,)
 
     np.testing.assert_array_almost_equal(theta_hpgeom, theta_healpy)
     np.testing.assert_array_almost_equal(phi_hpgeom, phi_healpy)
 
     lon_hpgeom, lat_hpgeom = hpgeom.boundaries(nside, pixels, step=step, nest=nest, lonlat=True, degrees=True)
     lon_healpy, lat_healpy = hp.vec2ang(hp.boundaries(
         nside,
```

### Comparing `hpgeom-0.8.2/tests/test_healpy_compat.py` & `hpgeom-0.8.4/tests/test_healpy_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,83 +89,83 @@
 
 @pytest.mark.skipif(not has_healpy, reason="Skipping test without healpy")
 def test_ring2nest():
     """Test hpgeom.healpy_compat.ring2nest."""
     pix_hpcompat = hpc.ring2nest(2048, 1000)
     pix_healpy = hp.ring2nest(2048, 1000)
 
-    assert(pix_hpcompat == pix_healpy)
+    assert pix_hpcompat == pix_healpy
 
     pix_hpcompat = hpc.ring2nest(2048, np.arange(100))
     pix_healpy = hp.ring2nest(2048, np.arange(100))
 
     np.testing.assert_array_equal(pix_hpcompat, pix_healpy)
 
 
 @pytest.mark.skipif(not has_healpy, reason="Skipping test without healpy")
 def test_nest2ring():
     """Test hpgeom.healpy_compat.nest2ring."""
     pix_hpcompat = hpc.nest2ring(2048, 1000)
     pix_healpy = hp.nest2ring(2048, 1000)
 
-    assert(pix_hpcompat == pix_healpy)
+    assert pix_hpcompat == pix_healpy
 
     pix_hpcompat = hpc.nest2ring(2048, np.arange(100))
     pix_healpy = hp.nest2ring(2048, np.arange(100))
 
     np.testing.assert_array_equal(pix_hpcompat, pix_healpy)
 
 
 @pytest.mark.skipif(not has_healpy, reason="Skipping test without healpy")
 def test_nside2npix():
     """Test hpgeom.healpy_compat.nside2npix."""
     npix_hpcompat = hpc.nside2npix(2048)
     npix_healpy = hp.nside2npix(2048)
 
-    assert(npix_hpcompat == npix_healpy)
+    assert npix_hpcompat == npix_healpy
 
 
 @pytest.mark.skipif(not has_healpy, reason="Skipping test without healpy")
 def test_npix2nside():
     """Test hpgeom.healpy_compat.npix2nside."""
     nside_hpcompat = hpc.nside2npix(12*2048*2048)
     nside_healpy = hp.nside2npix(12*2048*2048)
 
-    assert(nside_hpcompat == nside_healpy)
+    assert nside_hpcompat == nside_healpy
 
     with pytest.raises(ValueError, match=r"Illegal npixel"):
         hpc.npix2nside(100)
 
 
 @pytest.mark.skipif(not has_healpy, reason="Skipping test without healpy")
 def test_nside2pixarea():
     """Test hpgeom.healpy_compat.nside2pixarea."""
     pixarea_hpcompat = hpc.nside2pixarea(1024)
     pixarea_healpy = hp.nside2pixarea(1024)
 
-    assert (pixarea_hpcompat == pixarea_healpy)
+    assert pixarea_hpcompat == pixarea_healpy
 
     pixarea_hpcompat = hpc.nside2pixarea(1024, degrees=True)
     pixarea_healpy = hp.nside2pixarea(1024, degrees=True)
 
-    assert (pixarea_hpcompat == pixarea_healpy)
+    assert pixarea_hpcompat == pixarea_healpy
 
 
 @pytest.mark.skipif(not has_healpy, reason="Skipping test without healpy")
 def test_nside2resol():
     """Test hpgeom.healpy_compat.nside2resol."""
     resol_hpcompat = hpc.nside2resol(1024)
     resol_healpy = hp.nside2resol(1024)
 
-    assert (resol_hpcompat == resol_healpy)
+    assert resol_hpcompat == resol_healpy
 
     resol_hpcompat = hpc.nside2resol(1024, arcmin=True)
     resol_healpy = hp.nside2resol(1024, arcmin=True)
 
-    assert (resol_hpcompat == resol_healpy)
+    assert resol_hpcompat == resol_healpy
 
 
 @pytest.mark.skipif(not has_healpy, reason="Skipping test without healpy")
 def test_nside2order():
     """Test hpgeom.healpy_compat.nside2order."""
     order_hpcompat = hpc.nside2order(1024)
     order_healpy = hp.nside2order(1024)
```

### Comparing `hpgeom-0.8.2/tests/test_max_pixel_radius.py` & `hpgeom-0.8.4/tests/test_max_pixel_radius.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_neighbors.py` & `hpgeom-0.8.4/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_nest_to_ring.py` & `hpgeom-0.8.4/tests/test_nest_to_ring.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_pixel_functions.py` & `hpgeom-0.8.4/tests/test_pixel_functions.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_pixel_to_angle.py` & `hpgeom-0.8.4/tests/test_pixel_to_angle.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,27 +80,27 @@
     np.random.seed(12345)
 
     pix = np.random.randint(low=0, high=12*nside*nside-1, size=100, dtype=np.int64)
 
     lon_arr, lat_arr = hpgeom.pixel_to_angle(nside, pix, nest=True, lonlat=True, degrees=True)
     lon_scalar1, lat_scalar1 = hpgeom.pixel_to_angle(nside, pix[0], nest=True, lonlat=True, degrees=True)
 
-    assert(lon_scalar1 == lon_arr[0])
-    assert(lat_scalar1 == lat_arr[0])
+    assert lon_scalar1 == lon_arr[0]
+    assert lat_scalar1 == lat_arr[0]
 
     lon_scalar2, lat_scalar2 = hpgeom.pixel_to_angle(
         nside,
         int(pix[0]),
         nest=True,
         lonlat=True,
         degrees=True
     )
 
-    assert(lon_scalar2 == lon_arr[0])
-    assert(lat_scalar2 == lat_arr[0])
+    assert lon_scalar2 == lon_arr[0]
+    assert lat_scalar2 == lat_arr[0]
 
 
 @pytest.mark.parametrize("nside", [2**0, 2**5, 2**10, 2**15, 2**20, 2**25, 2**29])
 def test_pixel_to_angle_bad_pix(nside):
     """Test pixel_to_angle errors when given bad pixel"""
 
     with pytest.raises(ValueError, match=r"Pixel value .* out of range"):
```

### Comparing `hpgeom-0.8.2/tests/test_pixel_to_vector.py` & `hpgeom-0.8.4/tests/test_pixel_to_vector.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_query_box.py` & `hpgeom-0.8.4/tests/test_query_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,26 @@
     np.testing.assert_array_equal(pixels, pixels_circle[inside])
 
     # Do inclusive
     pixels_box = hpgeom.query_box(nside, *box, inclusive=True)
 
     # Ensure all the inner pixels are in the inclusive pixels
     sub1, sub2 = match_arrays(pixels_box, pixels)
-    assert(sub2.size == pixels.size)
+    assert sub2.size == pixels.size
 
     # Look at boundaries of the pixels, check if any are included.
     pixels_circle = hpgeom.query_circle(nside, lon, lat, radius*2.5)
     boundaries_lon, boundaries_lat = hpgeom.boundaries(nside, pixels_circle, step=4)
     cut = _pos_in_box(boundaries_lon.ravel(), boundaries_lat.ravel(), *box)
     test = cut.reshape(boundaries_lon.shape).sum(axis=1)
     pixels_circle_box = pixels_circle[test > 0]
 
     # Ensure all these pixels are in the inclusive list
     sub1, sub2 = match_arrays(pixels_circle_box, pixels_box)
-    assert(sub1.size == pixels_circle_box.size)
+    assert sub1.size == pixels_circle_box.size
 
 
 @pytest.mark.parametrize("nside_radius", [(2**7, 2.0),
                                           (2**10, 1.0),
                                           (2**20, 0.01)])
 @pytest.mark.parametrize("lon", [0.0, 360.0])
 @pytest.mark.parametrize("lat", [-45.0, 0.0, 45.0])
@@ -101,33 +101,33 @@
     np.testing.assert_array_equal(pixels, pixels_circle[inside])
 
     # Do inclusive
     pixels_box = hpgeom.query_box(nside, *box, inclusive=True)
 
     # Ensure all the inner pixels are in the inclusive pixels
     sub1, sub2 = match_arrays(pixels_box, pixels)
-    assert(sub2.size == pixels.size)
+    assert sub2.size == pixels.size
 
     # Look at boundaries of the pixels.
     pixels_circle = hpgeom.query_circle(nside, (box[0] + box[1])/2., lat, radius*2.5)
     boundaries_lon, boundaries_lat = hpgeom.boundaries(nside, pixels_circle, step=4)
     cut = _pos_in_box(boundaries_lon.ravel(), boundaries_lat.ravel(), *box)
     test = cut.reshape(boundaries_lon.shape).sum(axis=1)
     pixels_circle_box = pixels_circle[test > 0]
 
     # Ensure all these pixels are in the inclusive list
     sub1, sub2 = match_arrays(pixels_circle_box, pixels_box)
-    assert(sub1.size == pixels_circle_box.size)
+    assert sub1.size == pixels_circle_box.size
 
     # And ensure that we did wrap over the edge
     lon_box, lat_box = hpgeom.pixel_to_angle(nside, pixels_box)
     if (lon == 0.0):
-        assert(lon_box.max() > 355.0)
+        assert lon_box.max() > 355.0
     else:
-        assert(lon_box.min() < 5.0)
+        assert lon_box.min() < 5.0
 
 
 @pytest.mark.parametrize("nside_radius", [(2**5, 2.0),
                                           (2**10, 1.0),
                                           (2**20, 0.01)])
 @pytest.mark.parametrize("lon", [0.0, 90.0, 180.0, 270.0])
 @pytest.mark.parametrize("lat", [90.0, -90.0])
@@ -150,31 +150,31 @@
     np.testing.assert_array_equal(pixels, pixels_circle[inside])
 
     # Do inclusive
     pixels_box = hpgeom.query_box(nside, *box, inclusive=True)
 
     # Ensure all the inner pixels are in the inclusive pixels
     sub1, sub2 = match_arrays(pixels_box, pixels)
-    assert(sub2.size == pixels.size)
+    assert sub2.size == pixels.size
 
     # Look at boundaries of the pixels, check if any are included.
     pixels_circle = hpgeom.query_circle(nside, lon, lat, radius*2.5)
     boundaries_lon, boundaries_lat = hpgeom.boundaries(nside, pixels_circle, step=4)
     cut = _pos_in_box(boundaries_lon.ravel(), boundaries_lat.ravel(), *box)
     test = cut.reshape(boundaries_lon.shape).sum(axis=1)
     pixels_circle_box = pixels_circle[test > 0]
 
     # Ensure all these pixels are in the inclusive list
     sub1, sub2 = match_arrays(pixels_circle_box, pixels_box)
     if (lon == 0.0 and lat == -90.0):
         # There is some oddity with the polar pixel boundaries that needs to
         # be investigated.
-        assert(sub1.size == (pixels_circle_box.size - 2))
+        assert sub1.size == (pixels_circle_box.size - 2)
     else:
-        assert(sub1.size == pixels_circle_box.size)
+        assert sub1.size == pixels_circle_box.size
 
 
 @pytest.mark.parametrize("nside", [2**5, 2**10])
 @pytest.mark.parametrize("lat", [90.0, -90.0])
 def test_query_box_pole_full_longitude(nside, lat):
     """Test query_box at the latitude poles, full longitude."""
     radius = 2.0
@@ -192,15 +192,15 @@
     np.testing.assert_array_equal(pixels, pixels_circle)
 
     # Do inclusive
     pixels_box = hpgeom.query_box(nside, *box, inclusive=True)
 
     # Ensure all the inner pixels are in the inclusive pixels
     sub1, sub2 = match_arrays(pixels_box, pixels)
-    assert(sub2.size == pixels.size)
+    assert sub2.size == pixels.size
 
     pixels_circle_inc = hpgeom.query_circle(nside, 0.0, lat, radius, inclusive=True)
 
     np.testing.assert_array_equal(pixels_box, pixels_circle_inc)
 
 
 @pytest.mark.parametrize("nside", [2**5, 2**10])
@@ -220,26 +220,26 @@
     np.testing.assert_array_equal(pixels, pixels_all[inside])
 
     # Do inclusive
     pixels_box = hpgeom.query_box(nside, *box, inclusive=True)
 
     # Ensure all the inner pixels are in the inclusive pixels
     sub1, sub2 = match_arrays(pixels_box, pixels)
-    assert(sub2.size == pixels.size)
+    assert sub2.size == pixels.size
 
     # Look at boundaries of the pixels, check if any are included.
     inside_plus = ((lat_all >= (lat - 2*radius)) & (lat_all <= (lat + 2*radius)))
     boundaries_lon, boundaries_lat = hpgeom.boundaries(nside, pixels_all[inside_plus], step=4)
     cut = ((boundaries_lat.ravel() >= box[2]) & (boundaries_lat.ravel() < box[3]))
     test = cut.reshape(boundaries_lat.shape).sum(axis=1)
     pixels_all_box = pixels_all[inside_plus][test > 0]
 
     # Ensure all these pixels are in the inclusive list
     sub1, sub2 = match_arrays(pixels_all_box, pixels_box)
-    assert(sub1.size == pixels_all_box.size)
+    assert sub1.size == pixels_all_box.size
 
 
 @pytest.mark.parametrize("fact", [1, 2, 4, 8])
 def test_query_box_fact(fact):
     """Test query_box, use other fact values."""
     nside = 1024
     radius = 1.0
@@ -250,36 +250,36 @@
 
     pixels = hpgeom.query_box(nside, *box)
 
     pixels_box = hpgeom.query_box(nside, *box, inclusive=True, fact=fact)
 
     # Ensure all the inner pixels are in the inclusive pixels
     sub1, sub2 = match_arrays(pixels_box, pixels)
-    assert(sub2.size == pixels.size)
+    assert sub2.size == pixels.size
 
     # Look at boundaries of the pixels, check if any are included.
     pixels_circle = hpgeom.query_circle(nside, lon, lat, radius*2.5)
     boundaries_lon, boundaries_lat = hpgeom.boundaries(nside, pixels_circle, step=4)
     cut = _pos_in_box(boundaries_lon.ravel(), boundaries_lat.ravel(), *box)
     test = cut.reshape(boundaries_lon.shape).sum(axis=1)
     pixels_circle_box = pixels_circle[test > 0]
 
     # Ensure all these pixels are in the inclusive list
     sub1, sub2 = match_arrays(pixels_circle_box, pixels_box)
-    assert(sub1.size == pixels_circle_box.size)
+    assert sub1.size == pixels_circle_box.size
 
 
 def test_query_box_empty():
     """Test query box when it is empty."""
 
     pixels = hpgeom.query_box(1024, 25.0, 25.0, 0.0, 2.0)
-    assert(pixels.size == 0)
+    assert pixels.size == 0
 
     pixels = hpgeom.query_box(1024, 90.0, 92.0, 45.0, 45.0)
-    assert(pixels.size == 0)
+    assert pixels.size == 0
 
 
 def test_query_box_radians():
     """Test query_box, use lonlat and radians."""
     nside = 1024
     lon = 90.0
     lat = 45.0
```

### Comparing `hpgeom-0.8.2/tests/test_query_circle.py` & `hpgeom-0.8.4/tests/test_query_circle.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_query_ellipse.py` & `hpgeom-0.8.4/tests/test_query_ellipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,26 +156,26 @@
     minor = nside_major_minor[2]
 
     pixels = hpgeom.query_ellipse(nside, lon, lat, major, minor, alpha)
     pixels_ellipse = hpgeom.query_ellipse(nside, lon, lat, major, minor, alpha, inclusive=True)
 
     # Ensure all the inner pixels are in the inclusive pixels
     sub1, sub2 = match_arrays(pixels_ellipse, pixels)
-    assert(sub2.size == pixels.size)
+    assert sub2.size == pixels.size
 
     # Look at the boundaries of the pixels, check if any are included.
     pixels_circle = hpgeom.query_circle(nside, lon, lat, major*1.1)
     boundaries_lon, boundaries_lat = hpgeom.boundaries(nside, pixels_circle, step=4)
     cut = _pos_in_ellipse(boundaries_lon.ravel(), boundaries_lat.ravel(), lon, lat, major, minor, alpha)
     test = cut.reshape(boundaries_lon.shape).sum(axis=1)
     pixels_circle_ellipse = pixels_circle[test > 0]
 
     # Ensure all these pixels are in the inclusive list
     sub1, sub2 = match_arrays(pixels_circle_ellipse, pixels_ellipse)
-    assert(sub1.size == pixels_circle_ellipse.size)
+    assert sub1.size == pixels_circle_ellipse.size
 
 
 def test_query_ellipse_radians():
     """Test query_ellipse, use lonlat and radians."""
     nside = 1024
     major = 2.0
     minor = 1.0
@@ -243,16 +243,16 @@
     # We don't get 100% overlap, unfortunately, so we have to look above a threshold
     sub1 = np.searchsorted(pixels_ellipse, pixels_circle_ellipse)
     bad, = (sub1 == pixels_ellipse.size).nonzero()
     sub1[bad] = pixels_ellipse.size - 1
     sub2, = (pixels_ellipse[sub1] == pixels_circle_ellipse).nonzero()
     sub1 = sub1[sub2]
 
-    assert(sub1.size >= int(0.9*pixels_ellipse.size))
-    assert(sub1.size >= int(0.9*pixels_circle_ellipse.size))
+    assert sub1.size >= int(0.9*pixels_ellipse.size)
+    assert sub1.size >= int(0.9*pixels_circle_ellipse.size)
 
 
 def test_query_ellipse_badinputs():
     """Test query ellipse with bad inputs."""
     with pytest.raises(ValueError, match=r"lat .* out of range"):
         # Latitude out of range
         hpgeom.query_ellipse(2048, 0.0, 100.0, 1.0, 0.5, 0.0)
```

### Comparing `hpgeom-0.8.2/tests/test_query_polygon.py` & `hpgeom-0.8.4/tests/test_query_polygon.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_ring_to_nest.py` & `hpgeom-0.8.4/tests/test_ring_to_nest.py`

 * *Files identical despite different names*

### Comparing `hpgeom-0.8.2/tests/test_vector_functions.py` & `hpgeom-0.8.4/tests/test_vector_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     vec_healpy = hp.ang2vec(lon, lat, lonlat=True)
 
     np.testing.assert_array_almost_equal(vec_hpgeom, vec_healpy)
 
     vec_hpgeom = hpgeom.angle_to_vector(float(lon[0]), float(lat[0]))
     vec_healpy = hp.ang2vec(float(lon[0]), float(lat[0]), lonlat=True)
 
-    assert(vec_hpgeom.shape == (3, ))
+    assert vec_hpgeom.shape == (3, )
     np.testing.assert_array_almost_equal(vec_hpgeom, vec_healpy)
 
     theta, phi = hpgeom.lonlat_to_thetaphi(lon, lat)
 
     vec_hpgeom = hpgeom.angle_to_vector(theta, phi, lonlat=False)
     vec_healpy = hp.ang2vec(theta, phi)
```

### Comparing `hpgeom-0.8.2/tests/test_vector_to_pixel.py` & `hpgeom-0.8.4/tests/test_vector_to_pixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     """Test vector_to_pixel, single pixel."""
     x = 0.5
     y = 0.5
     z = 0.5
 
     pix_hpgeom = hpgeom.vector_to_pixel(1024, x, y, z)
 
-    assert(isinstance(pix_hpgeom, np.int64))
+    assert isinstance(pix_hpgeom, np.int64)
```

### Comparing `hpgeom-0.8.2/tests/utils.py` & `hpgeom-0.8.4/tests/utils.py`

 * *Files identical despite different names*

