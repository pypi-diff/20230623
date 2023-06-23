# Comparing `tmp/tabmat-3.1.8.tar.gz` & `tmp/tabmat-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabmat-3.1.8.tar", last modified: Tue Jun 13 17:05:37 2023, max compression
+gzip compressed data, was "tabmat-3.1.9.tar", last modified: Fri Jun 16 12:00:19 2023, max compression
```

## Comparing `tabmat-3.1.8.tar` & `tabmat-3.1.9.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.685170 tabmat-3.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.665169 tabmat-3.1.8/.ci_support/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/linux_64_python3.10_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/linux_64_python3.7_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/linux_64_python3.8_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/linux_64_python3.9_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/osx_64_python3.10_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/osx_64_python3.7_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/osx_64_python3.8_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/osx_64_python3.9_default.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/osx_arm64_python3.10.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/osx_arm64_python3.8.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/osx_arm64_python3.9.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/win_64_python3.10.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/win_64_python3.7.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/win_64_python3.8.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 17:05:20.000000 tabmat-3.1.8/.ci_support/win_64_python3.9.____cpython.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 17:05:20.000000 tabmat-3.1.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.665169 tabmat-3.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.661169 tabmat-3.1.8/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.665169 tabmat-3.1.8/.github/actions/conda-build/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/actions/conda-build/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.665169 tabmat-3.1.8/.github/actions/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/actions/linter/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.665169 tabmat-3.1.8/.github/actions/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/actions/unittests/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.669169 tabmat-3.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/base.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/build_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/build_wheels_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/conda-build-linux-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/conda-build-macos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/conda-build-win.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/conda-build.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/daily.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/macos-conda-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/macos.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/pre-commit.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1609 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/tests-macos-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/tests-macos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/tests-win-main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-13 17:05:20.000000 tabmat-3.1.8/.github/workflows/tests-win.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-13 17:05:20.000000 tabmat-3.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 17:05:20.000000 tabmat-3.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 17:05:20.000000 tabmat-3.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-13 17:05:20.000000 tabmat-3.1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-13 17:05:20.000000 tabmat-3.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-13 17:05:20.000000 tabmat-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-13 17:05:37.685170 tabmat-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-13 17:05:20.000000 tabmat-3.1.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-06-13 17:05:20.000000 tabmat-3.1.8/build_and_launch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.669169 tabmat-3.1.8/build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-13 17:05:20.000000 tabmat-3.1.8/build_tools/prepare_macos_wheel.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.669169 tabmat-3.1.8/conda.recipe/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 17:05:20.000000 tabmat-3.1.8/conda.recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.669169 tabmat-3.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.673169 tabmat-3.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   194670 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/_static/dense_bench.png
--rw-r--r--   0 runner    (1001) docker     (123)   243254 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/_static/dense_cat_bench.png
--rw-r--r--   0 runner    (1001) docker     (123)   367152 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/_static/headline.png
--rw-r--r--   0 runner    (1001) docker     (123)   256723 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/_static/one_cat_bench.png
--rw-r--r--   0 runner    (1001) docker     (123)   250426 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/_static/sparse_bench.png
--rw-r--r--   0 runner    (1001) docker     (123)   232045 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/_static/two_cat_bench.png
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/dev
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 17:05:20.000000 tabmat-3.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 17:05:20.000000 tabmat-3.1.8/environment-win.yml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 17:05:20.000000 tabmat-3.1.8/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.673169 tabmat-3.1.8/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28078 2023-06-13 17:05:20.000000 tabmat-3.1.8/images/intermediate_data_sandwich.png
--rw-r--r--   0 runner    (1001) docker     (123)    20274 2023-06-13 17:05:20.000000 tabmat-3.1.8/images/narrow_data_sandwich.png
--rw-r--r--   0 runner    (1001) docker     (123)    31362 2023-06-13 17:05:20.000000 tabmat-3.1.8/images/wide_data_sandwich.png
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-13 17:05:20.000000 tabmat-3.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 17:05:20.000000 tabmat-3.1.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 17:05:37.685170 tabmat-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-13 17:05:20.000000 tabmat-3.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.661169 tabmat-3.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.673169 tabmat-3.1.8/src/tabmat/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.677169 tabmat-3.1.8/src/tabmat/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/benchmark/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.677169 tabmat-3.1.8/src/tabmat/benchmark/data/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/benchmark/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/benchmark/generate_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/benchmark/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/benchmark/memory_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/benchmark/visualize_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19775 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/categorical_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/dense_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.685170 tabmat-3.1.8/src/tabmat/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/alloc.h
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/cat_split_helpers-tmpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)  1531001 2023-06-13 17:05:31.000000 tabmat-3.1.8/src/tabmat/ext/categorical.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/categorical.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1179999 2023-06-13 17:05:32.000000 tabmat-3.1.8/src/tabmat/ext/dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/dense.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/dense_helpers-tmpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)  2609092 2023-06-13 17:05:35.000000 tabmat-3.1.8/src/tabmat/ext/sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/sparse.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/sparse_helpers-tmpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)  1262994 2023-06-13 17:05:37.000000 tabmat-3.1.8/src/tabmat/ext/split.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/ext/split.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/matrix_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/sparse_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/split_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/standardized_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-13 17:05:20.000000 tabmat-3.1.8/src/tabmat/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.673169 tabmat-3.1.8/src/tabmat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-13 17:05:37.000000 tabmat-3.1.8/src/tabmat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-13 17:05:37.000000 tabmat-3.1.8/src/tabmat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:05:37.000000 tabmat-3.1.8/src/tabmat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:05:37.000000 tabmat-3.1.8/src/tabmat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 17:05:37.000000 tabmat-3.1.8/src/tabmat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:05:37.000000 tabmat-3.1.8/src/tabmat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:37.685170 tabmat-3.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/real_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_benchmark_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_categorical_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_fast_sandwich.py
--rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_mkl_sparse_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_real_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_split_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-13 17:05:20.000000 tabmat-3.1.8/tests/test_standardized_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.060297 tabmat-3.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.040296 tabmat-3.1.9/.ci_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/linux_64_python3.10_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/linux_64_python3.7_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/linux_64_python3.8_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/linux_64_python3.9_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/linux_aarch64_python3.10_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/linux_ppc64le_python3.10_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/osx_64_python3.10_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/osx_64_python3.7_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/osx_64_python3.8_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/osx_64_python3.9_default.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/osx_arm64_python3.10.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/osx_arm64_python3.8.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/osx_arm64_python3.9.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/win_64_python3.10.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/win_64_python3.7.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/win_64_python3.8.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 12:00:00.000000 tabmat-3.1.9/.ci_support/win_64_python3.9.____cpython.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 12:00:00.000000 tabmat-3.1.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.040296 tabmat-3.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.036296 tabmat-3.1.9/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.040296 tabmat-3.1.9/.github/actions/conda-build/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/actions/conda-build/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.040296 tabmat-3.1.9/.github/actions/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/actions/linter/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.040296 tabmat-3.1.9/.github/actions/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/actions/unittests/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.044296 tabmat-3.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/base.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/build_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/build_wheels_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/conda-build-linux-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/conda-build-macos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/conda-build-win.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      445 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/conda-build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/daily.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/macos-conda-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/macos.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/pre-commit.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1609 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/tests-macos-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/tests-macos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/tests-win-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-16 12:00:00.000000 tabmat-3.1.9/.github/workflows/tests-win.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 12:00:00.000000 tabmat-3.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-16 12:00:00.000000 tabmat-3.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 12:00:00.000000 tabmat-3.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-16 12:00:00.000000 tabmat-3.1.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-16 12:00:00.000000 tabmat-3.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-16 12:00:00.000000 tabmat-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-16 12:00:19.060297 tabmat-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-16 12:00:00.000000 tabmat-3.1.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-06-16 12:00:00.000000 tabmat-3.1.9/build_and_launch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.044296 tabmat-3.1.9/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-16 12:00:00.000000 tabmat-3.1.9/build_tools/prepare_macos_wheel.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.044296 tabmat-3.1.9/conda.recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-16 12:00:00.000000 tabmat-3.1.9/conda.recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.044296 tabmat-3.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.048297 tabmat-3.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   194670 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/_static/dense_bench.png
+-rw-r--r--   0 runner    (1001) docker     (123)   243254 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/_static/dense_cat_bench.png
+-rw-r--r--   0 runner    (1001) docker     (123)   367152 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/_static/headline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   256723 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/_static/one_cat_bench.png
+-rw-r--r--   0 runner    (1001) docker     (123)   250426 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/_static/sparse_bench.png
+-rw-r--r--   0 runner    (1001) docker     (123)   232045 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/_static/two_cat_bench.png
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/dev
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-16 12:00:00.000000 tabmat-3.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 12:00:00.000000 tabmat-3.1.9/environment-win.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 12:00:00.000000 tabmat-3.1.9/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.048297 tabmat-3.1.9/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28078 2023-06-16 12:00:00.000000 tabmat-3.1.9/images/intermediate_data_sandwich.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20274 2023-06-16 12:00:00.000000 tabmat-3.1.9/images/narrow_data_sandwich.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31362 2023-06-16 12:00:00.000000 tabmat-3.1.9/images/wide_data_sandwich.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-16 12:00:00.000000 tabmat-3.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 12:00:00.000000 tabmat-3.1.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-16 12:00:19.060297 tabmat-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-16 12:00:00.000000 tabmat-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.036296 tabmat-3.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.048297 tabmat-3.1.9/src/tabmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.048297 tabmat-3.1.9/src/tabmat/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/benchmark/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/benchmark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.048297 tabmat-3.1.9/src/tabmat/benchmark/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/benchmark/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/benchmark/generate_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/benchmark/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/benchmark/memory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/benchmark/visualize_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19775 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/categorical_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-16 12:00:00.000000 tabmat-3.1.9/src/tabmat/dense_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.056297 tabmat-3.1.9/src/tabmat/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/cat_split_helpers-tmpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)  1531001 2023-06-16 12:00:12.000000 tabmat-3.1.9/src/tabmat/ext/categorical.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/categorical.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1179999 2023-06-16 12:00:14.000000 tabmat-3.1.9/src/tabmat/ext/dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/dense.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/dense_helpers-tmpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)  2609092 2023-06-16 12:00:17.000000 tabmat-3.1.9/src/tabmat/ext/sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/sparse.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/sparse_helpers-tmpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)  1262994 2023-06-16 12:00:18.000000 tabmat-3.1.9/src/tabmat/ext/split.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/ext/split.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/matrix_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/sparse_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/split_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/standardized_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-16 12:00:01.000000 tabmat-3.1.9/src/tabmat/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.048297 tabmat-3.1.9/src/tabmat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-16 12:00:18.000000 tabmat-3.1.9/src/tabmat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-16 12:00:19.000000 tabmat-3.1.9/src/tabmat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:00:18.000000 tabmat-3.1.9/src/tabmat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:00:18.000000 tabmat-3.1.9/src/tabmat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 12:00:18.000000 tabmat-3.1.9/src/tabmat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 12:00:18.000000 tabmat-3.1.9/src/tabmat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:00:19.060297 tabmat-3.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/real_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_benchmark_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_categorical_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_fast_sandwich.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21161 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_mkl_sparse_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_real_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_split_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-16 12:00:01.000000 tabmat-3.1.9/tests/test_standardized_mat.py
```

### Comparing `tabmat-3.1.8/.flake8` & `tabmat-3.1.9/.flake8`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/actions/unittests/action.yml` & `tabmat-3.1.9/.github/actions/unittests/action.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/build_wheels.yml` & `tabmat-3.1.9/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/build_wheels_release.yml` & `tabmat-3.1.9/.github/workflows/build_wheels_release.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/ci.yml` & `tabmat-3.1.9/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     env:
       CI: True
     strategy:
       fail-fast: true
       matrix:
         CONDA_BUILD_YML:
           - linux_64_python3.7_default.____cpython
+          - linux_aarch64_python3.10_default.____cpython
+          - linux_ppc64le_python3.10_default.____cpython
     steps:
       - name: Pull image
         run: docker pull condaforge/mambaforge:latest
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
```

### Comparing `tabmat-3.1.8/.github/workflows/conda-build-linux-main.yml` & `tabmat-3.1.9/.github/workflows/conda-build-linux-main.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/conda-build-macos.yml` & `tabmat-3.1.9/.github/workflows/conda-build-macos.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/conda-build-win.yml` & `tabmat-3.1.9/.github/workflows/conda-build-win.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/daily.yml` & `tabmat-3.1.9/.github/workflows/daily.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/test.sh` & `tabmat-3.1.9/.github/workflows/test.sh`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/tests-macos-main.yml` & `tabmat-3.1.9/.github/workflows/tests-macos-main.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/tests-macos.yml` & `tabmat-3.1.9/.github/workflows/tests-macos.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/tests-win-main.yml` & `tabmat-3.1.9/.github/workflows/tests-win-main.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.github/workflows/tests-win.yml` & `tabmat-3.1.9/.github/workflows/tests-win.yml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.gitignore` & `tabmat-3.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/.pre-commit-config.yaml` & `tabmat-3.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/CHANGELOG.rst` & `tabmat-3.1.9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,21 @@
    * Update the major if you break the public API
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Changelog
 =========
 
+3.1.9 - 2023-06-16
+-------------------
+
+**Other changes:**
+
+- Support building on architectures that are unsupported by xsimd.
+
 3.1.8 - 2023-06-13
 ------------------
 
 **Other changes:**
 
 - The C++ types have been refactored. Loop indices are now using the ``Py_ssize_t`` type. Integers now have a templated type as well.
 - The documentation for `matvec` and `matvec_transpose` has been updated to reflect actual behavior
```

### Comparing `tabmat-3.1.8/CONTRIBUTING.md` & `tabmat-3.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/LICENSE` & `tabmat-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/PKG-INFO` & `tabmat-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabmat
-Version: 3.1.8
+Version: 3.1.9
 Summary: Efficient matrix representations for working with tabular data.
 Home-page: https://github.com/Quantco/tabmat
 Author: QuantCo, Inc.
 Author-email: noreply@quantco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `tabmat-3.1.8/README.md` & `tabmat-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/conda.recipe/meta.yaml` & `tabmat-3.1.9/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/Makefile` & `tabmat-3.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/_static/dense_bench.png` & `tabmat-3.1.9/docs/_static/dense_bench.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/_static/dense_cat_bench.png` & `tabmat-3.1.9/docs/_static/dense_cat_bench.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/_static/headline.png` & `tabmat-3.1.9/docs/_static/headline.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/_static/one_cat_bench.png` & `tabmat-3.1.9/docs/_static/one_cat_bench.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/_static/sparse_bench.png` & `tabmat-3.1.9/docs/_static/sparse_bench.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/_static/two_cat_bench.png` & `tabmat-3.1.9/docs/_static/two_cat_bench.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/api.rst` & `tabmat-3.1.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/benchmarks.rst` & `tabmat-3.1.9/docs/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/changelog.rst` & `tabmat-3.1.9/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,21 @@
    * Update the major if you break the public API
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Changelog
 =========
 
+3.1.9 - 2023-06-16
+-------------------
+
+**Other changes:**
+
+- Support building on architectures that are unsupported by xsimd.
+
 3.1.8 - 2023-06-13
 ------------------
 
 **Other changes:**
 
 - The C++ types have been refactored. Loop indices are now using the ``Py_ssize_t`` type. Integers now have a templated type as well.
 - The documentation for `matvec` and `matvec_transpose` has been updated to reflect actual behavior
```

### Comparing `tabmat-3.1.8/docs/conf.py` & `tabmat-3.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/docs/make.bat` & `tabmat-3.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/images/intermediate_data_sandwich.png` & `tabmat-3.1.9/images/intermediate_data_sandwich.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/images/narrow_data_sandwich.png` & `tabmat-3.1.9/images/narrow_data_sandwich.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/images/wide_data_sandwich.png` & `tabmat-3.1.9/images/wide_data_sandwich.png`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/pyproject.toml` & `tabmat-3.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/setup.py` & `tabmat-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/benchmark/generate_matrices.py` & `tabmat-3.1.9/src/tabmat/benchmark/generate_matrices.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/benchmark/main.py` & `tabmat-3.1.9/src/tabmat/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/benchmark/memory_tools.py` & `tabmat-3.1.9/src/tabmat/benchmark/memory_tools.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/benchmark/visualize_benchmarks.py` & `tabmat-3.1.9/src/tabmat/benchmark/visualize_benchmarks.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/categorical_matrix.py` & `tabmat-3.1.9/src/tabmat/categorical_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/constructor.py` & `tabmat-3.1.9/src/tabmat/constructor.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/dense_matrix.py` & `tabmat-3.1.9/src/tabmat/dense_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/alloc.h` & `tabmat-3.1.9/src/tabmat/ext/alloc.h`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/cat_split_helpers-tmpl.cpp` & `tabmat-3.1.9/src/tabmat/ext/cat_split_helpers-tmpl.cpp`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/categorical.cpp` & `tabmat-3.1.9/src/tabmat/ext/categorical.cpp`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/categorical.pyx` & `tabmat-3.1.9/src/tabmat/ext/categorical.pyx`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/dense.cpp` & `tabmat-3.1.9/src/tabmat/ext/dense.cpp`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/dense.pyx` & `tabmat-3.1.9/src/tabmat/ext/dense.pyx`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/dense_helpers-tmpl.cpp` & `tabmat-3.1.9/src/tabmat/ext/dense_helpers-tmpl.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 <%def name="middle_j(kparallel, IBLOCK, JBLOCK)">
     int jmaxblock = jmin + ((jmaxinner - jmin) / ${JBLOCK}) * ${JBLOCK};
     for (; j < jmaxblock; j += ${JBLOCK}) {
 
         // setup simd accumulators
         % for ir in range(IBLOCK):
             % for jr in range(JBLOCK):
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+		auto accumsimd${ir}_${jr} = (F)0.0;
+#else
                 auto accumsimd${ir}_${jr} = xs::XSIMD_BROADCAST(((F)0.0));
+#endif
             % endfor
         % endfor
 
         % for ir in range(IBLOCK):
             int basei${ir} = (i - imin2 + ${ir}) * kstep;
         % endfor
         % for jr in range(JBLOCK):
@@ -74,28 +78,40 @@
                     Lptr${ir} += simd_size
                 % else:
                     Lptr${ir} += simd_size,
                 % endif
             % endfor
             ) {
             % for ir in range(IBLOCK):
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+		auto Xtd${ir} = *Lptr${ir};
+#else
                 auto Xtd${ir} = xs::load_aligned(Lptr${ir});
+#endif
                 % for jr in range(JBLOCK):
                 {
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+		    auto Xsimd = *Rptr${jr};
+#else
                     auto Xsimd = xs::load_aligned(Rptr${jr});
+#endif
                     accumsimd${ir}_${jr} = xs::fma(Xtd${ir}, Xsimd, accumsimd${ir}_${jr});
                 }
                 % endfor
             % endfor
         }
 
         // horizontal sum of the simd blocks
         % for ir in range(IBLOCK):
             % for jr in range(JBLOCK):
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+		F accum${ir}_${jr} = accumsimd${ir}_${jr};
+#else
                 F accum${ir}_${jr} = xs::XSIMD_REDUCE_ADD(accumsimd${ir}_${jr});
+#endif
             % endfor
         % endfor
 
         // remainder loop handling the entries that can't be handled in a
         // simd_size stride
         for (int k = kblocksize; k < kmax - kmin; k++) {
             % for ir in range(IBLOCK):
@@ -146,15 +162,19 @@
 template <typename Int, typename F>
 void dense_base${kparallel}(F* R, F* L, F* d, F* out,
                 Py_ssize_t out_m,
                 Py_ssize_t imin2, Py_ssize_t imax2,
                 Py_ssize_t jmin2, Py_ssize_t jmax2, 
                 Py_ssize_t kmin, Py_ssize_t kmax, Int innerblock, Int kstep) 
 {
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+    constexpr std::size_t simd_size = 1;
+#else
     constexpr std::size_t simd_size = xsimd::simd_type<F>::size;
+#endif
     for (Py_ssize_t imin = imin2; imin < imax2; imin+=innerblock) {
         Py_ssize_t imax = imin + innerblock; 
         if (imax > imax2) {
             imax = imax2; 
         }
         for (Py_ssize_t jmin = jmin2; jmin < jmax2; jmin+=innerblock) {
             Py_ssize_t jmax = jmin + innerblock; 
@@ -244,15 +264,19 @@
 
 
 <%def name="dense_sandwich_tmpl(order)">
 template <typename Int, typename F>
 void _dense${order}_sandwich(Int* rows, Int* cols, F* X, F* d, F* out,
         Int in_n, Int out_m, Int m, Int n, Int thresh1d, Int kratio, Int innerblock) 
 {
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+    constexpr std::size_t simd_size = 1;
+#else
     constexpr std::size_t simd_size = xsimd::simd_type<F>::size;
+#endif
     constexpr auto alignment = simd_size * sizeof(F);
 
     bool kparallel = (in_n / (kratio*thresh1d)) > (out_m / thresh1d);
     Py_ssize_t Rsize = thresh1d*thresh1d*kratio*kratio;
     if (kparallel) {
         Rsize *= omp_get_max_threads();
     }
@@ -288,15 +312,19 @@
 
 
 <%def name="dense_rmatvec_tmpl(order)">
 template <typename Int, typename F>
 void _dense${order}_rmatvec(Int* rows, Int* cols, F* X, F* v, F* out,
         Int n_rows, Int n_cols, Int m, Int n) 
 {
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+    constexpr std::size_t simd_size = 1;
+#else
     constexpr std::size_t simd_size = xsimd::simd_type<F>::size;
+#endif
     constexpr std::size_t alignment = simd_size * sizeof(F);
 
     auto outglobal = make_aligned_unique<F>(omp_get_max_threads()*n_cols, alignment);
 
     constexpr int rowblocksize = 256;
     constexpr int colblocksize = 4;
```

### Comparing `tabmat-3.1.8/src/tabmat/ext/sparse.cpp` & `tabmat-3.1.9/src/tabmat/ext/sparse.cpp`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/sparse.pyx` & `tabmat-3.1.9/src/tabmat/ext/sparse.pyx`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/sparse_helpers-tmpl.cpp` & `tabmat-3.1.9/src/tabmat/ext/sparse_helpers-tmpl.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,20 @@
     F* Adata, Int* Aindices, Int* Aindptr,
     F* B, F* d, F* out,
     Int m, Int n, Int r,
     Int* rows, Int* A_cols, Int* B_cols,
     Int nrows, Int nA_cols, Int nB_cols
     ) 
 {
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+    constexpr Int simd_size = 1;
+#else
     constexpr Int simd_size = xsimd::simd_type<F>::size;
+#endif
+
     constexpr auto alignment = simd_size*sizeof(F);
 
     int kblock = 128;
     int jblock = 128;
     auto Rglobal = make_aligned_unique<F>(
         omp_get_max_threads() * kblock * jblock,
         alignment
@@ -91,23 +96,36 @@
                         Int i = Aindices[A_idx];
                         Py_ssize_t Ci = Acol_map[i];
                         if (Ci == -1) {
                             continue;
                         }
 
                         F Q = Adata[A_idx];
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+			auto Qsimd = Q;
+#else
                         auto Qsimd = xs::XSIMD_BROADCAST(Q);
+#endif
 
                         Py_ssize_t Cj = Cjj;
                         Py_ssize_t Cjmax2 = Cjj + ((Cjmax - Cjj) / simd_size) * simd_size;
                         for (; Cj < Cjmax2; Cj+=simd_size) {
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+                            auto Bsimd = R[(Py_ssize_t) (Ck-Ckk) * jblock + (Cj-Cjj)];
+                            auto outsimd = outtemp.get()[Ci * nB_cols_rounded + Cj];
+#else
                             auto Bsimd = xs::load_aligned(&R[(Py_ssize_t) (Ck-Ckk) * jblock + (Cj-Cjj)]);
                             auto outsimd = xs::load_aligned(&outtemp.get()[Ci * nB_cols_rounded + Cj]);
+#endif
                             outsimd = xs::fma(Qsimd, Bsimd, outsimd);
+#ifdef XSIMD_NO_SUPPORTED_ARCHITECTURE
+                            outtemp.get()[Ci * nB_cols_rounded + Cj] = outsimd;
+#else
                             outsimd.store_aligned(&outtemp.get()[Ci * nB_cols_rounded + Cj]);
+#endif
                         }
 
                         for (; Cj < Cjmax; Cj++) {
                             outtemp.get()[Ci * nB_cols_rounded + Cj] += Q * R[(Py_ssize_t) (Ck-Ckk) * jblock + (Cj-Cjj)];
                         }
                     }
                 }
```

### Comparing `tabmat-3.1.8/src/tabmat/ext/split.cpp` & `tabmat-3.1.9/src/tabmat/ext/split.cpp`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/ext/split.pyx` & `tabmat-3.1.9/src/tabmat/ext/split.pyx`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/matrix_base.py` & `tabmat-3.1.9/src/tabmat/matrix_base.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/sparse_matrix.py` & `tabmat-3.1.9/src/tabmat/sparse_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/split_matrix.py` & `tabmat-3.1.9/src/tabmat/split_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/standardized_mat.py` & `tabmat-3.1.9/src/tabmat/standardized_mat.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat/util.py` & `tabmat-3.1.9/src/tabmat/util.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/src/tabmat.egg-info/PKG-INFO` & `tabmat-3.1.9/src/tabmat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabmat
-Version: 3.1.8
+Version: 3.1.9
 Summary: Efficient matrix representations for working with tabular data.
 Home-page: https://github.com/Quantco/tabmat
 Author: QuantCo, Inc.
 Author-email: noreply@quantco.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `tabmat-3.1.8/src/tabmat.egg-info/SOURCES.txt` & `tabmat-3.1.9/src/tabmat.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 pytest.ini
 setup.cfg
 setup.py
 .ci_support/linux_64_python3.10_default.____cpython.yaml
 .ci_support/linux_64_python3.7_default.____cpython.yaml
 .ci_support/linux_64_python3.8_default.____cpython.yaml
 .ci_support/linux_64_python3.9_default.____cpython.yaml
+.ci_support/linux_aarch64_python3.10_default.____cpython.yaml
+.ci_support/linux_ppc64le_python3.10_default.____cpython.yaml
 .ci_support/osx_64_python3.10_default.____cpython.yaml
 .ci_support/osx_64_python3.7_default.____cpython.yaml
 .ci_support/osx_64_python3.8_default.____cpython.yaml
 .ci_support/osx_64_python3.9_default.____cpython.yaml
 .ci_support/osx_arm64_python3.10.____cpython.yaml
 .ci_support/osx_arm64_python3.8.____cpython.yaml
 .ci_support/osx_arm64_python3.9.____cpython.yaml
```

### Comparing `tabmat-3.1.8/tests/real_matrix.pkl` & `tabmat-3.1.9/tests/real_matrix.pkl`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_benchmark_cli.py` & `tabmat-3.1.9/tests/test_benchmark_cli.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_categorical_matrix.py` & `tabmat-3.1.9/tests/test_categorical_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_fast_sandwich.py` & `tabmat-3.1.9/tests/test_fast_sandwich.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_matrices.py` & `tabmat-3.1.9/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_mkl_sparse_matrix.py` & `tabmat-3.1.9/tests/test_mkl_sparse_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_real_matrix.py` & `tabmat-3.1.9/tests/test_real_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_split_matrix.py` & `tabmat-3.1.9/tests/test_split_matrix.py`

 * *Files identical despite different names*

### Comparing `tabmat-3.1.8/tests/test_standardized_mat.py` & `tabmat-3.1.9/tests/test_standardized_mat.py`

 * *Files identical despite different names*

