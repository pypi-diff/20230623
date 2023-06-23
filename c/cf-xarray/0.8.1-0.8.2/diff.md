# Comparing `tmp/cf_xarray-0.8.1.tar.gz` & `tmp/cf_xarray-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_xarray-0.8.1.tar", last modified: Wed May 10 03:07:03 2023, max compression
+gzip compressed data, was "cf_xarray-0.8.2.tar", last modified: Fri Jun 23 21:37:38 2023, max compression
```

## Comparing `cf_xarray-0.8.1.tar` & `cf_xarray-0.8.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.259348 cf_xarray-0.8.1/.binder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.259348 cf_xarray-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.259348 cf_xarray-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.tributors
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.267348 cf_xarray-0.8.1/cf_xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:07:02.000000 cf_xarray-0.8.1/cf_xarray/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    96676 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.267348 cf_xarray-0.8.1/cf_xarray/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/scripts/make_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/scripts/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/sgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.271348 cf_xarray-0.8.1/cf_xarray/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61220 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.267348 cf_xarray-0.8.1/cf_xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.271348 cf_xarray-0.8.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/environment-no-optional-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/upstream-dev-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.275348 cf_xarray-0.8.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/2D_bounds_averaged.png
--rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/2D_bounds_error.png
--rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/2D_bounds_nonunique.png
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/dataset-diagram-logo.tex
--rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/full-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/rich-repr-example.png
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/bounds.md
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/cartopy_rotated_pole.png
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/coding.md
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/coord_axes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/custom-criteria.md
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/dsg.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/flags.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/geometry.md
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/grid_mappings.md
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/howtouse.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/parametricz.md
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/plotting.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/provenance.md
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/selecting.md
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/sgrid_ugrid.md
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/units.md
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/whats-new.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.191434 cf_xarray-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.179434 cf_xarray-0.8.2/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.179434 cf_xarray-0.8.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.179434 cf_xarray-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/.tributors
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-06-23 21:37:38.191434 cf_xarray-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 21:37:37.000000 cf_xarray-0.8.2/cf_xarray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100886 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23849 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/scripts/make_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/scripts/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/sgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63574 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/cf_xarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/cf_xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 21:37:38.000000 cf_xarray-0.8.2/cf_xarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.183434 cf_xarray-0.8.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/environment-no-optional-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/ci/upstream-dev-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.187435 cf_xarray-0.8.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/2D_bounds_averaged.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/2D_bounds_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/2D_bounds_nonunique.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.187435 cf_xarray-0.8.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/dataset-diagram-logo.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/full-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/rich-repr-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/bounds.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/cartopy_rotated_pole.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/coding.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/coord_axes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/custom-criteria.md
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/dsg.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:37:38.187435 cf_xarray-0.8.2/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/flags.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/geometry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/grid_mappings.md
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/howtouse.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/parametricz.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/provenance.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/selecting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/sgrid_ugrid.md
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/units.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/doc/whats-new.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-23 21:37:11.000000 cf_xarray-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:37:38.191434 cf_xarray-0.8.2/setup.cfg
```

### Comparing `cf_xarray-0.8.1/.github/workflows/ci.yaml` & `cf_xarray-0.8.2/.github/workflows/ci.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
       - name: Install cf_xarray
         run: |
           python -m pip install --no-deps -e .
       - name: Run Tests
         run: |
           pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.3
+        uses: codecov/codecov-action@v3.1.4
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS,PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -87,15 +87,15 @@
       - name: Install cf_xarray
         run: |
           python -m pip install --no-deps -e .
       - name: Run Tests
         run: |
           pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.3
+        uses: codecov/codecov-action@v3.1.4
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS,PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -151,14 +151,14 @@
       - name: Install mypy
         run: |
           python -m pip install 'mypy'
       - name: Run mypy
         run: |
           python -m mypy --install-types --non-interactive --cobertura-xml-report mypy_report cf_xarray/
       - name: Upload mypy coverage to Codecov
-        uses: codecov/codecov-action@v3.1.3
+        uses: codecov/codecov-action@v3.1.4
         with:
           file: mypy_report/cobertura.xml
           flags: mypy
           env_vars: PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `cf_xarray-0.8.1/.github/workflows/parse_logs.py` & `cf_xarray-0.8.2/.github/workflows/parse_logs.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/.github/workflows/pypi.yaml` & `cf_xarray-0.8.2/.github/workflows/pypi.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install dist/cf_xarray*.whl
           python -m cf_xarray.scripts.print_versions
 
       - name: Publish package to TestPyPI
         if: github.event_name == 'push'
-        uses: pypa/gh-action-pypi-publish@v1.8.5
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           password: ${{ secrets.TESTPYPI_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
           verbose: true
 
 
   upload-to-pypi:
@@ -92,10 +92,10 @@
 
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.5
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           verbose: true
```

### Comparing `cf_xarray-0.8.1/.github/workflows/testpypi-release.yaml` & `cf_xarray-0.8.2/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/.github/workflows/upstream-dev-ci.yaml` & `cf_xarray-0.8.2/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/.gitignore` & `cf_xarray-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/.pre-commit-config.yaml` & `cf_xarray-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/.tributors` & `cf_xarray-0.8.2/.tributors`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/CITATION.cff` & `cf_xarray-0.8.2/CITATION.cff`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     given-names: Martin
     orcid: 'https://orcid.org/0000-0001-8075-589X'
     affiliation: DKRZ (German Climate Computing Centre)
   - family-names: Vo
     given-names: Tom
     orcid: 'https://orcid.org/0000-0002-2461-0191'
     affiliation: Lawrence Livermore National Laboratory
+  - family-names: Haëck
+    given-names: Clément
+    affiliation: Laboratoire d'Océanographie et du Climat (LOCEAN), Paris
 identifiers:
   - type: doi
     value: 10.5281/zenodo.4749735
     description: Zenodo DOI
 repository-code: 'https://github.com/xarray-contrib/cf-xarray'
 url: 'https://cf-xarray.readthedocs.io'
 abstract: >-
@@ -92,10 +95,10 @@
   Forecast metadata convention attributes present on xarray
   objects.
 keywords:
   - cf-conventions
   - xarray
   - metadata
 license: Apache-2.0
-commit: 1b373a21b558423da8f22c3ec79f58737871719b
-version: 0.8.0
-date-released: '2023-02-08'
+# commit: 1b373a21b558423da8f22c3ec79f58737871719b
+version: 0.8.2
+date-released: '2023-06-23'
```

### Comparing `cf_xarray-0.8.1/LICENSE` & `cf_xarray-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/PKG-INFO` & `cf_xarray-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_xarray
-Version: 0.8.1
+Version: 0.8.2
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.1/README.rst` & `cf_xarray-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/accessor.py` & `cf_xarray-0.8.2/cf_xarray/accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import functools
 import inspect
 import itertools
 import re
 import warnings
-from collections import ChainMap
+from collections import ChainMap, namedtuple
 from datetime import datetime
 from typing import (
     Any,
     Callable,
     Hashable,
     Iterable,
     List,
@@ -54,14 +54,16 @@
     _is_datetime_like,
     always_iterable,
     invert_mappings,
     parse_cell_methods_attr,
     parse_cf_standard_name_table,
 )
 
+FlagParam = namedtuple("FlagParam", ["flag_mask", "flag_value"])
+
 #: Classes wrapped by cf_xarray.
 _WRAPPED_CLASSES = (Resample, GroupBy, Rolling, Coarsen, Weighted)
 
 #:  `axis` names understood by cf_xarray
 _AXIS_NAMES = ("X", "Y", "Z", "T")
 
 #:  `coordinate` types understood by cf_xarray.
@@ -1053,26 +1055,47 @@
             key_mappers=dict.fromkeys(self._keys, (_single(_get_all),)),
             # TODO: "extra_decorator" is more complex than I would like it to be.
             # Not sure if there is a better way though
             extra_decorator=self._plot_decorator,
         )
 
 
-def create_flag_dict(da):
+def create_flag_dict(da) -> Mapping[Hashable, FlagParam]:
+    """
+    Return possible flag meanings and associated bitmask/values.
+
+    The mapping values are a tuple containing a bitmask and a value. Either
+    can be None.
+    If only a bitmask: Independent flags.
+    If only a value: Mutually exclusive flags.
+    If both: Mix of independent and mutually exclusive flags.
+    """
     if not da.cf.is_flag_variable:
         raise ValueError(
-            "Comparisons are only supported for DataArrays that represent CF flag variables."
-            ".attrs must contain 'flag_values' and 'flag_meanings'"
+            "Comparisons are only supported for DataArrays that represent "
+            "CF flag variables. .attrs must contain 'flag_meanings' and "
+            "'flag_values' or 'flag_masks'."
         )
 
     flag_meanings = da.attrs["flag_meanings"].split(" ")
-    flag_values = da.attrs["flag_values"]
-    # TODO: assert flag_values is iterable
-    assert len(flag_values) == len(flag_meanings)
-    return dict(zip(flag_meanings, flag_values))
+    n_flag = len(flag_meanings)
+
+    flag_values = da.attrs.get("flag_values", [None] * n_flag)
+    flag_masks = da.attrs.get("flag_masks", [None] * n_flag)
+
+    if not (n_flag == len(flag_values) == len(flag_masks)):
+        raise ValueError(
+            "Not as many flag meanings as values or masks. "
+            "Please check the flag_meanings, flag_values, flag_masks attributes "
+        )
+
+    flag_params = tuple(
+        FlagParam(mask, value) for mask, value in zip(flag_masks, flag_values)
+    )
+    return dict(zip(flag_meanings, flag_params))
 
 
 class CFAccessor:
     """
     Common Dataset and DataArray accessor functionality.
     """
 
@@ -1080,88 +1103,92 @@
         self._obj = obj
         self._all_cell_measures = None
 
     def __setstate__(self, d):
         self.__dict__ = d
 
     def _assert_valid_other_comparison(self, other):
+        # TODO cache this property
         flag_dict = create_flag_dict(self._obj)
         if other not in flag_dict:
             raise ValueError(
                 f"Did not find flag value meaning [{other}] in known flag meanings: [{flag_dict.keys()!r}]"
             )
+        if flag_dict[other].flag_mask is not None:
+            raise NotImplementedError(
+                "Only equals and not-equals comparisons with flag masks are supported."
+                " Please open an issue."
+            )
         return flag_dict
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> DataArray:  # type: ignore
         """
         Compare flag values against `other`.
 
         `other` must be in the 'flag_meanings' attribute.
         `other` is mapped to the corresponding value in the 'flag_values' attribute, and then
         compared.
         """
-        flag_dict = self._assert_valid_other_comparison(other)
-        return self._obj == flag_dict[other]
+        return self._extract_flags([other])[other].rename(self._obj.name)
 
-    def __ne__(self, other):
+    def __ne__(self, other) -> DataArray:  # type: ignore
         """
         Compare flag values against `other`.
 
         `other` must be in the 'flag_meanings' attribute.
         `other` is mapped to the corresponding value in the 'flag_values' attribute, and then
         compared.
         """
-        flag_dict = self._assert_valid_other_comparison(other)
-        return self._obj != flag_dict[other]
+        return ~self._extract_flags([other])[other].rename(self._obj.name)
 
-    def __lt__(self, other):
+    def __lt__(self, other) -> DataArray:
         """
         Compare flag values against `other`.
 
         `other` must be in the 'flag_meanings' attribute.
         `other` is mapped to the corresponding value in the 'flag_values' attribute, and then
         compared.
         """
         flag_dict = self._assert_valid_other_comparison(other)
-        return self._obj < flag_dict[other]
+        return self._obj < flag_dict[other].flag_value
 
-    def __le__(self, other):
+    def __le__(self, other) -> DataArray:
         """
         Compare flag values against `other`.
 
         `other` must be in the 'flag_meanings' attribute.
         `other` is mapped to the corresponding value in the 'flag_values' attribute, and then
         compared.
         """
         flag_dict = self._assert_valid_other_comparison(other)
-        return self._obj <= flag_dict[other]
+        return self._obj <= flag_dict[other].flag_value
 
-    def __gt__(self, other):
+    def __gt__(self, other) -> DataArray:
         """
         Compare flag values against `other`.
 
         `other` must be in the 'flag_meanings' attribute.
         `other` is mapped to the corresponding value in the 'flag_values' attribute, and then
         compared.
         """
         flag_dict = self._assert_valid_other_comparison(other)
-        return self._obj > flag_dict[other]
+        return self._obj > flag_dict[other].flag_value
 
-    def __ge__(self, other):
+    def __ge__(self, other) -> DataArray:
         """
         Compare flag values against `other`.
 
         `other` must be in the 'flag_meanings' attribute.
         `other` is mapped to the corresponding value in the 'flag_values' attribute, and then
         compared.
         """
         flag_dict = self._assert_valid_other_comparison(other)
-        return self._obj >= flag_dict[other]
+        return self._obj >= flag_dict[other].flag_value
 
-    def isin(self, test_elements):
+    def isin(self, test_elements) -> DataArray:
         """Test each value in the array for whether it is in test_elements.
 
         Parameters
         ----------
         test_elements : array_like, 1D
             The values against which to test each value of `element`.
             These must be in "flag_meanings" attribute, and are mapped
@@ -1173,22 +1200,23 @@
         isin : DataArray
             Has the same type and shape as this object, but with a bool dtype.
         """
         if not isinstance(self._obj, DataArray):
             raise ValueError(
                 ".cf.isin is only supported on DataArrays that contain CF flag attributes."
             )
+        # TODO cache this property
         flag_dict = create_flag_dict(self._obj)
         mapped_test_elements = []
         for elem in test_elements:
             if elem not in flag_dict:
                 raise ValueError(
                     f"Did not find flag value meaning [{elem}] in known flag meanings: [{flag_dict.keys()!r}]"
                 )
-            mapped_test_elements.append(flag_dict[elem])
+            mapped_test_elements.append(flag_dict[elem].flag_value)
         return self._obj.isin(mapped_test_elements)
 
     def _drop_missing_variables(self, variables: list[Hashable]) -> list[Hashable]:
         if isinstance(self._obj, Dataset):
             good_names = set(self._obj._variables)
         elif isinstance(self._obj, DataArray):
             good_names = set(self._obj._coords)
@@ -2750,26 +2778,108 @@
             raise KeyError(
                 f"Cannot use an Iterable of keys with DataArrays. Expected a single string. Received {key!r} instead."
             )
 
         return _getitem(self, key)
 
     @property
+    def flags(self) -> Dataset:
+        """
+        Dataset containing boolean masks of available flags.
+        """
+        return self._extract_flags()
+
+    def _extract_flags(self, flags: Sequence[Hashable] | None = None) -> Dataset:
+        """
+        Return dataset of boolean mask(s) corresponding to `flags`.
+
+        Parameters
+        ----------
+        flags: Sequence[str]
+            Flags to extract. If empty (string or list), return all flags in
+            `flag_meanings`.
+        """
+        # TODO cache this property
+        flag_dict = create_flag_dict(self._obj)
+
+        if flags is None:
+            flags = tuple(flag_dict.keys())
+
+        out = {}  # Output arrays
+
+        masks = []  # Bitmasks and values for asked flags
+        values = []
+        flags_reduced = []  # Flags left after removing mutually excl. flags
+        for flag in flags:
+            if flag not in flag_dict:
+                raise ValueError(
+                    f"Did not find flag value meaning [{flag}] in known flag meanings:"
+                    f" [{flag_dict.keys()!r}]"
+                )
+            mask, value = flag_dict[flag]
+            if mask is None:
+                out[flag] = self._obj == value
+            else:
+                masks.append(mask)
+                values.append(value)
+                flags_reduced.append(flag)
+
+        if len(masks) > 0:  # If independant masks are left
+            # We cast both masks and flag variable as integers to make the
+            # bitwise comparison. We could probably restrict the integer size
+            # but it's difficult to make it safely for mixed type flags.
+            bit_mask = DataArray(masks, dims=["_mask"]).astype("i")
+            x = self._obj.astype("i")
+            bit_comp = x & bit_mask
+
+            for i, (flag, value) in enumerate(zip(flags_reduced, values)):
+                bit = bit_comp.isel(_mask=i)
+                if value is not None:
+                    out[flag] = bit == value
+                else:
+                    out[flag] = bit.astype(bool)
+
+        return Dataset(out)
+
+    def isin(self, test_elements):
+        """
+        Test each value in the array for whether it is in test_elements.
+
+        Parameters
+        ----------
+        test_elements : array_like, 1D
+            The values against which to test each value of `element`.
+
+        Returns
+        -------
+        isin : DataArray
+            Has the same type and shape as this object, but with a bool dtype.
+        """
+        flags_masks = self.flags.drop_vars(
+            [v for v in self.flags.data_vars if v not in test_elements]
+        )
+        if len(flags_masks) == 0:
+            out = self.copy().astype(bool)
+            out.attrs = {}
+            out[:] = False
+            return out
+        # Merge into a single DataArray
+        flags_masks = xr.concat(flags_masks.data_vars.values(), dim="_flags")
+        return flags_masks.any(dim="_flags").rename(self._obj.name)
+
+    @property
     def is_flag_variable(self) -> bool:
         """
         Returns True if the DataArray satisfies CF conventions for flag variables.
 
-        .. warning::
-          Flag masks are not supported yet.
-
         Returns
         -------
         bool
         """
         if (
             isinstance(self._obj, DataArray)
             and "flag_meanings" in self._obj.attrs
-            and "flag_values" in self._obj.attrs
+            and ("flag_values" in self._obj.attrs or "flag_masks" in self._obj.attrs)
         ):
             return True
         else:
             return False
```

### Comparing `cf_xarray-0.8.1/cf_xarray/coding.py` & `cf_xarray-0.8.2/cf_xarray/coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/criteria.py` & `cf_xarray-0.8.2/cf_xarray/criteria.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/datasets.py` & `cf_xarray-0.8.2/cf_xarray/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -462,27 +462,65 @@
                     ),
                 }
             },
         }
     )
 )
 
-
+# Same as flags_excl but easier to read
 basin = xr.DataArray(
     [1, 2, 1, 1, 2, 2, 3, 3, 3, 3],
     dims=("time",),
     attrs={
         "flag_values": [1, 2, 3],
         "flag_meanings": "atlantic_ocean pacific_ocean indian_ocean",
         "standard_name": "region",
     },
     name="basin",
 )
 
 
+flag_excl = xr.DataArray(
+    np.array([1, 1, 2, 1, 2, 3, 3, 2], np.uint8),
+    dims=("time",),
+    coords={"time": [0, 1, 2, 3, 4, 5, 6, 7]},
+    attrs={
+        "flag_values": [1, 2, 3],
+        "flag_meanings": "flag_1 flag_2 flag_3",
+        "standard_name": "flag_mutual_exclusive",
+    },
+    name="flag_var",
+)
+
+
+flag_indep = xr.DataArray(
+    np.array([0, 1, 2, 3, 4, 5, 6, 7], dtype=np.uint8),
+    dims=("time",),
+    attrs={
+        "flag_masks": [1, 2, 4],
+        "flag_meanings": "flag_1 flag_2 flag_4",
+        "standard_name": "flag_independent",
+    },
+    name="flag_var",
+)
+
+
+flag_mix = xr.DataArray(
+    np.array([4, 8, 13, 5, 10, 14, 7, 3], np.uint8),
+    dims=("time",),
+    attrs={
+        "flag_values": [1, 2, 4, 8, 12],
+        "flag_masks": [1, 2, 12, 12, 12],
+        "flag_meanings": "flag_1 flag_2 flag_3 flag_4 flag_5",
+        "standard_name": "flag_mix",
+    },
+    name="flag_var",
+)
+
+
 ambig = xr.Dataset(
     data_vars={},
     coords={
         "lat": ("lat", np.zeros(5)),
         "lon": ("lon", np.zeros(5)),
         "vertices_latitude": (["lat", "bnds"], np.zeros((5, 2))),
         "vertices_longitude": (["lon", "bnds"], np.zeros((5, 2))),
```

### Comparing `cf_xarray-0.8.1/cf_xarray/formatting.py` & `cf_xarray-0.8.2/cf_xarray/formatting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import warnings
 from functools import partial
 from typing import Dict, Hashable, Iterable, List
 
 STAR = " * "
 TAB = len(STAR) * " "
 
+try:
+    from rich.table import Table
+except ImportError:
+    Table = None  # type: ignore
+
 
 def _format_missing_row(row: str, rich: bool) -> str:
     if rich:
         return f"[grey62]{row}[/grey62]"
     else:
         return row
 
@@ -118,39 +123,90 @@
     )
     if rich:
         row = row.rstrip()
     return row
 
 
 def _maybe_panel(textgen, title: str, rich: bool):
-    text = "".join(textgen)
     if rich:
         from rich.panel import Panel
 
-        return Panel(
-            f"[color(241)]{text.rstrip()}[/color(241)]",
+        kwargs = dict(
             expand=True,
             title_align="left",
             title=f"[bold][color(244)]{title}[/bold][/color(244)]",
             highlight=True,
             width=100,
         )
+        if isinstance(textgen, Table):
+            return Panel(textgen, padding=(0, 20), **kwargs)  # type: ignore
+        else:
+            text = "".join(textgen)
+            return Panel(f"[color(241)]{text.rstrip()}[/color(241)]", **kwargs)  # type: ignore
     else:
+        text = "".join(textgen)
         return title + ":\n" + text
 
 
 def _format_flags(accessor, rich):
     from .accessor import create_flag_dict
 
-    flag_dict = create_flag_dict(accessor._obj)
-    rows = [
-        f"{TAB}{_format_varname(v, rich)}: {_format_cf_name(k, rich)}"
-        for k, v in flag_dict.items()
-    ]
-    return _print_rows("Flag Meanings", rows, rich)
+    try:
+        flag_dict = create_flag_dict(accessor._obj)
+    except ValueError:
+        return _print_rows(
+            "Flag Meanings", ["Invalid Mapping. Check attributes."], rich
+        )
+
+    masks = [m for m, _ in flag_dict.values()]
+    repeated_masks = {m for m in masks if masks.count(m) > 1}
+    excl_flags = [f for f, (m, v) in flag_dict.items() if m in repeated_masks]
+    # indep_flags = [
+    #     f
+    #     for f, (m, _) in flag_dict.items()
+    #     if m is not None and m not in repeated_masks
+    # ]
+    if rich:
+        from rich import box
+        from rich.table import Table
+
+        table = Table(
+            box=box.SIMPLE,
+            width=None,
+            title_justify="left",
+            padding=(0, 2),
+            header_style="bold color(244)",
+        )
+
+        table.add_column("Meaning", justify="left")
+        table.add_column("Value", justify="right")
+        table.add_column("Bit?", justify="center")
+
+        for key, (mask, value) in flag_dict.items():
+            table.add_row(
+                _format_cf_name(key, rich),
+                str(value) if key in excl_flags else str(mask),
+                "✗" if key in excl_flags else "✓",
+            )
+
+        return table
+
+    else:
+        rows = [
+            f"{TAB}{_format_cf_name(key, rich)}: " f"{_format_varname(value, rich)}"
+            for key, (mask, value) in flag_dict.items()
+            if key in excl_flags
+        ]
+
+        rows += [
+            f"{TAB}{_format_cf_name(key, rich)}: " f"Bit {_format_varname(mask, rich)}"
+            for key, (mask, value) in flag_dict.items()
+            if key not in excl_flags
+        ]
+        return _print_rows("Flag Meanings", rows, rich)
 
 
 def _format_dsg_roles(accessor, dims, rich):
     from .criteria import _DSG_ROLES
 
     yield make_text_section(
         accessor,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cf_xarray-0.8.1/cf_xarray/geometry.py` & `cf_xarray-0.8.2/cf_xarray/geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/helpers.py` & `cf_xarray-0.8.2/cf_xarray/helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/options.py` & `cf_xarray-0.8.2/cf_xarray/options.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/scripts/make_doc.py` & `cf_xarray-0.8.2/cf_xarray/scripts/make_doc.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/sgrid.py` & `cf_xarray-0.8.2/cf_xarray/sgrid.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/tests/__init__.py` & `cf_xarray-0.8.2/cf_xarray/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/tests/test_accessor.py` & `cf_xarray-0.8.2/cf_xarray/tests/test_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     airds,
     ambig,
     anc,
     basin,
     ds_no_attrs,
     ds_with_tuple,
     dsg,
+    flag_excl,
+    flag_indep,
+    flag_mix,
     forecast,
     mollwds,
     multiple,
     pomds,
     popds,
     romsds,
     rotds,
@@ -155,14 +158,17 @@
 
                   Bounds:   n/a
 
            Grid Mappings:   n/a"""
     assert actual == dedent(expected)
 
     # Flag DataArray
+    assert "Flag Variable" in repr(flag_excl.cf)
+    assert "Flag Variable" in repr(flag_indep.cf)
+    assert "Flag Variable" in repr(flag_mix.cf)
     assert "Flag Variable" in repr(basin.cf)
 
     # "Temp" dataset
     actual = airds["air"]._to_temp_dataset().cf.__repr__()
     expected = """\
     Coordinates:
                  CF Axes: * X: ['lon']
@@ -1778,45 +1784,95 @@
 
         cf_da.attrs.pop("history")
         assert_identical(cf_da, cf_ds["air"])
 
     _check_unchanged(original, ds)
 
 
-@pytest.mark.parametrize("op", ["ge", "gt", "eq", "ne", "le", "lt"])
-def test_flag_features(op):
-    actual = getattr(basin.cf, f"__{op}__")("atlantic_ocean")
-    expected = getattr(basin, f"__{op}__")(1)
-    assert_identical(actual, expected)
-
-
-def test_flag_isin() -> None:
-    actual = basin.cf.isin(["atlantic_ocean", "pacific_ocean"])
-    expected = basin.isin([1, 2])
-    assert_identical(actual, expected)
-
-
-def test_flag_errors() -> None:
-    with pytest.raises(ValueError):
-        basin.cf.isin(["arctic_ocean"])
-
-    with pytest.raises(ValueError):
-        basin.cf == "arctic_ocean"
-
-    ds = xr.Dataset({"basin": basin})
-    with pytest.raises(ValueError):
-        ds.cf.isin(["atlantic_ocean"])
-
-    basin_ = basin.copy(deep=True)
-    basin_.attrs.pop("flag_values")
-    with pytest.raises(ValueError):
-        basin_.cf.isin(["pacific_ocean"])
+class TestFlags:
+    @pytest.mark.parametrize("op", ["ge", "gt", "eq", "ne", "le", "lt"])
+    def test_flag_rich_comp(self, op) -> None:
+        actual = getattr(basin.cf, f"__{op}__")("atlantic_ocean")
+        expected = getattr(basin, f"__{op}__")(1)
+        assert_identical(actual, expected)
+
+    def test_flag_excl(self) -> None:
+        for i in range(3):
+            name = f"flag_{i + 1}"
+            expected = (flag_excl == i + 1).rename(name)
+            actual = flag_excl.cf.flags[name]
+            assert_identical(actual, expected)
+
+    def test_flag_indep(self) -> None:
+        expected = [
+            [False, True, False, True, False, True, False, True],  # bit 1
+            [False, False, True, True, False, False, True, True],  # bit 2
+            [False, False, False, False, True, True, True, True],  # bit 3
+        ]
+        for i in range(3):
+            name = f"flag_{2**i}"
+            res = flag_indep.cf.flags[name]
+            np.testing.assert_equal(res.to_numpy(), expected[i])
+
+    def test_flag_mix(self) -> None:
+        expected = [
+            [False, False, True, True, False, False, True, True],  # flag 1
+            [False, False, False, False, True, True, True, True],  # flag 2
+            [True, False, False, True, False, False, True, False],  # flag 3
+            [False, True, False, False, True, False, False, False],  # flag 4
+            [False, False, True, False, False, True, False, False],  # flag 5
+        ]
+        for i in range(5):
+            name = f"flag_{i + 1}"
+            res = flag_mix.cf.flags[name]
+            np.testing.assert_equal(res.to_numpy(), expected[i])
+
+    @pytest.mark.parametrize(
+        "da, key", ((flag_indep, "flag_1"), (flag_mix, "flag_4"), (flag_excl, "flag_3"))
+    )
+    def test_flag_eq_ne(self, da, key) -> None:
+        assert_identical(da.cf.flags[key], (da.cf == key).rename(key))
+        assert_identical(~da.cf.flags[key], (da.cf != key).rename(key))
+
+    def test_flag_isin(self) -> None:
+        actual = flag_excl.cf.isin(["flag_1", "flag_3"])
+        expected = flag_excl.isin([1, 3])
+
+        actual = basin.cf.isin(["atlantic_ocean", "pacific_ocean"])
+        expected = basin.isin([1, 2])
+        assert_identical(actual, expected)
+
+        actual = flag_excl.cf.isin(["flag_ERR"])
+        assert not actual.any()
+
+    def test_flag_errors(self) -> None:
+        with pytest.raises(ValueError):
+            flag_mix.cf == "ERR"
+
+        flag_excl.attrs.pop("flag_values")
+        with pytest.raises(ValueError):
+            flag_excl.cf.isin(["flag_1"])
+
+        with pytest.raises(ValueError):
+            flag_excl.cf == "flag_1"
+
+        with pytest.raises(ValueError):
+            basin.cf == "arctic_ocean"
+
+        ds = xr.Dataset({"basin": basin})
+        with pytest.raises(ValueError):
+            ds.cf.isin(["atlantic_ocean"])
+
+        basin_ = basin.copy(deep=True)
+        basin_.attrs.pop("flag_values")
+        with pytest.raises(ValueError):
+            basin_.cf.isin(["pacific_ocean"])
 
-    with pytest.raises(ValueError):
-        basin_.cf == "pacific_ocean"
+        with pytest.raises(ValueError):
+            basin_.cf == "pacific_ocean"
 
 
 def test_missing_variables() -> None:
     # Bounds
     ds = mollwds.copy(deep=False)
     ds = ds.drop_vars("lon_bounds")
     assert ds.cf.bounds == {"lat": ["lat_bounds"], "latitude": ["lat_bounds"]}
```

### Comparing `cf_xarray-0.8.1/cf_xarray/tests/test_coding.py` & `cf_xarray-0.8.2/cf_xarray/tests/test_coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/tests/test_geometry.py` & `cf_xarray-0.8.2/cf_xarray/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/tests/test_helpers.py` & `cf_xarray-0.8.2/cf_xarray/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/tests/test_scripts.py` & `cf_xarray-0.8.2/cf_xarray/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/tests/test_units.py` & `cf_xarray-0.8.2/cf_xarray/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/units.py` & `cf_xarray-0.8.2/cf_xarray/units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray/utils.py` & `cf_xarray-0.8.2/cf_xarray/utils.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/cf_xarray.egg-info/PKG-INFO` & `cf_xarray-0.8.2/cf_xarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-xarray
-Version: 0.8.1
+Version: 0.8.2
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.1/cf_xarray.egg-info/SOURCES.txt` & `cf_xarray-0.8.2/cf_xarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/2D_bounds_averaged.png` & `cf_xarray-0.8.2/doc/2D_bounds_averaged.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/2D_bounds_error.png` & `cf_xarray-0.8.2/doc/2D_bounds_error.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/2D_bounds_nonunique.png` & `cf_xarray-0.8.2/doc/2D_bounds_nonunique.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/Makefile` & `cf_xarray-0.8.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/_static/dataset-diagram-logo.tex` & `cf_xarray-0.8.2/doc/_static/dataset-diagram-logo.tex`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/_static/full-logo.png` & `cf_xarray-0.8.2/doc/_static/full-logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/_static/logo.png` & `cf_xarray-0.8.2/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/_static/logo.svg` & `cf_xarray-0.8.2/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/_static/rich-repr-example.png` & `cf_xarray-0.8.2/doc/_static/rich-repr-example.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/api.rst` & `cf_xarray-0.8.2/doc/api.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/bounds.md` & `cf_xarray-0.8.2/doc/bounds.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/cartopy_rotated_pole.png` & `cf_xarray-0.8.2/doc/cartopy_rotated_pole.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/coding.md` & `cf_xarray-0.8.2/doc/coding.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/conf.py` & `cf_xarray-0.8.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/contributing.rst` & `cf_xarray-0.8.2/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/coord_axes.md` & `cf_xarray-0.8.2/doc/coord_axes.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/custom-criteria.md` & `cf_xarray-0.8.2/doc/custom-criteria.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/dsg.md` & `cf_xarray-0.8.2/doc/dsg.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/examples/introduction.ipynb` & `cf_xarray-0.8.2/doc/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/grid_mappings.md` & `cf_xarray-0.8.2/doc/grid_mappings.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/howtouse.md` & `cf_xarray-0.8.2/doc/howtouse.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/index.rst` & `cf_xarray-0.8.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/make.bat` & `cf_xarray-0.8.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/parametricz.md` & `cf_xarray-0.8.2/doc/parametricz.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/plotting.md` & `cf_xarray-0.8.2/doc/plotting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/provenance.md` & `cf_xarray-0.8.2/doc/provenance.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/quickstart.md` & `cf_xarray-0.8.2/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/roadmap.rst` & `cf_xarray-0.8.2/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/selecting.md` & `cf_xarray-0.8.2/doc/selecting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/sgrid_ugrid.md` & `cf_xarray-0.8.2/doc/sgrid_ugrid.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.1/doc/units.md` & `cf_xarray-0.8.2/doc/units.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 The xarray ecosystem supports unit-aware arrays using  [pint](https://pint.readthedocs.io) and [pint-xarray](https://pint-xarray.readthedocs.io). Some changes are required to make these packages work well with [UDUNITS format recommended by the CF conventions](http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#units).
 
 `cf_xarray` makes those recommended changes when you `import cf_xarray.units`. These changes allow pint to parse and format UDUNIT units strings, and add several custom units like `degrees_north`, `psu` etc.
 
 ## Formatting units
 
-For now, only the short format using [symbols](https://www.unidata.ucar.edu/software/udunits/udunits-2.2.28/udunits2lib.html#Syntax) is supported:
+For now, only the short format using [symbols](https://docs.unidata.ucar.edu/udunits/current/udunits2lib.html#Syntax) is supported:
 
 ```{code-cell}
 from pint import application_registry as ureg
 import cf_xarray.units
 
 u = ureg.Unit("m ** 3 / s ** 2")
 f"{u:~cf}"
```

### Comparing `cf_xarray-0.8.1/doc/whats-new.rst` & `cf_xarray-0.8.2/doc/whats-new.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. currentmodule:: xarray
 
 What's New
 ----------
 
+v0.8.2 (June 23, 2023)
+======================
+- Support for flag masks. By `Clément Haëck`_ and `Deepak Cherian`_.
+
 v0.8.1 (May 9, 2023)
 ====================
 - Stop bundling the standard name table and use ``pooch`` (new optional dependency) to download when needed.
   By `Deepak Cherian`_.
 - Major performance improvements.  By `Deepak Cherian`_.
 - Fix bug where code was looking for ``T`` axis in SGRID info.
   By `Kristen Thyng`_.
@@ -231,8 +235,9 @@
 .. _`Tom Vo`: https://github.com/tomvothecoder
 .. _`Romain Caneill`: https://github.com/rcaneill
 .. _`Lars Buntemeyer`: https://github.com/larsbuntemeyer
 .. _`Luke Davis`: https://github.com/lukelbd
 .. _`Martin Schupfner`: https://github.com/sol1105
 .. _`Mathias Hauser`: https://github.com/mathause
 .. _`Aidan Heerdegen`: https://github.com/aidanheerdegen
+.. _`Clément Haëck`: https://github.com/Descanonge
 .. _`flag variables`: http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#flags
```

### Comparing `cf_xarray-0.8.1/pyproject.toml` & `cf_xarray-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -126,13 +126,14 @@
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module=[
     "cftime",
     "pandas",
     "pooch",
+    "pint",
     "matplotlib",
     "pytest",
     "shapely.geometry",
     "xarray.core.pycompat",
 ]
 ignore_missing_imports = true
```

